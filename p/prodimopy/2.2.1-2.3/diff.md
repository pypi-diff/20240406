# Comparing `tmp/prodimopy-2.2.1.tar.gz` & `tmp/prodimopy-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodimopy-2.2.1.tar", last modified: Mon Sep  4 21:04:45 2023, max compression
+gzip compressed data, was "prodimopy-2.3.tar", last modified: Sat Apr  6 12:55:26 2024, max compression
```

## Comparing `prodimopy-2.2.1.tar` & `prodimopy-2.3.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-09-04 21:04:45.168438 prodimopy-2.2.1/
--rw-r--r--   0 work       (501) staff       (20)      790 2023-03-30 07:05:59.000000 prodimopy-2.2.1/DESCRIPTION.md
--rw-r--r--   0 work       (501) staff       (20)     1069 2023-03-30 07:05:59.000000 prodimopy-2.2.1/LICENSE
--rw-r--r--   0 work       (501) staff       (20)       23 2023-04-28 23:48:28.000000 prodimopy-2.2.1/MANIFEST.in
--rw-r--r--   0 work       (501) staff       (20)     1392 2023-09-04 21:04:45.168669 prodimopy-2.2.1/PKG-INFO
--rw-r--r--   0 work       (501) staff       (20)     2945 2023-09-04 20:54:58.000000 prodimopy-2.2.1/README.md
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-09-04 21:04:45.155131 prodimopy-2.2.1/prodimopy/
--rw-r--r--   0 work       (501) staff       (20)        0 2023-03-30 07:05:59.000000 prodimopy-2.2.1/prodimopy/__init__.py
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-09-04 21:04:45.161653 prodimopy-2.2.1/prodimopy/chemistry/
--rw-r--r--   0 work       (501) staff       (20)        0 2023-03-30 07:05:59.000000 prodimopy-2.2.1/prodimopy/chemistry/__init__.py
--rw-r--r--   0 work       (501) staff       (20)    25925 2023-05-27 16:54:54.000000 prodimopy-2.2.1/prodimopy/chemistry/network.py
--rw-r--r--   0 work       (501) staff       (20)    31556 2023-09-04 20:54:58.000000 prodimopy-2.2.1/prodimopy/compare.py
--rw-r--r--   0 work       (501) staff       (20)    18647 2023-03-30 07:05:59.000000 prodimopy-2.2.1/prodimopy/extinction.py
--rw-r--r--   0 work       (501) staff       (20)     8251 2023-03-30 07:05:59.000000 prodimopy-2.2.1/prodimopy/grid.py
--rw-r--r--   0 work       (501) staff       (20)    36560 2023-03-30 07:05:59.000000 prodimopy-2.2.1/prodimopy/hitran.py
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-09-04 21:04:45.165528 prodimopy-2.2.1/prodimopy/interface1D/
--rw-r--r--   0 work       (501) staff       (20)        0 2023-03-30 07:05:59.000000 prodimopy-2.2.1/prodimopy/interface1D/__init__.py
--rw-r--r--   0 work       (501) staff       (20)    19062 2023-03-30 07:05:59.000000 prodimopy-2.2.1/prodimopy/interface1D/infile.py
--rw-r--r--   0 work       (501) staff       (20)     8035 2023-03-30 07:05:59.000000 prodimopy-2.2.1/prodimopy/interface1D/twoppToProDiMo.py
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-09-04 21:04:45.167102 prodimopy-2.2.1/prodimopy/interface2D/
--rw-r--r--   0 work       (501) staff       (20)        0 2023-03-30 07:05:59.000000 prodimopy-2.2.1/prodimopy/interface2D/__init__.py
--rw-r--r--   0 work       (501) staff       (20)    10986 2023-07-13 12:33:52.000000 prodimopy-2.2.1/prodimopy/interface2D/infile.py
--rw-r--r--   0 work       (501) staff       (20)    14741 2023-03-30 07:05:59.000000 prodimopy-2.2.1/prodimopy/movie.py
--rw-r--r--   0 work       (501) staff       (20)    93911 2023-09-04 20:54:58.000000 prodimopy-2.2.1/prodimopy/plot.py
--rw-r--r--   0 work       (501) staff       (20)    31715 2023-04-28 23:48:28.000000 prodimopy-2.2.1/prodimopy/plot_casasim.py
--rw-r--r--   0 work       (501) staff       (20)    11783 2023-03-30 07:05:59.000000 prodimopy-2.2.1/prodimopy/plot_mc.py
--rw-r--r--   0 work       (501) staff       (20)    53940 2023-07-12 19:45:47.000000 prodimopy-2.2.1/prodimopy/plot_models.py
--rw-r--r--   0 work       (501) staff       (20)    22534 2023-04-28 23:48:28.000000 prodimopy-2.2.1/prodimopy/plot_slab.py
--rw-r--r--   0 work       (501) staff       (20)   124738 2023-07-13 12:33:52.000000 prodimopy-2.2.1/prodimopy/read.py
--rw-r--r--   0 work       (501) staff       (20)    20456 2023-03-30 07:05:59.000000 prodimopy-2.2.1/prodimopy/read_casasim.py
--rw-r--r--   0 work       (501) staff       (20)     8556 2023-04-28 23:48:28.000000 prodimopy-2.2.1/prodimopy/read_mc.py
--rw-r--r--   0 work       (501) staff       (20)    89257 2023-07-24 14:30:32.000000 prodimopy-2.2.1/prodimopy/read_slab.py
--rw-r--r--   0 work       (501) staff       (20)    18413 2023-07-24 14:30:32.000000 prodimopy-2.2.1/prodimopy/run_slab.py
--rwxr-xr-x   0 work       (501) staff       (20)     2442 2023-03-30 07:05:59.000000 prodimopy-2.2.1/prodimopy/script_compare.py
--rwxr-xr-x   0 work       (501) staff       (20)     2803 2023-03-30 07:05:59.000000 prodimopy-2.2.1/prodimopy/script_params.py
--rwxr-xr-x   0 work       (501) staff       (20)     6430 2023-04-28 23:48:28.000000 prodimopy-2.2.1/prodimopy/script_plot.py
--rw-r--r--   0 work       (501) staff       (20)     6667 2023-03-30 07:05:59.000000 prodimopy-2.2.1/prodimopy/script_plot_models.py
--rw-r--r--   0 work       (501) staff       (20)     3331 2023-03-30 07:06:00.000000 prodimopy-2.2.1/prodimopy/utils.py
--rw-r--r--   0 work       (501) staff       (20)    22755 2023-03-30 07:06:00.000000 prodimopy-2.2.1/prodimopy/utils_casasim.py
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-09-04 21:04:45.160400 prodimopy-2.2.1/prodimopy.egg-info/
--rw-r--r--   0 work       (501) staff       (20)     1392 2023-09-04 21:04:45.000000 prodimopy-2.2.1/prodimopy.egg-info/PKG-INFO
--rw-r--r--   0 work       (501) staff       (20)     1003 2023-09-04 21:04:45.000000 prodimopy-2.2.1/prodimopy.egg-info/SOURCES.txt
--rw-r--r--   0 work       (501) staff       (20)        1 2023-09-04 21:04:45.000000 prodimopy-2.2.1/prodimopy.egg-info/dependency_links.txt
--rw-r--r--   0 work       (501) staff       (20)      181 2023-09-04 21:04:45.000000 prodimopy-2.2.1/prodimopy.egg-info/entry_points.txt
--rw-r--r--   0 work       (501) staff       (20)       86 2023-09-04 21:04:45.000000 prodimopy-2.2.1/prodimopy.egg-info/requires.txt
--rw-r--r--   0 work       (501) staff       (20)       10 2023-09-04 21:04:45.000000 prodimopy-2.2.1/prodimopy.egg-info/top_level.txt
--rw-r--r--   0 work       (501) staff       (20)       67 2023-09-04 21:04:45.169471 prodimopy-2.2.1/setup.cfg
--rw-r--r--   0 work       (501) staff       (20)     5519 2023-09-04 20:59:01.000000 prodimopy-2.2.1/setup.py
+drwxr-xr-x   0 work       (501) staff       (20)        0 2024-04-06 12:55:26.508586 prodimopy-2.3/
+-rw-r--r--   0 work       (501) staff       (20)      888 2024-04-06 12:39:40.000000 prodimopy-2.3/DESCRIPTION.md
+-rw-r--r--   0 work       (501) staff       (20)     1069 2023-03-30 07:05:59.000000 prodimopy-2.3/LICENSE
+-rw-r--r--   0 work       (501) staff       (20)       23 2023-04-28 23:48:28.000000 prodimopy-2.3/MANIFEST.in
+-rw-r--r--   0 work       (501) staff       (20)     1679 2024-04-06 12:55:26.508309 prodimopy-2.3/PKG-INFO
+-rw-r--r--   0 work       (501) staff       (20)     2945 2023-09-04 20:54:58.000000 prodimopy-2.3/README.md
+drwxr-xr-x   0 work       (501) staff       (20)        0 2024-04-06 12:55:26.496286 prodimopy-2.3/prodimopy/
+-rw-r--r--   0 work       (501) staff       (20)        0 2023-03-30 07:05:59.000000 prodimopy-2.3/prodimopy/__init__.py
+drwxr-xr-x   0 work       (501) staff       (20)        0 2024-04-06 12:55:26.502890 prodimopy-2.3/prodimopy/chemistry/
+-rw-r--r--   0 work       (501) staff       (20)        0 2023-03-30 07:05:59.000000 prodimopy-2.3/prodimopy/chemistry/__init__.py
+-rw-r--r--   0 work       (501) staff       (20)    25925 2023-05-27 16:54:54.000000 prodimopy-2.3/prodimopy/chemistry/network.py
+-rw-r--r--   0 work       (501) staff       (20)    38858 2024-03-03 12:24:55.000000 prodimopy-2.3/prodimopy/compare.py
+-rw-r--r--   0 work       (501) staff       (20)    18648 2024-03-03 12:24:55.000000 prodimopy-2.3/prodimopy/extinction.py
+-rw-r--r--   0 work       (501) staff       (20)     8251 2023-03-30 07:05:59.000000 prodimopy-2.3/prodimopy/grid.py
+-rw-r--r--   0 work       (501) staff       (20)    51740 2024-04-06 12:35:55.000000 prodimopy-2.3/prodimopy/hitran.py
+drwxr-xr-x   0 work       (501) staff       (20)        0 2024-04-06 12:55:26.505053 prodimopy-2.3/prodimopy/interface1D/
+-rw-r--r--   0 work       (501) staff       (20)        0 2023-03-30 07:05:59.000000 prodimopy-2.3/prodimopy/interface1D/__init__.py
+-rw-r--r--   0 work       (501) staff       (20)    19062 2023-03-30 07:05:59.000000 prodimopy-2.3/prodimopy/interface1D/infile.py
+-rw-r--r--   0 work       (501) staff       (20)     8035 2023-03-30 07:05:59.000000 prodimopy-2.3/prodimopy/interface1D/twoppToProDiMo.py
+drwxr-xr-x   0 work       (501) staff       (20)        0 2024-04-06 12:55:26.506106 prodimopy-2.3/prodimopy/interface2D/
+-rw-r--r--   0 work       (501) staff       (20)        0 2023-03-30 07:05:59.000000 prodimopy-2.3/prodimopy/interface2D/__init__.py
+-rw-r--r--   0 work       (501) staff       (20)    12476 2024-04-06 12:35:55.000000 prodimopy-2.3/prodimopy/interface2D/infile.py
+-rw-r--r--   0 work       (501) staff       (20)    14741 2023-03-30 07:05:59.000000 prodimopy-2.3/prodimopy/movie.py
+-rw-r--r--   0 work       (501) staff       (20)   104796 2024-04-06 12:35:55.000000 prodimopy-2.3/prodimopy/plot.py
+-rw-r--r--   0 work       (501) staff       (20)    31715 2023-04-28 23:48:28.000000 prodimopy-2.3/prodimopy/plot_casasim.py
+-rw-r--r--   0 work       (501) staff       (20)    11783 2023-03-30 07:05:59.000000 prodimopy-2.3/prodimopy/plot_mc.py
+-rw-r--r--   0 work       (501) staff       (20)    54332 2024-03-03 12:24:55.000000 prodimopy-2.3/prodimopy/plot_models.py
+-rw-r--r--   0 work       (501) staff       (20)    22534 2023-04-28 23:48:28.000000 prodimopy-2.3/prodimopy/plot_slab.py
+-rw-r--r--   0 work       (501) staff       (20)     6418 2023-11-28 21:57:34.000000 prodimopy-2.3/prodimopy/postprocessing.py
+-rw-r--r--   0 work       (501) staff       (20)   126845 2024-04-06 12:35:55.000000 prodimopy-2.3/prodimopy/read.py
+-rw-r--r--   0 work       (501) staff       (20)    20456 2023-03-30 07:05:59.000000 prodimopy-2.3/prodimopy/read_casasim.py
+-rw-r--r--   0 work       (501) staff       (20)     8566 2023-12-11 23:39:33.000000 prodimopy-2.3/prodimopy/read_mc.py
+-rw-r--r--   0 work       (501) staff       (20)    94687 2024-04-06 12:35:55.000000 prodimopy-2.3/prodimopy/read_slab.py
+-rw-r--r--   0 work       (501) staff       (20)    19843 2023-09-25 15:21:16.000000 prodimopy-2.3/prodimopy/run_slab.py
+-rwxr-xr-x   0 work       (501) staff       (20)     2802 2023-12-02 15:01:37.000000 prodimopy-2.3/prodimopy/script_compare.py
+-rwxr-xr-x   0 work       (501) staff       (20)     2803 2023-03-30 07:05:59.000000 prodimopy-2.3/prodimopy/script_params.py
+-rwxr-xr-x   0 work       (501) staff       (20)     6430 2023-04-28 23:48:28.000000 prodimopy-2.3/prodimopy/script_plot.py
+-rw-r--r--   0 work       (501) staff       (20)     6667 2023-03-30 07:05:59.000000 prodimopy-2.3/prodimopy/script_plot_models.py
+-rw-r--r--   0 work       (501) staff       (20)     3737 2023-11-28 21:57:34.000000 prodimopy-2.3/prodimopy/utils.py
+-rw-r--r--   0 work       (501) staff       (20)    22755 2023-03-30 07:06:00.000000 prodimopy-2.3/prodimopy/utils_casasim.py
+drwxr-xr-x   0 work       (501) staff       (20)        0 2024-04-06 12:55:26.507344 prodimopy-2.3/prodimopy.egg-info/
+-rw-r--r--   0 work       (501) staff       (20)     1679 2024-04-06 12:55:26.000000 prodimopy-2.3/prodimopy.egg-info/PKG-INFO
+-rw-r--r--   0 work       (501) staff       (20)     1031 2024-04-06 12:55:26.000000 prodimopy-2.3/prodimopy.egg-info/SOURCES.txt
+-rw-r--r--   0 work       (501) staff       (20)        1 2024-04-06 12:55:26.000000 prodimopy-2.3/prodimopy.egg-info/dependency_links.txt
+-rw-r--r--   0 work       (501) staff       (20)      181 2024-04-06 12:55:26.000000 prodimopy-2.3/prodimopy.egg-info/entry_points.txt
+-rw-r--r--   0 work       (501) staff       (20)       86 2024-04-06 12:55:26.000000 prodimopy-2.3/prodimopy.egg-info/requires.txt
+-rw-r--r--   0 work       (501) staff       (20)       10 2024-04-06 12:55:26.000000 prodimopy-2.3/prodimopy.egg-info/top_level.txt
+-rw-r--r--   0 work       (501) staff       (20)       67 2024-04-06 12:55:26.509308 prodimopy-2.3/setup.cfg
+-rw-r--r--   0 work       (501) staff       (20)     5517 2024-04-06 12:45:59.000000 prodimopy-2.3/setup.py
```

### Comparing `prodimopy-2.2.1/LICENSE` & `prodimopy-2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prodimopy-2.2.1/README.md` & `prodimopy-2.3/README.md`

 * *Files identical despite different names*

### Comparing `prodimopy-2.2.1/prodimopy/chemistry/network.py` & `prodimopy-2.3/prodimopy/chemistry/network.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.2.1/prodimopy/compare.py` & `prodimopy-2.3/prodimopy/compare.py`

 * *Files 17% similar despite different names*

```diff
@@ -300,15 +300,15 @@
                           "{:40s}".format(str(self.m.abundances[maxa[sortidx[i]]+1,sortidx[i]])),
                           "{:40s}".format(str(self.mref.abundances[maxa[sortidx[i]]+1,sortidx[i]])))
                     lastIdents.append(self.m.species[sortidx[i]])
                     iprint+=1
                   if iprint>5: break
 
             elif val is None and not ok:
-              print("  Value/array is None in only one model.")
+              print("  Value/array is None in only one model or have different shapes.")
             else:
               print("")
 
 
 class Compare(CompareAbs):
   """
   Class for comparing to ProDiMo models of type :class:`~prodimopy.read.Data_ProDiMo`
@@ -349,14 +349,15 @@
     self.tolerances={}
     """ dict :
     A dictionary of tolerances. The naming convention has to follow the naming
     of the compare Function. e.g. If one wants to provide tolerances for
     `compareAbundances` the key names are `Abundances.rtol` and `Abundances.atol`.
 
     FIXME: This is still experimental and not implemented for all compare routines.
+    FIXME: This should be something that is in CompareAbs
 
     """
 
     # the default allowed difference
 
 #     self.d=1.e-3
 #     self.dcdnmol=0.5  # the allowed differences for the column densities (radial and vertical)
@@ -435,32 +436,46 @@
 
     if self.m.lines is not None and self.mref.lines is None: return False,None
 
     if self.m.lines is None and self.mref.lines is not None: return False,None
 
     mFluxes=np.array([x.flux for x in self.m.lines])
     mrefFluxes=np.array([x.flux for x in self.mref.lines])
+
+    # if they have different shapes it will not work: catch this here
+    # FIXME: not nice but should not happen to much, and this way it at least does not crash
+    if mFluxes.shape!=mrefFluxes.shape:
+      return False,None
+
     return self.diffArray(mFluxes,mrefFluxes,**self.getTols(rtol=0.05))
 
   def compareLineEstimates(self):
     '''
     Compares the fluxes from the line estimates
     Currently assumes that both models include the same lines in the same order.
 
-    TODO: can actually be merged with compareLineFluxes
+    .. todo::
+      * it might be worth to make this smarter and compare the individual line estimates.
+        currently the comparison fails if e.g. there are more level for one line ... but the rest is fine
+
     '''
     if self.m.lineEstimates is None and self.mref.lineEstimates is None: return True,None
 
     if self.m.lineEstimates is not None and self.mref.lineEstimates is None: return False,None
 
     if self.m.lineEstimates is None and self.mref.lineEstimates is not None: return False,None
 
     mFluxes=np.array([x.flux for x in self.m.lineEstimates])
     mrefFluxes=np.array([x.flux for x in self.mref.lineEstimates])
 
+    # if they have different shapes it will not work: catch this here
+    # FIXME: not nice but should not happen to much, and this way it at least does not crash
+    if mFluxes.shape!=mrefFluxes.shape:
+      return False,None
+
     mask=np.logical_and(mFluxes<1.e-24,mrefFluxes<1.e-24)
 
     return self.diffArray(mFluxes,mrefFluxes,mask=mask,**self.getTols(rtol=3.e-1,nlimfrac=0.01))
 
   def compareSED(self):
     """
     Compares the SEDs
@@ -778,14 +793,20 @@
 
   def compareFitsFileMie(self):
     '''
     Makes a fits file comparison with Mie.fits.gz
     '''
     return self.diffFitsFile("Mie.fits.gz",rtol=1.e-5)
 
+  def compareFitsFileFLiTs(self):
+    '''
+    Makes a fits file comparison with ProDiMoForFLits.fits
+    '''
+    return self.diffFitsFile("ProDiMoForFLiTs.fits",rtol=1.e-5)
+
   def compareFitsFileLineCubes(self):
     '''
     Makes a fits file comparison with for all line cubes (LINE_3D_*)
     '''
     fcubes=glob.glob(self.m.directory+"/LINE_3D_???.fits")
 
     # FIXME: rtol is pretty high
@@ -866,42 +887,256 @@
     if len(self.m.ratecoefficients)!=len(self.mref.ratecoefficients):
       return False,None,None
 
     mask=np.logical_and(self.m.ratecoefficients<1.e-50,self.mref.ratecoefficients<1.e-50)
     return self.diffArray(self.m.ratecoefficients,self.mref.ratecoefficients,rtol=2.e-7,mask=mask)
 
 
+class CompareSlab(CompareAbs):
+  """
+  Class for comparing two ProDiMo SLAB models of type :class:`~prodimopy.read_slab.slab_data`
+
+  Every compare Function returns true or false, and the relative differences
+  (in case of arrays these are arrays).
+
+  Can be used in e.g. automatic testing routines or in simple command line
+  tools to compare ProDiMo model results.
+  """
+
+  def __init__(self,model,modelref):
+    """
+    Parameters
+    ----------
+    model : :class:`~prodimopy.read_slab.slab_data`
+      The model one wants to compare.
+
+    modelref : :class:`~prodimopy.read_slab.slab_data`
+      The reference model to compare with.
+
+    Attributes
+    ----------
+
+    """
+
+    if model is None or modelref is None:
+      raise TypeError("Either model or modelref is None, no comparison possible.")
+
+    self.m=model
+    """ :class:`~prodimopy.read_slab.slab_data` :
+    The model one wants to compare.
+    """
+    self.mref=modelref
+    """ :class:`~prodimopy.read_slab.slab_data`  :
+    The reference model to compare with.
+    """
+
+  def compareLbLFluxes(self):
+    """
+    Compares the FNLTE and FLTE of the linedata for all the models in line-by-line mode
+    If number of models is not the same return false.
+
+
+    Assumes that both models used the same number of species in the same order.
+    """
+
+    if len(self.mref.models)!=len(self.m.models):
+      return False,None,None
+
+    for m,mref in zip(self.m.models,self.mref.models):
+      arrm=np.array(m.linedata[["FNLTE","FLTE"]])
+      arrmref=np.array(mref.linedata[["FNLTE","FLTE"]])
+
+      eq,da,dbool=self.diffArray(arrm,arrmref,rtol=1.e-4)
+
+      # Current stop at the first error not great
+      if not eq: return eq,da,dbool
+
+    # That means all got
+    return eq,da,dbool
+
+  def compareLbLTau(self):
+    """
+    Compares the FNLTE and FLTE of the linedata for all the models in line-by-line mode
+    If number of models is not the same return false.
+
+
+    Assumes that both models used the same number of species in the same order.
+    """
+
+    if len(self.mref.models)!=len(self.m.models):
+      return False,None,None
+
+    for m,mref in zip(self.m.models,self.mref.models):
+      arrm=np.array(m.linedata[["tauNLTE","tauLTE"]])
+      arrmref=np.array(mref.linedata[["tauNLTE","tauLTE"]])
+
+      eq,da,dbool=self.diffArray(arrm,arrmref,rtol=1.e-4)
+
+      # Current stop at the first error not great
+      if not eq: return eq,da,dbool
+
+    # That means all got
+    return eq,da,dbool
+
+  def compareLbLPop(self):
+    """
+    Compares the LTE and NLTE level populations of the linedata for all the models in line-by-line mode
+    If number of models is not the same return false.
+
+
+    Assumes that both models used the same number of species in the same order.
+    """
+
+    if len(self.mref.models)!=len(self.m.models):
+      return False,None,None
+
+    for m,mref in zip(self.m.models,self.mref.models):
+      arrm=np.array(m.linedata[["pop","ltepop"]])
+      arrmref=np.array(mref.linedata[["pop","ltepop"]])
+
+      eq,da,dbool=self.diffArray(arrm,arrmref,rtol=1.e-4)
+
+      # Current stop at the first error not great
+      if not eq: return eq,da,dbool
+
+    for m,mref in zip(self.m.models,self.mref.models):
+      arrm=np.array(m.leveldata[["pop","ltepop"]])
+      arrmref=np.array(mref.leveldata[["pop","ltepop"]])
+
+      eq,da,dbool=self.diffArray(arrm,arrmref,rtol=1.e-4)
+
+      # Current stop at the first error not great
+      if not eq: return eq,da,dbool
+
+    # That means all got
+    return eq,da,dbool
+
+  # def compareOverlapFluxes(self):
+  #   """
+  #   Compares the FNLTE and FLTE of the linedata for all the models in line overlap mode
+  #   If number of models is not the same return false.
+  #
+  #
+  #   Assumes that both models used the same number of species in the same order.
+  #   """
+  #
+  #   if len(self.mref.models)!=len(self.m.models):
+  #     return False,None,None
+  #
+  #   # for m,mref in zip(self.m.models,self.mref.models):
+  #   #   arrm=np.array(m.overlapLTE)
+  #   #   arrmref=np.array(mref.overlapLTE)
+  #   #   print(arrm)
+  #   #   print(arrmref)
+  #   #
+  #   #   eq,da,dbool=self.diffArray(arrm,arrmref,rtol=1.e-4)
+  #   #
+  #   #   # Current stop at the first error not great
+  #   #   if not eq: return eq,da,dbool
+  #
+  #   for m,mref in zip(self.m.models,self.mref.models):
+  #     arrm=np.array(m.overlapNLTE)
+  #     arrmref=np.array(mref.overlapNLTE)
+  #
+  #     eq,da,dbool=self.diffArray(arrm,arrmref,rtol=1.e-4)
+  #
+  #     # Current stop at the first error not great
+  #     if not eq: return eq,da,dbool
+  #
+  #   # That means all got
+  #   return eq,da,dbool
+
+  # def compareOverlapTau(self):
+  #   """
+  #   Compares the LTE and NLTE optical depths for all the models in line overlap mode
+  #   If number of models is not the same return false.
+  #
+  #
+  #   Assumes that both models used the same number of species in the same order.
+  #   """
+  #
+  #   if len(self.mref.models)!=len(self.m.models):
+  #     return False,None,None
+  #
+  #   for m,mref in zip(self.m.models,self.mref.models):
+  #     arrm=np.array(m.overlapTauLTE)
+  #     arrmref=np.array(mref.overlapTauLTE)
+  #
+  #     eq,da,dbool=self.diffArray(arrm,arrmref,rtol=1.e-4)
+  #
+  #     # Current stop at the first error not great
+  #     if not eq: return eq,da,dbool
+  #
+  #   for m,mref in zip(self.m.models,self.mref.models):
+  #     arrm=np.array(m.overlapTauNLTE)
+  #     arrmref=np.array(mref.overlapTauNLTE)
+  #
+  #     eq,da,dbool=self.diffArray(arrm,arrmref,rtol=1.e-4)
+  #
+  #     # Current stop at the first error not great
+  #     if not eq: return eq,da,dbool
+  #
+  #   # That means all got
+  #   return eq,da,dbool
+
+  # def compareOverlapFreq(self):
+  #   """
+  #   Compares the frequency grid of all the models in line overlap mode
+  #   If number of models is not the same return false.
+  #
+  #
+  #   Assumes that both models used the same number of species in the same order.
+  #   """
+  #
+  #   if len(self.mref.models)!=len(self.m.models):
+  #     return False,None,None
+  #
+  #   for m,mref in zip(self.m.models,self.mref.models):
+  #     arrm=np.array(m.overlapFreq)
+  #     arrmref=np.array(mref.overlapFreq)
+  #
+  #     eq,da,dbool=self.diffArray(arrm,arrmref,rtol=1.e-4)
+  #
+  #     # Current stop at the first error not great
+  #     if not eq: return eq,da,dbool
+  #
+  #   # That means all got
+  #   return eq,da,dbool
+
+
 def eval_model_type(modelDir):
   """
   Try to guess the model type (e.g. mc, full prodimo etc.).
   Default is always prodimo.
 
   Possible types:
 
     `prodimo` .... full prodimo model (:class:`prodimopy.read.Data_ProDiMo`)
 
     `mc` ......... molecular cloud model (:class:`prodimopy.read_mc.Data_mc`)
 
   Returns
   -------
-    str either `prodimo` or `mc`
+    str either `prodimo`, `prodiomTD`, `slab` or `mc`
 
   FIXME: this is maybe not the best place for this routine
   FIXME: provide constants for the values (what's the best way to do this in pyhton?)
   FIXME: this is just a quick hack, it would be better to use the parameters in Parameter.in
 
   """
 
   if os.path.isfile(modelDir+"/ProDiMo_01.out") or \
      os.path.isfile(modelDir+"/ProDiMo_001.out") or \
      os.path.isfile(modelDir+"/ProDiMo_0001.out") or \
      os.path.isfile(modelDir+"/ProDiMo_00001.out"):
     mtype="prodimoTD"
   elif os.path.isfile(modelDir+"/Molecular_Cloud_Input.in"):
     mtype="mc"
+  elif os.path.isfile(modelDir+"/SlabInput.in"):
+    mtype="slab"
   else:
     mtype="prodimo"
 
   return mtype
 
 #   def compareFlineEstimates(self):
 #     '''
```

### Comparing `prodimopy-2.2.1/prodimopy/extinction.py` & `prodimopy-2.3/prodimopy/extinction.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 """Extinction law functions."""
 
 from __future__ import division
 import numpy as np
 #import warnings
 
 def extinction(wave, ebv=None, a_v=None, r_v=3.1, model='f99'):
-    """Return extinction in magnitudes at given wavelength(s).
+    r"""Return extinction in magnitudes at given wavelength(s).
 
     Parameters
     ----------
     wave : float or list_like
         Wavelength(s) in Angstroms at which to evaluate the reddening.
     ebv or a_v : float
         E(B-V) differential extinction, or A(V) total V band extinction,
```

### Comparing `prodimopy-2.2.1/prodimopy/grid.py` & `prodimopy-2.3/prodimopy/grid.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.2.1/prodimopy/interface1D/infile.py` & `prodimopy-2.3/prodimopy/interface1D/infile.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.2.1/prodimopy/interface1D/twoppToProDiMo.py` & `prodimopy-2.3/prodimopy/interface1D/twoppToProDiMo.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.2.1/prodimopy/interface2D/infile.py` & `prodimopy-2.3/prodimopy/interface2D/infile.py`

 * *Files 12% similar despite different names*

```diff
@@ -143,15 +143,19 @@
     if self.g2d is not None:
       pg2d=griddata(points,self.g2d.flatten(),(pmodel.x,pmodel.z),method=imethod)
     else:
       pg2d=None
 
     # assumes grid is from spherical so height cannot be larger then the radius
     # make some cutoff grid from spherical coordinates so height cannot be larger then the radius
+      
+
     cutoff=np.max(self.x)/autocm
+    # if the prodimo grid is smaller then the input grid, then take the cutoff from the prodimo grid
+    cutoff=np.min([pmodel.x[-1,0],cutoff])    
     print("cutoff: ",cutoff)
     # print(pmodel.z)
 
     pnx=len(pmodel.x[:,0])
     pnz=len(pmodel.z[0,:])
 
     # density to check for NaN etc.
@@ -190,15 +194,15 @@
         arr[cnan]=0.0
 
     # special treatment for g2d if it is nan set it to a large number
     if pg2d is not None:
       cnan=np.isnan(pg2d)
       if (cnan.any()):
         print("Found NaNs in g2d set them to 1.e10.")
-        pg2d[cnan]=1.e10
+        pg2d[cnan]=1.e10                 
 
     # TODO: check this again, doesn"t seem to work very good
     if fixmethod==1:
       # FIXME: I think all this is really not very general
       # fix some stuff in the innner region ... because of the spherical grid of MOCASSIN/PLUTO
       # this assumes that the density always increases towards the midplane (should be the case for disks)
       for ix in range(pnx):
@@ -233,15 +237,34 @@
 
             if pvel is not None:
               pvel[ix,iz,0]=pvel[ix+1,iz,0]
               pvel[ix,iz,2]=pvel[ix+1,iz,2]
           # check explicitly for vy
           if (pvel is not None) and pvel[ix,iz,1]<pvel[ix,iz+1,1]:
             pvel[ix,iz,1]=pvel[ix+1,iz,1]
+    elif fixmethod==3: # fixes only the vy ... in the disk should never be zero
+      for iz in range(pnz-2):  # from bottom to top
+        for ix in range(pnx-2,-1,-1):  # outside to inside                  
+          if  pvel is not None and pvel[ix,iz,1]< pvel[ix+1,iz,1] and pvel[ix,iz,1] <=0.0 and (pmodel.z[ix,iz]/pmodel.x[ix,iz])<1.0:
+            
+            # print("Fix (3): ",ix,iz,pmodel.x[ix,iz],pmodel.z[ix,iz],"{:15.5e}".format(pdens[ix,iz]),"{:15.5e}".format(pdens[ix+1,iz]))
+            print("Fix (3): ",ix,iz,pmodel.x[ix,iz],pmodel.z[ix,iz],pvel[ix,iz,1],pvel[ix+1,iz,1])
+            #print("Fix (3): ",ix,iz,pmodel.x[ix,iz],pmodel.z[ix,iz],"{:15.5e}".format(pvel[ix,iz,1]),"{:15.5e}".format(pvel[ix+1,iz,1]))
+
+            pvel[ix,iz,1]=pvel[ix+1,iz,1]            
+            
+            # does not really work, because the density can drop towartds the inner radius
+            # f = interpolate.interp1d(np.log10(pmodel.x[ix+1:,iz]), np.log10(pdens[ix+1:,iz]), fill_value = "extrapolate")  
+            # pdens[ix,iz]=10**f(np.log10(pmodel.x[ix,iz]))
+            #if np.isnan(pdens[ix,iz]): pdens[ix,iz]=pdens[ix+1,iz] 
+            # pdens[ix,iz]=pdens[ix+1,iz]
+            
+            # if pg2d is not None: pg2d[ix,iz]=pg2d[ix+1,iz]
 
+                                                         
     return prhoGas,pnHtot,pvel,pg2d
 
   def toProDiMo(self,pmodel,outdir=".",imethod="linear",fixmethod=1):
     '''
     Interpolates the given density/velocity structure onto the ProDiMo grid and writes
     the intput files for ProDimo.
```

### Comparing `prodimopy-2.2.1/prodimopy/movie.py` & `prodimopy-2.3/prodimopy/movie.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.2.1/prodimopy/plot.py` & `prodimopy-2.3/prodimopy/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -345,57 +345,98 @@
                 bgcolor=None,cb_format="%.1f",scalexy=[1,1],patches=None,
                 rasterized=False,returnFig=False,fig=None,ax=None,movie=False,**kwargs):
     '''
     Plot routine for 2D filled contour plots.
 
     If an `ax` object is passed to this routine, it is use
     use to do the plotting. This is especially useful if you want to use that
-    routine together with subplots (e.g. a grid of plots). see for example
+    routine together with subplots (e.g. a grid of plots). See for example
     :func:`~prodimopy.plot.Plot.plot_abuncont_grid`.
 
-    .. todo::
-      * Option for passing a norm (`:class:matplotlib.colors.LogNorm`).
-        But that does not work nicely fith contourf and colorbars ... works
-        with imshow and pcolormesh though ... maybe switch to pcolormesh.
-
-      * option to pass the name of a color map
-
     Parameters
     ----------
     model : :class:`~prodimopy.read.Data_ProDiMo`
       the model data
 
     values : array_like(float,ndim=2)
       a 2D array with numeric values for the plotting. E.g. any 2D array
       of the :class:`~prodimopy.read.Data_ProDiMo` object.
 
+    label : str
+      The label for the colorbar (color scale). Default: `value`
+      Should be the quqntity and unit of the field that is shown.
+
+    zlog : boolean
+      Using log scaling for the values. Default: True
+
+    grid : boolean
+      Use the grid (ix,iz) as spatial coordinates. Default: False
+
+    zlim : array_like(float,ndim=2)
+      The minimum and maximum values for the color scale. Default: `[None,None]`
+
+    zr : boolean
+      Use z/r as the spatial coordinate for the y-axis. Default: `True`
+
     cmap : str or :class:`matplotlib.colors.Colormap`
       this is simply passed on to the contourf routine of matplotlib
       see :func:`matplotlib.pyplot.contourf` for detail
-
+    
+    clevels : array_like(float,ndim=1)
+      The contour levels to plot. Default: `None`
+      This will also set the labels shown in the colour bar. 
+      If `None` the levels are determined by the `MaxNLocator` routine and will be 6.
+
+    clabels : array_like(str,ndim=1)
+      Overwrite the labels for the colorbar. Default: `None`
+
+    contour : boolean
+      Show contour lines for the `clevels`. Default: `True`
+
+    extend : str
+      The extend of the colorbar. Default: `neither` (see :func:`matplotlib.pyplot.colorbar`)
+    
     oconts : array_like(:class:`~prodimopy.plot.Contour`,ndim=1)
       list of :class:`~prodimopy.plot.Contour` objects which will be drawn
       as additional contour levels. See also the example at the top of the page.
 
+    acont : array_like(float,ndim=2)
+      Should not be used anymore. Default: `None`
+      Use `oconts` instead.
+
+    acontl : array_like(float,ndim=1)
+      Should not be used anymore. Default: `None`
+
+    nbins : int
+      The number of bins for the color scale. Default: 70
+
+    bgcolor : str
+      The background color of the plot. Default: `None`
+      Can be useful to set the background color in the plot to `black` for example.
+
+    cb_format : str
+      The format string for the colorbar labels. Default: `%.1f`
+
+    scalexy : array_like(float,ndim=1)
+      A scaling factor (multiplicative) for the x and y coordinates. Default: `[1,1]`
+      W.g. plot in 1000 of au instead of au. 
+
     ax : :class:`matplotlib.axes.Axes`
       a matplotlib axis object which will be used for plotting
 
-    scalexy: apply a scaling factor for the x and y coordinate (multiplicative)
-
-    patches: a list of matplotlib.patches objects. For each object in the list
-      simply ax.add_patch() is called (at the very end of the routine)
+    patches : array_like(:class:`matplotlib.patches.Patch`,ndim=1)        
+      a list of patches objects. For each object in the list, simply ax.add_patch() is called (at the very end of the routine)
 
     movie : boolean
       Special mode for movies ...
 
-
+      
     .. todo::
 
-      * allow to use grid (ix,iz) as spatial coordinates.
-      * update documenation for parameters
+       * Option for passing a norm (`:class:matplotlib.colors.LogNorm`). But that does not work nicely with contourf and colorbars ... works with imshow and pcolormesh though ... maybe switch to pcolormesh.
 
     '''
     if not ("nolog" in kwargs):
       print("PLOT: plot_cont ...")
 
     # prepare the data values
     if zlog is True:
@@ -516,15 +557,19 @@
 
     if oconts is not None:
       for cont in oconts:
         if grid:
           ACS=ax.contour(cont.field.T,levels=cont.levels,extent=(-0.5,model.nx-0.5,0.0,model.nz-1.0),
                          colors=cont.colors,linestyles=cont.linestyles,linewidths=cont.linewidths)
         else:
-          ACS=ax.contour(x,y,cont.field,levels=cont.levels,
+          if cont.filled is True:
+            ACS=ax.contourf(x,y,cont.field,levels=cont.levels,
+                         colors=cont.colors,linestyles=cont.linestyles,linewidths=cont.linewidths)
+          else:
+            ACS=ax.contour(x,y,cont.field,levels=cont.levels,
                          colors=cont.colors,linestyles=cont.linestyles,linewidths=cont.linewidths)
         if cont.showlabels:
           ax.clabel(ACS,inline=True,inline_spacing=cont.label_inline_spacing,
                     fmt=cont.label_fmt,manual=cont.label_locations,fontsize=cont.label_fontsize)
 
     if acont is not None:
       print("WARN: plot_cont: please use the oconts for additional contours ...")
@@ -560,14 +605,503 @@
     if movie: return fig,CS
 
     if returnFig:
       return fig
     else:
       return self._closefig(fig)
 
+  def streamplot_overlay(self,model,axes,resolution=0.1,streamprops={}):
+    '''
+    Creates a streamplot using the plt.streamplot routine from for the vx and vz velocity components of the model. 
+    Is plotted on top of the passed axes object (e.g. from a contour plot).
+    Please note for a "normal" ProDiMo model the vx and vz components are zero and so nothing will be plotted. 
+    
+    Parameters
+    ----------
+
+    model : :class:`~prodimopy.read.Data_ProDiMo`
+      The ProDiMo model data.
+
+    axes : :class:`matplotlib.axes.Axes`
+      The axes object on which the streamplot should be plotted.
+
+    resolution : float
+      The resolution of the regular grid on which the velocity components are interpolated. Unit: au.
+      Default: 0.1
+
+    streamprops : dict
+      A dictionary with properties for the streamplot. This is passed on to the streamplot routine of matplotlib.
+      Default: {}
+    
+    '''
+    from scipy.interpolate import griddata
+    
+    print(model)
+    print("Axes",axes)
+
+    defstreamprops={"color" : 'k',"density" : 3,"linewidth" : 0.4,"arrowsize": 0.5}
+    
+    
+    defstreamprops["maxlength"]=np.max(axes.get_ylim())/3
+    
+    for key in streamprops.keys():
+      defstreamprops[key]=streamprops[key]
+    
+    
+    rmin=model.x[0,0]
+    rmax=model.x[-1,0]
+    zmax=model.z[-1,-1]
+    rmax=np.min([rmax,zmax]) # always square at the moment
+
+
+    [xC,zC]=np.meshgrid(np.arange(rmin,rmax,resolution),np.arange(0,rmax,resolution),indexing='ij')
+
+    points=np.array([model.x.flatten(),model.z.flatten()]).T  
+    vxC=griddata(points,model.velocity[:,:,0].flatten(),(xC,zC),method="linear")
+    vzC=griddata(points,model.velocity[:,:,2].flatten(),(xC,zC),method="linear")
+            
+    axes.streamplot(xC[:,0],zC[0,:],vxC.T,vzC.T,**defstreamprops)
+
+  def plot_abuncont(self,model,species='O',rel2H=True,label=None,zlog=True,
+                zlim=[None,None],zr=True,cmap=None,clevels=None,clabels=None,contour=True,
+                extend="neither",oconts=None,acont=None,acontl=None,nbins=70,
+                bgcolor=None,cb_format="%.1f",scalexy=[1,1],patches=None,
+                rasterized=False,ax=None,movie=False,**kwargs):
+    '''
+    Plots the 2D abundance structure of a species.
+
+    This is a convenience function and is simply a wrapper for
+    :func:`~prodimopy.plot.Plot.plot_cont` routine.
+
+    The routine checks if the species exists, calculates the abundance and sets some
+    defaults (e.g. label) for the :func:`~prodimopy.plot.Plot.plot_cont` routine and calls it.
+    However, all the defaults can be overwritten by providing the corresponding parameter.
+
+    Contributors: L. Klarmann, Ch. Rab
+
+    .. todo::
+
+      can be improved with better and smarter default values (e.g. for the colorbar)
+
+
+    Parameters
+    ----------
+
+    model : :class:`prodimopy.read.Data_ProDiMo`
+      the model data
+
+    species : str
+      the name of the species as given in |prodimo|
+
+    rel2H : boolean
+      plot abundances relative to the total H nuclei number density.
+      If `False` the number density of the species is plotted
+
+    label : str
+      the label for the colorbar. If None the default is plotted
+
+
+    For all other parameters see :func:`~prodimopy.plot.Plot.plot_cont`
+
+    '''
+    print('PLOT: plot_abuncont ...')
+
+    values,labelN,zlogN,zlimN,extendN=self._prepareAbunForPlot(model,species,label,rel2H,zlog,zlim,extend)
+
+    return self.plot_cont(model,values,label=labelN,zlog=zlogN,
+                zlim=zlimN,zr=zr,cmap=cmap,clevels=clevels,clabels=clabels,contour=contour,
+                extend=extendN,oconts=oconts,acont=acont,acontl=acontl,nbins=nbins,
+                bgcolor=bgcolor,cb_format=cb_format,scalexy=scalexy,patches=patches,
+                rasterized=rasterized,nolog=True,ax=ax,movie=movie,**kwargs)
+
+  def plot_abuncont_grid(self,model,speciesList=['e-','H2','CO',"H2O"],nrows=2,ncols=2,rel2H=True,label=None,zlog=True,
+                zlim=[None,None],zr=True,cmap=None,clevels=None,clabels=None,contour=True,
+                extend="neither",oconts=None,acont=None,acontl=None,nbins=70,
+                bgcolor=None,cb_format="%.1f",scalexy=[1,1],patches=None,
+                rasterized=False,**kwargs):
+    '''
+    Convenience routine to plot a grid of abundance plots in the same way as
+    :func:`~prodimopy.plot.Plot.plot_abuncont`.
+
+    The number of plots is given by `nrows` times `ncols` and should be equal to
+    the number of species in `speciesList`
+
+    Parameters
+    ----------
+
+    model : :class:`~prodimopy.read.Data_ProDiMo`
+      the model data
+
+    speciesList : array_like(str,ndim=1) :
+      a list of species names that should be plotted. The plots will be made
+      in order of that list, starting from top left to the bottom right of the grid.
+
+    nrows : int
+      how many rows should the subplots grid have.
+
+    ncols : in
+      how many columns should teh subplots grid have.
+
+    zlim : array_like
+      can either be of the form [zmin,zmax] ore a list of such entries ([zmin1,zmax1],[zmin1,zmax1], ....).
+      For the latter the number of entries must be equal to the number of species.
+
+
+    For the other parameters see :func:`~prodimopy.plot.Plot.plot_abuncont`
+
+    '''
+
+    print("PLOT: plot_abuncont_grid ...")
+
+    fig,axes=plt.subplots(nrows,ncols,figsize=scale_figs([ncols,nrows]))
+
+    if zlim==None:
+      zlims=[(None,None)]*len(speciesList)
+    elif len(np.shape(zlim))==1:
+      print(zlim)
+      zlims=[zlim]*len(speciesList)
+    else:
+      zlims=zlim
+
+    iax=0
+    for species,zliml in zip(speciesList,zlims):
+      if species not in model.spnames:
+        print("ERROR: Species "+species+" dose not exist in model.")
+        iax=iax+1
+        continue
+
+      values,labelG,zlogG,zlimG,extendG=self._prepareAbunForPlot(model,species,label,rel2H,zlog,zliml,extend)
+
+      self.plot_cont(model,values,label=labelG,zlog=zlogG,
+                zlim=zlimG,zr=zr,cmap=cmap,clevels=clevels,clabels=clabels,contour=contour,
+                extend=extendG,oconts=oconts,acont=acont,acontl=acontl,nbins=nbins,
+                bgcolor=bgcolor,cb_format=cb_format,scalexy=scalexy,patches=patches,
+                rasterized=rasterized,fig=fig,ax=axes.flatten()[iax],nolog=True,**kwargs)
+
+      iax=iax+1
+
+    fig.tight_layout()
+
+    return self._closefig(fig)
+
+  def plot_reaccont(self,model,chemana,rtype,level=1,showAbun=False,values=None,
+                    label=None,cmap=None,zlog=True,zlim=[None,None],
+                    clevels=None,clabels=None,contour=True,
+                    extend="neither",oconts=None,nbins=70,
+                    bgcolor=None,cb_format="%.1f",patches=None,
+                    rasterized=True,ax=None,**kwargs):
+    '''
+    Make a contour plot with the reactions numbers from chemanalyse on top.
+    As spatial coordinates the indices of the spatial grid are used.
+
+    This is a convenience function and is simply a wrapper for
+    :func:`~prodimopy.plot.Plot.plot_cont` routine.
+
+    The same can be achieved by simply using plot_cont and plot the numbers
+    on top (see last part of this routine). Then one has more flexibility.
+
+    Parameters
+    ----------
+
+    model : :class:`prodimopy.read.Data_ProDiMo`
+      the model data
+
+    chemana : class:`prodimopy.read.Chemistry`
+      data resulting from `prodimopy.read.analise_chemistry` on a single species
+
+    rtype : str
+      keyword which sets the type of reactions to be shown (destruction or formation)
+      must be set to either 'd' (destruction) or 'f' (formation)
+
+    level : int
+      1 means most important, 2 second most important etc.
+
+    showAbun : boolean
+      Show the abundances of the species that is analysed as filled contours.
+
+    values : array_like(float,ndim=2)
+      a 2D array with numeric values for the plotting like in :func:`~prodimopy.plot.Plot.plot_cont`.
+      Howver, it an also be `None` (default) in that case the total formation/destruction rate is plotted.
+
+
+    sfigs : array_like(float,ndim=2)
+      Is part of kwargs. But this one is relevant here as one might needs to make
+      the figure larger to see the reactoins numbers. e.g. just pass `sfigs=[2.,2.]`
+    '''
+
+    if showAbun:
+      values=model.getAbun(chemana.species)
+      label=r"$\epsilon("+spnToLatex(chemana.species)+"$)"
+      if zlog: label="log "+label
+
+    if rtype is None or rtype!="d": rtype="f"
+
+    reacs=chemana.get_reac_grid(level,rtype)
+
+    rlabel="form."
+    if rtype=="d": rlabel="dest."
+
+    if values is None:
+      if rtype=="d":
+        values=chemana.totdrate
+      else:
+        values=chemana.totdrate
+
+      label=r"(total "+rlabel+" rate) $[cm^{-3} s^{-1}]$"
+      if zlog: label="log "+label
+
+    if not "title" in kwargs:
+      if level==1:
+        tit="main "+rlabel+" reactions"
+      else:
+        tit=str(level).strip()+r"$^{nd}$ "+rlabel+" reactions"
+
+      kwargs["title"]=tit
+
+    fig=self.plot_cont(model,values,label=label,zlog=zlog,grid=True,
+            zlim=zlim,zr=False,cmap=cmap,clevels=clevels,clabels=clabels,contour=contour,
+            extend=extend,oconts=oconts,acont=None,acontl=None,nbins=nbins,
+            bgcolor=bgcolor,cb_format=cb_format,scalexy=[1.0,1.0],patches=patches,
+            rasterized=rasterized,nolog=True,ax=ax,movie=False,returnFig=True,**kwargs)
+
+    # this is potentially very slow
+    xstart=0
+    xend=model.nx
+    ystart=0
+    yend=model.nz-1
+    if "xlim" in kwargs:
+      if kwargs["xlim"][0] is not None:
+        xstart=kwargs["xlim"][0]
+
+      if kwargs["xlim"][1] is not None:
+        xend=kwargs["xlim"][1]
+
+    if "ylim" in kwargs:
+      if kwargs["ylim"][0] is not None:
+        ystart=kwargs["ylim"][0]
+
+      if kwargs["ylim"][1] is not None:
+        yend=kwargs["ylim"][1]
+
+    for i in range(xstart,xend,1):
+      for j in range(ystart,yend,1):
+        fig.axes[0].text(i,j,reacs[0][i,j],fontsize=3.0,horizontalalignment="center",verticalalignment="bottom",color="white")
+
+    return fig
+
+  def plot_line_origin(self,model,lineIdents,field,label="value",boxcolors=None,showBox=True,showRadialLines=True,showztauD1=True,boxlinewidths=1.5,
+                       boxlinestyles=None,boxhatches=None,lineLabels=None,showLineLabels=True,lineLabelsFontsize=6.0,lineLabelsAlign="left",
+                       showContOrigin=False,
+                       zlog=True,zlim=[None,None],zr=True,clevels=None,clabels=None,contour=False,extend="neither",oconts=None,nbins=70,
+                       bgcolor=None,cb_format="%.1f",scalexy=[1,1],patches=None,rasterized=False,ax=None,**kwargs):
+    '''
+    Plots the line origins for a list of lineestimates given by their lineIdents
+    (["ident",wavelength]).
+
+    Does not give the exact same results as the corresponding idl routines
+    as we do not use interpolation here. We rather use the same method for
+    calculating the averaged values over the emission area and for plotting
+    this area.
+
+    Note most other parameters, especially for plotting styles (line widths), are also 
+    arrays/lists. Those lists should have the same lenght as the lineIdents list.
+
+    The routine uses :func:`plot_cont` for plotting, hence a number of parameters have the same meaning as in plot_cont. 
+    They are just passed through to plot_cont).
+
+    Parameters
+    ----------
+    model : :class:`~prodimopy.read.Data_ProDiMo`
+      the model data
+
+    lineIdents : array_like()
+      list of line identifactor of the form `[["ident",wl],["ident2",wl2]]`.
+
+    field : array_like(float,ndim=2)
+      a 2D array with numeric values for the plotting. E.g. any 2D array
+      of the :class:`~prodimopy.read.Data_ProDiMo` object.
+
+    boxcolors : array_like
+      list of colors for the boxes for each line one wants to plot (should have the same number of entries as lineIdents). 
+      If not given the default colors are used.
+
+    showBox : boolean
+      if `True` (default) the box for the emitting region for each line is shown.
+
+    showRadialLines : boolean
+      if `True` (default) than two dotted lines are shown for the z15 and z85 values at each radius.
+      This is the main line emitting layer at each radius. 
+
+    showztauD1 : boolean
+      show the z_level where taudust_ver=1 for each line. For detail of this quantity see
+      :class:`~prodimopy.read.DataLineEstimateRInfo`
+
+    boxlinewidths : array_like
+      the widths of the line for each box showing the line origin. Can be a
+      scalar, in that case all boxes have the same linewidth.
+
+    boxlinestyles : array_like
+      the line styles for the boxes (line emitting regions). Can be a scalar, in that case all boxes have the same linestyle.
+
+    boxhatches : array_like
+      use hatching for the vertical line emitting regions. Only used if `showRadialLines` is `True`.
+      Hatches are the ones from matplotlib (e.g. ["//"])
+
+    lineLabels : array_like
+      list of labels for the lines. If not given the labels are generated from the lineIdents.      
+
+    showLineLabels : boolean
+      show the labels for the lines. Default: `True`.
+
+    lineLabelsFontsize : float
+      fontsize for the line labels. Default: `6.0`.
+
+    lineLabelsAlign : str
+      alignment of the line labels. Default: `left`. Other options is `right`.
+
+    showContOrigin : boolean
+      Also show the box for the continuum emitting regions (at the wavelength of the line). Default: `False`.
+              
+    '''
+    if boxcolors is None:
+      boxcolors=[self.pcolors["red"],self.pcolors["orange"],self.pcolors["brown"],
+                 self.pcolors["purple"],self.pcolors["gray"]]
+
+    if boxlinestyles is None:
+      boxlinestyles=["-"]*10
+    elif np.isscalar(boxlinestyles):
+      boxlinestyles=[boxlinestyles]*10
+
+    if np.isscalar(boxlinewidths):
+      boxlinewidths=[boxlinewidths]*10
+
+    # if it is only one line (no list of list) make it a list
+    if (type(lineIdents[0])==str): lineIdents=[lineIdents]
+
+    lestimates=list()
+    for id in lineIdents:
+      lestimates.append(model.getLineEstimate(id[0],id[1]))
+
+    if patches is None:
+      patches=list()
+
+    if len(boxcolors)<len(lestimates) or len(boxlinestyles)<len(lestimates):
+      print("Not enough boxcolors or boxlinestyles available! ")
+      return
+
+    ibox=0
+    for lesti in lestimates:
+      # to be consistent we use the LineOriginMask to determine the box
+      # as a result the plotted region is not necessarely the same as in idl
+      # as we do not interpolate here
+      xmasked=np.ma.masked_array(model.x,mask=model.getLineOriginMask(lesti))
+      x15=np.min(xmasked)
+      x85=np.max(xmasked)
+      xi15=np.argmin(np.abs(model.x[:,0]-x15))
+      xi85=np.argmin(np.abs(model.x[:,0]-x85))
+
+      z85s=[[model.x[rp.ix,0],rp.z85] for rp in lesti.rInfo[xi15:xi85+1]]
+      z15s=[[model.x[rp.ix,0],rp.z15] for rp in lesti.rInfo[xi85:xi15-1:-1]]
+      points=z85s+z15s
+
+      if zr is True:
+        for point in points:
+          point[1]=point[1]/point[0]
+
+      if showBox:
+        if len(points)>1:
+          patch=mpl.patches.Polygon(points,closed=True,fill=False,color=boxcolors[ibox],
+                                      linestyle=boxlinestyles[ibox],
+                                      zorder=100,linewidth=boxlinewidths[ibox])
+
+          patches.append(patch)
+        else:
+          print("WARN: Unable to calculate a proper region for the line origin: "+str(lesti))
+
+      if showContOrigin is True:
+        if (model.sed is not None and model.sed.sedAna is not None):
+          pointsc=self._getSEDana_boxpoints(lesti.wl,model,zr)
+          if len(pointsc)>1:
+            patchc=mpl.patches.Polygon(pointsc,closed=True,fill=False,
+                                         color=boxcolors[ibox],zorder=100,
+                                         linewidth=1.0,linestyle="--")
+            patches.append(patchc)
+          else:
+            print("WARN: Unable to calculate a proper region for the continuum origin: "+str(lesti))
+
+      ibox+=1
+
+    fig=self.plot_cont(model,field,label=label,zlog=zlog,
+                zlim=zlim,zr=zr,clevels=clevels,clabels=clabels,contour=False,
+                extend=extend,oconts=oconts,acont=None,acontl=None,nbins=nbins,
+                bgcolor=bgcolor,cb_format=cb_format,scalexy=scalexy,patches=patches,
+                rasterized=rasterized,returnFig=True,ax=ax,**kwargs)
+
+    if ax is None:
+      ax=fig.axes[0]
+
+    # show the full emitting layer as function of radius
+    # maybe this slows down the pl
+    if showRadialLines or showztauD1:
+      iest=0
+      r=model.x[:,0]
+      for lesti in lestimates:
+        z15=[rinf.z15 for rinf in lesti.rInfo]
+        z85=[rinf.z85 for rinf in lesti.rInfo]
+        if zr is True:
+          z15=z15/r
+          z85=z85/r
+
+        if showBox is False:
+          lsrad=boxlinestyles[iest]
+        else:
+          lsrad=":"
+
+        if showRadialLines:
+          ax.plot(r,z15,color=boxcolors[iest],linestyle=lsrad,linewidth=1.0)
+          ax.plot(r,z85,color=boxcolors[iest],linestyle=lsrad,linewidth=1.0)
+          if boxhatches is not None:
+            ax.fill_between(r,z15,z85,edgecolor=boxcolors[iest],hatch=boxhatches[iest],facecolor="none",linewidth=0.0)
+
+        # can be None just check the first entry
+        if showztauD1 and lesti.rInfo[0].ztauD1 is not None:
+          ztauD1=[rinf.ztauD1 for rinf in lesti.rInfo]
+          if zr: ztauD1=ztauD1/r
+
+          ax.plot(r,ztauD1,color=boxcolors[iest],linestyle="--",linewidth=1.0)
+
+        iest+=1
+
+    if showLineLabels:
+      ibox=0
+      for idline,lesti in zip(lineIdents,lestimates):
+        if lineLabels is not None:
+          label=lineLabels[ibox]
+        else:
+          label="$"+spnToLatex(idline[0])+"$ "+("{:10.2f}".format(lesti.wl)).strip()+r" $\mu$m"
+
+        # FIXME: quick and dirty, ref fontsize =6.0
+        vpos=ibox/(18.0-(lineLabelsFontsize/6.0-1.0)*12)
+        if lineLabelsAlign=="right":
+          ax.text(0.95,0.97-vpos,label,
+                horizontalalignment='right',
+                verticalalignment='top',fontsize=lineLabelsFontsize,
+                transform=ax.transAxes,color=boxcolors[ibox],
+                bbox=dict(boxstyle='square,pad=0.1',fc='white',ec='none'))
+        else:
+          ax.text(0.02,0.97-vpos,label,
+                horizontalalignment='left',
+                verticalalignment='top',fontsize=lineLabelsFontsize,
+                transform=ax.transAxes,color=boxcolors[ibox],
+                bbox=dict(boxstyle='square,pad=0.1',fc='white',ec='none'))
+        ibox+=1
+
+    return self._closefig(fig)
+
+
   def plot_ionrates_midplane(self,model,ax=None,**kwargs):
 
     print("PLOT: plot_ionrates_midplane ...")
 
     cX=self.pcolors["red"]
     cSP=self.pcolors["blue"]
     cCR=self.pcolors["gray"]
@@ -728,16 +1262,16 @@
       y=values
     else:
       x=np.sqrt(model.x[:,zidx]**2.0+model.z[:,zidx]**2.0)
       y=values[:,zidx]
 
     ax.plot(x,y,marker=None,color=color)
 
-    ax.set_xlim(np.min(x),np.max(x))
-    ax.set_ylim(np.min(y),np.max(y))
+    ax.set_xlim(np.nanmin(x),np.nanmax(x))
+    ax.set_ylim(np.nanmin(y),np.nanmax(y))
     ax.semilogy()
 
     ax.set_xlabel(r"r [au]")
     ax.set_ylabel(ylabel)
 
     self._dokwargs(ax,**kwargs)
     # self._legend(ax)
@@ -912,240 +1446,14 @@
       values=model.nmol[:,:,n_rel_index]
       if label is None:
         label=r"$\mathrm{n("+spnToLatex(species)+") [cm^{-3}]}$"
         if zlog: label="log "+label
 
     return values,label,zlog,zlim,extend
 
-  def plot_abuncont(self,model,species='O',rel2H=True,label=None,zlog=True,
-                zlim=[None,None],zr=True,cmap=None,clevels=None,clabels=None,contour=True,
-                extend="neither",oconts=None,acont=None,acontl=None,nbins=70,
-                bgcolor=None,cb_format="%.1f",scalexy=[1,1],patches=None,
-                rasterized=False,ax=None,movie=False,**kwargs):
-    '''
-    Plots the 2D abundance structure of a species.
-
-    This is a convenience function and is simply a wrapper for
-    :func:`~prodimopy.plot.Plot.plot_cont` routine.
-
-    The routine checks if the species exists, calculates the abundance and sets some
-    defaults (e.g. label) for the :func:`~prodimopy.plot.Plot.plot_cont` routine and calls it.
-    However, all the defaults can be overwritten by providing the corresponding parameter.
-
-    Contributors: L. Klarmann, Ch. Rab
-
-    .. todo::
-
-      can be improved with better and smarter default values (e.g. for the colorbar)
-
-
-    Parameters
-    ----------
-
-    model : :class:`prodimopy.read.Data_ProDiMo`
-      the model data
-
-    species : str
-      the name of the species as given in |prodimo|
-
-    rel2H : boolean
-      plot abundances relative to the total H nuclei number density.
-      If `False` the number density of the species is plotted
-
-    label : str
-      the label for the colorbar. If None the default is plotted
-
-
-    For all other parameters see :func:`~prodimopy.plot.Plot.plot_cont`
-
-    '''
-    print('PLOT: plot_abuncont ...')
-
-    values,labelN,zlogN,zlimN,extendN=self._prepareAbunForPlot(model,species,label,rel2H,zlog,zlim,extend)
-
-    return self.plot_cont(model,values,label=labelN,zlog=zlogN,
-                zlim=zlimN,zr=zr,cmap=cmap,clevels=clevels,clabels=clabels,contour=contour,
-                extend=extendN,oconts=oconts,acont=acont,acontl=acontl,nbins=nbins,
-                bgcolor=bgcolor,cb_format=cb_format,scalexy=scalexy,patches=patches,
-                rasterized=rasterized,nolog=True,ax=ax,movie=movie,**kwargs)
-
-  def plot_abuncont_grid(self,model,speciesList=['e-','H2','CO',"H2O"],nrows=2,ncols=2,rel2H=True,label=None,zlog=True,
-                zlim=[None,None],zr=True,cmap=None,clevels=None,clabels=None,contour=True,
-                extend="neither",oconts=None,acont=None,acontl=None,nbins=70,
-                bgcolor=None,cb_format="%.1f",scalexy=[1,1],patches=None,
-                rasterized=False,**kwargs):
-    '''
-    Convenience routine to plot a grid of abundance plots in the same way as
-    :func:`~prodimopy.plot.Plot.plot_abuncont`.
-
-    The number of plots is given by `nrows` times `ncols` and should be equal to
-    the number of species in `speciesList`
-
-    Parameters
-    ----------
-
-    model : :class:`~prodimopy.read.Data_ProDiMo`
-      the model data
-
-    speciesList : array_like(str,ndim=1) :
-      a list of species names that should be plotted. The plots will be made
-      in order of that list, starting from top left to the bottom right of the grid.
-
-    nrows : int
-      how many rows should the subplots grid have.
-
-    ncols : in
-      how many columns should teh subplots grid have.
-
-    zlim : array_like
-      can either be of the form [zmin,zmax] ore a list of such entries ([zmin1,zmax1],[zmin1,zmax1], ....).
-      For the latter the number of entries must be equal to the number of species.
-
-
-    For the other parameters see :func:`~prodimopy.plot.Plot.plot_abuncont`
-
-    '''
-
-    print("PLOT: plot_abuncont_grid ...")
-
-    fig,axes=plt.subplots(nrows,ncols,figsize=scale_figs([ncols,nrows]))
-
-    if zlim==None:
-      zlims=[(None,None)]*len(speciesList)
-    elif len(np.shape(zlim))==1:
-      print(zlim)
-      zlims=[zlim]*len(speciesList)
-    else:
-      zlims=zlim
-
-    iax=0
-    for species,zliml in zip(speciesList,zlims):
-      if species not in model.spnames:
-        print("ERROR: Species "+species+" dose not exist in model.")
-        iax=iax+1
-        continue
-
-      values,labelG,zlogG,zlimG,extendG=self._prepareAbunForPlot(model,species,label,rel2H,zlog,zliml,extend)
-
-      self.plot_cont(model,values,label=labelG,zlog=zlogG,
-                zlim=zlimG,zr=zr,cmap=cmap,clevels=clevels,clabels=clabels,contour=contour,
-                extend=extendG,oconts=oconts,acont=acont,acontl=acontl,nbins=nbins,
-                bgcolor=bgcolor,cb_format=cb_format,scalexy=scalexy,patches=patches,
-                rasterized=rasterized,fig=fig,ax=axes.flatten()[iax],nolog=True,**kwargs)
-
-      iax=iax+1
-
-    fig.tight_layout()
-
-    return self._closefig(fig)
-
-  def plot_reaccont(self,model,chemana,rtype,level=1,showAbun=False,values=None,
-                    label=None,cmap=None,zlog=True,zlim=[None,None],
-                    clevels=None,clabels=None,contour=True,
-                    extend="neither",oconts=None,nbins=70,
-                    bgcolor=None,cb_format="%.1f",patches=None,
-                    rasterized=True,ax=None,**kwargs):
-    '''
-    Make a contour plot with the reactions numbers from chemanalyse on top.
-    As spatial coordinates the indices of the spatial grid are used.
-
-    This is a convenience function and is simply a wrapper for
-    :func:`~prodimopy.plot.Plot.plot_cont` routine.
-
-    The same can be achieved by simply using plot_cont and plot the numbers
-    on top (see last part of this routine). Then one has more flexibility.
-
-    Parameters
-    ----------
-
-    model : :class:`prodimopy.read.Data_ProDiMo`
-      the model data
-
-    chemana : class:`prodimopy.read.Chemistry`
-      data resulting from `prodimopy.read.analise_chemistry` on a single species
-
-    rtype : str
-      keyword which sets the type of reactions to be shown (destruction or formation)
-      must be set to either 'd' (destruction) or 'f' (formation)
-
-    level : int
-      1 means most important, 2 second most important etc.
-
-    showAbun : boolean
-      Show the abundances of the species that is analysed as filled contours.
-
-    values : array_like(float,ndim=2)
-      a 2D array with numeric values for the plotting like in :func:`~prodimopy.plot.Plot.plot_cont`.
-      Howver, it an also be `None` (default) in that case the total formation/destruction rate is plotted.
-
-
-    sfigs : array_like(float,ndim=2)
-      Is part of kwargs. But this one is relevant here as one might needs to make
-      the figure larger to see the reactoins numbers. e.g. just pass `sfigs=[2.,2.]`
-    '''
-
-    if showAbun:
-      values=model.getAbun(chemana.species)
-      label=r"$\epsilon("+spnToLatex(chemana.species)+"$)"
-      if zlog: label="log "+label
-
-    if rtype is None or rtype!="d": rtype="f"
-
-    reacs=chemana.get_reac_grid(level,rtype)
-
-    rlabel="form."
-    if rtype=="d": rlabel="dest."
-
-    if values is None:
-      if rtype=="d":
-        values=chemana.totdrate
-      else:
-        values=chemana.totdrate
-
-      label=r"(total "+rlabel+" rate) $[cm^{-3} s^{-1}]$"
-      if zlog: label="log "+label
-
-    if not "title" in kwargs:
-      if level==1:
-        tit="main "+rlabel+" reactions"
-      else:
-        tit=str(level).strip()+r"$^{nd}$ "+rlabel+" reactions"
-
-      kwargs["title"]=tit
-
-    fig=self.plot_cont(model,values,label=label,zlog=zlog,grid=True,
-            zlim=zlim,zr=False,cmap=cmap,clevels=clevels,clabels=clabels,contour=contour,
-            extend=extend,oconts=oconts,acont=None,acontl=None,nbins=nbins,
-            bgcolor=bgcolor,cb_format=cb_format,scalexy=[1.0,1.0],patches=patches,
-            rasterized=rasterized,nolog=True,ax=ax,movie=False,returnFig=True,**kwargs)
-
-    # this is potentially very slow
-    xstart=0
-    xend=model.nx
-    ystart=0
-    yend=model.nz-1
-    if "xlim" in kwargs:
-      if kwargs["xlim"][0] is not None:
-        xstart=kwargs["xlim"][0]
-
-      if kwargs["xlim"][1] is not None:
-        xend=kwargs["xlim"][1]
-
-    if "ylim" in kwargs:
-      if kwargs["ylim"][0] is not None:
-        ystart=kwargs["ylim"][0]
-
-      if kwargs["ylim"][1] is not None:
-        yend=kwargs["ylim"][1]
-
-    for i in range(xstart,xend,1):
-      for j in range(ystart,yend,1):
-        fig.axes[0].text(i,j,reacs[0][i,j],fontsize=3.0,horizontalalignment="center",verticalalignment="bottom",color="white")
-
-    return fig
 
   def plot_reac_ixiz(self,ix,iz,rtype,chemanas,ages,chemana_steadystate=None,ax=None,**kwargs):
     '''
     Plots the rates for the most important reactions and the point ix,iz for the
     given models and chemanalysis list (i.e. a time-dependent |prodimo| disk model.
 
     Parameters
@@ -1869,15 +2177,15 @@
     ax.legend(handles,labels,loc="best",fancybox=False)
     ax.text(0.025,0.025,rstr,
        verticalalignment='bottom',horizontalalignment='left',
        transform=ax.transAxes,alpha=0.75)
 
     return self._closefig(fig)
 
-  def plot_starspec(self,model,ax=None,step=10,xunit="micron",**kwargs):
+  def plot_starspec(self,model,ax=None,step=10,xunit="micron",nuInu=True,**kwargs):
     '''
     Plots the full Stellar Spectrum
 
     Parameters
     ----------
 
     step : int
@@ -1894,67 +2202,89 @@
     if xunit=="eV":
       x=(x*u.micron).to(u.eV,equivalencies=u.spectral()).value
       # switch the axes
       xmin=(1000.0*u.micron).to(u.eV,equivalencies=u.spectral()).value
       xmax=x.max()
       xlabel=r"energy [eV]"
     else:
-
       xmin=x.min()
       xmax=1000.0
       xlabel=r"wavelength [$\mathrm{\mu}$m]"
 
-    y=(model.starSpec.nu*model.starSpec.Inu)[0::step]
+    y=(model.starSpec.Inu)[0::step]
+    if nuInu:
+      y=y*model.starSpec.nu[0::step]
 
     ymin=np.min(y[x>1])
 
     ax.plot(x,y,color="black")
 
     # set defaults, can be overwritten by the kwargs
 
     ax.set_xlim([xmin,xmax])
     ax.set_ylim([ymin,None])
     ax.semilogx()
     ax.semilogy()
     ax.set_xlabel(xlabel)
-    ax.set_ylabel(r"$\mathrm{\nu F_{\nu}\,[erg\,cm^{-2}\,s^{-1}]}$")
+    if nuInu:
+      ax.set_ylabel(r"$\mathrm{\nu I_\nu\,[erg\,cm^{-2}\,s^{-1}\,sr^{-1}]}$")
+    else:
+      ax.set_ylabel(r"$\mathrm{I_\nu\,[erg\,cm^{-2}\,s^{-1}\,sr^{-1}\,Hz^{-1}]}$")
 
     self._dokwargs(ax,**kwargs)
 
     return self._closefig(fig)
 
-  def plot_sed(self,model,plot_starSpec=True,sedObs=None,unit="erg",reddening=False,
-               incidx=0,ax=None,**kwargs):
+  def plot_sed(self,model,plot_starSpec=True,incidx=0,unit="erg",sedObs=None,reddening=False,
+               ax=None,**kwargs):
     '''
-    Plots the seds and the StarSpectrum
+    Plots the sed(s) including the stellar spectrum and observations (last two are optional).
+
+    Parameters
+    ----------
+    model : :class:`~prodimopy.read.Data_ProDiMo`
+      the model data. Only required if wl,ident and or lineObs are passed.
+
+    plot_starSpec : boolean
+      also show the (unobscured) stellar spectrum. Default: True
+
+    incidx : int or array_like(ndim=1)
+      which inclination (index) should be used for plotting (0 is the first one and default).
+      If it is a single value only the profile for that inclination index is plotted.
+
+      If it is an array of values all profiles for that chosen inclinations are plotted.
+      If `incidx=[]` profiles for all inclinations will be plotted.
+
+    unit : str
+      in what unit should the sed be plotted. Possible valuees: `erg`, `W`, `Jy`
+
+    sedObs : :class:`~prodimopy.read.DataContinuumObs`
+      if  :attr:`~prodimopy.read.Data_ProDiMo.sedObs` (e.g. sedObs=model.sedOBS) is provided
+      also the observational data is plotted. But in principal can be any object of type
+      :class:`~prodimopy.read.DataContinuumObs`.
+
+    reddening : boolean
+      Apply reddening. Only possible if sedObs is provided `None`.
+
     '''
     print("PLOT: plot_sed ...")
     fig,ax=self._initfig(ax,**kwargs)
 
     xmin=0.1
     if model.sed==None: return
-    # to be sure we have the right inclination
-    model.sedinc(iinc=incidx)
 
-    # only use every 5 element to speed up plotting
-    x=model.sed.lam
-    if unit=="W":
-      y=model.sed.nuFnuW
-    elif unit=="Jy":
-      y=model.sed.fnuJy
+    if not isinstance(incidx,(collections.abc.Sequence,np.ndarray)):
+        incidx=[incidx]
+      # just for convenience if it is an empty array take all the inclinations
+    elif len(incidx)==0:  # empty array, plot all inclinations
+        # need the line for that
+        incidx=np.arange(len(model.sed._inclinations))
     else:
-      y=model.sed.nu*model.sed.fnuErg
-
-    ymin=np.min(y[model.sed.lam>1])
-
-    if reddening==True and sedObs is not None and sedObs.A_V is not None:
-      # idx validity of extinction function
-      ist=np.argmin(np.abs(x-0.0912))
-      ien=np.argmin(np.abs(x-6.0))
-      y[ist:ien]=y[ist:ien]/prodimopy.extinction.reddening(x[ist:ien]*1.e4,a_v=sedObs.A_V,r_v=sedObs.R_V,model="f99")
+      # make sure that in that case only one inclinations is done
+      incidx=[0]
 
     dist=((model.sed.distance*u.pc).to(u.cm)).value
 
     if plot_starSpec:
       # scale input Stellar Spectrum to the distance for comparison to the SED
       r=((model.starSpec.r*u.R_sun).to(u.cm)).value
 
@@ -1967,16 +2297,41 @@
       elif unit=="Jy":
         yStar=(model.starSpec.Inu)[0::1]
         yStar=yStar*(r**2.0*math.pi*dist**(-2.0))
         yStar=(yStar*u.erg/(u.s*u.cm**2*u.Hz)).to(u.Jy).value
 
       ax.plot(xStar,yStar,color="black")
 
-    # plot the SED
-    ax.plot(x,y,marker=None,label=model.name)
+    # plot it for all selected inclinations
+    for iinc in incidx:
+      # to be sure we have the right inclination
+      model.sedinc(iinc=iinc)
+
+      incstr=r"$i="+"{:3.1f}".format(model.sed.inclination)+r"^\degree$"
+
+      # only use every 5 element to speed up plotting
+      x=model.sed.lam
+      if unit=="W":
+        y=model.sed.nuFnuW
+      elif unit=="Jy":
+        y=model.sed.fnuJy
+      else:
+        y=model.sed.nu*model.sed.fnuErg
+
+      ymin=np.min(y[model.sed.lam>1])
+
+      if reddening==True and sedObs is not None and sedObs.A_V is not None:
+        # idx validity of extinction function
+        ist=np.argmin(np.abs(x-0.0912))
+        ien=np.argmin(np.abs(x-6.0))
+        y[ist:ien]=y[ist:ien]/prodimopy.extinction.reddening(x[ist:ien]*1.e4,a_v=sedObs.A_V,r_v=sedObs.R_V,model="f99")
+
+      # plot the SED
+      print(iinc,incidx,incstr)
+      ax.plot(x,y,marker=None,label=incstr)
 
     if sedObs is not None:
       okidx=np.where(sedObs.flag=="ok")
 
       xsedObs=sedObs.lam
       ysedObs=sedObs.nu*sedObs.fnuErg
       ysedObsErr=sedObs.nu*sedObs.fnuErgErr
@@ -2012,14 +2367,16 @@
       ax.set_ylabel(r"$\mathrm{\lambda F_{\lambda}\,[W\,m^{-2}]}$")
     elif unit=="Jy":
       ax.set_ylabel(r"$\mathrm{flux\,[Jy]}$")
     else:
       ax.set_ylabel(r"$\mathrm{\nu F_{\nu}\,[erg\,cm^{-2}\,s^{-1}]}$")
 #    ax.yaxis.tick_right()
 #    ax.yaxis.set_label_position("right")
+    if len(incidx)>1:  # backward compatibility, dont show lables if only one inclination
+      ax.legend()
 
     self._dokwargs(ax,**kwargs)
 
     return self._closefig(fig)
 
   def _getSEDana_boxpoints(self,lam,model,zr=True):
     '''
@@ -2188,184 +2545,18 @@
     ax.set_xlabel(r"r [au]")
     ax.set_ylabel(r"$\mathrm{\tau_{line}}$")
 
     self._dokwargs(ax,**kwargs)
     self._legend(ax,**kwargs)
 
     return self._closefig(fig)
-
-  def plot_line_origin(self,model,lineIdents,field,label="value",boxcolors=None,showBox=True,showRadialLines=True,showztauD1=True,boxlinewidths=1.5,
-                       boxlinestyles=None,boxhatches=None,lineLabels=None,showLineLabels=True,lineLabelsFontsize=6.0,lineLabelsAlign="left",zlog=True,
-                zlim=[None,None],zr=True,clevels=None,clabels=None,contour=False,
-                extend="neither",oconts=None,nbins=70,
-                bgcolor=None,cb_format="%.1f",scalexy=[1,1],patches=None,
-                rasterized=False,showContOrigin=False,ax=None,**kwargs):
-    '''
-    Plots the line origins for a list of lineestimates given by their lineIdents
-    (["ident",wavelength]).
-
-    Does not give the exact same results as the corresponding idl routines
-    as we do not use interpolation here. We rather use the same method for
-    calculating the averaged values over the emission area and for plotting
-    this area.
-
-    Parameters
-    ----------
-    model : :class:`~prodimopy.read.Data_ProDiMo`
-      the model data
-
-    lineIdents : array_like()
-      list of line identifactor of the form `[["ident",wl],["ident2",wl2]]`.
-
-    field : array_like(float,ndim=2)
-      a 2D array with numeric values for the plotting. E.g. any 2D array
-      of the :class:`~prodimopy.read.Data_ProDiMo` object.
-
-    boxlinewidths : array_like
-      the widths of the line for each box showing the line origin. Can be a
-      scalar, in that case all boxes have the same linewidth
-
-    '''
-    if boxcolors is None:
-      boxcolors=[self.pcolors["red"],self.pcolors["orange"],self.pcolors["brown"],
-                 self.pcolors["purple"],self.pcolors["gray"]]
-
-    if boxlinestyles is None:
-      boxlinestyles=["-"]*10
-    elif np.isscalar(boxlinestyles):
-      boxlinestyles=[boxlinestyles]*10
-
-    if np.isscalar(boxlinewidths):
-      boxlinewidths=[boxlinewidths]*10
-
-    # if it is only one line (no list of list) make it a list
-    if (type(lineIdents[0])==str): lineIdents=[lineIdents]
-
-    lestimates=list()
-    for id in lineIdents:
-      lestimates.append(model.getLineEstimate(id[0],id[1]))
-
-    if patches is None:
-      patches=list()
-
-    if len(boxcolors)<len(lestimates) or len(boxlinestyles)<len(lestimates):
-      print("Not enough boxcolors or boxlinestyles available! ")
-      return
-
-    ibox=0
-    for lesti in lestimates:
-      # to be consistent we use the LineOriginMask to determine the box
-      # as a result the plotted region is not necessarely the same as in idl
-      # as we do not interpolate here
-      xmasked=np.ma.masked_array(model.x,mask=model.getLineOriginMask(lesti))
-      x15=np.min(xmasked)
-      x85=np.max(xmasked)
-      xi15=np.argmin(np.abs(model.x[:,0]-x15))
-      xi85=np.argmin(np.abs(model.x[:,0]-x85))
-
-      z85s=[[model.x[rp.ix,0],rp.z85] for rp in lesti.rInfo[xi15:xi85+1]]
-      z15s=[[model.x[rp.ix,0],rp.z15] for rp in lesti.rInfo[xi85:xi15-1:-1]]
-      points=z85s+z15s
-
-      if zr is True:
-        for point in points:
-          point[1]=point[1]/point[0]
-
-      if showBox:
-        if len(points)>1:
-          patch=mpl.patches.Polygon(points,closed=True,fill=False,color=boxcolors[ibox],
-                                      linestyle=boxlinestyles[ibox],
-                                      zorder=100,linewidth=boxlinewidths[ibox])
-
-          patches.append(patch)
-        else:
-          print("WARN: Unable to calculate a proper region for the line origin: "+str(lesti))
-
-      if showContOrigin is True:
-        if (model.sed is not None and model.sed.sedAna is not None):
-          pointsc=self._getSEDana_boxpoints(lesti.wl,model,zr)
-          if len(pointsc)>1:
-            patchc=mpl.patches.Polygon(pointsc,closed=True,fill=False,
-                                         color=boxcolors[ibox],zorder=100,
-                                         linewidth=1.0,linestyle="--")
-            patches.append(patchc)
-          else:
-            print("WARN: Unable to calculate a proper region for the continuum origin: "+str(lesti))
-
-      ibox+=1
-
-    fig=self.plot_cont(model,field,label=label,zlog=zlog,
-                zlim=zlim,zr=zr,clevels=clevels,clabels=clabels,contour=False,
-                extend=extend,oconts=oconts,acont=None,acontl=None,nbins=nbins,
-                bgcolor=bgcolor,cb_format=cb_format,scalexy=scalexy,patches=patches,
-                rasterized=rasterized,returnFig=True,ax=ax,**kwargs)
-
-    if ax is None:
-      ax=fig.axes[0]
-
-    # show the full emitting layer as function of radius
-    # maybe this slows down the pl
-    if showRadialLines or showztauD1:
-      iest=0
-      r=model.x[:,0]
-      for lesti in lestimates:
-        z15=[rinf.z15 for rinf in lesti.rInfo]
-        z85=[rinf.z85 for rinf in lesti.rInfo]
-        if zr is True:
-          z15=z15/r
-          z85=z85/r
-
-        if showBox is False:
-          lsrad=boxlinestyles[iest]
-        else:
-          lsrad=":"
-
-        if showRadialLines:
-          ax.plot(r,z15,color=boxcolors[iest],linestyle=lsrad,linewidth=1.0)
-          ax.plot(r,z85,color=boxcolors[iest],linestyle=lsrad,linewidth=1.0)
-          if boxhatches is not None:
-            ax.fill_between(r,z15,z85,edgecolor=boxcolors[iest],hatch=boxhatches[iest],facecolor="none",linewidth=0.0)
-
-        # can be None just check the first entry
-        if showztauD1 and lesti.rInfo[0].ztauD1 is not None:
-          ztauD1=[rinf.ztauD1 for rinf in lesti.rInfo]
-          if zr: ztauD1=ztauD1/r
-
-          ax.plot(r,ztauD1,color=boxcolors[iest],linestyle="--",linewidth=1.0)
-
-        iest+=1
-
-    if showLineLabels:
-      ibox=0
-      for idline,lesti in zip(lineIdents,lestimates):
-        if lineLabels is not None:
-          label=lineLabels[ibox]
-        else:
-          label="$"+spnToLatex(idline[0])+"$ "+("{:10.2f}".format(lesti.wl)).strip()+r" $\mu$m"
-
-        # FIXME: quick and dirty, ref fontsize =6.0
-        vpos=ibox/(18.0-(lineLabelsFontsize/6.0-1.0)*12.0)
-        if lineLabelsAlign=="right":
-          ax.text(0.95,0.92-vpos,label,
-                horizontalalignment='right',
-                verticalalignment='bottom',fontsize=lineLabelsFontsize,
-                transform=ax.transAxes,color=boxcolors[ibox],
-                bbox=dict(boxstyle='square,pad=0.1',fc='white',ec='none'))
-        else:
-          ax.text(0.02,0.92-vpos,label,
-                horizontalalignment='left',
-                verticalalignment='bottom',fontsize=lineLabelsFontsize,
-                transform=ax.transAxes,color=boxcolors[ibox],
-                bbox=dict(boxstyle='square,pad=0.1',fc='white',ec='none'))
-        ibox+=1
-
-    return self._closefig(fig)
+  
 
   def plot_lineprofile(self,model=None,wl=None,ident=None,lineObj=None,linetxt=None,lineObs=None,incidx=0,
-                       unit="Jy",normalized=False,convolved=False,style=None,color=None,ax=None,**kwargs):
+                       unit="Jy",normalized=False,convolved=False,removecont=True,style=None,color=None,ax=None,**kwargs):
     '''
     Plots the line profile for the given line (id wavelength and optionally the line ident)
 
     Parameters
     ----------
     model : :class:`~prodimopy.read.Data_ProDiMo`
       the model data. Only required if wl,ident and or lineObs are passed.
@@ -2373,22 +2564,22 @@
     wl : float
       The wavelength of the line in micrometer. Plotted is the line with the wavelength
       closest to `wl`.
 
     ident : str
       The optional line ident which is additionally use to identify the line.
 
-    lineObj : :class:`prodimopy.read.DataLine`
+    lineObj : :class:`~prodimopy.read.DataLine`
       Pass `DataLine` object. In that case wl and ident are ignored.
 
     linetxt : str
-      A string the is used as the label for the line
+      A string that is used as the label for the line.
 
     lineObs : array_like(ndim=1)
-      list of :class:`prodimopy.read.DataLineObs` objects. Must be consistent with the list of
+      list of :class:`~prodimopy.read.DataLineObs` objects. Must be consistent with the list of
       lines from the line radiative transfer.
 
     incidx : int or array_like(ndim=1)
       which inclination (index) should be used for plotting (0 is the first one and default).
       If it is a single value only the profile for that inclination index is plotted.
 
       If it is an array of values all profiles for that chosen inclinations are plotted.
@@ -2402,14 +2593,17 @@
       `unit="Jy"` (default) and `unit="ErgAng"`
 
     normalized : boolean
       if `True` normalize the profile to the peak flux
 
     convolved : boolean
       if `True` plot the convolved profile.
+    
+    removecont : boolean
+      if `True` remove the continuum from the profile. Default: `True`
 
     color : str
       the color for the plotted profile.
 
     style : str
       if style is `step` the profile is plotted as a step function assuming
       the values are the mid point of the bin.
@@ -2454,17 +2648,19 @@
 
       # text for the title
 
       # FIXME: ist not up to date anymore with the unit treatment in lineprofile
       x=line.profile.velo
 
       if convolved:
-        y=line.profile.flux_conv-line.profile.flux_conv[0]
+        y=line.profile.flux_conv
+        if removecont: y=y-line.profile.flux_conv[0]          
       else:
-        y=line.profile.flux-line.profile.flux[0]
+        y=line.profile.flux
+        if removecont: y=y-line.profile.flux[0]
 
       if normalized:
         if i==0:  # always normalize to the first inclination
           norm=np.max(y)
         y=y/norm
 
       if linetxt is None:
@@ -2794,14 +2990,121 @@
       CB=fig.colorbar(CS,ax=axcb,pad=0.01,format="%3.1e",fraction=cb_fraction)
       CB.set_label(r"$I_\mathrm{\nu}\,[erg/cm^2/s/Hz/sr]$")
 
     self._dokwargs(ax,**kwargs)
 
     return self._closefig(fig)
 
+  def plot_sled(self,models,lineIdents,units='W',
+                ax=None,title='SLED',**kwargs):
+    '''
+    Plots the Spectral Line Energy Distribution
+
+    Parameters
+    ----------
+    models : list(:class:`~prodimopy.read.Data_ProDiMo`)
+            or a single model
+      the model(s) to plot
+
+    lineIdents : array_like
+      a list of line identifiers. Examples
+
+      `lineIdents = ['CO']`
+      
+      `lineIdents = ['CO', 'o-H2', 'p-H2O']`
+
+    units : str, optional
+      In which units should be plotted.
+      Allowed values: `erg` [erg/s/cm^2], `W` [W/m^2]
+      default : `W`
+
+    Example
+    -------
+    
+    In the directory of the ProDiMo model
+
+    .. code-block:: python
+
+       from matplotlib.backends.backend_pdf import PdfPages
+       import prodimopy.plot as pplot
+       import prodimopy.read as pread
+    
+       outfile = "out_test.pdf"
+       model=pread.read_prodimo()
+      
+       with PdfPages(outfile) as pdf:
+         pp=pplot.Plot(pdf, title=model.name)
+         pp.plot_sled(model, ["CO", "o-H2"])
+    '''
+
+    print("PLOT: plot_sled ...")
+
+    if not isinstance(models, list):
+      models = [models]
+
+    if units == "erg":
+        # 1 erg/s/cm2 = 1000 W/m2
+        flux_correction = 1e3
+    else:
+        flux_correction = 1.0
+
+    fig, ax = self._initfig(ax,**kwargs)
+
+    iplot=0
+    xmin=1.e100
+    xmax=0
+    ymin=1.e100
+    ymax=-1.e00
+    for model in models:
+      for sp in lineIdents:
+        lests = model.selectLineEstimates(sp)
+        if lests != '':
+          lam, flux = [], []
+          for lest in lests:
+            lam.append(lest.wl)
+            flux.append(lest.flux)
+
+        x = np.array(lam)  # micron
+        y = np.array(flux) * flux_correction  # u.W / u.m**2
+
+        # line flux estimates can be negative
+        # aka absorption lines
+        ythres = 1e-30
+        wneg = y <= 0. 
+        y[wneg] = ythres
+
+        ax.scatter(x,y,s=1,alpha=0.5,label=sp)
+        
+        if min(x) < xmin: xmin = 0.5 * min(x)
+        if max(x) > xmax: xmax = 5.0 * max(x)
+        if min(y) < ymin: ymin = 0.5 * min(y)
+        if max(y) > ymax: ymax = 10.0 * max(y)
+
+      iplot = iplot + 1
+      if iplot == 0: return
+
+      # set defaults, can be overwritten by the kwargs
+      if ymin < 1e-30: ymin = ythres
+      ax.set_xlim(xmin,xmax)
+      ax.set_ylim([ymin,ymax])
+      ax.semilogx()
+      ax.semilogy()
+      ax.set_title(title)
+      ax.set_xlabel(r"wavelength [$\mu$m]")
+      if units == "W":
+        ax.set_ylabel(r"$\mathrm{\lambda F_{\lambda}\,[W\,m^{-2}]}$")
+      else:
+        ax.set_ylabel(r"$\mathrm{\nu F_{\nu}\,[erg\,cm^{-2}\,s^{-1}]}$")
+
+    self._dokwargs(ax,**kwargs)
+
+    self._legend(ax,**kwargs)
+
+    return self._closefig(fig)
+
 
 class Contour(object):
   '''
   Define a Contour that can be used in the contour plotting routines.
 
   Objects of this class can be passed to e.g. the :func:`~prodimopy.plot.Plot.plot_cont` routine and will be drawn their.
 
@@ -2848,17 +3151,30 @@
     self.showlabels=showlabels
     """ boolean : `False`
       show text label for each level or not (default: False)
       Still kind of experimental
     """
     self.label_locations=label_locations
     self.label_fmt=label_fmt
+    """ str : "%.1f"
+      Format string for the labels if shown. Example: `r"A$_V$=%1.0f"`
+    """
     self.label_fontsize=label_fontsize
+    """ int : `7`
+      The fontsize of the contour levedl if they are shown
+    """
     self.label_inline_spacing=label_inline_spacing
+    """ int : `5`
+      Control the space around the contour label (i.e. if it overlaps with the line)
+    """
     self.filled=filled
+    """ boolean : `False`
+      Use filled contours (contourf) instead of lines. Can be usefull sometimes.
+      But not supported everywhere (just try).
+    """
 
 
 def spnToLatex(spname):
   """
   Utilitiy function to convert species names to proper latex math strings.
 
   The returned string can directly be embedded in a latex $ $ statement.
```

### Comparing `prodimopy-2.2.1/prodimopy/plot_casasim.py` & `prodimopy-2.3/prodimopy/plot_casasim.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.2.1/prodimopy/plot_mc.py` & `prodimopy-2.3/prodimopy/plot_mc.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.2.1/prodimopy/plot_models.py` & `prodimopy-2.3/prodimopy/plot_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -702,14 +702,20 @@
     r : float
       The radius at which the plot should be made
       UNIT: `[au]`
 
     species : str
       The species name for which the abundance should be plotted.
 
+
+    .. todo::
+
+      Make this a wrapper of :func:`~prodimopy.PlotModels.plot_vertical`. Just pass `nmol` as fieldname and
+      species name
+
     '''
 
     print("PLOT: plot_abunvert ...")
 
     rstr=r"r$\approx${:.2f} au".format(r)
 
     fig,ax=plt.subplots(1,1)
@@ -1628,26 +1634,26 @@
     else:
       ax.set_ylabel(r"$\mathrm{I_\nu\,[erg\,cm^{-2}\,s^{-1}\,sr^{-1}\,Hz^{-1}]}$")
 #    ax.set_ylabel(r"$\mathrm{\nu F_{\nu}\,[erg\,cm^{-2}\,s^{-1}]}$")
     ax.set_xlabel(xlabel)
 
     self._dokwargs(ax,**kwargs)
 
-    self._legend(ax)
+    self._legend(ax,**kwargs)
 
     return self._closefig(fig)
 
   def plot_line_profil(self,models,wl,ident=None,linetxt=None,lineObs=None,
                        unit="Jy",normalized=False,**kwargs):
 
     print("WARN: plot_line profil ... please use plot_lineprofile instead. This routine will be removed in the next version.")
     return self.plot_lineprofile(models,wl,ident=ident,linetxt=linetxt,lineObs=lineObs,
                        unit=unit,normalized=normalized,**kwargs)
 
-  def plot_lineprofile(self,models,wl,ident=None,contsub=True,linetxt=None,lineObs=None,
+  def plot_lineprofile(self,models,wl,ident=None,contsub=True,linetxt=None,lineObs=None,incidx=0,
                        normalized=False,convolved=False,style=None,ax=None,**kwargs):
     '''
     Plots the line profile for the given line (id wavelength and line ident)
 
     Parameters
     ----------
     models : array_like(:class:`~prodimopy.read.Data_ProDiMo`,dim=1)
@@ -1666,14 +1672,19 @@
     linetxt : str
       A string the is used as the label for the line. Default: `None`
 
     lineObs : array_like(ndim=1)
       list of :class:`prodimopy.read.DataLineObs` objects. Must be consistent with the list of
       lines from the line radiative transfer.
 
+    incidx : int
+      which inclination (index) should be used for plotting (0 is the first one and default).      
+      
+      If lineObj is passed only one inclination (the one set in that obj) will be plotted.
+
     normalized : boolean
       if `True` normalize the profile to the peak flux of each line
 
     convolved : boolean
       if `True` plot the convolved profile.
 
     style : str
@@ -1687,15 +1698,15 @@
 
     iplot=0
     xmin=1.e100
     xmax=-1.e100
     ymin=1.e100
     ymax=-1.e100
     for model in models:
-      line=model.getLine(wl,ident=ident)
+      line=model.getLine(wl,ident=ident,incidx=incidx)
       if line==None: continue
 
       # text for the title
       if iplot==0 and linetxt is None:
         linetxt=line.species+"@"+"{:.2f}".format(line.wl)+r" $\mathrm{\mu m}$"
       x=line.profile.velo
```

### Comparing `prodimopy-2.2.1/prodimopy/plot_slab.py` & `prodimopy-2.3/prodimopy/plot_slab.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.2.1/prodimopy/read.py` & `prodimopy-2.3/prodimopy/read.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,14 +114,24 @@
     """ int :
       The number of cooling processes included in the model.
     """
     self.p_dust_to_gas=None
     """ float :
       The global dust to gass mass ratio (single value, given Parameter)
     """
+    self.p_v_turb=None
+    """ float :
+      The global turbulent velocity (single value)
+      `UNIT:` |kms^-1|
+    """
+    self.p_rho_grain=None
+    """ float :
+      The global grain mass density (the density of one dust grain)
+      `UNIT:` |gcm^-3|
+    """      
     self.mstar=None
     """ float :
       The stellar mass in solar units.
       is taken from ProDiMo.out
     """
     self.x=None
     """ array_like(float,ndim=2) :
@@ -1680,15 +1690,15 @@
 
   @property
   def flux(self):
     return self._fluxs[self.__incidx]
 
   @property
   def fcont(self):
-    return self._fcont[self.__incidx]
+    return self._fconts[self.__incidx]
 
   @property
   def profile(self):
     return self._profiles[self.__incidx]
 
   @property
   def inclination(self):
@@ -1747,26 +1757,51 @@
     for i in range(len(self._inclinations)):
       self._profiles[i].convolve(R)
 
 
 class DataLineObs(DataLine):
   '''
   Holds the observational data for one line.
+
+  Differently to DataLine DataLineObs does not care about 
+  multiple inclinations. So simply some setter and getters are used
+  to fill the list quantities (first entry).   
   '''
 
   def __init__(self,flux,flux_err,fwhm,fwhm_err,flag):
     super(DataLineObs,self).__init__()
     self.flux=flux
     self.flux_err=flux_err
     self.fwhm=fwhm
     self.fwhm_err=fwhm_err
     self.flag=flag.lower()
     self.profile=None
     self.profileErr=None
 
+  @property
+  def flux(self):
+    return self._fluxs[0]
+
+  @flux.setter
+  def flux(self,flux):
+    self._fluxs.append(flux)
+
+  @property
+  def profile(self):
+    # FIXME: check what happens if _profiles is empty
+    return self._profiles[0]
+
+  @profile.setter
+  def profile(self,value):
+    # Not very nice, but per definition there can be only one line profile
+    # from the observations (this avoids mutliple entries)
+    if len(self._profiles)>0:
+      self._profiles[0]=value
+    else:  
+      self._profiles.append(value)
 
 class DataFLiTsSpec(object):
   '''
   Data container for a FLiTs spectrum.
   Currently provides only the wavelength grid and the flux in Jy, as produced
   by FLiTs.
   '''
@@ -1864,30 +1899,29 @@
     """""
     self.ident=ident
     """ string :
       The line identifications (species)
     """
     self.wl=wl
     """ float :
-      The wavelength of the line.
-      `UNIT: micron`
+      The wavelength of the line. `UNIT: micron`
     """
     self.jup=jup
     """ int :
     Upper level as defined in ProDiMo ((not the real one!)
     """
     self.jlow=jlow
     """  int :
     Lower level as defined in ProDiMo (not the real one!).
     """
     self.flux=flux
     self.rInfo=None
-    """ :class:`prodimopy.read.DataLineEstimateRinfo`
+    """ list(:class:`prodimopy.read.DataLineEstimateRInfo`) :
       The extra radial information of the line.
-    """
+    """    
     self.__posrInfo=None  # stores the position of the radial information to access is later on
 
   @property
   def frequency(self):
     '''
     Frequency of the line in [GHz].
     '''
@@ -1908,20 +1942,48 @@
           str(self.flux))
     return text
 
 
 class DataLineEstimateRInfo(object):
   '''
   Data container for the extra radial information for a single line estimate.
-  The data is read from FlineEstimates.out
+  The data is read from `FlineEstimates.out`. 
+  This object corresponds to one line of the radial information in `FlineEstimates.out`
+
   '''
 
   def __init__(self,ix,iz,Fcolumn,tauLine,tauDust,z15,z85,ztauD1,Ncol):
+    """
+
+    Parameters
+    ----------
+
+    ix : int
+    iz : int
+    Fcolumn : float
+    tauLine : float
+    tauDust : float
+    z15 : float
+    z85 : float
+    ztauD1 : float
+    Ncol : float    
+   
+    Attributes
+    ----------
+
+    """
+
     self.ix=ix
+    """ int :
+    The x-coordinate index.
+    """
     self.iz=iz
+    """ int :
+    The z-coordinate index.
+    """
     self.Fcolumn=Fcolumn
     """ float :
     the line flux in the particular column (check again, i guess the iz coordinate is irrelevant for that)
     """
     self.tauLine=tauLine
     """ float :
     the total vertical optical depth of the line measured from tauDust=1 upwards f(r)
@@ -1942,14 +2004,15 @@
     """ float :
      z-level where taudust_ver(lambda_line)=1; `UNIT:` au
      Is `None` for FlineEstimates version < 3
     """
     self.Ncol=Ncol
     """ float :
     The column density of the species as f(r) measured from ztauD1 upwards; `UNIT:` |cm^-2|
+    
     It considers both halfs of the disks (i.e. for the case of tauDust <1 ) so the values can be different to
     :attr:`~prodimopy.read.Data_ProDiMo.cdnmol` where only one half of the disk is considered.
     Is `None` for FlineEstimates version < 3
     """
 
 
 class DataGas(object):
@@ -2620,14 +2683,16 @@
   # data is filled in the routine
   data.species=read_species(directory,tarfile=tarfile)
   if data.species is not None:  # None should not happen
     data.nspec=len(data.species.mass)
 
   data.mstar=float(lines[0].split()[1])
   data.p_dust_to_gas=float(lines[9].split()[1])
+  data.p_rho_grain=float(lines[10].split()[1])
+  data.p_v_turb=float(lines[18].split()[1])
 
   strs=lines[21].split()
   data.nx=int(strs[1])
   data.nz=int(strs[2])
   # is not set in read_species() FIXME: not nice
   nspecreal=int(strs[3])
   if data.nspec is None:  # should not happen
@@ -3318,15 +3383,19 @@
 
   return profile,err
 
 
 def read_gas(directory,filename="gas_cs.out",tarfile=None):
   '''
   Reads gas_cs.out
-  Returns an object of Type DataDust
+
+  Returns
+  -------
+  :class:`~prodimopy.read.DataGas`
+
   '''
   f,dummy=_getfile(filename,directory,tarfile)
   if f is None: return None
 
   nlam=int(f.readline().strip())
 
   # skip one line
@@ -3658,18 +3727,22 @@
 
   return bgSpec
 
 
 def read_dust(directory,filename="dust_opac.out",tarfile=None):
   '''
   Reads dust_opac.out and if it exists dust_sigmaa.out.
-  Returns an object of Type DataDust
   Does not read the dust composition yet
 
   FIXME: reading of dust_opac.out should be in separate routine.
+
+  Returns
+  -------
+  :class:`~prodimopy.read.DataDust`
+
   '''
   f,dummy=_getfile(filename,directory,tarfile)
   if f is None: return None
 
   fields=[int(field) for field in f.readline().split()]
   ndsp=fields[0]
   nlam=fields[1]
@@ -3877,28 +3950,45 @@
   # FIXME: test the integration error can be at most 16% ... good enough for now (most fields are better)
   # nHverC=data._rcdnmol[:,:,data.spnames["H"]]+data._rcdnmol[:,:,data.spnames["H+"]]+data._rcdnmol[:,:,data.spnames["H2"]]*2.0
   # izt=data.nz-2
   # print(nHverC[:,izt],data.NHrad[:,izt])
   # print(np.max(np.abs(1.0-nHverC[1:,:]/data.NHrad[1:,:])))
 
 
-def analyse_chemistry(species,model,name=None,directory=None,filenameReactions="Reactions.out",
-                      filenameChemistry='chemanalysis.out',to_txt=True,td_fileIdx=None):
+def analyse_chemistry(species,model,to_txt=True,td_fileIdx=None,filenameReactions="Reactions.out",
+                      filenameChemistry='chemanalysis.out',name=None,directory=None):
   """
   Function that analyses the chemistry in a similar way to chemanalysis.pro.
 
   Parameters
   ----------
 
   species : str
     The species name one wants to analyze.
 
-  model : :class:`prodimopy.read.Data_ProDiMo`
+  model : :class:`~prodimopy.read.Data_ProDiMo`
     the |prodimo| model data.
 
+  to_txt : boolean
+    Write info about formation and destruction reactions for the selecte molecule
+    to a txt file. Default: `True`
+
+  td_fileIdx : str
+    For time-dependent chemanalysis. Provide here the idx for the timestep.
+    E.g. `"0001"` for the first one.
+
+  .. todo::
+    * `name` and `directory` are not used anymore (I think) can be removed
+
+  Returns
+  -------
+  :class:`prodimopy.read.Chemistry`
+    Object that holds all the required information and can be use for the plotting routines
+    or for :func:`~prodimopy.read.reac_rates_ix_iz`
+
   """
   chemistry=Chemistry(None)
 
   # has to be from the particular model.
   if directory is None:
     directory=model.directory
 
@@ -4024,26 +4114,24 @@
   print("INFO: Calc time: ","{:4.2f}".format(timer()-start)+" s")
   return chemistry
 
 
 def reac_rates_ix_iz(model,chemana,ix=None,iz=None,locau=None):
   """
   Function that analyses the chemana manually via a point-by-point
-  analysis for a given species.
-  Start by entering the point-coordinates ix,iz, then you can have a look
-  at the most important formation and destruction rates.
+  analysis for a given species. Shows the most important formation and destruction rates for the given point ix,iz (or in au via Parameter `locau`).
 
   Parameters
   ----------
 
-  model : :class:`prodimopy.read.Data_ProDiMo`
+  model : :class:`~prodimopy.read.Data_ProDiMo`
     the model data
 
-  chemana : class:`prodimopy.read.Chemistry`
-    data resulting from `prodimopy.read.analise_chemistry` on a single species
+  chemana : :class:`~prodimopy.read.Chemistry`
+    data resulting from :func:`~prodimopy.read.analyse_chemistry` on a single species
 
   ix : int
     ix corresponding to desired radial location in grid, starting at 0
 
   iz : int
     iz corresponding to desired radial location in grid, starting at 0
```

### Comparing `prodimopy-2.2.1/prodimopy/read_casasim.py` & `prodimopy-2.3/prodimopy/read_casasim.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.2.1/prodimopy/read_mc.py` & `prodimopy-2.3/prodimopy/read_mc.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,15 +258,15 @@
   # if name == None: name=
   #  dirfields = directory.split("/")
   #  name = dirfields[len(dirfields) - 1]
 
   mc=Data_mc(name)
 
   mc.directory=directory
-  mc.ratecoefficients=_read_ratecoefficients(directory+"/"+rcfile)
+  mc.ratecoefficients=_read_ratecoefficients(os.path.join(directory,rcfile))
 
   # if there is a MC_conc_tdep.out and no mc_ages.txt read the data from there
   if (not os.path.isfile(directory+"/"+agesfile) and
       os.path.isfile(directory+"/MC_conc_tdep.out")):
     mc.species,mc.ages,mc.abundances=read_tdep_file(directory+"/MC_conc_tdep.out")
   else:
     mc.species=_read_species(directory+"/"+speciesfile)
```

### Comparing `prodimopy-2.2.1/prodimopy/read_slab.py` & `prodimopy-2.3/prodimopy/read_slab.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,5558 +22,5897 @@
 00000150: 616c 5f75 6e69 7420 6173 2061 750a 6672  al_unit as au.fr
 00000160: 6f6d 2073 6369 7079 2e63 6f6e 7374 616e  om scipy.constan
 00000170: 7473 2069 6d70 6f72 7420 682c 632c 6b0a  ts import h,c,k.
 00000180: 6672 6f6d 2073 6369 7079 2e63 6f6e 7374  from scipy.const
 00000190: 616e 7473 2069 6d70 6f72 7420 7061 7273  ants import pars
 000001a0: 6563 2061 7320 7063 0a66 726f 6d20 7363  ec as pc.from sc
 000001b0: 6970 792e 7370 6563 6961 6c20 696d 706f  ipy.special impo
-000001c0: 7274 2065 7266 2061 7320 7365 7266 0a69  rt erf as serf.i
-000001d0: 6d70 6f72 7420 7370 6563 7472 6573 0a0a  mport spectres..
-000001e0: 696d 706f 7274 206e 756d 7079 2061 7320  import numpy as 
-000001f0: 6e70 0a69 6d70 6f72 7420 7061 6e64 6173  np.import pandas
-00000200: 2061 7320 7064 0a0a 0a63 6c61 7373 2073   as pd...class s
-00000210: 6c61 625f 6461 7461 3a0a 2020 2020 2222  lab_data:.    ""
-00000220: 220a 2020 2020 5374 7275 6374 7572 6520  ".    Structure 
-00000230: 6f66 2074 6865 206d 6f64 656c 7320 7365  of the models se
-00000240: 7420 7570 2066 726f 6d20 7468 6520 536c  t up from the Sl
-00000250: 6162 496e 7075 742e 696e 2066 696c 653a  abInput.in file:
-00000260: 0a0a 2020 2020 5072 6f44 694d 6f20 7275  ..    ProDiMo ru
-00000270: 6e0a 0a20 2020 207c 5f5f 4d6f 6465 6c5f  n..    |__Model_
-00000280: 310a 2020 2020 2020 2020 7c5f 5f6d 6f6c  1.        |__mol
-00000290: 6563 756c 655f 310a 0a20 2020 2020 2020  ecule_1..       
-000002a0: 207c 5f5f 6d6f 6c65 6375 6c65 5f32 0a0a   |__molecule_2..
-000002b0: 2020 2020 2020 2020 7c5f 5f2e 2e2e 0a0a          |__.....
-000002c0: 2020 2020 2020 2020 7c5f 5f6d 6f6c 6563          |__molec
-000002d0: 756c 655f 6e0a 2020 2020 7c5f 5f4d 6f64  ule_n.    |__Mod
-000002e0: 656c 5f32 0a20 2020 2020 2020 207c 5f5f  el_2.        |__
-000002f0: 6d6f 6c65 6375 6c65 5f31 0a0a 2020 2020  molecule_1..    
-00000300: 2020 2020 7c5f 5f6d 6f6c 6563 756c 655f      |__molecule_
-00000310: 320a 0a20 2020 2020 2020 207c 5f5f 2e2e  2..        |__..
-00000320: 2e0a 0a20 2020 2020 2020 207c 5f5f 6d6f  ...        |__mo
-00000330: 6c65 6375 6c65 5f6e 0a20 2020 207c 5f5f  lecule_n.    |__
-00000340: 2e2e 2e0a 2020 2020 2020 2020 7c5f 5f2e  ....        |__.
-00000350: 2e2e 0a0a 2020 2020 2020 2020 7c5f 5f2e  ....        |__.
-00000360: 2e2e 0a0a 2020 2020 2020 2020 7c5f 5f2e  ....        |__.
-00000370: 2e2e 0a20 2020 207c 5f5f 4d6f 6465 6c5f  ...    |__Model_
-00000380: 6e0a 2020 2020 2020 2020 7c5f 5f6d 6f6c  n.        |__mol
-00000390: 6563 756c 655f 310a 0a20 2020 2020 2020  ecule_1..       
-000003a0: 207c 5f5f 6d6f 6c65 6375 6c65 5f32 0a0a   |__molecule_2..
-000003b0: 2020 2020 2020 2020 7c5f 5f2e 2e2e 0a0a          |__.....
-000003c0: 2020 2020 2020 2020 7c5f 5f6d 6f6c 6563          |__molec
-000003d0: 756c 655f 6e0a 0a20 2020 2044 6174 6120  ule_n..    Data 
-000003e0: 7374 7275 6374 7572 6520 746f 2068 6f6c  structure to hol
-000003f0: 6420 7468 6520 636f 7272 6573 706f 6e64  d the correspond
-00000400: 696e 6720 736c 6162 206d 6f64 656c 206f  ing slab model o
-00000410: 7574 7075 740a 2020 2020 736c 6162 5f64  utput.    slab_d
-00000420: 6174 610a 0a20 2020 207c 5f64 6972 6563  ata..    |_direc
-00000430: 746f 7279 0a0a 2020 2020 7c5f 6d6f 6465  tory..    |_mode
-00000440: 6c73 0a20 2020 2020 2020 207c 5f5f 6d6f  ls.        |__mo
-00000450: 6465 6c5f 3120 2874 7970 653a 736c 6162  del_1 (type:slab
-00000460: 290a 2020 2020 2020 2020 2020 207c 5f5f  ).           |__
-00000470: 7072 6f64 696d 6f5f 4d6f 6465 6c5f 315f  prodimo_Model_1_
-00000480: 6d6f 6c65 6375 6c65 5f31 0a20 2020 2020  molecule_1.     
-00000490: 2020 207c 5f5f 6d6f 6465 6c5f 3220 2874     |__model_2 (t
-000004a0: 7970 653a 736c 6162 290a 2020 2020 2020  ype:slab).      
-000004b0: 2020 2020 207c 5f5f 7072 6f64 696d 6f5f       |__prodimo_
-000004c0: 4d6f 6465 6c5f 315f 6d6f 6c65 6375 6c65  Model_1_molecule
-000004d0: 5f32 0a20 2020 2020 2020 207c 5f5f 6d6f  _2.        |__mo
-000004e0: 6465 6c5f 2e2e 2e20 2874 7970 653a 736c  del_... (type:sl
-000004f0: 6162 290a 2020 2020 2020 2020 2020 207c  ab).           |
-00000500: 5f5f 2e2e 2e0a 2020 2020 2020 2020 7c5f  __....        |_
-00000510: 5f6d 6f64 656c 5f6e 2028 7479 7065 3a73  _model_n (type:s
-00000520: 6c61 6229 0a20 2020 2020 2020 2020 2020  lab).           
-00000530: 7c5f 5f70 726f 6469 6d6f 5f4d 6f64 656c  |__prodimo_Model
-00000540: 5f32 5f6d 6f6c 6563 756c 655f 6e0a 2020  _2_molecule_n.  
-00000550: 2020 2020 2020 7c5f 5f6d 6f64 656c 5f6e        |__model_n
-00000560: 2b31 2028 7479 7065 3a73 6c61 6229 0a20  +1 (type:slab). 
-00000570: 2020 2020 2020 2020 2020 7c5f 5f70 726f            |__pro
-00000580: 6469 6d6f 5f4d 6f64 656c 5f32 5f6d 6f6c  dimo_Model_2_mol
-00000590: 6563 756c 655f 310a 2020 2020 2020 2020  ecule_1.        
-000005a0: 7c5f 5f6d 6f64 656c 5f6e 2b32 2028 7479  |__model_n+2 (ty
-000005b0: 7065 3a73 6c61 6229 0a20 2020 2020 2020  pe:slab).       
-000005c0: 2020 2020 7c5f 5f70 726f 6469 6d6f 5f4d      |__prodimo_M
-000005d0: 6f64 656c 5f32 5f6d 6f6c 6563 756c 655f  odel_2_molecule_
-000005e0: 320a 2020 2020 2020 2020 7c5f 5f6d 6f64  2.        |__mod
-000005f0: 656c 5f2e 2e2e 2028 7479 7065 3a73 6c61  el_... (type:sla
-00000600: 6229 0a20 2020 2020 2020 2020 2020 7c5f  b).           |_
-00000610: 5f2e 2e2e 0a20 2020 2020 2020 207c 5f5f  _....        |__
-00000620: 6d6f 6465 6c5f 6e2b 6e20 2874 7970 653a  model_n+n (type:
-00000630: 736c 6162 290a 2020 2020 2020 2020 2020  slab).          
-00000640: 207c 5f5f 7072 6f64 696d 6f5f 6d6f 6465   |__prodimo_mode
-00000650: 6c5f 325f 6d6f 6c65 6375 6c65 5f6e 0a20  l_2_molecule_n. 
-00000660: 2020 2020 2020 207c 5f5f 6d6f 6465 6c5f         |__model_
-00000670: 2e2e 2e20 2874 7970 653a 736c 6162 290a  ... (type:slab).
-00000680: 2020 2020 2020 2020 2020 207c 5f5f 2e2e             |__..
-00000690: 2e0a 2020 2020 2222 220a 0a20 2020 2064  ..    """..    d
-000006a0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-000006b0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-000006c0: 5f6e 6d6f 6465 6c73 3d30 0a20 2020 2020  _nmodels=0.     
-000006d0: 2020 2022 2222 2069 6e74 6567 6572 203a     """ integer :
-000006e0: 0a20 2020 2020 2020 206e 756d 6265 7220  .        number 
-000006f0: 6f66 206d 6f64 656c 732e 0a20 2020 2020  of models..     
-00000700: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
-00000710: 7365 6c66 2e64 6972 6563 746f 7279 3d4e  self.directory=N
-00000720: 6f6e 650a 2020 2020 2020 2020 2222 2220  one.        """ 
-00000730: 7374 7269 6e67 203a 0a20 2020 2020 2020  string :.       
-00000740: 2054 6865 2064 6972 6563 746f 7279 2066   The directory f
-00000750: 726f 6d20 7768 6963 6820 7468 6520 6d6f  rom which the mo
-00000760: 6465 6c20 7761 7320 7265 6164 2e0a 2020  del was read..  
-00000770: 2020 2020 2020 4361 6e20 6265 2061 2072        Can be a r
-00000780: 656c 6174 6976 6520 7061 7468 2e0a 2020  elative path..  
-00000790: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000007a0: 2020 7365 6c66 2e6d 6f64 656c 733d 5b5d    self.models=[]
-000007b0: 0a20 2020 2020 2020 2022 2222 206c 6973  .        """ lis
-000007c0: 7420 3a0a 2020 2020 2020 2020 5468 6520  t :.        The 
-000007d0: 6c69 7374 2063 6f6e 7461 696e 696e 6720  list containing 
-000007e0: 7468 6520 6d6f 6465 6c73 0a20 2020 2020  the models.     
-000007f0: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
-00000800: 7365 6c66 2e5f 7370 6563 6965 735f 6e75  self._species_nu
-00000810: 6d62 6572 3d4e 6f6e 650a 2020 2020 2020  mber=None.      
-00000820: 2020 2222 2220 6c69 7374 3a0a 2020 2020    """ list:.    
-00000830: 2020 2020 4974 2073 746f 7265 7320 7468      It stores th
-00000840: 6520 7370 6563 6965 7320 6e75 6d62 6572  e species number
-00000850: 2061 6363 6f72 6469 6e67 2074 6f20 536c   according to Sl
-00000860: 6162 496e 7075 742e 696e 206f 6620 616c  abInput.in of al
-00000870: 6c20 6d6f 6465 6c73 0a20 2020 2020 2020  l models.       
-00000880: 2022 2222 0a0a 2020 2020 2020 2020 7365   """..        se
-00000890: 6c66 2e5f 6d6f 6465 6c5f 6e75 6d62 6572  lf._model_number
-000008a0: 3d4e 6f6e 650a 2020 2020 2020 2020 2222  =None.        ""
-000008b0: 2220 6c69 7374 3a0a 2020 2020 2020 2020  " list:.        
-000008c0: 4974 2073 746f 7265 7320 7468 6520 6d6f  It stores the mo
-000008d0: 6465 6c20 6e75 6d62 6572 2061 6363 6f72  del number accor
-000008e0: 6469 6e67 2074 6f20 536c 6162 496e 7075  ding to SlabInpu
-000008f0: 742e 696e 206f 6620 616c 6c20 6d6f 6465  t.in of all mode
-00000900: 6c73 0a20 2020 2020 2020 2022 2222 0a0a  ls.        """..
-00000910: 2020 2020 2020 2020 7365 6c66 2e5f 4e48          self._NH
-00000920: 3d4e 6f6e 650a 2020 2020 2020 2020 2222  =None.        ""
-00000930: 2220 6c69 7374 3a0a 2020 2020 2020 2020  " list:.        
-00000940: 4974 2073 746f 7265 7320 7468 6520 746f  It stores the to
-00000950: 7461 6c20 6761 7320 6465 6e73 6974 6965  tal gas densitie
-00000960: 7320 6f66 2061 6c6c 206d 6f64 656c 730a  s of all models.
-00000970: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-00000980: 2020 2020 2073 656c 662e 5f6e 436f 6c6c       self._nColl
-00000990: 3d4e 6f6e 650a 2020 2020 2020 2020 2222  =None.        ""
-000009a0: 2220 6c69 7374 3a0a 2020 2020 2020 2020  " list:.        
-000009b0: 4974 2073 746f 7265 7320 7468 6520 746f  It stores the to
-000009c0: 7461 6c20 636f 6c6c 6973 696f 6e20 7061  tal collision pa
-000009d0: 7274 6e65 7220 6162 756e 6461 6e63 6520  rtner abundance 
-000009e0: 6f66 2061 6c6c 206d 6f64 656c 730a 2020  of all models.  
-000009f0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-00000a00: 2020 2073 656c 662e 5f6e 653d 4e6f 6e65     self._ne=None
-00000a10: 0a20 2020 2020 2020 2022 2222 206c 6973  .        """ lis
-00000a20: 743a 0a20 2020 2020 2020 2049 7420 7374  t:.        It st
-00000a30: 6f72 6573 2074 6865 2065 6c65 6374 726f  ores the electro
-00000a40: 6e20 6162 756e 6461 6e63 6520 6f66 2061  n abundance of a
-00000a50: 6c6c 206d 6f64 656c 730a 2020 2020 2020  ll models.      
-00000a60: 2020 2222 220a 0a20 2020 2020 2020 2073    """..        s
-00000a70: 656c 662e 5f6e 4865 3d4e 6f6e 650a 2020  elf._nHe=None.  
-00000a80: 2020 2020 2020 2222 2220 6c69 7374 3a0a        """ list:.
-00000a90: 2020 2020 2020 2020 4974 2073 746f 7265          It store
-00000aa0: 7320 7468 6520 4865 2061 6275 6e64 616e  s the He abundan
-00000ab0: 6365 206f 6620 616c 6c20 6d6f 6465 6c73  ce of all models
-00000ac0: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
-00000ad0: 2020 2020 2020 7365 6c66 2e5f 6e48 4949        self._nHII
-00000ae0: 3d4e 6f6e 650a 2020 2020 2020 2020 2222  =None.        ""
-00000af0: 2220 6c69 7374 3a0a 2020 2020 2020 2020  " list:.        
-00000b00: 4974 2073 746f 7265 7320 7468 6520 4849  It stores the HI
-00000b10: 4920 6162 756e 6461 6e63 6520 6f66 2061  I abundance of a
-00000b20: 6c6c 206d 6f64 656c 730a 2020 2020 2020  ll models.      
-00000b30: 2020 2222 220a 0a20 2020 2020 2020 2073    """..        s
-00000b40: 656c 662e 5f6e 4849 3d4e 6f6e 650a 2020  elf._nHI=None.  
-00000b50: 2020 2020 2020 2222 2220 6c69 7374 3a0a        """ list:.
-00000b60: 2020 2020 2020 2020 4974 2073 746f 7265          It store
-00000b70: 7320 7468 6520 4849 2061 6275 6e64 616e  s the HI abundan
-00000b80: 6365 206f 6620 616c 6c20 6d6f 6465 6c73  ce of all models
-00000b90: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
-00000ba0: 2020 2020 2020 7365 6c66 2e5f 6e48 323d        self._nH2=
-00000bb0: 4e6f 6e65 0a20 2020 2020 2020 2022 2222  None.        """
-00000bc0: 206c 6973 743a 0a20 2020 2020 2020 2049   list:.        I
-00000bd0: 7420 7374 6f72 6573 2074 6865 206d 6f6c  t stores the mol
-00000be0: 6563 756c 6172 2068 7964 726f 6765 6e20  ecular hydrogen 
-00000bf0: 6162 756e 6461 6e63 6520 6f66 2061 6c6c  abundance of all
-00000c00: 206d 6f64 656c 730a 2020 2020 2020 2020   models.        
-00000c10: 2222 220a 0a20 2020 2020 2020 2073 656c  """..        sel
-00000c20: 662e 5f64 7573 745f 746f 5f67 6173 3d4e  f._dust_to_gas=N
-00000c30: 6f6e 650a 2020 2020 2020 2020 2222 2220  one.        """ 
-00000c40: 6c69 7374 3a0a 2020 2020 2020 2020 4974  list:.        It
-00000c50: 2073 746f 7265 7320 7468 6520 6475 7374   stores the dust
-00000c60: 2074 6f20 6761 7320 7261 7469 6f20 6f66   to gas ratio of
-00000c70: 2061 6c6c 206d 6f64 656c 730a 2020 2020   all models.    
-00000c80: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-00000c90: 2073 656c 662e 5f76 7475 7262 3d4e 6f6e   self._vturb=Non
-00000ca0: 650a 2020 2020 2020 2020 2222 2220 6c69  e.        """ li
-00000cb0: 7374 3a0a 2020 2020 2020 2020 4974 2073  st:.        It s
-00000cc0: 746f 7265 7320 7468 6520 7475 7262 756c  tores the turbul
-00000cd0: 656e 7420 6272 6f61 6465 6e69 6e67 206f  ent broadening o
-00000ce0: 6620 616c 6c20 6d6f 6465 6c73 0a20 2020  f all models.   
-00000cf0: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-00000d00: 2020 7365 6c66 2e5f 5467 3d4e 6f6e 650a    self._Tg=None.
-00000d10: 2020 2020 2020 2020 2222 2220 6c69 7374          """ list
-00000d20: 3a0a 2020 2020 2020 2020 4974 2073 746f  :.        It sto
-00000d30: 7265 7320 7468 6520 6761 7320 7465 6d70  res the gas temp
-00000d40: 6572 6174 7572 6573 206f 6620 616c 6c20  eratures of all 
-00000d50: 6d6f 6465 6c73 0a20 2020 2020 2020 2022  models.        "
-00000d60: 2222 0a0a 2020 2020 2020 2020 7365 6c66  ""..        self
-00000d70: 2e5f 5464 3d4e 6f6e 650a 2020 2020 2020  ._Td=None.      
-00000d80: 2020 2222 2220 6c69 7374 3a0a 2020 2020    """ list:.    
-00000d90: 2020 2020 4974 2073 746f 7265 7320 7468      It stores th
-00000da0: 6520 6475 7374 2074 656d 7065 7261 7475  e dust temperatu
-00000db0: 7265 7320 6f66 2061 6c6c 206d 6f64 656c  res of all model
-00000dc0: 730a 2020 2020 2020 2020 2222 220a 0a20  s.        """.. 
-00000dd0: 2020 2020 2020 2073 656c 662e 5f73 7065         self._spe
-00000de0: 6369 6573 5f6e 616d 653d 4e6f 6e65 0a20  cies_name=None. 
-00000df0: 2020 2020 2020 2022 2222 206c 6973 743a         """ list:
-00000e00: 0a20 2020 2020 2020 2049 7420 7374 6f72  .        It stor
-00000e10: 6573 2074 6865 206e 616d 6520 6f66 2074  es the name of t
-00000e20: 6865 206d 6f6c 6563 756c 6573 206f 6620  he molecules of 
-00000e30: 616c 6c20 6d6f 6465 6c73 0a20 2020 2020  all models.     
-00000e40: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
-00000e50: 7365 6c66 2e5f 7370 6563 6965 735f 696e  self._species_in
-00000e60: 6465 783d 4e6f 6e65 0a20 2020 2020 2020  dex=None.       
-00000e70: 2022 2222 206c 6973 743a 0a20 2020 2020   """ list:.     
-00000e80: 2020 2049 7420 7374 6f72 6573 2074 6865     It stores the
-00000e90: 2050 726f 4469 4d6f 2073 7065 6369 6573   ProDiMo species
-00000ea0: 2069 6e64 6578 206f 6620 616c 6c20 6d6f   index of all mo
-00000eb0: 6465 6c73 0a20 2020 2020 2020 2022 2222  dels.        """
-00000ec0: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-00000ed0: 6162 756e 6461 6e63 653d 4e6f 6e65 0a20  abundance=None. 
-00000ee0: 2020 2020 2020 2022 2222 206c 6973 743a         """ list:
-00000ef0: 0a20 2020 2020 2020 2049 7420 7374 6f72  .        It stor
-00000f00: 6573 2074 6865 2073 7065 6369 6573 2061  es the species a
-00000f10: 6275 6e64 616e 6365 2061 6363 6f72 6469  bundance accordi
-00000f20: 6e67 2074 6f20 536c 6162 496e 7075 742e  ng to SlabInput.
-00000f30: 696e 206f 6620 616c 6c20 6d6f 6465 6c73  in of all models
-00000f40: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
-00000f50: 2020 2020 2020 7365 6c66 2e5f 6476 3d4e        self._dv=N
-00000f60: 6f6e 650a 2020 2020 2020 2020 2222 2220  one.        """ 
-00000f70: 6c69 7374 3a0a 2020 2020 2020 2020 4974  list:.        It
-00000f80: 2073 746f 7265 7320 7468 6520 7665 6c6f   stores the velo
-00000f90: 6369 7479 2077 6964 7468 206f 6620 616c  city width of al
-00000fa0: 6c20 6d6f 6465 6c73 0a20 2020 2020 2020  l models.       
-00000fb0: 2022 2222 0a0a 2020 2020 2020 2020 7365   """..        se
-00000fc0: 6c66 2e5f 6e6c 6576 656c 733d 4e6f 6e65  lf._nlevels=None
+000001c0: 7274 2065 7266 2061 7320 7365 7266 0a74  rt erf as serf.t
+000001d0: 7279 3a0a 2020 2020 6672 6f6d 2073 7065  ry:.    from spe
+000001e0: 6374 7265 7320 696d 706f 7274 2073 7065  ctres import spe
+000001f0: 6374 7265 735f 6e75 6d62 6120 6173 2073  ctres_numba as s
+00000200: 7065 6374 7265 730a 6578 6365 7074 3a20  pectres.except: 
+00000210: 0a20 2020 2066 726f 6d20 7370 6563 7472  .    from spectr
+00000220: 6573 2069 6d70 6f72 7420 7370 6563 7472  es import spectr
+00000230: 6573 0a0a 696d 706f 7274 206e 756d 7079  es..import numpy
+00000240: 2061 7320 6e70 0a69 6d70 6f72 7420 7061   as np.import pa
+00000250: 6e64 6173 2061 7320 7064 0a0a 636c 6173  ndas as pd..clas
+00000260: 7320 4d79 466f 726d 6174 7465 7228 7374  s MyFormatter(st
+00000270: 7269 6e67 2e46 6f72 6d61 7474 6572 293a  ring.Formatter):
+00000280: 0a20 2020 2022 2222 0a20 2020 2053 7472  .    """.    Str
+00000290: 696e 6720 666f 726d 6174 7465 7220 666f  ing formatter fo
+000002a0: 7220 7072 6f64 7563 696e 6720 696e 7075  r producing inpu
+000002b0: 7420 6669 6c65 730a 2020 2020 2222 220a  t files.    """.
+000002c0: 0a20 2020 2064 6566 2066 6f72 6d61 745f  .    def format_
+000002d0: 6669 656c 6428 7365 6c66 2c76 616c 7565  field(self,value
+000002e0: 2c66 6f72 6d61 745f 7370 6563 293a 0a20  ,format_spec):. 
+000002f0: 2020 2020 2020 2069 6620 666f 726d 6174         if format
+00000300: 5f73 7065 635b 2d31 5d3d 3d27 6d27 3a0a  _spec[-1]=='m':.
+00000310: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00000320: 726e 2073 7570 6572 2829 2e66 6f72 6d61  rn super().forma
+00000330: 745f 6669 656c 6428 7661 6c75 652c 666f  t_field(value,fo
+00000340: 726d 6174 5f73 7065 635b 3a2d 315d 2b27  rmat_spec[:-1]+'
+00000350: 6527 292e 7265 706c 6163 6528 2765 2b27  e').replace('e+'
+00000360: 2c27 6527 290a 2020 2020 2020 2020 656c  ,'e').        el
+00000370: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00000380: 7265 7475 726e 2073 7570 6572 2829 2e66  return super().f
+00000390: 6f72 6d61 745f 6669 656c 6428 7661 6c75  ormat_field(valu
+000003a0: 652c 666f 726d 6174 5f73 7065 6329 0a0a  e,format_spec)..
+000003b0: 0a66 6d74 3d4d 7946 6f72 6d61 7474 6572  .fmt=MyFormatter
+000003c0: 2829 0a0a 636c 6173 7320 736c 6162 5f64  ()..class slab_d
+000003d0: 6174 613a 0a20 2020 2022 2222 0a20 2020  ata:.    """.   
+000003e0: 2053 7472 7563 7475 7265 206f 6620 7468   Structure of th
+000003f0: 6520 6d6f 6465 6c73 2073 6574 2075 7020  e models set up 
+00000400: 6672 6f6d 2074 6865 2053 6c61 6249 6e70  from the SlabInp
+00000410: 7574 2e69 6e20 6669 6c65 3a0a 0a20 2020  ut.in file:..   
+00000420: 2050 726f 4469 4d6f 2072 756e 0a0a 2020   ProDiMo run..  
+00000430: 2020 5c7c 5f5f 4d6f 6465 6c5f 310a 2020    \|__Model_1.  
+00000440: 2020 2020 2020 5c7c 5f5f 6d6f 6c65 6375        \|__molecu
+00000450: 6c65 5f31 0a0a 2020 2020 2020 2020 5c7c  le_1..        \|
+00000460: 5f5f 6d6f 6c65 6375 6c65 5f32 0a0a 2020  __molecule_2..  
+00000470: 2020 2020 2020 5c7c 5f5f 2e2e 2e0a 0a20        \|__..... 
+00000480: 2020 2020 2020 205c 7c5f 5f6d 6f6c 6563         \|__molec
+00000490: 756c 655f 6e0a 2020 2020 5c7c 5f5f 4d6f  ule_n.    \|__Mo
+000004a0: 6465 6c5f 320a 2020 2020 2020 2020 5c7c  del_2.        \|
+000004b0: 5f5f 6d6f 6c65 6375 6c65 5f31 0a0a 2020  __molecule_1..  
+000004c0: 2020 2020 2020 5c7c 5f5f 6d6f 6c65 6375        \|__molecu
+000004d0: 6c65 5f32 0a0a 2020 2020 2020 2020 5c7c  le_2..        \|
+000004e0: 5f5f 2e2e 2e0a 0a20 2020 2020 2020 205c  __.....        \
+000004f0: 7c5f 5f6d 6f6c 6563 756c 655f 6e0a 2020  |__molecule_n.  
+00000500: 2020 5c7c 5f5f 2e2e 2e0a 2020 2020 2020    \|__....      
+00000510: 2020 5c7c 5f5f 2e2e 2e0a 0a20 2020 2020    \|__.....     
+00000520: 2020 205c 7c5f 5f2e 2e2e 0a0a 2020 2020     \|__.....    
+00000530: 2020 2020 5c7c 5f5f 2e2e 2e0a 2020 2020      \|__....    
+00000540: 5c7c 5f5f 4d6f 6465 6c5f 6e0a 2020 2020  \|__Model_n.    
+00000550: 2020 2020 5c7c 5f5f 6d6f 6c65 6375 6c65      \|__molecule
+00000560: 5f31 0a0a 2020 2020 2020 2020 5c7c 5f5f  _1..        \|__
+00000570: 6d6f 6c65 6375 6c65 5f32 0a0a 2020 2020  molecule_2..    
+00000580: 2020 2020 5c7c 5f5f 2e2e 2e0a 0a20 2020      \|__.....   
+00000590: 2020 2020 205c 7c5f 5f6d 6f6c 6563 756c       \|__molecul
+000005a0: 655f 6e0a 0a20 2020 2044 6174 6120 7374  e_n..    Data st
+000005b0: 7275 6374 7572 6520 746f 2068 6f6c 6420  ructure to hold 
+000005c0: 7468 6520 636f 7272 6573 706f 6e64 696e  the correspondin
+000005d0: 6720 736c 6162 206d 6f64 656c 206f 7574  g slab model out
+000005e0: 7075 740a 2020 2020 736c 6162 5f64 6174  put.    slab_dat
+000005f0: 610a 0a20 2020 205c 7c5f 6469 7265 6374  a..    \|_direct
+00000600: 6f72 790a 0a20 2020 205c 7c5f 6d6f 6465  ory..    \|_mode
+00000610: 6c73 0a20 2020 2020 2020 205c 7c5f 5f6d  ls.        \|__m
+00000620: 6f64 656c 5f31 2028 7479 7065 3a73 6c61  odel_1 (type:sla
+00000630: 6229 0a20 2020 2020 2020 2020 2020 5c7c  b).           \|
+00000640: 5f5f 7072 6f64 696d 6f5f 4d6f 6465 6c5f  __prodimo_Model_
+00000650: 315f 6d6f 6c65 6375 6c65 5f31 0a20 2020  1_molecule_1.   
+00000660: 2020 2020 205c 7c5f 5f6d 6f64 656c 5f32       \|__model_2
+00000670: 2028 7479 7065 3a73 6c61 6229 0a20 2020   (type:slab).   
+00000680: 2020 2020 2020 2020 5c7c 5f5f 7072 6f64          \|__prod
+00000690: 696d 6f5f 4d6f 6465 6c5f 315f 6d6f 6c65  imo_Model_1_mole
+000006a0: 6375 6c65 5f32 0a20 2020 2020 2020 205c  cule_2.        \
+000006b0: 7c5f 5f6d 6f64 656c 5f2e 2e2e 2028 7479  |__model_... (ty
+000006c0: 7065 3a73 6c61 6229 0a20 2020 2020 2020  pe:slab).       
+000006d0: 2020 2020 5c7c 5f5f 2e2e 2e0a 2020 2020      \|__....    
+000006e0: 2020 2020 5c7c 5f5f 6d6f 6465 6c5f 6e20      \|__model_n 
+000006f0: 2874 7970 653a 736c 6162 290a 2020 2020  (type:slab).    
+00000700: 2020 2020 2020 205c 7c5f 5f70 726f 6469         \|__prodi
+00000710: 6d6f 5f4d 6f64 656c 5f32 5f6d 6f6c 6563  mo_Model_2_molec
+00000720: 756c 655f 6e0a 2020 2020 2020 2020 5c7c  ule_n.        \|
+00000730: 5f5f 6d6f 6465 6c5f 6e2b 3120 2874 7970  __model_n+1 (typ
+00000740: 653a 736c 6162 290a 2020 2020 2020 2020  e:slab).        
+00000750: 2020 205c 7c5f 5f70 726f 6469 6d6f 5f4d     \|__prodimo_M
+00000760: 6f64 656c 5f32 5f6d 6f6c 6563 756c 655f  odel_2_molecule_
+00000770: 310a 2020 2020 2020 2020 5c7c 5f5f 6d6f  1.        \|__mo
+00000780: 6465 6c5f 6e2b 3220 2874 7970 653a 736c  del_n+2 (type:sl
+00000790: 6162 290a 2020 2020 2020 2020 2020 205c  ab).           \
+000007a0: 7c5f 5f70 726f 6469 6d6f 5f4d 6f64 656c  |__prodimo_Model
+000007b0: 5f32 5f6d 6f6c 6563 756c 655f 320a 2020  _2_molecule_2.  
+000007c0: 2020 2020 2020 5c7c 5f5f 6d6f 6465 6c5f        \|__model_
+000007d0: 2e2e 2e20 2874 7970 653a 736c 6162 290a  ... (type:slab).
+000007e0: 2020 2020 2020 2020 2020 205c 7c5f 5f2e             \|__.
+000007f0: 2e2e 0a20 2020 2020 2020 205c 7c5f 5f6d  ...        \|__m
+00000800: 6f64 656c 5f6e 2b6e 2028 7479 7065 3a73  odel_n+n (type:s
+00000810: 6c61 6229 0a20 2020 2020 2020 2020 2020  lab).           
+00000820: 5c7c 5f5f 7072 6f64 696d 6f5f 6d6f 6465  \|__prodimo_mode
+00000830: 6c5f 325f 6d6f 6c65 6375 6c65 5f6e 0a20  l_2_molecule_n. 
+00000840: 2020 2020 2020 205c 7c5f 5f6d 6f64 656c         \|__model
+00000850: 5f2e 2e2e 2028 7479 7065 3a73 6c61 6229  _... (type:slab)
+00000860: 0a20 2020 2020 2020 2020 2020 5c7c 5f5f  .           \|__
+00000870: 2e2e 2e0a 2020 2020 2222 220a 0a20 2020  ....    """..   
+00000880: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00000890: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
+000008a0: 662e 5f6e 6d6f 6465 6c73 3d30 0a20 2020  f._nmodels=0.   
+000008b0: 2020 2020 2022 2222 2069 6e74 6567 6572       """ integer
+000008c0: 203a 0a20 2020 2020 2020 206e 756d 6265   :.        numbe
+000008d0: 7220 6f66 206d 6f64 656c 732e 0a20 2020  r of models..   
+000008e0: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+000008f0: 2020 7365 6c66 2e64 6972 6563 746f 7279    self.directory
+00000900: 3d4e 6f6e 650a 2020 2020 2020 2020 2222  =None.        ""
+00000910: 2220 7374 7269 6e67 203a 0a20 2020 2020  " string :.     
+00000920: 2020 2054 6865 2064 6972 6563 746f 7279     The directory
+00000930: 2066 726f 6d20 7768 6963 6820 7468 6520   from which the 
+00000940: 6d6f 6465 6c20 7761 7320 7265 6164 2e0a  model was read..
+00000950: 2020 2020 2020 2020 4361 6e20 6265 2061          Can be a
+00000960: 2072 656c 6174 6976 6520 7061 7468 2e0a   relative path..
+00000970: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00000980: 2020 2020 7365 6c66 2e6d 6f64 656c 733d      self.models=
+00000990: 5b5d 0a20 2020 2020 2020 2022 2222 206c  [].        """ l
+000009a0: 6973 7420 3a0a 2020 2020 2020 2020 5468  ist :.        Th
+000009b0: 6520 6c69 7374 2063 6f6e 7461 696e 696e  e list containin
+000009c0: 6720 7468 6520 6d6f 6465 6c73 0a20 2020  g the models.   
+000009d0: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+000009e0: 2020 7365 6c66 2e5f 7370 6563 6965 735f    self._species_
+000009f0: 6e75 6d62 6572 3d4e 6f6e 650a 2020 2020  number=None.    
+00000a00: 2020 2020 2222 2220 6c69 7374 3a0a 2020      """ list:.  
+00000a10: 2020 2020 2020 4974 2073 746f 7265 7320        It stores 
+00000a20: 7468 6520 7370 6563 6965 7320 6e75 6d62  the species numb
+00000a30: 6572 2061 6363 6f72 6469 6e67 2074 6f20  er according to 
+00000a40: 536c 6162 496e 7075 742e 696e 206f 6620  SlabInput.in of 
+00000a50: 616c 6c20 6d6f 6465 6c73 0a20 2020 2020  all models.     
+00000a60: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+00000a70: 7365 6c66 2e5f 6d6f 6465 6c5f 6e75 6d62  self._model_numb
+00000a80: 6572 3d4e 6f6e 650a 2020 2020 2020 2020  er=None.        
+00000a90: 2222 2220 6c69 7374 3a0a 2020 2020 2020  """ list:.      
+00000aa0: 2020 4974 2073 746f 7265 7320 7468 6520    It stores the 
+00000ab0: 6d6f 6465 6c20 6e75 6d62 6572 2061 6363  model number acc
+00000ac0: 6f72 6469 6e67 2074 6f20 536c 6162 496e  ording to SlabIn
+00000ad0: 7075 742e 696e 206f 6620 616c 6c20 6d6f  put.in of all mo
+00000ae0: 6465 6c73 0a20 2020 2020 2020 2022 2222  dels.        """
+00000af0: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+00000b00: 4e48 3d4e 6f6e 650a 2020 2020 2020 2020  NH=None.        
+00000b10: 2222 2220 6c69 7374 3a0a 2020 2020 2020  """ list:.      
+00000b20: 2020 4974 2073 746f 7265 7320 7468 6520    It stores the 
+00000b30: 746f 7461 6c20 6761 7320 6465 6e73 6974  total gas densit
+00000b40: 6965 7320 6f66 2061 6c6c 206d 6f64 656c  ies of all model
+00000b50: 730a 2020 2020 2020 2020 2222 220a 0a20  s.        """.. 
+00000b60: 2020 2020 2020 2073 656c 662e 5f6e 436f         self._nCo
+00000b70: 6c6c 3d4e 6f6e 650a 2020 2020 2020 2020  ll=None.        
+00000b80: 2222 2220 6c69 7374 3a0a 2020 2020 2020  """ list:.      
+00000b90: 2020 4974 2073 746f 7265 7320 7468 6520    It stores the 
+00000ba0: 746f 7461 6c20 636f 6c6c 6973 696f 6e20  total collision 
+00000bb0: 7061 7274 6e65 7220 6162 756e 6461 6e63  partner abundanc
+00000bc0: 6520 6f66 2061 6c6c 206d 6f64 656c 730a  e of all models.
+00000bd0: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+00000be0: 2020 2020 2073 656c 662e 5f6e 653d 4e6f       self._ne=No
+00000bf0: 6e65 0a20 2020 2020 2020 2022 2222 206c  ne.        """ l
+00000c00: 6973 743a 0a20 2020 2020 2020 2049 7420  ist:.        It 
+00000c10: 7374 6f72 6573 2074 6865 2065 6c65 6374  stores the elect
+00000c20: 726f 6e20 6162 756e 6461 6e63 6520 6f66  ron abundance of
+00000c30: 2061 6c6c 206d 6f64 656c 730a 2020 2020   all models.    
+00000c40: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+00000c50: 2073 656c 662e 5f6e 4865 3d4e 6f6e 650a   self._nHe=None.
+00000c60: 2020 2020 2020 2020 2222 2220 6c69 7374          """ list
+00000c70: 3a0a 2020 2020 2020 2020 4974 2073 746f  :.        It sto
+00000c80: 7265 7320 7468 6520 4865 2061 6275 6e64  res the He abund
+00000c90: 616e 6365 206f 6620 616c 6c20 6d6f 6465  ance of all mode
+00000ca0: 6c73 0a20 2020 2020 2020 2022 2222 0a0a  ls.        """..
+00000cb0: 2020 2020 2020 2020 7365 6c66 2e5f 6e48          self._nH
+00000cc0: 4949 3d4e 6f6e 650a 2020 2020 2020 2020  II=None.        
+00000cd0: 2222 2220 6c69 7374 3a0a 2020 2020 2020  """ list:.      
+00000ce0: 2020 4974 2073 746f 7265 7320 7468 6520    It stores the 
+00000cf0: 4849 4920 6162 756e 6461 6e63 6520 6f66  HII abundance of
+00000d00: 2061 6c6c 206d 6f64 656c 730a 2020 2020   all models.    
+00000d10: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+00000d20: 2073 656c 662e 5f6e 4849 3d4e 6f6e 650a   self._nHI=None.
+00000d30: 2020 2020 2020 2020 2222 2220 6c69 7374          """ list
+00000d40: 3a0a 2020 2020 2020 2020 4974 2073 746f  :.        It sto
+00000d50: 7265 7320 7468 6520 4849 2061 6275 6e64  res the HI abund
+00000d60: 616e 6365 206f 6620 616c 6c20 6d6f 6465  ance of all mode
+00000d70: 6c73 0a20 2020 2020 2020 2022 2222 0a0a  ls.        """..
+00000d80: 2020 2020 2020 2020 7365 6c66 2e5f 6e48          self._nH
+00000d90: 323d 4e6f 6e65 0a20 2020 2020 2020 2022  2=None.        "
+00000da0: 2222 206c 6973 743a 0a20 2020 2020 2020  "" list:.       
+00000db0: 2049 7420 7374 6f72 6573 2074 6865 206d   It stores the m
+00000dc0: 6f6c 6563 756c 6172 2068 7964 726f 6765  olecular hydroge
+00000dd0: 6e20 6162 756e 6461 6e63 6520 6f66 2061  n abundance of a
+00000de0: 6c6c 206d 6f64 656c 730a 2020 2020 2020  ll models.      
+00000df0: 2020 2222 220a 0a20 2020 2020 2020 2073    """..        s
+00000e00: 656c 662e 5f64 7573 745f 746f 5f67 6173  elf._dust_to_gas
+00000e10: 3d4e 6f6e 650a 2020 2020 2020 2020 2222  =None.        ""
+00000e20: 2220 6c69 7374 3a0a 2020 2020 2020 2020  " list:.        
+00000e30: 4974 2073 746f 7265 7320 7468 6520 6475  It stores the du
+00000e40: 7374 2074 6f20 6761 7320 7261 7469 6f20  st to gas ratio 
+00000e50: 6f66 2061 6c6c 206d 6f64 656c 730a 2020  of all models.  
+00000e60: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+00000e70: 2020 2073 656c 662e 5f76 7475 7262 3d4e     self._vturb=N
+00000e80: 6f6e 650a 2020 2020 2020 2020 2222 2220  one.        """ 
+00000e90: 6c69 7374 3a0a 2020 2020 2020 2020 4974  list:.        It
+00000ea0: 2073 746f 7265 7320 7468 6520 7475 7262   stores the turb
+00000eb0: 756c 656e 7420 6272 6f61 6465 6e69 6e67  ulent broadening
+00000ec0: 206f 6620 616c 6c20 6d6f 6465 6c73 0a20   of all models. 
+00000ed0: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
+00000ee0: 2020 2020 7365 6c66 2e5f 5467 3d4e 6f6e      self._Tg=Non
+00000ef0: 650a 2020 2020 2020 2020 2222 2220 6c69  e.        """ li
+00000f00: 7374 3a0a 2020 2020 2020 2020 4974 2073  st:.        It s
+00000f10: 746f 7265 7320 7468 6520 6761 7320 7465  tores the gas te
+00000f20: 6d70 6572 6174 7572 6573 206f 6620 616c  mperatures of al
+00000f30: 6c20 6d6f 6465 6c73 0a20 2020 2020 2020  l models.       
+00000f40: 2022 2222 0a0a 2020 2020 2020 2020 7365   """..        se
+00000f50: 6c66 2e5f 5464 3d4e 6f6e 650a 2020 2020  lf._Td=None.    
+00000f60: 2020 2020 2222 2220 6c69 7374 3a0a 2020      """ list:.  
+00000f70: 2020 2020 2020 4974 2073 746f 7265 7320        It stores 
+00000f80: 7468 6520 6475 7374 2074 656d 7065 7261  the dust tempera
+00000f90: 7475 7265 7320 6f66 2061 6c6c 206d 6f64  tures of all mod
+00000fa0: 656c 730a 2020 2020 2020 2020 2222 220a  els.        """.
+00000fb0: 0a20 2020 2020 2020 2073 656c 662e 5f73  .        self._s
+00000fc0: 7065 6369 6573 5f6e 616d 653d 4e6f 6e65  pecies_name=None
 00000fd0: 0a20 2020 2020 2020 2022 2222 206c 6973  .        """ lis
 00000fe0: 743a 0a20 2020 2020 2020 2049 7420 7374  t:.        It st
-00000ff0: 6f72 6573 2074 6865 206e 756d 6265 7220  ores the number 
-00001000: 6f66 206c 6576 656c 7320 6f66 2061 6c6c  of levels of all
-00001010: 206d 6f64 656c 730a 2020 2020 2020 2020   models.        
-00001020: 2222 220a 0a20 2020 2020 2020 2073 656c  """..        sel
-00001030: 662e 5f6e 6c69 6e65 733d 4e6f 6e65 0a20  f._nlines=None. 
-00001040: 2020 2020 2020 2022 2222 206c 6973 743a         """ list:
-00001050: 0a20 2020 2020 2020 2049 7420 7374 6f72  .        It stor
-00001060: 6573 2074 6865 206e 756d 6265 7220 6f66  es the number of
-00001070: 206c 696e 6573 206f 6620 616c 6c20 6d6f   lines of all mo
-00001080: 6465 6c73 0a20 2020 2020 2020 2022 2222  dels.        """
-00001090: 0a20 2020 2020 2020 2073 656c 662e 5f6c  .        self._l
-000010a0: 696e 6564 6174 613d 4e6f 6e65 0a20 2020  inedata=None.   
-000010b0: 2020 2020 2022 2222 206c 6973 743a 0a20       """ list:. 
-000010c0: 2020 2020 2020 2049 7420 7374 6f72 6573         It stores
-000010d0: 2074 6865 206c 696e 6520 6461 7461 206f   the line data o
-000010e0: 6620 616c 6c20 6d6f 6465 6c73 0a20 2020  f all models.   
-000010f0: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-00001100: 2020 7365 6c66 2e5f 6c65 7665 6c64 6174    self._leveldat
-00001110: 613d 4e6f 6e65 0a20 2020 2020 2020 2022  a=None.        "
-00001120: 2222 206c 6973 743a 0a20 2020 2020 2020  "" list:.       
-00001130: 2049 7420 7374 6f72 6573 2074 6865 206c   It stores the l
-00001140: 6576 656c 2064 6174 6120 6f66 2061 6c6c  evel data of all
-00001150: 206d 6f64 656c 730a 2020 2020 2020 2020   models.        
-00001160: 2222 220a 0a20 2020 2020 2020 2073 656c  """..        sel
-00001170: 662e 5f63 6f6e 7657 6176 656c 656e 6774  f._convWavelengt
-00001180: 683d 4e6f 6e65 0a20 2020 2020 2020 2022  h=None.        "
-00001190: 2222 206c 6973 743a 0a20 2020 2020 2020  "" list:.       
-000011a0: 2049 7420 7374 6f72 6573 2074 6865 2063   It stores the c
-000011b0: 6f6e 766f 6c76 6564 2077 6176 656c 656e  onvolved wavelen
-000011c0: 6774 6820 6772 6964 206f 6620 616c 6c20  gth grid of all 
-000011d0: 6d6f 6465 6c73 0a20 2020 2020 2020 2022  models.        "
-000011e0: 2222 0a0a 2020 2020 2020 2020 7365 6c66  ""..        self
-000011f0: 2e5f 636f 6e76 4c54 4566 6c75 783d 4e6f  ._convLTEflux=No
-00001200: 6e65 0a20 2020 2020 2020 2022 2222 206c  ne.        """ l
-00001210: 6973 743a 0a20 2020 2020 2020 2049 7420  ist:.        It 
-00001220: 7374 6f72 6573 2074 6865 2063 6f6e 766f  stores the convo
-00001230: 6c76 6564 204c 5445 2066 6c75 7820 6f66  lved LTE flux of
-00001240: 2061 6c6c 206d 6f64 656c 730a 2020 2020   all models.    
-00001250: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-00001260: 2073 656c 662e 5f63 6f6e 764e 4c54 4566   self._convNLTEf
-00001270: 6c75 783d 4e6f 6e65 0a20 2020 2020 2020  lux=None.       
-00001280: 2022 2222 206c 6973 743a 0a20 2020 2020   """ list:.     
-00001290: 2020 2049 7420 7374 6f72 6573 2074 6865     It stores the
-000012a0: 2063 6f6e 766f 6c76 6564 204e 4c54 4520   convolved NLTE 
-000012b0: 666c 7578 206f 6620 616c 6c20 6d6f 6465  flux of all mode
-000012c0: 6c73 0a20 2020 2020 2020 2022 2222 0a0a  ls.        """..
-000012d0: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
-000012e0: 6e76 5479 7065 3d4e 6f6e 650a 2020 2020  nvType=None.    
-000012f0: 2020 2020 2222 2220 6c69 7374 3a0a 2020      """ list:.  
-00001300: 2020 2020 2020 4974 2073 746f 7265 7320        It stores 
-00001310: 7468 6520 636f 6e76 6f6c 7574 696f 6e20  the convolution 
-00001320: 7479 7065 206f 6620 616c 6c20 6d6f 6465  type of all mode
-00001330: 6c73 0a20 2020 2020 2020 2022 2222 0a0a  ls.        """..
-00001340: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
-00001350: 6e76 523d 4e6f 6e65 0a20 2020 2020 2020  nvR=None.       
-00001360: 2022 2222 206c 6973 743a 0a20 2020 2020   """ list:.     
-00001370: 2020 2049 7420 7374 6f72 6573 2074 6865     It stores the
-00001380: 2063 6f6e 766f 6c76 6564 2072 6573 6f6c   convolved resol
-00001390: 7669 6e67 2070 6f77 6572 2052 206f 6620  ving power R of 
-000013a0: 616c 6c20 6d6f 6465 6c73 0a20 2020 2020  all models.     
-000013b0: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
-000013c0: 7365 6c66 2e5f 636f 6e76 4f76 6572 6c61  self._convOverla
-000013d0: 7046 7265 713d 4e6f 6e65 0a20 2020 2020  pFreq=None.     
-000013e0: 2020 2022 2222 206c 6973 743a 0a20 2020     """ list:.   
-000013f0: 2020 2020 2049 7420 7374 6f72 6573 2074       It stores t
-00001400: 6865 2063 6f6e 766f 6c76 6564 2066 7265  he convolved fre
-00001410: 7175 656e 6379 2067 7269 6420 6f66 2061  quency grid of a
-00001420: 6c6c 206c 696e 6520 6f76 6572 6c61 7020  ll line overlap 
-00001430: 6d6f 6465 6c73 0a20 2020 2020 2020 2022  models.        "
-00001440: 2222 0a0a 2020 2020 2020 2020 7365 6c66  ""..        self
-00001450: 2e5f 636f 6e76 4f76 6572 6c61 7057 6176  ._convOverlapWav
-00001460: 3d4e 6f6e 650a 2020 2020 2020 2020 2222  =None.        ""
-00001470: 2220 6c69 7374 3a0a 2020 2020 2020 2020  " list:.        
-00001480: 4974 2073 746f 7265 7320 7468 6520 636f  It stores the co
-00001490: 6e76 6f6c 7665 6420 7761 7665 6c65 6e67  nvolved waveleng
-000014a0: 7468 2067 7269 6420 6f66 2061 6c6c 206c  th grid of all l
-000014b0: 696e 6520 6f76 6572 6c61 7020 6d6f 6465  ine overlap mode
-000014c0: 6c73 0a20 2020 2020 2020 2022 2222 0a0a  ls.        """..
-000014d0: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
-000014e0: 6e76 4f76 6572 6c61 704c 5445 666c 7578  nvOverlapLTEflux
-000014f0: 3d4e 6f6e 650a 2020 2020 2020 2020 2222  =None.        ""
-00001500: 2220 6c69 7374 3a0a 2020 2020 2020 2020  " list:.        
-00001510: 4974 2073 746f 7265 7320 7468 6520 636f  It stores the co
-00001520: 6e76 6f6c 7665 6420 4c54 4520 666c 7578  nvolved LTE flux
-00001530: 206f 6620 616c 6c20 6c69 6e65 206f 7665   of all line ove
-00001540: 726c 6170 206d 6f64 656c 730a 2020 2020  rlap models.    
-00001550: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-00001560: 2073 656c 662e 5f63 6f6e 764f 7665 726c   self._convOverl
-00001570: 6170 4e4c 5445 666c 7578 3d4e 6f6e 650a  apNLTEflux=None.
-00001580: 2020 2020 2020 2020 2222 2220 6c69 7374          """ list
-00001590: 3a0a 2020 2020 2020 2020 4974 2073 746f  :.        It sto
-000015a0: 7265 7320 7468 6520 636f 6e76 6f6c 7665  res the convolve
-000015b0: 6420 4e4c 5445 2066 6c75 7820 6f66 2061  d NLTE flux of a
-000015c0: 6c6c 206c 696e 6520 6f76 6572 6c61 7020  ll line overlap 
-000015d0: 6d6f 6465 6c73 0a20 2020 2020 2020 2022  models.        "
-000015e0: 2222 0a0a 2020 2020 2020 2020 7365 6c66  ""..        self
-000015f0: 2e5f 6f76 6572 6c61 7046 7265 713d 4e6f  ._overlapFreq=No
-00001600: 6e65 0a20 2020 2020 2020 2022 2222 206c  ne.        """ l
-00001610: 6973 743a 0a20 2020 2020 2020 2049 7420  ist:.        It 
-00001620: 7374 6f72 6573 2074 6865 2066 7265 7175  stores the frequ
-00001630: 656e 6379 2067 7269 6420 6f66 2061 6c6c  ency grid of all
-00001640: 206c 696e 6520 6f76 6572 6c61 7020 6d6f   line overlap mo
-00001650: 6465 6c73 0a20 2020 2020 2020 2022 2222  dels.        """
-00001660: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-00001670: 6f76 6572 6c61 704c 5445 3d4e 6f6e 650a  overlapLTE=None.
-00001680: 2020 2020 2020 2020 2222 2220 6c69 7374          """ list
-00001690: 3a0a 2020 2020 2020 2020 4974 2073 746f  :.        It sto
-000016a0: 7265 7320 7468 6520 636f 6e76 6f6c 7665  res the convolve
-000016b0: 6420 4c54 4520 666c 7578 206f 6620 616c  d LTE flux of al
-000016c0: 6c20 6c69 6e65 206f 7665 726c 6170 206d  l line overlap m
-000016d0: 6f64 656c 730a 2020 2020 2020 2020 2222  odels.        ""
-000016e0: 220a 0a20 2020 2020 2020 2073 656c 662e  "..        self.
-000016f0: 5f6f 7665 726c 6170 4e4c 5445 3d4e 6f6e  _overlapNLTE=Non
-00001700: 650a 2020 2020 2020 2020 2222 2220 6c69  e.        """ li
-00001710: 7374 3a0a 2020 2020 2020 2020 4974 2073  st:.        It s
-00001720: 746f 7265 7320 7468 6520 636f 6e76 6f6c  tores the convol
-00001730: 7665 6420 4e4c 5445 2066 6c75 7820 6f66  ved NLTE flux of
-00001740: 2061 6c6c 206c 696e 6520 6f76 6572 6c61   all line overla
-00001750: 7020 6d6f 6465 6c73 0a20 2020 2020 2020  p models.       
-00001760: 2022 2222 0a0a 2020 2020 2020 2020 7365   """..        se
-00001770: 6c66 2e5f 6f76 6572 6c61 7054 6175 4c54  lf._overlapTauLT
-00001780: 453d 4e6f 6e65 0a20 2020 2020 2020 2022  E=None.        "
-00001790: 2222 206c 6973 743a 0a20 2020 2020 2020  "" list:.       
-000017a0: 2049 7420 7374 6f72 6573 2074 6865 2063   It stores the c
-000017b0: 6f6e 766f 6c76 6564 204c 5445 206f 7074  onvolved LTE opt
-000017c0: 6963 616c 2064 6570 7468 7320 6f66 2061  ical depths of a
-000017d0: 6c6c 206c 696e 6520 6f76 6572 6c61 7020  ll line overlap 
-000017e0: 6d6f 6465 6c73 0a20 2020 2020 2020 2022  models.        "
-000017f0: 2222 0a0a 2020 2020 2020 2020 7365 6c66  ""..        self
-00001800: 2e5f 6f76 6572 6c61 7054 6175 4e4c 5445  ._overlapTauNLTE
-00001810: 3d4e 6f6e 650a 2020 2020 2020 2020 2222  =None.        ""
-00001820: 2220 6c69 7374 3a0a 2020 2020 2020 2020  " list:.        
-00001830: 4974 2073 746f 7265 7320 7468 6520 636f  It stores the co
-00001840: 6e76 6f6c 7665 6420 4e4c 5445 206f 7074  nvolved NLTE opt
-00001850: 6963 616c 2064 6570 7468 7320 6f66 2061  ical depths of a
-00001860: 6c6c 206c 696e 6520 6f76 6572 6c61 7020  ll line overlap 
-00001870: 6d6f 6465 6c73 0a20 2020 2020 2020 2022  models.        "
-00001880: 2222 0a0a 2020 2020 2020 2020 7365 6c66  ""..        self
-00001890: 2e5f 6f76 6572 6c61 7052 3d4e 6f6e 650a  ._overlapR=None.
-000018a0: 2020 2020 2020 2020 2222 2220 6c69 7374          """ list
-000018b0: 3a0a 2020 2020 2020 2020 4974 2073 746f  :.        It sto
-000018c0: 7265 7320 7468 6520 7265 736f 6c76 696e  res the resolvin
-000018d0: 6720 706f 7765 7220 5220 6f66 2061 6c6c  g power R of all
-000018e0: 206c 696e 6520 6f76 6572 6c61 7020 6d6f   line overlap mo
-000018f0: 6465 6c73 0a20 2020 2020 2020 2022 2222  dels.        """
-00001900: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-00001910: 636f 6e76 4f76 6572 6c61 7052 3d4e 6f6e  convOverlapR=Non
-00001920: 650a 2020 2020 2020 2020 2222 2220 6c69  e.        """ li
-00001930: 7374 3a0a 2020 2020 2020 2020 4974 2073  st:.        It s
-00001940: 746f 7265 7320 7468 6520 636f 6e76 6f6c  tores the convol
-00001950: 7665 6420 7265 736f 6c76 696e 6720 706f  ved resolving po
-00001960: 7765 7220 5220 6f66 2061 6c6c 206c 696e  wer R of all lin
-00001970: 6520 6f76 6572 6c61 7020 6d6f 6465 6c73  e overlap models
-00001980: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
-00001990: 2020 6465 6620 5f5f 7374 725f 5f28 7365    def __str__(se
-000019a0: 6c66 293a 0a20 2020 2020 2020 206f 7574  lf):.        out
-000019b0: 7075 743d 2249 6e66 6f3a 205c 6e22 0a20  put="Info: \n". 
-000019c0: 2020 2020 2020 206f 7574 7075 742b 3d22         output+="
-000019d0: 5c6e 204e 4d6f 6465 6c73 3a20 220a 2020  \n NModels: ".  
-000019e0: 2020 2020 2020 6f75 7470 7574 2b3d 7374        output+=st
-000019f0: 7228 7365 6c66 2e6e 6d6f 6465 6c73 290a  r(self.nmodels).
-00001a00: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-00001a10: 7461 6e63 6528 7365 6c66 2e64 6972 6563  tance(self.direc
-00001a20: 746f 7279 2c6c 6973 7429 3a0a 2020 2020  tory,list):.    
-00001a30: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00001a40: 2073 656c 662e 6469 7265 6374 6f72 793a   self.directory:
-00001a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001a60: 206f 7574 7075 742b 3d22 5c6e 5c6e 2044   output+="\n\n D
-00001a70: 6972 6563 746f 7279 3a20 222b 690a 2020  irectory: "+i.  
-00001a80: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00001a90: 2020 2020 2020 2020 6f75 7470 7574 2b3d          output+=
-00001aa0: 225c 6e5c 6e20 4469 7265 6374 6f72 793a  "\n\n Directory:
-00001ab0: 2022 2b73 656c 662e 6469 7265 6374 6f72   "+self.director
-00001ac0: 790a 2020 2020 2020 2020 7265 7475 726e  y.        return
-00001ad0: 206f 7574 7075 740a 0a20 2020 2064 6566   output..    def
-00001ae0: 2073 686f 7728 7365 6c66 293a 0a20 2020   show(self):.   
-00001af0: 2020 2020 2070 7269 6e74 2873 656c 6629       print(self)
-00001b00: 0a20 2020 2020 2020 2066 6f72 2069 2069  .        for i i
-00001b10: 6e20 7261 6e67 6528 7365 6c66 2e6e 6d6f  n range(self.nmo
-00001b20: 6465 6c73 293a 0a20 2020 2020 2020 2020  dels):.         
-00001b30: 2020 2073 656c 662e 6d6f 6465 6c73 5b69     self.models[i
-00001b40: 5d2e 7368 6f77 2829 0a20 2020 2020 2020  ].show().       
-00001b50: 2020 2020 2070 7269 6e74 2827 5c6e 2729       print('\n')
-00001b60: 0a0a 2020 2020 6465 6620 6164 645f 6d6f  ..    def add_mo
-00001b70: 6465 6c28 7365 6c66 2c6d 6f64 656c 5f64  del(self,model_d
-00001b80: 6174 6129 3a0a 2020 2020 2020 2020 6966  ata):.        if
-00001b90: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
-00001ba0: 6d6f 6465 6c5f 6461 7461 2c73 6c61 6229  model_data,slab)
-00001bb0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00001bc0: 6973 6520 5479 7065 4572 726f 7228 2770  ise TypeError('p
-00001bd0: 6174 6820 6d75 7374 2062 6520 6f66 2063  ath must be of c
-00001be0: 6c61 7373 3a6d 6f64 656c 2729 0a20 2020  lass:model').   
-00001bf0: 2020 2020 2073 656c 662e 6d6f 6465 6c73       self.models
-00001c00: 2e61 7070 656e 6428 6d6f 6465 6c5f 6461  .append(model_da
-00001c10: 7461 290a 0a20 2020 2064 6566 2072 656d  ta)..    def rem
-00001c20: 6f76 655f 6d6f 6465 6c28 7365 6c66 2c69  ove_model(self,i
-00001c30: 6e64 6578 293a 0a20 2020 2020 2020 2069  ndex):.        i
-00001c40: 6620 696e 6465 783c 303a 0a20 2020 2020  f index<0:.     
-00001c50: 2020 2020 2020 2069 6e64 6578 2b3d 7365         index+=se
-00001c60: 6c66 2e6e 6d6f 6465 6c73 0a20 2020 2020  lf.nmodels.     
-00001c70: 2020 2069 6620 696e 6465 782b 313e 7365     if index+1>se
-00001c80: 6c66 2e6e 6d6f 6465 6c73 206f 7220 696e  lf.nmodels or in
-00001c90: 6465 783c 303a 0a20 2020 2020 2020 2020  dex<0:.         
-00001ca0: 2020 2072 6169 7365 2049 6e64 6578 4572     raise IndexEr
-00001cb0: 726f 7228 2749 6e64 6578 206f 7574 206f  ror('Index out o
-00001cc0: 6620 7261 6e67 6527 290a 2020 2020 2020  f range').      
-00001cd0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00001ce0: 2020 2020 7365 6c66 2e6e 6d6f 6465 6c73      self.nmodels
-00001cf0: 2d3d 310a 2020 2020 2020 2020 2020 2020  -=1.            
-00001d00: 7365 6c66 2e6d 6f64 656c 732e 706f 7028  self.models.pop(
-00001d10: 696e 6465 7829 0a0a 2020 2020 6465 6620  index)..    def 
-00001d20: 5f5f 6765 7469 7465 6d5f 5f28 7365 6c66  __getitem__(self
-00001d30: 2c61 7267 293a 0a20 2020 2020 2020 2072  ,arg):.        r
-00001d40: 6574 5f64 6174 613d 736c 6162 5f64 6174  et_data=slab_dat
-00001d50: 6128 290a 2020 2020 2020 2020 6966 2069  a().        if i
-00001d60: 7369 6e73 7461 6e63 6528 6172 672c 696e  sinstance(arg,in
-00001d70: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-00001d80: 6966 2061 7267 3e73 656c 662e 6e6d 6f64  if arg>self.nmod
-00001d90: 656c 733a 0a20 2020 2020 2020 2020 2020  els:.           
-00001da0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00001db0: 4572 726f 7228 6627 696e 6465 7820 7b61  Error(f'index {a
-00001dc0: 7267 7d20 6772 6561 7465 7220 7468 616e  rg} greater than
-00001dd0: 206e 756d 6265 7220 6f66 206d 6f64 656c   number of model
-00001de0: 7320 7b73 656c 662e 6e6d 6f64 656c 737d  s {self.nmodels}
-00001df0: 2729 0a20 2020 2020 2020 2020 2020 2072  ').            r
-00001e00: 6574 5f64 6174 612e 6164 645f 6d6f 6465  et_data.add_mode
-00001e10: 6c28 7365 6c66 2e6d 6f64 656c 735b 6172  l(self.models[ar
-00001e20: 675d 290a 2020 2020 2020 2020 656c 6966  g]).        elif
-00001e30: 2069 7369 6e73 7461 6e63 6528 6172 672c   isinstance(arg,
-00001e40: 7479 7065 284e 6f6e 6529 293a 0a20 2020  type(None)):.   
-00001e50: 2020 2020 2020 2020 2066 6f72 206d 6f64           for mod
-00001e60: 656c 2069 6e20 7365 6c66 2e6d 6f64 656c  el in self.model
-00001e70: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00001e80: 2020 2072 6574 5f64 6174 612e 6164 645f     ret_data.add_
-00001e90: 6d6f 6465 6c28 6d6f 6465 6c29 0a20 2020  model(model).   
-00001ea0: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
-00001eb0: 616e 6365 2861 7267 2c73 6c69 6365 293a  ance(arg,slice):
-00001ec0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00001ed0: 6973 696e 7374 616e 6365 2861 7267 2e73  isinstance(arg.s
-00001ee0: 7461 7274 2c69 6e74 293a 0a20 2020 2020  tart,int):.     
-00001ef0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-00001f00: 696e 7374 616e 6365 2861 7267 2e73 746f  instance(arg.sto
-00001f10: 702c 696e 7429 3a0a 2020 2020 2020 2020  p,int):.        
-00001f20: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00001f30: 6d6f 6465 6c20 696e 2073 656c 662e 6d6f  model in self.mo
-00001f40: 6465 6c73 5b61 7267 5d3a 0a20 2020 2020  dels[arg]:.     
-00001f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f60: 2020 2072 6574 5f64 6174 612e 6164 645f     ret_data.add_
-00001f70: 6d6f 6465 6c28 6d6f 6465 6c29 0a20 2020  model(model).   
-00001f80: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-00001f90: 6620 6973 696e 7374 616e 6365 2861 7267  f isinstance(arg
-00001fa0: 2e73 746f 702c 7479 7065 284e 6f6e 6529  .stop,type(None)
-00001fb0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00001fc0: 2020 2020 2020 2072 6574 5f64 6174 612e         ret_data.
-00001fd0: 6164 645f 6d6f 6465 6c28 7365 6c66 2e6d  add_model(self.m
-00001fe0: 6f64 656c 735b 6172 672e 7374 6172 745d  odels[arg.start]
-00001ff0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00002000: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00002010: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00002020: 6520 496e 6465 7845 7272 6f72 2866 2773  e IndexError(f's
-00002030: 6c69 6369 6e67 206e 6f74 2075 6e64 6572  licing not under
-00002040: 7374 616e 6461 626c 6520 7b61 7267 7d27  standable {arg}'
-00002050: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-00002060: 6966 2069 7369 6e73 7461 6e63 6528 6172  if isinstance(ar
-00002070: 672e 7374 6172 742c 7374 7229 3a0a 2020  g.start,str):.  
-00002080: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00002090: 2061 7267 2e73 7461 7274 3d3d 2773 7065   arg.start=='spe
-000020a0: 6369 6573 5f6e 616d 6527 3a0a 2020 2020  cies_name':.    
-000020b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020c0: 7365 6c5f 7370 6563 6965 733d 5b5d 0a20  sel_species=[]. 
-000020d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020e0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-000020f0: 2861 7267 2e73 746f 702c 7374 7229 3a0a  (arg.stop,str):.
-00002100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002110: 2020 2020 2020 2020 7365 6c5f 7370 6563          sel_spec
-00002120: 6965 732e 6170 7065 6e64 2861 7267 2e73  ies.append(arg.s
-00002130: 746f 7029 0a20 2020 2020 2020 2020 2020  top).           
-00002140: 2020 2020 2020 2020 2065 6c69 6620 6973           elif is
-00002150: 696e 7374 616e 6365 2861 7267 2e73 746f  instance(arg.sto
-00002160: 702c 6c69 7374 293a 0a20 2020 2020 2020  p,list):.       
-00002170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002180: 2073 656c 5f73 7065 6369 6573 3d61 7267   sel_species=arg
-00002190: 2e73 746f 700a 2020 2020 2020 2020 2020  .stop.          
-000021a0: 2020 2020 2020 2020 2020 6966 206c 656e            if len
-000021b0: 2873 656c 5f73 7065 6369 6573 293e 303a  (sel_species)>0:
-000021c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000021d0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-000021e0: 6e20 7261 6e67 6528 7365 6c66 2e6e 6d6f  n range(self.nmo
-000021f0: 6465 6c73 293a 0a20 2020 2020 2020 2020  dels):.         
-00002200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002210: 2020 2069 6620 7365 6c66 2e6d 6f64 656c     if self.model
-00002220: 735b 695d 2e73 7065 6369 6573 5f6e 616d  s[i].species_nam
-00002230: 6520 696e 2073 656c 5f73 7065 6369 6573  e in sel_species
-00002240: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002260: 2020 7265 745f 6461 7461 2e61 6464 5f6d    ret_data.add_m
-00002270: 6f64 656c 2873 656c 662e 6d6f 6465 6c73  odel(self.models
-00002280: 5b69 5d29 0a20 2020 2020 2020 2020 2020  [i]).           
-00002290: 2020 2020 2065 6c69 6620 6172 672e 7374       elif arg.st
-000022a0: 6172 743d 3d27 7370 6563 6965 735f 6e75  art=='species_nu
-000022b0: 6d62 6572 273a 0a20 2020 2020 2020 2020  mber':.         
-000022c0: 2020 2020 2020 2020 2020 2073 656c 5f73             sel_s
-000022d0: 7065 6369 6573 5f6e 756d 6265 723d 5b5d  pecies_number=[]
-000022e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000022f0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-00002300: 6365 2861 7267 2e73 746f 702c 696e 7429  ce(arg.stop,int)
-00002310: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002320: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
-00002330: 6e73 7461 6e63 6528 6172 672e 7374 6570  nstance(arg.step
-00002340: 2c69 6e74 293a 0a20 2020 2020 2020 2020  ,int):.         
+00000ff0: 6f72 6573 2074 6865 206e 616d 6520 6f66  ores the name of
+00001000: 2074 6865 206d 6f6c 6563 756c 6573 206f   the molecules o
+00001010: 6620 616c 6c20 6d6f 6465 6c73 0a20 2020  f all models.   
+00001020: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+00001030: 2020 7365 6c66 2e5f 7370 6563 6965 735f    self._species_
+00001040: 696e 6465 783d 4e6f 6e65 0a20 2020 2020  index=None.     
+00001050: 2020 2022 2222 206c 6973 743a 0a20 2020     """ list:.   
+00001060: 2020 2020 2049 7420 7374 6f72 6573 2074       It stores t
+00001070: 6865 2050 726f 4469 4d6f 2073 7065 6369  he ProDiMo speci
+00001080: 6573 2069 6e64 6578 206f 6620 616c 6c20  es index of all 
+00001090: 6d6f 6465 6c73 0a20 2020 2020 2020 2022  models.        "
+000010a0: 2222 0a0a 2020 2020 2020 2020 7365 6c66  ""..        self
+000010b0: 2e5f 6162 756e 6461 6e63 653d 4e6f 6e65  ._abundance=None
+000010c0: 0a20 2020 2020 2020 2022 2222 206c 6973  .        """ lis
+000010d0: 743a 0a20 2020 2020 2020 2049 7420 7374  t:.        It st
+000010e0: 6f72 6573 2074 6865 2073 7065 6369 6573  ores the species
+000010f0: 2061 6275 6e64 616e 6365 2061 6363 6f72   abundance accor
+00001100: 6469 6e67 2074 6f20 536c 6162 496e 7075  ding to SlabInpu
+00001110: 742e 696e 206f 6620 616c 6c20 6d6f 6465  t.in of all mode
+00001120: 6c73 0a20 2020 2020 2020 2022 2222 0a0a  ls.        """..
+00001130: 2020 2020 2020 2020 7365 6c66 2e5f 6476          self._dv
+00001140: 3d4e 6f6e 650a 2020 2020 2020 2020 2222  =None.        ""
+00001150: 2220 6c69 7374 3a0a 2020 2020 2020 2020  " list:.        
+00001160: 4974 2073 746f 7265 7320 7468 6520 7665  It stores the ve
+00001170: 6c6f 6369 7479 2077 6964 7468 206f 6620  locity width of 
+00001180: 616c 6c20 6d6f 6465 6c73 0a20 2020 2020  all models.     
+00001190: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+000011a0: 7365 6c66 2e5f 6e6c 6576 656c 733d 4e6f  self._nlevels=No
+000011b0: 6e65 0a20 2020 2020 2020 2022 2222 206c  ne.        """ l
+000011c0: 6973 743a 0a20 2020 2020 2020 2049 7420  ist:.        It 
+000011d0: 7374 6f72 6573 2074 6865 206e 756d 6265  stores the numbe
+000011e0: 7220 6f66 206c 6576 656c 7320 6f66 2061  r of levels of a
+000011f0: 6c6c 206d 6f64 656c 730a 2020 2020 2020  ll models.      
+00001200: 2020 2222 220a 0a20 2020 2020 2020 2073    """..        s
+00001210: 656c 662e 5f6e 6c69 6e65 733d 4e6f 6e65  elf._nlines=None
+00001220: 0a20 2020 2020 2020 2022 2222 206c 6973  .        """ lis
+00001230: 743a 0a20 2020 2020 2020 2049 7420 7374  t:.        It st
+00001240: 6f72 6573 2074 6865 206e 756d 6265 7220  ores the number 
+00001250: 6f66 206c 696e 6573 206f 6620 616c 6c20  of lines of all 
+00001260: 6d6f 6465 6c73 0a20 2020 2020 2020 2022  models.        "
+00001270: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
+00001280: 5f6c 696e 6564 6174 613d 4e6f 6e65 0a20  _linedata=None. 
+00001290: 2020 2020 2020 2022 2222 206c 6973 743a         """ list:
+000012a0: 0a20 2020 2020 2020 2049 7420 7374 6f72  .        It stor
+000012b0: 6573 2074 6865 206c 696e 6520 6461 7461  es the line data
+000012c0: 206f 6620 616c 6c20 6d6f 6465 6c73 0a20   of all models. 
+000012d0: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
+000012e0: 2020 2020 7365 6c66 2e5f 6c65 7665 6c64      self._leveld
+000012f0: 6174 613d 4e6f 6e65 0a20 2020 2020 2020  ata=None.       
+00001300: 2022 2222 206c 6973 743a 0a20 2020 2020   """ list:.     
+00001310: 2020 2049 7420 7374 6f72 6573 2074 6865     It stores the
+00001320: 206c 6576 656c 2064 6174 6120 6f66 2061   level data of a
+00001330: 6c6c 206d 6f64 656c 730a 2020 2020 2020  ll models.      
+00001340: 2020 2222 220a 0a20 2020 2020 2020 2073    """..        s
+00001350: 656c 662e 5f63 6f6e 7657 6176 656c 656e  elf._convWavelen
+00001360: 6774 683d 4e6f 6e65 0a20 2020 2020 2020  gth=None.       
+00001370: 2022 2222 206c 6973 743a 0a20 2020 2020   """ list:.     
+00001380: 2020 2049 7420 7374 6f72 6573 2074 6865     It stores the
+00001390: 2063 6f6e 766f 6c76 6564 2077 6176 656c   convolved wavel
+000013a0: 656e 6774 6820 6772 6964 206f 6620 616c  ength grid of al
+000013b0: 6c20 6d6f 6465 6c73 0a20 2020 2020 2020  l models.       
+000013c0: 2022 2222 0a0a 2020 2020 2020 2020 7365   """..        se
+000013d0: 6c66 2e5f 636f 6e76 4c54 4566 6c75 783d  lf._convLTEflux=
+000013e0: 4e6f 6e65 0a20 2020 2020 2020 2022 2222  None.        """
+000013f0: 206c 6973 743a 0a20 2020 2020 2020 2049   list:.        I
+00001400: 7420 7374 6f72 6573 2074 6865 2063 6f6e  t stores the con
+00001410: 766f 6c76 6564 204c 5445 2066 6c75 7820  volved LTE flux 
+00001420: 6f66 2061 6c6c 206d 6f64 656c 730a 2020  of all models.  
+00001430: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+00001440: 2020 2073 656c 662e 5f63 6f6e 764e 4c54     self._convNLT
+00001450: 4566 6c75 783d 4e6f 6e65 0a20 2020 2020  Eflux=None.     
+00001460: 2020 2022 2222 206c 6973 743a 0a20 2020     """ list:.   
+00001470: 2020 2020 2049 7420 7374 6f72 6573 2074       It stores t
+00001480: 6865 2063 6f6e 766f 6c76 6564 204e 4c54  he convolved NLT
+00001490: 4520 666c 7578 206f 6620 616c 6c20 6d6f  E flux of all mo
+000014a0: 6465 6c73 0a20 2020 2020 2020 2022 2222  dels.        """
+000014b0: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+000014c0: 636f 6e76 5479 7065 3d4e 6f6e 650a 2020  convType=None.  
+000014d0: 2020 2020 2020 2222 2220 6c69 7374 3a0a        """ list:.
+000014e0: 2020 2020 2020 2020 4974 2073 746f 7265          It store
+000014f0: 7320 7468 6520 636f 6e76 6f6c 7574 696f  s the convolutio
+00001500: 6e20 7479 7065 206f 6620 616c 6c20 6d6f  n type of all mo
+00001510: 6465 6c73 0a20 2020 2020 2020 2022 2222  dels.        """
+00001520: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+00001530: 636f 6e76 523d 4e6f 6e65 0a20 2020 2020  convR=None.     
+00001540: 2020 2022 2222 206c 6973 743a 0a20 2020     """ list:.   
+00001550: 2020 2020 2049 7420 7374 6f72 6573 2074       It stores t
+00001560: 6865 2063 6f6e 766f 6c76 6564 2072 6573  he convolved res
+00001570: 6f6c 7669 6e67 2070 6f77 6572 2052 206f  olving power R o
+00001580: 6620 616c 6c20 6d6f 6465 6c73 0a20 2020  f all models.   
+00001590: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+000015a0: 2020 7365 6c66 2e5f 636f 6e76 4f76 6572    self._convOver
+000015b0: 6c61 7046 7265 713d 4e6f 6e65 0a20 2020  lapFreq=None.   
+000015c0: 2020 2020 2022 2222 206c 6973 743a 0a20       """ list:. 
+000015d0: 2020 2020 2020 2049 7420 7374 6f72 6573         It stores
+000015e0: 2074 6865 2063 6f6e 766f 6c76 6564 2066   the convolved f
+000015f0: 7265 7175 656e 6379 2067 7269 6420 6f66  requency grid of
+00001600: 2061 6c6c 206c 696e 6520 6f76 6572 6c61   all line overla
+00001610: 7020 6d6f 6465 6c73 0a20 2020 2020 2020  p models.       
+00001620: 2022 2222 0a0a 2020 2020 2020 2020 7365   """..        se
+00001630: 6c66 2e5f 636f 6e76 4f76 6572 6c61 7057  lf._convOverlapW
+00001640: 6176 3d4e 6f6e 650a 2020 2020 2020 2020  av=None.        
+00001650: 2222 2220 6c69 7374 3a0a 2020 2020 2020  """ list:.      
+00001660: 2020 4974 2073 746f 7265 7320 7468 6520    It stores the 
+00001670: 636f 6e76 6f6c 7665 6420 7761 7665 6c65  convolved wavele
+00001680: 6e67 7468 2067 7269 6420 6f66 2061 6c6c  ngth grid of all
+00001690: 206c 696e 6520 6f76 6572 6c61 7020 6d6f   line overlap mo
+000016a0: 6465 6c73 0a20 2020 2020 2020 2022 2222  dels.        """
+000016b0: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+000016c0: 636f 6e76 4f76 6572 6c61 704c 5445 666c  convOverlapLTEfl
+000016d0: 7578 3d4e 6f6e 650a 2020 2020 2020 2020  ux=None.        
+000016e0: 2222 2220 6c69 7374 3a0a 2020 2020 2020  """ list:.      
+000016f0: 2020 4974 2073 746f 7265 7320 7468 6520    It stores the 
+00001700: 636f 6e76 6f6c 7665 6420 4c54 4520 666c  convolved LTE fl
+00001710: 7578 206f 6620 616c 6c20 6c69 6e65 206f  ux of all line o
+00001720: 7665 726c 6170 206d 6f64 656c 730a 2020  verlap models.  
+00001730: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+00001740: 2020 2073 656c 662e 5f63 6f6e 764f 7665     self._convOve
+00001750: 726c 6170 4e4c 5445 666c 7578 3d4e 6f6e  rlapNLTEflux=Non
+00001760: 650a 2020 2020 2020 2020 2222 2220 6c69  e.        """ li
+00001770: 7374 3a0a 2020 2020 2020 2020 4974 2073  st:.        It s
+00001780: 746f 7265 7320 7468 6520 636f 6e76 6f6c  tores the convol
+00001790: 7665 6420 4e4c 5445 2066 6c75 7820 6f66  ved NLTE flux of
+000017a0: 2061 6c6c 206c 696e 6520 6f76 6572 6c61   all line overla
+000017b0: 7020 6d6f 6465 6c73 0a20 2020 2020 2020  p models.       
+000017c0: 2022 2222 0a0a 2020 2020 2020 2020 7365   """..        se
+000017d0: 6c66 2e5f 6f76 6572 6c61 7046 7265 713d  lf._overlapFreq=
+000017e0: 4e6f 6e65 0a20 2020 2020 2020 2022 2222  None.        """
+000017f0: 206c 6973 743a 0a20 2020 2020 2020 2049   list:.        I
+00001800: 7420 7374 6f72 6573 2074 6865 2066 7265  t stores the fre
+00001810: 7175 656e 6379 2067 7269 6420 6f66 2061  quency grid of a
+00001820: 6c6c 206c 696e 6520 6f76 6572 6c61 7020  ll line overlap 
+00001830: 6d6f 6465 6c73 0a20 2020 2020 2020 2022  models.        "
+00001840: 2222 0a0a 2020 2020 2020 2020 7365 6c66  ""..        self
+00001850: 2e5f 6f76 6572 6c61 704c 5445 3d4e 6f6e  ._overlapLTE=Non
+00001860: 650a 2020 2020 2020 2020 2222 2220 6c69  e.        """ li
+00001870: 7374 3a0a 2020 2020 2020 2020 4974 2073  st:.        It s
+00001880: 746f 7265 7320 7468 6520 636f 6e76 6f6c  tores the convol
+00001890: 7665 6420 4c54 4520 666c 7578 206f 6620  ved LTE flux of 
+000018a0: 616c 6c20 6c69 6e65 206f 7665 726c 6170  all line overlap
+000018b0: 206d 6f64 656c 730a 2020 2020 2020 2020   models.        
+000018c0: 2222 220a 0a20 2020 2020 2020 2073 656c  """..        sel
+000018d0: 662e 5f6f 7665 726c 6170 4e4c 5445 3d4e  f._overlapNLTE=N
+000018e0: 6f6e 650a 2020 2020 2020 2020 2222 2220  one.        """ 
+000018f0: 6c69 7374 3a0a 2020 2020 2020 2020 4974  list:.        It
+00001900: 2073 746f 7265 7320 7468 6520 636f 6e76   stores the conv
+00001910: 6f6c 7665 6420 4e4c 5445 2066 6c75 7820  olved NLTE flux 
+00001920: 6f66 2061 6c6c 206c 696e 6520 6f76 6572  of all line over
+00001930: 6c61 7020 6d6f 6465 6c73 0a20 2020 2020  lap models.     
+00001940: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+00001950: 7365 6c66 2e5f 6f76 6572 6c61 7054 6175  self._overlapTau
+00001960: 4c54 453d 4e6f 6e65 0a20 2020 2020 2020  LTE=None.       
+00001970: 2022 2222 206c 6973 743a 0a20 2020 2020   """ list:.     
+00001980: 2020 2049 7420 7374 6f72 6573 2074 6865     It stores the
+00001990: 2063 6f6e 766f 6c76 6564 204c 5445 206f   convolved LTE o
+000019a0: 7074 6963 616c 2064 6570 7468 7320 6f66  ptical depths of
+000019b0: 2061 6c6c 206c 696e 6520 6f76 6572 6c61   all line overla
+000019c0: 7020 6d6f 6465 6c73 0a20 2020 2020 2020  p models.       
+000019d0: 2022 2222 0a0a 2020 2020 2020 2020 7365   """..        se
+000019e0: 6c66 2e5f 6f76 6572 6c61 7054 6175 4e4c  lf._overlapTauNL
+000019f0: 5445 3d4e 6f6e 650a 2020 2020 2020 2020  TE=None.        
+00001a00: 2222 2220 6c69 7374 3a0a 2020 2020 2020  """ list:.      
+00001a10: 2020 4974 2073 746f 7265 7320 7468 6520    It stores the 
+00001a20: 636f 6e76 6f6c 7665 6420 4e4c 5445 206f  convolved NLTE o
+00001a30: 7074 6963 616c 2064 6570 7468 7320 6f66  ptical depths of
+00001a40: 2061 6c6c 206c 696e 6520 6f76 6572 6c61   all line overla
+00001a50: 7020 6d6f 6465 6c73 0a20 2020 2020 2020  p models.       
+00001a60: 2022 2222 0a0a 2020 2020 2020 2020 7365   """..        se
+00001a70: 6c66 2e5f 6f76 6572 6c61 7052 3d4e 6f6e  lf._overlapR=Non
+00001a80: 650a 2020 2020 2020 2020 2222 2220 6c69  e.        """ li
+00001a90: 7374 3a0a 2020 2020 2020 2020 4974 2073  st:.        It s
+00001aa0: 746f 7265 7320 7468 6520 7265 736f 6c76  tores the resolv
+00001ab0: 696e 6720 706f 7765 7220 5220 6f66 2061  ing power R of a
+00001ac0: 6c6c 206c 696e 6520 6f76 6572 6c61 7020  ll line overlap 
+00001ad0: 6d6f 6465 6c73 0a20 2020 2020 2020 2022  models.        "
+00001ae0: 2222 0a0a 2020 2020 2020 2020 7365 6c66  ""..        self
+00001af0: 2e5f 636f 6e76 4f76 6572 6c61 7052 3d4e  ._convOverlapR=N
+00001b00: 6f6e 650a 2020 2020 2020 2020 2222 2220  one.        """ 
+00001b10: 6c69 7374 3a0a 2020 2020 2020 2020 4974  list:.        It
+00001b20: 2073 746f 7265 7320 7468 6520 636f 6e76   stores the conv
+00001b30: 6f6c 7665 6420 7265 736f 6c76 696e 6720  olved resolving 
+00001b40: 706f 7765 7220 5220 6f66 2061 6c6c 206c  power R of all l
+00001b50: 696e 6520 6f76 6572 6c61 7020 6d6f 6465  ine overlap mode
+00001b60: 6c73 0a20 2020 2020 2020 2022 2222 0a0a  ls.        """..
+00001b70: 2020 2020 6465 6620 5f5f 7374 725f 5f28      def __str__(
+00001b80: 7365 6c66 293a 0a20 2020 2020 2020 206f  self):.        o
+00001b90: 7574 7075 743d 2249 6e66 6f3a 205c 6e22  utput="Info: \n"
+00001ba0: 0a20 2020 2020 2020 206f 7574 7075 742b  .        output+
+00001bb0: 3d22 5c6e 204e 4d6f 6465 6c73 3a20 220a  ="\n NModels: ".
+00001bc0: 2020 2020 2020 2020 6f75 7470 7574 2b3d          output+=
+00001bd0: 7374 7228 7365 6c66 2e6e 6d6f 6465 6c73  str(self.nmodels
+00001be0: 290a 2020 2020 2020 2020 6966 2069 7369  ).        if isi
+00001bf0: 6e73 7461 6e63 6528 7365 6c66 2e64 6972  nstance(self.dir
+00001c00: 6563 746f 7279 2c6c 6973 7429 3a0a 2020  ectory,list):.  
+00001c10: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
+00001c20: 696e 2073 656c 662e 6469 7265 6374 6f72  in self.director
+00001c30: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
+00001c40: 2020 206f 7574 7075 742b 3d22 5c6e 5c6e     output+="\n\n
+00001c50: 2044 6972 6563 746f 7279 3a20 222b 690a   Directory: "+i.
+00001c60: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00001c70: 2020 2020 2020 2020 2020 6f75 7470 7574            output
+00001c80: 2b3d 225c 6e5c 6e20 4469 7265 6374 6f72  +="\n\n Director
+00001c90: 793a 2022 2b73 656c 662e 6469 7265 6374  y: "+self.direct
+00001ca0: 6f72 790a 2020 2020 2020 2020 7265 7475  ory.        retu
+00001cb0: 726e 206f 7574 7075 740a 0a20 2020 2064  rn output..    d
+00001cc0: 6566 2073 686f 7728 7365 6c66 293a 0a20  ef show(self):. 
+00001cd0: 2020 2020 2020 2070 7269 6e74 2873 656c         print(sel
+00001ce0: 6629 0a20 2020 2020 2020 2066 6f72 2069  f).        for i
+00001cf0: 2069 6e20 7261 6e67 6528 7365 6c66 2e6e   in range(self.n
+00001d00: 6d6f 6465 6c73 293a 0a20 2020 2020 2020  models):.       
+00001d10: 2020 2020 2073 656c 662e 6d6f 6465 6c73       self.models
+00001d20: 5b69 5d2e 7368 6f77 2829 0a20 2020 2020  [i].show().     
+00001d30: 2020 2020 2020 2070 7269 6e74 2827 5c6e         print('\n
+00001d40: 2729 0a0a 2020 2020 6465 6620 6164 645f  ')..    def add_
+00001d50: 6d6f 6465 6c28 7365 6c66 2c6d 6f64 656c  model(self,model
+00001d60: 5f64 6174 6129 3a0a 2020 2020 2020 2020  _data):.        
+00001d70: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
+00001d80: 6528 6d6f 6465 6c5f 6461 7461 2c73 6c61  e(model_data,sla
+00001d90: 6229 3a0a 2020 2020 2020 2020 2020 2020  b):.            
+00001da0: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
+00001db0: 2770 6174 6820 6d75 7374 2062 6520 6f66  'path must be of
+00001dc0: 2063 6c61 7373 3a6d 6f64 656c 2729 0a20   class:model'). 
+00001dd0: 2020 2020 2020 2073 656c 662e 6d6f 6465         self.mode
+00001de0: 6c73 2e61 7070 656e 6428 6d6f 6465 6c5f  ls.append(model_
+00001df0: 6461 7461 290a 0a20 2020 2064 6566 2072  data)..    def r
+00001e00: 656d 6f76 655f 6d6f 6465 6c28 7365 6c66  emove_model(self
+00001e10: 2c69 6e64 6578 293a 0a20 2020 2020 2020  ,index):.       
+00001e20: 2069 6620 696e 6465 783c 303a 0a20 2020   if index<0:.   
+00001e30: 2020 2020 2020 2020 2069 6e64 6578 2b3d           index+=
+00001e40: 7365 6c66 2e6e 6d6f 6465 6c73 0a20 2020  self.nmodels.   
+00001e50: 2020 2020 2069 6620 696e 6465 782b 313e       if index+1>
+00001e60: 7365 6c66 2e6e 6d6f 6465 6c73 206f 7220  self.nmodels or 
+00001e70: 696e 6465 783c 303a 0a20 2020 2020 2020  index<0:.       
+00001e80: 2020 2020 2072 6169 7365 2049 6e64 6578       raise Index
+00001e90: 4572 726f 7228 2749 6e64 6578 206f 7574  Error('Index out
+00001ea0: 206f 6620 7261 6e67 6527 290a 2020 2020   of range').    
+00001eb0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00001ec0: 2020 2020 2020 7365 6c66 2e6e 6d6f 6465        self.nmode
+00001ed0: 6c73 2d3d 310a 2020 2020 2020 2020 2020  ls-=1.          
+00001ee0: 2020 7365 6c66 2e6d 6f64 656c 732e 706f    self.models.po
+00001ef0: 7028 696e 6465 7829 0a0a 2020 2020 6465  p(index)..    de
+00001f00: 6620 5f5f 6765 7469 7465 6d5f 5f28 7365  f __getitem__(se
+00001f10: 6c66 2c61 7267 293a 0a20 2020 2020 2020  lf,arg):.       
+00001f20: 2072 6574 5f64 6174 613d 736c 6162 5f64   ret_data=slab_d
+00001f30: 6174 6128 290a 2020 2020 2020 2020 6966  ata().        if
+00001f40: 2069 7369 6e73 7461 6e63 6528 6172 672c   isinstance(arg,
+00001f50: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
+00001f60: 2020 6966 2061 7267 3e73 656c 662e 6e6d    if arg>self.nm
+00001f70: 6f64 656c 733a 0a20 2020 2020 2020 2020  odels:.         
+00001f80: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00001f90: 7565 4572 726f 7228 6627 696e 6465 7820  ueError(f'index 
+00001fa0: 7b61 7267 7d20 6772 6561 7465 7220 7468  {arg} greater th
+00001fb0: 616e 206e 756d 6265 7220 6f66 206d 6f64  an number of mod
+00001fc0: 656c 7320 7b73 656c 662e 6e6d 6f64 656c  els {self.nmodel
+00001fd0: 737d 2729 0a20 2020 2020 2020 2020 2020  s}').           
+00001fe0: 2072 6574 5f64 6174 612e 6164 645f 6d6f   ret_data.add_mo
+00001ff0: 6465 6c28 7365 6c66 2e6d 6f64 656c 735b  del(self.models[
+00002000: 6172 675d 290a 2020 2020 2020 2020 656c  arg]).        el
+00002010: 6966 2069 7369 6e73 7461 6e63 6528 6172  if isinstance(ar
+00002020: 672c 7479 7065 284e 6f6e 6529 293a 0a20  g,type(None)):. 
+00002030: 2020 2020 2020 2020 2020 2066 6f72 206d             for m
+00002040: 6f64 656c 2069 6e20 7365 6c66 2e6d 6f64  odel in self.mod
+00002050: 656c 733a 0a20 2020 2020 2020 2020 2020  els:.           
+00002060: 2020 2020 2072 6574 5f64 6174 612e 6164       ret_data.ad
+00002070: 645f 6d6f 6465 6c28 6d6f 6465 6c29 0a20  d_model(model). 
+00002080: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
+00002090: 7374 616e 6365 2861 7267 2c73 6c69 6365  stance(arg,slice
+000020a0: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+000020b0: 6620 6973 696e 7374 616e 6365 2861 7267  f isinstance(arg
+000020c0: 2e73 7461 7274 2c69 6e74 293a 0a20 2020  .start,int):.   
+000020d0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000020e0: 6973 696e 7374 616e 6365 2861 7267 2e73  isinstance(arg.s
+000020f0: 746f 702c 696e 7429 3a0a 2020 2020 2020  top,int):.      
+00002100: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00002110: 7220 6d6f 6465 6c20 696e 2073 656c 662e  r model in self.
+00002120: 6d6f 6465 6c73 5b61 7267 5d3a 0a20 2020  models[arg]:.   
+00002130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002140: 2020 2020 2072 6574 5f64 6174 612e 6164       ret_data.ad
+00002150: 645f 6d6f 6465 6c28 6d6f 6465 6c29 0a20  d_model(model). 
+00002160: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00002170: 6c69 6620 6973 696e 7374 616e 6365 2861  lif isinstance(a
+00002180: 7267 2e73 746f 702c 7479 7065 284e 6f6e  rg.stop,type(Non
+00002190: 6529 293a 0a20 2020 2020 2020 2020 2020  e)):.           
+000021a0: 2020 2020 2020 2020 2072 6574 5f64 6174           ret_dat
+000021b0: 612e 6164 645f 6d6f 6465 6c28 7365 6c66  a.add_model(self
+000021c0: 2e6d 6f64 656c 735b 6172 672e 7374 6172  .models[arg.star
+000021d0: 745d 290a 2020 2020 2020 2020 2020 2020  t]).            
+000021e0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+000021f0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00002200: 6973 6520 496e 6465 7845 7272 6f72 2866  ise IndexError(f
+00002210: 2773 6c69 6369 6e67 206e 6f74 2075 6e64  'slicing not und
+00002220: 6572 7374 616e 6461 626c 6520 7b61 7267  erstandable {arg
+00002230: 7d27 290a 2020 2020 2020 2020 2020 2020  }').            
+00002240: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
+00002250: 6172 672e 7374 6172 742c 7374 7229 3a0a  arg.start,str):.
+00002260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002270: 6966 2061 7267 2e73 7461 7274 3d3d 2773  if arg.start=='s
+00002280: 7065 6369 6573 5f6e 616d 6527 3a0a 2020  pecies_name':.  
+00002290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022a0: 2020 7365 6c5f 7370 6563 6965 733d 5b5d    sel_species=[]
+000022b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000022c0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+000022d0: 6365 2861 7267 2e73 746f 702c 7374 7229  ce(arg.stop,str)
+000022e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000022f0: 2020 2020 2020 2020 2020 7365 6c5f 7370            sel_sp
+00002300: 6563 6965 732e 6170 7065 6e64 2861 7267  ecies.append(arg
+00002310: 2e73 746f 7029 0a20 2020 2020 2020 2020  .stop).         
+00002320: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00002330: 6973 696e 7374 616e 6365 2861 7267 2e73  isinstance(arg.s
+00002340: 746f 702c 6c69 7374 293a 0a20 2020 2020  top,list):.     
 00002350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002360: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-00002370: 6528 6172 672e 7374 6f70 2c61 7267 2e73  e(arg.stop,arg.s
-00002380: 7465 7029 3a0a 2020 2020 2020 2020 2020  tep):.          
-00002390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023a0: 2020 2020 2020 7365 6c5f 7370 6563 6965        sel_specie
-000023b0: 735f 6e75 6d62 6572 2e61 7070 656e 6428  s_number.append(
-000023c0: 6929 0a20 2020 2020 2020 2020 2020 2020  i).             
-000023d0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000023e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000023f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00002400: 5f73 7065 6369 6573 5f6e 756d 6265 722e  _species_number.
-00002410: 6170 7065 6e64 2861 7267 2e73 746f 7029  append(arg.stop)
-00002420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002430: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
-00002440: 616e 6365 2861 7267 2e73 746f 702c 6c69  ance(arg.stop,li
-00002450: 7374 293a 0a20 2020 2020 2020 2020 2020  st):.           
-00002460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002470: 2073 656c 5f73 7065 6369 6573 5f6e 756d   sel_species_num
-00002480: 6265 723d 6172 672e 7374 6f70 0a20 2020  ber=arg.stop.   
-00002490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024a0: 2069 6620 6c65 6e28 7365 6c5f 7370 6563   if len(sel_spec
-000024b0: 6965 735f 6e75 6d62 6572 293e 303a 0a20  ies_number)>0:. 
-000024c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024d0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-000024e0: 7261 6e67 6528 7365 6c66 2e6e 6d6f 6465  range(self.nmode
-000024f0: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
-00002500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002510: 2069 6620 7365 6c66 2e6d 6f64 656c 735b   if self.models[
-00002520: 695d 2e73 7065 6369 6573 5f6e 756d 6265  i].species_numbe
-00002530: 7220 696e 2073 656c 5f73 7065 6369 6573  r in sel_species
-00002540: 5f6e 756d 6265 723a 0a20 2020 2020 2020  _number:.       
-00002550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002560: 2020 2020 2020 2020 2072 6574 5f64 6174           ret_dat
-00002570: 612e 6164 645f 6d6f 6465 6c28 7365 6c66  a.add_model(self
-00002580: 2e6d 6f64 656c 735b 695d 290a 2020 2020  .models[i]).    
-00002590: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-000025a0: 2061 7267 2e73 7461 7274 3d3d 276d 6f64   arg.start=='mod
-000025b0: 656c 5f6e 756d 6265 7227 3a0a 2020 2020  el_number':.    
-000025c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025d0: 7365 6c5f 7370 6563 6965 735f 6e75 6d62  sel_species_numb
-000025e0: 6572 3d5b 5d0a 2020 2020 2020 2020 2020  er=[].          
-000025f0: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
-00002600: 6e73 7461 6e63 6528 6172 672e 7374 6f70  nstance(arg.stop
-00002610: 2c69 6e74 293a 0a20 2020 2020 2020 2020  ,int):.         
-00002620: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00002630: 6620 6973 696e 7374 616e 6365 2861 7267  f isinstance(arg
-00002640: 2e73 7465 702c 696e 7429 3a0a 2020 2020  .step,int):.    
-00002650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002660: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00002670: 2072 616e 6765 2861 7267 2e73 746f 702c   range(arg.stop,
-00002680: 6172 672e 7374 6570 293a 0a20 2020 2020  arg.step):.     
-00002690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026a0: 2020 2020 2020 2020 2020 2073 656c 5f73             sel_s
-000026b0: 7065 6369 6573 5f6e 756d 6265 722e 6170  pecies_number.ap
-000026c0: 7065 6e64 2869 290a 2020 2020 2020 2020  pend(i).        
-000026d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026e0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000026f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002700: 2020 7365 6c5f 7370 6563 6965 735f 6e75    sel_species_nu
-00002710: 6d62 6572 2e61 7070 656e 6428 6172 672e  mber.append(arg.
-00002720: 7374 6f70 290a 2020 2020 2020 2020 2020  stop).          
-00002730: 2020 2020 2020 2020 2020 656c 6966 2069            elif i
-00002740: 7369 6e73 7461 6e63 6528 6172 672e 7374  sinstance(arg.st
-00002750: 6f70 2c6c 6973 7429 3a0a 2020 2020 2020  op,list):.      
-00002760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002770: 2020 2020 2020 7365 6c5f 7370 6563 6965        sel_specie
-00002780: 735f 6e75 6d62 6572 3d61 7267 2e73 746f  s_number=arg.sto
-00002790: 700a 2020 2020 2020 2020 2020 2020 2020  p.              
-000027a0: 2020 2020 2020 6966 206c 656e 2873 656c        if len(sel
-000027b0: 5f73 7065 6369 6573 5f6e 756d 6265 7229  _species_number)
-000027c0: 3e30 3a0a 2020 2020 2020 2020 2020 2020  >0:.            
-000027d0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000027e0: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
-000027f0: 6e6d 6f64 656c 7329 3a0a 2020 2020 2020  nmodels):.      
+00002360: 2020 2073 656c 5f73 7065 6369 6573 3d61     sel_species=a
+00002370: 7267 2e73 746f 700a 2020 2020 2020 2020  rg.stop.        
+00002380: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+00002390: 656e 2873 656c 5f73 7065 6369 6573 293e  en(sel_species)>
+000023a0: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
+000023b0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+000023c0: 2069 6e20 7261 6e67 6528 7365 6c66 2e6e   in range(self.n
+000023d0: 6d6f 6465 6c73 293a 0a20 2020 2020 2020  models):.       
+000023e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023f0: 2020 2020 2069 6620 7365 6c66 2e6d 6f64       if self.mod
+00002400: 656c 735b 695d 2e73 7065 6369 6573 5f6e  els[i].species_n
+00002410: 616d 6520 696e 2073 656c 5f73 7065 6369  ame in sel_speci
+00002420: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00002430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002440: 2020 2020 7265 745f 6461 7461 2e61 6464      ret_data.add
+00002450: 5f6d 6f64 656c 2873 656c 662e 6d6f 6465  _model(self.mode
+00002460: 6c73 5b69 5d29 0a20 2020 2020 2020 2020  ls[i]).         
+00002470: 2020 2020 2020 2065 6c69 6620 6172 672e         elif arg.
+00002480: 7374 6172 743d 3d27 7370 6563 6965 735f  start=='species_
+00002490: 6e75 6d62 6572 273a 0a20 2020 2020 2020  number':.       
+000024a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000024b0: 5f73 7065 6369 6573 5f6e 756d 6265 723d  _species_number=
+000024c0: 5b5d 0a20 2020 2020 2020 2020 2020 2020  [].             
+000024d0: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+000024e0: 616e 6365 2861 7267 2e73 746f 702c 696e  ance(arg.stop,in
+000024f0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+00002500: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00002510: 7369 6e73 7461 6e63 6528 6172 672e 7374  sinstance(arg.st
+00002520: 6570 2c69 6e74 293a 0a20 2020 2020 2020  ep,int):.       
+00002530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002540: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+00002550: 6e67 6528 6172 672e 7374 6f70 2c61 7267  nge(arg.stop,arg
+00002560: 2e73 7465 7029 3a0a 2020 2020 2020 2020  .step):.        
+00002570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002580: 2020 2020 2020 2020 7365 6c5f 7370 6563          sel_spec
+00002590: 6965 735f 6e75 6d62 6572 2e61 7070 656e  ies_number.appen
+000025a0: 6428 6929 0a20 2020 2020 2020 2020 2020  d(i).           
+000025b0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+000025c0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000025d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000025e0: 656c 5f73 7065 6369 6573 5f6e 756d 6265  el_species_numbe
+000025f0: 722e 6170 7065 6e64 2861 7267 2e73 746f  r.append(arg.sto
+00002600: 7029 0a20 2020 2020 2020 2020 2020 2020  p).             
+00002610: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
+00002620: 7374 616e 6365 2861 7267 2e73 746f 702c  stance(arg.stop,
+00002630: 6c69 7374 293a 0a20 2020 2020 2020 2020  list):.         
+00002640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002650: 2020 2073 656c 5f73 7065 6369 6573 5f6e     sel_species_n
+00002660: 756d 6265 723d 6172 672e 7374 6f70 0a20  umber=arg.stop. 
+00002670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002680: 2020 2069 6620 6c65 6e28 7365 6c5f 7370     if len(sel_sp
+00002690: 6563 6965 735f 6e75 6d62 6572 293e 303a  ecies_number)>0:
+000026a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000026b0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+000026c0: 6e20 7261 6e67 6528 7365 6c66 2e6e 6d6f  n range(self.nmo
+000026d0: 6465 6c73 293a 0a20 2020 2020 2020 2020  dels):.         
+000026e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026f0: 2020 2069 6620 7365 6c66 2e6d 6f64 656c     if self.model
+00002700: 735b 695d 2e73 7065 6369 6573 5f6e 756d  s[i].species_num
+00002710: 6265 7220 696e 2073 656c 5f73 7065 6369  ber in sel_speci
+00002720: 6573 5f6e 756d 6265 723a 0a20 2020 2020  es_number:.     
+00002730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002740: 2020 2020 2020 2020 2020 2072 6574 5f64             ret_d
+00002750: 6174 612e 6164 645f 6d6f 6465 6c28 7365  ata.add_model(se
+00002760: 6c66 2e6d 6f64 656c 735b 695d 290a 2020  lf.models[i]).  
+00002770: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00002780: 6966 2061 7267 2e73 7461 7274 3d3d 276d  if arg.start=='m
+00002790: 6f64 656c 5f6e 756d 6265 7227 3a0a 2020  odel_number':.  
+000027a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027b0: 2020 7365 6c5f 7370 6563 6965 735f 6e75    sel_species_nu
+000027c0: 6d62 6572 3d5b 5d0a 2020 2020 2020 2020  mber=[].        
+000027d0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+000027e0: 7369 6e73 7461 6e63 6528 6172 672e 7374  sinstance(arg.st
+000027f0: 6f70 2c69 6e74 293a 0a20 2020 2020 2020  op,int):.       
 00002800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002810: 2020 2020 2020 6966 2073 656c 662e 6d6f        if self.mo
-00002820: 6465 6c73 5b69 5d2e 6d6f 6465 6c5f 6e75  dels[i].model_nu
-00002830: 6d62 6572 2069 6e20 7365 6c5f 7370 6563  mber in sel_spec
-00002840: 6965 735f 6e75 6d62 6572 3a0a 2020 2020  ies_number:.    
-00002850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002860: 2020 2020 2020 2020 2020 2020 7265 745f              ret_
-00002870: 6461 7461 2e61 6464 5f6d 6f64 656c 2873  data.add_model(s
-00002880: 656c 662e 6d6f 6465 6c73 5b69 5d29 0a20  elf.models[i]). 
-00002890: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-000028a0: 6c69 6620 6172 672e 7374 6172 743d 3d27  lif arg.start=='
-000028b0: 4e48 273a 0a20 2020 2020 2020 2020 2020  NH':.           
-000028c0: 2020 2020 2020 2020 2075 7070 6572 3d6e           upper=n
-000028d0: 702e 6e61 6e0a 2020 2020 2020 2020 2020  p.nan.          
-000028e0: 2020 2020 2020 2020 2020 6c6f 7765 723d            lower=
-000028f0: 6e70 2e6e 616e 0a20 2020 2020 2020 2020  np.nan.         
-00002900: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-00002910: 696e 7374 616e 6365 2861 7267 2e73 746f  instance(arg.sto
-00002920: 702c 666c 6f61 7429 206f 7220 6973 696e  p,float) or isin
-00002930: 7374 616e 6365 2861 7267 2e73 746f 702c  stance(arg.stop,
-00002940: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
-00002950: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00002960: 2069 7369 6e73 7461 6e63 6528 6172 672e   isinstance(arg.
-00002970: 7374 6570 2c66 6c6f 6174 2920 6f72 2069  step,float) or i
-00002980: 7369 6e73 7461 6e63 6528 6172 672e 7374  sinstance(arg.st
-00002990: 6570 2c69 6e74 293a 0a20 2020 2020 2020  ep,int):.       
-000029a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029b0: 2020 2020 206c 6f77 6572 2c75 7070 6572       lower,upper
-000029c0: 3d61 7267 2e73 746f 702c 6172 672e 7374  =arg.stop,arg.st
-000029d0: 6570 0a20 2020 2020 2020 2020 2020 2020  ep.             
-000029e0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000029f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002a00: 2020 2020 2020 2020 2020 2020 2075 7070               upp
-00002a10: 6572 3d61 7267 2e73 746f 700a 2020 2020  er=arg.stop.    
-00002a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a30: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00002a40: 6765 2873 656c 662e 6e6d 6f64 656c 7329  ge(self.nmodels)
-00002a50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002a60: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00002a70: 206e 6f74 206e 702e 6973 6e61 6e28 6c6f   not np.isnan(lo
-00002a80: 7765 7229 3a0a 2020 2020 2020 2020 2020  wer):.          
-00002a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002aa0: 2020 2020 2020 6966 2073 656c 662e 6d6f        if self.mo
-00002ab0: 6465 6c73 5b69 5d2e 4e48 3c75 7070 6572  dels[i].NH<upper
-00002ac0: 2061 6e64 2073 656c 662e 6d6f 6465 6c73   and self.models
-00002ad0: 5b69 5d2e 4e48 3e6c 6f77 6572 3a0a 2020  [i].NH>lower:.  
-00002ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b00: 2020 7265 745f 6461 7461 2e61 6464 5f6d    ret_data.add_m
-00002b10: 6f64 656c 2873 656c 662e 6d6f 6465 6c73  odel(self.models
-00002b20: 5b69 5d29 0a20 2020 2020 2020 2020 2020  [i]).           
+00002810: 2069 6620 6973 696e 7374 616e 6365 2861   if isinstance(a
+00002820: 7267 2e73 7465 702c 696e 7429 3a0a 2020  rg.step,int):.  
+00002830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002840: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
+00002850: 696e 2072 616e 6765 2861 7267 2e73 746f  in range(arg.sto
+00002860: 702c 6172 672e 7374 6570 293a 0a20 2020  p,arg.step):.   
+00002870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002880: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00002890: 5f73 7065 6369 6573 5f6e 756d 6265 722e  _species_number.
+000028a0: 6170 7065 6e64 2869 290a 2020 2020 2020  append(i).      
+000028b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028c0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000028d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028e0: 2020 2020 7365 6c5f 7370 6563 6965 735f      sel_species_
+000028f0: 6e75 6d62 6572 2e61 7070 656e 6428 6172  number.append(ar
+00002900: 672e 7374 6f70 290a 2020 2020 2020 2020  g.stop).        
+00002910: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00002920: 2069 7369 6e73 7461 6e63 6528 6172 672e   isinstance(arg.
+00002930: 7374 6f70 2c6c 6973 7429 3a0a 2020 2020  stop,list):.    
+00002940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002950: 2020 2020 2020 2020 7365 6c5f 7370 6563          sel_spec
+00002960: 6965 735f 6e75 6d62 6572 3d61 7267 2e73  ies_number=arg.s
+00002970: 746f 700a 2020 2020 2020 2020 2020 2020  top.            
+00002980: 2020 2020 2020 2020 6966 206c 656e 2873          if len(s
+00002990: 656c 5f73 7065 6369 6573 5f6e 756d 6265  el_species_numbe
+000029a0: 7229 3e30 3a0a 2020 2020 2020 2020 2020  r)>0:.          
+000029b0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+000029c0: 7220 6920 696e 2072 616e 6765 2873 656c  r i in range(sel
+000029d0: 662e 6e6d 6f64 656c 7329 3a0a 2020 2020  f.nmodels):.    
+000029e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00002a00: 6d6f 6465 6c73 5b69 5d2e 6d6f 6465 6c5f  models[i].model_
+00002a10: 6e75 6d62 6572 2069 6e20 7365 6c5f 7370  number in sel_sp
+00002a20: 6563 6965 735f 6e75 6d62 6572 3a0a 2020  ecies_number:.  
+00002a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a40: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00002a50: 745f 6461 7461 2e61 6464 5f6d 6f64 656c  t_data.add_model
+00002a60: 2873 656c 662e 6d6f 6465 6c73 5b69 5d29  (self.models[i])
+00002a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002a80: 2065 6c69 6620 6172 672e 7374 6172 743d   elif arg.start=
+00002a90: 3d27 4e48 273a 0a20 2020 2020 2020 2020  ='NH':.         
+00002aa0: 2020 2020 2020 2020 2020 2075 7070 6572             upper
+00002ab0: 3d6e 702e 6e61 6e0a 2020 2020 2020 2020  =np.nan.        
+00002ac0: 2020 2020 2020 2020 2020 2020 6c6f 7765              lowe
+00002ad0: 723d 6e70 2e6e 616e 0a20 2020 2020 2020  r=np.nan.       
+00002ae0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00002af0: 6973 696e 7374 616e 6365 2861 7267 2e73  isinstance(arg.s
+00002b00: 746f 702c 666c 6f61 7429 206f 7220 6973  top,float) or is
+00002b10: 696e 7374 616e 6365 2861 7267 2e73 746f  instance(arg.sto
+00002b20: 702c 696e 7429 3a0a 2020 2020 2020 2020  p,int):.        
 00002b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b40: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00002b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b60: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
-00002b70: 6f64 656c 735b 695d 2e4e 483d 3d75 7070  odels[i].NH==upp
-00002b80: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
-00002b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ba0: 2020 2020 2020 2020 7265 745f 6461 7461          ret_data
-00002bb0: 2e61 6464 5f6d 6f64 656c 2873 656c 662e  .add_model(self.
-00002bc0: 6d6f 6465 6c73 5b69 5d29 0a20 2020 2020  models[i]).     
-00002bd0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00002be0: 6c69 6620 6973 696e 7374 616e 6365 2861  lif isinstance(a
-00002bf0: 7267 2e73 746f 702c 6c69 7374 293a 0a20  rg.stop,list):. 
+00002b40: 6966 2069 7369 6e73 7461 6e63 6528 6172  if isinstance(ar
+00002b50: 672e 7374 6570 2c66 6c6f 6174 2920 6f72  g.step,float) or
+00002b60: 2069 7369 6e73 7461 6e63 6528 6172 672e   isinstance(arg.
+00002b70: 7374 6570 2c69 6e74 293a 0a20 2020 2020  step,int):.     
+00002b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b90: 2020 2020 2020 206c 6f77 6572 2c75 7070         lower,upp
+00002ba0: 6572 3d61 7267 2e73 746f 702c 6172 672e  er=arg.stop,arg.
+00002bb0: 7374 6570 0a20 2020 2020 2020 2020 2020  step.           
+00002bc0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00002bd0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00002be0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+00002bf0: 7070 6572 3d61 7267 2e73 746f 700a 2020  pper=arg.stop.  
 00002c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c10: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-00002c20: 7261 6e67 6528 7365 6c66 2e6e 6d6f 6465  range(self.nmode
-00002c30: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
+00002c10: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+00002c20: 616e 6765 2873 656c 662e 6e6d 6f64 656c  ange(self.nmodel
+00002c30: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
 00002c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c50: 2069 6620 7365 6c66 2e6d 6f64 656c 735b   if self.models[
-00002c60: 695d 2e4e 4820 696e 2061 7267 2e73 746f  i].NH in arg.sto
-00002c70: 703a 0a20 2020 2020 2020 2020 2020 2020  p:.             
-00002c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c90: 2020 2072 6574 5f64 6174 612e 6164 645f     ret_data.add_
-00002ca0: 6d6f 6465 6c28 7365 6c66 2e6d 6f64 656c  model(self.model
-00002cb0: 735b 695d 290a 2020 2020 2020 2020 2020  s[i]).          
-00002cc0: 2020 2020 2020 656c 6966 2061 7267 2e73        elif arg.s
-00002cd0: 7461 7274 3d3d 276e 436f 6c6c 273a 0a20  tart=='nColl':. 
-00002ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cf0: 2020 2075 7070 6572 3d6e 702e 6e61 6e0a     upper=np.nan.
-00002d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d10: 2020 2020 6c6f 7765 723d 6e70 2e6e 616e      lower=np.nan
-00002d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002d30: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-00002d40: 6365 2861 7267 2e73 746f 702c 666c 6f61  ce(arg.stop,floa
-00002d50: 7429 206f 7220 6973 696e 7374 616e 6365  t) or isinstance
-00002d60: 2861 7267 2e73 746f 702c 696e 7429 3a0a  (arg.stop,int):.
+00002c50: 6966 206e 6f74 206e 702e 6973 6e61 6e28  if not np.isnan(
+00002c60: 6c6f 7765 7229 3a0a 2020 2020 2020 2020  lower):.        
+00002c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c80: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00002c90: 6d6f 6465 6c73 5b69 5d2e 4e48 3c75 7070  models[i].NH<upp
+00002ca0: 6572 2061 6e64 2073 656c 662e 6d6f 6465  er and self.mode
+00002cb0: 6c73 5b69 5d2e 4e48 3e6c 6f77 6572 3a0a  ls[i].NH>lower:.
+00002cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ce0: 2020 2020 7265 745f 6461 7461 2e61 6464      ret_data.add
+00002cf0: 5f6d 6f64 656c 2873 656c 662e 6d6f 6465  _model(self.mode
+00002d00: 6c73 5b69 5d29 0a20 2020 2020 2020 2020  ls[i]).         
+00002d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d20: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00002d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d40: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00002d50: 2e6d 6f64 656c 735b 695d 2e4e 483d 3d75  .models[i].NH==u
+00002d60: 7070 6572 3a0a 2020 2020 2020 2020 2020  pper:.          
 00002d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d80: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-00002d90: 7461 6e63 6528 6172 672e 7374 6570 2c66  tance(arg.step,f
-00002da0: 6c6f 6174 2920 6f72 2069 7369 6e73 7461  loat) or isinsta
-00002db0: 6e63 6528 6172 672e 7374 6570 2c69 6e74  nce(arg.step,int
-00002dc0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00002dd0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00002de0: 6f77 6572 2c75 7070 6572 3d61 7267 2e73  ower,upper=arg.s
-00002df0: 746f 702c 6172 672e 7374 6570 0a20 2020  top,arg.step.   
-00002e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e10: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00002d80: 2020 2020 2020 2020 2020 7265 745f 6461            ret_da
+00002d90: 7461 2e61 6464 5f6d 6f64 656c 2873 656c  ta.add_model(sel
+00002da0: 662e 6d6f 6465 6c73 5b69 5d29 0a20 2020  f.models[i]).   
+00002db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002dc0: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+00002dd0: 2861 7267 2e73 746f 702c 6c69 7374 293a  (arg.stop,list):
+00002de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002df0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+00002e00: 6e20 7261 6e67 6528 7365 6c66 2e6e 6d6f  n range(self.nmo
+00002e10: 6465 6c73 293a 0a20 2020 2020 2020 2020  dels):.         
 00002e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e30: 2020 2020 2020 2075 7070 6572 3d61 7267         upper=arg
-00002e40: 2e73 746f 700a 2020 2020 2020 2020 2020  .stop.          
-00002e50: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00002e60: 7220 6920 696e 2072 616e 6765 2873 656c  r i in range(sel
-00002e70: 662e 6e6d 6f64 656c 7329 3a0a 2020 2020  f.nmodels):.    
-00002e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e90: 2020 2020 2020 2020 6966 206e 6f74 206e          if not n
-00002ea0: 702e 6973 6e61 6e28 6c6f 7765 7229 3a0a  p.isnan(lower):.
-00002eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ed0: 6966 2073 656c 662e 6d6f 6465 6c73 5b69  if self.models[i
-00002ee0: 5d2e 6e43 6f6c 6c3c 7570 7065 7220 616e  ].nColl<upper an
-00002ef0: 6420 7365 6c66 2e6d 6f64 656c 735b 695d  d self.models[i]
-00002f00: 2e6e 436f 6c6c 3e6c 6f77 6572 3a0a 2020  .nColl>lower:.  
-00002f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f30: 2020 7265 745f 6461 7461 2e61 6464 5f6d    ret_data.add_m
-00002f40: 6f64 656c 2873 656c 662e 6d6f 6465 6c73  odel(self.models
-00002f50: 5b69 5d29 0a20 2020 2020 2020 2020 2020  [i]).           
-00002f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f70: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00002f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f90: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
-00002fa0: 6f64 656c 735b 695d 2e6e 436f 6c6c 3d3d  odels[i].nColl==
-00002fb0: 7570 7065 723a 0a20 2020 2020 2020 2020  upper:.         
-00002fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002fd0: 2020 2020 2020 2020 2020 2072 6574 5f64             ret_d
-00002fe0: 6174 612e 6164 645f 6d6f 6465 6c28 7365  ata.add_model(se
-00002ff0: 6c66 2e6d 6f64 656c 735b 695d 290a 2020  lf.models[i]).  
+00002e30: 2020 2069 6620 7365 6c66 2e6d 6f64 656c     if self.model
+00002e40: 735b 695d 2e4e 4820 696e 2061 7267 2e73  s[i].NH in arg.s
+00002e50: 746f 703a 0a20 2020 2020 2020 2020 2020  top:.           
+00002e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e70: 2020 2020 2072 6574 5f64 6174 612e 6164       ret_data.ad
+00002e80: 645f 6d6f 6465 6c28 7365 6c66 2e6d 6f64  d_model(self.mod
+00002e90: 656c 735b 695d 290a 2020 2020 2020 2020  els[i]).        
+00002ea0: 2020 2020 2020 2020 656c 6966 2061 7267          elif arg
+00002eb0: 2e73 7461 7274 3d3d 276e 436f 6c6c 273a  .start=='nColl':
+00002ec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002ed0: 2020 2020 2075 7070 6572 3d6e 702e 6e61       upper=np.na
+00002ee0: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+00002ef0: 2020 2020 2020 6c6f 7765 723d 6e70 2e6e        lower=np.n
+00002f00: 616e 0a20 2020 2020 2020 2020 2020 2020  an.             
+00002f10: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00002f20: 616e 6365 2861 7267 2e73 746f 702c 666c  ance(arg.stop,fl
+00002f30: 6f61 7429 206f 7220 6973 696e 7374 616e  oat) or isinstan
+00002f40: 6365 2861 7267 2e73 746f 702c 696e 7429  ce(arg.stop,int)
+00002f50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00002f60: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+00002f70: 6e73 7461 6e63 6528 6172 672e 7374 6570  nstance(arg.step
+00002f80: 2c66 6c6f 6174 2920 6f72 2069 7369 6e73  ,float) or isins
+00002f90: 7461 6e63 6528 6172 672e 7374 6570 2c69  tance(arg.step,i
+00002fa0: 6e74 293a 0a20 2020 2020 2020 2020 2020  nt):.           
+00002fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002fc0: 206c 6f77 6572 2c75 7070 6572 3d61 7267   lower,upper=arg
+00002fd0: 2e73 746f 702c 6172 672e 7374 6570 0a20  .stop,arg.step. 
+00002fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ff0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
 00003000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003010: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
-00003020: 6528 6172 672e 7374 6f70 2c6c 6973 7429  e(arg.stop,list)
-00003030: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00003040: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
-00003050: 696e 2072 616e 6765 2873 656c 662e 6e6d  in range(self.nm
-00003060: 6f64 656c 7329 3a0a 2020 2020 2020 2020  odels):.        
-00003070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003080: 2020 2020 6966 2073 656c 662e 6d6f 6465      if self.mode
-00003090: 6c73 5b69 5d2e 6e43 6f6c 6c20 696e 2061  ls[i].nColl in a
-000030a0: 7267 2e73 746f 703a 0a20 2020 2020 2020  rg.stop:.       
-000030b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030c0: 2020 2020 2020 2020 2072 6574 5f64 6174           ret_dat
-000030d0: 612e 6164 645f 6d6f 6465 6c28 7365 6c66  a.add_model(self
-000030e0: 2e6d 6f64 656c 735b 695d 290a 2020 2020  .models[i]).    
-000030f0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00003100: 2061 7267 2e73 7461 7274 3d3d 276e 6527   arg.start=='ne'
-00003110: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00003120: 2020 2020 2020 7570 7065 723d 6e70 2e6e        upper=np.n
-00003130: 616e 0a20 2020 2020 2020 2020 2020 2020  an.             
-00003140: 2020 2020 2020 206c 6f77 6572 3d6e 702e         lower=np.
-00003150: 6e61 6e0a 2020 2020 2020 2020 2020 2020  nan.            
-00003160: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-00003170: 7461 6e63 6528 6172 672e 7374 6f70 2c66  tance(arg.stop,f
-00003180: 6c6f 6174 2920 6f72 2069 7369 6e73 7461  loat) or isinsta
-00003190: 6e63 6528 6172 672e 7374 6f70 2c69 6e74  nce(arg.stop,int
-000031a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000031b0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-000031c0: 696e 7374 616e 6365 2861 7267 2e73 7465  instance(arg.ste
-000031d0: 702c 666c 6f61 7429 206f 7220 6973 696e  p,float) or isin
-000031e0: 7374 616e 6365 2861 7267 2e73 7465 702c  stance(arg.step,
-000031f0: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
-00003200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003210: 2020 6c6f 7765 722c 7570 7065 723d 6172    lower,upper=ar
-00003220: 672e 7374 6f70 2c61 7267 2e73 7465 700a  g.stop,arg.step.
-00003230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003240: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00003010: 2020 2020 2020 2020 2075 7070 6572 3d61           upper=a
+00003020: 7267 2e73 746f 700a 2020 2020 2020 2020  rg.stop.        
+00003030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003040: 666f 7220 6920 696e 2072 616e 6765 2873  for i in range(s
+00003050: 656c 662e 6e6d 6f64 656c 7329 3a0a 2020  elf.nmodels):.  
+00003060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003070: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+00003080: 206e 702e 6973 6e61 6e28 6c6f 7765 7229   np.isnan(lower)
+00003090: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000030a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030b0: 2020 6966 2073 656c 662e 6d6f 6465 6c73    if self.models
+000030c0: 5b69 5d2e 6e43 6f6c 6c3c 7570 7065 7220  [i].nColl<upper 
+000030d0: 616e 6420 7365 6c66 2e6d 6f64 656c 735b  and self.models[
+000030e0: 695d 2e6e 436f 6c6c 3e6c 6f77 6572 3a0a  i].nColl>lower:.
+000030f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003110: 2020 2020 7265 745f 6461 7461 2e61 6464      ret_data.add
+00003120: 5f6d 6f64 656c 2873 656c 662e 6d6f 6465  _model(self.mode
+00003130: 6c73 5b69 5d29 0a20 2020 2020 2020 2020  ls[i]).         
+00003140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003150: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00003160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003170: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00003180: 2e6d 6f64 656c 735b 695d 2e6e 436f 6c6c  .models[i].nColl
+00003190: 3d3d 7570 7065 723a 0a20 2020 2020 2020  ==upper:.       
+000031a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031b0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+000031c0: 5f64 6174 612e 6164 645f 6d6f 6465 6c28  _data.add_model(
+000031d0: 7365 6c66 2e6d 6f64 656c 735b 695d 290a  self.models[i]).
+000031e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031f0: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
+00003200: 6e63 6528 6172 672e 7374 6f70 2c6c 6973  nce(arg.stop,lis
+00003210: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+00003220: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00003230: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
+00003240: 6e6d 6f64 656c 7329 3a0a 2020 2020 2020  nmodels):.      
 00003250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003260: 2020 2020 2020 2020 2020 7570 7065 723d            upper=
-00003270: 6172 672e 7374 6f70 0a20 2020 2020 2020  arg.stop.       
-00003280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003290: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-000032a0: 7365 6c66 2e6e 6d6f 6465 6c73 293a 0a20  self.nmodels):. 
-000032b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032c0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-000032d0: 7420 6e70 2e69 736e 616e 286c 6f77 6572  t np.isnan(lower
-000032e0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000032f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003300: 2020 2069 6620 7365 6c66 2e6d 6f64 656c     if self.model
-00003310: 735b 695d 2e6e 653c 7570 7065 7220 616e  s[i].ne<upper an
-00003320: 6420 7365 6c66 2e6d 6f64 656c 735b 695d  d self.models[i]
-00003330: 2e6e 653e 6c6f 7765 723a 0a20 2020 2020  .ne>lower:.     
-00003340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003350: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00003360: 6574 5f64 6174 612e 6164 645f 6d6f 6465  et_data.add_mode
-00003370: 6c28 7365 6c66 2e6d 6f64 656c 735b 695d  l(self.models[i]
-00003380: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00003390: 2020 2020 2020 2020 2020 2020 2020 656c                el
-000033a0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000033b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033c0: 2020 2020 6966 2073 656c 662e 6d6f 6465      if self.mode
-000033d0: 6c73 5b69 5d2e 6e65 3d3d 7570 7065 723a  ls[i].ne==upper:
-000033e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000033f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003400: 2020 2020 2072 6574 5f64 6174 612e 6164       ret_data.ad
-00003410: 645f 6d6f 6465 6c28 7365 6c66 2e6d 6f64  d_model(self.mod
-00003420: 656c 735b 695d 290a 2020 2020 2020 2020  els[i]).        
-00003430: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00003440: 2069 7369 6e73 7461 6e63 6528 6172 672e   isinstance(arg.
-00003450: 7374 6f70 2c6c 6973 7429 3a0a 0a20 2020  stop,list):..   
+00003260: 2020 2020 2020 6966 2073 656c 662e 6d6f        if self.mo
+00003270: 6465 6c73 5b69 5d2e 6e43 6f6c 6c20 696e  dels[i].nColl in
+00003280: 2061 7267 2e73 746f 703a 0a20 2020 2020   arg.stop:.     
+00003290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032a0: 2020 2020 2020 2020 2020 2072 6574 5f64             ret_d
+000032b0: 6174 612e 6164 645f 6d6f 6465 6c28 7365  ata.add_model(se
+000032c0: 6c66 2e6d 6f64 656c 735b 695d 290a 2020  lf.models[i]).  
+000032d0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+000032e0: 6966 2061 7267 2e73 7461 7274 3d3d 276e  if arg.start=='n
+000032f0: 6527 3a0a 2020 2020 2020 2020 2020 2020  e':.            
+00003300: 2020 2020 2020 2020 7570 7065 723d 6e70          upper=np
+00003310: 2e6e 616e 0a20 2020 2020 2020 2020 2020  .nan.           
+00003320: 2020 2020 2020 2020 206c 6f77 6572 3d6e           lower=n
+00003330: 702e 6e61 6e0a 2020 2020 2020 2020 2020  p.nan.          
+00003340: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+00003350: 6e73 7461 6e63 6528 6172 672e 7374 6f70  nstance(arg.stop
+00003360: 2c66 6c6f 6174 2920 6f72 2069 7369 6e73  ,float) or isins
+00003370: 7461 6e63 6528 6172 672e 7374 6f70 2c69  tance(arg.stop,i
+00003380: 6e74 293a 0a20 2020 2020 2020 2020 2020  nt):.           
+00003390: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000033a0: 6973 696e 7374 616e 6365 2861 7267 2e73  isinstance(arg.s
+000033b0: 7465 702c 666c 6f61 7429 206f 7220 6973  tep,float) or is
+000033c0: 696e 7374 616e 6365 2861 7267 2e73 7465  instance(arg.ste
+000033d0: 702c 696e 7429 3a0a 2020 2020 2020 2020  p,int):.        
+000033e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033f0: 2020 2020 6c6f 7765 722c 7570 7065 723d      lower,upper=
+00003400: 6172 672e 7374 6f70 2c61 7267 2e73 7465  arg.stop,arg.ste
+00003410: 700a 2020 2020 2020 2020 2020 2020 2020  p.              
+00003420: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00003430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003440: 2020 2020 2020 2020 2020 2020 7570 7065              uppe
+00003450: 723d 6172 672e 7374 6f70 0a20 2020 2020  r=arg.stop.     
 00003460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003470: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-00003480: 6e67 6528 7365 6c66 2e6e 6d6f 6465 6c73  nge(self.nmodels
-00003490: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000034a0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000034b0: 6620 7365 6c66 2e6d 6f64 656c 735b 695d  f self.models[i]
-000034c0: 2e6e 6520 696e 2061 7267 2e73 746f 703a  .ne in arg.stop:
-000034d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000034e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034f0: 2072 6574 5f64 6174 612e 6164 645f 6d6f   ret_data.add_mo
-00003500: 6465 6c28 7365 6c66 2e6d 6f64 656c 735b  del(self.models[
-00003510: 695d 290a 2020 2020 2020 2020 2020 2020  i]).            
-00003520: 2020 2020 656c 6966 2061 7267 2e73 7461      elif arg.sta
-00003530: 7274 3d3d 276e 4865 273a 0a20 2020 2020  rt=='nHe':.     
-00003540: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00003550: 7070 6572 3d6e 702e 6e61 6e0a 2020 2020  pper=np.nan.    
-00003560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003570: 6c6f 7765 723d 6e70 2e6e 616e 0a20 2020  lower=np.nan.   
-00003580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003590: 2069 6620 6973 696e 7374 616e 6365 2861   if isinstance(a
-000035a0: 7267 2e73 746f 702c 666c 6f61 7429 206f  rg.stop,float) o
-000035b0: 7220 6973 696e 7374 616e 6365 2861 7267  r isinstance(arg
-000035c0: 2e73 746f 702c 696e 7429 3a0a 2020 2020  .stop,int):.    
+00003470: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+00003480: 6528 7365 6c66 2e6e 6d6f 6465 6c73 293a  e(self.nmodels):
+00003490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000034a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000034b0: 6e6f 7420 6e70 2e69 736e 616e 286c 6f77  not np.isnan(low
+000034c0: 6572 293a 0a20 2020 2020 2020 2020 2020  er):.           
+000034d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034e0: 2020 2020 2069 6620 7365 6c66 2e6d 6f64       if self.mod
+000034f0: 656c 735b 695d 2e6e 653c 7570 7065 7220  els[i].ne<upper 
+00003500: 616e 6420 7365 6c66 2e6d 6f64 656c 735b  and self.models[
+00003510: 695d 2e6e 653e 6c6f 7765 723a 0a20 2020  i].ne>lower:.   
+00003520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003540: 2072 6574 5f64 6174 612e 6164 645f 6d6f   ret_data.add_mo
+00003550: 6465 6c28 7365 6c66 2e6d 6f64 656c 735b  del(self.models[
+00003560: 695d 290a 2020 2020 2020 2020 2020 2020  i]).            
+00003570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003580: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00003590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000035a0: 2020 2020 2020 6966 2073 656c 662e 6d6f        if self.mo
+000035b0: 6465 6c73 5b69 5d2e 6e65 3d3d 7570 7065  dels[i].ne==uppe
+000035c0: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
 000035d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035e0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-000035f0: 6528 6172 672e 7374 6570 2c66 6c6f 6174  e(arg.step,float
-00003600: 2920 6f72 2069 7369 6e73 7461 6e63 6528  ) or isinstance(
-00003610: 6172 672e 7374 6570 2c69 6e74 293a 0a20  arg.step,int):. 
-00003620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003630: 2020 2020 2020 2020 2020 206c 6f77 6572             lower
-00003640: 2c75 7070 6572 3d61 7267 2e73 746f 702c  ,upper=arg.stop,
-00003650: 6172 672e 7374 6570 0a20 2020 2020 2020  arg.step.       
-00003660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003670: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000035e0: 2020 2020 2020 2072 6574 5f64 6174 612e         ret_data.
+000035f0: 6164 645f 6d6f 6465 6c28 7365 6c66 2e6d  add_model(self.m
+00003600: 6f64 656c 735b 695d 290a 2020 2020 2020  odels[i]).      
+00003610: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00003620: 6966 2069 7369 6e73 7461 6e63 6528 6172  if isinstance(ar
+00003630: 672e 7374 6f70 2c6c 6973 7429 3a0a 0a20  g.stop,list):.. 
+00003640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003650: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+00003660: 7261 6e67 6528 7365 6c66 2e6e 6d6f 6465  range(self.nmode
+00003670: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
 00003680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003690: 2020 2075 7070 6572 3d61 7267 2e73 746f     upper=arg.sto
-000036a0: 700a 2020 2020 2020 2020 2020 2020 2020  p.              
-000036b0: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
-000036c0: 696e 2072 616e 6765 2873 656c 662e 6e6d  in range(self.nm
-000036d0: 6f64 656c 7329 3a0a 2020 2020 2020 2020  odels):.        
-000036e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036f0: 2020 2020 6966 206e 6f74 206e 702e 6973      if not np.is
-00003700: 6e61 6e28 6c6f 7765 7229 3a0a 2020 2020  nan(lower):.    
-00003710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003720: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00003730: 656c 662e 6d6f 6465 6c73 5b69 5d2e 6e48  elf.models[i].nH
-00003740: 653c 7570 7065 7220 616e 6420 7365 6c66  e<upper and self
-00003750: 2e6d 6f64 656c 735b 695d 2e6e 4865 3e6c  .models[i].nHe>l
-00003760: 6f77 6572 3a0a 2020 2020 2020 2020 2020  ower:.          
-00003770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003780: 2020 2020 2020 2020 2020 7265 745f 6461            ret_da
-00003790: 7461 2e61 6464 5f6d 6f64 656c 2873 656c  ta.add_model(sel
-000037a0: 662e 6d6f 6465 6c73 5b69 5d29 0a20 2020  f.models[i]).   
+00003690: 2069 6620 7365 6c66 2e6d 6f64 656c 735b   if self.models[
+000036a0: 695d 2e6e 6520 696e 2061 7267 2e73 746f  i].ne in arg.sto
+000036b0: 703a 0a20 2020 2020 2020 2020 2020 2020  p:.             
+000036c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036d0: 2020 2072 6574 5f64 6174 612e 6164 645f     ret_data.add_
+000036e0: 6d6f 6465 6c28 7365 6c66 2e6d 6f64 656c  model(self.model
+000036f0: 735b 695d 290a 2020 2020 2020 2020 2020  s[i]).          
+00003700: 2020 2020 2020 656c 6966 2061 7267 2e73        elif arg.s
+00003710: 7461 7274 3d3d 276e 4865 273a 0a20 2020  tart=='nHe':.   
+00003720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003730: 2075 7070 6572 3d6e 702e 6e61 6e0a 2020   upper=np.nan.  
+00003740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003750: 2020 6c6f 7765 723d 6e70 2e6e 616e 0a20    lower=np.nan. 
+00003760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003770: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00003780: 2861 7267 2e73 746f 702c 666c 6f61 7429  (arg.stop,float)
+00003790: 206f 7220 6973 696e 7374 616e 6365 2861   or isinstance(a
+000037a0: 7267 2e73 746f 702c 696e 7429 3a0a 2020  rg.stop,int):.  
 000037b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037c0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-000037d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000037f0: 6620 7365 6c66 2e6d 6f64 656c 735b 695d  f self.models[i]
-00003800: 2e6e 4865 3d3d 7570 7065 723a 0a20 2020  .nHe==upper:.   
-00003810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003830: 2072 6574 5f64 6174 612e 6164 645f 6d6f   ret_data.add_mo
-00003840: 6465 6c28 7365 6c66 2e6d 6f64 656c 735b  del(self.models[
-00003850: 695d 290a 2020 2020 2020 2020 2020 2020  i]).            
-00003860: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
-00003870: 6e73 7461 6e63 6528 6172 672e 7374 6f70  nstance(arg.stop
-00003880: 2c6c 6973 7429 3a0a 0a20 2020 2020 2020  ,list):..       
-00003890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038a0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-000038b0: 7365 6c66 2e6e 6d6f 6465 6c73 293a 0a20  self.nmodels):. 
+000037c0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+000037d0: 6e63 6528 6172 672e 7374 6570 2c66 6c6f  nce(arg.step,flo
+000037e0: 6174 2920 6f72 2069 7369 6e73 7461 6e63  at) or isinstanc
+000037f0: 6528 6172 672e 7374 6570 2c69 6e74 293a  e(arg.step,int):
+00003800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003810: 2020 2020 2020 2020 2020 2020 206c 6f77               low
+00003820: 6572 2c75 7070 6572 3d61 7267 2e73 746f  er,upper=arg.sto
+00003830: 702c 6172 672e 7374 6570 0a20 2020 2020  p,arg.step.     
+00003840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003850: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00003860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003870: 2020 2020 2075 7070 6572 3d61 7267 2e73       upper=arg.s
+00003880: 746f 700a 2020 2020 2020 2020 2020 2020  top.            
+00003890: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000038a0: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
+000038b0: 6e6d 6f64 656c 7329 3a0a 2020 2020 2020  nmodels):.      
 000038c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038d0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-000038e0: 6c66 2e6d 6f64 656c 735b 695d 2e6e 4865  lf.models[i].nHe
-000038f0: 2069 6e20 6172 672e 7374 6f70 3a0a 2020   in arg.stop:.  
-00003900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003910: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00003920: 745f 6461 7461 2e61 6464 5f6d 6f64 656c  t_data.add_model
-00003930: 2873 656c 662e 6d6f 6465 6c73 5b69 5d29  (self.models[i])
-00003940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003950: 2065 6c69 6620 6172 672e 7374 6172 743d   elif arg.start=
-00003960: 3d27 6e48 4949 273a 0a20 2020 2020 2020  ='nHII':.       
-00003970: 2020 2020 2020 2020 2020 2020 2075 7070               upp
-00003980: 6572 3d6e 702e 6e61 6e0a 2020 2020 2020  er=np.nan.      
-00003990: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-000039a0: 7765 723d 6e70 2e6e 616e 0a20 2020 2020  wer=np.nan.     
-000039b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000039c0: 6620 6973 696e 7374 616e 6365 2861 7267  f isinstance(arg
-000039d0: 2e73 746f 702c 666c 6f61 7429 206f 7220  .stop,float) or 
-000039e0: 6973 696e 7374 616e 6365 2861 7267 2e73  isinstance(arg.s
-000039f0: 746f 702c 696e 7429 3a0a 2020 2020 2020  top,int):.      
+000038d0: 2020 2020 2020 6966 206e 6f74 206e 702e        if not np.
+000038e0: 6973 6e61 6e28 6c6f 7765 7229 3a0a 2020  isnan(lower):.  
+000038f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003900: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00003910: 2073 656c 662e 6d6f 6465 6c73 5b69 5d2e   self.models[i].
+00003920: 6e48 653c 7570 7065 7220 616e 6420 7365  nHe<upper and se
+00003930: 6c66 2e6d 6f64 656c 735b 695d 2e6e 4865  lf.models[i].nHe
+00003940: 3e6c 6f77 6572 3a0a 2020 2020 2020 2020  >lower:.        
+00003950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003960: 2020 2020 2020 2020 2020 2020 7265 745f              ret_
+00003970: 6461 7461 2e61 6464 5f6d 6f64 656c 2873  data.add_model(s
+00003980: 656c 662e 6d6f 6465 6c73 5b69 5d29 0a20  elf.models[i]). 
+00003990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039a0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000039b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000039c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039d0: 2069 6620 7365 6c66 2e6d 6f64 656c 735b   if self.models[
+000039e0: 695d 2e6e 4865 3d3d 7570 7065 723a 0a20  i].nHe==upper:. 
+000039f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a10: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00003a20: 6172 672e 7374 6570 2c66 6c6f 6174 2920  arg.step,float) 
-00003a30: 6f72 2069 7369 6e73 7461 6e63 6528 6172  or isinstance(ar
-00003a40: 672e 7374 6570 2c69 6e74 293a 0a20 2020  g.step,int):.   
-00003a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a60: 2020 2020 2020 2020 206c 6f77 6572 2c75           lower,u
-00003a70: 7070 6572 3d61 7267 2e73 746f 702c 6172  pper=arg.stop,ar
-00003a80: 672e 7374 6570 0a20 2020 2020 2020 2020  g.step.         
-00003a90: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00003aa0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00003ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ac0: 2075 7070 6572 3d61 7267 2e73 746f 700a   upper=arg.stop.
-00003ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ae0: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00003af0: 2072 616e 6765 2873 656c 662e 6e6d 6f64   range(self.nmod
-00003b00: 656c 7329 3a0a 2020 2020 2020 2020 2020  els):.          
-00003b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b20: 2020 6966 206e 6f74 206e 702e 6973 6e61    if not np.isna
-00003b30: 6e28 6c6f 7765 7229 3a0a 2020 2020 2020  n(lower):.      
-00003b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b50: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00003b60: 662e 6d6f 6465 6c73 5b69 5d2e 6e48 4949  f.models[i].nHII
-00003b70: 3c75 7070 6572 2061 6e64 2073 656c 662e  <upper and self.
-00003b80: 6d6f 6465 6c73 5b69 5d2e 6e48 4949 3e6c  models[i].nHII>l
-00003b90: 6f77 6572 3a0a 2020 2020 2020 2020 2020  ower:.          
-00003ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003bb0: 2020 2020 2020 2020 2020 7265 745f 6461            ret_da
-00003bc0: 7461 2e61 6464 5f6d 6f64 656c 2873 656c  ta.add_model(sel
-00003bd0: 662e 6d6f 6465 6c73 5b69 5d29 0a20 2020  f.models[i]).   
+00003a10: 2020 2072 6574 5f64 6174 612e 6164 645f     ret_data.add_
+00003a20: 6d6f 6465 6c28 7365 6c66 2e6d 6f64 656c  model(self.model
+00003a30: 735b 695d 290a 2020 2020 2020 2020 2020  s[i]).          
+00003a40: 2020 2020 2020 2020 2020 656c 6966 2069            elif i
+00003a50: 7369 6e73 7461 6e63 6528 6172 672e 7374  sinstance(arg.st
+00003a60: 6f70 2c6c 6973 7429 3a0a 0a20 2020 2020  op,list):..     
+00003a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a80: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+00003a90: 6528 7365 6c66 2e6e 6d6f 6465 6c73 293a  e(self.nmodels):
+00003aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003ab0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00003ac0: 7365 6c66 2e6d 6f64 656c 735b 695d 2e6e  self.models[i].n
+00003ad0: 4865 2069 6e20 6172 672e 7374 6f70 3a0a  He in arg.stop:.
+00003ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b00: 7265 745f 6461 7461 2e61 6464 5f6d 6f64  ret_data.add_mod
+00003b10: 656c 2873 656c 662e 6d6f 6465 6c73 5b69  el(self.models[i
+00003b20: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+00003b30: 2020 2065 6c69 6620 6172 672e 7374 6172     elif arg.star
+00003b40: 743d 3d27 6e48 4949 273a 0a20 2020 2020  t=='nHII':.     
+00003b50: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+00003b60: 7070 6572 3d6e 702e 6e61 6e0a 2020 2020  pper=np.nan.    
+00003b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b80: 6c6f 7765 723d 6e70 2e6e 616e 0a20 2020  lower=np.nan.   
+00003b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ba0: 2069 6620 6973 696e 7374 616e 6365 2861   if isinstance(a
+00003bb0: 7267 2e73 746f 702c 666c 6f61 7429 206f  rg.stop,float) o
+00003bc0: 7220 6973 696e 7374 616e 6365 2861 7267  r isinstance(arg
+00003bd0: 2e73 746f 702c 696e 7429 3a0a 2020 2020  .stop,int):.    
 00003be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003bf0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00003c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c10: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00003c20: 6620 7365 6c66 2e6d 6f64 656c 735b 695d  f self.models[i]
-00003c30: 2e6e 4849 493d 3d75 7070 6572 3a0a 2020  .nHII==upper:.  
-00003c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c60: 2020 7265 745f 6461 7461 2e61 6464 5f6d    ret_data.add_m
-00003c70: 6f64 656c 2873 656c 662e 6d6f 6465 6c73  odel(self.models
-00003c80: 5b69 5d29 0a20 2020 2020 2020 2020 2020  [i]).           
-00003c90: 2020 2020 2020 2020 2065 6c69 6620 6973           elif is
-00003ca0: 696e 7374 616e 6365 2861 7267 2e73 746f  instance(arg.sto
-00003cb0: 702c 6c69 7374 293a 0a20 2020 2020 2020  p,list):.       
-00003cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003cd0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-00003ce0: 7365 6c66 2e6e 6d6f 6465 6c73 293a 0a20  self.nmodels):. 
+00003bf0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00003c00: 6528 6172 672e 7374 6570 2c66 6c6f 6174  e(arg.step,float
+00003c10: 2920 6f72 2069 7369 6e73 7461 6e63 6528  ) or isinstance(
+00003c20: 6172 672e 7374 6570 2c69 6e74 293a 0a20  arg.step,int):. 
+00003c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c40: 2020 2020 2020 2020 2020 206c 6f77 6572             lower
+00003c50: 2c75 7070 6572 3d61 7267 2e73 746f 702c  ,upper=arg.stop,
+00003c60: 6172 672e 7374 6570 0a20 2020 2020 2020  arg.step.       
+00003c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c80: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00003c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ca0: 2020 2075 7070 6572 3d61 7267 2e73 746f     upper=arg.sto
+00003cb0: 700a 2020 2020 2020 2020 2020 2020 2020  p.              
+00003cc0: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
+00003cd0: 696e 2072 616e 6765 2873 656c 662e 6e6d  in range(self.nm
+00003ce0: 6f64 656c 7329 3a0a 2020 2020 2020 2020  odels):.        
 00003cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d00: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00003d10: 6c66 2e6d 6f64 656c 735b 695d 2e6e 4849  lf.models[i].nHI
-00003d20: 4920 696e 2061 7267 2e73 746f 703a 0a20  I in arg.stop:. 
-00003d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d40: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00003d50: 6574 5f64 6174 612e 6164 645f 6d6f 6465  et_data.add_mode
-00003d60: 6c28 7365 6c66 2e6d 6f64 656c 735b 695d  l(self.models[i]
-00003d70: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00003d80: 2020 656c 6966 2061 7267 2e73 7461 7274    elif arg.start
-00003d90: 3d3d 276e 4849 273a 0a20 2020 2020 2020  =='nHI':.       
-00003da0: 2020 2020 2020 2020 2020 2020 2075 7070               upp
-00003db0: 6572 3d6e 702e 6e61 6e0a 2020 2020 2020  er=np.nan.      
-00003dc0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00003dd0: 7765 723d 6e70 2e6e 616e 0a20 2020 2020  wer=np.nan.     
-00003de0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00003df0: 6620 6973 696e 7374 616e 6365 2861 7267  f isinstance(arg
-00003e00: 2e73 746f 702c 666c 6f61 7429 206f 7220  .stop,float) or 
-00003e10: 6973 696e 7374 616e 6365 2861 7267 2e73  isinstance(arg.s
-00003e20: 746f 702c 696e 7429 3a0a 2020 2020 2020  top,int):.      
+00003d00: 2020 2020 6966 206e 6f74 206e 702e 6973      if not np.is
+00003d10: 6e61 6e28 6c6f 7765 7229 3a0a 2020 2020  nan(lower):.    
+00003d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d30: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00003d40: 656c 662e 6d6f 6465 6c73 5b69 5d2e 6e48  elf.models[i].nH
+00003d50: 4949 3c75 7070 6572 2061 6e64 2073 656c  II<upper and sel
+00003d60: 662e 6d6f 6465 6c73 5b69 5d2e 6e48 4949  f.models[i].nHII
+00003d70: 3e6c 6f77 6572 3a0a 2020 2020 2020 2020  >lower:.        
+00003d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d90: 2020 2020 2020 2020 2020 2020 7265 745f              ret_
+00003da0: 6461 7461 2e61 6464 5f6d 6f64 656c 2873  data.add_model(s
+00003db0: 656c 662e 6d6f 6465 6c73 5b69 5d29 0a20  elf.models[i]). 
+00003dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003dd0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00003de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e00: 2069 6620 7365 6c66 2e6d 6f64 656c 735b   if self.models[
+00003e10: 695d 2e6e 4849 493d 3d75 7070 6572 3a0a  i].nHII==upper:.
+00003e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e40: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00003e50: 6172 672e 7374 6570 2c66 6c6f 6174 2920  arg.step,float) 
-00003e60: 6f72 2069 7369 6e73 7461 6e63 6528 6172  or isinstance(ar
-00003e70: 672e 7374 6570 2c69 6e74 293a 0a20 2020  g.step,int):.   
-00003e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e90: 2020 2020 2020 2020 206c 6f77 6572 2c75           lower,u
-00003ea0: 7070 6572 3d61 7267 2e73 746f 702c 6172  pper=arg.stop,ar
-00003eb0: 672e 7374 6570 0a20 2020 2020 2020 2020  g.step.         
-00003ec0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00003ed0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00003ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ef0: 2075 7070 6572 3d61 7267 2e73 746f 700a   upper=arg.stop.
-00003f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f10: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00003f20: 2072 616e 6765 2873 656c 662e 6e6d 6f64   range(self.nmod
-00003f30: 656c 7329 3a0a 2020 2020 2020 2020 2020  els):.          
-00003f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f50: 2020 6966 206e 6f74 206e 702e 6973 6e61    if not np.isna
-00003f60: 6e28 6c6f 7765 7229 3a0a 2020 2020 2020  n(lower):.      
-00003f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f80: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00003f90: 662e 6d6f 6465 6c73 5b69 5d2e 6e48 493c  f.models[i].nHI<
-00003fa0: 7570 7065 7220 616e 6420 7365 6c66 2e6d  upper and self.m
-00003fb0: 6f64 656c 735b 695d 2e6e 4849 3e6c 6f77  odels[i].nHI>low
-00003fc0: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
-00003fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003fe0: 2020 2020 2020 2020 7265 745f 6461 7461          ret_data
-00003ff0: 2e61 6464 5f6d 6f64 656c 2873 656c 662e  .add_model(self.
-00004000: 6d6f 6465 6c73 5b69 5d29 0a20 2020 2020  models[i]).     
+00003e40: 2020 2020 7265 745f 6461 7461 2e61 6464      ret_data.add
+00003e50: 5f6d 6f64 656c 2873 656c 662e 6d6f 6465  _model(self.mode
+00003e60: 6c73 5b69 5d29 0a20 2020 2020 2020 2020  ls[i]).         
+00003e70: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00003e80: 6973 696e 7374 616e 6365 2861 7267 2e73  isinstance(arg.s
+00003e90: 746f 702c 6c69 7374 293a 0a20 2020 2020  top,list):.     
+00003ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003eb0: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+00003ec0: 6528 7365 6c66 2e6e 6d6f 6465 6c73 293a  e(self.nmodels):
+00003ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003ee0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00003ef0: 7365 6c66 2e6d 6f64 656c 735b 695d 2e6e  self.models[i].n
+00003f00: 4849 4920 696e 2061 7267 2e73 746f 703a  HII in arg.stop:
+00003f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f30: 2072 6574 5f64 6174 612e 6164 645f 6d6f   ret_data.add_mo
+00003f40: 6465 6c28 7365 6c66 2e6d 6f64 656c 735b  del(self.models[
+00003f50: 695d 290a 2020 2020 2020 2020 2020 2020  i]).            
+00003f60: 2020 2020 656c 6966 2061 7267 2e73 7461      elif arg.sta
+00003f70: 7274 3d3d 276e 4849 273a 0a20 2020 2020  rt=='nHI':.     
+00003f80: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+00003f90: 7070 6572 3d6e 702e 6e61 6e0a 2020 2020  pper=np.nan.    
+00003fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003fb0: 6c6f 7765 723d 6e70 2e6e 616e 0a20 2020  lower=np.nan.   
+00003fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003fd0: 2069 6620 6973 696e 7374 616e 6365 2861   if isinstance(a
+00003fe0: 7267 2e73 746f 702c 666c 6f61 7429 206f  rg.stop,float) o
+00003ff0: 7220 6973 696e 7374 616e 6365 2861 7267  r isinstance(arg
+00004000: 2e73 746f 702c 696e 7429 3a0a 2020 2020  .stop,int):.    
 00004010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004020: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00004030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004040: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00004050: 7365 6c66 2e6d 6f64 656c 735b 695d 2e6e  self.models[i].n
-00004060: 4849 3d3d 7570 7065 723a 0a20 2020 2020  HI==upper:.     
-00004070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004080: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00004090: 6574 5f64 6174 612e 6164 645f 6d6f 6465  et_data.add_mode
-000040a0: 6c28 7365 6c66 2e6d 6f64 656c 735b 695d  l(self.models[i]
-000040b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000040c0: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
-000040d0: 7461 6e63 6528 6172 672e 7374 6f70 2c6c  tance(arg.stop,l
-000040e0: 6973 7429 3a0a 2020 2020 2020 2020 2020  ist):.          
-000040f0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00004100: 7220 6920 696e 2072 616e 6765 2873 656c  r i in range(sel
-00004110: 662e 6e6d 6f64 656c 7329 3a0a 2020 2020  f.nmodels):.    
+00004020: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00004030: 6528 6172 672e 7374 6570 2c66 6c6f 6174  e(arg.step,float
+00004040: 2920 6f72 2069 7369 6e73 7461 6e63 6528  ) or isinstance(
+00004050: 6172 672e 7374 6570 2c69 6e74 293a 0a20  arg.step,int):. 
+00004060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004070: 2020 2020 2020 2020 2020 206c 6f77 6572             lower
+00004080: 2c75 7070 6572 3d61 7267 2e73 746f 702c  ,upper=arg.stop,
+00004090: 6172 672e 7374 6570 0a20 2020 2020 2020  arg.step.       
+000040a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000040b0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000040c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000040d0: 2020 2075 7070 6572 3d61 7267 2e73 746f     upper=arg.sto
+000040e0: 700a 2020 2020 2020 2020 2020 2020 2020  p.              
+000040f0: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
+00004100: 696e 2072 616e 6765 2873 656c 662e 6e6d  in range(self.nm
+00004110: 6f64 656c 7329 3a0a 2020 2020 2020 2020  odels):.        
 00004120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004130: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00004140: 6d6f 6465 6c73 5b69 5d2e 6e48 4920 696e  models[i].nHI in
-00004150: 2061 7267 2e73 746f 703a 0a20 2020 2020   arg.stop:.     
-00004160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004170: 2020 2020 2020 2020 2020 2072 6574 5f64             ret_d
-00004180: 6174 612e 6164 645f 6d6f 6465 6c28 7365  ata.add_model(se
-00004190: 6c66 2e6d 6f64 656c 735b 695d 290a 2020  lf.models[i]).  
-000041a0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-000041b0: 6966 2061 7267 2e73 7461 7274 3d3d 276e  if arg.start=='n
-000041c0: 4832 273a 0a20 2020 2020 2020 2020 2020  H2':.           
-000041d0: 2020 2020 2020 2020 2075 7070 6572 3d6e           upper=n
-000041e0: 702e 6e61 6e0a 2020 2020 2020 2020 2020  p.nan.          
-000041f0: 2020 2020 2020 2020 2020 6c6f 7765 723d            lower=
-00004200: 6e70 2e6e 616e 0a20 2020 2020 2020 2020  np.nan.         
-00004210: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-00004220: 696e 7374 616e 6365 2861 7267 2e73 746f  instance(arg.sto
-00004230: 702c 666c 6f61 7429 206f 7220 6973 696e  p,float) or isin
-00004240: 7374 616e 6365 2861 7267 2e73 746f 702c  stance(arg.stop,
-00004250: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
-00004260: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00004270: 2069 7369 6e73 7461 6e63 6528 6172 672e   isinstance(arg.
-00004280: 7374 6570 2c66 6c6f 6174 2920 6f72 2069  step,float) or i
-00004290: 7369 6e73 7461 6e63 6528 6172 672e 7374  sinstance(arg.st
-000042a0: 6570 2c69 6e74 293a 0a20 2020 2020 2020  ep,int):.       
-000042b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000042c0: 2020 2020 206c 6f77 6572 2c75 7070 6572       lower,upper
-000042d0: 3d61 7267 2e73 746f 702c 6172 672e 7374  =arg.stop,arg.st
-000042e0: 6570 0a20 2020 2020 2020 2020 2020 2020  ep.             
-000042f0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00004300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004310: 2020 2020 2020 2020 2020 2020 2075 7070               upp
-00004320: 6572 3d61 7267 2e73 746f 700a 2020 2020  er=arg.stop.    
-00004330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004340: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00004350: 6765 2873 656c 662e 6e6d 6f64 656c 7329  ge(self.nmodels)
-00004360: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00004370: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00004380: 206e 6f74 206e 702e 6973 6e61 6e28 6c6f   not np.isnan(lo
-00004390: 7765 7229 3a0a 2020 2020 2020 2020 2020  wer):.          
-000043a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000043b0: 2020 2020 2020 6966 2073 656c 662e 6d6f        if self.mo
-000043c0: 6465 6c73 5b69 5d2e 6e48 323c 7570 7065  dels[i].nH2<uppe
-000043d0: 7220 616e 6420 7365 6c66 2e6d 6f64 656c  r and self.model
-000043e0: 735b 695d 2e6e 4832 3e6c 6f77 6572 3a0a  s[i].nH2>lower:.
-000043f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004410: 2020 2020 7265 745f 6461 7461 2e61 6464      ret_data.add
-00004420: 5f6d 6f64 656c 2873 656c 662e 6d6f 6465  _model(self.mode
-00004430: 6c73 5b69 5d29 0a20 2020 2020 2020 2020  ls[i]).         
+00004130: 2020 2020 6966 206e 6f74 206e 702e 6973      if not np.is
+00004140: 6e61 6e28 6c6f 7765 7229 3a0a 2020 2020  nan(lower):.    
+00004150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004160: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00004170: 656c 662e 6d6f 6465 6c73 5b69 5d2e 6e48  elf.models[i].nH
+00004180: 493c 7570 7065 7220 616e 6420 7365 6c66  I<upper and self
+00004190: 2e6d 6f64 656c 735b 695d 2e6e 4849 3e6c  .models[i].nHI>l
+000041a0: 6f77 6572 3a0a 2020 2020 2020 2020 2020  ower:.          
+000041b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000041c0: 2020 2020 2020 2020 2020 7265 745f 6461            ret_da
+000041d0: 7461 2e61 6464 5f6d 6f64 656c 2873 656c  ta.add_model(sel
+000041e0: 662e 6d6f 6465 6c73 5b69 5d29 0a20 2020  f.models[i]).   
+000041f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004200: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00004210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004220: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00004230: 6620 7365 6c66 2e6d 6f64 656c 735b 695d  f self.models[i]
+00004240: 2e6e 4849 3d3d 7570 7065 723a 0a20 2020  .nHI==upper:.   
+00004250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004270: 2072 6574 5f64 6174 612e 6164 645f 6d6f   ret_data.add_mo
+00004280: 6465 6c28 7365 6c66 2e6d 6f64 656c 735b  del(self.models[
+00004290: 695d 290a 2020 2020 2020 2020 2020 2020  i]).            
+000042a0: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
+000042b0: 6e73 7461 6e63 6528 6172 672e 7374 6f70  nstance(arg.stop
+000042c0: 2c6c 6973 7429 3a0a 2020 2020 2020 2020  ,list):.        
+000042d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000042e0: 666f 7220 6920 696e 2072 616e 6765 2873  for i in range(s
+000042f0: 656c 662e 6e6d 6f64 656c 7329 3a0a 2020  elf.nmodels):.  
+00004300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004310: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00004320: 662e 6d6f 6465 6c73 5b69 5d2e 6e48 4920  f.models[i].nHI 
+00004330: 696e 2061 7267 2e73 746f 703a 0a20 2020  in arg.stop:.   
+00004340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004350: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00004360: 5f64 6174 612e 6164 645f 6d6f 6465 6c28  _data.add_model(
+00004370: 7365 6c66 2e6d 6f64 656c 735b 695d 290a  self.models[i]).
+00004380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004390: 656c 6966 2061 7267 2e73 7461 7274 3d3d  elif arg.start==
+000043a0: 276e 4832 273a 0a20 2020 2020 2020 2020  'nH2':.         
+000043b0: 2020 2020 2020 2020 2020 2075 7070 6572             upper
+000043c0: 3d6e 702e 6e61 6e0a 2020 2020 2020 2020  =np.nan.        
+000043d0: 2020 2020 2020 2020 2020 2020 6c6f 7765              lowe
+000043e0: 723d 6e70 2e6e 616e 0a20 2020 2020 2020  r=np.nan.       
+000043f0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00004400: 6973 696e 7374 616e 6365 2861 7267 2e73  isinstance(arg.s
+00004410: 746f 702c 666c 6f61 7429 206f 7220 6973  top,float) or is
+00004420: 696e 7374 616e 6365 2861 7267 2e73 746f  instance(arg.sto
+00004430: 702c 696e 7429 3a0a 2020 2020 2020 2020  p,int):.        
 00004440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004450: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00004460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004470: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00004480: 2e6d 6f64 656c 735b 695d 2e6e 4832 3d3d  .models[i].nH2==
-00004490: 7570 7065 723a 0a20 2020 2020 2020 2020  upper:.         
-000044a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044b0: 2020 2020 2020 2020 2020 2072 6574 5f64             ret_d
-000044c0: 6174 612e 6164 645f 6d6f 6465 6c28 7365  ata.add_model(se
-000044d0: 6c66 2e6d 6f64 656c 735b 695d 290a 2020  lf.models[i]).  
-000044e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044f0: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
-00004500: 6528 6172 672e 7374 6f70 2c6c 6973 7429  e(arg.stop,list)
-00004510: 3a0a 0a20 2020 2020 2020 2020 2020 2020  :..             
-00004520: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-00004530: 2069 6e20 7261 6e67 6528 7365 6c66 2e6e   in range(self.n
-00004540: 6d6f 6465 6c73 293a 0a20 2020 2020 2020  models):.       
+00004450: 6966 2069 7369 6e73 7461 6e63 6528 6172  if isinstance(ar
+00004460: 672e 7374 6570 2c66 6c6f 6174 2920 6f72  g.step,float) or
+00004470: 2069 7369 6e73 7461 6e63 6528 6172 672e   isinstance(arg.
+00004480: 7374 6570 2c69 6e74 293a 0a20 2020 2020  step,int):.     
+00004490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044a0: 2020 2020 2020 206c 6f77 6572 2c75 7070         lower,upp
+000044b0: 6572 3d61 7267 2e73 746f 702c 6172 672e  er=arg.stop,arg.
+000044c0: 7374 6570 0a20 2020 2020 2020 2020 2020  step.           
+000044d0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+000044e0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000044f0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+00004500: 7070 6572 3d61 7267 2e73 746f 700a 2020  pper=arg.stop.  
+00004510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004520: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+00004530: 616e 6765 2873 656c 662e 6e6d 6f64 656c  ange(self.nmodel
+00004540: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
 00004550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004560: 2020 2020 2069 6620 7365 6c66 2e6d 6f64       if self.mod
-00004570: 656c 735b 695d 2e6e 4832 2069 6e20 6172  els[i].nH2 in ar
-00004580: 672e 7374 6f70 3a0a 2020 2020 2020 2020  g.stop:.        
-00004590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045a0: 2020 2020 2020 2020 7265 745f 6461 7461          ret_data
-000045b0: 2e61 6464 5f6d 6f64 656c 2873 656c 662e  .add_model(self.
-000045c0: 6d6f 6465 6c73 5b69 5d29 0a20 2020 2020  models[i]).     
-000045d0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-000045e0: 6172 672e 7374 6172 743d 3d27 6475 7374  arg.start=='dust
-000045f0: 5f74 6f5f 6761 7327 3a0a 2020 2020 2020  _to_gas':.      
-00004600: 2020 2020 2020 2020 2020 2020 2020 7570                up
-00004610: 7065 723d 6e70 2e6e 616e 0a20 2020 2020  per=np.nan.     
-00004620: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00004630: 6f77 6572 3d6e 702e 6e61 6e0a 2020 2020  ower=np.nan.    
+00004560: 6966 206e 6f74 206e 702e 6973 6e61 6e28  if not np.isnan(
+00004570: 6c6f 7765 7229 3a0a 2020 2020 2020 2020  lower):.        
+00004580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004590: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000045a0: 6d6f 6465 6c73 5b69 5d2e 6e48 323c 7570  models[i].nH2<up
+000045b0: 7065 7220 616e 6420 7365 6c66 2e6d 6f64  per and self.mod
+000045c0: 656c 735b 695d 2e6e 4832 3e6c 6f77 6572  els[i].nH2>lower
+000045d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000045e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000045f0: 2020 2020 2020 7265 745f 6461 7461 2e61        ret_data.a
+00004600: 6464 5f6d 6f64 656c 2873 656c 662e 6d6f  dd_model(self.mo
+00004610: 6465 6c73 5b69 5d29 0a20 2020 2020 2020  dels[i]).       
+00004620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004630: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
 00004640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004650: 6966 2069 7369 6e73 7461 6e63 6528 6172  if isinstance(ar
-00004660: 672e 7374 6f70 2c66 6c6f 6174 2920 6f72  g.stop,float) or
-00004670: 2069 7369 6e73 7461 6e63 6528 6172 672e   isinstance(arg.
-00004680: 7374 6f70 2c69 6e74 293a 0a20 2020 2020  stop,int):.     
-00004690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046a0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-000046b0: 2861 7267 2e73 7465 702c 666c 6f61 7429  (arg.step,float)
-000046c0: 206f 7220 6973 696e 7374 616e 6365 2861   or isinstance(a
-000046d0: 7267 2e73 7465 702c 696e 7429 3a0a 2020  rg.step,int):.  
-000046e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046f0: 2020 2020 2020 2020 2020 6c6f 7765 722c            lower,
-00004700: 7570 7065 723d 6172 672e 7374 6f70 2c61  upper=arg.stop,a
-00004710: 7267 2e73 7465 700a 2020 2020 2020 2020  rg.step.        
-00004720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004730: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00004740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004750: 2020 7570 7065 723d 6172 672e 7374 6f70    upper=arg.stop
-00004760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004770: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-00004780: 6e20 7261 6e67 6528 7365 6c66 2e6e 6d6f  n range(self.nmo
-00004790: 6465 6c73 293a 0a20 2020 2020 2020 2020  dels):.         
-000047a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047b0: 2020 2069 6620 6e6f 7420 6e70 2e69 736e     if not np.isn
-000047c0: 616e 286c 6f77 6572 293a 0a20 2020 2020  an(lower):.     
-000047d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047e0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-000047f0: 6c66 2e6d 6f64 656c 735b 695d 2e64 7573  lf.models[i].dus
-00004800: 745f 746f 5f67 6173 3c75 7070 6572 2061  t_to_gas<upper a
-00004810: 6e64 2073 656c 662e 6d6f 6465 6c73 5b69  nd self.models[i
-00004820: 5d2e 6475 7374 5f74 6f5f 6761 733e 6c6f  ].dust_to_gas>lo
-00004830: 7765 723a 0a20 2020 2020 2020 2020 2020  wer:.           
-00004840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004850: 2020 2020 2020 2020 2072 6574 5f64 6174           ret_dat
-00004860: 612e 6164 645f 6d6f 6465 6c28 7365 6c66  a.add_model(self
-00004870: 2e6d 6f64 656c 735b 695d 290a 2020 2020  .models[i]).    
-00004880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004890: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000048a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048b0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000048c0: 2073 656c 662e 6d6f 6465 6c73 5b69 5d2e   self.models[i].
-000048d0: 6475 7374 5f74 6f5f 6761 733d 3d75 7070  dust_to_gas==upp
-000048e0: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
-000048f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004900: 2020 2020 2020 2020 7265 745f 6461 7461          ret_data
-00004910: 2e61 6464 5f6d 6f64 656c 2873 656c 662e  .add_model(self.
-00004920: 6d6f 6465 6c73 5b69 5d29 0a20 2020 2020  models[i]).     
-00004930: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00004940: 6c69 6620 6973 696e 7374 616e 6365 2861  lif isinstance(a
-00004950: 7267 2e73 746f 702c 6c69 7374 293a 0a0a  rg.stop,list):..
-00004960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004970: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00004980: 2072 616e 6765 2873 656c 662e 6e6d 6f64   range(self.nmod
-00004990: 656c 7329 3a0a 2020 2020 2020 2020 2020  els):.          
-000049a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049b0: 2020 6966 2073 656c 662e 6d6f 6465 6c73    if self.models
-000049c0: 5b69 5d2e 6475 7374 5f74 6f5f 6761 7320  [i].dust_to_gas 
-000049d0: 696e 2061 7267 2e73 746f 703a 0a20 2020  in arg.stop:.   
-000049e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049f0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00004a00: 5f64 6174 612e 6164 645f 6d6f 6465 6c28  _data.add_model(
-00004a10: 7365 6c66 2e6d 6f64 656c 735b 695d 290a  self.models[i]).
+00004650: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00004660: 6c66 2e6d 6f64 656c 735b 695d 2e6e 4832  lf.models[i].nH2
+00004670: 3d3d 7570 7065 723a 0a20 2020 2020 2020  ==upper:.       
+00004680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004690: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+000046a0: 5f64 6174 612e 6164 645f 6d6f 6465 6c28  _data.add_model(
+000046b0: 7365 6c66 2e6d 6f64 656c 735b 695d 290a  self.models[i]).
+000046c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046d0: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
+000046e0: 6e63 6528 6172 672e 7374 6f70 2c6c 6973  nce(arg.stop,lis
+000046f0: 7429 3a0a 0a20 2020 2020 2020 2020 2020  t):..           
+00004700: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00004710: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
+00004720: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
+00004730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004740: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
+00004750: 6f64 656c 735b 695d 2e6e 4832 2069 6e20  odels[i].nH2 in 
+00004760: 6172 672e 7374 6f70 3a0a 2020 2020 2020  arg.stop:.      
+00004770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004780: 2020 2020 2020 2020 2020 7265 745f 6461            ret_da
+00004790: 7461 2e61 6464 5f6d 6f64 656c 2873 656c  ta.add_model(sel
+000047a0: 662e 6d6f 6465 6c73 5b69 5d29 0a20 2020  f.models[i]).   
+000047b0: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+000047c0: 6620 6172 672e 7374 6172 743d 3d27 6475  f arg.start=='du
+000047d0: 7374 5f74 6f5f 6761 7327 3a0a 2020 2020  st_to_gas':.    
+000047e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047f0: 7570 7065 723d 6e70 2e6e 616e 0a20 2020  upper=np.nan.   
+00004800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004810: 206c 6f77 6572 3d6e 702e 6e61 6e0a 2020   lower=np.nan.  
+00004820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004830: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00004840: 6172 672e 7374 6f70 2c66 6c6f 6174 2920  arg.stop,float) 
+00004850: 6f72 2069 7369 6e73 7461 6e63 6528 6172  or isinstance(ar
+00004860: 672e 7374 6f70 2c69 6e74 293a 0a20 2020  g.stop,int):.   
+00004870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004880: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+00004890: 6365 2861 7267 2e73 7465 702c 666c 6f61  ce(arg.step,floa
+000048a0: 7429 206f 7220 6973 696e 7374 616e 6365  t) or isinstance
+000048b0: 2861 7267 2e73 7465 702c 696e 7429 3a0a  (arg.step,int):.
+000048c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048d0: 2020 2020 2020 2020 2020 2020 6c6f 7765              lowe
+000048e0: 722c 7570 7065 723d 6172 672e 7374 6f70  r,upper=arg.stop
+000048f0: 2c61 7267 2e73 7465 700a 2020 2020 2020  ,arg.step.      
+00004900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004910: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00004920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004930: 2020 2020 7570 7065 723d 6172 672e 7374      upper=arg.st
+00004940: 6f70 0a20 2020 2020 2020 2020 2020 2020  op.             
+00004950: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+00004960: 2069 6e20 7261 6e67 6528 7365 6c66 2e6e   in range(self.n
+00004970: 6d6f 6465 6c73 293a 0a20 2020 2020 2020  models):.       
+00004980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004990: 2020 2020 2069 6620 6e6f 7420 6e70 2e69       if not np.i
+000049a0: 736e 616e 286c 6f77 6572 293a 0a20 2020  snan(lower):.   
+000049b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000049c0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000049d0: 7365 6c66 2e6d 6f64 656c 735b 695d 2e64  self.models[i].d
+000049e0: 7573 745f 746f 5f67 6173 3c75 7070 6572  ust_to_gas<upper
+000049f0: 2061 6e64 2073 656c 662e 6d6f 6465 6c73   and self.models
+00004a00: 5b69 5d2e 6475 7374 5f74 6f5f 6761 733e  [i].dust_to_gas>
+00004a10: 6c6f 7765 723a 0a20 2020 2020 2020 2020  lower:.         
 00004a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a30: 656c 6966 2061 7267 2e73 7461 7274 3d3d  elif arg.start==
-00004a40: 2776 7475 7262 273a 0a20 2020 2020 2020  'vturb':.       
-00004a50: 2020 2020 2020 2020 2020 2020 2075 7070               upp
-00004a60: 6572 3d6e 702e 6e61 6e0a 2020 2020 2020  er=np.nan.      
-00004a70: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00004a80: 7765 723d 6e70 2e6e 616e 0a20 2020 2020  wer=np.nan.     
-00004a90: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00004aa0: 6620 6973 696e 7374 616e 6365 2861 7267  f isinstance(arg
-00004ab0: 2e73 746f 702c 666c 6f61 7429 206f 7220  .stop,float) or 
-00004ac0: 6973 696e 7374 616e 6365 2861 7267 2e73  isinstance(arg.s
-00004ad0: 746f 702c 696e 7429 3a0a 2020 2020 2020  top,int):.      
-00004ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004af0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00004b00: 6172 672e 7374 6570 2c66 6c6f 6174 2920  arg.step,float) 
-00004b10: 6f72 2069 7369 6e73 7461 6e63 6528 6172  or isinstance(ar
-00004b20: 672e 7374 6570 2c69 6e74 293a 0a20 2020  g.step,int):.   
-00004b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b40: 2020 2020 2020 2020 206c 6f77 6572 2c75           lower,u
-00004b50: 7070 6572 3d61 7267 2e73 746f 702c 6172  pper=arg.stop,ar
-00004b60: 672e 7374 6570 0a20 2020 2020 2020 2020  g.step.         
-00004b70: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00004b80: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00004b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ba0: 2075 7070 6572 3d61 7267 2e73 746f 700a   upper=arg.stop.
-00004bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004bc0: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00004bd0: 2072 616e 6765 2873 656c 662e 6e6d 6f64   range(self.nmod
-00004be0: 656c 7329 3a0a 2020 2020 2020 2020 2020  els):.          
-00004bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c00: 2020 6966 206e 6f74 206e 702e 6973 6e61    if not np.isna
-00004c10: 6e28 6c6f 7765 7229 3a0a 2020 2020 2020  n(lower):.      
-00004c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c30: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00004c40: 662e 6d6f 6465 6c73 5b69 5d2e 7674 7572  f.models[i].vtur
-00004c50: 623c 7570 7065 7220 616e 6420 7365 6c66  b<upper and self
-00004c60: 2e6d 6f64 656c 735b 695d 2e76 7475 7262  .models[i].vturb
-00004c70: 3e6c 6f77 6572 3a0a 2020 2020 2020 2020  >lower:.        
-00004c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c90: 2020 2020 2020 2020 2020 2020 7265 745f              ret_
-00004ca0: 6461 7461 2e61 6464 5f6d 6f64 656c 2873  data.add_model(s
-00004cb0: 656c 662e 6d6f 6465 6c73 5b69 5d29 0a20  elf.models[i]). 
+00004a30: 2020 2020 2020 2020 2020 2072 6574 5f64             ret_d
+00004a40: 6174 612e 6164 645f 6d6f 6465 6c28 7365  ata.add_model(se
+00004a50: 6c66 2e6d 6f64 656c 735b 695d 290a 2020  lf.models[i]).  
+00004a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a70: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00004a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004aa0: 6966 2073 656c 662e 6d6f 6465 6c73 5b69  if self.models[i
+00004ab0: 5d2e 6475 7374 5f74 6f5f 6761 733d 3d75  ].dust_to_gas==u
+00004ac0: 7070 6572 3a0a 2020 2020 2020 2020 2020  pper:.          
+00004ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ae0: 2020 2020 2020 2020 2020 7265 745f 6461            ret_da
+00004af0: 7461 2e61 6464 5f6d 6f64 656c 2873 656c  ta.add_model(sel
+00004b00: 662e 6d6f 6465 6c73 5b69 5d29 0a20 2020  f.models[i]).   
+00004b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b20: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+00004b30: 2861 7267 2e73 746f 702c 6c69 7374 293a  (arg.stop,list):
+00004b40: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004b50: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
+00004b60: 696e 2072 616e 6765 2873 656c 662e 6e6d  in range(self.nm
+00004b70: 6f64 656c 7329 3a0a 2020 2020 2020 2020  odels):.        
+00004b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b90: 2020 2020 6966 2073 656c 662e 6d6f 6465      if self.mode
+00004ba0: 6c73 5b69 5d2e 6475 7374 5f74 6f5f 6761  ls[i].dust_to_ga
+00004bb0: 7320 696e 2061 7267 2e73 746f 703a 0a20  s in arg.stop:. 
+00004bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004bd0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00004be0: 6574 5f64 6174 612e 6164 645f 6d6f 6465  et_data.add_mode
+00004bf0: 6c28 7365 6c66 2e6d 6f64 656c 735b 695d  l(self.models[i]
+00004c00: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00004c10: 2020 656c 6966 2061 7267 2e73 7461 7274    elif arg.start
+00004c20: 3d3d 2776 7475 7262 273a 0a20 2020 2020  =='vturb':.     
+00004c30: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+00004c40: 7070 6572 3d6e 702e 6e61 6e0a 2020 2020  pper=np.nan.    
+00004c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c60: 6c6f 7765 723d 6e70 2e6e 616e 0a20 2020  lower=np.nan.   
+00004c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c80: 2069 6620 6973 696e 7374 616e 6365 2861   if isinstance(a
+00004c90: 7267 2e73 746f 702c 666c 6f61 7429 206f  rg.stop,float) o
+00004ca0: 7220 6973 696e 7374 616e 6365 2861 7267  r isinstance(arg
+00004cb0: 2e73 746f 702c 696e 7429 3a0a 2020 2020  .stop,int):.    
 00004cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cd0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00004ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d00: 2069 6620 7365 6c66 2e6d 6f64 656c 735b   if self.models[
-00004d10: 695d 2e76 7475 7262 3d3d 7570 7065 723a  i].vturb==upper:
-00004d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d40: 2020 2020 2072 6574 5f64 6174 612e 6164       ret_data.ad
-00004d50: 645f 6d6f 6465 6c28 7365 6c66 2e6d 6f64  d_model(self.mod
-00004d60: 656c 735b 695d 290a 2020 2020 2020 2020  els[i]).        
-00004d70: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00004d80: 2069 7369 6e73 7461 6e63 6528 6172 672e   isinstance(arg.
-00004d90: 7374 6f70 2c6c 6973 7429 3a0a 2020 2020  stop,list):.    
-00004da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004db0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00004dc0: 6765 2873 656c 662e 6e6d 6f64 656c 7329  ge(self.nmodels)
-00004dd0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00004de0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00004df0: 2073 656c 662e 6d6f 6465 6c73 5b69 5d2e   self.models[i].
-00004e00: 7674 7572 6220 696e 2061 7267 2e73 746f  vturb in arg.sto
-00004e10: 703a 0a20 2020 2020 2020 2020 2020 2020  p:.             
-00004e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e30: 2020 2072 6574 5f64 6174 612e 6164 645f     ret_data.add_
-00004e40: 6d6f 6465 6c28 7365 6c66 2e6d 6f64 656c  model(self.model
-00004e50: 735b 695d 290a 2020 2020 2020 2020 2020  s[i]).          
-00004e60: 2020 2020 2020 656c 6966 2061 7267 2e73        elif arg.s
-00004e70: 7461 7274 3d3d 2754 6727 3a0a 2020 2020  tart=='Tg':.    
-00004e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e90: 7570 7065 723d 6e70 2e6e 616e 0a20 2020  upper=np.nan.   
-00004ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004eb0: 206c 6f77 6572 3d6e 702e 6e61 6e0a 2020   lower=np.nan.  
-00004ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ed0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00004ee0: 6172 672e 7374 6f70 2c66 6c6f 6174 2920  arg.stop,float) 
-00004ef0: 6f72 2069 7369 6e73 7461 6e63 6528 6172  or isinstance(ar
-00004f00: 672e 7374 6f70 2c69 6e74 293a 0a20 2020  g.stop,int):.   
+00004cd0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00004ce0: 6528 6172 672e 7374 6570 2c66 6c6f 6174  e(arg.step,float
+00004cf0: 2920 6f72 2069 7369 6e73 7461 6e63 6528  ) or isinstance(
+00004d00: 6172 672e 7374 6570 2c69 6e74 293a 0a20  arg.step,int):. 
+00004d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d20: 2020 2020 2020 2020 2020 206c 6f77 6572             lower
+00004d30: 2c75 7070 6572 3d61 7267 2e73 746f 702c  ,upper=arg.stop,
+00004d40: 6172 672e 7374 6570 0a20 2020 2020 2020  arg.step.       
+00004d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d60: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00004d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d80: 2020 2075 7070 6572 3d61 7267 2e73 746f     upper=arg.sto
+00004d90: 700a 2020 2020 2020 2020 2020 2020 2020  p.              
+00004da0: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
+00004db0: 696e 2072 616e 6765 2873 656c 662e 6e6d  in range(self.nm
+00004dc0: 6f64 656c 7329 3a0a 2020 2020 2020 2020  odels):.        
+00004dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004de0: 2020 2020 6966 206e 6f74 206e 702e 6973      if not np.is
+00004df0: 6e61 6e28 6c6f 7765 7229 3a0a 2020 2020  nan(lower):.    
+00004e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e10: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00004e20: 656c 662e 6d6f 6465 6c73 5b69 5d2e 7674  elf.models[i].vt
+00004e30: 7572 623c 7570 7065 7220 616e 6420 7365  urb<upper and se
+00004e40: 6c66 2e6d 6f64 656c 735b 695d 2e76 7475  lf.models[i].vtu
+00004e50: 7262 3e6c 6f77 6572 3a0a 2020 2020 2020  rb>lower:.      
+00004e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e70: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00004e80: 745f 6461 7461 2e61 6464 5f6d 6f64 656c  t_data.add_model
+00004e90: 2873 656c 662e 6d6f 6465 6c73 5b69 5d29  (self.models[i])
+00004ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004eb0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00004ec0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00004ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ee0: 2020 2069 6620 7365 6c66 2e6d 6f64 656c     if self.model
+00004ef0: 735b 695d 2e76 7475 7262 3d3d 7570 7065  s[i].vturb==uppe
+00004f00: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
 00004f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f20: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-00004f30: 6365 2861 7267 2e73 7465 702c 666c 6f61  ce(arg.step,floa
-00004f40: 7429 206f 7220 6973 696e 7374 616e 6365  t) or isinstance
-00004f50: 2861 7267 2e73 7465 702c 696e 7429 3a0a  (arg.step,int):.
-00004f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f70: 2020 2020 2020 2020 2020 2020 6c6f 7765              lowe
-00004f80: 722c 7570 7065 723d 6172 672e 7374 6f70  r,upper=arg.stop
-00004f90: 2c61 7267 2e73 7465 700a 2020 2020 2020  ,arg.step.      
-00004fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fb0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00004f20: 2020 2020 2020 2072 6574 5f64 6174 612e         ret_data.
+00004f30: 6164 645f 6d6f 6465 6c28 7365 6c66 2e6d  add_model(self.m
+00004f40: 6f64 656c 735b 695d 290a 2020 2020 2020  odels[i]).      
+00004f50: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00004f60: 6966 2069 7369 6e73 7461 6e63 6528 6172  if isinstance(ar
+00004f70: 672e 7374 6f70 2c6c 6973 7429 3a0a 2020  g.stop,list):.  
+00004f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f90: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+00004fa0: 616e 6765 2873 656c 662e 6e6d 6f64 656c  ange(self.nmodel
+00004fb0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
 00004fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fd0: 2020 2020 7570 7065 723d 6172 672e 7374      upper=arg.st
-00004fe0: 6f70 0a20 2020 2020 2020 2020 2020 2020  op.             
-00004ff0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-00005000: 2069 6e20 7261 6e67 6528 7365 6c66 2e6e   in range(self.n
-00005010: 6d6f 6465 6c73 293a 0a20 2020 2020 2020  models):.       
-00005020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005030: 2020 2020 2069 6620 6e6f 7420 6e70 2e69       if not np.i
-00005040: 736e 616e 286c 6f77 6572 293a 0a20 2020  snan(lower):.   
-00005050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005060: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00005070: 7365 6c66 2e6d 6f64 656c 735b 695d 2e54  self.models[i].T
-00005080: 673c 7570 7065 7220 616e 6420 7365 6c66  g<upper and self
-00005090: 2e6d 6f64 656c 735b 695d 2e54 673e 6c6f  .models[i].Tg>lo
-000050a0: 7765 723a 0a20 2020 2020 2020 2020 2020  wer:.           
-000050b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000050c0: 2020 2020 2020 2020 2072 6574 5f64 6174           ret_dat
-000050d0: 612e 6164 645f 6d6f 6465 6c28 7365 6c66  a.add_model(self
-000050e0: 2e6d 6f64 656c 735b 695d 290a 2020 2020  .models[i]).    
+00004fd0: 6966 2073 656c 662e 6d6f 6465 6c73 5b69  if self.models[i
+00004fe0: 5d2e 7674 7572 6220 696e 2061 7267 2e73  ].vturb in arg.s
+00004ff0: 746f 703a 0a20 2020 2020 2020 2020 2020  top:.           
+00005000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005010: 2020 2020 2072 6574 5f64 6174 612e 6164       ret_data.ad
+00005020: 645f 6d6f 6465 6c28 7365 6c66 2e6d 6f64  d_model(self.mod
+00005030: 656c 735b 695d 290a 2020 2020 2020 2020  els[i]).        
+00005040: 2020 2020 2020 2020 656c 6966 2061 7267          elif arg
+00005050: 2e73 7461 7274 3d3d 2754 6727 3a0a 2020  .start=='Tg':.  
+00005060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005070: 2020 7570 7065 723d 6e70 2e6e 616e 0a20    upper=np.nan. 
+00005080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005090: 2020 206c 6f77 6572 3d6e 702e 6e61 6e0a     lower=np.nan.
+000050a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000050b0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+000050c0: 6528 6172 672e 7374 6f70 2c66 6c6f 6174  e(arg.stop,float
+000050d0: 2920 6f72 2069 7369 6e73 7461 6e63 6528  ) or isinstance(
+000050e0: 6172 672e 7374 6f70 2c69 6e74 293a 0a20  arg.stop,int):. 
 000050f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005100: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00005110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005120: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00005130: 2073 656c 662e 6d6f 6465 6c73 5b69 5d2e   self.models[i].
-00005140: 5467 3d3d 7570 7065 723a 0a20 2020 2020  Tg==upper:.     
-00005150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005160: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00005170: 6574 5f64 6174 612e 6164 645f 6d6f 6465  et_data.add_mode
-00005180: 6c28 7365 6c66 2e6d 6f64 656c 735b 695d  l(self.models[i]
-00005190: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000051a0: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
-000051b0: 7461 6e63 6528 6172 672e 7374 6f70 2c6c  tance(arg.stop,l
-000051c0: 6973 7429 3a0a 2020 2020 2020 2020 2020  ist):.          
-000051d0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-000051e0: 7220 6920 696e 2072 616e 6765 2873 656c  r i in range(sel
-000051f0: 662e 6e6d 6f64 656c 7329 3a0a 2020 2020  f.nmodels):.    
+00005100: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00005110: 616e 6365 2861 7267 2e73 7465 702c 666c  ance(arg.step,fl
+00005120: 6f61 7429 206f 7220 6973 696e 7374 616e  oat) or isinstan
+00005130: 6365 2861 7267 2e73 7465 702c 696e 7429  ce(arg.step,int)
+00005140: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00005150: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00005160: 7765 722c 7570 7065 723d 6172 672e 7374  wer,upper=arg.st
+00005170: 6f70 2c61 7267 2e73 7465 700a 2020 2020  op,arg.step.    
+00005180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005190: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+000051a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051b0: 2020 2020 2020 7570 7065 723d 6172 672e        upper=arg.
+000051c0: 7374 6f70 0a20 2020 2020 2020 2020 2020  stop.           
+000051d0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+000051e0: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
+000051f0: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
 00005200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005210: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00005220: 6d6f 6465 6c73 5b69 5d2e 5467 2069 6e20  models[i].Tg in 
-00005230: 6172 672e 7374 6f70 3a0a 2020 2020 2020  arg.stop:.      
-00005240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005250: 2020 2020 2020 2020 2020 7265 745f 6461            ret_da
-00005260: 7461 2e61 6464 5f6d 6f64 656c 2873 656c  ta.add_model(sel
-00005270: 662e 6d6f 6465 6c73 5b69 5d29 0a20 2020  f.models[i]).   
-00005280: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-00005290: 6620 6172 672e 7374 6172 743d 3d27 5464  f arg.start=='Td
-000052a0: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
-000052b0: 2020 2020 2020 2075 7070 6572 3d6e 702e         upper=np.
-000052c0: 6e61 6e0a 2020 2020 2020 2020 2020 2020  nan.            
-000052d0: 2020 2020 2020 2020 6c6f 7765 723d 6e70          lower=np
-000052e0: 2e6e 616e 0a20 2020 2020 2020 2020 2020  .nan.           
-000052f0: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
-00005300: 7374 616e 6365 2861 7267 2e73 746f 702c  stance(arg.stop,
-00005310: 666c 6f61 7429 206f 7220 6973 696e 7374  float) or isinst
-00005320: 616e 6365 2861 7267 2e73 746f 702c 696e  ance(arg.stop,in
-00005330: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-00005340: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00005350: 7369 6e73 7461 6e63 6528 6172 672e 7374  sinstance(arg.st
-00005360: 6570 2c66 6c6f 6174 2920 6f72 2069 7369  ep,float) or isi
-00005370: 6e73 7461 6e63 6528 6172 672e 7374 6570  nstance(arg.step
-00005380: 2c69 6e74 293a 0a20 2020 2020 2020 2020  ,int):.         
-00005390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053a0: 2020 206c 6f77 6572 2c75 7070 6572 3d61     lower,upper=a
-000053b0: 7267 2e73 746f 702c 6172 672e 7374 6570  rg.stop,arg.step
-000053c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000053d0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00005210: 2020 2020 2020 2069 6620 6e6f 7420 6e70         if not np
+00005220: 2e69 736e 616e 286c 6f77 6572 293a 0a20  .isnan(lower):. 
+00005230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005240: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00005250: 6620 7365 6c66 2e6d 6f64 656c 735b 695d  f self.models[i]
+00005260: 2e54 673c 7570 7065 7220 616e 6420 7365  .Tg<upper and se
+00005270: 6c66 2e6d 6f64 656c 735b 695d 2e54 673e  lf.models[i].Tg>
+00005280: 6c6f 7765 723a 0a20 2020 2020 2020 2020  lower:.         
+00005290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000052a0: 2020 2020 2020 2020 2020 2072 6574 5f64             ret_d
+000052b0: 6174 612e 6164 645f 6d6f 6465 6c28 7365  ata.add_model(se
+000052c0: 6c66 2e6d 6f64 656c 735b 695d 290a 2020  lf.models[i]).  
+000052d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000052e0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+000052f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005310: 6966 2073 656c 662e 6d6f 6465 6c73 5b69  if self.models[i
+00005320: 5d2e 5467 3d3d 7570 7065 723a 0a20 2020  ].Tg==upper:.   
+00005330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005350: 2072 6574 5f64 6174 612e 6164 645f 6d6f   ret_data.add_mo
+00005360: 6465 6c28 7365 6c66 2e6d 6f64 656c 735b  del(self.models[
+00005370: 695d 290a 2020 2020 2020 2020 2020 2020  i]).            
+00005380: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
+00005390: 6e73 7461 6e63 6528 6172 672e 7374 6f70  nstance(arg.stop
+000053a0: 2c6c 6973 7429 3a0a 2020 2020 2020 2020  ,list):.        
+000053b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000053c0: 666f 7220 6920 696e 2072 616e 6765 2873  for i in range(s
+000053d0: 656c 662e 6e6d 6f64 656c 7329 3a0a 2020  elf.nmodels):.  
 000053e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053f0: 2020 2020 2020 2020 2020 2075 7070 6572             upper
-00005400: 3d61 7267 2e73 746f 700a 2020 2020 2020  =arg.stop.      
-00005410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005420: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-00005430: 2873 656c 662e 6e6d 6f64 656c 7329 3a0a  (self.nmodels):.
-00005440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005450: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00005460: 6f74 206e 702e 6973 6e61 6e28 6c6f 7765  ot np.isnan(lowe
-00005470: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00005480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005490: 2020 2020 6966 2073 656c 662e 6d6f 6465      if self.mode
-000054a0: 6c73 5b69 5d2e 5464 3c75 7070 6572 2061  ls[i].Td<upper a
-000054b0: 6e64 2073 656c 662e 6d6f 6465 6c73 5b69  nd self.models[i
-000054c0: 5d2e 5464 3e6c 6f77 6572 3a0a 2020 2020  ].Td>lower:.    
-000054d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054f0: 7265 745f 6461 7461 2e61 6464 5f6d 6f64  ret_data.add_mod
-00005500: 656c 2873 656c 662e 6d6f 6465 6c73 5b69  el(self.models[i
-00005510: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-00005520: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00005530: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00005540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005550: 2020 2020 2069 6620 7365 6c66 2e6d 6f64       if self.mod
-00005560: 656c 735b 695d 2e54 643d 3d75 7070 6572  els[i].Td==upper
-00005570: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00005580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005590: 2020 2020 2020 7265 745f 6461 7461 2e61        ret_data.a
-000055a0: 6464 5f6d 6f64 656c 2873 656c 662e 6d6f  dd_model(self.mo
-000055b0: 6465 6c73 5b69 5d29 0a20 2020 2020 2020  dels[i]).       
-000055c0: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-000055d0: 6620 6973 696e 7374 616e 6365 2861 7267  f isinstance(arg
-000055e0: 2e73 746f 702c 6c69 7374 293a 0a20 2020  .stop,list):.   
+000053f0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00005400: 662e 6d6f 6465 6c73 5b69 5d2e 5467 2069  f.models[i].Tg i
+00005410: 6e20 6172 672e 7374 6f70 3a0a 2020 2020  n arg.stop:.    
+00005420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005430: 2020 2020 2020 2020 2020 2020 7265 745f              ret_
+00005440: 6461 7461 2e61 6464 5f6d 6f64 656c 2873  data.add_model(s
+00005450: 656c 662e 6d6f 6465 6c73 5b69 5d29 0a20  elf.models[i]). 
+00005460: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00005470: 6c69 6620 6172 672e 7374 6172 743d 3d27  lif arg.start=='
+00005480: 5464 273a 0a20 2020 2020 2020 2020 2020  Td':.           
+00005490: 2020 2020 2020 2020 2075 7070 6572 3d6e           upper=n
+000054a0: 702e 6e61 6e0a 2020 2020 2020 2020 2020  p.nan.          
+000054b0: 2020 2020 2020 2020 2020 6c6f 7765 723d            lower=
+000054c0: 6e70 2e6e 616e 0a20 2020 2020 2020 2020  np.nan.         
+000054d0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+000054e0: 696e 7374 616e 6365 2861 7267 2e73 746f  instance(arg.sto
+000054f0: 702c 666c 6f61 7429 206f 7220 6973 696e  p,float) or isin
+00005500: 7374 616e 6365 2861 7267 2e73 746f 702c  stance(arg.stop,
+00005510: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
+00005520: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00005530: 2069 7369 6e73 7461 6e63 6528 6172 672e   isinstance(arg.
+00005540: 7374 6570 2c66 6c6f 6174 2920 6f72 2069  step,float) or i
+00005550: 7369 6e73 7461 6e63 6528 6172 672e 7374  sinstance(arg.st
+00005560: 6570 2c69 6e74 293a 0a20 2020 2020 2020  ep,int):.       
+00005570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005580: 2020 2020 206c 6f77 6572 2c75 7070 6572       lower,upper
+00005590: 3d61 7267 2e73 746f 702c 6172 672e 7374  =arg.stop,arg.st
+000055a0: 6570 0a20 2020 2020 2020 2020 2020 2020  ep.             
+000055b0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000055c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000055d0: 2020 2020 2020 2020 2020 2020 2075 7070               upp
+000055e0: 6572 3d61 7267 2e73 746f 700a 2020 2020  er=arg.stop.    
 000055f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005600: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-00005610: 6e67 6528 7365 6c66 2e6e 6d6f 6465 6c73  nge(self.nmodels
-00005620: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00005630: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00005640: 6620 7365 6c66 2e6d 6f64 656c 735b 695d  f self.models[i]
-00005650: 2e54 6420 696e 2061 7267 2e73 746f 703a  .Td in arg.stop:
-00005660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005680: 2072 6574 5f64 6174 612e 6164 645f 6d6f   ret_data.add_mo
-00005690: 6465 6c28 7365 6c66 2e6d 6f64 656c 735b  del(self.models[
-000056a0: 695d 290a 2020 2020 2020 2020 2020 2020  i]).            
-000056b0: 2020 2020 656c 6966 2061 7267 2e73 7461      elif arg.sta
-000056c0: 7274 3d3d 2773 7065 6369 6573 5f69 6e64  rt=='species_ind
-000056d0: 6578 273a 0a20 2020 2020 2020 2020 2020  ex':.           
-000056e0: 2020 2020 2020 2020 2073 656c 5f73 7065           sel_spe
-000056f0: 6369 6573 5f6e 756d 6265 723d 5b5d 0a20  cies_number=[]. 
+00005600: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00005610: 6765 2873 656c 662e 6e6d 6f64 656c 7329  ge(self.nmodels)
+00005620: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00005630: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00005640: 206e 6f74 206e 702e 6973 6e61 6e28 6c6f   not np.isnan(lo
+00005650: 7765 7229 3a0a 2020 2020 2020 2020 2020  wer):.          
+00005660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005670: 2020 2020 2020 6966 2073 656c 662e 6d6f        if self.mo
+00005680: 6465 6c73 5b69 5d2e 5464 3c75 7070 6572  dels[i].Td<upper
+00005690: 2061 6e64 2073 656c 662e 6d6f 6465 6c73   and self.models
+000056a0: 5b69 5d2e 5464 3e6c 6f77 6572 3a0a 2020  [i].Td>lower:.  
+000056b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056d0: 2020 7265 745f 6461 7461 2e61 6464 5f6d    ret_data.add_m
+000056e0: 6f64 656c 2873 656c 662e 6d6f 6465 6c73  odel(self.models
+000056f0: 5b69 5d29 0a20 2020 2020 2020 2020 2020  [i]).           
 00005700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005710: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00005720: 2861 7267 2e73 746f 702c 696e 7429 3a0a  (arg.stop,int):.
-00005730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005740: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-00005750: 7461 6e63 6528 6172 672e 7374 6570 2c69  tance(arg.step,i
-00005760: 6e74 293a 0a20 2020 2020 2020 2020 2020  nt):.           
-00005770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005780: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-00005790: 6172 672e 7374 6f70 2c61 7267 2e73 7465  arg.stop,arg.ste
-000057a0: 7029 3a0a 2020 2020 2020 2020 2020 2020  p):.            
-000057b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057c0: 2020 2020 7365 6c5f 7370 6563 6965 735f      sel_species_
-000057d0: 6e75 6d62 6572 2e61 7070 656e 6428 6929  number.append(i)
-000057e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000057f0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00005800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005810: 2020 2020 2020 2020 2020 2073 656c 5f73             sel_s
-00005820: 7065 6369 6573 5f6e 756d 6265 722e 6170  pecies_number.ap
-00005830: 7065 6e64 2861 7267 2e73 746f 7029 0a20  pend(arg.stop). 
-00005840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005850: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
-00005860: 6365 2861 7267 2e73 746f 702c 6c69 7374  ce(arg.stop,list
-00005870: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00005880: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00005890: 656c 5f73 7065 6369 6573 5f6e 756d 6265  el_species_numbe
-000058a0: 723d 6172 672e 7374 6f70 0a20 2020 2020  r=arg.stop.     
-000058b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000058c0: 6620 6c65 6e28 7365 6c5f 7370 6563 6965  f len(sel_specie
-000058d0: 735f 6e75 6d62 6572 293e 303a 0a20 2020  s_number)>0:.   
-000058e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058f0: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-00005900: 6e67 6528 7365 6c66 2e6e 6d6f 6465 6c73  nge(self.nmodels
-00005910: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00005920: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00005930: 6620 7365 6c66 2e6d 6f64 656c 735b 695d  f self.models[i]
-00005940: 2e73 7065 6369 6573 5f69 6e64 6578 2069  .species_index i
-00005950: 6e20 7365 6c5f 7370 6563 6965 735f 6e75  n sel_species_nu
-00005960: 6d62 6572 3a0a 2020 2020 2020 2020 2020  mber:.          
-00005970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005980: 2020 2020 2020 7265 745f 6461 7461 2e61        ret_data.a
-00005990: 6464 5f6d 6f64 656c 2873 656c 662e 6d6f  dd_model(self.mo
-000059a0: 6465 6c73 5b69 5d29 0a20 2020 2020 2020  dels[i]).       
-000059b0: 2020 2020 2020 2020 2065 6c69 6620 6172           elif ar
-000059c0: 672e 7374 6172 743d 3d27 6162 756e 6461  g.start=='abunda
-000059d0: 6e63 6527 3a0a 2020 2020 2020 2020 2020  nce':.          
-000059e0: 2020 2020 2020 2020 2020 7570 7065 723d            upper=
-000059f0: 6e70 2e6e 616e 0a20 2020 2020 2020 2020  np.nan.         
-00005a00: 2020 2020 2020 2020 2020 206c 6f77 6572             lower
-00005a10: 3d6e 702e 6e61 6e0a 2020 2020 2020 2020  =np.nan.        
-00005a20: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00005a30: 7369 6e73 7461 6e63 6528 6172 672e 7374  sinstance(arg.st
-00005a40: 6f70 2c66 6c6f 6174 2920 6f72 2069 7369  op,float) or isi
-00005a50: 6e73 7461 6e63 6528 6172 672e 7374 6f70  nstance(arg.stop
-00005a60: 2c69 6e74 293a 0a20 2020 2020 2020 2020  ,int):.         
-00005a70: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00005a80: 6620 6973 696e 7374 616e 6365 2861 7267  f isinstance(arg
-00005a90: 2e73 7465 702c 666c 6f61 7429 206f 7220  .step,float) or 
-00005aa0: 6973 696e 7374 616e 6365 2861 7267 2e73  isinstance(arg.s
-00005ab0: 7465 702c 696e 7429 3a0a 2020 2020 2020  tep,int):.      
+00005710: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00005720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005730: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
+00005740: 6f64 656c 735b 695d 2e54 643d 3d75 7070  odels[i].Td==upp
+00005750: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
+00005760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005770: 2020 2020 2020 2020 7265 745f 6461 7461          ret_data
+00005780: 2e61 6464 5f6d 6f64 656c 2873 656c 662e  .add_model(self.
+00005790: 6d6f 6465 6c73 5b69 5d29 0a20 2020 2020  models[i]).     
+000057a0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000057b0: 6c69 6620 6973 696e 7374 616e 6365 2861  lif isinstance(a
+000057c0: 7267 2e73 746f 702c 6c69 7374 293a 0a20  rg.stop,list):. 
+000057d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057e0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+000057f0: 7261 6e67 6528 7365 6c66 2e6e 6d6f 6465  range(self.nmode
+00005800: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
+00005810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005820: 2069 6620 7365 6c66 2e6d 6f64 656c 735b   if self.models[
+00005830: 695d 2e54 6420 696e 2061 7267 2e73 746f  i].Td in arg.sto
+00005840: 703a 0a20 2020 2020 2020 2020 2020 2020  p:.             
+00005850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005860: 2020 2072 6574 5f64 6174 612e 6164 645f     ret_data.add_
+00005870: 6d6f 6465 6c28 7365 6c66 2e6d 6f64 656c  model(self.model
+00005880: 735b 695d 290a 2020 2020 2020 2020 2020  s[i]).          
+00005890: 2020 2020 2020 656c 6966 2061 7267 2e73        elif arg.s
+000058a0: 7461 7274 3d3d 2773 7065 6369 6573 5f69  tart=='species_i
+000058b0: 6e64 6578 273a 0a20 2020 2020 2020 2020  ndex':.         
+000058c0: 2020 2020 2020 2020 2020 2073 656c 5f73             sel_s
+000058d0: 7065 6369 6573 5f6e 756d 6265 723d 5b5d  pecies_number=[]
+000058e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000058f0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+00005900: 6365 2861 7267 2e73 746f 702c 696e 7429  ce(arg.stop,int)
+00005910: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00005920: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+00005930: 6e73 7461 6e63 6528 6172 672e 7374 6570  nstance(arg.step
+00005940: 2c69 6e74 293a 0a20 2020 2020 2020 2020  ,int):.         
+00005950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005960: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+00005970: 6528 6172 672e 7374 6f70 2c61 7267 2e73  e(arg.stop,arg.s
+00005980: 7465 7029 3a0a 2020 2020 2020 2020 2020  tep):.          
+00005990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000059a0: 2020 2020 2020 7365 6c5f 7370 6563 6965        sel_specie
+000059b0: 735f 6e75 6d62 6572 2e61 7070 656e 6428  s_number.append(
+000059c0: 6929 0a20 2020 2020 2020 2020 2020 2020  i).             
+000059d0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000059e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000059f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00005a00: 5f73 7065 6369 6573 5f6e 756d 6265 722e  _species_number.
+00005a10: 6170 7065 6e64 2861 7267 2e73 746f 7029  append(arg.stop)
+00005a20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005a30: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
+00005a40: 616e 6365 2861 7267 2e73 746f 702c 6c69  ance(arg.stop,li
+00005a50: 7374 293a 0a20 2020 2020 2020 2020 2020  st):.           
+00005a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a70: 2073 656c 5f73 7065 6369 6573 5f6e 756d   sel_species_num
+00005a80: 6265 723d 6172 672e 7374 6f70 0a20 2020  ber=arg.stop.   
+00005a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005aa0: 2069 6620 6c65 6e28 7365 6c5f 7370 6563   if len(sel_spec
+00005ab0: 6965 735f 6e75 6d62 6572 293e 303a 0a20  ies_number)>0:. 
 00005ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ad0: 2020 2020 2020 6c6f 7765 722c 7570 7065        lower,uppe
-00005ae0: 723d 6172 672e 7374 6f70 2c61 7267 2e73  r=arg.stop,arg.s
-00005af0: 7465 700a 2020 2020 2020 2020 2020 2020  tep.            
-00005b00: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00005b10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00005b20: 2020 2020 2020 2020 2020 2020 2020 7570                up
-00005b30: 7065 723d 6172 672e 7374 6f70 0a20 2020  per=arg.stop.   
-00005b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b50: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-00005b60: 6e67 6528 7365 6c66 2e6e 6d6f 6465 6c73  nge(self.nmodels
-00005b70: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00005b80: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00005b90: 6620 6e6f 7420 6e70 2e69 736e 616e 286c  f not np.isnan(l
-00005ba0: 6f77 6572 293a 0a20 2020 2020 2020 2020  ower):.         
-00005bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005bc0: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
-00005bd0: 6f64 656c 735b 695d 2e61 6275 6e64 616e  odels[i].abundan
-00005be0: 6365 3c75 7070 6572 2061 6e64 2073 656c  ce<upper and sel
-00005bf0: 662e 6d6f 6465 6c73 5b69 5d2e 6162 756e  f.models[i].abun
-00005c00: 6461 6e63 653e 6c6f 7765 723a 0a20 2020  dance>lower:.   
-00005c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c30: 2072 6574 5f64 6174 612e 6164 645f 6d6f   ret_data.add_mo
-00005c40: 6465 6c28 7365 6c66 2e6d 6f64 656c 735b  del(self.models[
-00005c50: 695d 290a 2020 2020 2020 2020 2020 2020  i]).            
-00005c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c70: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00005c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c90: 2020 2020 2020 6966 2073 656c 662e 6d6f        if self.mo
-00005ca0: 6465 6c73 5b69 5d2e 6162 756e 6461 6e63  dels[i].abundanc
-00005cb0: 653d 3d75 7070 6572 3a0a 2020 2020 2020  e==upper:.      
-00005cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cd0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00005ce0: 745f 6461 7461 2e61 6464 5f6d 6f64 656c  t_data.add_model
-00005cf0: 2873 656c 662e 6d6f 6465 6c73 5b69 5d29  (self.models[i])
-00005d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005d10: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
-00005d20: 616e 6365 2861 7267 2e73 746f 702c 6c69  ance(arg.stop,li
-00005d30: 7374 293a 0a20 2020 2020 2020 2020 2020  st):.           
-00005d40: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00005d50: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
-00005d60: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
-00005d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d80: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
-00005d90: 6f64 656c 735b 695d 2e61 6275 6e64 616e  odels[i].abundan
-00005da0: 6365 2069 6e20 6172 672e 7374 6f70 3a0a  ce in arg.stop:.
-00005db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005dd0: 7265 745f 6461 7461 2e61 6464 5f6d 6f64  ret_data.add_mod
-00005de0: 656c 2873 656c 662e 6d6f 6465 6c73 5b69  el(self.models[i
-00005df0: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-00005e00: 2020 2065 6c69 6620 6172 672e 7374 6172     elif arg.star
-00005e10: 743d 3d27 6476 273a 0a20 2020 2020 2020  t=='dv':.       
-00005e20: 2020 2020 2020 2020 2020 2020 2075 7070               upp
-00005e30: 6572 3d6e 702e 6e61 6e0a 2020 2020 2020  er=np.nan.      
-00005e40: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00005e50: 7765 723d 6e70 2e6e 616e 0a20 2020 2020  wer=np.nan.     
-00005e60: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00005e70: 6620 6973 696e 7374 616e 6365 2861 7267  f isinstance(arg
-00005e80: 2e73 746f 702c 666c 6f61 7429 206f 7220  .stop,float) or 
-00005e90: 6973 696e 7374 616e 6365 2861 7267 2e73  isinstance(arg.s
-00005ea0: 746f 702c 696e 7429 3a0a 2020 2020 2020  top,int):.      
+00005ad0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+00005ae0: 7261 6e67 6528 7365 6c66 2e6e 6d6f 6465  range(self.nmode
+00005af0: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
+00005b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b10: 2069 6620 7365 6c66 2e6d 6f64 656c 735b   if self.models[
+00005b20: 695d 2e73 7065 6369 6573 5f69 6e64 6578  i].species_index
+00005b30: 2069 6e20 7365 6c5f 7370 6563 6965 735f   in sel_species_
+00005b40: 6e75 6d62 6572 3a0a 2020 2020 2020 2020  number:.        
+00005b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b60: 2020 2020 2020 2020 7265 745f 6461 7461          ret_data
+00005b70: 2e61 6464 5f6d 6f64 656c 2873 656c 662e  .add_model(self.
+00005b80: 6d6f 6465 6c73 5b69 5d29 0a20 2020 2020  models[i]).     
+00005b90: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00005ba0: 6172 672e 7374 6172 743d 3d27 6162 756e  arg.start=='abun
+00005bb0: 6461 6e63 6527 3a0a 2020 2020 2020 2020  dance':.        
+00005bc0: 2020 2020 2020 2020 2020 2020 7570 7065              uppe
+00005bd0: 723d 6e70 2e6e 616e 0a20 2020 2020 2020  r=np.nan.       
+00005be0: 2020 2020 2020 2020 2020 2020 206c 6f77               low
+00005bf0: 6572 3d6e 702e 6e61 6e0a 2020 2020 2020  er=np.nan.      
+00005c00: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00005c10: 2069 7369 6e73 7461 6e63 6528 6172 672e   isinstance(arg.
+00005c20: 7374 6f70 2c66 6c6f 6174 2920 6f72 2069  stop,float) or i
+00005c30: 7369 6e73 7461 6e63 6528 6172 672e 7374  sinstance(arg.st
+00005c40: 6f70 2c69 6e74 293a 0a20 2020 2020 2020  op,int):.       
+00005c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c60: 2069 6620 6973 696e 7374 616e 6365 2861   if isinstance(a
+00005c70: 7267 2e73 7465 702c 666c 6f61 7429 206f  rg.step,float) o
+00005c80: 7220 6973 696e 7374 616e 6365 2861 7267  r isinstance(arg
+00005c90: 2e73 7465 702c 696e 7429 3a0a 2020 2020  .step,int):.    
+00005ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005cb0: 2020 2020 2020 2020 6c6f 7765 722c 7570          lower,up
+00005cc0: 7065 723d 6172 672e 7374 6f70 2c61 7267  per=arg.stop,arg
+00005cd0: 2e73 7465 700a 2020 2020 2020 2020 2020  .step.          
+00005ce0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00005cf0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00005d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d10: 7570 7065 723d 6172 672e 7374 6f70 0a20  upper=arg.stop. 
+00005d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d30: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+00005d40: 7261 6e67 6528 7365 6c66 2e6e 6d6f 6465  range(self.nmode
+00005d50: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
+00005d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d70: 2069 6620 6e6f 7420 6e70 2e69 736e 616e   if not np.isnan
+00005d80: 286c 6f77 6572 293a 0a20 2020 2020 2020  (lower):.       
+00005d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005da0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00005db0: 2e6d 6f64 656c 735b 695d 2e61 6275 6e64  .models[i].abund
+00005dc0: 616e 6365 3c75 7070 6572 2061 6e64 2073  ance<upper and s
+00005dd0: 656c 662e 6d6f 6465 6c73 5b69 5d2e 6162  elf.models[i].ab
+00005de0: 756e 6461 6e63 653e 6c6f 7765 723a 0a20  undance>lower:. 
+00005df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e10: 2020 2072 6574 5f64 6174 612e 6164 645f     ret_data.add_
+00005e20: 6d6f 6465 6c28 7365 6c66 2e6d 6f64 656c  model(self.model
+00005e30: 735b 695d 290a 2020 2020 2020 2020 2020  s[i]).          
+00005e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e50: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00005e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e70: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00005e80: 6d6f 6465 6c73 5b69 5d2e 6162 756e 6461  models[i].abunda
+00005e90: 6e63 653d 3d75 7070 6572 3a0a 2020 2020  nce==upper:.    
+00005ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ec0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00005ed0: 6172 672e 7374 6570 2c66 6c6f 6174 2920  arg.step,float) 
-00005ee0: 6f72 2069 7369 6e73 7461 6e63 6528 6172  or isinstance(ar
-00005ef0: 672e 7374 6570 2c69 6e74 293a 0a20 2020  g.step,int):.   
-00005f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f10: 2020 2020 2020 2020 206c 6f77 6572 2c75           lower,u
-00005f20: 7070 6572 3d61 7267 2e73 746f 702c 6172  pper=arg.stop,ar
-00005f30: 672e 7374 6570 0a20 2020 2020 2020 2020  g.step.         
-00005f40: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00005f50: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00005f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f70: 2075 7070 6572 3d61 7267 2e73 746f 700a   upper=arg.stop.
-00005f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f90: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00005fa0: 2072 616e 6765 2873 656c 662e 6e6d 6f64   range(self.nmod
-00005fb0: 656c 7329 3a0a 2020 2020 2020 2020 2020  els):.          
-00005fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fd0: 2020 6966 206e 6f74 206e 702e 6973 6e61    if not np.isna
-00005fe0: 6e28 6c6f 7765 7229 3a0a 2020 2020 2020  n(lower):.      
-00005ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006000: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00006010: 662e 6d6f 6465 6c73 5b69 5d2e 6476 3c75  f.models[i].dv<u
-00006020: 7070 6572 2061 6e64 2073 656c 662e 6d6f  pper and self.mo
-00006030: 6465 6c73 5b69 5d2e 6476 3e6c 6f77 6572  dels[i].dv>lower
-00006040: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00006050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006060: 2020 2020 2020 7265 745f 6461 7461 2e61        ret_data.a
-00006070: 6464 5f6d 6f64 656c 2873 656c 662e 6d6f  dd_model(self.mo
-00006080: 6465 6c73 5b69 5d29 0a20 2020 2020 2020  dels[i]).       
+00005ec0: 7265 745f 6461 7461 2e61 6464 5f6d 6f64  ret_data.add_mod
+00005ed0: 656c 2873 656c 662e 6d6f 6465 6c73 5b69  el(self.models[i
+00005ee0: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+00005ef0: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
+00005f00: 7374 616e 6365 2861 7267 2e73 746f 702c  stance(arg.stop,
+00005f10: 6c69 7374 293a 0a20 2020 2020 2020 2020  list):.         
+00005f20: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00005f30: 6f72 2069 2069 6e20 7261 6e67 6528 7365  or i in range(se
+00005f40: 6c66 2e6e 6d6f 6465 6c73 293a 0a20 2020  lf.nmodels):.   
+00005f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f60: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00005f70: 2e6d 6f64 656c 735b 695d 2e61 6275 6e64  .models[i].abund
+00005f80: 616e 6365 2069 6e20 6172 672e 7374 6f70  ance in arg.stop
+00005f90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00005fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fb0: 2020 7265 745f 6461 7461 2e61 6464 5f6d    ret_data.add_m
+00005fc0: 6f64 656c 2873 656c 662e 6d6f 6465 6c73  odel(self.models
+00005fd0: 5b69 5d29 0a20 2020 2020 2020 2020 2020  [i]).           
+00005fe0: 2020 2020 2065 6c69 6620 6172 672e 7374       elif arg.st
+00005ff0: 6172 743d 3d27 6476 273a 0a20 2020 2020  art=='dv':.     
+00006000: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+00006010: 7070 6572 3d6e 702e 6e61 6e0a 2020 2020  pper=np.nan.    
+00006020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006030: 6c6f 7765 723d 6e70 2e6e 616e 0a20 2020  lower=np.nan.   
+00006040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006050: 2069 6620 6973 696e 7374 616e 6365 2861   if isinstance(a
+00006060: 7267 2e73 746f 702c 666c 6f61 7429 206f  rg.stop,float) o
+00006070: 7220 6973 696e 7374 616e 6365 2861 7267  r isinstance(arg
+00006080: 2e73 746f 702c 696e 7429 3a0a 2020 2020  .stop,int):.    
 00006090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060a0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000060b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060c0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-000060d0: 6c66 2e6d 6f64 656c 735b 695d 2e64 763d  lf.models[i].dv=
-000060e0: 3d75 7070 6572 3a0a 2020 2020 2020 2020  =upper:.        
-000060f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006100: 2020 2020 2020 2020 2020 2020 7265 745f              ret_
-00006110: 6461 7461 2e61 6464 5f6d 6f64 656c 2873  data.add_model(s
-00006120: 656c 662e 6d6f 6465 6c73 5b69 5d29 0a20  elf.models[i]). 
-00006130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006140: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
-00006150: 6365 2861 7267 2e73 746f 702c 6c69 7374  ce(arg.stop,list
-00006160: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00006170: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-00006180: 2069 6e20 7261 6e67 6528 7365 6c66 2e6e   in range(self.n
-00006190: 6d6f 6465 6c73 293a 0a20 2020 2020 2020  models):.       
+000060a0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+000060b0: 6528 6172 672e 7374 6570 2c66 6c6f 6174  e(arg.step,float
+000060c0: 2920 6f72 2069 7369 6e73 7461 6e63 6528  ) or isinstance(
+000060d0: 6172 672e 7374 6570 2c69 6e74 293a 0a20  arg.step,int):. 
+000060e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060f0: 2020 2020 2020 2020 2020 206c 6f77 6572             lower
+00006100: 2c75 7070 6572 3d61 7267 2e73 746f 702c  ,upper=arg.stop,
+00006110: 6172 672e 7374 6570 0a20 2020 2020 2020  arg.step.       
+00006120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006130: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00006140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006150: 2020 2075 7070 6572 3d61 7267 2e73 746f     upper=arg.sto
+00006160: 700a 2020 2020 2020 2020 2020 2020 2020  p.              
+00006170: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
+00006180: 696e 2072 616e 6765 2873 656c 662e 6e6d  in range(self.nm
+00006190: 6f64 656c 7329 3a0a 2020 2020 2020 2020  odels):.        
 000061a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061b0: 2020 2020 2069 6620 7365 6c66 2e6d 6f64       if self.mod
-000061c0: 656c 735b 695d 2e64 7620 696e 2061 7267  els[i].dv in arg
-000061d0: 2e73 746f 703a 0a20 2020 2020 2020 2020  .stop:.         
-000061e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061f0: 2020 2020 2020 2072 6574 5f64 6174 612e         ret_data.
-00006200: 6164 645f 6d6f 6465 6c28 7365 6c66 2e6d  add_model(self.m
-00006210: 6f64 656c 735b 695d 290a 2020 2020 2020  odels[i]).      
-00006220: 2020 2020 2020 2020 2020 656c 6966 2061            elif a
-00006230: 7267 2e73 7461 7274 3d3d 276e 6c65 7665  rg.start=='nleve
-00006240: 6c73 273a 0a20 2020 2020 2020 2020 2020  ls':.           
-00006250: 2020 2020 2020 2020 2073 656c 5f73 7065           sel_spe
-00006260: 6369 6573 5f6e 756d 6265 723d 5b5d 0a20  cies_number=[]. 
+000061b0: 2020 2020 6966 206e 6f74 206e 702e 6973      if not np.is
+000061c0: 6e61 6e28 6c6f 7765 7229 3a0a 2020 2020  nan(lower):.    
+000061d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061e0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+000061f0: 656c 662e 6d6f 6465 6c73 5b69 5d2e 6476  elf.models[i].dv
+00006200: 3c75 7070 6572 2061 6e64 2073 656c 662e  <upper and self.
+00006210: 6d6f 6465 6c73 5b69 5d2e 6476 3e6c 6f77  models[i].dv>low
+00006220: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
+00006230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006240: 2020 2020 2020 2020 7265 745f 6461 7461          ret_data
+00006250: 2e61 6464 5f6d 6f64 656c 2873 656c 662e  .add_model(self.
+00006260: 6d6f 6465 6c73 5b69 5d29 0a20 2020 2020  models[i]).     
 00006270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006280: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00006290: 2861 7267 2e73 746f 702c 696e 7429 3a0a  (arg.stop,int):.
-000062a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062b0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-000062c0: 7461 6e63 6528 6172 672e 7374 6570 2c69  tance(arg.step,i
-000062d0: 6e74 293a 0a20 2020 2020 2020 2020 2020  nt):.           
-000062e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062f0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-00006300: 6172 672e 7374 6f70 2c61 7267 2e73 7465  arg.stop,arg.ste
-00006310: 7029 3a0a 2020 2020 2020 2020 2020 2020  p):.            
-00006320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006330: 2020 2020 7365 6c5f 7370 6563 6965 735f      sel_species_
-00006340: 6e75 6d62 6572 2e61 7070 656e 6428 6929  number.append(i)
-00006350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006360: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00006370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006380: 2020 2020 2020 2020 2020 2073 656c 5f73             sel_s
-00006390: 7065 6369 6573 5f6e 756d 6265 722e 6170  pecies_number.ap
-000063a0: 7065 6e64 2861 7267 2e73 746f 7029 0a20  pend(arg.stop). 
-000063b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063c0: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
-000063d0: 6365 2861 7267 2e73 746f 702c 6c69 7374  ce(arg.stop,list
-000063e0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000063f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00006400: 656c 5f73 7065 6369 6573 5f6e 756d 6265  el_species_numbe
-00006410: 723d 6172 672e 7374 6f70 0a20 2020 2020  r=arg.stop.     
-00006420: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00006430: 6620 6c65 6e28 7365 6c5f 7370 6563 6965  f len(sel_specie
-00006440: 735f 6e75 6d62 6572 293e 303a 0a20 2020  s_number)>0:.   
-00006450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006460: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-00006470: 6e67 6528 7365 6c66 2e6e 6d6f 6465 6c73  nge(self.nmodels
-00006480: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00006490: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000064a0: 6620 7365 6c66 2e6d 6f64 656c 735b 695d  f self.models[i]
-000064b0: 2e6e 6c65 7665 6c73 2069 6e20 7365 6c5f  .nlevels in sel_
-000064c0: 7370 6563 6965 735f 6e75 6d62 6572 3a0a  species_number:.
-000064d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064f0: 7265 745f 6461 7461 2e61 6464 5f6d 6f64  ret_data.add_mod
-00006500: 656c 2873 656c 662e 6d6f 6465 6c73 5b69  el(self.models[i
-00006510: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-00006520: 2020 2065 6c69 6620 6172 672e 7374 6172     elif arg.star
-00006530: 743d 3d27 6e6c 696e 6573 273a 0a20 2020  t=='nlines':.   
-00006540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006550: 2073 656c 5f73 7065 6369 6573 5f6e 756d   sel_species_num
-00006560: 6265 723d 5b5d 0a20 2020 2020 2020 2020  ber=[].         
-00006570: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-00006580: 696e 7374 616e 6365 2861 7267 2e73 746f  instance(arg.sto
-00006590: 702c 696e 7429 3a0a 2020 2020 2020 2020  p,int):.        
-000065a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065b0: 6966 2069 7369 6e73 7461 6e63 6528 6172  if isinstance(ar
-000065c0: 672e 7374 6570 2c69 6e74 293a 0a20 2020  g.step,int):.   
+00006280: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00006290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000062b0: 7365 6c66 2e6d 6f64 656c 735b 695d 2e64  self.models[i].d
+000062c0: 763d 3d75 7070 6572 3a0a 2020 2020 2020  v==upper:.      
+000062d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062e0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000062f0: 745f 6461 7461 2e61 6464 5f6d 6f64 656c  t_data.add_model
+00006300: 2873 656c 662e 6d6f 6465 6c73 5b69 5d29  (self.models[i])
+00006310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006320: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
+00006330: 616e 6365 2861 7267 2e73 746f 702c 6c69  ance(arg.stop,li
+00006340: 7374 293a 0a20 2020 2020 2020 2020 2020  st):.           
+00006350: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00006360: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
+00006370: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
+00006380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006390: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
+000063a0: 6f64 656c 735b 695d 2e64 7620 696e 2061  odels[i].dv in a
+000063b0: 7267 2e73 746f 703a 0a20 2020 2020 2020  rg.stop:.       
+000063c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063d0: 2020 2020 2020 2020 2072 6574 5f64 6174           ret_dat
+000063e0: 612e 6164 645f 6d6f 6465 6c28 7365 6c66  a.add_model(self
+000063f0: 2e6d 6f64 656c 735b 695d 290a 2020 2020  .models[i]).    
+00006400: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00006410: 2061 7267 2e73 7461 7274 3d3d 276e 6c65   arg.start=='nle
+00006420: 7665 6c73 273a 0a20 2020 2020 2020 2020  vels':.         
+00006430: 2020 2020 2020 2020 2020 2073 656c 5f73             sel_s
+00006440: 7065 6369 6573 5f6e 756d 6265 723d 5b5d  pecies_number=[]
+00006450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006460: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+00006470: 6365 2861 7267 2e73 746f 702c 696e 7429  ce(arg.stop,int)
+00006480: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00006490: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+000064a0: 6e73 7461 6e63 6528 6172 672e 7374 6570  nstance(arg.step
+000064b0: 2c69 6e74 293a 0a20 2020 2020 2020 2020  ,int):.         
+000064c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000064d0: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+000064e0: 6528 6172 672e 7374 6f70 2c61 7267 2e73  e(arg.stop,arg.s
+000064f0: 7465 7029 3a0a 2020 2020 2020 2020 2020  tep):.          
+00006500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006510: 2020 2020 2020 7365 6c5f 7370 6563 6965        sel_specie
+00006520: 735f 6e75 6d62 6572 2e61 7070 656e 6428  s_number.append(
+00006530: 6929 0a20 2020 2020 2020 2020 2020 2020  i).             
+00006540: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00006550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006560: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00006570: 5f73 7065 6369 6573 5f6e 756d 6265 722e  _species_number.
+00006580: 6170 7065 6e64 2861 7267 2e73 746f 7029  append(arg.stop)
+00006590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000065a0: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
+000065b0: 616e 6365 2861 7267 2e73 746f 702c 6c69  ance(arg.stop,li
+000065c0: 7374 293a 0a20 2020 2020 2020 2020 2020  st):.           
 000065d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065e0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-000065f0: 6e20 7261 6e67 6528 6172 672e 7374 6f70  n range(arg.stop
-00006600: 2c61 7267 2e73 7465 7029 3a0a 2020 2020  ,arg.step):.    
-00006610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006620: 2020 2020 2020 2020 2020 2020 7365 6c5f              sel_
-00006630: 7370 6563 6965 735f 6e75 6d62 6572 2e61  species_number.a
-00006640: 7070 656e 6428 6929 0a20 2020 2020 2020  ppend(i).       
-00006650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006660: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000065e0: 2073 656c 5f73 7065 6369 6573 5f6e 756d   sel_species_num
+000065f0: 6265 723d 6172 672e 7374 6f70 0a20 2020  ber=arg.stop.   
+00006600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006610: 2069 6620 6c65 6e28 7365 6c5f 7370 6563   if len(sel_spec
+00006620: 6965 735f 6e75 6d62 6572 293e 303a 0a20  ies_number)>0:. 
+00006630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006640: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+00006650: 7261 6e67 6528 7365 6c66 2e6e 6d6f 6465  range(self.nmode
+00006660: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
 00006670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006680: 2020 2073 656c 5f73 7065 6369 6573 5f6e     sel_species_n
-00006690: 756d 6265 722e 6170 7065 6e64 2861 7267  umber.append(arg
-000066a0: 2e73 746f 7029 0a20 2020 2020 2020 2020  .stop).         
-000066b0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-000066c0: 6973 696e 7374 616e 6365 2861 7267 2e73  isinstance(arg.s
-000066d0: 746f 702c 6c69 7374 293a 0a20 2020 2020  top,list):.     
-000066e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066f0: 2020 2020 2020 2073 656c 5f73 7065 6369         sel_speci
-00006700: 6573 5f6e 756d 6265 723d 6172 672e 7374  es_number=arg.st
-00006710: 6f70 0a20 2020 2020 2020 2020 2020 2020  op.             
-00006720: 2020 2020 2020 2069 6620 6c65 6e28 7365         if len(se
-00006730: 6c5f 7370 6563 6965 735f 6e75 6d62 6572  l_species_number
-00006740: 293e 303a 0a20 2020 2020 2020 2020 2020  )>0:.           
-00006750: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00006760: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
-00006770: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
+00006680: 2069 6620 7365 6c66 2e6d 6f64 656c 735b   if self.models[
+00006690: 695d 2e6e 6c65 7665 6c73 2069 6e20 7365  i].nlevels in se
+000066a0: 6c5f 7370 6563 6965 735f 6e75 6d62 6572  l_species_number
+000066b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000066c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000066d0: 2020 7265 745f 6461 7461 2e61 6464 5f6d    ret_data.add_m
+000066e0: 6f64 656c 2873 656c 662e 6d6f 6465 6c73  odel(self.models
+000066f0: 5b69 5d29 0a20 2020 2020 2020 2020 2020  [i]).           
+00006700: 2020 2020 2065 6c69 6620 6172 672e 7374       elif arg.st
+00006710: 6172 743d 3d27 6e6c 696e 6573 273a 0a20  art=='nlines':. 
+00006720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006730: 2020 2073 656c 5f73 7065 6369 6573 5f6e     sel_species_n
+00006740: 756d 6265 723d 5b5d 0a20 2020 2020 2020  umber=[].       
+00006750: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00006760: 6973 696e 7374 616e 6365 2861 7267 2e73  isinstance(arg.s
+00006770: 746f 702c 696e 7429 3a0a 2020 2020 2020  top,int):.      
 00006780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006790: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
-000067a0: 6f64 656c 735b 695d 2e6e 6c69 6e65 7320  odels[i].nlines 
-000067b0: 696e 2073 656c 5f73 7065 6369 6573 5f6e  in sel_species_n
-000067c0: 756d 6265 723a 0a20 2020 2020 2020 2020  umber:.         
-000067d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067e0: 2020 2020 2020 2072 6574 5f64 6174 612e         ret_data.
-000067f0: 6164 645f 6d6f 6465 6c28 7365 6c66 2e6d  add_model(self.m
-00006800: 6f64 656c 735b 695d 290a 2020 2020 2020  odels[i]).      
-00006810: 2020 2020 2020 2020 2020 656c 6966 2061            elif a
-00006820: 7267 2e73 7461 7274 3d3d 2763 6f6e 7654  rg.start=='convT
-00006830: 7970 6527 3a0a 2020 2020 2020 2020 2020  ype':.          
-00006840: 2020 2020 2020 2020 2020 7365 6c5f 7370            sel_sp
-00006850: 6563 6965 735f 6e75 6d62 6572 3d5b 5d0a  ecies_number=[].
-00006860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006870: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00006880: 6528 6172 672e 7374 6f70 2c69 6e74 293a  e(arg.stop,int):
-00006890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000068a0: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
-000068b0: 7374 616e 6365 2861 7267 2e73 7465 702c  stance(arg.step,
-000068c0: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
-000068d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068e0: 2020 7365 6c5f 7370 6563 6965 735f 6e75    sel_species_nu
-000068f0: 6d62 6572 3d5b 6172 672e 7374 6f70 2c61  mber=[arg.stop,a
-00006900: 7267 2e73 7465 705d 0a20 2020 2020 2020  rg.step].       
-00006910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006920: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00006930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006940: 2020 2073 656c 5f73 7065 6369 6573 5f6e     sel_species_n
-00006950: 756d 6265 722e 6170 7065 6e64 2861 7267  umber.append(arg
-00006960: 2e73 746f 7029 0a20 2020 2020 2020 2020  .stop).         
-00006970: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00006980: 6973 696e 7374 616e 6365 2861 7267 2e73  isinstance(arg.s
-00006990: 746f 702c 6c69 7374 293a 0a20 2020 2020  top,list):.     
-000069a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069b0: 2020 2020 2020 2073 656c 5f73 7065 6369         sel_speci
-000069c0: 6573 5f6e 756d 6265 723d 6172 672e 7374  es_number=arg.st
-000069d0: 6f70 0a20 2020 2020 2020 2020 2020 2020  op.             
-000069e0: 2020 2020 2020 2069 6620 6c65 6e28 7365         if len(se
-000069f0: 6c5f 7370 6563 6965 735f 6e75 6d62 6572  l_species_number
-00006a00: 293e 303a 0a20 2020 2020 2020 2020 2020  )>0:.           
-00006a10: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00006a20: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
-00006a30: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
-00006a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a50: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
-00006a60: 6f64 656c 735b 695d 2e63 6f6e 7654 7970  odels[i].convTyp
-00006a70: 6520 696e 2073 656c 5f73 7065 6369 6573  e in sel_species
-00006a80: 5f6e 756d 6265 723a 0a20 2020 2020 2020  _number:.       
-00006a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006aa0: 2020 2020 2020 2020 2072 6574 5f64 6174           ret_dat
-00006ab0: 612e 6164 645f 6d6f 6465 6c28 7365 6c66  a.add_model(self
-00006ac0: 2e6d 6f64 656c 735b 695d 290a 2020 2020  .models[i]).    
-00006ad0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00006ae0: 2061 7267 2e73 7461 7274 3d3d 2763 6f6e   arg.start=='con
-00006af0: 7652 273a 0a20 2020 2020 2020 2020 2020  vR':.           
-00006b00: 2020 2020 2020 2020 2075 7070 6572 3d6e           upper=n
-00006b10: 702e 6e61 6e0a 2020 2020 2020 2020 2020  p.nan.          
-00006b20: 2020 2020 2020 2020 2020 6c6f 7765 723d            lower=
-00006b30: 6e70 2e6e 616e 0a20 2020 2020 2020 2020  np.nan.         
-00006b40: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-00006b50: 696e 7374 616e 6365 2861 7267 2e73 746f  instance(arg.sto
-00006b60: 702c 666c 6f61 7429 206f 7220 6973 696e  p,float) or isin
-00006b70: 7374 616e 6365 2861 7267 2e73 746f 702c  stance(arg.stop,
-00006b80: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
-00006b90: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00006ba0: 2069 7369 6e73 7461 6e63 6528 6172 672e   isinstance(arg.
-00006bb0: 7374 6570 2c66 6c6f 6174 2920 6f72 2069  step,float) or i
-00006bc0: 7369 6e73 7461 6e63 6528 6172 672e 7374  sinstance(arg.st
-00006bd0: 6570 2c69 6e74 293a 0a20 2020 2020 2020  ep,int):.       
-00006be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006bf0: 2020 2020 206c 6f77 6572 2c75 7070 6572       lower,upper
-00006c00: 3d61 7267 2e73 746f 702c 6172 672e 7374  =arg.stop,arg.st
-00006c10: 6570 0a20 2020 2020 2020 2020 2020 2020  ep.             
-00006c20: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00006c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006c40: 2020 2020 2020 2020 2020 2020 2075 7070               upp
-00006c50: 6572 3d61 7267 2e73 746f 700a 2020 2020  er=arg.stop.    
-00006c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c70: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00006c80: 6765 2873 656c 662e 6e6d 6f64 656c 7329  ge(self.nmodels)
-00006c90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00006ca0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00006cb0: 206e 6f74 206e 702e 6973 6e61 6e28 6c6f   not np.isnan(lo
-00006cc0: 7765 7229 3a0a 2020 2020 2020 2020 2020  wer):.          
-00006cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ce0: 2020 2020 2020 6966 2073 656c 662e 6d6f        if self.mo
-00006cf0: 6465 6c73 5b69 5d2e 636f 6e76 523c 7570  dels[i].convR<up
-00006d00: 7065 7220 616e 6420 7365 6c66 2e6d 6f64  per and self.mod
-00006d10: 656c 735b 695d 2e63 6f6e 7652 3e6c 6f77  els[i].convR>low
-00006d20: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
-00006d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d40: 2020 2020 2020 2020 7265 745f 6461 7461          ret_data
-00006d50: 2e61 6464 5f6d 6f64 656c 2873 656c 662e  .add_model(self.
-00006d60: 6d6f 6465 6c73 5b69 5d29 0a20 2020 2020  models[i]).     
+00006790: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+000067a0: 6172 672e 7374 6570 2c69 6e74 293a 0a20  arg.step,int):. 
+000067b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067c0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+000067d0: 2069 6e20 7261 6e67 6528 6172 672e 7374   in range(arg.st
+000067e0: 6f70 2c61 7267 2e73 7465 7029 3a0a 2020  op,arg.step):.  
+000067f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006800: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00006810: 6c5f 7370 6563 6965 735f 6e75 6d62 6572  l_species_number
+00006820: 2e61 7070 656e 6428 6929 0a20 2020 2020  .append(i).     
+00006830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006840: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00006850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006860: 2020 2020 2073 656c 5f73 7065 6369 6573       sel_species
+00006870: 5f6e 756d 6265 722e 6170 7065 6e64 2861  _number.append(a
+00006880: 7267 2e73 746f 7029 0a20 2020 2020 2020  rg.stop).       
+00006890: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+000068a0: 6620 6973 696e 7374 616e 6365 2861 7267  f isinstance(arg
+000068b0: 2e73 746f 702c 6c69 7374 293a 0a20 2020  .stop,list):.   
+000068c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068d0: 2020 2020 2020 2020 2073 656c 5f73 7065           sel_spe
+000068e0: 6369 6573 5f6e 756d 6265 723d 6172 672e  cies_number=arg.
+000068f0: 7374 6f70 0a20 2020 2020 2020 2020 2020  stop.           
+00006900: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
+00006910: 7365 6c5f 7370 6563 6965 735f 6e75 6d62  sel_species_numb
+00006920: 6572 293e 303a 0a20 2020 2020 2020 2020  er)>0:.         
+00006930: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00006940: 6f72 2069 2069 6e20 7261 6e67 6528 7365  or i in range(se
+00006950: 6c66 2e6e 6d6f 6465 6c73 293a 0a20 2020  lf.nmodels):.   
+00006960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006970: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00006980: 2e6d 6f64 656c 735b 695d 2e6e 6c69 6e65  .models[i].nline
+00006990: 7320 696e 2073 656c 5f73 7065 6369 6573  s in sel_species
+000069a0: 5f6e 756d 6265 723a 0a20 2020 2020 2020  _number:.       
+000069b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000069c0: 2020 2020 2020 2020 2072 6574 5f64 6174           ret_dat
+000069d0: 612e 6164 645f 6d6f 6465 6c28 7365 6c66  a.add_model(self
+000069e0: 2e6d 6f64 656c 735b 695d 290a 2020 2020  .models[i]).    
+000069f0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00006a00: 2061 7267 2e73 7461 7274 3d3d 2763 6f6e   arg.start=='con
+00006a10: 7654 7970 6527 3a0a 2020 2020 2020 2020  vType':.        
+00006a20: 2020 2020 2020 2020 2020 2020 7365 6c5f              sel_
+00006a30: 7370 6563 6965 735f 6e75 6d62 6572 3d5b  species_number=[
+00006a40: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00006a50: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+00006a60: 6e63 6528 6172 672e 7374 6f70 2c69 6e74  nce(arg.stop,int
+00006a70: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00006a80: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+00006a90: 696e 7374 616e 6365 2861 7267 2e73 7465  instance(arg.ste
+00006aa0: 702c 696e 7429 3a0a 2020 2020 2020 2020  p,int):.        
+00006ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ac0: 2020 2020 7365 6c5f 7370 6563 6965 735f      sel_species_
+00006ad0: 6e75 6d62 6572 3d5b 6172 672e 7374 6f70  number=[arg.stop
+00006ae0: 2c61 7267 2e73 7465 705d 0a20 2020 2020  ,arg.step].     
+00006af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b00: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00006b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b20: 2020 2020 2073 656c 5f73 7065 6369 6573       sel_species
+00006b30: 5f6e 756d 6265 722e 6170 7065 6e64 2861  _number.append(a
+00006b40: 7267 2e73 746f 7029 0a20 2020 2020 2020  rg.stop).       
+00006b50: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+00006b60: 6620 6973 696e 7374 616e 6365 2861 7267  f isinstance(arg
+00006b70: 2e73 746f 702c 6c69 7374 293a 0a20 2020  .stop,list):.   
+00006b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b90: 2020 2020 2020 2020 2073 656c 5f73 7065           sel_spe
+00006ba0: 6369 6573 5f6e 756d 6265 723d 6172 672e  cies_number=arg.
+00006bb0: 7374 6f70 0a20 2020 2020 2020 2020 2020  stop.           
+00006bc0: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
+00006bd0: 7365 6c5f 7370 6563 6965 735f 6e75 6d62  sel_species_numb
+00006be0: 6572 293e 303a 0a20 2020 2020 2020 2020  er)>0:.         
+00006bf0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00006c00: 6f72 2069 2069 6e20 7261 6e67 6528 7365  or i in range(se
+00006c10: 6c66 2e6e 6d6f 6465 6c73 293a 0a20 2020  lf.nmodels):.   
+00006c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c30: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00006c40: 2e6d 6f64 656c 735b 695d 2e63 6f6e 7654  .models[i].convT
+00006c50: 7970 6520 696e 2073 656c 5f73 7065 6369  ype in sel_speci
+00006c60: 6573 5f6e 756d 6265 723a 0a20 2020 2020  es_number:.     
+00006c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c80: 2020 2020 2020 2020 2020 2072 6574 5f64             ret_d
+00006c90: 6174 612e 6164 645f 6d6f 6465 6c28 7365  ata.add_model(se
+00006ca0: 6c66 2e6d 6f64 656c 735b 695d 290a 2020  lf.models[i]).  
+00006cb0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00006cc0: 6966 2061 7267 2e73 7461 7274 3d3d 2763  if arg.start=='c
+00006cd0: 6f6e 7652 273a 0a20 2020 2020 2020 2020  onvR':.         
+00006ce0: 2020 2020 2020 2020 2020 2075 7070 6572             upper
+00006cf0: 3d6e 702e 6e61 6e0a 2020 2020 2020 2020  =np.nan.        
+00006d00: 2020 2020 2020 2020 2020 2020 6c6f 7765              lowe
+00006d10: 723d 6e70 2e6e 616e 0a20 2020 2020 2020  r=np.nan.       
+00006d20: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00006d30: 6973 696e 7374 616e 6365 2861 7267 2e73  isinstance(arg.s
+00006d40: 746f 702c 666c 6f61 7429 206f 7220 6973  top,float) or is
+00006d50: 696e 7374 616e 6365 2861 7267 2e73 746f  instance(arg.sto
+00006d60: 702c 696e 7429 3a0a 2020 2020 2020 2020  p,int):.        
 00006d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d80: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00006d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006da0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00006db0: 7365 6c66 2e6d 6f64 656c 735b 695d 2e63  self.models[i].c
-00006dc0: 6f6e 7652 3d3d 7570 7065 723a 0a20 2020  onvR==upper:.   
-00006dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006df0: 2072 6574 5f64 6174 612e 6164 645f 6d6f   ret_data.add_mo
-00006e00: 6465 6c28 7365 6c66 2e6d 6f64 656c 735b  del(self.models[
-00006e10: 695d 290a 2020 2020 2020 2020 2020 2020  i]).            
-00006e20: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
-00006e30: 6e73 7461 6e63 6528 6172 672e 7374 6f70  nstance(arg.stop
-00006e40: 2c6c 6973 7429 3a0a 2020 2020 2020 2020  ,list):.        
-00006e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e60: 666f 7220 6920 696e 2072 616e 6765 2873  for i in range(s
-00006e70: 656c 662e 6e6d 6f64 656c 7329 3a0a 2020  elf.nmodels):.  
+00006d80: 6966 2069 7369 6e73 7461 6e63 6528 6172  if isinstance(ar
+00006d90: 672e 7374 6570 2c66 6c6f 6174 2920 6f72  g.step,float) or
+00006da0: 2069 7369 6e73 7461 6e63 6528 6172 672e   isinstance(arg.
+00006db0: 7374 6570 2c69 6e74 293a 0a20 2020 2020  step,int):.     
+00006dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006dd0: 2020 2020 2020 206c 6f77 6572 2c75 7070         lower,upp
+00006de0: 6572 3d61 7267 2e73 746f 702c 6172 672e  er=arg.stop,arg.
+00006df0: 7374 6570 0a20 2020 2020 2020 2020 2020  step.           
+00006e00: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00006e10: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00006e20: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+00006e30: 7070 6572 3d61 7267 2e73 746f 700a 2020  pper=arg.stop.  
+00006e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e50: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+00006e60: 616e 6765 2873 656c 662e 6e6d 6f64 656c  ange(self.nmodel
+00006e70: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
 00006e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e90: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00006ea0: 662e 6d6f 6465 6c73 5b69 5d2e 636f 6e76  f.models[i].conv
-00006eb0: 5220 696e 2061 7267 2e73 746f 703a 0a20  R in arg.stop:. 
-00006ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ed0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00006ee0: 6574 5f64 6174 612e 6164 645f 6d6f 6465  et_data.add_mode
-00006ef0: 6c28 7365 6c66 2e6d 6f64 656c 735b 695d  l(self.models[i]
-00006f00: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00006f10: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00006f20: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00006f30: 6520 4b65 7945 7272 6f72 2827 556e 7265  e KeyError('Unre
-00006f40: 636f 676e 6973 6564 2070 6172 616d 6574  cognised paramet
-00006f50: 6572 2066 6f72 2073 6c69 6369 6e67 2729  er for slicing')
-00006f60: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00006f70: 7265 745f 6461 7461 0a0a 2020 2020 6465  ret_data..    de
-00006f80: 6620 636f 6e76 6f6c 7665 2873 656c 662c  f convolve(self,
-00006f90: 6672 6571 5f62 696e 733d 4e6f 6e65 2c52  freq_bins=None,R
-00006fa0: 3d31 2c6c 616d 6264 615f 303d 312c 6c61  =1,lambda_0=1,la
-00006fb0: 6d62 6461 5f6e 3d31 2c76 723d 3133 3030  mbda_n=1,vr=1300
-00006fc0: 2c4e 4c54 453d 4661 6c73 652c 636f 6e76  ,NLTE=False,conv
-00006fd0: 5f74 7970 653d 312c 7665 7262 6f73 653d  _type=1,verbose=
-00006fe0: 5472 7565 2c6f 7665 726c 6170 3d46 616c  True,overlap=Fal
-00006ff0: 7365 293a 0a20 2020 2020 2020 2066 6f72  se):.        for
-00007000: 2069 2c64 2069 6e20 656e 756d 6572 6174   i,d in enumerat
-00007010: 6528 7365 6c66 2e6d 6f64 656c 7329 3a0a  e(self.models):.
-00007020: 2020 2020 2020 2020 2020 2020 6966 2076              if v
-00007030: 6572 626f 7365 3a20 7072 696e 7428 275c  erbose: print('\
-00007040: 6e27 2c69 2b31 2c27 3b20 4d6f 6465 6c20  n',i+1,'; Model 
-00007050: 6e75 6d62 6572 2027 2c73 656c 662e 6d6f  number ',self.mo
-00007060: 6465 6c73 5b69 5d2e 6d6f 6465 6c5f 6e75  dels[i].model_nu
-00007070: 6d62 6572 2c27 3b20 5370 6563 6965 7320  mber,'; Species 
-00007080: 6e75 6d62 6572 2027 2c73 656c 662e 6d6f  number ',self.mo
-00007090: 6465 6c73 5b69 5d2e 7370 6563 6965 735f  dels[i].species_
-000070a0: 6e75 6d62 6572 290a 2020 2020 2020 2020  number).        
-000070b0: 2020 2020 642e 636f 6e76 6f6c 7665 2866      d.convolve(f
-000070c0: 7265 715f 6269 6e73 3d66 7265 715f 6269  req_bins=freq_bi
-000070d0: 6e73 2c52 3d52 2c6c 616d 6264 615f 303d  ns,R=R,lambda_0=
-000070e0: 6c61 6d62 6461 5f30 2c6c 616d 6264 615f  lambda_0,lambda_
-000070f0: 6e3d 6c61 6d62 6461 5f6e 2c76 723d 7672  n=lambda_n,vr=vr
-00007100: 2c4e 4c54 453d 4e4c 5445 2c63 6f6e 765f  ,NLTE=NLTE,conv_
-00007110: 7479 7065 3d63 6f6e 765f 7479 7065 2c6f  type=conv_type,o
-00007120: 7665 726c 6170 3d6f 7665 726c 6170 290a  verlap=overlap).
-00007130: 0a20 2020 2064 6566 2063 6f6e 766f 6c76  .    def convolv
-00007140: 655f 6f76 6572 6c61 7028 7365 6c66 2c52  e_overlap(self,R
-00007150: 3d31 2c6c 616d 6264 615f 303d 312c 6c61  =1,lambda_0=1,la
-00007160: 6d62 6461 5f6e 3d31 2c76 6572 626f 7365  mbda_n=1,verbose
-00007170: 3d54 7275 6529 3a0a 2020 2020 2020 2020  =True):.        
-00007180: 666f 7220 692c 6420 696e 2065 6e75 6d65  for i,d in enume
-00007190: 7261 7465 2873 656c 662e 6d6f 6465 6c73  rate(self.models
-000071a0: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
-000071b0: 6620 7665 7262 6f73 653a 2070 7269 6e74  f verbose: print
-000071c0: 2827 5c6e 272c 692b 312c 273b 204d 6f64  ('\n',i+1,'; Mod
-000071d0: 656c 206e 756d 6265 7220 272c 7365 6c66  el number ',self
-000071e0: 2e6d 6f64 656c 735b 695d 2e6d 6f64 656c  .models[i].model
-000071f0: 5f6e 756d 6265 7229 0a20 2020 2020 2020  _number).       
-00007200: 2020 2020 2064 2e63 6f6e 766f 6c76 655f       d.convolve_
-00007210: 6f76 6572 6c61 7028 523d 522c 6c61 6d62  overlap(R=R,lamb
-00007220: 6461 5f30 3d6c 616d 6264 615f 302c 6c61  da_0=lambda_0,la
-00007230: 6d62 6461 5f6e 3d6c 616d 6264 615f 6e29  mbda_n=lambda_n)
-00007240: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-00007250: 2020 2020 6465 6620 6e6d 6f64 656c 7328      def nmodels(
-00007260: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
-00007270: 656c 662e 5f6e 6d6f 6465 6c73 3d6c 656e  elf._nmodels=len
-00007280: 2873 656c 662e 6d6f 6465 6c73 290a 2020  (self.models).  
-00007290: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000072a0: 662e 5f6e 6d6f 6465 6c73 0a0a 2020 2020  f._nmodels..    
-000072b0: 406e 6d6f 6465 6c73 2e73 6574 7465 720a  @nmodels.setter.
-000072c0: 2020 2020 6465 6620 6e6d 6f64 656c 7328      def nmodels(
-000072d0: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
-000072e0: 2020 2020 2073 656c 662e 5f6e 6d6f 6465       self._nmode
-000072f0: 6c73 3d76 616c 7565 0a0a 2020 2020 4070  ls=value..    @p
-00007300: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00007310: 7370 6563 6965 735f 6e75 6d62 6572 2873  species_number(s
-00007320: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
-00007330: 2073 656c 662e 6e6d 6f64 656c 733e 313a   self.nmodels>1:
-00007340: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00007350: 662e 5f73 7065 6369 6573 5f6e 756d 6265  f._species_numbe
-00007360: 723d 5b5d 0a20 2020 2020 2020 2020 2020  r=[].           
-00007370: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-00007380: 7365 6c66 2e6e 6d6f 6465 6c73 293a 0a20  self.nmodels):. 
-00007390: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000073a0: 656c 662e 5f73 7065 6369 6573 5f6e 756d  elf._species_num
-000073b0: 6265 722e 6170 7065 6e64 2873 656c 662e  ber.append(self.
-000073c0: 6d6f 6465 6c73 5b69 5d2e 7370 6563 6965  models[i].specie
-000073d0: 735f 6e75 6d62 6572 290a 2020 2020 2020  s_number).      
-000073e0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000073f0: 2020 2020 7365 6c66 2e5f 7370 6563 6965      self._specie
-00007400: 735f 6e75 6d62 6572 3d73 656c 662e 6d6f  s_number=self.mo
-00007410: 6465 6c73 5b30 5d2e 7370 6563 6965 735f  dels[0].species_
-00007420: 6e75 6d62 6572 0a20 2020 2020 2020 2072  number.        r
-00007430: 6574 7572 6e20 7365 6c66 2e5f 7370 6563  eturn self._spec
-00007440: 6965 735f 6e75 6d62 6572 0a0a 2020 2020  ies_number..    
-00007450: 4073 7065 6369 6573 5f6e 756d 6265 722e  @species_number.
-00007460: 7365 7474 6572 0a20 2020 2064 6566 2073  setter.    def s
-00007470: 7065 6369 6573 5f6e 756d 6265 7228 7365  pecies_number(se
-00007480: 6c66 2c76 616c 7565 293a 0a20 2020 2020  lf,value):.     
-00007490: 2020 2073 656c 662e 5f73 7065 6369 6573     self._species
-000074a0: 5f6e 756d 6265 723d 7661 6c75 650a 0a20  _number=value.. 
-000074b0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-000074c0: 2064 6566 206d 6f64 656c 5f6e 756d 6265   def model_numbe
-000074d0: 7228 7365 6c66 293a 0a20 2020 2020 2020  r(self):.       
-000074e0: 2069 6620 7365 6c66 2e6e 6d6f 6465 6c73   if self.nmodels
-000074f0: 3e31 3a0a 2020 2020 2020 2020 2020 2020  >1:.            
-00007500: 7365 6c66 2e5f 6d6f 6465 6c5f 6e75 6d62  self._model_numb
-00007510: 6572 3d5b 5d0a 2020 2020 2020 2020 2020  er=[].          
-00007520: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-00007530: 2873 656c 662e 6e6d 6f64 656c 7329 3a0a  (self.nmodels):.
-00007540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007550: 7365 6c66 2e5f 6d6f 6465 6c5f 6e75 6d62  self._model_numb
-00007560: 6572 2e61 7070 656e 6428 7365 6c66 2e6d  er.append(self.m
-00007570: 6f64 656c 735b 695d 2e6d 6f64 656c 5f6e  odels[i].model_n
-00007580: 756d 6265 7229 0a20 2020 2020 2020 2065  umber).        e
-00007590: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-000075a0: 2073 656c 662e 5f6d 6f64 656c 5f6e 756d   self._model_num
-000075b0: 6265 723d 7365 6c66 2e6d 6f64 656c 735b  ber=self.models[
-000075c0: 305d 2e6d 6f64 656c 5f6e 756d 6265 720a  0].model_number.
-000075d0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000075e0: 656c 662e 5f6d 6f64 656c 5f6e 756d 6265  elf._model_numbe
-000075f0: 720a 0a20 2020 2040 6d6f 6465 6c5f 6e75  r..    @model_nu
-00007600: 6d62 6572 2e73 6574 7465 720a 2020 2020  mber.setter.    
-00007610: 6465 6620 6d6f 6465 6c5f 6e75 6d62 6572  def model_number
-00007620: 2873 656c 662c 7661 6c75 6529 3a0a 2020  (self,value):.  
-00007630: 2020 2020 2020 7365 6c66 2e5f 6d6f 6465        self._mode
-00007640: 6c5f 6e75 6d62 6572 3d76 616c 7565 0a0a  l_number=value..
-00007650: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-00007660: 2020 6465 6620 4e48 2873 656c 6629 3a0a    def NH(self):.
-00007670: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00007680: 6e6d 6f64 656c 733e 313a 0a20 2020 2020  nmodels>1:.     
-00007690: 2020 2020 2020 2073 656c 662e 5f4e 483d         self._NH=
-000076a0: 5b5d 0a20 2020 2020 2020 2020 2020 2066  [].            f
-000076b0: 6f72 2069 2069 6e20 7261 6e67 6528 7365  or i in range(se
-000076c0: 6c66 2e6e 6d6f 6465 6c73 293a 0a20 2020  lf.nmodels):.   
-000076d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000076e0: 662e 5f4e 482e 6170 7065 6e64 2873 656c  f._NH.append(sel
-000076f0: 662e 6d6f 6465 6c73 5b69 5d2e 4e48 290a  f.models[i].NH).
-00007700: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00007710: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00007720: 4e48 3d73 656c 662e 6d6f 6465 6c73 5b30  NH=self.models[0
-00007730: 5d2e 4e48 0a20 2020 2020 2020 2072 6574  ].NH.        ret
-00007740: 7572 6e20 7365 6c66 2e5f 4e48 0a0a 2020  urn self._NH..  
-00007750: 2020 404e 482e 7365 7474 6572 0a20 2020    @NH.setter.   
-00007760: 2064 6566 204e 4828 7365 6c66 2c76 616c   def NH(self,val
-00007770: 7565 293a 0a20 2020 2020 2020 2073 656c  ue):.        sel
-00007780: 662e 5f4e 483d 7661 6c75 650a 0a20 2020  f._NH=value..   
-00007790: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-000077a0: 6566 206e 436f 6c6c 2873 656c 6629 3a0a  ef nColl(self):.
-000077b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000077c0: 6e6d 6f64 656c 733e 313a 0a20 2020 2020  nmodels>1:.     
-000077d0: 2020 2020 2020 2073 656c 662e 5f6e 436f         self._nCo
-000077e0: 6c6c 3d5b 5d0a 2020 2020 2020 2020 2020  ll=[].          
-000077f0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-00007800: 2873 656c 662e 6e6d 6f64 656c 7329 3a0a  (self.nmodels):.
-00007810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007820: 7365 6c66 2e5f 6e43 6f6c 6c2e 6170 7065  self._nColl.appe
-00007830: 6e64 2873 656c 662e 6d6f 6465 6c73 5b69  nd(self.models[i
-00007840: 5d2e 6e43 6f6c 6c29 0a20 2020 2020 2020  ].nColl).       
-00007850: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00007860: 2020 2073 656c 662e 5f6e 436f 6c6c 3d73     self._nColl=s
-00007870: 656c 662e 6d6f 6465 6c73 5b30 5d2e 6e43  elf.models[0].nC
-00007880: 6f6c 6c0a 2020 2020 2020 2020 7265 7475  oll.        retu
-00007890: 726e 2073 656c 662e 5f6e 436f 6c6c 0a0a  rn self._nColl..
-000078a0: 2020 2020 406e 436f 6c6c 2e73 6574 7465      @nColl.sette
-000078b0: 720a 2020 2020 6465 6620 6e43 6f6c 6c28  r.    def nColl(
-000078c0: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
-000078d0: 2020 2020 2073 656c 662e 5f6e 436f 6c6c       self._nColl
-000078e0: 3d76 616c 7565 0a0a 2020 2020 4070 726f  =value..    @pro
-000078f0: 7065 7274 790a 2020 2020 6465 6620 6e65  perty.    def ne
-00007900: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00007910: 6966 2073 656c 662e 6e6d 6f64 656c 733e  if self.nmodels>
-00007920: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
-00007930: 656c 662e 5f6e 653d 5b5d 0a20 2020 2020  elf._ne=[].     
-00007940: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-00007950: 7261 6e67 6528 7365 6c66 2e6e 6d6f 6465  range(self.nmode
-00007960: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
-00007970: 2020 2020 2073 656c 662e 5f6e 652e 6170       self._ne.ap
-00007980: 7065 6e64 2873 656c 662e 6d6f 6465 6c73  pend(self.models
-00007990: 5b69 5d2e 6e65 290a 2020 2020 2020 2020  [i].ne).        
-000079a0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000079b0: 2020 7365 6c66 2e5f 6e65 3d73 656c 662e    self._ne=self.
-000079c0: 6d6f 6465 6c73 5b30 5d2e 6e65 0a20 2020  models[0].ne.   
-000079d0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-000079e0: 2e5f 6e65 0a0a 2020 2020 406e 652e 7365  ._ne..    @ne.se
-000079f0: 7474 6572 0a20 2020 2064 6566 206e 6528  tter.    def ne(
-00007a00: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
-00007a10: 2020 2020 2073 656c 662e 5f6e 653d 7661       self._ne=va
-00007a20: 6c75 650a 0a20 2020 2040 7072 6f70 6572  lue..    @proper
-00007a30: 7479 0a20 2020 2064 6566 206e 4865 2873  ty.    def nHe(s
-00007a40: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
-00007a50: 2073 656c 662e 6e6d 6f64 656c 733e 313a   self.nmodels>1:
-00007a60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00007a70: 662e 5f6e 4865 3d5b 5d0a 2020 2020 2020  f._nHe=[].      
-00007a80: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-00007a90: 616e 6765 2873 656c 662e 6e6d 6f64 656c  ange(self.nmodel
-00007aa0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-00007ab0: 2020 2020 7365 6c66 2e5f 6e48 652e 6170      self._nHe.ap
-00007ac0: 7065 6e64 2873 656c 662e 6d6f 6465 6c73  pend(self.models
-00007ad0: 5b69 5d2e 6e48 6529 0a20 2020 2020 2020  [i].nHe).       
-00007ae0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00007af0: 2020 2073 656c 662e 5f6e 4865 3d73 656c     self._nHe=sel
-00007b00: 662e 6d6f 6465 6c73 5b30 5d2e 6e48 650a  f.models[0].nHe.
-00007b10: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00007b20: 656c 662e 5f6e 4865 0a0a 2020 2020 406e  elf._nHe..    @n
-00007b30: 4865 2e73 6574 7465 720a 2020 2020 6465  He.setter.    de
-00007b40: 6620 6e48 6528 7365 6c66 2c76 616c 7565  f nHe(self,value
-00007b50: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-00007b60: 5f6e 4865 3d76 616c 7565 0a0a 2020 2020  _nHe=value..    
-00007b70: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-00007b80: 6620 6e48 4949 2873 656c 6629 3a0a 2020  f nHII(self):.  
-00007b90: 2020 2020 2020 6966 2073 656c 662e 6e6d        if self.nm
-00007ba0: 6f64 656c 733e 313a 0a20 2020 2020 2020  odels>1:.       
-00007bb0: 2020 2020 2073 656c 662e 5f6e 4849 493d       self._nHII=
-00007bc0: 5b5d 0a20 2020 2020 2020 2020 2020 2066  [].            f
-00007bd0: 6f72 2069 2069 6e20 7261 6e67 6528 7365  or i in range(se
-00007be0: 6c66 2e6e 6d6f 6465 6c73 293a 0a20 2020  lf.nmodels):.   
-00007bf0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00007c00: 662e 5f6e 4849 492e 6170 7065 6e64 2873  f._nHII.append(s
-00007c10: 656c 662e 6d6f 6465 6c73 5b69 5d2e 6e48  elf.models[i].nH
-00007c20: 4949 290a 2020 2020 2020 2020 656c 7365  II).        else
-00007c30: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00007c40: 6c66 2e5f 6e48 4949 3d73 656c 662e 6d6f  lf._nHII=self.mo
-00007c50: 6465 6c73 5b30 5d2e 6e48 4949 0a20 2020  dels[0].nHII.   
-00007c60: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00007c70: 2e5f 6e48 4949 0a0a 2020 2020 406e 4849  ._nHII..    @nHI
-00007c80: 492e 7365 7474 6572 0a20 2020 2064 6566  I.setter.    def
-00007c90: 206e 4849 4928 7365 6c66 2c76 616c 7565   nHII(self,value
-00007ca0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-00007cb0: 5f6e 4849 493d 7661 6c75 650a 0a20 2020  _nHII=value..   
-00007cc0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-00007cd0: 6566 206e 4849 2873 656c 6629 3a0a 2020  ef nHI(self):.  
-00007ce0: 2020 2020 2020 6966 2073 656c 662e 6e6d        if self.nm
-00007cf0: 6f64 656c 733e 313a 0a20 2020 2020 2020  odels>1:.       
-00007d00: 2020 2020 2073 656c 662e 5f6e 4849 3d5b       self._nHI=[
-00007d10: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
-00007d20: 7220 6920 696e 2072 616e 6765 2873 656c  r i in range(sel
-00007d30: 662e 6e6d 6f64 656c 7329 3a0a 2020 2020  f.nmodels):.    
-00007d40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00007d50: 2e5f 6e48 492e 6170 7065 6e64 2873 656c  ._nHI.append(sel
-00007d60: 662e 6d6f 6465 6c73 5b69 5d2e 6e48 4929  f.models[i].nHI)
-00007d70: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00007d80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007d90: 5f6e 4849 3d73 656c 662e 6d6f 6465 6c73  _nHI=self.models
-00007da0: 5b30 5d2e 6e48 490a 2020 2020 2020 2020  [0].nHI.        
-00007db0: 7265 7475 726e 2073 656c 662e 5f6e 4849  return self._nHI
-00007dc0: 0a0a 2020 2020 406e 4849 2e73 6574 7465  ..    @nHI.sette
-00007dd0: 720a 2020 2020 6465 6620 6e48 4928 7365  r.    def nHI(se
-00007de0: 6c66 2c76 616c 7565 293a 0a20 2020 2020  lf,value):.     
-00007df0: 2020 2073 656c 662e 5f6e 4849 3d76 616c     self._nHI=val
-00007e00: 7565 0a0a 2020 2020 4070 726f 7065 7274  ue..    @propert
-00007e10: 790a 2020 2020 6465 6620 6e48 3228 7365  y.    def nH2(se
-00007e20: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
-00007e30: 7365 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a  self.nmodels>1:.
-00007e40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00007e50: 2e5f 6e48 323d 5b5d 0a20 2020 2020 2020  ._nH2=[].       
-00007e60: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-00007e70: 6e67 6528 7365 6c66 2e6e 6d6f 6465 6c73  nge(self.nmodels
-00007e80: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00007e90: 2020 2073 656c 662e 5f6e 4832 2e61 7070     self._nH2.app
-00007ea0: 656e 6428 7365 6c66 2e6d 6f64 656c 735b  end(self.models[
-00007eb0: 695d 2e6e 4832 290a 2020 2020 2020 2020  i].nH2).        
-00007ec0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00007ed0: 2020 7365 6c66 2e5f 6e48 323d 7365 6c66    self._nH2=self
-00007ee0: 2e6d 6f64 656c 735b 305d 2e6e 4832 0a20  .models[0].nH2. 
-00007ef0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00007f00: 6c66 2e5f 6e48 320a 0a20 2020 2040 6e48  lf._nH2..    @nH
-00007f10: 322e 7365 7474 6572 0a20 2020 2064 6566  2.setter.    def
-00007f20: 206e 4832 2873 656c 662c 7661 6c75 6529   nH2(self,value)
-00007f30: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
-00007f40: 6e48 323d 7661 6c75 650a 0a20 2020 2040  nH2=value..    @
-00007f50: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-00007f60: 2064 7573 745f 746f 5f67 6173 2873 656c   dust_to_gas(sel
-00007f70: 6629 3a0a 2020 2020 2020 2020 6966 2073  f):.        if s
-00007f80: 656c 662e 6e6d 6f64 656c 733e 313a 0a20  elf.nmodels>1:. 
-00007f90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007fa0: 5f64 7573 745f 746f 5f67 6173 3d5b 5d0a  _dust_to_gas=[].
-00007fb0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00007fc0: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
-00007fd0: 6e6d 6f64 656c 7329 3a0a 2020 2020 2020  nmodels):.      
-00007fe0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00007ff0: 6475 7374 5f74 6f5f 6761 732e 6170 7065  dust_to_gas.appe
-00008000: 6e64 2873 656c 662e 6d6f 6465 6c73 5b69  nd(self.models[i
-00008010: 5d2e 6475 7374 5f74 6f5f 6761 7329 0a20  ].dust_to_gas). 
-00008020: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00008030: 2020 2020 2020 2020 2073 656c 662e 5f64           self._d
-00008040: 7573 745f 746f 5f67 6173 3d73 656c 662e  ust_to_gas=self.
-00008050: 6d6f 6465 6c73 5b30 5d2e 6475 7374 5f74  models[0].dust_t
-00008060: 6f5f 6761 730a 2020 2020 2020 2020 7265  o_gas.        re
-00008070: 7475 726e 2073 656c 662e 5f64 7573 745f  turn self._dust_
-00008080: 746f 5f67 6173 0a0a 2020 2020 4064 7573  to_gas..    @dus
-00008090: 745f 746f 5f67 6173 2e73 6574 7465 720a  t_to_gas.setter.
-000080a0: 2020 2020 6465 6620 6475 7374 5f74 6f5f      def dust_to_
-000080b0: 6761 7328 7365 6c66 2c76 616c 7565 293a  gas(self,value):
-000080c0: 0a20 2020 2020 2020 2073 656c 662e 5f64  .        self._d
-000080d0: 7573 745f 746f 5f67 6173 3d76 616c 7565  ust_to_gas=value
-000080e0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-000080f0: 2020 2020 6465 6620 7674 7572 6228 7365      def vturb(se
-00008100: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
-00008110: 7365 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a  self.nmodels>1:.
-00008120: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00008130: 2e5f 7674 7572 623d 5b5d 0a20 2020 2020  ._vturb=[].     
-00008140: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-00008150: 7261 6e67 6528 7365 6c66 2e6e 6d6f 6465  range(self.nmode
-00008160: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
-00008170: 2020 2020 2073 656c 662e 5f76 7475 7262       self._vturb
-00008180: 2e61 7070 656e 6428 7365 6c66 2e6d 6f64  .append(self.mod
-00008190: 656c 735b 695d 2e76 7475 7262 290a 2020  els[i].vturb).  
-000081a0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000081b0: 2020 2020 2020 2020 7365 6c66 2e5f 7674          self._vt
-000081c0: 7572 623d 7365 6c66 2e6d 6f64 656c 735b  urb=self.models[
-000081d0: 305d 2e76 7475 7262 0a20 2020 2020 2020  0].vturb.       
-000081e0: 2072 6574 7572 6e20 7365 6c66 2e5f 7674   return self._vt
-000081f0: 7572 620a 0a20 2020 2040 7674 7572 622e  urb..    @vturb.
-00008200: 7365 7474 6572 0a20 2020 2064 6566 2076  setter.    def v
-00008210: 7475 7262 2873 656c 662c 7661 6c75 6529  turb(self,value)
-00008220: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
-00008230: 7674 7572 623d 7661 6c75 650a 0a20 2020  vturb=value..   
-00008240: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-00008250: 6566 2054 6728 7365 6c66 293a 0a20 2020  ef Tg(self):.   
-00008260: 2020 2020 2069 6620 7365 6c66 2e6e 6d6f       if self.nmo
-00008270: 6465 6c73 3e31 3a0a 2020 2020 2020 2020  dels>1:.        
-00008280: 2020 2020 7365 6c66 2e5f 5467 3d5b 5d0a      self._Tg=[].
-00008290: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000082a0: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
-000082b0: 6e6d 6f64 656c 7329 3a0a 2020 2020 2020  nmodels):.      
-000082c0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-000082d0: 5467 2e61 7070 656e 6428 7365 6c66 2e6d  Tg.append(self.m
-000082e0: 6f64 656c 735b 695d 2e54 6729 0a20 2020  odels[i].Tg).   
-000082f0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00008300: 2020 2020 2020 2073 656c 662e 5f54 673d         self._Tg=
-00008310: 7365 6c66 2e6d 6f64 656c 735b 305d 2e54  self.models[0].T
-00008320: 670a 2020 2020 2020 2020 7265 7475 726e  g.        return
-00008330: 2073 656c 662e 5f54 670a 0a20 2020 2040   self._Tg..    @
-00008340: 5467 2e73 6574 7465 720a 2020 2020 6465  Tg.setter.    de
-00008350: 6620 5467 2873 656c 662c 7661 6c75 6529  f Tg(self,value)
-00008360: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
-00008370: 5467 3d76 616c 7565 0a0a 2020 2020 4070  Tg=value..    @p
-00008380: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00008390: 5464 2873 656c 6629 3a0a 2020 2020 2020  Td(self):.      
-000083a0: 2020 6966 2073 656c 662e 6e6d 6f64 656c    if self.nmodel
-000083b0: 733e 313a 0a20 2020 2020 2020 2020 2020  s>1:.           
-000083c0: 2073 656c 662e 5f54 643d 5b5d 0a20 2020   self._Td=[].   
-000083d0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-000083e0: 6e20 7261 6e67 6528 7365 6c66 2e6e 6d6f  n range(self.nmo
-000083f0: 6465 6c73 293a 0a20 2020 2020 2020 2020  dels):.         
-00008400: 2020 2020 2020 2073 656c 662e 5f54 642e         self._Td.
-00008410: 6170 7065 6e64 2873 656c 662e 6d6f 6465  append(self.mode
-00008420: 6c73 5b69 5d2e 5464 290a 2020 2020 2020  ls[i].Td).      
-00008430: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00008440: 2020 2020 7365 6c66 2e5f 5464 3d73 656c      self._Td=sel
-00008450: 662e 6d6f 6465 6c73 5b30 5d2e 5464 0a20  f.models[0].Td. 
-00008460: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00008470: 6c66 2e5f 5464 0a0a 2020 2020 4054 642e  lf._Td..    @Td.
-00008480: 7365 7474 6572 0a20 2020 2064 6566 2054  setter.    def T
-00008490: 6428 7365 6c66 2c76 616c 7565 293a 0a20  d(self,value):. 
-000084a0: 2020 2020 2020 2073 656c 662e 5f54 643d         self._Td=
-000084b0: 7661 6c75 650a 0a20 2020 2040 7072 6f70  value..    @prop
-000084c0: 6572 7479 0a20 2020 2064 6566 2073 7065  erty.    def spe
-000084d0: 6369 6573 5f6e 616d 6528 7365 6c66 293a  cies_name(self):
-000084e0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000084f0: 2e6e 6d6f 6465 6c73 3e31 3a0a 2020 2020  .nmodels>1:.    
-00008500: 2020 2020 2020 2020 7365 6c66 2e5f 7370          self._sp
-00008510: 6563 6965 735f 6e61 6d65 3d5b 5d0a 2020  ecies_name=[].  
-00008520: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
-00008530: 696e 2072 616e 6765 2873 656c 662e 6e6d  in range(self.nm
-00008540: 6f64 656c 7329 3a0a 2020 2020 2020 2020  odels):.        
-00008550: 2020 2020 2020 2020 7365 6c66 2e5f 7370          self._sp
-00008560: 6563 6965 735f 6e61 6d65 2e61 7070 656e  ecies_name.appen
-00008570: 6428 7365 6c66 2e6d 6f64 656c 735b 695d  d(self.models[i]
-00008580: 2e73 7065 6369 6573 5f6e 616d 6529 0a20  .species_name). 
-00008590: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000085a0: 2020 2020 2020 2020 2073 656c 662e 5f73           self._s
-000085b0: 7065 6369 6573 5f6e 616d 653d 7365 6c66  pecies_name=self
-000085c0: 2e6d 6f64 656c 735b 305d 2e73 7065 6369  .models[0].speci
-000085d0: 6573 5f6e 616d 650a 2020 2020 2020 2020  es_name.        
-000085e0: 7265 7475 726e 2073 656c 662e 5f73 7065  return self._spe
-000085f0: 6369 6573 5f6e 616d 650a 0a20 2020 2040  cies_name..    @
-00008600: 7370 6563 6965 735f 6e61 6d65 2e73 6574  species_name.set
-00008610: 7465 720a 2020 2020 6465 6620 7370 6563  ter.    def spec
-00008620: 6965 735f 6e61 6d65 2873 656c 662c 7661  ies_name(self,va
-00008630: 6c75 6529 3a0a 2020 2020 2020 2020 7365  lue):.        se
-00008640: 6c66 2e5f 7370 6563 6965 735f 6e61 6d65  lf._species_name
-00008650: 3d76 616c 7565 0a0a 2020 2020 4070 726f  =value..    @pro
-00008660: 7065 7274 790a 2020 2020 6465 6620 7370  perty.    def sp
-00008670: 6563 6965 735f 696e 6465 7828 7365 6c66  ecies_index(self
-00008680: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
-00008690: 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a 2020  lf.nmodels>1:.  
-000086a0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-000086b0: 7370 6563 6965 735f 696e 6465 783d 5b5d  species_index=[]
-000086c0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-000086d0: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
-000086e0: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
-000086f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008700: 5f73 7065 6369 6573 5f69 6e64 6578 2e61  _species_index.a
-00008710: 7070 656e 6428 7365 6c66 2e6d 6f64 656c  ppend(self.model
-00008720: 735b 695d 2e73 7065 6369 6573 5f69 6e64  s[i].species_ind
-00008730: 6578 290a 2020 2020 2020 2020 656c 7365  ex).        else
-00008740: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00008750: 6c66 2e5f 7370 6563 6965 735f 696e 6465  lf._species_inde
-00008760: 783d 7365 6c66 2e6d 6f64 656c 735b 305d  x=self.models[0]
-00008770: 2e73 7065 6369 6573 5f69 6e64 6578 0a20  .species_index. 
-00008780: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00008790: 6c66 2e5f 7370 6563 6965 735f 696e 6465  lf._species_inde
-000087a0: 780a 0a20 2020 2040 7370 6563 6965 735f  x..    @species_
-000087b0: 696e 6465 782e 7365 7474 6572 0a20 2020  index.setter.   
-000087c0: 2064 6566 2073 7065 6369 6573 5f69 6e64   def species_ind
-000087d0: 6578 2873 656c 662c 7661 6c75 6529 3a0a  ex(self,value):.
-000087e0: 2020 2020 2020 2020 7365 6c66 2e5f 7370          self._sp
-000087f0: 6563 6965 735f 696e 6465 783d 7661 6c75  ecies_index=valu
-00008800: 650a 0a20 2020 2040 7072 6f70 6572 7479  e..    @property
-00008810: 0a20 2020 2064 6566 2061 6275 6e64 616e  .    def abundan
-00008820: 6365 2873 656c 6629 3a0a 2020 2020 2020  ce(self):.      
-00008830: 2020 6966 2073 656c 662e 6e6d 6f64 656c    if self.nmodel
-00008840: 733e 313a 0a20 2020 2020 2020 2020 2020  s>1:.           
-00008850: 2073 656c 662e 5f61 6275 6e64 616e 6365   self._abundance
-00008860: 3d5b 5d0a 2020 2020 2020 2020 2020 2020  =[].            
-00008870: 666f 7220 6920 696e 2072 616e 6765 2873  for i in range(s
-00008880: 656c 662e 6e6d 6f64 656c 7329 3a0a 2020  elf.nmodels):.  
-00008890: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000088a0: 6c66 2e5f 6162 756e 6461 6e63 652e 6170  lf._abundance.ap
-000088b0: 7065 6e64 2873 656c 662e 6d6f 6465 6c73  pend(self.models
-000088c0: 5b69 5d2e 6162 756e 6461 6e63 6529 0a20  [i].abundance). 
-000088d0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000088e0: 2020 2020 2020 2020 2073 656c 662e 5f61           self._a
-000088f0: 6275 6e64 616e 6365 3d73 656c 662e 6d6f  bundance=self.mo
-00008900: 6465 6c73 5b30 5d2e 6162 756e 6461 6e63  dels[0].abundanc
-00008910: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
-00008920: 2073 656c 662e 5f61 6275 6e64 616e 6365   self._abundance
-00008930: 0a0a 2020 2020 4061 6275 6e64 616e 6365  ..    @abundance
-00008940: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
-00008950: 6162 756e 6461 6e63 6528 7365 6c66 2c76  abundance(self,v
-00008960: 616c 7565 293a 0a20 2020 2020 2020 2073  alue):.        s
-00008970: 656c 662e 5f61 6275 6e64 616e 6365 3d76  elf._abundance=v
-00008980: 616c 7565 0a0a 2020 2020 4070 726f 7065  alue..    @prope
-00008990: 7274 790a 2020 2020 6465 6620 6476 2873  rty.    def dv(s
-000089a0: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
-000089b0: 2073 656c 662e 6e6d 6f64 656c 733e 313a   self.nmodels>1:
-000089c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000089d0: 662e 5f64 763d 5b5d 0a20 2020 2020 2020  f._dv=[].       
-000089e0: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-000089f0: 6e67 6528 7365 6c66 2e6e 6d6f 6465 6c73  nge(self.nmodels
-00008a00: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00008a10: 2020 2073 656c 662e 5f64 762e 6170 7065     self._dv.appe
-00008a20: 6e64 2873 656c 662e 6d6f 6465 6c73 5b69  nd(self.models[i
-00008a30: 5d2e 6476 290a 2020 2020 2020 2020 656c  ].dv).        el
-00008a40: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00008a50: 7365 6c66 2e5f 6476 3d73 656c 662e 6d6f  self._dv=self.mo
-00008a60: 6465 6c73 5b30 5d2e 6476 0a20 2020 2020  dels[0].dv.     
-00008a70: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-00008a80: 6476 0a0a 2020 2020 4064 762e 7365 7474  dv..    @dv.sett
-00008a90: 6572 0a20 2020 2064 6566 2064 7628 7365  er.    def dv(se
-00008aa0: 6c66 2c76 616c 7565 293a 0a20 2020 2020  lf,value):.     
-00008ab0: 2020 2073 656c 662e 5f64 763d 7661 6c75     self._dv=valu
-00008ac0: 650a 0a20 2020 2040 7072 6f70 6572 7479  e..    @property
-00008ad0: 0a20 2020 2064 6566 206e 6c65 7665 6c73  .    def nlevels
-00008ae0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00008af0: 6966 2073 656c 662e 6e6d 6f64 656c 733e  if self.nmodels>
-00008b00: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
-00008b10: 656c 662e 5f6e 6c65 7665 6c73 3d5b 5d0a  elf._nlevels=[].
-00008b20: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00008b30: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
-00008b40: 6e6d 6f64 656c 7329 3a0a 2020 2020 2020  nmodels):.      
-00008b50: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00008b60: 6e6c 6576 656c 732e 6170 7065 6e64 2873  nlevels.append(s
-00008b70: 656c 662e 6d6f 6465 6c73 5b69 5d2e 6e6c  elf.models[i].nl
-00008b80: 6576 656c 7329 0a20 2020 2020 2020 2065  evels).        e
-00008b90: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00008ba0: 2073 656c 662e 5f6e 6c65 7665 6c73 3d73   self._nlevels=s
-00008bb0: 656c 662e 6d6f 6465 6c73 5b30 5d2e 6e6c  elf.models[0].nl
-00008bc0: 6576 656c 730a 2020 2020 2020 2020 7265  evels.        re
-00008bd0: 7475 726e 2073 656c 662e 5f6e 6c65 7665  turn self._nleve
-00008be0: 6c73 0a0a 2020 2020 406e 6c65 7665 6c73  ls..    @nlevels
-00008bf0: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
-00008c00: 6e6c 6576 656c 7328 7365 6c66 2c76 616c  nlevels(self,val
-00008c10: 7565 293a 0a20 2020 2020 2020 2073 656c  ue):.        sel
-00008c20: 662e 5f6e 6c65 7665 6c73 3d76 616c 7565  f._nlevels=value
-00008c30: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-00008c40: 2020 2020 6465 6620 6e6c 696e 6573 2873      def nlines(s
-00008c50: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
-00008c60: 2073 656c 662e 6e6d 6f64 656c 733e 313a   self.nmodels>1:
-00008c70: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00008c80: 662e 5f6e 6c69 6e65 733d 5b5d 0a20 2020  f._nlines=[].   
-00008c90: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-00008ca0: 6e20 7261 6e67 6528 7365 6c66 2e6e 6d6f  n range(self.nmo
-00008cb0: 6465 6c73 293a 0a20 2020 2020 2020 2020  dels):.         
-00008cc0: 2020 2020 2020 2073 656c 662e 5f6e 6c69         self._nli
-00008cd0: 6e65 732e 6170 7065 6e64 2873 656c 662e  nes.append(self.
-00008ce0: 6d6f 6465 6c73 5b69 5d2e 6e6c 696e 6573  models[i].nlines
-00008cf0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00008d00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00008d10: 2e5f 6e6c 696e 6573 3d73 656c 662e 6d6f  ._nlines=self.mo
-00008d20: 6465 6c73 5b30 5d2e 6e6c 696e 6573 0a20  dels[0].nlines. 
-00008d30: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00008d40: 6c66 2e5f 6e6c 696e 6573 0a0a 2020 2020  lf._nlines..    
-00008d50: 406e 6c69 6e65 732e 7365 7474 6572 0a20  @nlines.setter. 
-00008d60: 2020 2064 6566 206e 6c69 6e65 7328 7365     def nlines(se
-00008d70: 6c66 2c76 616c 7565 293a 0a20 2020 2020  lf,value):.     
-00008d80: 2020 2073 656c 662e 5f6e 6c69 6e65 733d     self._nlines=
-00008d90: 7661 6c75 650a 0a20 2020 2040 7072 6f70  value..    @prop
-00008da0: 6572 7479 0a20 2020 2064 6566 206c 696e  erty.    def lin
-00008db0: 6564 6174 6128 7365 6c66 293a 0a20 2020  edata(self):.   
-00008dc0: 2020 2020 2069 6620 7365 6c66 2e6e 6d6f       if self.nmo
-00008dd0: 6465 6c73 3e31 3a0a 2020 2020 2020 2020  dels>1:.        
-00008de0: 2020 2020 7365 6c66 2e5f 6c69 6e65 6461      self._lineda
-00008df0: 7461 3d5b 5d0a 2020 2020 2020 2020 2020  ta=[].          
-00008e00: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-00008e10: 2873 656c 662e 6e6d 6f64 656c 7329 3a0a  (self.nmodels):.
-00008e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e30: 7365 6c66 2e5f 6c69 6e65 6461 7461 2e61  self._linedata.a
-00008e40: 7070 656e 6428 7365 6c66 2e6d 6f64 656c  ppend(self.model
-00008e50: 735b 695d 2e6c 696e 6564 6174 6129 0a20  s[i].linedata). 
-00008e60: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00008e70: 2020 2020 2020 2020 2073 656c 662e 5f6c           self._l
-00008e80: 696e 6564 6174 613d 7365 6c66 2e6d 6f64  inedata=self.mod
-00008e90: 656c 735b 305d 2e6c 696e 6564 6174 610a  els[0].linedata.
-00008ea0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00008eb0: 656c 662e 5f6c 696e 6564 6174 610a 0a20  elf._linedata.. 
-00008ec0: 2020 2040 6c69 6e65 6461 7461 2e73 6574     @linedata.set
-00008ed0: 7465 720a 2020 2020 6465 6620 6c69 6e65  ter.    def line
-00008ee0: 6461 7461 2873 656c 662c 7661 6c75 6529  data(self,value)
-00008ef0: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
-00008f00: 6c69 6e65 6461 7461 3d76 616c 7565 0a0a  linedata=value..
-00008f10: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-00008f20: 2020 6465 6620 6c65 7665 6c64 6174 6128    def leveldata(
-00008f30: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
-00008f40: 6620 7365 6c66 2e6e 6d6f 6465 6c73 3e31  f self.nmodels>1
-00008f50: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00008f60: 6c66 2e5f 6c65 7665 6c64 6174 613d 5b5d  lf._leveldata=[]
-00008f70: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00008f80: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
-00008f90: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
-00008fa0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008fb0: 5f6c 6576 656c 6461 7461 2e61 7070 656e  _leveldata.appen
-00008fc0: 6428 7365 6c66 2e6d 6f64 656c 735b 695d  d(self.models[i]
-00008fd0: 2e6c 6576 656c 6461 7461 290a 2020 2020  .leveldata).    
-00008fe0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00008ff0: 2020 2020 2020 7365 6c66 2e5f 6c65 7665        self._leve
-00009000: 6c64 6174 613d 7365 6c66 2e6d 6f64 656c  ldata=self.model
-00009010: 735b 305d 2e6c 6576 656c 6461 7461 0a20  s[0].leveldata. 
-00009020: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00009030: 6c66 2e5f 6c65 7665 6c64 6174 610a 0a20  lf._leveldata.. 
-00009040: 2020 2040 6c65 7665 6c64 6174 612e 7365     @leveldata.se
-00009050: 7474 6572 0a20 2020 2064 6566 206c 6576  tter.    def lev
-00009060: 656c 6461 7461 2873 656c 662c 7661 6c75  eldata(self,valu
-00009070: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
-00009080: 2e5f 6c65 7665 6c64 6174 613d 7661 6c75  ._leveldata=valu
-00009090: 650a 0a20 2020 2040 7072 6f70 6572 7479  e..    @property
-000090a0: 0a20 2020 2064 6566 2063 6f6e 7657 6176  .    def convWav
-000090b0: 656c 656e 6774 6828 7365 6c66 293a 0a20  elength(self):. 
-000090c0: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
-000090d0: 6d6f 6465 6c73 3e31 3a0a 2020 2020 2020  models>1:.      
-000090e0: 2020 2020 2020 7365 6c66 2e5f 636f 6e76        self._conv
-000090f0: 5761 7665 6c65 6e67 7468 3d5b 5d0a 2020  Wavelength=[].  
-00009100: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
-00009110: 696e 2072 616e 6765 2873 656c 662e 6e6d  in range(self.nm
-00009120: 6f64 656c 7329 3a0a 2020 2020 2020 2020  odels):.        
-00009130: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
-00009140: 6e76 5761 7665 6c65 6e67 7468 2e61 7070  nvWavelength.app
-00009150: 656e 6428 7365 6c66 2e6d 6f64 656c 735b  end(self.models[
-00009160: 695d 2e63 6f6e 7657 6176 656c 656e 6774  i].convWavelengt
-00009170: 6829 0a20 2020 2020 2020 2065 6c73 653a  h).        else:
-00009180: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00009190: 662e 5f63 6f6e 7657 6176 656c 656e 6774  f._convWavelengt
-000091a0: 683d 7365 6c66 2e6d 6f64 656c 735b 305d  h=self.models[0]
-000091b0: 2e63 6f6e 7657 6176 656c 656e 6774 680a  .convWavelength.
-000091c0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000091d0: 656c 662e 5f63 6f6e 7657 6176 656c 656e  elf._convWavelen
-000091e0: 6774 680a 0a20 2020 2040 636f 6e76 5761  gth..    @convWa
-000091f0: 7665 6c65 6e67 7468 2e73 6574 7465 720a  velength.setter.
-00009200: 2020 2020 6465 6620 636f 6e76 5761 7665      def convWave
-00009210: 6c65 6e67 7468 2873 656c 662c 7661 6c75  length(self,valu
-00009220: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
-00009230: 2e5f 636f 6e76 5761 7665 6c65 6e67 7468  ._convWavelength
-00009240: 3d76 616c 7565 0a0a 2020 2020 4070 726f  =value..    @pro
-00009250: 7065 7274 790a 2020 2020 6465 6620 636f  perty.    def co
-00009260: 6e76 4c54 4566 6c75 7828 7365 6c66 293a  nvLTEflux(self):
-00009270: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00009280: 2e6e 6d6f 6465 6c73 3e31 3a0a 2020 2020  .nmodels>1:.    
-00009290: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
-000092a0: 6e76 4c54 4566 6c75 783d 5b5d 0a20 2020  nvLTEflux=[].   
-000092b0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-000092c0: 6e20 7261 6e67 6528 7365 6c66 2e6e 6d6f  n range(self.nmo
-000092d0: 6465 6c73 293a 0a20 2020 2020 2020 2020  dels):.         
-000092e0: 2020 2020 2020 2073 656c 662e 5f63 6f6e         self._con
-000092f0: 764c 5445 666c 7578 2e61 7070 656e 6428  vLTEflux.append(
-00009300: 7365 6c66 2e6d 6f64 656c 735b 695d 2e63  self.models[i].c
-00009310: 6f6e 764c 5445 666c 7578 290a 2020 2020  onvLTEflux).    
-00009320: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00009330: 2020 2020 2020 7365 6c66 2e5f 636f 6e76        self._conv
-00009340: 4c54 4566 6c75 783d 7365 6c66 2e6d 6f64  LTEflux=self.mod
-00009350: 656c 735b 305d 2e63 6f6e 764c 5445 666c  els[0].convLTEfl
-00009360: 7578 0a20 2020 2020 2020 2072 6574 7572  ux.        retur
-00009370: 6e20 7365 6c66 2e5f 636f 6e76 4c54 4566  n self._convLTEf
-00009380: 6c75 780a 0a20 2020 2040 636f 6e76 4c54  lux..    @convLT
-00009390: 4566 6c75 782e 7365 7474 6572 0a20 2020  Eflux.setter.   
-000093a0: 2064 6566 2063 6f6e 764c 5445 666c 7578   def convLTEflux
-000093b0: 2873 656c 662c 7661 6c75 6529 3a0a 2020  (self,value):.  
-000093c0: 2020 2020 2020 7365 6c66 2e5f 636f 6e76        self._conv
-000093d0: 4c54 4566 6c75 783d 7661 6c75 650a 0a20  LTEflux=value.. 
-000093e0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-000093f0: 2064 6566 2063 6f6e 764e 4c54 4566 6c75   def convNLTEflu
-00009400: 7828 7365 6c66 293a 0a20 2020 2020 2020  x(self):.       
-00009410: 2069 6620 7365 6c66 2e6e 6d6f 6465 6c73   if self.nmodels
-00009420: 3e31 3a0a 2020 2020 2020 2020 2020 2020  >1:.            
-00009430: 7365 6c66 2e5f 636f 6e76 4e4c 5445 666c  self._convNLTEfl
-00009440: 7578 3d5b 5d0a 2020 2020 2020 2020 2020  ux=[].          
-00009450: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-00009460: 2873 656c 662e 6e6d 6f64 656c 7329 3a0a  (self.nmodels):.
-00009470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009480: 7365 6c66 2e5f 636f 6e76 4e4c 5445 666c  self._convNLTEfl
-00009490: 7578 2e61 7070 656e 6428 7365 6c66 2e6d  ux.append(self.m
-000094a0: 6f64 656c 735b 695d 2e63 6f6e 764e 4c54  odels[i].convNLT
-000094b0: 4566 6c75 7829 0a20 2020 2020 2020 2065  Eflux).        e
-000094c0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-000094d0: 2073 656c 662e 5f63 6f6e 764e 4c54 4566   self._convNLTEf
-000094e0: 6c75 783d 7365 6c66 2e6d 6f64 656c 735b  lux=self.models[
-000094f0: 305d 2e63 6f6e 764e 4c54 4566 6c75 780a  0].convNLTEflux.
-00009500: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00009510: 656c 662e 5f63 6f6e 764e 4c54 4566 6c75  elf._convNLTEflu
-00009520: 780a 0a20 2020 2040 636f 6e76 4e4c 5445  x..    @convNLTE
-00009530: 666c 7578 2e73 6574 7465 720a 2020 2020  flux.setter.    
-00009540: 6465 6620 636f 6e76 4e4c 5445 666c 7578  def convNLTEflux
-00009550: 2873 656c 662c 7661 6c75 6529 3a0a 2020  (self,value):.  
-00009560: 2020 2020 2020 7365 6c66 2e5f 636f 6e76        self._conv
-00009570: 4e4c 5445 666c 7578 3d76 616c 7565 0a0a  NLTEflux=value..
-00009580: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-00009590: 2020 6465 6620 636f 6e76 5479 7065 2873    def convType(s
-000095a0: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
-000095b0: 2073 656c 662e 6e6d 6f64 656c 733e 313a   self.nmodels>1:
-000095c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000095d0: 662e 5f63 6f6e 7654 7970 653d 5b5d 0a20  f._convType=[]. 
-000095e0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-000095f0: 2069 6e20 7261 6e67 6528 7365 6c66 2e6e   in range(self.n
-00009600: 6d6f 6465 6c73 293a 0a20 2020 2020 2020  models):.       
-00009610: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
-00009620: 6f6e 7654 7970 652e 6170 7065 6e64 2873  onvType.append(s
-00009630: 656c 662e 6d6f 6465 6c73 5b69 5d2e 636f  elf.models[i].co
-00009640: 6e76 5479 7065 290a 2020 2020 2020 2020  nvType).        
-00009650: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00009660: 2020 7365 6c66 2e5f 636f 6e76 5479 7065    self._convType
-00009670: 3d73 656c 662e 6d6f 6465 6c73 5b30 5d2e  =self.models[0].
-00009680: 636f 6e76 5479 7065 0a20 2020 2020 2020  convType.       
-00009690: 2072 6574 7572 6e20 7365 6c66 2e5f 636f   return self._co
-000096a0: 6e76 5479 7065 0a0a 2020 2020 4063 6f6e  nvType..    @con
-000096b0: 7654 7970 652e 7365 7474 6572 0a20 2020  vType.setter.   
-000096c0: 2064 6566 2063 6f6e 7654 7970 6528 7365   def convType(se
-000096d0: 6c66 2c76 616c 7565 293a 0a20 2020 2020  lf,value):.     
-000096e0: 2020 2073 656c 662e 5f63 6f6e 7654 7970     self._convTyp
-000096f0: 653d 7661 6c75 650a 0a20 2020 2040 7072  e=value..    @pr
-00009700: 6f70 6572 7479 0a20 2020 2064 6566 2063  operty.    def c
-00009710: 6f6e 7652 2873 656c 6629 3a0a 2020 2020  onvR(self):.    
-00009720: 2020 2020 6966 2073 656c 662e 6e6d 6f64      if self.nmod
-00009730: 656c 733e 313a 0a20 2020 2020 2020 2020  els>1:.         
-00009740: 2020 2073 656c 662e 5f63 6f6e 7652 3d5b     self._convR=[
-00009750: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
-00009760: 7220 6920 696e 2072 616e 6765 2873 656c  r i in range(sel
-00009770: 662e 6e6d 6f64 656c 7329 3a0a 2020 2020  f.nmodels):.    
-00009780: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00009790: 2e5f 636f 6e76 522e 6170 7065 6e64 2873  ._convR.append(s
-000097a0: 656c 662e 6d6f 6465 6c73 5b69 5d2e 636f  elf.models[i].co
-000097b0: 6e76 5229 0a20 2020 2020 2020 2065 6c73  nvR).        els
-000097c0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-000097d0: 656c 662e 5f63 6f6e 7652 3d73 656c 662e  elf._convR=self.
-000097e0: 6d6f 6465 6c73 5b30 5d2e 636f 6e76 520a  models[0].convR.
-000097f0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00009800: 656c 662e 5f63 6f6e 7652 0a0a 2020 2020  elf._convR..    
-00009810: 4063 6f6e 7652 2e73 6574 7465 720a 2020  @convR.setter.  
-00009820: 2020 6465 6620 636f 6e76 5228 7365 6c66    def convR(self
-00009830: 2c76 616c 7565 293a 0a20 2020 2020 2020  ,value):.       
-00009840: 2073 656c 662e 5f63 6f6e 7652 3d76 616c   self._convR=val
-00009850: 7565 0a0a 2020 2020 4070 726f 7065 7274  ue..    @propert
-00009860: 790a 2020 2020 6465 6620 636f 6e76 4f76  y.    def convOv
-00009870: 6572 6c61 7046 7265 7128 7365 6c66 293a  erlapFreq(self):
-00009880: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00009890: 2e6e 6d6f 6465 6c73 3e31 3a0a 2020 2020  .nmodels>1:.    
-000098a0: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
-000098b0: 6e76 4f76 6572 6c61 7046 7265 713d 5b5d  nvOverlapFreq=[]
-000098c0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-000098d0: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
-000098e0: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
-000098f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00009900: 5f63 6f6e 764f 7665 726c 6170 4672 6571  _convOverlapFreq
-00009910: 2e61 7070 656e 6428 7365 6c66 2e6d 6f64  .append(self.mod
-00009920: 656c 735b 695d 2e63 6f6e 764f 7665 726c  els[i].convOverl
-00009930: 6170 4672 6571 290a 2020 2020 2020 2020  apFreq).        
-00009940: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00009950: 2020 7365 6c66 2e5f 636f 6e76 4f76 6572    self._convOver
-00009960: 6c61 7046 7265 713d 7365 6c66 2e6d 6f64  lapFreq=self.mod
-00009970: 656c 735b 305d 2e63 6f6e 764f 7665 726c  els[0].convOverl
-00009980: 6170 4672 6571 0a20 2020 2020 2020 2072  apFreq.        r
-00009990: 6574 7572 6e20 7365 6c66 2e5f 636f 6e76  eturn self._conv
-000099a0: 4f76 6572 6c61 7046 7265 710a 0a20 2020  OverlapFreq..   
-000099b0: 2040 636f 6e76 4f76 6572 6c61 7046 7265   @convOverlapFre
-000099c0: 712e 7365 7474 6572 0a20 2020 2064 6566  q.setter.    def
-000099d0: 2063 6f6e 764f 7665 726c 6170 4672 6571   convOverlapFreq
-000099e0: 2873 656c 662c 7661 6c75 6529 3a0a 2020  (self,value):.  
-000099f0: 2020 2020 2020 7365 6c66 2e5f 636f 6e76        self._conv
-00009a00: 4f76 6572 6c61 7046 7265 713d 7661 6c75  OverlapFreq=valu
-00009a10: 650a 0a20 2020 2040 7072 6f70 6572 7479  e..    @property
-00009a20: 0a20 2020 2064 6566 2063 6f6e 764f 7665  .    def convOve
-00009a30: 726c 6170 5761 7665 2873 656c 6629 3a0a  rlapWave(self):.
-00009a40: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00009a50: 6e6d 6f64 656c 733e 313a 0a20 2020 2020  nmodels>1:.     
-00009a60: 2020 2020 2020 2073 656c 662e 5f63 6f6e         self._con
-00009a70: 764f 7665 726c 6170 5761 7665 3d5b 5d0a  vOverlapWave=[].
-00009a80: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00009a90: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
-00009aa0: 6e6d 6f64 656c 7329 3a0a 2020 2020 2020  nmodels):.      
-00009ab0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00009ac0: 636f 6e76 4f76 6572 6c61 7057 6176 652e  convOverlapWave.
-00009ad0: 6170 7065 6e64 2873 656c 662e 6d6f 6465  append(self.mode
-00009ae0: 6c73 5b69 5d2e 636f 6e76 4f76 6572 6c61  ls[i].convOverla
-00009af0: 7057 6176 6529 0a20 2020 2020 2020 2065  pWave).        e
-00009b00: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00009b10: 2073 656c 662e 5f63 6f6e 764f 7665 726c   self._convOverl
-00009b20: 6170 5761 7665 3d73 656c 662e 6d6f 6465  apWave=self.mode
-00009b30: 6c73 5b30 5d2e 636f 6e76 4f76 6572 6c61  ls[0].convOverla
-00009b40: 7057 6176 650a 2020 2020 2020 2020 7265  pWave.        re
-00009b50: 7475 726e 2073 656c 662e 5f63 6f6e 764f  turn self._convO
-00009b60: 7665 726c 6170 5761 7665 0a0a 2020 2020  verlapWave..    
-00009b70: 4063 6f6e 764f 7665 726c 6170 5761 7665  @convOverlapWave
-00009b80: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
-00009b90: 636f 6e76 4f76 6572 6c61 7057 6176 6528  convOverlapWave(
-00009ba0: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
-00009bb0: 2020 2020 2073 656c 662e 5f63 6f6e 764f       self._convO
-00009bc0: 7665 726c 6170 5761 7665 3d76 616c 7565  verlapWave=value
-00009bd0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-00009be0: 2020 2020 6465 6620 6f76 6572 6c61 7046      def overlapF
-00009bf0: 7265 7128 7365 6c66 293a 0a20 2020 2020  req(self):.     
-00009c00: 2020 2069 6620 7365 6c66 2e6e 6d6f 6465     if self.nmode
-00009c10: 6c73 3e31 3a0a 2020 2020 2020 2020 2020  ls>1:.          
-00009c20: 2020 7365 6c66 2e5f 6f76 6572 6c61 7046    self._overlapF
-00009c30: 7265 713d 5b5d 0a20 2020 2020 2020 2020  req=[].         
-00009c40: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-00009c50: 6528 7365 6c66 2e6e 6d6f 6465 6c73 293a  e(self.nmodels):
-00009c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009c70: 2073 656c 662e 5f6f 7665 726c 6170 4672   self._overlapFr
-00009c80: 6571 2e61 7070 656e 6428 7365 6c66 2e6d  eq.append(self.m
-00009c90: 6f64 656c 735b 695d 2e6f 7665 726c 6170  odels[i].overlap
-00009ca0: 4672 6571 290a 2020 2020 2020 2020 656c  Freq).        el
-00009cb0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00009cc0: 7365 6c66 2e5f 6f76 6572 6c61 7046 7265  self._overlapFre
-00009cd0: 713d 7365 6c66 2e6d 6f64 656c 735b 305d  q=self.models[0]
-00009ce0: 2e6f 7665 726c 6170 4672 6571 0a20 2020  .overlapFreq.   
-00009cf0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00009d00: 2e5f 6f76 6572 6c61 7046 7265 710a 0a20  ._overlapFreq.. 
-00009d10: 2020 2040 6f76 6572 6c61 7046 7265 712e     @overlapFreq.
-00009d20: 7365 7474 6572 0a20 2020 2064 6566 206f  setter.    def o
-00009d30: 7665 726c 6170 4672 6571 2873 656c 662c  verlapFreq(self,
-00009d40: 7661 6c75 6529 3a0a 2020 2020 2020 2020  value):.        
-00009d50: 7365 6c66 2e5f 6f76 6572 6c61 7046 7265  self._overlapFre
-00009d60: 713d 7661 6c75 650a 0a20 2020 2040 7072  q=value..    @pr
-00009d70: 6f70 6572 7479 0a20 2020 2064 6566 2063  operty.    def c
-00009d80: 6f6e 764f 7665 726c 6170 4c54 4528 7365  onvOverlapLTE(se
-00009d90: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
-00009da0: 7365 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a  self.nmodels>1:.
-00009db0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00009dc0: 2e5f 636f 6e76 4f76 6572 6c61 704c 5445  ._convOverlapLTE
-00009dd0: 3d5b 5d0a 2020 2020 2020 2020 2020 2020  =[].            
-00009de0: 666f 7220 6920 696e 2072 616e 6765 2873  for i in range(s
-00009df0: 656c 662e 6e6d 6f64 656c 7329 3a0a 2020  elf.nmodels):.  
-00009e00: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00009e10: 6c66 2e5f 636f 6e76 4f76 6572 6c61 704c  lf._convOverlapL
-00009e20: 5445 2e61 7070 656e 6428 7365 6c66 2e6d  TE.append(self.m
-00009e30: 6f64 656c 735b 695d 2e63 6f6e 764f 7665  odels[i].convOve
-00009e40: 726c 6170 4c54 4529 0a20 2020 2020 2020  rlapLTE).       
-00009e50: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00009e60: 2020 2073 656c 662e 5f63 6f6e 764f 7665     self._convOve
-00009e70: 726c 6170 4c54 453d 7365 6c66 2e6d 6f64  rlapLTE=self.mod
-00009e80: 656c 735b 305d 2e63 6f6e 764f 7665 726c  els[0].convOverl
-00009e90: 6170 4c54 450a 2020 2020 2020 2020 7265  apLTE.        re
-00009ea0: 7475 726e 2073 656c 662e 5f63 6f6e 764f  turn self._convO
-00009eb0: 7665 726c 6170 4c54 450a 0a20 2020 2040  verlapLTE..    @
-00009ec0: 636f 6e76 4f76 6572 6c61 704c 5445 2e73  convOverlapLTE.s
-00009ed0: 6574 7465 720a 2020 2020 6465 6620 636f  etter.    def co
-00009ee0: 6e76 4f76 6572 6c61 704c 5445 2873 656c  nvOverlapLTE(sel
-00009ef0: 662c 7661 6c75 6529 3a0a 2020 2020 2020  f,value):.      
-00009f00: 2020 7365 6c66 2e5f 636f 6e76 4f76 6572    self._convOver
-00009f10: 6c61 704c 5445 3d76 616c 7565 0a0a 2020  lapLTE=value..  
-00009f20: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-00009f30: 6465 6620 636f 6e76 4f76 6572 6c61 704e  def convOverlapN
-00009f40: 4c54 4528 7365 6c66 293a 0a20 2020 2020  LTE(self):.     
-00009f50: 2020 2069 6620 7365 6c66 2e6e 6d6f 6465     if self.nmode
-00009f60: 6c73 3e31 3a0a 2020 2020 2020 2020 2020  ls>1:.          
-00009f70: 2020 7365 6c66 2e5f 636f 6e76 4f76 6572    self._convOver
-00009f80: 6c61 704e 4c54 453d 5b5d 0a20 2020 2020  lapNLTE=[].     
-00009f90: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-00009fa0: 7261 6e67 6528 7365 6c66 2e6e 6d6f 6465  range(self.nmode
-00009fb0: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
-00009fc0: 2020 2020 2073 656c 662e 5f63 6f6e 764f       self._convO
-00009fd0: 7665 726c 6170 4e4c 5445 2e61 7070 656e  verlapNLTE.appen
-00009fe0: 6428 7365 6c66 2e6d 6f64 656c 735b 695d  d(self.models[i]
-00009ff0: 2e63 6f6e 764f 7665 726c 6170 4e4c 5445  .convOverlapNLTE
-0000a000: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-0000a010: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000a020: 2e5f 636f 6e76 4f76 6572 6c61 704e 4c54  ._convOverlapNLT
-0000a030: 453d 7365 6c66 2e6d 6f64 656c 735b 305d  E=self.models[0]
-0000a040: 2e63 6f6e 764f 7665 726c 6170 4e4c 5445  .convOverlapNLTE
-0000a050: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000a060: 7365 6c66 2e5f 636f 6e76 4f76 6572 6c61  self._convOverla
-0000a070: 704e 4c54 450a 0a20 2020 2040 636f 6e76  pNLTE..    @conv
-0000a080: 4f76 6572 6c61 704e 4c54 452e 7365 7474  OverlapNLTE.sett
-0000a090: 6572 0a20 2020 2064 6566 2063 6f6e 764f  er.    def convO
-0000a0a0: 7665 726c 6170 4e4c 5445 2873 656c 662c  verlapNLTE(self,
-0000a0b0: 7661 6c75 6529 3a0a 2020 2020 2020 2020  value):.        
-0000a0c0: 7365 6c66 2e5f 636f 6e76 4f76 6572 6c61  self._convOverla
-0000a0d0: 704e 4c54 453d 7661 6c75 650a 0a20 2020  pNLTE=value..   
-0000a0e0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-0000a0f0: 6566 206f 7665 726c 6170 4c54 4528 7365  ef overlapLTE(se
-0000a100: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
-0000a110: 7365 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a  self.nmodels>1:.
-0000a120: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000a130: 2e5f 6f76 6572 6c61 704c 5445 3d5b 5d0a  ._overlapLTE=[].
-0000a140: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000a150: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
-0000a160: 6e6d 6f64 656c 7329 3a0a 2020 2020 2020  nmodels):.      
-0000a170: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000a180: 6f76 6572 6c61 704c 5445 2e61 7070 656e  overlapLTE.appen
-0000a190: 6428 7365 6c66 2e6d 6f64 656c 735b 695d  d(self.models[i]
-0000a1a0: 2e6f 7665 726c 6170 4c54 4529 0a20 2020  .overlapLTE).   
-0000a1b0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000a1c0: 2020 2020 2020 2073 656c 662e 5f6f 7665         self._ove
-0000a1d0: 726c 6170 4c54 453d 7365 6c66 2e6d 6f64  rlapLTE=self.mod
-0000a1e0: 656c 735b 305d 2e6f 7665 726c 6170 4c54  els[0].overlapLT
-0000a1f0: 450a 2020 2020 2020 2020 7265 7475 726e  E.        return
-0000a200: 2073 656c 662e 5f6f 7665 726c 6170 4c54   self._overlapLT
-0000a210: 450a 0a20 2020 2040 6f76 6572 6c61 704c  E..    @overlapL
-0000a220: 5445 2e73 6574 7465 720a 2020 2020 6465  TE.setter.    de
-0000a230: 6620 6f76 6572 6c61 704c 5445 2873 656c  f overlapLTE(sel
-0000a240: 662c 7661 6c75 6529 3a0a 2020 2020 2020  f,value):.      
-0000a250: 2020 7365 6c66 2e5f 6f76 6572 6c61 704c    self._overlapL
-0000a260: 5445 3d76 616c 7565 0a0a 2020 2020 4070  TE=value..    @p
-0000a270: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-0000a280: 6f76 6572 6c61 704e 4c54 4528 7365 6c66  overlapNLTE(self
-0000a290: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
-0000a2a0: 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a 2020  lf.nmodels>1:.  
-0000a2b0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000a2c0: 6f76 6572 6c61 704e 4c54 453d 5b5d 0a20  overlapNLTE=[]. 
-0000a2d0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-0000a2e0: 2069 6e20 7261 6e67 6528 7365 6c66 2e6e   in range(self.n
-0000a2f0: 6d6f 6465 6c73 293a 0a20 2020 2020 2020  models):.       
-0000a300: 2020 2020 2020 2020 2073 656c 662e 5f6f           self._o
-0000a310: 7665 726c 6170 4e4c 5445 2e61 7070 656e  verlapNLTE.appen
-0000a320: 6428 7365 6c66 2e6d 6f64 656c 735b 695d  d(self.models[i]
-0000a330: 2e6f 7665 726c 6170 4e4c 5445 290a 2020  .overlapNLTE).  
-0000a340: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000a350: 2020 2020 2020 2020 7365 6c66 2e5f 6f76          self._ov
-0000a360: 6572 6c61 704e 4c54 453d 7365 6c66 2e6d  erlapNLTE=self.m
-0000a370: 6f64 656c 735b 305d 2e6f 7665 726c 6170  odels[0].overlap
-0000a380: 4e4c 5445 0a20 2020 2020 2020 2072 6574  NLTE.        ret
-0000a390: 7572 6e20 7365 6c66 2e5f 6f76 6572 6c61  urn self._overla
-0000a3a0: 704e 4c54 450a 0a20 2020 2040 6f76 6572  pNLTE..    @over
-0000a3b0: 6c61 704e 4c54 452e 7365 7474 6572 0a20  lapNLTE.setter. 
-0000a3c0: 2020 2064 6566 206f 7665 726c 6170 4e4c     def overlapNL
-0000a3d0: 5445 2873 656c 662c 7661 6c75 6529 3a0a  TE(self,value):.
-0000a3e0: 2020 2020 2020 2020 7365 6c66 2e5f 6f76          self._ov
-0000a3f0: 6572 6c61 704e 4c54 453d 7661 6c75 650a  erlapNLTE=value.
-0000a400: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-0000a410: 2020 2064 6566 206f 7665 726c 6170 5461     def overlapTa
-0000a420: 754c 5445 2873 656c 6629 3a0a 2020 2020  uLTE(self):.    
-0000a430: 2020 2020 6966 2073 656c 662e 6e6d 6f64      if self.nmod
-0000a440: 656c 733e 313a 0a20 2020 2020 2020 2020  els>1:.         
-0000a450: 2020 2073 656c 662e 5f6f 7665 726c 6170     self._overlap
-0000a460: 5461 754c 5445 3d5b 5d0a 2020 2020 2020  TauLTE=[].      
-0000a470: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-0000a480: 616e 6765 2873 656c 662e 6e6d 6f64 656c  ange(self.nmodel
-0000a490: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-0000a4a0: 2020 2020 7365 6c66 2e5f 6f76 6572 6c61      self._overla
-0000a4b0: 7054 6175 4c54 452e 6170 7065 6e64 2873  pTauLTE.append(s
-0000a4c0: 656c 662e 6d6f 6465 6c73 5b69 5d2e 6f76  elf.models[i].ov
-0000a4d0: 6572 6c61 7054 6175 4c54 4529 0a20 2020  erlapTauLTE).   
-0000a4e0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000a4f0: 2020 2020 2020 2073 656c 662e 5f6f 7665         self._ove
-0000a500: 726c 6170 5461 754c 5445 3d73 656c 662e  rlapTauLTE=self.
-0000a510: 6d6f 6465 6c73 5b30 5d2e 6f76 6572 6c61  models[0].overla
-0000a520: 7054 6175 4c54 450a 2020 2020 2020 2020  pTauLTE.        
-0000a530: 7265 7475 726e 2073 656c 662e 5f6f 7665  return self._ove
-0000a540: 726c 6170 5461 754c 5445 0a0a 2020 2020  rlapTauLTE..    
-0000a550: 406f 7665 726c 6170 5461 754c 5445 2e73  @overlapTauLTE.s
-0000a560: 6574 7465 720a 2020 2020 6465 6620 6f76  etter.    def ov
-0000a570: 6572 6c61 7054 6175 4c54 4528 7365 6c66  erlapTauLTE(self
-0000a580: 2c76 616c 7565 293a 0a20 2020 2020 2020  ,value):.       
-0000a590: 2073 656c 662e 5f6f 7665 726c 6170 5461   self._overlapTa
-0000a5a0: 754c 5445 3d76 616c 7565 0a0a 2020 2020  uLTE=value..    
-0000a5b0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-0000a5c0: 6620 6f76 6572 6c61 7054 6175 4e4c 5445  f overlapTauNLTE
-0000a5d0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000a5e0: 6966 2073 656c 662e 6e6d 6f64 656c 733e  if self.nmodels>
-0000a5f0: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
-0000a600: 656c 662e 5f6f 7665 726c 6170 5461 754e  elf._overlapTauN
-0000a610: 4c54 453d 5b5d 0a20 2020 2020 2020 2020  LTE=[].         
-0000a620: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-0000a630: 6528 7365 6c66 2e6e 6d6f 6465 6c73 293a  e(self.nmodels):
-0000a640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a650: 2073 656c 662e 5f6f 7665 726c 6170 5461   self._overlapTa
-0000a660: 754e 4c54 452e 6170 7065 6e64 2873 656c  uNLTE.append(sel
-0000a670: 662e 6d6f 6465 6c73 5b69 5d2e 6f76 6572  f.models[i].over
-0000a680: 6c61 7054 6175 4e4c 5445 290a 2020 2020  lapTauNLTE).    
-0000a690: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000a6a0: 2020 2020 2020 7365 6c66 2e5f 6f76 6572        self._over
-0000a6b0: 6c61 7054 6175 4e4c 5445 3d73 656c 662e  lapTauNLTE=self.
-0000a6c0: 6d6f 6465 6c73 5b30 5d2e 6f76 6572 6c61  models[0].overla
-0000a6d0: 7054 6175 4e4c 5445 0a20 2020 2020 2020  pTauNLTE.       
-0000a6e0: 2072 6574 7572 6e20 7365 6c66 2e5f 6f76   return self._ov
-0000a6f0: 6572 6c61 7054 6175 4e4c 5445 0a0a 2020  erlapTauNLTE..  
-0000a700: 2020 406f 7665 726c 6170 5461 754e 4c54    @overlapTauNLT
-0000a710: 452e 7365 7474 6572 0a20 2020 2064 6566  E.setter.    def
-0000a720: 206f 7665 726c 6170 5461 754e 4c54 4528   overlapTauNLTE(
-0000a730: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
-0000a740: 2020 2020 2073 656c 662e 5f6f 7665 726c       self._overl
-0000a750: 6170 5461 754e 4c54 453d 7661 6c75 650a  apTauNLTE=value.
-0000a760: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-0000a770: 2020 2064 6566 2063 6f6e 764f 7665 726c     def convOverl
-0000a780: 6170 5228 7365 6c66 293a 0a20 2020 2020  apR(self):.     
-0000a790: 2020 2069 6620 7365 6c66 2e6e 6d6f 6465     if self.nmode
-0000a7a0: 6c73 3e31 3a0a 2020 2020 2020 2020 2020  ls>1:.          
-0000a7b0: 2020 7365 6c66 2e5f 636f 6e76 4f76 6572    self._convOver
-0000a7c0: 6c61 7052 3d5b 5d0a 2020 2020 2020 2020  lapR=[].        
-0000a7d0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-0000a7e0: 6765 2873 656c 662e 6e6d 6f64 656c 7329  ge(self.nmodels)
-0000a7f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000a800: 2020 7365 6c66 2e5f 636f 6e76 4f76 6572    self._convOver
-0000a810: 6c61 7052 2e61 7070 656e 6428 7365 6c66  lapR.append(self
-0000a820: 2e6d 6f64 656c 735b 695d 2e63 6f6e 764f  .models[i].convO
-0000a830: 7665 726c 6170 5229 0a20 2020 2020 2020  verlapR).       
-0000a840: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000a850: 2020 2073 656c 662e 5f63 6f6e 764f 7665     self._convOve
-0000a860: 726c 6170 523d 7365 6c66 2e6d 6f64 656c  rlapR=self.model
-0000a870: 735b 305d 2e63 6f6e 764f 7665 726c 6170  s[0].convOverlap
-0000a880: 520a 2020 2020 2020 2020 7265 7475 726e  R.        return
-0000a890: 2073 656c 662e 5f63 6f6e 764f 7665 726c   self._convOverl
-0000a8a0: 6170 520a 0a20 2020 2040 636f 6e76 4f76  apR..    @convOv
-0000a8b0: 6572 6c61 7052 2e73 6574 7465 720a 2020  erlapR.setter.  
-0000a8c0: 2020 6465 6620 636f 6e76 4f76 6572 6c61    def convOverla
-0000a8d0: 7052 2873 656c 662c 7661 6c75 6529 3a0a  pR(self,value):.
-0000a8e0: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
-0000a8f0: 6e76 4f76 6572 6c61 7052 3d76 616c 7565  nvOverlapR=value
-0000a900: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-0000a910: 2020 2020 6465 6620 6f76 6572 6c61 7052      def overlapR
-0000a920: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000a930: 6966 2073 656c 662e 6e6d 6f64 656c 733e  if self.nmodels>
-0000a940: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
-0000a950: 656c 662e 5f6f 7665 726c 6170 523d 5b5d  elf._overlapR=[]
-0000a960: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0000a970: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
-0000a980: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
-0000a990: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000a9a0: 5f6f 7665 726c 6170 522e 6170 7065 6e64  _overlapR.append
-0000a9b0: 2873 656c 662e 6d6f 6465 6c73 5b69 5d2e  (self.models[i].
-0000a9c0: 6f76 6572 6c61 7052 290a 2020 2020 2020  overlapR).      
-0000a9d0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000a9e0: 2020 2020 7365 6c66 2e5f 6f76 6572 6c61      self._overla
-0000a9f0: 7052 3d73 656c 662e 6d6f 6465 6c73 5b30  pR=self.models[0
-0000aa00: 5d2e 6f76 6572 6c61 7052 0a20 2020 2020  ].overlapR.     
-0000aa10: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-0000aa20: 6f76 6572 6c61 7052 0a0a 2020 2020 406f  overlapR..    @o
-0000aa30: 7665 726c 6170 522e 7365 7474 6572 0a20  verlapR.setter. 
-0000aa40: 2020 2064 6566 206f 7665 726c 6170 5228     def overlapR(
-0000aa50: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
-0000aa60: 2020 2020 2073 656c 662e 5f6f 7665 726c       self._overl
-0000aa70: 6170 523d 7661 6c75 650a 0a0a 636c 6173  apR=value...clas
-0000aa80: 7320 736c 6162 3a0a 2020 2020 2222 220a  s slab:.    """.
-0000aa90: 2020 2020 636c 6173 733a 3a20 736c 6162      class:: slab
-0000aaa0: 0a20 2020 2043 6c61 7373 2074 6f20 686f  .    Class to ho
-0000aab0: 6c64 2074 6865 2064 6174 6120 6f66 2069  ld the data of i
-0000aac0: 6e64 6976 6964 7561 6c20 736c 6162 206d  ndividual slab m
-0000aad0: 6f64 656c 730a 2020 2020 2222 220a 0a20  odels.    """.. 
-0000aae0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-0000aaf0: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
-0000ab00: 656c 662e 7370 6563 6965 735f 6e75 6d62  elf.species_numb
-0000ab10: 6572 3d4e 6f6e 650a 2020 2020 2020 2020  er=None.        
-0000ab20: 7365 6c66 2e6d 6f64 656c 5f6e 756d 6265  self.model_numbe
-0000ab30: 723d 4e6f 6e65 0a20 2020 2020 2020 2073  r=None.        s
-0000ab40: 656c 662e 4e48 3d4e 6f6e 650a 2020 2020  elf.NH=None.    
-0000ab50: 2020 2020 7365 6c66 2e6e 436f 6c6c 3d4e      self.nColl=N
-0000ab60: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
-0000ab70: 2e6e 653d 4e6f 6e65 0a20 2020 2020 2020  .ne=None.       
-0000ab80: 2073 656c 662e 6e48 653d 4e6f 6e65 0a20   self.nHe=None. 
-0000ab90: 2020 2020 2020 2073 656c 662e 6e48 4949         self.nHII
-0000aba0: 3d4e 6f6e 650a 2020 2020 2020 2020 7365  =None.        se
-0000abb0: 6c66 2e6e 4849 3d4e 6f6e 650a 2020 2020  lf.nHI=None.    
-0000abc0: 2020 2020 7365 6c66 2e6e 4832 3d4e 6f6e      self.nH2=Non
-0000abd0: 650a 2020 2020 2020 2020 7365 6c66 2e64  e.        self.d
-0000abe0: 7573 745f 746f 5f67 6173 3d4e 6f6e 650a  ust_to_gas=None.
-0000abf0: 2020 2020 2020 2020 7365 6c66 2e76 7475          self.vtu
-0000ac00: 7262 3d4e 6f6e 650a 2020 2020 2020 2020  rb=None.        
-0000ac10: 7365 6c66 2e54 673d 4e6f 6e65 0a20 2020  self.Tg=None.   
-0000ac20: 2020 2020 2073 656c 662e 5464 3d4e 6f6e       self.Td=Non
-0000ac30: 650a 2020 2020 2020 2020 7365 6c66 2e73  e.        self.s
-0000ac40: 7065 6369 6573 5f6e 616d 653d 4e6f 6e65  pecies_name=None
-0000ac50: 0a20 2020 2020 2020 2073 656c 662e 7370  .        self.sp
-0000ac60: 6563 6965 735f 696e 6465 783d 4e6f 6e65  ecies_index=None
-0000ac70: 0a20 2020 2020 2020 2073 656c 662e 6162  .        self.ab
-0000ac80: 756e 6461 6e63 653d 4e6f 6e65 0a20 2020  undance=None.   
-0000ac90: 2020 2020 2073 656c 662e 6476 3d4e 6f6e       self.dv=Non
-0000aca0: 650a 2020 2020 2020 2020 7365 6c66 2e6e  e.        self.n
-0000acb0: 6c65 7665 6c73 3d4e 6f6e 650a 2020 2020  levels=None.    
-0000acc0: 2020 2020 7365 6c66 2e6e 6c69 6e65 733d      self.nlines=
-0000acd0: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
-0000ace0: 662e 6c69 6e65 6461 7461 3d4e 6f6e 650a  f.linedata=None.
-0000acf0: 2020 2020 2020 2020 7365 6c66 2e6c 6576          self.lev
-0000ad00: 656c 6461 7461 3d4e 6f6e 650a 2020 2020  eldata=None.    
-0000ad10: 2020 2020 7365 6c66 2e63 6f6e 7657 6176      self.convWav
-0000ad20: 656c 656e 6774 683d 4e6f 6e65 0a20 2020  elength=None.   
-0000ad30: 2020 2020 2073 656c 662e 636f 6e76 4c54       self.convLT
-0000ad40: 4566 6c75 783d 4e6f 6e65 0a20 2020 2020  Eflux=None.     
-0000ad50: 2020 2073 656c 662e 636f 6e76 4e4c 5445     self.convNLTE
-0000ad60: 666c 7578 3d4e 6f6e 650a 2020 2020 2020  flux=None.      
-0000ad70: 2020 7365 6c66 2e63 6f6e 7654 7970 653d    self.convType=
-0000ad80: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
-0000ad90: 662e 636f 6e76 523d 4e6f 6e65 0a20 2020  f.convR=None.   
-0000ada0: 2020 2020 2073 656c 662e 6f76 6572 6c61       self.overla
-0000adb0: 704c 5445 3d4e 6f6e 650a 2020 2020 2020  pLTE=None.      
-0000adc0: 2020 7365 6c66 2e6f 7665 726c 6170 4e4c    self.overlapNL
-0000add0: 5445 3d4e 6f6e 650a 2020 2020 2020 2020  TE=None.        
-0000ade0: 7365 6c66 2e6f 7665 726c 6170 5461 754c  self.overlapTauL
-0000adf0: 5445 3d4e 6f6e 650a 2020 2020 2020 2020  TE=None.        
-0000ae00: 7365 6c66 2e6f 7665 726c 6170 5461 754e  self.overlapTauN
-0000ae10: 4c54 453d 4e6f 6e65 0a20 2020 2020 2020  LTE=None.       
-0000ae20: 2073 656c 662e 6f76 6572 6c61 7046 7265   self.overlapFre
-0000ae30: 713d 4e6f 6e65 0a20 2020 2020 2020 2073  q=None.        s
-0000ae40: 656c 662e 636f 6e76 4f76 6572 6c61 704c  elf.convOverlapL
-0000ae50: 5445 3d4e 6f6e 650a 2020 2020 2020 2020  TE=None.        
-0000ae60: 7365 6c66 2e63 6f6e 764f 7665 726c 6170  self.convOverlap
-0000ae70: 4e4c 5445 3d4e 6f6e 650a 2020 2020 2020  NLTE=None.      
-0000ae80: 2020 7365 6c66 2e63 6f6e 764f 7665 726c    self.convOverl
-0000ae90: 6170 4672 6571 3d4e 6f6e 650a 2020 2020  apFreq=None.    
-0000aea0: 2020 2020 7365 6c66 2e63 6f6e 764f 7665      self.convOve
-0000aeb0: 726c 6170 5761 7665 3d4e 6f6e 650a 2020  rlapWave=None.  
-0000aec0: 2020 2020 2020 7365 6c66 2e63 6f6e 764f        self.convO
-0000aed0: 7665 726c 6170 523d 3165 350a 2020 2020  verlapR=1e5.    
-0000aee0: 2020 2020 7365 6c66 2e6f 7665 726c 6170      self.overlap
-0000aef0: 523d 3165 350a 0a20 2020 2064 6566 205f  R=1e5..    def _
-0000af00: 5f73 7472 5f5f 2873 656c 6629 3a0a 2020  _str__(self):.  
-0000af10: 2020 2020 2020 6f75 7470 7574 3d22 496e        output="In
-0000af20: 666f 204d 6f64 656c 3a20 5c6e 220a 2020  fo Model: \n".  
-0000af30: 2020 2020 2020 6f75 7470 7574 2b3d 2773        output+='s
-0000af40: 7065 6369 6573 5f6e 756d 6265 723d 2027  pecies_number= '
-0000af50: 0a20 2020 2020 2020 206f 7574 7075 742b  .        output+
-0000af60: 3d73 7472 2873 656c 662e 7370 6563 6965  =str(self.specie
-0000af70: 735f 6e75 6d62 6572 292b 275c 6e5c 6e27  s_number)+'\n\n'
-0000af80: 0a20 2020 2020 2020 206f 7574 7075 742b  .        output+
-0000af90: 3d27 6d6f 6465 6c5f 6e75 6d62 6572 2020  ='model_number  
-0000afa0: 3d20 270a 2020 2020 2020 2020 6f75 7470  = '.        outp
-0000afb0: 7574 2b3d 7374 7228 7365 6c66 2e6d 6f64  ut+=str(self.mod
-0000afc0: 656c 5f6e 756d 6265 7229 2b27 5c6e 5c6e  el_number)+'\n\n
-0000afd0: 270a 2020 2020 2020 2020 6f75 7470 7574  '.        output
-0000afe0: 2b3d 274e 4820 2020 2020 2020 2020 2020  +='NH           
-0000aff0: 203d 2027 0a20 2020 2020 2020 206f 7574   = '.        out
-0000b000: 7075 742b 3d73 7472 2873 656c 662e 4e48  put+=str(self.NH
-0000b010: 292b 275c 6e5c 6e27 0a20 2020 2020 2020  )+'\n\n'.       
-0000b020: 206f 7574 7075 742b 3d27 6e43 6f6c 6c20   output+='nColl 
-0000b030: 2020 2020 2020 2020 3d20 270a 2020 2020          = '.    
-0000b040: 2020 2020 6f75 7470 7574 2b3d 7374 7228      output+=str(
-0000b050: 7365 6c66 2e6e 436f 6c6c 292b 275c 6e5c  self.nColl)+'\n\
-0000b060: 6e27 0a20 2020 2020 2020 206f 7574 7075  n'.        outpu
-0000b070: 742b 3d27 6e65 2020 2020 2020 2020 2020  t+='ne          
-0000b080: 2020 3d20 270a 2020 2020 2020 2020 6f75    = '.        ou
-0000b090: 7470 7574 2b3d 7374 7228 7365 6c66 2e6e  tput+=str(self.n
-0000b0a0: 6529 2b27 5c6e 5c6e 270a 2020 2020 2020  e)+'\n\n'.      
-0000b0b0: 2020 6f75 7470 7574 2b3d 276e 4865 2020    output+='nHe  
-0000b0c0: 2020 2020 2020 2020 203d 2027 0a20 2020           = '.   
-0000b0d0: 2020 2020 206f 7574 7075 742b 3d73 7472       output+=str
-0000b0e0: 2873 656c 662e 6e48 6529 2b27 5c6e 5c6e  (self.nHe)+'\n\n
-0000b0f0: 270a 2020 2020 2020 2020 6f75 7470 7574  '.        output
-0000b100: 2b3d 276e 4849 4920 2020 2020 2020 2020  +='nHII         
-0000b110: 203d 2027 0a20 2020 2020 2020 206f 7574   = '.        out
-0000b120: 7075 742b 3d73 7472 2873 656c 662e 6e48  put+=str(self.nH
-0000b130: 4949 292b 275c 6e5c 6e27 0a20 2020 2020  II)+'\n\n'.     
-0000b140: 2020 206f 7574 7075 742b 3d27 6e48 4920     output+='nHI 
-0000b150: 2020 2020 2020 2020 2020 3d20 270a 2020            = '.  
-0000b160: 2020 2020 2020 6f75 7470 7574 2b3d 7374        output+=st
-0000b170: 7228 7365 6c66 2e6e 4849 292b 275c 6e5c  r(self.nHI)+'\n\
-0000b180: 6e27 0a20 2020 2020 2020 206f 7574 7075  n'.        outpu
-0000b190: 742b 3d27 6e48 3220 2020 2020 2020 2020  t+='nH2         
-0000b1a0: 2020 3d20 270a 2020 2020 2020 2020 6f75    = '.        ou
-0000b1b0: 7470 7574 2b3d 7374 7228 7365 6c66 2e6e  tput+=str(self.n
-0000b1c0: 4832 292b 275c 6e5c 6e27 0a20 2020 2020  H2)+'\n\n'.     
-0000b1d0: 2020 206f 7574 7075 742b 3d27 6475 7374     output+='dust
-0000b1e0: 5f74 6f5f 6761 7320 2020 3d20 270a 2020  _to_gas   = '.  
-0000b1f0: 2020 2020 2020 6f75 7470 7574 2b3d 7374        output+=st
-0000b200: 7228 7365 6c66 2e64 7573 745f 746f 5f67  r(self.dust_to_g
-0000b210: 6173 292b 275c 6e5c 6e27 0a20 2020 2020  as)+'\n\n'.     
-0000b220: 2020 206f 7574 7075 742b 3d27 7674 7572     output+='vtur
-0000b230: 6220 2020 2020 2020 2020 3d20 270a 2020  b         = '.  
-0000b240: 2020 2020 2020 6f75 7470 7574 2b3d 7374        output+=st
-0000b250: 7228 7365 6c66 2e76 7475 7262 292b 275c  r(self.vturb)+'\
-0000b260: 6e5c 6e27 0a20 2020 2020 2020 206f 7574  n\n'.        out
-0000b270: 7075 742b 3d27 5467 2020 2020 2020 2020  put+='Tg        
-0000b280: 2020 2020 3d20 270a 2020 2020 2020 2020      = '.        
-0000b290: 6f75 7470 7574 2b3d 7374 7228 7365 6c66  output+=str(self
-0000b2a0: 2e54 6729 2b27 5c6e 5c6e 270a 2020 2020  .Tg)+'\n\n'.    
-0000b2b0: 2020 2020 6f75 7470 7574 2b3d 2754 6420      output+='Td 
-0000b2c0: 2020 2020 2020 2020 2020 203d 2027 0a20             = '. 
-0000b2d0: 2020 2020 2020 206f 7574 7075 742b 3d73         output+=s
-0000b2e0: 7472 2873 656c 662e 5464 292b 275c 6e5c  tr(self.Td)+'\n\
-0000b2f0: 6e27 0a20 2020 2020 2020 206f 7574 7075  n'.        outpu
-0000b300: 742b 3d27 7370 6563 6965 735f 6e61 6d65  t+='species_name
-0000b310: 2020 203d 2027 0a20 2020 2020 2020 206f     = '.        o
-0000b320: 7574 7075 742b 3d73 656c 662e 7370 6563  utput+=self.spec
-0000b330: 6965 735f 6e61 6d65 2b27 5c6e 5c6e 270a  ies_name+'\n\n'.
+00006e90: 6966 206e 6f74 206e 702e 6973 6e61 6e28  if not np.isnan(
+00006ea0: 6c6f 7765 7229 3a0a 2020 2020 2020 2020  lower):.        
+00006eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ec0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00006ed0: 6d6f 6465 6c73 5b69 5d2e 636f 6e76 523c  models[i].convR<
+00006ee0: 7570 7065 7220 616e 6420 7365 6c66 2e6d  upper and self.m
+00006ef0: 6f64 656c 735b 695d 2e63 6f6e 7652 3e6c  odels[i].convR>l
+00006f00: 6f77 6572 3a0a 2020 2020 2020 2020 2020  ower:.          
+00006f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f20: 2020 2020 2020 2020 2020 7265 745f 6461            ret_da
+00006f30: 7461 2e61 6464 5f6d 6f64 656c 2873 656c  ta.add_model(sel
+00006f40: 662e 6d6f 6465 6c73 5b69 5d29 0a20 2020  f.models[i]).   
+00006f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f60: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00006f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f80: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00006f90: 6620 7365 6c66 2e6d 6f64 656c 735b 695d  f self.models[i]
+00006fa0: 2e63 6f6e 7652 3d3d 7570 7065 723a 0a20  .convR==upper:. 
+00006fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006fd0: 2020 2072 6574 5f64 6174 612e 6164 645f     ret_data.add_
+00006fe0: 6d6f 6465 6c28 7365 6c66 2e6d 6f64 656c  model(self.model
+00006ff0: 735b 695d 290a 2020 2020 2020 2020 2020  s[i]).          
+00007000: 2020 2020 2020 2020 2020 656c 6966 2069            elif i
+00007010: 7369 6e73 7461 6e63 6528 6172 672e 7374  sinstance(arg.st
+00007020: 6f70 2c6c 6973 7429 3a0a 2020 2020 2020  op,list):.      
+00007030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007040: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+00007050: 2873 656c 662e 6e6d 6f64 656c 7329 3a0a  (self.nmodels):.
+00007060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007070: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00007080: 656c 662e 6d6f 6465 6c73 5b69 5d2e 636f  elf.models[i].co
+00007090: 6e76 5220 696e 2061 7267 2e73 746f 703a  nvR in arg.stop:
+000070a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000070b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070c0: 2072 6574 5f64 6174 612e 6164 645f 6d6f   ret_data.add_mo
+000070d0: 6465 6c28 7365 6c66 2e6d 6f64 656c 735b  del(self.models[
+000070e0: 695d 290a 2020 2020 2020 2020 2020 2020  i]).            
+000070f0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00007100: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00007110: 6973 6520 4b65 7945 7272 6f72 2827 556e  ise KeyError('Un
+00007120: 7265 636f 676e 6973 6564 2070 6172 616d  recognised param
+00007130: 6574 6572 2066 6f72 2073 6c69 6369 6e67  eter for slicing
+00007140: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
+00007150: 6e20 7265 745f 6461 7461 0a0a 2020 2020  n ret_data..    
+00007160: 6465 6620 636f 6e76 6f6c 7665 2873 656c  def convolve(sel
+00007170: 662c 6672 6571 5f62 696e 733d 4e6f 6e65  f,freq_bins=None
+00007180: 2c52 3d31 2c6c 616d 6264 615f 303d 312c  ,R=1,lambda_0=1,
+00007190: 6c61 6d62 6461 5f6e 3d31 2c76 723d 3133  lambda_n=1,vr=13
+000071a0: 3030 2c4e 4c54 453d 4661 6c73 652c 636f  00,NLTE=False,co
+000071b0: 6e76 5f74 7970 653d 312c 7665 7262 6f73  nv_type=1,verbos
+000071c0: 653d 5472 7565 2c6f 7665 726c 6170 3d46  e=True,overlap=F
+000071d0: 616c 7365 293a 0a20 2020 2020 2020 2066  alse):.        f
+000071e0: 6f72 2069 2c64 2069 6e20 656e 756d 6572  or i,d in enumer
+000071f0: 6174 6528 7365 6c66 2e6d 6f64 656c 7329  ate(self.models)
+00007200: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00007210: 2076 6572 626f 7365 3a20 7072 696e 7428   verbose: print(
+00007220: 275c 6e27 2c69 2b31 2c27 3b20 4d6f 6465  '\n',i+1,'; Mode
+00007230: 6c20 6e75 6d62 6572 2027 2c73 656c 662e  l number ',self.
+00007240: 6d6f 6465 6c73 5b69 5d2e 6d6f 6465 6c5f  models[i].model_
+00007250: 6e75 6d62 6572 2c27 3b20 5370 6563 6965  number,'; Specie
+00007260: 7320 6e75 6d62 6572 2027 2c73 656c 662e  s number ',self.
+00007270: 6d6f 6465 6c73 5b69 5d2e 7370 6563 6965  models[i].specie
+00007280: 735f 6e75 6d62 6572 290a 2020 2020 2020  s_number).      
+00007290: 2020 2020 2020 642e 636f 6e76 6f6c 7665        d.convolve
+000072a0: 2866 7265 715f 6269 6e73 3d66 7265 715f  (freq_bins=freq_
+000072b0: 6269 6e73 2c52 3d52 2c6c 616d 6264 615f  bins,R=R,lambda_
+000072c0: 303d 6c61 6d62 6461 5f30 2c6c 616d 6264  0=lambda_0,lambd
+000072d0: 615f 6e3d 6c61 6d62 6461 5f6e 2c76 723d  a_n=lambda_n,vr=
+000072e0: 7672 2c4e 4c54 453d 4e4c 5445 2c63 6f6e  vr,NLTE=NLTE,con
+000072f0: 765f 7479 7065 3d63 6f6e 765f 7479 7065  v_type=conv_type
+00007300: 2c6f 7665 726c 6170 3d6f 7665 726c 6170  ,overlap=overlap
+00007310: 290a 0a20 2020 2064 6566 2063 6f6e 766f  )..    def convo
+00007320: 6c76 655f 6f76 6572 6c61 7028 7365 6c66  lve_overlap(self
+00007330: 2c52 3d31 2c6c 616d 6264 615f 303d 312c  ,R=1,lambda_0=1,
+00007340: 6c61 6d62 6461 5f6e 3d31 2c76 6572 626f  lambda_n=1,verbo
+00007350: 7365 3d54 7275 6529 3a0a 2020 2020 2020  se=True):.      
+00007360: 2020 666f 7220 692c 6420 696e 2065 6e75    for i,d in enu
+00007370: 6d65 7261 7465 2873 656c 662e 6d6f 6465  merate(self.mode
+00007380: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
+00007390: 2069 6620 7665 7262 6f73 653a 2070 7269   if verbose: pri
+000073a0: 6e74 2827 5c6e 272c 692b 312c 273b 204d  nt('\n',i+1,'; M
+000073b0: 6f64 656c 206e 756d 6265 7220 272c 7365  odel number ',se
+000073c0: 6c66 2e6d 6f64 656c 735b 695d 2e6d 6f64  lf.models[i].mod
+000073d0: 656c 5f6e 756d 6265 7229 0a20 2020 2020  el_number).     
+000073e0: 2020 2020 2020 2064 2e63 6f6e 766f 6c76         d.convolv
+000073f0: 655f 6f76 6572 6c61 7028 523d 522c 6c61  e_overlap(R=R,la
+00007400: 6d62 6461 5f30 3d6c 616d 6264 615f 302c  mbda_0=lambda_0,
+00007410: 6c61 6d62 6461 5f6e 3d6c 616d 6264 615f  lambda_n=lambda_
+00007420: 6e29 0a0a 2020 2020 4070 726f 7065 7274  n)..    @propert
+00007430: 790a 2020 2020 6465 6620 6e6d 6f64 656c  y.    def nmodel
+00007440: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
+00007450: 2073 656c 662e 5f6e 6d6f 6465 6c73 3d6c   self._nmodels=l
+00007460: 656e 2873 656c 662e 6d6f 6465 6c73 290a  en(self.models).
+00007470: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00007480: 656c 662e 5f6e 6d6f 6465 6c73 0a0a 2020  elf._nmodels..  
+00007490: 2020 406e 6d6f 6465 6c73 2e73 6574 7465    @nmodels.sette
+000074a0: 720a 2020 2020 6465 6620 6e6d 6f64 656c  r.    def nmodel
+000074b0: 7328 7365 6c66 2c76 616c 7565 293a 0a20  s(self,value):. 
+000074c0: 2020 2020 2020 2073 656c 662e 5f6e 6d6f         self._nmo
+000074d0: 6465 6c73 3d76 616c 7565 0a0a 2020 2020  dels=value..    
+000074e0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+000074f0: 6620 7370 6563 6965 735f 6e75 6d62 6572  f species_number
+00007500: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00007510: 6966 2073 656c 662e 6e6d 6f64 656c 733e  if self.nmodels>
+00007520: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
+00007530: 656c 662e 5f73 7065 6369 6573 5f6e 756d  elf._species_num
+00007540: 6265 723d 5b5d 0a20 2020 2020 2020 2020  ber=[].         
+00007550: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+00007560: 6528 7365 6c66 2e6e 6d6f 6465 6c73 293a  e(self.nmodels):
+00007570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007580: 2073 656c 662e 5f73 7065 6369 6573 5f6e   self._species_n
+00007590: 756d 6265 722e 6170 7065 6e64 2873 656c  umber.append(sel
+000075a0: 662e 6d6f 6465 6c73 5b69 5d2e 7370 6563  f.models[i].spec
+000075b0: 6965 735f 6e75 6d62 6572 290a 2020 2020  ies_number).    
+000075c0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+000075d0: 2020 2020 2020 7365 6c66 2e5f 7370 6563        self._spec
+000075e0: 6965 735f 6e75 6d62 6572 3d73 656c 662e  ies_number=self.
+000075f0: 6d6f 6465 6c73 5b30 5d2e 7370 6563 6965  models[0].specie
+00007600: 735f 6e75 6d62 6572 0a20 2020 2020 2020  s_number.       
+00007610: 2072 6574 7572 6e20 7365 6c66 2e5f 7370   return self._sp
+00007620: 6563 6965 735f 6e75 6d62 6572 0a0a 2020  ecies_number..  
+00007630: 2020 4073 7065 6369 6573 5f6e 756d 6265    @species_numbe
+00007640: 722e 7365 7474 6572 0a20 2020 2064 6566  r.setter.    def
+00007650: 2073 7065 6369 6573 5f6e 756d 6265 7228   species_number(
+00007660: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
+00007670: 2020 2020 2073 656c 662e 5f73 7065 6369       self._speci
+00007680: 6573 5f6e 756d 6265 723d 7661 6c75 650a  es_number=value.
+00007690: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+000076a0: 2020 2064 6566 206d 6f64 656c 5f6e 756d     def model_num
+000076b0: 6265 7228 7365 6c66 293a 0a20 2020 2020  ber(self):.     
+000076c0: 2020 2069 6620 7365 6c66 2e6e 6d6f 6465     if self.nmode
+000076d0: 6c73 3e31 3a0a 2020 2020 2020 2020 2020  ls>1:.          
+000076e0: 2020 7365 6c66 2e5f 6d6f 6465 6c5f 6e75    self._model_nu
+000076f0: 6d62 6572 3d5b 5d0a 2020 2020 2020 2020  mber=[].        
+00007700: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00007710: 6765 2873 656c 662e 6e6d 6f64 656c 7329  ge(self.nmodels)
+00007720: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00007730: 2020 7365 6c66 2e5f 6d6f 6465 6c5f 6e75    self._model_nu
+00007740: 6d62 6572 2e61 7070 656e 6428 7365 6c66  mber.append(self
+00007750: 2e6d 6f64 656c 735b 695d 2e6d 6f64 656c  .models[i].model
+00007760: 5f6e 756d 6265 7229 0a20 2020 2020 2020  _number).       
+00007770: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00007780: 2020 2073 656c 662e 5f6d 6f64 656c 5f6e     self._model_n
+00007790: 756d 6265 723d 7365 6c66 2e6d 6f64 656c  umber=self.model
+000077a0: 735b 305d 2e6d 6f64 656c 5f6e 756d 6265  s[0].model_numbe
+000077b0: 720a 2020 2020 2020 2020 7265 7475 726e  r.        return
+000077c0: 2073 656c 662e 5f6d 6f64 656c 5f6e 756d   self._model_num
+000077d0: 6265 720a 0a20 2020 2040 6d6f 6465 6c5f  ber..    @model_
+000077e0: 6e75 6d62 6572 2e73 6574 7465 720a 2020  number.setter.  
+000077f0: 2020 6465 6620 6d6f 6465 6c5f 6e75 6d62    def model_numb
+00007800: 6572 2873 656c 662c 7661 6c75 6529 3a0a  er(self,value):.
+00007810: 2020 2020 2020 2020 7365 6c66 2e5f 6d6f          self._mo
+00007820: 6465 6c5f 6e75 6d62 6572 3d76 616c 7565  del_number=value
+00007830: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00007840: 2020 2020 6465 6620 4e48 2873 656c 6629      def NH(self)
+00007850: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
+00007860: 662e 6e6d 6f64 656c 733e 313a 0a20 2020  f.nmodels>1:.   
+00007870: 2020 2020 2020 2020 2073 656c 662e 5f4e           self._N
+00007880: 483d 5b5d 0a20 2020 2020 2020 2020 2020  H=[].           
+00007890: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+000078a0: 7365 6c66 2e6e 6d6f 6465 6c73 293a 0a20  self.nmodels):. 
+000078b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000078c0: 656c 662e 5f4e 482e 6170 7065 6e64 2873  elf._NH.append(s
+000078d0: 656c 662e 6d6f 6465 6c73 5b69 5d2e 4e48  elf.models[i].NH
+000078e0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+000078f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007900: 2e5f 4e48 3d73 656c 662e 6d6f 6465 6c73  ._NH=self.models
+00007910: 5b30 5d2e 4e48 0a20 2020 2020 2020 2072  [0].NH.        r
+00007920: 6574 7572 6e20 7365 6c66 2e5f 4e48 0a0a  eturn self._NH..
+00007930: 2020 2020 404e 482e 7365 7474 6572 0a20      @NH.setter. 
+00007940: 2020 2064 6566 204e 4828 7365 6c66 2c76     def NH(self,v
+00007950: 616c 7565 293a 0a20 2020 2020 2020 2073  alue):.        s
+00007960: 656c 662e 5f4e 483d 7661 6c75 650a 0a20  elf._NH=value.. 
+00007970: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00007980: 2064 6566 206e 436f 6c6c 2873 656c 6629   def nColl(self)
+00007990: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
+000079a0: 662e 6e6d 6f64 656c 733e 313a 0a20 2020  f.nmodels>1:.   
+000079b0: 2020 2020 2020 2020 2073 656c 662e 5f6e           self._n
+000079c0: 436f 6c6c 3d5b 5d0a 2020 2020 2020 2020  Coll=[].        
+000079d0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+000079e0: 6765 2873 656c 662e 6e6d 6f64 656c 7329  ge(self.nmodels)
+000079f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00007a00: 2020 7365 6c66 2e5f 6e43 6f6c 6c2e 6170    self._nColl.ap
+00007a10: 7065 6e64 2873 656c 662e 6d6f 6465 6c73  pend(self.models
+00007a20: 5b69 5d2e 6e43 6f6c 6c29 0a20 2020 2020  [i].nColl).     
+00007a30: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00007a40: 2020 2020 2073 656c 662e 5f6e 436f 6c6c       self._nColl
+00007a50: 3d73 656c 662e 6d6f 6465 6c73 5b30 5d2e  =self.models[0].
+00007a60: 6e43 6f6c 6c0a 2020 2020 2020 2020 7265  nColl.        re
+00007a70: 7475 726e 2073 656c 662e 5f6e 436f 6c6c  turn self._nColl
+00007a80: 0a0a 2020 2020 406e 436f 6c6c 2e73 6574  ..    @nColl.set
+00007a90: 7465 720a 2020 2020 6465 6620 6e43 6f6c  ter.    def nCol
+00007aa0: 6c28 7365 6c66 2c76 616c 7565 293a 0a20  l(self,value):. 
+00007ab0: 2020 2020 2020 2073 656c 662e 5f6e 436f         self._nCo
+00007ac0: 6c6c 3d76 616c 7565 0a0a 2020 2020 4070  ll=value..    @p
+00007ad0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00007ae0: 6e65 2873 656c 6629 3a0a 2020 2020 2020  ne(self):.      
+00007af0: 2020 6966 2073 656c 662e 6e6d 6f64 656c    if self.nmodel
+00007b00: 733e 313a 0a20 2020 2020 2020 2020 2020  s>1:.           
+00007b10: 2073 656c 662e 5f6e 653d 5b5d 0a20 2020   self._ne=[].   
+00007b20: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+00007b30: 6e20 7261 6e67 6528 7365 6c66 2e6e 6d6f  n range(self.nmo
+00007b40: 6465 6c73 293a 0a20 2020 2020 2020 2020  dels):.         
+00007b50: 2020 2020 2020 2073 656c 662e 5f6e 652e         self._ne.
+00007b60: 6170 7065 6e64 2873 656c 662e 6d6f 6465  append(self.mode
+00007b70: 6c73 5b69 5d2e 6e65 290a 2020 2020 2020  ls[i].ne).      
+00007b80: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00007b90: 2020 2020 7365 6c66 2e5f 6e65 3d73 656c      self._ne=sel
+00007ba0: 662e 6d6f 6465 6c73 5b30 5d2e 6e65 0a20  f.models[0].ne. 
+00007bb0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00007bc0: 6c66 2e5f 6e65 0a0a 2020 2020 406e 652e  lf._ne..    @ne.
+00007bd0: 7365 7474 6572 0a20 2020 2064 6566 206e  setter.    def n
+00007be0: 6528 7365 6c66 2c76 616c 7565 293a 0a20  e(self,value):. 
+00007bf0: 2020 2020 2020 2073 656c 662e 5f6e 653d         self._ne=
+00007c00: 7661 6c75 650a 0a20 2020 2040 7072 6f70  value..    @prop
+00007c10: 6572 7479 0a20 2020 2064 6566 206e 4865  erty.    def nHe
+00007c20: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00007c30: 6966 2073 656c 662e 6e6d 6f64 656c 733e  if self.nmodels>
+00007c40: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
+00007c50: 656c 662e 5f6e 4865 3d5b 5d0a 2020 2020  elf._nHe=[].    
+00007c60: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+00007c70: 2072 616e 6765 2873 656c 662e 6e6d 6f64   range(self.nmod
+00007c80: 656c 7329 3a0a 2020 2020 2020 2020 2020  els):.          
+00007c90: 2020 2020 2020 7365 6c66 2e5f 6e48 652e        self._nHe.
+00007ca0: 6170 7065 6e64 2873 656c 662e 6d6f 6465  append(self.mode
+00007cb0: 6c73 5b69 5d2e 6e48 6529 0a20 2020 2020  ls[i].nHe).     
+00007cc0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00007cd0: 2020 2020 2073 656c 662e 5f6e 4865 3d73       self._nHe=s
+00007ce0: 656c 662e 6d6f 6465 6c73 5b30 5d2e 6e48  elf.models[0].nH
+00007cf0: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
+00007d00: 2073 656c 662e 5f6e 4865 0a0a 2020 2020   self._nHe..    
+00007d10: 406e 4865 2e73 6574 7465 720a 2020 2020  @nHe.setter.    
+00007d20: 6465 6620 6e48 6528 7365 6c66 2c76 616c  def nHe(self,val
+00007d30: 7565 293a 0a20 2020 2020 2020 2073 656c  ue):.        sel
+00007d40: 662e 5f6e 4865 3d76 616c 7565 0a0a 2020  f._nHe=value..  
+00007d50: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+00007d60: 6465 6620 6e48 4949 2873 656c 6629 3a0a  def nHII(self):.
+00007d70: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00007d80: 6e6d 6f64 656c 733e 313a 0a20 2020 2020  nmodels>1:.     
+00007d90: 2020 2020 2020 2073 656c 662e 5f6e 4849         self._nHI
+00007da0: 493d 5b5d 0a20 2020 2020 2020 2020 2020  I=[].           
+00007db0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00007dc0: 7365 6c66 2e6e 6d6f 6465 6c73 293a 0a20  self.nmodels):. 
+00007dd0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00007de0: 656c 662e 5f6e 4849 492e 6170 7065 6e64  elf._nHII.append
+00007df0: 2873 656c 662e 6d6f 6465 6c73 5b69 5d2e  (self.models[i].
+00007e00: 6e48 4949 290a 2020 2020 2020 2020 656c  nHII).        el
+00007e10: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00007e20: 7365 6c66 2e5f 6e48 4949 3d73 656c 662e  self._nHII=self.
+00007e30: 6d6f 6465 6c73 5b30 5d2e 6e48 4949 0a20  models[0].nHII. 
+00007e40: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00007e50: 6c66 2e5f 6e48 4949 0a0a 2020 2020 406e  lf._nHII..    @n
+00007e60: 4849 492e 7365 7474 6572 0a20 2020 2064  HII.setter.    d
+00007e70: 6566 206e 4849 4928 7365 6c66 2c76 616c  ef nHII(self,val
+00007e80: 7565 293a 0a20 2020 2020 2020 2073 656c  ue):.        sel
+00007e90: 662e 5f6e 4849 493d 7661 6c75 650a 0a20  f._nHII=value.. 
+00007ea0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00007eb0: 2064 6566 206e 4849 2873 656c 6629 3a0a   def nHI(self):.
+00007ec0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00007ed0: 6e6d 6f64 656c 733e 313a 0a20 2020 2020  nmodels>1:.     
+00007ee0: 2020 2020 2020 2073 656c 662e 5f6e 4849         self._nHI
+00007ef0: 3d5b 5d0a 2020 2020 2020 2020 2020 2020  =[].            
+00007f00: 666f 7220 6920 696e 2072 616e 6765 2873  for i in range(s
+00007f10: 656c 662e 6e6d 6f64 656c 7329 3a0a 2020  elf.nmodels):.  
+00007f20: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00007f30: 6c66 2e5f 6e48 492e 6170 7065 6e64 2873  lf._nHI.append(s
+00007f40: 656c 662e 6d6f 6465 6c73 5b69 5d2e 6e48  elf.models[i].nH
+00007f50: 4929 0a20 2020 2020 2020 2065 6c73 653a  I).        else:
+00007f60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00007f70: 662e 5f6e 4849 3d73 656c 662e 6d6f 6465  f._nHI=self.mode
+00007f80: 6c73 5b30 5d2e 6e48 490a 2020 2020 2020  ls[0].nHI.      
+00007f90: 2020 7265 7475 726e 2073 656c 662e 5f6e    return self._n
+00007fa0: 4849 0a0a 2020 2020 406e 4849 2e73 6574  HI..    @nHI.set
+00007fb0: 7465 720a 2020 2020 6465 6620 6e48 4928  ter.    def nHI(
+00007fc0: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
+00007fd0: 2020 2020 2073 656c 662e 5f6e 4849 3d76       self._nHI=v
+00007fe0: 616c 7565 0a0a 2020 2020 4070 726f 7065  alue..    @prope
+00007ff0: 7274 790a 2020 2020 6465 6620 6e48 3228  rty.    def nH2(
+00008000: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
+00008010: 6620 7365 6c66 2e6e 6d6f 6465 6c73 3e31  f self.nmodels>1
+00008020: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00008030: 6c66 2e5f 6e48 323d 5b5d 0a20 2020 2020  lf._nH2=[].     
+00008040: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+00008050: 7261 6e67 6528 7365 6c66 2e6e 6d6f 6465  range(self.nmode
+00008060: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
+00008070: 2020 2020 2073 656c 662e 5f6e 4832 2e61       self._nH2.a
+00008080: 7070 656e 6428 7365 6c66 2e6d 6f64 656c  ppend(self.model
+00008090: 735b 695d 2e6e 4832 290a 2020 2020 2020  s[i].nH2).      
+000080a0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000080b0: 2020 2020 7365 6c66 2e5f 6e48 323d 7365      self._nH2=se
+000080c0: 6c66 2e6d 6f64 656c 735b 305d 2e6e 4832  lf.models[0].nH2
+000080d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000080e0: 7365 6c66 2e5f 6e48 320a 0a20 2020 2040  self._nH2..    @
+000080f0: 6e48 322e 7365 7474 6572 0a20 2020 2064  nH2.setter.    d
+00008100: 6566 206e 4832 2873 656c 662c 7661 6c75  ef nH2(self,valu
+00008110: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
+00008120: 2e5f 6e48 323d 7661 6c75 650a 0a20 2020  ._nH2=value..   
+00008130: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+00008140: 6566 2064 7573 745f 746f 5f67 6173 2873  ef dust_to_gas(s
+00008150: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
+00008160: 2073 656c 662e 6e6d 6f64 656c 733e 313a   self.nmodels>1:
+00008170: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00008180: 662e 5f64 7573 745f 746f 5f67 6173 3d5b  f._dust_to_gas=[
+00008190: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
+000081a0: 7220 6920 696e 2072 616e 6765 2873 656c  r i in range(sel
+000081b0: 662e 6e6d 6f64 656c 7329 3a0a 2020 2020  f.nmodels):.    
+000081c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000081d0: 2e5f 6475 7374 5f74 6f5f 6761 732e 6170  ._dust_to_gas.ap
+000081e0: 7065 6e64 2873 656c 662e 6d6f 6465 6c73  pend(self.models
+000081f0: 5b69 5d2e 6475 7374 5f74 6f5f 6761 7329  [i].dust_to_gas)
+00008200: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00008210: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00008220: 5f64 7573 745f 746f 5f67 6173 3d73 656c  _dust_to_gas=sel
+00008230: 662e 6d6f 6465 6c73 5b30 5d2e 6475 7374  f.models[0].dust
+00008240: 5f74 6f5f 6761 730a 2020 2020 2020 2020  _to_gas.        
+00008250: 7265 7475 726e 2073 656c 662e 5f64 7573  return self._dus
+00008260: 745f 746f 5f67 6173 0a0a 2020 2020 4064  t_to_gas..    @d
+00008270: 7573 745f 746f 5f67 6173 2e73 6574 7465  ust_to_gas.sette
+00008280: 720a 2020 2020 6465 6620 6475 7374 5f74  r.    def dust_t
+00008290: 6f5f 6761 7328 7365 6c66 2c76 616c 7565  o_gas(self,value
+000082a0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+000082b0: 5f64 7573 745f 746f 5f67 6173 3d76 616c  _dust_to_gas=val
+000082c0: 7565 0a0a 2020 2020 4070 726f 7065 7274  ue..    @propert
+000082d0: 790a 2020 2020 6465 6620 7674 7572 6228  y.    def vturb(
+000082e0: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
+000082f0: 6620 7365 6c66 2e6e 6d6f 6465 6c73 3e31  f self.nmodels>1
+00008300: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00008310: 6c66 2e5f 7674 7572 623d 5b5d 0a20 2020  lf._vturb=[].   
+00008320: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+00008330: 6e20 7261 6e67 6528 7365 6c66 2e6e 6d6f  n range(self.nmo
+00008340: 6465 6c73 293a 0a20 2020 2020 2020 2020  dels):.         
+00008350: 2020 2020 2020 2073 656c 662e 5f76 7475         self._vtu
+00008360: 7262 2e61 7070 656e 6428 7365 6c66 2e6d  rb.append(self.m
+00008370: 6f64 656c 735b 695d 2e76 7475 7262 290a  odels[i].vturb).
+00008380: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00008390: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+000083a0: 7674 7572 623d 7365 6c66 2e6d 6f64 656c  vturb=self.model
+000083b0: 735b 305d 2e76 7475 7262 0a20 2020 2020  s[0].vturb.     
+000083c0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+000083d0: 7674 7572 620a 0a20 2020 2040 7674 7572  vturb..    @vtur
+000083e0: 622e 7365 7474 6572 0a20 2020 2064 6566  b.setter.    def
+000083f0: 2076 7475 7262 2873 656c 662c 7661 6c75   vturb(self,valu
+00008400: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
+00008410: 2e5f 7674 7572 623d 7661 6c75 650a 0a20  ._vturb=value.. 
+00008420: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00008430: 2064 6566 2054 6728 7365 6c66 293a 0a20   def Tg(self):. 
+00008440: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
+00008450: 6d6f 6465 6c73 3e31 3a0a 2020 2020 2020  models>1:.      
+00008460: 2020 2020 2020 7365 6c66 2e5f 5467 3d5b        self._Tg=[
+00008470: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
+00008480: 7220 6920 696e 2072 616e 6765 2873 656c  r i in range(sel
+00008490: 662e 6e6d 6f64 656c 7329 3a0a 2020 2020  f.nmodels):.    
+000084a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000084b0: 2e5f 5467 2e61 7070 656e 6428 7365 6c66  ._Tg.append(self
+000084c0: 2e6d 6f64 656c 735b 695d 2e54 6729 0a20  .models[i].Tg). 
+000084d0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000084e0: 2020 2020 2020 2020 2073 656c 662e 5f54           self._T
+000084f0: 673d 7365 6c66 2e6d 6f64 656c 735b 305d  g=self.models[0]
+00008500: 2e54 670a 2020 2020 2020 2020 7265 7475  .Tg.        retu
+00008510: 726e 2073 656c 662e 5f54 670a 0a20 2020  rn self._Tg..   
+00008520: 2040 5467 2e73 6574 7465 720a 2020 2020   @Tg.setter.    
+00008530: 6465 6620 5467 2873 656c 662c 7661 6c75  def Tg(self,valu
+00008540: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
+00008550: 2e5f 5467 3d76 616c 7565 0a0a 2020 2020  ._Tg=value..    
+00008560: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+00008570: 6620 5464 2873 656c 6629 3a0a 2020 2020  f Td(self):.    
+00008580: 2020 2020 6966 2073 656c 662e 6e6d 6f64      if self.nmod
+00008590: 656c 733e 313a 0a20 2020 2020 2020 2020  els>1:.         
+000085a0: 2020 2073 656c 662e 5f54 643d 5b5d 0a20     self._Td=[]. 
+000085b0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+000085c0: 2069 6e20 7261 6e67 6528 7365 6c66 2e6e   in range(self.n
+000085d0: 6d6f 6465 6c73 293a 0a20 2020 2020 2020  models):.       
+000085e0: 2020 2020 2020 2020 2073 656c 662e 5f54           self._T
+000085f0: 642e 6170 7065 6e64 2873 656c 662e 6d6f  d.append(self.mo
+00008600: 6465 6c73 5b69 5d2e 5464 290a 2020 2020  dels[i].Td).    
+00008610: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00008620: 2020 2020 2020 7365 6c66 2e5f 5464 3d73        self._Td=s
+00008630: 656c 662e 6d6f 6465 6c73 5b30 5d2e 5464  elf.models[0].Td
+00008640: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00008650: 7365 6c66 2e5f 5464 0a0a 2020 2020 4054  self._Td..    @T
+00008660: 642e 7365 7474 6572 0a20 2020 2064 6566  d.setter.    def
+00008670: 2054 6428 7365 6c66 2c76 616c 7565 293a   Td(self,value):
+00008680: 0a20 2020 2020 2020 2073 656c 662e 5f54  .        self._T
+00008690: 643d 7661 6c75 650a 0a20 2020 2040 7072  d=value..    @pr
+000086a0: 6f70 6572 7479 0a20 2020 2064 6566 2073  operty.    def s
+000086b0: 7065 6369 6573 5f6e 616d 6528 7365 6c66  pecies_name(self
+000086c0: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
+000086d0: 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a 2020  lf.nmodels>1:.  
+000086e0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+000086f0: 7370 6563 6965 735f 6e61 6d65 3d5b 5d0a  species_name=[].
+00008700: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00008710: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
+00008720: 6e6d 6f64 656c 7329 3a0a 2020 2020 2020  nmodels):.      
+00008730: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00008740: 7370 6563 6965 735f 6e61 6d65 2e61 7070  species_name.app
+00008750: 656e 6428 7365 6c66 2e6d 6f64 656c 735b  end(self.models[
+00008760: 695d 2e73 7065 6369 6573 5f6e 616d 6529  i].species_name)
+00008770: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00008780: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00008790: 5f73 7065 6369 6573 5f6e 616d 653d 7365  _species_name=se
+000087a0: 6c66 2e6d 6f64 656c 735b 305d 2e73 7065  lf.models[0].spe
+000087b0: 6369 6573 5f6e 616d 650a 2020 2020 2020  cies_name.      
+000087c0: 2020 7265 7475 726e 2073 656c 662e 5f73    return self._s
+000087d0: 7065 6369 6573 5f6e 616d 650a 0a20 2020  pecies_name..   
+000087e0: 2040 7370 6563 6965 735f 6e61 6d65 2e73   @species_name.s
+000087f0: 6574 7465 720a 2020 2020 6465 6620 7370  etter.    def sp
+00008800: 6563 6965 735f 6e61 6d65 2873 656c 662c  ecies_name(self,
+00008810: 7661 6c75 6529 3a0a 2020 2020 2020 2020  value):.        
+00008820: 7365 6c66 2e5f 7370 6563 6965 735f 6e61  self._species_na
+00008830: 6d65 3d76 616c 7565 0a0a 2020 2020 4070  me=value..    @p
+00008840: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00008850: 7370 6563 6965 735f 696e 6465 7828 7365  species_index(se
+00008860: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
+00008870: 7365 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a  self.nmodels>1:.
+00008880: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00008890: 2e5f 7370 6563 6965 735f 696e 6465 783d  ._species_index=
+000088a0: 5b5d 0a20 2020 2020 2020 2020 2020 2066  [].            f
+000088b0: 6f72 2069 2069 6e20 7261 6e67 6528 7365  or i in range(se
+000088c0: 6c66 2e6e 6d6f 6465 6c73 293a 0a20 2020  lf.nmodels):.   
+000088d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000088e0: 662e 5f73 7065 6369 6573 5f69 6e64 6578  f._species_index
+000088f0: 2e61 7070 656e 6428 7365 6c66 2e6d 6f64  .append(self.mod
+00008900: 656c 735b 695d 2e73 7065 6369 6573 5f69  els[i].species_i
+00008910: 6e64 6578 290a 2020 2020 2020 2020 656c  ndex).        el
+00008920: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00008930: 7365 6c66 2e5f 7370 6563 6965 735f 696e  self._species_in
+00008940: 6465 783d 7365 6c66 2e6d 6f64 656c 735b  dex=self.models[
+00008950: 305d 2e73 7065 6369 6573 5f69 6e64 6578  0].species_index
+00008960: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00008970: 7365 6c66 2e5f 7370 6563 6965 735f 696e  self._species_in
+00008980: 6465 780a 0a20 2020 2040 7370 6563 6965  dex..    @specie
+00008990: 735f 696e 6465 782e 7365 7474 6572 0a20  s_index.setter. 
+000089a0: 2020 2064 6566 2073 7065 6369 6573 5f69     def species_i
+000089b0: 6e64 6578 2873 656c 662c 7661 6c75 6529  ndex(self,value)
+000089c0: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+000089d0: 7370 6563 6965 735f 696e 6465 783d 7661  species_index=va
+000089e0: 6c75 650a 0a20 2020 2040 7072 6f70 6572  lue..    @proper
+000089f0: 7479 0a20 2020 2064 6566 2061 6275 6e64  ty.    def abund
+00008a00: 616e 6365 2873 656c 6629 3a0a 2020 2020  ance(self):.    
+00008a10: 2020 2020 6966 2073 656c 662e 6e6d 6f64      if self.nmod
+00008a20: 656c 733e 313a 0a20 2020 2020 2020 2020  els>1:.         
+00008a30: 2020 2073 656c 662e 5f61 6275 6e64 616e     self._abundan
+00008a40: 6365 3d5b 5d0a 2020 2020 2020 2020 2020  ce=[].          
+00008a50: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+00008a60: 2873 656c 662e 6e6d 6f64 656c 7329 3a0a  (self.nmodels):.
+00008a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a80: 7365 6c66 2e5f 6162 756e 6461 6e63 652e  self._abundance.
+00008a90: 6170 7065 6e64 2873 656c 662e 6d6f 6465  append(self.mode
+00008aa0: 6c73 5b69 5d2e 6162 756e 6461 6e63 6529  ls[i].abundance)
+00008ab0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00008ac0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00008ad0: 5f61 6275 6e64 616e 6365 3d73 656c 662e  _abundance=self.
+00008ae0: 6d6f 6465 6c73 5b30 5d2e 6162 756e 6461  models[0].abunda
+00008af0: 6e63 650a 2020 2020 2020 2020 7265 7475  nce.        retu
+00008b00: 726e 2073 656c 662e 5f61 6275 6e64 616e  rn self._abundan
+00008b10: 6365 0a0a 2020 2020 4061 6275 6e64 616e  ce..    @abundan
+00008b20: 6365 2e73 6574 7465 720a 2020 2020 6465  ce.setter.    de
+00008b30: 6620 6162 756e 6461 6e63 6528 7365 6c66  f abundance(self
+00008b40: 2c76 616c 7565 293a 0a20 2020 2020 2020  ,value):.       
+00008b50: 2073 656c 662e 5f61 6275 6e64 616e 6365   self._abundance
+00008b60: 3d76 616c 7565 0a0a 2020 2020 4070 726f  =value..    @pro
+00008b70: 7065 7274 790a 2020 2020 6465 6620 6476  perty.    def dv
+00008b80: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00008b90: 6966 2073 656c 662e 6e6d 6f64 656c 733e  if self.nmodels>
+00008ba0: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
+00008bb0: 656c 662e 5f64 763d 5b5d 0a20 2020 2020  elf._dv=[].     
+00008bc0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+00008bd0: 7261 6e67 6528 7365 6c66 2e6e 6d6f 6465  range(self.nmode
+00008be0: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
+00008bf0: 2020 2020 2073 656c 662e 5f64 762e 6170       self._dv.ap
+00008c00: 7065 6e64 2873 656c 662e 6d6f 6465 6c73  pend(self.models
+00008c10: 5b69 5d2e 6476 290a 2020 2020 2020 2020  [i].dv).        
+00008c20: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00008c30: 2020 7365 6c66 2e5f 6476 3d73 656c 662e    self._dv=self.
+00008c40: 6d6f 6465 6c73 5b30 5d2e 6476 0a20 2020  models[0].dv.   
+00008c50: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00008c60: 2e5f 6476 0a0a 2020 2020 4064 762e 7365  ._dv..    @dv.se
+00008c70: 7474 6572 0a20 2020 2064 6566 2064 7628  tter.    def dv(
+00008c80: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
+00008c90: 2020 2020 2073 656c 662e 5f64 763d 7661       self._dv=va
+00008ca0: 6c75 650a 0a20 2020 2040 7072 6f70 6572  lue..    @proper
+00008cb0: 7479 0a20 2020 2064 6566 206e 6c65 7665  ty.    def nleve
+00008cc0: 6c73 2873 656c 6629 3a0a 2020 2020 2020  ls(self):.      
+00008cd0: 2020 6966 2073 656c 662e 6e6d 6f64 656c    if self.nmodel
+00008ce0: 733e 313a 0a20 2020 2020 2020 2020 2020  s>1:.           
+00008cf0: 2073 656c 662e 5f6e 6c65 7665 6c73 3d5b   self._nlevels=[
+00008d00: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
+00008d10: 7220 6920 696e 2072 616e 6765 2873 656c  r i in range(sel
+00008d20: 662e 6e6d 6f64 656c 7329 3a0a 2020 2020  f.nmodels):.    
+00008d30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00008d40: 2e5f 6e6c 6576 656c 732e 6170 7065 6e64  ._nlevels.append
+00008d50: 2873 656c 662e 6d6f 6465 6c73 5b69 5d2e  (self.models[i].
+00008d60: 6e6c 6576 656c 7329 0a20 2020 2020 2020  nlevels).       
+00008d70: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00008d80: 2020 2073 656c 662e 5f6e 6c65 7665 6c73     self._nlevels
+00008d90: 3d73 656c 662e 6d6f 6465 6c73 5b30 5d2e  =self.models[0].
+00008da0: 6e6c 6576 656c 730a 2020 2020 2020 2020  nlevels.        
+00008db0: 7265 7475 726e 2073 656c 662e 5f6e 6c65  return self._nle
+00008dc0: 7665 6c73 0a0a 2020 2020 406e 6c65 7665  vels..    @nleve
+00008dd0: 6c73 2e73 6574 7465 720a 2020 2020 6465  ls.setter.    de
+00008de0: 6620 6e6c 6576 656c 7328 7365 6c66 2c76  f nlevels(self,v
+00008df0: 616c 7565 293a 0a20 2020 2020 2020 2073  alue):.        s
+00008e00: 656c 662e 5f6e 6c65 7665 6c73 3d76 616c  elf._nlevels=val
+00008e10: 7565 0a0a 2020 2020 4070 726f 7065 7274  ue..    @propert
+00008e20: 790a 2020 2020 6465 6620 6e6c 696e 6573  y.    def nlines
+00008e30: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00008e40: 6966 2073 656c 662e 6e6d 6f64 656c 733e  if self.nmodels>
+00008e50: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
+00008e60: 656c 662e 5f6e 6c69 6e65 733d 5b5d 0a20  elf._nlines=[]. 
+00008e70: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+00008e80: 2069 6e20 7261 6e67 6528 7365 6c66 2e6e   in range(self.n
+00008e90: 6d6f 6465 6c73 293a 0a20 2020 2020 2020  models):.       
+00008ea0: 2020 2020 2020 2020 2073 656c 662e 5f6e           self._n
+00008eb0: 6c69 6e65 732e 6170 7065 6e64 2873 656c  lines.append(sel
+00008ec0: 662e 6d6f 6465 6c73 5b69 5d2e 6e6c 696e  f.models[i].nlin
+00008ed0: 6573 290a 2020 2020 2020 2020 656c 7365  es).        else
+00008ee0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00008ef0: 6c66 2e5f 6e6c 696e 6573 3d73 656c 662e  lf._nlines=self.
+00008f00: 6d6f 6465 6c73 5b30 5d2e 6e6c 696e 6573  models[0].nlines
+00008f10: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00008f20: 7365 6c66 2e5f 6e6c 696e 6573 0a0a 2020  self._nlines..  
+00008f30: 2020 406e 6c69 6e65 732e 7365 7474 6572    @nlines.setter
+00008f40: 0a20 2020 2064 6566 206e 6c69 6e65 7328  .    def nlines(
+00008f50: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
+00008f60: 2020 2020 2073 656c 662e 5f6e 6c69 6e65       self._nline
+00008f70: 733d 7661 6c75 650a 0a20 2020 2040 7072  s=value..    @pr
+00008f80: 6f70 6572 7479 0a20 2020 2064 6566 206c  operty.    def l
+00008f90: 696e 6564 6174 6128 7365 6c66 293a 0a20  inedata(self):. 
+00008fa0: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
+00008fb0: 6d6f 6465 6c73 3e31 3a0a 2020 2020 2020  models>1:.      
+00008fc0: 2020 2020 2020 7365 6c66 2e5f 6c69 6e65        self._line
+00008fd0: 6461 7461 3d5b 5d0a 2020 2020 2020 2020  data=[].        
+00008fe0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00008ff0: 6765 2873 656c 662e 6e6d 6f64 656c 7329  ge(self.nmodels)
+00009000: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00009010: 2020 7365 6c66 2e5f 6c69 6e65 6461 7461    self._linedata
+00009020: 2e61 7070 656e 6428 7365 6c66 2e6d 6f64  .append(self.mod
+00009030: 656c 735b 695d 2e6c 696e 6564 6174 6129  els[i].linedata)
+00009040: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00009050: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00009060: 5f6c 696e 6564 6174 613d 7365 6c66 2e6d  _linedata=self.m
+00009070: 6f64 656c 735b 305d 2e6c 696e 6564 6174  odels[0].linedat
+00009080: 610a 2020 2020 2020 2020 7265 7475 726e  a.        return
+00009090: 2073 656c 662e 5f6c 696e 6564 6174 610a   self._linedata.
+000090a0: 0a20 2020 2040 6c69 6e65 6461 7461 2e73  .    @linedata.s
+000090b0: 6574 7465 720a 2020 2020 6465 6620 6c69  etter.    def li
+000090c0: 6e65 6461 7461 2873 656c 662c 7661 6c75  nedata(self,valu
+000090d0: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
+000090e0: 2e5f 6c69 6e65 6461 7461 3d76 616c 7565  ._linedata=value
+000090f0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00009100: 2020 2020 6465 6620 6c65 7665 6c64 6174      def leveldat
+00009110: 6128 7365 6c66 293a 0a20 2020 2020 2020  a(self):.       
+00009120: 2069 6620 7365 6c66 2e6e 6d6f 6465 6c73   if self.nmodels
+00009130: 3e31 3a0a 2020 2020 2020 2020 2020 2020  >1:.            
+00009140: 7365 6c66 2e5f 6c65 7665 6c64 6174 613d  self._leveldata=
+00009150: 5b5d 0a20 2020 2020 2020 2020 2020 2066  [].            f
+00009160: 6f72 2069 2069 6e20 7261 6e67 6528 7365  or i in range(se
+00009170: 6c66 2e6e 6d6f 6465 6c73 293a 0a20 2020  lf.nmodels):.   
+00009180: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00009190: 662e 5f6c 6576 656c 6461 7461 2e61 7070  f._leveldata.app
+000091a0: 656e 6428 7365 6c66 2e6d 6f64 656c 735b  end(self.models[
+000091b0: 695d 2e6c 6576 656c 6461 7461 290a 2020  i].leveldata).  
+000091c0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+000091d0: 2020 2020 2020 2020 7365 6c66 2e5f 6c65          self._le
+000091e0: 7665 6c64 6174 613d 7365 6c66 2e6d 6f64  veldata=self.mod
+000091f0: 656c 735b 305d 2e6c 6576 656c 6461 7461  els[0].leveldata
+00009200: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00009210: 7365 6c66 2e5f 6c65 7665 6c64 6174 610a  self._leveldata.
+00009220: 0a20 2020 2040 6c65 7665 6c64 6174 612e  .    @leveldata.
+00009230: 7365 7474 6572 0a20 2020 2064 6566 206c  setter.    def l
+00009240: 6576 656c 6461 7461 2873 656c 662c 7661  eveldata(self,va
+00009250: 6c75 6529 3a0a 2020 2020 2020 2020 7365  lue):.        se
+00009260: 6c66 2e5f 6c65 7665 6c64 6174 613d 7661  lf._leveldata=va
+00009270: 6c75 650a 0a20 2020 2040 7072 6f70 6572  lue..    @proper
+00009280: 7479 0a20 2020 2064 6566 2063 6f6e 7657  ty.    def convW
+00009290: 6176 656c 656e 6774 6828 7365 6c66 293a  avelength(self):
+000092a0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000092b0: 2e6e 6d6f 6465 6c73 3e31 3a0a 2020 2020  .nmodels>1:.    
+000092c0: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
+000092d0: 6e76 5761 7665 6c65 6e67 7468 3d5b 5d0a  nvWavelength=[].
+000092e0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000092f0: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
+00009300: 6e6d 6f64 656c 7329 3a0a 2020 2020 2020  nmodels):.      
+00009310: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00009320: 636f 6e76 5761 7665 6c65 6e67 7468 2e61  convWavelength.a
+00009330: 7070 656e 6428 7365 6c66 2e6d 6f64 656c  ppend(self.model
+00009340: 735b 695d 2e63 6f6e 7657 6176 656c 656e  s[i].convWavelen
+00009350: 6774 6829 0a20 2020 2020 2020 2065 6c73  gth).        els
+00009360: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00009370: 656c 662e 5f63 6f6e 7657 6176 656c 656e  elf._convWavelen
+00009380: 6774 683d 7365 6c66 2e6d 6f64 656c 735b  gth=self.models[
+00009390: 305d 2e63 6f6e 7657 6176 656c 656e 6774  0].convWavelengt
+000093a0: 680a 2020 2020 2020 2020 7265 7475 726e  h.        return
+000093b0: 2073 656c 662e 5f63 6f6e 7657 6176 656c   self._convWavel
+000093c0: 656e 6774 680a 0a20 2020 2040 636f 6e76  ength..    @conv
+000093d0: 5761 7665 6c65 6e67 7468 2e73 6574 7465  Wavelength.sette
+000093e0: 720a 2020 2020 6465 6620 636f 6e76 5761  r.    def convWa
+000093f0: 7665 6c65 6e67 7468 2873 656c 662c 7661  velength(self,va
+00009400: 6c75 6529 3a0a 2020 2020 2020 2020 7365  lue):.        se
+00009410: 6c66 2e5f 636f 6e76 5761 7665 6c65 6e67  lf._convWaveleng
+00009420: 7468 3d76 616c 7565 0a0a 2020 2020 4070  th=value..    @p
+00009430: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00009440: 636f 6e76 4c54 4566 6c75 7828 7365 6c66  convLTEflux(self
+00009450: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
+00009460: 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a 2020  lf.nmodels>1:.  
+00009470: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00009480: 636f 6e76 4c54 4566 6c75 783d 5b5d 0a20  convLTEflux=[]. 
+00009490: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+000094a0: 2069 6e20 7261 6e67 6528 7365 6c66 2e6e   in range(self.n
+000094b0: 6d6f 6465 6c73 293a 0a20 2020 2020 2020  models):.       
+000094c0: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
+000094d0: 6f6e 764c 5445 666c 7578 2e61 7070 656e  onvLTEflux.appen
+000094e0: 6428 7365 6c66 2e6d 6f64 656c 735b 695d  d(self.models[i]
+000094f0: 2e63 6f6e 764c 5445 666c 7578 290a 2020  .convLTEflux).  
+00009500: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00009510: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
+00009520: 6e76 4c54 4566 6c75 783d 7365 6c66 2e6d  nvLTEflux=self.m
+00009530: 6f64 656c 735b 305d 2e63 6f6e 764c 5445  odels[0].convLTE
+00009540: 666c 7578 0a20 2020 2020 2020 2072 6574  flux.        ret
+00009550: 7572 6e20 7365 6c66 2e5f 636f 6e76 4c54  urn self._convLT
+00009560: 4566 6c75 780a 0a20 2020 2040 636f 6e76  Eflux..    @conv
+00009570: 4c54 4566 6c75 782e 7365 7474 6572 0a20  LTEflux.setter. 
+00009580: 2020 2064 6566 2063 6f6e 764c 5445 666c     def convLTEfl
+00009590: 7578 2873 656c 662c 7661 6c75 6529 3a0a  ux(self,value):.
+000095a0: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
+000095b0: 6e76 4c54 4566 6c75 783d 7661 6c75 650a  nvLTEflux=value.
+000095c0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+000095d0: 2020 2064 6566 2063 6f6e 764e 4c54 4566     def convNLTEf
+000095e0: 6c75 7828 7365 6c66 293a 0a20 2020 2020  lux(self):.     
+000095f0: 2020 2069 6620 7365 6c66 2e6e 6d6f 6465     if self.nmode
+00009600: 6c73 3e31 3a0a 2020 2020 2020 2020 2020  ls>1:.          
+00009610: 2020 7365 6c66 2e5f 636f 6e76 4e4c 5445    self._convNLTE
+00009620: 666c 7578 3d5b 5d0a 2020 2020 2020 2020  flux=[].        
+00009630: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00009640: 6765 2873 656c 662e 6e6d 6f64 656c 7329  ge(self.nmodels)
+00009650: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00009660: 2020 7365 6c66 2e5f 636f 6e76 4e4c 5445    self._convNLTE
+00009670: 666c 7578 2e61 7070 656e 6428 7365 6c66  flux.append(self
+00009680: 2e6d 6f64 656c 735b 695d 2e63 6f6e 764e  .models[i].convN
+00009690: 4c54 4566 6c75 7829 0a20 2020 2020 2020  LTEflux).       
+000096a0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000096b0: 2020 2073 656c 662e 5f63 6f6e 764e 4c54     self._convNLT
+000096c0: 4566 6c75 783d 7365 6c66 2e6d 6f64 656c  Eflux=self.model
+000096d0: 735b 305d 2e63 6f6e 764e 4c54 4566 6c75  s[0].convNLTEflu
+000096e0: 780a 2020 2020 2020 2020 7265 7475 726e  x.        return
+000096f0: 2073 656c 662e 5f63 6f6e 764e 4c54 4566   self._convNLTEf
+00009700: 6c75 780a 0a20 2020 2040 636f 6e76 4e4c  lux..    @convNL
+00009710: 5445 666c 7578 2e73 6574 7465 720a 2020  TEflux.setter.  
+00009720: 2020 6465 6620 636f 6e76 4e4c 5445 666c    def convNLTEfl
+00009730: 7578 2873 656c 662c 7661 6c75 6529 3a0a  ux(self,value):.
+00009740: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
+00009750: 6e76 4e4c 5445 666c 7578 3d76 616c 7565  nvNLTEflux=value
+00009760: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00009770: 2020 2020 6465 6620 636f 6e76 5479 7065      def convType
+00009780: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00009790: 6966 2073 656c 662e 6e6d 6f64 656c 733e  if self.nmodels>
+000097a0: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
+000097b0: 656c 662e 5f63 6f6e 7654 7970 653d 5b5d  elf._convType=[]
+000097c0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+000097d0: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
+000097e0: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
+000097f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00009800: 5f63 6f6e 7654 7970 652e 6170 7065 6e64  _convType.append
+00009810: 2873 656c 662e 6d6f 6465 6c73 5b69 5d2e  (self.models[i].
+00009820: 636f 6e76 5479 7065 290a 2020 2020 2020  convType).      
+00009830: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00009840: 2020 2020 7365 6c66 2e5f 636f 6e76 5479      self._convTy
+00009850: 7065 3d73 656c 662e 6d6f 6465 6c73 5b30  pe=self.models[0
+00009860: 5d2e 636f 6e76 5479 7065 0a20 2020 2020  ].convType.     
+00009870: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00009880: 636f 6e76 5479 7065 0a0a 2020 2020 4063  convType..    @c
+00009890: 6f6e 7654 7970 652e 7365 7474 6572 0a20  onvType.setter. 
+000098a0: 2020 2064 6566 2063 6f6e 7654 7970 6528     def convType(
+000098b0: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
+000098c0: 2020 2020 2073 656c 662e 5f63 6f6e 7654       self._convT
+000098d0: 7970 653d 7661 6c75 650a 0a20 2020 2040  ype=value..    @
+000098e0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+000098f0: 2063 6f6e 7652 2873 656c 6629 3a0a 2020   convR(self):.  
+00009900: 2020 2020 2020 6966 2073 656c 662e 6e6d        if self.nm
+00009910: 6f64 656c 733e 313a 0a20 2020 2020 2020  odels>1:.       
+00009920: 2020 2020 2073 656c 662e 5f63 6f6e 7652       self._convR
+00009930: 3d5b 5d0a 2020 2020 2020 2020 2020 2020  =[].            
+00009940: 666f 7220 6920 696e 2072 616e 6765 2873  for i in range(s
+00009950: 656c 662e 6e6d 6f64 656c 7329 3a0a 2020  elf.nmodels):.  
+00009960: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00009970: 6c66 2e5f 636f 6e76 522e 6170 7065 6e64  lf._convR.append
+00009980: 2873 656c 662e 6d6f 6465 6c73 5b69 5d2e  (self.models[i].
+00009990: 636f 6e76 5229 0a20 2020 2020 2020 2065  convR).        e
+000099a0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+000099b0: 2073 656c 662e 5f63 6f6e 7652 3d73 656c   self._convR=sel
+000099c0: 662e 6d6f 6465 6c73 5b30 5d2e 636f 6e76  f.models[0].conv
+000099d0: 520a 2020 2020 2020 2020 7265 7475 726e  R.        return
+000099e0: 2073 656c 662e 5f63 6f6e 7652 0a0a 2020   self._convR..  
+000099f0: 2020 4063 6f6e 7652 2e73 6574 7465 720a    @convR.setter.
+00009a00: 2020 2020 6465 6620 636f 6e76 5228 7365      def convR(se
+00009a10: 6c66 2c76 616c 7565 293a 0a20 2020 2020  lf,value):.     
+00009a20: 2020 2073 656c 662e 5f63 6f6e 7652 3d76     self._convR=v
+00009a30: 616c 7565 0a0a 2020 2020 4070 726f 7065  alue..    @prope
+00009a40: 7274 790a 2020 2020 6465 6620 636f 6e76  rty.    def conv
+00009a50: 4f76 6572 6c61 7046 7265 7128 7365 6c66  OverlapFreq(self
+00009a60: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
+00009a70: 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a 2020  lf.nmodels>1:.  
+00009a80: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00009a90: 636f 6e76 4f76 6572 6c61 7046 7265 713d  convOverlapFreq=
+00009aa0: 5b5d 0a20 2020 2020 2020 2020 2020 2066  [].            f
+00009ab0: 6f72 2069 2069 6e20 7261 6e67 6528 7365  or i in range(se
+00009ac0: 6c66 2e6e 6d6f 6465 6c73 293a 0a20 2020  lf.nmodels):.   
+00009ad0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00009ae0: 662e 5f63 6f6e 764f 7665 726c 6170 4672  f._convOverlapFr
+00009af0: 6571 2e61 7070 656e 6428 7365 6c66 2e6d  eq.append(self.m
+00009b00: 6f64 656c 735b 695d 2e63 6f6e 764f 7665  odels[i].convOve
+00009b10: 726c 6170 4672 6571 290a 2020 2020 2020  rlapFreq).      
+00009b20: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00009b30: 2020 2020 7365 6c66 2e5f 636f 6e76 4f76      self._convOv
+00009b40: 6572 6c61 7046 7265 713d 7365 6c66 2e6d  erlapFreq=self.m
+00009b50: 6f64 656c 735b 305d 2e63 6f6e 764f 7665  odels[0].convOve
+00009b60: 726c 6170 4672 6571 0a20 2020 2020 2020  rlapFreq.       
+00009b70: 2072 6574 7572 6e20 7365 6c66 2e5f 636f   return self._co
+00009b80: 6e76 4f76 6572 6c61 7046 7265 710a 0a20  nvOverlapFreq.. 
+00009b90: 2020 2040 636f 6e76 4f76 6572 6c61 7046     @convOverlapF
+00009ba0: 7265 712e 7365 7474 6572 0a20 2020 2064  req.setter.    d
+00009bb0: 6566 2063 6f6e 764f 7665 726c 6170 4672  ef convOverlapFr
+00009bc0: 6571 2873 656c 662c 7661 6c75 6529 3a0a  eq(self,value):.
+00009bd0: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
+00009be0: 6e76 4f76 6572 6c61 7046 7265 713d 7661  nvOverlapFreq=va
+00009bf0: 6c75 650a 0a20 2020 2040 7072 6f70 6572  lue..    @proper
+00009c00: 7479 0a20 2020 2064 6566 2063 6f6e 764f  ty.    def convO
+00009c10: 7665 726c 6170 5761 7665 2873 656c 6629  verlapWave(self)
+00009c20: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
+00009c30: 662e 6e6d 6f64 656c 733e 313a 0a20 2020  f.nmodels>1:.   
+00009c40: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
+00009c50: 6f6e 764f 7665 726c 6170 5761 7665 3d5b  onvOverlapWave=[
+00009c60: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
+00009c70: 7220 6920 696e 2072 616e 6765 2873 656c  r i in range(sel
+00009c80: 662e 6e6d 6f64 656c 7329 3a0a 2020 2020  f.nmodels):.    
+00009c90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00009ca0: 2e5f 636f 6e76 4f76 6572 6c61 7057 6176  ._convOverlapWav
+00009cb0: 652e 6170 7065 6e64 2873 656c 662e 6d6f  e.append(self.mo
+00009cc0: 6465 6c73 5b69 5d2e 636f 6e76 4f76 6572  dels[i].convOver
+00009cd0: 6c61 7057 6176 6529 0a20 2020 2020 2020  lapWave).       
+00009ce0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00009cf0: 2020 2073 656c 662e 5f63 6f6e 764f 7665     self._convOve
+00009d00: 726c 6170 5761 7665 3d73 656c 662e 6d6f  rlapWave=self.mo
+00009d10: 6465 6c73 5b30 5d2e 636f 6e76 4f76 6572  dels[0].convOver
+00009d20: 6c61 7057 6176 650a 2020 2020 2020 2020  lapWave.        
+00009d30: 7265 7475 726e 2073 656c 662e 5f63 6f6e  return self._con
+00009d40: 764f 7665 726c 6170 5761 7665 0a0a 2020  vOverlapWave..  
+00009d50: 2020 4063 6f6e 764f 7665 726c 6170 5761    @convOverlapWa
+00009d60: 7665 2e73 6574 7465 720a 2020 2020 6465  ve.setter.    de
+00009d70: 6620 636f 6e76 4f76 6572 6c61 7057 6176  f convOverlapWav
+00009d80: 6528 7365 6c66 2c76 616c 7565 293a 0a20  e(self,value):. 
+00009d90: 2020 2020 2020 2073 656c 662e 5f63 6f6e         self._con
+00009da0: 764f 7665 726c 6170 5761 7665 3d76 616c  vOverlapWave=val
+00009db0: 7565 0a0a 2020 2020 4070 726f 7065 7274  ue..    @propert
+00009dc0: 790a 2020 2020 6465 6620 6f76 6572 6c61  y.    def overla
+00009dd0: 7046 7265 7128 7365 6c66 293a 0a20 2020  pFreq(self):.   
+00009de0: 2020 2020 2069 6620 7365 6c66 2e6e 6d6f       if self.nmo
+00009df0: 6465 6c73 3e31 3a0a 2020 2020 2020 2020  dels>1:.        
+00009e00: 2020 2020 7365 6c66 2e5f 6f76 6572 6c61      self._overla
+00009e10: 7046 7265 713d 5b5d 0a20 2020 2020 2020  pFreq=[].       
+00009e20: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+00009e30: 6e67 6528 7365 6c66 2e6e 6d6f 6465 6c73  nge(self.nmodels
+00009e40: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00009e50: 2020 2073 656c 662e 5f6f 7665 726c 6170     self._overlap
+00009e60: 4672 6571 2e61 7070 656e 6428 7365 6c66  Freq.append(self
+00009e70: 2e6d 6f64 656c 735b 695d 2e6f 7665 726c  .models[i].overl
+00009e80: 6170 4672 6571 290a 2020 2020 2020 2020  apFreq).        
+00009e90: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00009ea0: 2020 7365 6c66 2e5f 6f76 6572 6c61 7046    self._overlapF
+00009eb0: 7265 713d 7365 6c66 2e6d 6f64 656c 735b  req=self.models[
+00009ec0: 305d 2e6f 7665 726c 6170 4672 6571 0a20  0].overlapFreq. 
+00009ed0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00009ee0: 6c66 2e5f 6f76 6572 6c61 7046 7265 710a  lf._overlapFreq.
+00009ef0: 0a20 2020 2040 6f76 6572 6c61 7046 7265  .    @overlapFre
+00009f00: 712e 7365 7474 6572 0a20 2020 2064 6566  q.setter.    def
+00009f10: 206f 7665 726c 6170 4672 6571 2873 656c   overlapFreq(sel
+00009f20: 662c 7661 6c75 6529 3a0a 2020 2020 2020  f,value):.      
+00009f30: 2020 7365 6c66 2e5f 6f76 6572 6c61 7046    self._overlapF
+00009f40: 7265 713d 7661 6c75 650a 0a20 2020 2040  req=value..    @
+00009f50: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+00009f60: 2063 6f6e 764f 7665 726c 6170 4c54 4528   convOverlapLTE(
+00009f70: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
+00009f80: 6620 7365 6c66 2e6e 6d6f 6465 6c73 3e31  f self.nmodels>1
+00009f90: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00009fa0: 6c66 2e5f 636f 6e76 4f76 6572 6c61 704c  lf._convOverlapL
+00009fb0: 5445 3d5b 5d0a 2020 2020 2020 2020 2020  TE=[].          
+00009fc0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+00009fd0: 2873 656c 662e 6e6d 6f64 656c 7329 3a0a  (self.nmodels):.
+00009fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ff0: 7365 6c66 2e5f 636f 6e76 4f76 6572 6c61  self._convOverla
+0000a000: 704c 5445 2e61 7070 656e 6428 7365 6c66  pLTE.append(self
+0000a010: 2e6d 6f64 656c 735b 695d 2e63 6f6e 764f  .models[i].convO
+0000a020: 7665 726c 6170 4c54 4529 0a20 2020 2020  verlapLTE).     
+0000a030: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000a040: 2020 2020 2073 656c 662e 5f63 6f6e 764f       self._convO
+0000a050: 7665 726c 6170 4c54 453d 7365 6c66 2e6d  verlapLTE=self.m
+0000a060: 6f64 656c 735b 305d 2e63 6f6e 764f 7665  odels[0].convOve
+0000a070: 726c 6170 4c54 450a 2020 2020 2020 2020  rlapLTE.        
+0000a080: 7265 7475 726e 2073 656c 662e 5f63 6f6e  return self._con
+0000a090: 764f 7665 726c 6170 4c54 450a 0a20 2020  vOverlapLTE..   
+0000a0a0: 2040 636f 6e76 4f76 6572 6c61 704c 5445   @convOverlapLTE
+0000a0b0: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
+0000a0c0: 636f 6e76 4f76 6572 6c61 704c 5445 2873  convOverlapLTE(s
+0000a0d0: 656c 662c 7661 6c75 6529 3a0a 2020 2020  elf,value):.    
+0000a0e0: 2020 2020 7365 6c66 2e5f 636f 6e76 4f76      self._convOv
+0000a0f0: 6572 6c61 704c 5445 3d76 616c 7565 0a0a  erlapLTE=value..
+0000a100: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+0000a110: 2020 6465 6620 636f 6e76 4f76 6572 6c61    def convOverla
+0000a120: 704e 4c54 4528 7365 6c66 293a 0a20 2020  pNLTE(self):.   
+0000a130: 2020 2020 2069 6620 7365 6c66 2e6e 6d6f       if self.nmo
+0000a140: 6465 6c73 3e31 3a0a 2020 2020 2020 2020  dels>1:.        
+0000a150: 2020 2020 7365 6c66 2e5f 636f 6e76 4f76      self._convOv
+0000a160: 6572 6c61 704e 4c54 453d 5b5d 0a20 2020  erlapNLTE=[].   
+0000a170: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+0000a180: 6e20 7261 6e67 6528 7365 6c66 2e6e 6d6f  n range(self.nmo
+0000a190: 6465 6c73 293a 0a20 2020 2020 2020 2020  dels):.         
+0000a1a0: 2020 2020 2020 2073 656c 662e 5f63 6f6e         self._con
+0000a1b0: 764f 7665 726c 6170 4e4c 5445 2e61 7070  vOverlapNLTE.app
+0000a1c0: 656e 6428 7365 6c66 2e6d 6f64 656c 735b  end(self.models[
+0000a1d0: 695d 2e63 6f6e 764f 7665 726c 6170 4e4c  i].convOverlapNL
+0000a1e0: 5445 290a 2020 2020 2020 2020 656c 7365  TE).        else
+0000a1f0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000a200: 6c66 2e5f 636f 6e76 4f76 6572 6c61 704e  lf._convOverlapN
+0000a210: 4c54 453d 7365 6c66 2e6d 6f64 656c 735b  LTE=self.models[
+0000a220: 305d 2e63 6f6e 764f 7665 726c 6170 4e4c  0].convOverlapNL
+0000a230: 5445 0a20 2020 2020 2020 2072 6574 7572  TE.        retur
+0000a240: 6e20 7365 6c66 2e5f 636f 6e76 4f76 6572  n self._convOver
+0000a250: 6c61 704e 4c54 450a 0a20 2020 2040 636f  lapNLTE..    @co
+0000a260: 6e76 4f76 6572 6c61 704e 4c54 452e 7365  nvOverlapNLTE.se
+0000a270: 7474 6572 0a20 2020 2064 6566 2063 6f6e  tter.    def con
+0000a280: 764f 7665 726c 6170 4e4c 5445 2873 656c  vOverlapNLTE(sel
+0000a290: 662c 7661 6c75 6529 3a0a 2020 2020 2020  f,value):.      
+0000a2a0: 2020 7365 6c66 2e5f 636f 6e76 4f76 6572    self._convOver
+0000a2b0: 6c61 704e 4c54 453d 7661 6c75 650a 0a20  lapNLTE=value.. 
+0000a2c0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+0000a2d0: 2064 6566 206f 7665 726c 6170 4c54 4528   def overlapLTE(
+0000a2e0: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
+0000a2f0: 6620 7365 6c66 2e6e 6d6f 6465 6c73 3e31  f self.nmodels>1
+0000a300: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000a310: 6c66 2e5f 6f76 6572 6c61 704c 5445 3d5b  lf._overlapLTE=[
+0000a320: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
+0000a330: 7220 6920 696e 2072 616e 6765 2873 656c  r i in range(sel
+0000a340: 662e 6e6d 6f64 656c 7329 3a0a 2020 2020  f.nmodels):.    
+0000a350: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000a360: 2e5f 6f76 6572 6c61 704c 5445 2e61 7070  ._overlapLTE.app
+0000a370: 656e 6428 7365 6c66 2e6d 6f64 656c 735b  end(self.models[
+0000a380: 695d 2e6f 7665 726c 6170 4c54 4529 0a20  i].overlapLTE). 
+0000a390: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000a3a0: 2020 2020 2020 2020 2073 656c 662e 5f6f           self._o
+0000a3b0: 7665 726c 6170 4c54 453d 7365 6c66 2e6d  verlapLTE=self.m
+0000a3c0: 6f64 656c 735b 305d 2e6f 7665 726c 6170  odels[0].overlap
+0000a3d0: 4c54 450a 2020 2020 2020 2020 7265 7475  LTE.        retu
+0000a3e0: 726e 2073 656c 662e 5f6f 7665 726c 6170  rn self._overlap
+0000a3f0: 4c54 450a 0a20 2020 2040 6f76 6572 6c61  LTE..    @overla
+0000a400: 704c 5445 2e73 6574 7465 720a 2020 2020  pLTE.setter.    
+0000a410: 6465 6620 6f76 6572 6c61 704c 5445 2873  def overlapLTE(s
+0000a420: 656c 662c 7661 6c75 6529 3a0a 2020 2020  elf,value):.    
+0000a430: 2020 2020 7365 6c66 2e5f 6f76 6572 6c61      self._overla
+0000a440: 704c 5445 3d76 616c 7565 0a0a 2020 2020  pLTE=value..    
+0000a450: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+0000a460: 6620 6f76 6572 6c61 704e 4c54 4528 7365  f overlapNLTE(se
+0000a470: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
+0000a480: 7365 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a  self.nmodels>1:.
+0000a490: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000a4a0: 2e5f 6f76 6572 6c61 704e 4c54 453d 5b5d  ._overlapNLTE=[]
+0000a4b0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0000a4c0: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
+0000a4d0: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
+0000a4e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000a4f0: 5f6f 7665 726c 6170 4e4c 5445 2e61 7070  _overlapNLTE.app
+0000a500: 656e 6428 7365 6c66 2e6d 6f64 656c 735b  end(self.models[
+0000a510: 695d 2e6f 7665 726c 6170 4e4c 5445 290a  i].overlapNLTE).
+0000a520: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000a530: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000a540: 6f76 6572 6c61 704e 4c54 453d 7365 6c66  overlapNLTE=self
+0000a550: 2e6d 6f64 656c 735b 305d 2e6f 7665 726c  .models[0].overl
+0000a560: 6170 4e4c 5445 0a20 2020 2020 2020 2072  apNLTE.        r
+0000a570: 6574 7572 6e20 7365 6c66 2e5f 6f76 6572  eturn self._over
+0000a580: 6c61 704e 4c54 450a 0a20 2020 2040 6f76  lapNLTE..    @ov
+0000a590: 6572 6c61 704e 4c54 452e 7365 7474 6572  erlapNLTE.setter
+0000a5a0: 0a20 2020 2064 6566 206f 7665 726c 6170  .    def overlap
+0000a5b0: 4e4c 5445 2873 656c 662c 7661 6c75 6529  NLTE(self,value)
+0000a5c0: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+0000a5d0: 6f76 6572 6c61 704e 4c54 453d 7661 6c75  overlapNLTE=valu
+0000a5e0: 650a 0a20 2020 2040 7072 6f70 6572 7479  e..    @property
+0000a5f0: 0a20 2020 2064 6566 206f 7665 726c 6170  .    def overlap
+0000a600: 5461 754c 5445 2873 656c 6629 3a0a 2020  TauLTE(self):.  
+0000a610: 2020 2020 2020 6966 2073 656c 662e 6e6d        if self.nm
+0000a620: 6f64 656c 733e 313a 0a20 2020 2020 2020  odels>1:.       
+0000a630: 2020 2020 2073 656c 662e 5f6f 7665 726c       self._overl
+0000a640: 6170 5461 754c 5445 3d5b 5d0a 2020 2020  apTauLTE=[].    
+0000a650: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+0000a660: 2072 616e 6765 2873 656c 662e 6e6d 6f64   range(self.nmod
+0000a670: 656c 7329 3a0a 2020 2020 2020 2020 2020  els):.          
+0000a680: 2020 2020 2020 7365 6c66 2e5f 6f76 6572        self._over
+0000a690: 6c61 7054 6175 4c54 452e 6170 7065 6e64  lapTauLTE.append
+0000a6a0: 2873 656c 662e 6d6f 6465 6c73 5b69 5d2e  (self.models[i].
+0000a6b0: 6f76 6572 6c61 7054 6175 4c54 4529 0a20  overlapTauLTE). 
+0000a6c0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000a6d0: 2020 2020 2020 2020 2073 656c 662e 5f6f           self._o
+0000a6e0: 7665 726c 6170 5461 754c 5445 3d73 656c  verlapTauLTE=sel
+0000a6f0: 662e 6d6f 6465 6c73 5b30 5d2e 6f76 6572  f.models[0].over
+0000a700: 6c61 7054 6175 4c54 450a 2020 2020 2020  lapTauLTE.      
+0000a710: 2020 7265 7475 726e 2073 656c 662e 5f6f    return self._o
+0000a720: 7665 726c 6170 5461 754c 5445 0a0a 2020  verlapTauLTE..  
+0000a730: 2020 406f 7665 726c 6170 5461 754c 5445    @overlapTauLTE
+0000a740: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
+0000a750: 6f76 6572 6c61 7054 6175 4c54 4528 7365  overlapTauLTE(se
+0000a760: 6c66 2c76 616c 7565 293a 0a20 2020 2020  lf,value):.     
+0000a770: 2020 2073 656c 662e 5f6f 7665 726c 6170     self._overlap
+0000a780: 5461 754c 5445 3d76 616c 7565 0a0a 2020  TauLTE=value..  
+0000a790: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+0000a7a0: 6465 6620 6f76 6572 6c61 7054 6175 4e4c  def overlapTauNL
+0000a7b0: 5445 2873 656c 6629 3a0a 2020 2020 2020  TE(self):.      
+0000a7c0: 2020 6966 2073 656c 662e 6e6d 6f64 656c    if self.nmodel
+0000a7d0: 733e 313a 0a20 2020 2020 2020 2020 2020  s>1:.           
+0000a7e0: 2073 656c 662e 5f6f 7665 726c 6170 5461   self._overlapTa
+0000a7f0: 754e 4c54 453d 5b5d 0a20 2020 2020 2020  uNLTE=[].       
+0000a800: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+0000a810: 6e67 6528 7365 6c66 2e6e 6d6f 6465 6c73  nge(self.nmodels
+0000a820: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000a830: 2020 2073 656c 662e 5f6f 7665 726c 6170     self._overlap
+0000a840: 5461 754e 4c54 452e 6170 7065 6e64 2873  TauNLTE.append(s
+0000a850: 656c 662e 6d6f 6465 6c73 5b69 5d2e 6f76  elf.models[i].ov
+0000a860: 6572 6c61 7054 6175 4e4c 5445 290a 2020  erlapTauNLTE).  
+0000a870: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000a880: 2020 2020 2020 2020 7365 6c66 2e5f 6f76          self._ov
+0000a890: 6572 6c61 7054 6175 4e4c 5445 3d73 656c  erlapTauNLTE=sel
+0000a8a0: 662e 6d6f 6465 6c73 5b30 5d2e 6f76 6572  f.models[0].over
+0000a8b0: 6c61 7054 6175 4e4c 5445 0a20 2020 2020  lapTauNLTE.     
+0000a8c0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+0000a8d0: 6f76 6572 6c61 7054 6175 4e4c 5445 0a0a  overlapTauNLTE..
+0000a8e0: 2020 2020 406f 7665 726c 6170 5461 754e      @overlapTauN
+0000a8f0: 4c54 452e 7365 7474 6572 0a20 2020 2064  LTE.setter.    d
+0000a900: 6566 206f 7665 726c 6170 5461 754e 4c54  ef overlapTauNLT
+0000a910: 4528 7365 6c66 2c76 616c 7565 293a 0a20  E(self,value):. 
+0000a920: 2020 2020 2020 2073 656c 662e 5f6f 7665         self._ove
+0000a930: 726c 6170 5461 754e 4c54 453d 7661 6c75  rlapTauNLTE=valu
+0000a940: 650a 0a20 2020 2040 7072 6f70 6572 7479  e..    @property
+0000a950: 0a20 2020 2064 6566 2063 6f6e 764f 7665  .    def convOve
+0000a960: 726c 6170 5228 7365 6c66 293a 0a20 2020  rlapR(self):.   
+0000a970: 2020 2020 2069 6620 7365 6c66 2e6e 6d6f       if self.nmo
+0000a980: 6465 6c73 3e31 3a0a 2020 2020 2020 2020  dels>1:.        
+0000a990: 2020 2020 7365 6c66 2e5f 636f 6e76 4f76      self._convOv
+0000a9a0: 6572 6c61 7052 3d5b 5d0a 2020 2020 2020  erlapR=[].      
+0000a9b0: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+0000a9c0: 616e 6765 2873 656c 662e 6e6d 6f64 656c  ange(self.nmodel
+0000a9d0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+0000a9e0: 2020 2020 7365 6c66 2e5f 636f 6e76 4f76      self._convOv
+0000a9f0: 6572 6c61 7052 2e61 7070 656e 6428 7365  erlapR.append(se
+0000aa00: 6c66 2e6d 6f64 656c 735b 695d 2e63 6f6e  lf.models[i].con
+0000aa10: 764f 7665 726c 6170 5229 0a20 2020 2020  vOverlapR).     
+0000aa20: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000aa30: 2020 2020 2073 656c 662e 5f63 6f6e 764f       self._convO
+0000aa40: 7665 726c 6170 523d 7365 6c66 2e6d 6f64  verlapR=self.mod
+0000aa50: 656c 735b 305d 2e63 6f6e 764f 7665 726c  els[0].convOverl
+0000aa60: 6170 520a 2020 2020 2020 2020 7265 7475  apR.        retu
+0000aa70: 726e 2073 656c 662e 5f63 6f6e 764f 7665  rn self._convOve
+0000aa80: 726c 6170 520a 0a20 2020 2040 636f 6e76  rlapR..    @conv
+0000aa90: 4f76 6572 6c61 7052 2e73 6574 7465 720a  OverlapR.setter.
+0000aaa0: 2020 2020 6465 6620 636f 6e76 4f76 6572      def convOver
+0000aab0: 6c61 7052 2873 656c 662c 7661 6c75 6529  lapR(self,value)
+0000aac0: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+0000aad0: 636f 6e76 4f76 6572 6c61 7052 3d76 616c  convOverlapR=val
+0000aae0: 7565 0a0a 2020 2020 4070 726f 7065 7274  ue..    @propert
+0000aaf0: 790a 2020 2020 6465 6620 6f76 6572 6c61  y.    def overla
+0000ab00: 7052 2873 656c 6629 3a0a 2020 2020 2020  pR(self):.      
+0000ab10: 2020 6966 2073 656c 662e 6e6d 6f64 656c    if self.nmodel
+0000ab20: 733e 313a 0a20 2020 2020 2020 2020 2020  s>1:.           
+0000ab30: 2073 656c 662e 5f6f 7665 726c 6170 523d   self._overlapR=
+0000ab40: 5b5d 0a20 2020 2020 2020 2020 2020 2066  [].            f
+0000ab50: 6f72 2069 2069 6e20 7261 6e67 6528 7365  or i in range(se
+0000ab60: 6c66 2e6e 6d6f 6465 6c73 293a 0a20 2020  lf.nmodels):.   
+0000ab70: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000ab80: 662e 5f6f 7665 726c 6170 522e 6170 7065  f._overlapR.appe
+0000ab90: 6e64 2873 656c 662e 6d6f 6465 6c73 5b69  nd(self.models[i
+0000aba0: 5d2e 6f76 6572 6c61 7052 290a 2020 2020  ].overlapR).    
+0000abb0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000abc0: 2020 2020 2020 7365 6c66 2e5f 6f76 6572        self._over
+0000abd0: 6c61 7052 3d73 656c 662e 6d6f 6465 6c73  lapR=self.models
+0000abe0: 5b30 5d2e 6f76 6572 6c61 7052 0a20 2020  [0].overlapR.   
+0000abf0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000ac00: 2e5f 6f76 6572 6c61 7052 0a0a 2020 2020  ._overlapR..    
+0000ac10: 406f 7665 726c 6170 522e 7365 7474 6572  @overlapR.setter
+0000ac20: 0a20 2020 2064 6566 206f 7665 726c 6170  .    def overlap
+0000ac30: 5228 7365 6c66 2c76 616c 7565 293a 0a20  R(self,value):. 
+0000ac40: 2020 2020 2020 2073 656c 662e 5f6f 7665         self._ove
+0000ac50: 726c 6170 523d 7661 6c75 650a 0a0a 636c  rlapR=value...cl
+0000ac60: 6173 7320 736c 6162 3a0a 2020 2020 2222  ass slab:.    ""
+0000ac70: 220a 2020 2020 636c 6173 733a 3a20 736c  ".    class:: sl
+0000ac80: 6162 0a20 2020 2043 6c61 7373 2074 6f20  ab.    Class to 
+0000ac90: 686f 6c64 2074 6865 2064 6174 6120 6f66  hold the data of
+0000aca0: 2069 6e64 6976 6964 7561 6c20 736c 6162   individual slab
+0000acb0: 206d 6f64 656c 730a 2020 2020 2222 220a   models.    """.
+0000acc0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+0000acd0: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
+0000ace0: 2073 656c 662e 7370 6563 6965 735f 6e75   self.species_nu
+0000acf0: 6d62 6572 3d4e 6f6e 650a 2020 2020 2020  mber=None.      
+0000ad00: 2020 7365 6c66 2e6d 6f64 656c 5f6e 756d    self.model_num
+0000ad10: 6265 723d 4e6f 6e65 0a20 2020 2020 2020  ber=None.       
+0000ad20: 2073 656c 662e 4e48 3d4e 6f6e 650a 2020   self.NH=None.  
+0000ad30: 2020 2020 2020 7365 6c66 2e6e 436f 6c6c        self.nColl
+0000ad40: 3d4e 6f6e 650a 2020 2020 2020 2020 7365  =None.        se
+0000ad50: 6c66 2e6e 653d 4e6f 6e65 0a20 2020 2020  lf.ne=None.     
+0000ad60: 2020 2073 656c 662e 6e48 653d 4e6f 6e65     self.nHe=None
+0000ad70: 0a20 2020 2020 2020 2073 656c 662e 6e48  .        self.nH
+0000ad80: 4949 3d4e 6f6e 650a 2020 2020 2020 2020  II=None.        
+0000ad90: 7365 6c66 2e6e 4849 3d4e 6f6e 650a 2020  self.nHI=None.  
+0000ada0: 2020 2020 2020 7365 6c66 2e6e 4832 3d4e        self.nH2=N
+0000adb0: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+0000adc0: 2e64 7573 745f 746f 5f67 6173 3d4e 6f6e  .dust_to_gas=Non
+0000add0: 650a 2020 2020 2020 2020 7365 6c66 2e76  e.        self.v
+0000ade0: 7475 7262 3d4e 6f6e 650a 2020 2020 2020  turb=None.      
+0000adf0: 2020 7365 6c66 2e54 673d 4e6f 6e65 0a20    self.Tg=None. 
+0000ae00: 2020 2020 2020 2073 656c 662e 5464 3d4e         self.Td=N
+0000ae10: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+0000ae20: 2e73 7065 6369 6573 5f6e 616d 653d 4e6f  .species_name=No
+0000ae30: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
+0000ae40: 7370 6563 6965 735f 696e 6465 783d 4e6f  species_index=No
+0000ae50: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
+0000ae60: 6162 756e 6461 6e63 653d 4e6f 6e65 0a20  abundance=None. 
+0000ae70: 2020 2020 2020 2073 656c 662e 6476 3d4e         self.dv=N
+0000ae80: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+0000ae90: 2e6e 6c65 7665 6c73 3d4e 6f6e 650a 2020  .nlevels=None.  
+0000aea0: 2020 2020 2020 7365 6c66 2e6e 6c69 6e65        self.nline
+0000aeb0: 733d 4e6f 6e65 0a20 2020 2020 2020 2073  s=None.        s
+0000aec0: 656c 662e 6c69 6e65 6461 7461 3d4e 6f6e  elf.linedata=Non
+0000aed0: 650a 2020 2020 2020 2020 7365 6c66 2e6c  e.        self.l
+0000aee0: 6576 656c 6461 7461 3d4e 6f6e 650a 2020  eveldata=None.  
+0000aef0: 2020 2020 2020 7365 6c66 2e63 6f6e 7657        self.convW
+0000af00: 6176 656c 656e 6774 683d 4e6f 6e65 0a20  avelength=None. 
+0000af10: 2020 2020 2020 2073 656c 662e 636f 6e76         self.conv
+0000af20: 4c54 4566 6c75 783d 4e6f 6e65 0a20 2020  LTEflux=None.   
+0000af30: 2020 2020 2073 656c 662e 636f 6e76 4e4c       self.convNL
+0000af40: 5445 666c 7578 3d4e 6f6e 650a 2020 2020  TEflux=None.    
+0000af50: 2020 2020 7365 6c66 2e63 6f6e 7654 7970      self.convTyp
+0000af60: 653d 4e6f 6e65 0a20 2020 2020 2020 2073  e=None.        s
+0000af70: 656c 662e 636f 6e76 523d 4e6f 6e65 0a20  elf.convR=None. 
+0000af80: 2020 2020 2020 2073 656c 662e 6f76 6572         self.over
+0000af90: 6c61 704c 5445 3d4e 6f6e 650a 2020 2020  lapLTE=None.    
+0000afa0: 2020 2020 7365 6c66 2e6f 7665 726c 6170      self.overlap
+0000afb0: 4e4c 5445 3d4e 6f6e 650a 2020 2020 2020  NLTE=None.      
+0000afc0: 2020 7365 6c66 2e6f 7665 726c 6170 5461    self.overlapTa
+0000afd0: 754c 5445 3d4e 6f6e 650a 2020 2020 2020  uLTE=None.      
+0000afe0: 2020 7365 6c66 2e6f 7665 726c 6170 5461    self.overlapTa
+0000aff0: 754e 4c54 453d 4e6f 6e65 0a20 2020 2020  uNLTE=None.     
+0000b000: 2020 2073 656c 662e 6f76 6572 6c61 7046     self.overlapF
+0000b010: 7265 713d 4e6f 6e65 0a20 2020 2020 2020  req=None.       
+0000b020: 2073 656c 662e 636f 6e76 4f76 6572 6c61   self.convOverla
+0000b030: 704c 5445 3d4e 6f6e 650a 2020 2020 2020  pLTE=None.      
+0000b040: 2020 7365 6c66 2e63 6f6e 764f 7665 726c    self.convOverl
+0000b050: 6170 4e4c 5445 3d4e 6f6e 650a 2020 2020  apNLTE=None.    
+0000b060: 2020 2020 7365 6c66 2e63 6f6e 764f 7665      self.convOve
+0000b070: 726c 6170 4672 6571 3d4e 6f6e 650a 2020  rlapFreq=None.  
+0000b080: 2020 2020 2020 7365 6c66 2e63 6f6e 764f        self.convO
+0000b090: 7665 726c 6170 5761 7665 3d4e 6f6e 650a  verlapWave=None.
+0000b0a0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+0000b0b0: 764f 7665 726c 6170 523d 3165 350a 2020  vOverlapR=1e5.  
+0000b0c0: 2020 2020 2020 7365 6c66 2e6f 7665 726c        self.overl
+0000b0d0: 6170 523d 3165 350a 0a20 2020 2064 6566  apR=1e5..    def
+0000b0e0: 205f 5f73 7472 5f5f 2873 656c 6629 3a0a   __str__(self):.
+0000b0f0: 2020 2020 2020 2020 6f75 7470 7574 3d22          output="
+0000b100: 496e 666f 204d 6f64 656c 3a20 5c6e 220a  Info Model: \n".
+0000b110: 2020 2020 2020 2020 6f75 7470 7574 2b3d          output+=
+0000b120: 2773 7065 6369 6573 5f6e 756d 6265 723d  'species_number=
+0000b130: 2027 0a20 2020 2020 2020 206f 7574 7075   '.        outpu
+0000b140: 742b 3d73 7472 2873 656c 662e 7370 6563  t+=str(self.spec
+0000b150: 6965 735f 6e75 6d62 6572 292b 275c 6e5c  ies_number)+'\n\
+0000b160: 6e27 0a20 2020 2020 2020 206f 7574 7075  n'.        outpu
+0000b170: 742b 3d27 6d6f 6465 6c5f 6e75 6d62 6572  t+='model_number
+0000b180: 2020 3d20 270a 2020 2020 2020 2020 6f75    = '.        ou
+0000b190: 7470 7574 2b3d 7374 7228 7365 6c66 2e6d  tput+=str(self.m
+0000b1a0: 6f64 656c 5f6e 756d 6265 7229 2b27 5c6e  odel_number)+'\n
+0000b1b0: 5c6e 270a 2020 2020 2020 2020 6f75 7470  \n'.        outp
+0000b1c0: 7574 2b3d 274e 4820 2020 2020 2020 2020  ut+='NH         
+0000b1d0: 2020 203d 2027 0a20 2020 2020 2020 206f     = '.        o
+0000b1e0: 7574 7075 742b 3d73 7472 2873 656c 662e  utput+=str(self.
+0000b1f0: 4e48 292b 275c 6e5c 6e27 0a20 2020 2020  NH)+'\n\n'.     
+0000b200: 2020 206f 7574 7075 742b 3d27 6e43 6f6c     output+='nCol
+0000b210: 6c20 2020 2020 2020 2020 3d20 270a 2020  l         = '.  
+0000b220: 2020 2020 2020 6f75 7470 7574 2b3d 7374        output+=st
+0000b230: 7228 7365 6c66 2e6e 436f 6c6c 292b 275c  r(self.nColl)+'\
+0000b240: 6e5c 6e27 0a20 2020 2020 2020 206f 7574  n\n'.        out
+0000b250: 7075 742b 3d27 6e65 2020 2020 2020 2020  put+='ne        
+0000b260: 2020 2020 3d20 270a 2020 2020 2020 2020      = '.        
+0000b270: 6f75 7470 7574 2b3d 7374 7228 7365 6c66  output+=str(self
+0000b280: 2e6e 6529 2b27 5c6e 5c6e 270a 2020 2020  .ne)+'\n\n'.    
+0000b290: 2020 2020 6f75 7470 7574 2b3d 276e 4865      output+='nHe
+0000b2a0: 2020 2020 2020 2020 2020 203d 2027 0a20             = '. 
+0000b2b0: 2020 2020 2020 206f 7574 7075 742b 3d73         output+=s
+0000b2c0: 7472 2873 656c 662e 6e48 6529 2b27 5c6e  tr(self.nHe)+'\n
+0000b2d0: 5c6e 270a 2020 2020 2020 2020 6f75 7470  \n'.        outp
+0000b2e0: 7574 2b3d 276e 4849 4920 2020 2020 2020  ut+='nHII       
+0000b2f0: 2020 203d 2027 0a20 2020 2020 2020 206f     = '.        o
+0000b300: 7574 7075 742b 3d73 7472 2873 656c 662e  utput+=str(self.
+0000b310: 6e48 4949 292b 275c 6e5c 6e27 0a20 2020  nHII)+'\n\n'.   
+0000b320: 2020 2020 206f 7574 7075 742b 3d27 6e48       output+='nH
+0000b330: 4920 2020 2020 2020 2020 2020 3d20 270a  I           = '.
 0000b340: 2020 2020 2020 2020 6f75 7470 7574 2b3d          output+=
-0000b350: 2761 6275 6e64 616e 6365 2020 2020 203d  'abundance     =
-0000b360: 2027 0a20 2020 2020 2020 206f 7574 7075   '.        outpu
-0000b370: 742b 3d73 7472 2873 656c 662e 6162 756e  t+=str(self.abun
-0000b380: 6461 6e63 6529 2b27 5c6e 5c6e 270a 2020  dance)+'\n\n'.  
-0000b390: 2020 2020 2020 6f75 7470 7574 2b3d 2764        output+='d
-0000b3a0: 7620 2020 2020 2020 2020 2020 203d 2027  v            = '
-0000b3b0: 0a20 2020 2020 2020 206f 7574 7075 742b  .        output+
-0000b3c0: 3d73 7472 2873 656c 662e 6476 292b 275c  =str(self.dv)+'\
-0000b3d0: 6e5c 6e27 0a20 2020 2020 2020 206f 7574  n\n'.        out
-0000b3e0: 7075 742b 3d27 6e6c 6576 656c 7320 2020  put+='nlevels   
-0000b3f0: 2020 2020 3d20 270a 2020 2020 2020 2020      = '.        
-0000b400: 6f75 7470 7574 2b3d 7374 7228 7365 6c66  output+=str(self
-0000b410: 2e6e 6c65 7665 6c73 292b 275c 6e5c 6e27  .nlevels)+'\n\n'
-0000b420: 0a20 2020 2020 2020 206f 7574 7075 742b  .        output+
-0000b430: 3d27 6e6c 696e 6573 2020 2020 2020 2020  ='nlines        
-0000b440: 3d20 270a 2020 2020 2020 2020 6f75 7470  = '.        outp
-0000b450: 7574 2b3d 7374 7228 7365 6c66 2e6e 6c69  ut+=str(self.nli
-0000b460: 6e65 7329 2b27 5c6e 5c6e 270a 2020 2020  nes)+'\n\n'.    
-0000b470: 2020 2020 6f75 7470 7574 2b3d 2763 6f6e      output+='con
-0000b480: 7654 7970 6520 2020 2020 2020 3d20 270a  vType       = '.
-0000b490: 2020 2020 2020 2020 6f75 7470 7574 2b3d          output+=
-0000b4a0: 7374 7228 7365 6c66 2e63 6f6e 7654 7970  str(self.convTyp
-0000b4b0: 6529 2b27 5c6e 5c6e 270a 2020 2020 2020  e)+'\n\n'.      
-0000b4c0: 2020 6f75 7470 7574 2b3d 2763 6f6e 7652    output+='convR
-0000b4d0: 2020 2020 2020 2020 3d20 270a 2020 2020          = '.    
-0000b4e0: 2020 2020 6f75 7470 7574 2b3d 7374 7228      output+=str(
-0000b4f0: 7365 6c66 2e63 6f6e 7652 292b 275c 6e5c  self.convR)+'\n\
-0000b500: 6e27 0a20 2020 2020 2020 2072 6574 7572  n'.        retur
-0000b510: 6e20 6f75 7470 7574 0a0a 2020 2020 6465  n output..    de
-0000b520: 6620 636f 6e76 6f6c 7665 2873 656c 662c  f convolve(self,
-0000b530: 6672 6571 5f62 696e 733d 4e6f 6e65 2c52  freq_bins=None,R
-0000b540: 3d31 2c6c 616d 6264 615f 303d 312c 6c61  =1,lambda_0=1,la
-0000b550: 6d62 6461 5f6e 3d31 2c76 723d 3133 3030  mbda_n=1,vr=1300
-0000b560: 2c4e 4c54 453d 4661 6c73 652c 636f 6e76  ,NLTE=False,conv
-0000b570: 5f74 7970 653d 312c 6f76 6572 6c61 703d  _type=1,overlap=
-0000b580: 4661 6c73 6529 3a0a 2020 2020 2020 2020  False):.        
-0000b590: 6966 206f 7665 726c 6170 3a0a 2020 2020  if overlap:.    
-0000b5a0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-0000b5b0: 766f 6c76 655f 6f76 6572 6c61 7028 523d  volve_overlap(R=
-0000b5c0: 522c 6c61 6d62 6461 5f30 3d6c 616d 6264  R,lambda_0=lambd
-0000b5d0: 615f 302c 6c61 6d62 6461 5f6e 3d6c 616d  a_0,lambda_n=lam
-0000b5e0: 6264 615f 6e29 0a20 2020 2020 2020 2020  bda_n).         
-0000b5f0: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-0000b600: 2020 743d 2746 4c54 4527 0a20 2020 2020    t='FLTE'.     
-0000b610: 2020 2069 6620 4e4c 5445 3a0a 2020 2020     if NLTE:.    
-0000b620: 2020 2020 2020 2020 743d 2746 4e4c 5445          t='FNLTE
-0000b630: 270a 2020 2020 2020 2020 6461 3d73 656c  '.        da=sel
-0000b640: 662e 6c69 6e65 6461 7461 0a20 2020 2020  f.linedata.     
-0000b650: 2020 2069 6620 6c61 6d62 6461 5f30 3d3d     if lambda_0==
-0000b660: 6c61 6d62 6461 5f6e 3a0a 2020 2020 2020  lambda_n:.      
-0000b670: 2020 2020 2020 6c61 6d62 6461 5f30 3d6e        lambda_0=n
-0000b680: 702e 616d 696e 2864 615b 2747 487a 275d  p.amin(da['GHz']
-0000b690: 3e63 2f6c 616d 6264 615f 6e2a 3165 2d33  >c/lambda_n*1e-3
-0000b6a0: 290a 2020 2020 2020 2020 2020 2020 6c61  ).            la
-0000b6b0: 6d62 6461 5f6e 3d6e 702e 616d 6178 2864  mbda_n=np.amax(d
-0000b6c0: 615b 2747 487a 275d 3e63 2f6c 616d 6264  a['GHz']>c/lambd
-0000b6d0: 615f 6e2a 3165 2d33 290a 2020 2020 2020  a_n*1e-3).      
-0000b6e0: 2020 2020 2020 6c61 6d62 6461 5f30 3d6c        lambda_0=l
-0000b6f0: 616d 6264 615f 302a 3130 2a2a 2d30 2e30  ambda_0*10**-0.0
-0000b700: 350a 2020 2020 2020 2020 2020 2020 6c61  5.            la
-0000b710: 6d62 6461 5f6e 3d6c 616d 6264 615f 6e2a  mbda_n=lambda_n*
-0000b720: 3130 2a2a 302e 3035 0a20 2020 2020 2020  10**0.05.       
-0000b730: 2064 615f 7265 713d 6461 5b28 6461 5b27   da_req=da[(da['
-0000b740: 4748 7a27 5d3e 632f 6c61 6d62 6461 5f6e  GHz']>c/lambda_n
-0000b750: 2a31 652d 3329 2628 6461 5b27 4748 7a27  *1e-3)&(da['GHz'
-0000b760: 5d3c 632f 6c61 6d62 6461 5f30 2a31 652d  ]<c/lambda_0*1e-
-0000b770: 3329 5d0a 2020 2020 2020 2020 6461 5f72  3)].        da_r
-0000b780: 6571 2e72 6573 6574 5f69 6e64 6578 2864  eq.reset_index(d
-0000b790: 726f 703d 5472 7565 2c69 6e70 6c61 6365  rop=True,inplace
-0000b7a0: 3d54 7275 6529 0a20 2020 2020 2020 2069  =True).        i
-0000b7b0: 6620 636f 6e76 5f74 7970 653d 3d31 3a0a  f conv_type==1:.
-0000b7c0: 2020 2020 2020 2020 2020 2020 6c2c 663d              l,f=
-0000b7d0: 6765 6e65 7261 6c43 6f6e 766f 6c76 6528  generalConvolve(
-0000b7e0: 6461 5f72 6571 5b74 5d2c 6461 5f72 6571  da_req[t],da_req
-0000b7f0: 5b27 4748 7a27 5d2c 523d 522c 6c61 6d62  ['GHz'],R=R,lamb
-0000b800: 6461 5f30 3d6c 616d 6264 615f 302c 6c61  da_0=lambda_0,la
-0000b810: 6d62 6461 5f6e 3d6c 616d 6264 615f 6e29  mbda_n=lambda_n)
-0000b820: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-0000b830: 2020 2020 2020 2020 2020 206c 2c66 3d73             l,f=s
-0000b840: 7065 6343 6f6e 766f 6c76 6528 6461 5f72  pecConvolve(da_r
-0000b850: 6571 5b74 5d2c 6461 5f72 6571 5b27 4748  eq[t],da_req['GH
-0000b860: 7a27 5d2c 6672 6571 5f62 696e 733d 6672  z'],freq_bins=fr
-0000b870: 6571 5f62 696e 732c 523d 522c 6c61 6d62  eq_bins,R=R,lamb
-0000b880: 6461 5f30 3d6c 616d 6264 615f 302c 6c61  da_0=lambda_0,la
-0000b890: 6d62 6461 5f6e 3d6c 616d 6264 615f 6e2c  mbda_n=lambda_n,
-0000b8a0: 7672 3d76 7229 0a20 2020 2020 2020 2073  vr=vr).        s
-0000b8b0: 656c 662e 636f 6e76 5761 7665 6c65 6e67  elf.convWaveleng
-0000b8c0: 7468 3d6c 0a20 2020 2020 2020 2073 656c  th=l.        sel
-0000b8d0: 662e 636f 6e76 5479 7065 3d63 6f6e 765f  f.convType=conv_
-0000b8e0: 7479 7065 0a20 2020 2020 2020 2073 656c  type.        sel
-0000b8f0: 662e 636f 6e76 523d 520a 2020 2020 2020  f.convR=R.      
-0000b900: 2020 6966 204e 4c54 453a 0a20 2020 2020    if NLTE:.     
-0000b910: 2020 2020 2020 2073 656c 662e 636f 6e76         self.conv
-0000b920: 4e4c 5445 666c 7578 3d66 0a20 2020 2020  NLTEflux=f.     
-0000b930: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000b940: 2020 2020 2073 656c 662e 636f 6e76 4c54       self.convLT
-0000b950: 4566 6c75 783d 660a 0a20 2020 2064 6566  Eflux=f..    def
-0000b960: 2063 6f6e 766f 6c76 655f 6f76 6572 6c61   convolve_overla
-0000b970: 7028 7365 6c66 2c52 3d31 2c6c 616d 6264  p(self,R=1,lambd
-0000b980: 615f 303d 312c 6c61 6d62 6461 5f6e 3d31  a_0=1,lambda_n=1
-0000b990: 293a 0a20 2020 2020 2020 2069 6620 6c61  ):.        if la
-0000b9a0: 6d62 6461 5f30 3d3d 6c61 6d62 6461 5f6e  mbda_0==lambda_n
-0000b9b0: 3a0a 2020 2020 2020 2020 2020 2020 6c61  :.            la
-0000b9c0: 6d62 6461 5f30 3d6e 702e 616d 696e 2863  mbda_0=np.amin(c
-0000b9d0: 2f73 656c 662e 6f76 6572 6c61 7046 7265  /self.overlapFre
-0000b9e0: 712a 3165 2d33 290a 2020 2020 2020 2020  q*1e-3).        
-0000b9f0: 2020 2020 6c61 6d62 6461 5f6e 3d6e 702e      lambda_n=np.
-0000ba00: 616d 6178 2863 2f73 656c 662e 6f76 6572  amax(c/self.over
-0000ba10: 6c61 7046 7265 712a 3165 2d33 290a 2020  lapFreq*1e-3).  
-0000ba20: 2020 2020 2020 2020 2020 6c61 6d62 6461            lambda
-0000ba30: 5f30 3d6c 616d 6264 615f 302a 3130 2a2a  _0=lambda_0*10**
-0000ba40: 2d30 2e30 350a 2020 2020 2020 2020 2020  -0.05.          
-0000ba50: 2020 6c61 6d62 6461 5f6e 3d6c 616d 6264    lambda_n=lambd
-0000ba60: 615f 6e2a 3130 2a2a 302e 3035 0a20 2020  a_n*10**0.05.   
-0000ba70: 2020 2020 206d 6173 6b3d 2873 656c 662e       mask=(self.
-0000ba80: 6f76 6572 6c61 7046 7265 713e 632f 6c61  overlapFreq>c/la
-0000ba90: 6d62 6461 5f6e 2a31 652d 3329 2628 7365  mbda_n*1e-3)&(se
-0000baa0: 6c66 2e6f 7665 726c 6170 4672 6571 3c63  lf.overlapFreq<c
-0000bab0: 2f6c 616d 6264 615f 302a 3165 2d33 290a  /lambda_0*1e-3).
-0000bac0: 2020 2020 2020 2020 4657 484d 3d73 656c          FWHM=sel
-0000bad0: 662e 6f76 6572 6c61 7052 2f52 2f32 2e33  f.overlapR/R/2.3
-0000bae0: 3535 0a20 2020 2020 2020 2067 3d47 6175  55.        g=Gau
-0000baf0: 7373 6961 6e31 444b 6572 6e65 6c28 7374  ssian1DKernel(st
-0000bb00: 6464 6576 3d46 5748 4d2c 6661 6374 6f72  ddev=FWHM,factor
-0000bb10: 3d37 290a 2020 2020 2020 2020 7365 6c66  =7).        self
-0000bb20: 2e63 6f6e 764f 7665 726c 6170 4c54 453d  .convOverlapLTE=
-0000bb30: 6170 795f 636f 6e76 6f6c 7665 2873 656c  apy_convolve(sel
-0000bb40: 662e 6f76 6572 6c61 704c 5445 5b6d 6173  f.overlapLTE[mas
-0000bb50: 6b5d 2c67 290a 2020 2020 2020 2020 7365  k],g).        se
-0000bb60: 6c66 2e63 6f6e 764f 7665 726c 6170 4e4c  lf.convOverlapNL
-0000bb70: 5445 3d61 7079 5f63 6f6e 766f 6c76 6528  TE=apy_convolve(
-0000bb80: 7365 6c66 2e6f 7665 726c 6170 4e4c 5445  self.overlapNLTE
-0000bb90: 5b6d 6173 6b5d 2c67 290a 2020 2020 2020  [mask],g).      
-0000bba0: 2020 7365 6c66 2e63 6f6e 764f 7665 726c    self.convOverl
-0000bbb0: 6170 4672 6571 3d73 656c 662e 6f76 6572  apFreq=self.over
-0000bbc0: 6c61 7046 7265 715b 6d61 736b 5d2a 312e  lapFreq[mask]*1.
-0000bbd0: 300a 2020 2020 2020 2020 7365 6c66 2e63  0.        self.c
-0000bbe0: 6f6e 764f 7665 726c 6170 5761 7665 3d63  onvOverlapWave=c
-0000bbf0: 2f73 656c 662e 636f 6e76 4f76 6572 6c61  /self.convOverla
-0000bc00: 7046 7265 712a 3165 2d33 0a20 2020 2020  pFreq*1e-3.     
-0000bc10: 2020 2073 656c 662e 636f 6e76 4f76 6572     self.convOver
-0000bc20: 6c61 7052 3d52 0a0a 2020 2020 6465 6620  lapR=R..    def 
-0000bc30: 7368 6f77 2873 656c 6629 3a0a 2020 2020  show(self):.    
-0000bc40: 2020 2020 7072 696e 7428 7365 6c66 290a      print(self).
-0000bc50: 2020 2020 2020 2020 7072 696e 7428 276c          print('l
-0000bc60: 696e 6544 6174 6120 2020 203d 2027 290a  ineData    = ').
-0000bc70: 2020 2020 2020 2020 7072 696e 7428 7365          print(se
-0000bc80: 6c66 2e6c 696e 6564 6174 6129 0a20 2020  lf.linedata).   
-0000bc90: 2020 2020 2070 7269 6e74 2827 6c65 7665       print('leve
-0000bca0: 6c44 6174 6120 2020 3d20 2729 0a20 2020  lData   = ').   
-0000bcb0: 2020 2020 2070 7269 6e74 2873 656c 662e       print(self.
-0000bcc0: 6c65 7665 6c64 6174 6129 0a0a 0a63 6c61  leveldata)...cla
-0000bcd0: 7373 2073 6c61 6231 443a 0a20 2020 2022  ss slab1D:.    "
-0000bce0: 2222 0a20 2020 2063 6c61 7373 3a3a 2073  "".    class:: s
-0000bcf0: 6c61 6231 440a 2020 2020 436c 6173 7320  lab1D.    Class 
-0000bd00: 746f 2068 6f6c 6420 7468 6520 6461 7461  to hold the data
-0000bd10: 206f 6620 3144 2073 6c61 6220 6d6f 6465   of 1D slab mode
-0000bd20: 6c73 0a20 2020 2022 2222 0a0a 2020 2020  ls.    """..    
-0000bd30: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-0000bd40: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
-0000bd50: 2e64 6972 6563 746f 7279 3d4e 6f6e 650a  .directory=None.
-0000bd60: 2020 2020 2020 2020 7365 6c66 2e66 6c75          self.flu
-0000bd70: 783d 4e6f 6e65 0a20 2020 2020 2020 2073  x=None.        s
-0000bd80: 656c 662e 6672 6571 7565 6e63 793d 4e6f  elf.frequency=No
-0000bd90: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
-0000bda0: 4e73 7065 6369 6573 3d4e 6f6e 650a 2020  Nspecies=None.  
-0000bdb0: 2020 2020 2020 7365 6c66 2e73 7065 6369        self.speci
-0000bdc0: 6573 3d5b 5d0a 2020 2020 2020 2020 7365  es=[].        se
-0000bdd0: 6c66 2e4e 6772 6964 3d4e 6f6e 650a 2020  lf.Ngrid=None.  
-0000bde0: 2020 2020 2020 7365 6c66 2e52 3d4e 6f6e        self.R=Non
-0000bdf0: 650a 2020 2020 2020 2020 7365 6c66 2e67  e.        self.g
-0000be00: 7269 643d 7064 2e44 6174 6146 7261 6d65  rid=pd.DataFrame
-0000be10: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-0000be20: 736f 7572 6365 5f66 756e 6374 696f 6e3d  source_function=
-0000be30: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
-0000be40: 662e 736f 7572 6365 5f66 756e 6374 696f  f.source_functio
-0000be50: 6e5f 6761 733d 4e6f 6e65 0a20 2020 2020  n_gas=None.     
-0000be60: 2020 2073 656c 662e 7461 755f 6475 7374     self.tau_dust
-0000be70: 3d4e 6f6e 650a 2020 2020 2020 2020 7365  =None.        se
-0000be80: 6c66 2e74 6175 5f67 6173 3d4e 6f6e 650a  lf.tau_gas=None.
-0000be90: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-0000bea0: 7657 6176 656c 656e 6774 683d 4e6f 6e65  vWavelength=None
-0000beb0: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-0000bec0: 6e76 4672 6571 7565 6e63 793d 4e6f 6e65  nvFrequency=None
-0000bed0: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-0000bee0: 6e76 5f66 6c75 783d 4e6f 6e65 0a20 2020  nv_flux=None.   
-0000bef0: 2020 2020 2073 656c 662e 636f 6e76 523d       self.convR=
-0000bf00: 4e6f 6e65 0a0a 2020 2020 6465 6620 5f5f  None..    def __
-0000bf10: 7374 725f 5f28 7365 6c66 293a 0a20 2020  str__(self):.   
-0000bf20: 2020 2020 206f 7574 7075 743d 2249 6e66       output="Inf
-0000bf30: 6f20 4d6f 6465 6c3a 205c 6e22 0a20 2020  o Model: \n".   
-0000bf40: 2020 2020 206f 7574 7075 742b 3d27 4e75       output+='Nu
-0000bf50: 6d62 6572 206f 6620 7370 6563 6965 7320  mber of species 
-0000bf60: 2020 2020 2020 2020 203d 2027 0a20 2020           = '.   
-0000bf70: 2020 2020 206f 7574 7075 742b 3d73 7472       output+=str
-0000bf80: 2873 656c 662e 4e73 7065 6369 6573 292b  (self.Nspecies)+
-0000bf90: 275c 6e5c 6e27 0a20 2020 2020 2020 206f  '\n\n'.        o
-0000bfa0: 7574 7075 742b 3d27 4772 6964 2073 697a  utput+='Grid siz
-0000bfb0: 6520 2020 2020 2020 2020 2020 2020 2020  e               
-0000bfc0: 2020 203d 2027 0a20 2020 2020 2020 206f     = '.        o
-0000bfd0: 7574 7075 742b 3d73 7472 2873 656c 662e  utput+=str(self.
-0000bfe0: 4e67 7269 6429 2b27 5c6e 5c6e 270a 2020  Ngrid)+'\n\n'.  
-0000bff0: 2020 2020 2020 6f75 7470 7574 2b3d 2752        output+='R
-0000c000: 6573 6f6c 7669 6e67 2070 6f77 6572 206f  esolving power o
-0000c010: 6620 7370 6563 7472 6120 3d20 270a 2020  f spectra = '.  
-0000c020: 2020 2020 2020 6f75 7470 7574 2b3d 7374        output+=st
-0000c030: 7228 7365 6c66 2e52 292b 275c 6e5c 6e27  r(self.R)+'\n\n'
-0000c040: 0a20 2020 2020 2020 206f 7574 7075 742b  .        output+
-0000c050: 3d27 4f75 7470 7574 2066 696c 6520 7061  ='Output file pa
-0000c060: 7468 203d 2027 0a20 2020 2020 2020 206f  th = '.        o
-0000c070: 7574 7075 742b 3d73 7472 2873 656c 662e  utput+=str(self.
-0000c080: 6469 7265 6374 6f72 7929 2b27 5c6e 5c6e  directory)+'\n\n
-0000c090: 270a 2020 2020 2020 2020 7265 7475 726e  '.        return
-0000c0a0: 206f 7574 7075 740a 0a20 2020 2064 6566   output..    def
-0000c0b0: 2063 6f6e 766f 6c76 6528 7365 6c66 2c52   convolve(self,R
-0000c0c0: 3d31 2c6c 616d 6264 615f 303d 312c 6c61  =1,lambda_0=1,la
-0000c0d0: 6d62 6461 5f6e 3d31 2c76 6572 626f 7365  mbda_n=1,verbose
-0000c0e0: 3d54 7275 6529 3a0a 2020 2020 2020 2020  =True):.        
-0000c0f0: 6966 2076 6572 626f 7365 3a20 7072 696e  if verbose: prin
-0000c100: 7428 2243 6f6e 766f 6c76 696e 6720 746f  t("Convolving to
-0000c110: 2022 2c52 290a 2020 2020 2020 2020 6966   ",R).        if
-0000c120: 206c 616d 6264 615f 303d 3d6c 616d 6264   lambda_0==lambd
-0000c130: 615f 6e3a 0a20 2020 2020 2020 2020 2020  a_n:.           
-0000c140: 206c 616d 6264 615f 303d 6e70 2e61 6d69   lambda_0=np.ami
-0000c150: 6e28 632f 7365 6c66 2e66 7265 7175 656e  n(c/self.frequen
-0000c160: 6379 2a31 652d 3329 0a20 2020 2020 2020  cy*1e-3).       
-0000c170: 2020 2020 206c 616d 6264 615f 6e3d 6e70       lambda_n=np
-0000c180: 2e61 6d61 7828 632f 7365 6c66 2e66 7265  .amax(c/self.fre
-0000c190: 7175 656e 6379 2a31 652d 3329 0a20 2020  quency*1e-3).   
-0000c1a0: 2020 2020 2020 2020 206c 616d 6264 615f           lambda_
-0000c1b0: 303d 6c61 6d62 6461 5f30 2a31 302a 2a2d  0=lambda_0*10**-
-0000c1c0: 302e 3035 0a20 2020 2020 2020 2020 2020  0.05.           
-0000c1d0: 206c 616d 6264 615f 6e3d 6c61 6d62 6461   lambda_n=lambda
-0000c1e0: 5f6e 2a31 302a 2a30 2e30 350a 2020 2020  _n*10**0.05.    
-0000c1f0: 2020 2020 6d61 736b 3d28 7365 6c66 2e66      mask=(self.f
-0000c200: 7265 7175 656e 6379 3e63 2f6c 616d 6264  requency>c/lambd
-0000c210: 615f 6e2a 3165 2d33 2926 2873 656c 662e  a_n*1e-3)&(self.
-0000c220: 6672 6571 7565 6e63 793c 632f 6c61 6d62  frequency<c/lamb
-0000c230: 6461 5f30 2a31 652d 3329 0a20 2020 2020  da_0*1e-3).     
-0000c240: 2020 2046 5748 4d3d 7365 6c66 2e52 2f52     FWHM=self.R/R
-0000c250: 2f32 2e33 3535 0a20 2020 2020 2020 2067  /2.355.        g
-0000c260: 3d47 6175 7373 6961 6e31 444b 6572 6e65  =Gaussian1DKerne
-0000c270: 6c28 7374 6464 6576 3d46 5748 4d2c 6661  l(stddev=FWHM,fa
-0000c280: 6374 6f72 3d37 290a 2020 2020 2020 2020  ctor=7).        
-0000c290: 7365 6c66 2e63 6f6e 765f 666c 7578 3d61  self.conv_flux=a
-0000c2a0: 7079 5f63 6f6e 766f 6c76 6528 7365 6c66  py_convolve(self
-0000c2b0: 2e66 6c75 785b 6d61 736b 5d2c 6729 0a20  .flux[mask],g). 
-0000c2c0: 2020 2020 2020 2073 656c 662e 636f 6e76         self.conv
-0000c2d0: 4672 6571 7565 6e63 793d 7365 6c66 2e66  Frequency=self.f
-0000c2e0: 7265 7175 656e 6379 5b6d 6173 6b5d 2a31  requency[mask]*1
-0000c2f0: 2e30 0a20 2020 2020 2020 2073 656c 662e  .0.        self.
-0000c300: 636f 6e76 523d 520a 2020 2020 2020 2020  convR=R.        
-0000c310: 7365 6c66 2e63 6f6e 7657 6176 656c 656e  self.convWavelen
-0000c320: 6774 683d 632f 7365 6c66 2e63 6f6e 7646  gth=c/self.convF
-0000c330: 7265 7175 656e 6379 2a31 652d 330a 0a20  requency*1e-3.. 
-0000c340: 2020 2064 6566 2073 686f 7728 7365 6c66     def show(self
-0000c350: 293a 0a20 2020 2020 2020 2070 7269 6e74  ):.        print
-0000c360: 2873 656c 6629 0a20 2020 2020 2020 2070  (self).        p
-0000c370: 7269 6e74 2827 4772 6964 2020 2020 3d20  rint('Grid    = 
-0000c380: 2729 0a20 2020 2020 2020 2070 7269 6e74  ').        print
-0000c390: 2873 656c 662e 6772 6964 290a 2020 2020  (self.grid).    
-0000c3a0: 2020 2020 7072 696e 7428 2753 6f75 7263      print('Sourc
-0000c3b0: 6520 6675 6e63 7469 6f6e 2020 203d 2027  e function   = '
-0000c3c0: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
-0000c3d0: 7365 6c66 2e73 6f75 7263 655f 6675 6e63  self.source_func
-0000c3e0: 7469 6f6e 290a 2020 2020 2020 2020 7072  tion).        pr
-0000c3f0: 696e 7428 2747 6173 206f 6e6c 7920 736f  int('Gas only so
-0000c400: 7572 6365 2066 756e 6374 696f 6e20 2020  urce function   
-0000c410: 3d20 2729 0a20 2020 2020 2020 2070 7269  = ').        pri
-0000c420: 6e74 2873 656c 662e 736f 7572 6365 5f66  nt(self.source_f
-0000c430: 756e 6374 696f 6e5f 6761 7329 0a20 2020  unction_gas).   
-0000c440: 2020 2020 2070 7269 6e74 2827 4475 7374       print('Dust
-0000c450: 206f 7074 6963 616c 2064 6570 7468 2020   optical depth  
-0000c460: 203d 2027 290a 2020 2020 2020 2020 7072   = ').        pr
-0000c470: 696e 7428 7365 6c66 2e74 6175 5f64 7573  int(self.tau_dus
-0000c480: 7429 0a20 2020 2020 2020 2070 7269 6e74  t).        print
-0000c490: 2827 4761 7320 6f70 7469 6361 6c20 6465  ('Gas optical de
-0000c4a0: 7074 6820 2020 3d20 2729 0a20 2020 2020  pth   = ').     
-0000c4b0: 2020 2070 7269 6e74 2873 656c 662e 7461     print(self.ta
-0000c4c0: 755f 6761 7329 0a0a 0a64 6566 2072 6561  u_gas)...def rea
-0000c4d0: 645f 3144 5f73 6c61 6228 6d6f 6465 6c5f  d_1D_slab(model_
-0000c4e0: 7061 7468 3d27 536c 6162 5265 7375 6c74  path='SlabResult
-0000c4f0: 732e 6669 7473 2e67 7a27 2c76 6572 626f  s.fits.gz',verbo
-0000c500: 7365 3d54 7275 6529 3a0a 2020 2020 2222  se=True):.    ""
-0000c510: 220a 2020 2020 4675 6e63 7469 6f6e 2074  ".    Function t
-0000c520: 6f20 7265 6164 2031 4420 7072 6f64 696d  o read 1D prodim
-0000c530: 6f20 736c 6162 206d 6f64 656c 206f 7574  o slab model out
-0000c540: 7075 740a 2020 2020 2222 220a 2020 2020  put.    """.    
-0000c550: 6966 2076 6572 626f 7365 3a20 7072 696e  if verbose: prin
-0000c560: 7428 2252 6561 6469 6e67 2031 4420 736c  t("Reading 1D sl
-0000c570: 6162 206d 6f64 656c 206f 7574 7075 7420  ab model output 
-0000c580: 6672 6f6d 3a20 222c 6d6f 6465 6c5f 7061  from: ",model_pa
-0000c590: 7468 290a 2020 2020 6966 2027 2e66 6974  th).    if '.fit
-0000c5a0: 732e 677a 2720 696e 206d 6f64 656c 5f70  s.gz' in model_p
-0000c5b0: 6174 683a 0a20 2020 2020 2020 2068 6475  ath:.        hdu
-0000c5c0: 6c3d 6669 7473 2e6f 7065 6e28 6d6f 6465  l=fits.open(mode
-0000c5d0: 6c5f 7061 7468 290a 2020 2020 2020 2020  l_path).        
-0000c5e0: 6461 7461 3d73 6c61 6231 4428 290a 2020  data=slab1D().  
-0000c5f0: 2020 2020 2020 6461 7461 2e64 6972 6563        data.direc
-0000c600: 746f 7279 3d6d 6f64 656c 5f70 6174 680a  tory=model_path.
-0000c610: 2020 2020 2020 2020 6461 7461 2e66 6c75          data.flu
-0000c620: 783d 6864 756c 5b30 5d2e 6461 7461 2e54  x=hdul[0].data.T
-0000c630: 5b3a 2c31 5d0a 2020 2020 2020 2020 6461  [:,1].        da
-0000c640: 7461 2e66 7265 7175 656e 6379 3d68 6475  ta.frequency=hdu
-0000c650: 6c5b 305d 2e64 6174 612e 545b 3a2c 305d  l[0].data.T[:,0]
-0000c660: 0a20 2020 2020 2020 2064 6174 612e 4e73  .        data.Ns
-0000c670: 7065 6369 6573 3d68 6475 6c5b 305d 2e68  pecies=hdul[0].h
-0000c680: 6561 6465 725b 274e 5350 4543 4945 5327  eader['NSPECIES'
-0000c690: 5d0a 2020 2020 2020 2020 6461 7461 2e73  ].        data.s
-0000c6a0: 7065 6369 6573 3d68 6475 6c5b 305d 2e68  pecies=hdul[0].h
-0000c6b0: 6561 6465 722e 636f 6d6d 656e 7473 5b27  eader.comments['
-0000c6c0: 4e53 5045 4349 4553 275d 2e73 706c 6974  NSPECIES'].split
-0000c6d0: 2827 2c27 290a 2020 2020 2020 2020 6461  (',').        da
-0000c6e0: 7461 2e4e 6772 6964 3d68 6475 6c5b 305d  ta.Ngrid=hdul[0]
-0000c6f0: 2e68 6561 6465 725b 274e 4752 4944 275d  .header['NGRID']
-0000c700: 0a20 2020 2020 2020 2064 6174 612e 523d  .        data.R=
-0000c710: 6864 756c 5b30 5d2e 6865 6164 6572 5b27  hdul[0].header['
-0000c720: 525f 4f56 4c50 275d 0a20 2020 2020 2020  R_OVLP'].       
-0000c730: 2069 6620 2828 392b 6461 7461 2e4e 7370   if ((9+data.Nsp
-0000c740: 6563 6965 732a 3229 2c64 6174 612e 4e67  ecies*2),data.Ng
-0000c750: 7269 6429 3d3d 6864 756c 5b31 5d2e 6461  rid)==hdul[1].da
-0000c760: 7461 2e54 2e73 6861 7065 3a0a 2020 2020  ta.T.shape:.    
-0000c770: 2020 2020 2020 2020 6772 6964 3d68 6475          grid=hdu
-0000c780: 6c5b 315d 2e64 6174 610a 2020 2020 2020  l[1].data.      
-0000c790: 2020 2020 2020 6461 7461 2e67 7269 645b        data.grid[
-0000c7a0: 2764 7a27 5d3d 6772 6964 5b3a 2c30 5d0a  'dz']=grid[:,0].
-0000c7b0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-0000c7c0: 2e67 7269 645b 2776 7475 7262 275d 3d67  .grid['vturb']=g
-0000c7d0: 7269 645b 3a2c 315d 0a20 2020 2020 2020  rid[:,1].       
-0000c7e0: 2020 2020 2064 6174 612e 6772 6964 5b27       data.grid['
-0000c7f0: 6e64 275d 3d67 7269 645b 3a2c 325d 0a20  nd']=grid[:,2]. 
-0000c800: 2020 2020 2020 2020 2020 2064 6174 612e             data.
-0000c810: 6772 6964 5b27 5464 275d 3d67 7269 645b  grid['Td']=grid[
-0000c820: 3a2c 335d 0a20 2020 2020 2020 2020 2020  :,3].           
-0000c830: 2064 6174 612e 6772 6964 5b27 6e48 3227   data.grid['nH2'
-0000c840: 5d3d 6772 6964 5b3a 2c34 5d0a 2020 2020  ]=grid[:,4].    
-0000c850: 2020 2020 2020 2020 6461 7461 2e67 7269          data.gri
-0000c860: 645b 276e 4849 275d 3d67 7269 645b 3a2c  d['nHI']=grid[:,
-0000c870: 355d 0a20 2020 2020 2020 2020 2020 2064  5].            d
-0000c880: 6174 612e 6772 6964 5b27 6e48 4949 275d  ata.grid['nHII']
-0000c890: 3d67 7269 645b 3a2c 365d 0a20 2020 2020  =grid[:,6].     
-0000c8a0: 2020 2020 2020 2064 6174 612e 6772 6964         data.grid
-0000c8b0: 5b27 6e48 6527 5d3d 6772 6964 5b3a 2c37  ['nHe']=grid[:,7
-0000c8c0: 5d0a 2020 2020 2020 2020 2020 2020 6461  ].            da
-0000c8d0: 7461 2e67 7269 645b 276e 656c 6563 275d  ta.grid['nelec']
-0000c8e0: 3d67 7269 645b 3a2c 385d 0a20 2020 2020  =grid[:,8].     
-0000c8f0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-0000c900: 7261 6e67 6528 6461 7461 2e4e 7370 6563  range(data.Nspec
-0000c910: 6965 7329 3a0a 2020 2020 2020 2020 2020  ies):.          
-0000c920: 2020 2020 2020 6b65 793d 276e 272b 6461        key='n'+da
-0000c930: 7461 2e73 7065 6369 6573 5b69 5d0a 2020  ta.species[i].  
-0000c940: 2020 2020 2020 2020 2020 2020 2020 6461                da
-0000c950: 7461 2e67 7269 645b 6b65 795d 3d67 7269  ta.grid[key]=gri
-0000c960: 645b 3a2c 392b 695d 0a20 2020 2020 2020  d[:,9+i].       
-0000c970: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-0000c980: 6e67 6528 6461 7461 2e4e 7370 6563 6965  nge(data.Nspecie
-0000c990: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-0000c9a0: 2020 2020 6b65 793d 2754 675f 272b 6461      key='Tg_'+da
-0000c9b0: 7461 2e73 7065 6369 6573 5b69 5d0a 2020  ta.species[i].  
-0000c9c0: 2020 2020 2020 2020 2020 2020 2020 6461                da
-0000c9d0: 7461 2e67 7269 645b 6b65 795d 3d67 7269  ta.grid[key]=gri
-0000c9e0: 645b 3a2c 392b 6461 7461 2e4e 7370 6563  d[:,9+data.Nspec
-0000c9f0: 6965 732b 695d 0a20 2020 2020 2020 2065  ies+i].        e
-0000ca00: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000ca10: 2072 6169 7365 2041 7373 6572 7469 6f6e   raise Assertion
-0000ca20: 4572 726f 7228 2747 7269 6420 696e 206f  Error('Grid in o
-0000ca30: 7574 7075 7420 6669 6c65 2064 6f65 7320  utput file does 
-0000ca40: 6e6f 7420 6d61 7463 6820 7468 6520 6163  not match the ac
-0000ca50: 7475 616c 2067 7269 6420 6f75 7470 7574  tual grid output
-0000ca60: 2061 7272 6179 2729 0a0a 2020 2020 2020   array')..      
-0000ca70: 2020 6966 2028 6c65 6e28 6461 7461 2e66    if (len(data.f
-0000ca80: 7265 7175 656e 6379 292c 6461 7461 2e4e  requency),data.N
-0000ca90: 6772 6964 293d 3d68 6475 6c5b 325d 2e64  grid)==hdul[2].d
-0000caa0: 6174 612e 542e 7368 6170 653a 0a20 2020  ata.T.shape:.   
-0000cab0: 2020 2020 2020 2020 2064 6174 612e 736f           data.so
-0000cac0: 7572 6365 5f66 756e 6374 696f 6e3d 6864  urce_function=hd
-0000cad0: 756c 5b32 5d2e 6461 7461 0a20 2020 2020  ul[2].data.     
-0000cae0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000caf0: 2020 2020 2072 6169 7365 2041 7373 6572       raise Asser
-0000cb00: 7469 6f6e 4572 726f 7228 2753 6f75 7263  tionError('Sourc
-0000cb10: 6520 6675 6e63 7469 6f6e 2067 7269 6420  e function grid 
-0000cb20: 696e 206f 7574 7075 7420 6669 6c65 2064  in output file d
-0000cb30: 6f65 7320 6e6f 7420 6d61 7463 6820 7468  oes not match th
-0000cb40: 6520 7370 6174 6961 6c20 616e 6420 6672  e spatial and fr
-0000cb50: 6571 7565 6e63 7920 6772 6964 2073 697a  equency grid siz
-0000cb60: 6527 290a 0a20 2020 2020 2020 2069 6620  e')..        if 
-0000cb70: 286c 656e 2864 6174 612e 6672 6571 7565  (len(data.freque
-0000cb80: 6e63 7929 2c64 6174 612e 4e67 7269 6429  ncy),data.Ngrid)
-0000cb90: 3d3d 6864 756c 5b33 5d2e 6461 7461 2e54  ==hdul[3].data.T
-0000cba0: 2e73 6861 7065 3a0a 2020 2020 2020 2020  .shape:.        
-0000cbb0: 2020 2020 6461 7461 2e73 6f75 7263 655f      data.source_
-0000cbc0: 6675 6e63 7469 6f6e 5f67 6173 3d68 6475  function_gas=hdu
-0000cbd0: 6c5b 335d 2e64 6174 610a 2020 2020 2020  l[3].data.      
-0000cbe0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000cbf0: 2020 2020 7261 6973 6520 4173 7365 7274      raise Assert
-0000cc00: 696f 6e45 7272 6f72 2827 4761 7320 736f  ionError('Gas so
-0000cc10: 7572 6365 2066 756e 6374 696f 6e20 6772  urce function gr
-0000cc20: 6964 2069 6e20 6f75 7470 7574 2066 696c  id in output fil
-0000cc30: 6520 646f 6573 206e 6f74 206d 6174 6368  e does not match
-0000cc40: 2074 6865 2073 7061 7469 616c 2061 6e64   the spatial and
-0000cc50: 2066 7265 7175 656e 6379 2067 7269 6420   frequency grid 
-0000cc60: 7369 7a65 2729 0a0a 2020 2020 2020 2020  size')..        
-0000cc70: 6966 2028 6c65 6e28 6461 7461 2e66 7265  if (len(data.fre
-0000cc80: 7175 656e 6379 292c 6461 7461 2e4e 6772  quency),data.Ngr
-0000cc90: 6964 293d 3d68 6475 6c5b 345d 2e64 6174  id)==hdul[4].dat
-0000cca0: 612e 542e 7368 6170 653a 0a20 2020 2020  a.T.shape:.     
-0000ccb0: 2020 2020 2020 2064 6174 612e 7461 755f         data.tau_
-0000ccc0: 6475 7374 3d68 6475 6c5b 345d 2e64 6174  dust=hdul[4].dat
-0000ccd0: 610a 2020 2020 2020 2020 656c 7365 3a0a  a.        else:.
-0000cce0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0000ccf0: 6520 4173 7365 7274 696f 6e45 7272 6f72  e AssertionError
-0000cd00: 2827 4475 7374 206f 7074 6963 616c 2064  ('Dust optical d
-0000cd10: 6570 7468 2067 7269 6420 696e 206f 7574  epth grid in out
-0000cd20: 7075 7420 6669 6c65 2064 6f65 7320 6e6f  put file does no
-0000cd30: 7420 6d61 7463 6820 7468 6520 7370 6174  t match the spat
-0000cd40: 6961 6c20 616e 6420 6672 6571 7565 6e63  ial and frequenc
-0000cd50: 7920 6772 6964 2073 697a 6527 290a 0a20  y grid size').. 
-0000cd60: 2020 2020 2020 2069 6620 286c 656e 2864         if (len(d
-0000cd70: 6174 612e 6672 6571 7565 6e63 7929 2c64  ata.frequency),d
-0000cd80: 6174 612e 4e67 7269 6429 3d3d 6864 756c  ata.Ngrid)==hdul
-0000cd90: 5b35 5d2e 6461 7461 2e54 2e73 6861 7065  [5].data.T.shape
-0000cda0: 3a0a 2020 2020 2020 2020 2020 2020 6461  :.            da
-0000cdb0: 7461 2e74 6175 5f67 6173 3d68 6475 6c5b  ta.tau_gas=hdul[
-0000cdc0: 355d 2e64 6174 610a 2020 2020 2020 2020  5].data.        
-0000cdd0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000cde0: 2020 7261 6973 6520 4173 7365 7274 696f    raise Assertio
-0000cdf0: 6e45 7272 6f72 2827 4761 7320 6f70 7469  nError('Gas opti
-0000ce00: 6361 6c20 6465 7074 6820 6772 6964 2069  cal depth grid i
-0000ce10: 6e20 6f75 7470 7574 2066 696c 6520 646f  n output file do
-0000ce20: 6573 206e 6f74 206d 6174 6368 2074 6865  es not match the
-0000ce30: 2073 7061 7469 616c 2061 6e64 2066 7265   spatial and fre
-0000ce40: 7175 656e 6379 2067 7269 6420 7369 7a65  quency grid size
-0000ce50: 2729 0a20 2020 2065 6c73 653a 0a20 2020  ').    else:.   
-0000ce60: 2020 2020 2064 6174 615f 7265 6164 3d6e       data_read=n
-0000ce70: 702e 6c6f 6164 7478 7428 6d6f 6465 6c5f  p.loadtxt(model_
-0000ce80: 7061 7468 2c73 6b69 7072 6f77 733d 3129  path,skiprows=1)
-0000ce90: 0a20 2020 2020 2020 2064 6174 613d 736c  .        data=sl
-0000cea0: 6162 3144 2829 0a20 2020 2020 2020 2064  ab1D().        d
-0000ceb0: 6174 612e 6469 7265 6374 6f72 793d 6d6f  ata.directory=mo
-0000cec0: 6465 6c5f 7061 7468 0a20 2020 2020 2020  del_path.       
-0000ced0: 2064 6174 612e 666c 7578 3d64 6174 615f   data.flux=data_
-0000cee0: 7265 6164 5b3a 2c31 5d0a 2020 2020 2020  read[:,1].      
-0000cef0: 2020 6461 7461 2e66 7265 7175 656e 6379    data.frequency
-0000cf00: 3d64 6174 615f 7265 6164 5b3a 2c30 5d0a  =data_read[:,0].
-0000cf10: 2020 2020 7265 7475 726e 2864 6174 6129      return(data)
-0000cf20: 0a0a 0a64 6566 2072 6561 645f 736c 6162  ...def read_slab
-0000cf30: 286d 6f64 656c 5f70 6174 683d 2753 6c61  (model_path='Sla
-0000cf40: 6252 6573 756c 7473 2e6f 7574 272c 7665  bResults.out',ve
-0000cf50: 7262 6f73 653d 5472 7565 2c73 686f 7274  rbose=True,short
-0000cf60: 5f66 6f72 6d61 743d 4661 6c73 652c 6f76  _format=False,ov
-0000cf70: 6572 6c61 705f 6d6f 6465 6c3d 4661 6c73  erlap_model=Fals
-0000cf80: 6529 3a0a 2020 2020 2222 220a 2020 2020  e):.    """.    
-0000cf90: 4675 6e63 7469 6f6e 2074 6f20 7265 6164  Function to read
-0000cfa0: 2073 6c61 6220 6d6f 6465 6c20 6f75 7470   slab model outp
-0000cfb0: 7574 0a20 2020 2022 2222 0a20 2020 2069  ut.    """.    i
-0000cfc0: 6620 6973 696e 7374 616e 6365 286d 6f64  f isinstance(mod
-0000cfd0: 656c 5f70 6174 682c 6c69 7374 293a 0a20  el_path,list):. 
-0000cfe0: 2020 2020 2020 2064 6174 613d 736c 6162         data=slab
-0000cff0: 5f64 6174 6128 290a 2020 2020 2020 2020  _data().        
-0000d000: 6461 7461 2e64 6972 6563 746f 7279 3d6d  data.directory=m
-0000d010: 6f64 656c 5f70 6174 680a 2020 2020 2020  odel_path.      
-0000d020: 2020 666f 7220 6920 696e 206d 6f64 656c    for i in model
-0000d030: 5f70 6174 683a 0a20 2020 2020 2020 2020  _path:.         
-0000d040: 2020 2072 6461 7461 3d72 6561 645f 736c     rdata=read_sl
-0000d050: 6162 2869 2c76 6572 626f 7365 3d76 6572  ab(i,verbose=ver
-0000d060: 626f 7365 2c73 686f 7274 5f66 6f72 6d61  bose,short_forma
-0000d070: 743d 7368 6f72 745f 666f 726d 6174 290a  t=short_format).
-0000d080: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000d090: 6a20 696e 2072 616e 6765 2872 6461 7461  j in range(rdata
-0000d0a0: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
-0000d0b0: 2020 2020 2020 2020 2020 2064 6174 612e             data.
-0000d0c0: 6164 645f 6d6f 6465 6c28 7264 6174 612e  add_model(rdata.
-0000d0d0: 6d6f 6465 6c73 5b6a 5d29 0a20 2020 2020  models[j]).     
-0000d0e0: 2020 2072 6574 7572 6e28 6461 7461 290a     return(data).
-0000d0f0: 2020 2020 0a20 2020 2069 6620 6f76 6572      .    if over
-0000d100: 6c61 705f 6d6f 6465 6c3a 2072 6574 7572  lap_model: retur
-0000d110: 6e28 7265 6164 5f6f 7665 726c 6170 5f73  n(read_overlap_s
-0000d120: 7065 6374 7261 2870 6174 683d 6d6f 6465  pectra(path=mode
-0000d130: 6c5f 7061 7468 2c76 6572 626f 7365 3d76  l_path,verbose=v
-0000d140: 6572 626f 7365 2929 0a20 2020 200a 2020  erbose)).    .  
-0000d150: 2020 6966 2076 6572 626f 7365 3a20 7072    if verbose: pr
-0000d160: 696e 7428 2252 6561 6469 6e67 2073 6c61  int("Reading sla
-0000d170: 6220 6d6f 6465 6c20 6f75 7470 7574 2066  b model output f
-0000d180: 726f 6d3a 2022 2c6d 6f64 656c 5f70 6174  rom: ",model_pat
-0000d190: 6829 0a20 2020 2066 3d6f 7065 6e28 6d6f  h).    f=open(mo
-0000d1a0: 6465 6c5f 7061 7468 290a 2020 2020 6461  del_path).    da
-0000d1b0: 7461 3d73 6c61 625f 6461 7461 2829 0a20  ta=slab_data(). 
-0000d1c0: 2020 206e 6d6f 6465 6c73 3d69 6e74 2866     nmodels=int(f
-0000d1d0: 2e72 6561 646c 696e 6528 292e 7370 6c69  .readline().spli
-0000d1e0: 7428 295b 305d 290a 2020 2020 6461 7461  t()[0]).    data
-0000d1f0: 2e64 6972 6563 746f 7279 3d6d 6f64 656c  .directory=model
-0000d200: 5f70 6174 680a 2020 2020 666f 7220 6920  _path.    for i 
-0000d210: 696e 2072 616e 6765 286e 6d6f 6465 6c73  in range(nmodels
-0000d220: 293a 0a23 2020 2020 2020 2020 2074 656d  ):.#         tem
-0000d230: 706f 2020 2020 2020 2020 2020 2020 2020  po              
-0000d240: 2020 3d20 2020 736c 6162 2829 0a20 2020    =   slab().   
-0000d250: 2020 2020 2074 656d 706f 5f6d 6f64 656c       tempo_model
-0000d260: 5f6e 756d 6265 723d 696e 7428 662e 7265  _number=int(f.re
-0000d270: 6164 6c69 6e65 2829 2e73 706c 6974 2829  adline().split()
-0000d280: 5b30 5d29 0a20 2020 2020 2020 206e 7370  [0]).        nsp
-0000d290: 6563 6965 733d 696e 7428 662e 7265 6164  ecies=int(f.read
-0000d2a0: 6c69 6e65 2829 2e73 706c 6974 2829 5b30  line().split()[0
-0000d2b0: 5d29 0a23 2020 2020 2020 2020 2074 656d  ]).#         tem
-0000d2c0: 706f 2e73 7065 6369 6573 5f6e 756d 6265  po.species_numbe
-0000d2d0: 7220 3d20 2020 696e 7428 662e 7265 6164  r =   int(f.read
-0000d2e0: 6c69 6e65 2829 2e73 706c 6974 2829 5b30  line().split()[0
-0000d2f0: 5d29 0a20 2020 2020 2020 2074 656d 706f  ]).        tempo
-0000d300: 5f6e 4874 6f74 3d66 6c6f 6174 2866 2e72  _nHtot=float(f.r
-0000d310: 6561 646c 696e 6528 292e 7370 6c69 7428  eadline().split(
-0000d320: 295b 305d 290a 2020 2020 2020 2020 7465  )[0]).        te
-0000d330: 6d70 6f5f 6761 7344 656e 733d 666c 6f61  mpo_gasDens=floa
-0000d340: 7428 662e 7265 6164 6c69 6e65 2829 2e73  t(f.readline().s
-0000d350: 706c 6974 2829 5b30 5d29 0a20 2020 2020  plit()[0]).     
-0000d360: 2020 2074 656d 706f 5f6e 656c 6563 3d66     tempo_nelec=f
-0000d370: 6c6f 6174 2866 2e72 6561 646c 696e 6528  loat(f.readline(
-0000d380: 292e 7370 6c69 7428 295b 305d 290a 2020  ).split()[0]).  
-0000d390: 2020 2020 2020 7465 6d70 6f5f 6e48 653d        tempo_nHe=
-0000d3a0: 666c 6f61 7428 662e 7265 6164 6c69 6e65  float(f.readline
-0000d3b0: 2829 2e73 706c 6974 2829 5b30 5d29 0a20  ().split()[0]). 
-0000d3c0: 2020 2020 2020 2074 656d 706f 5f6e 4849         tempo_nHI
-0000d3d0: 493d 666c 6f61 7428 662e 7265 6164 6c69  I=float(f.readli
-0000d3e0: 6e65 2829 2e73 706c 6974 2829 5b30 5d29  ne().split()[0])
-0000d3f0: 0a20 2020 2020 2020 2074 656d 706f 5f6e  .        tempo_n
-0000d400: 4849 3d66 6c6f 6174 2866 2e72 6561 646c  HI=float(f.readl
-0000d410: 696e 6528 292e 7370 6c69 7428 295b 305d  ine().split()[0]
-0000d420: 290a 2020 2020 2020 2020 7465 6d70 6f5f  ).        tempo_
-0000d430: 6e48 323d 666c 6f61 7428 662e 7265 6164  nH2=float(f.read
-0000d440: 6c69 6e65 2829 2e73 706c 6974 2829 5b30  line().split()[0
-0000d450: 5d29 0a20 2020 2020 2020 2074 656d 706f  ]).        tempo
-0000d460: 5f64 7573 745f 746f 5f67 6173 3d66 6c6f  _dust_to_gas=flo
-0000d470: 6174 2866 2e72 6561 646c 696e 6528 292e  at(f.readline().
-0000d480: 7370 6c69 7428 295b 305d 290a 2020 2020  split()[0]).    
-0000d490: 2020 2020 7465 6d70 6f5f 7674 7572 623d      tempo_vturb=
-0000d4a0: 666c 6f61 7428 662e 7265 6164 6c69 6e65  float(f.readline
-0000d4b0: 2829 2e73 706c 6974 2829 5b30 5d29 0a20  ().split()[0]). 
-0000d4c0: 2020 2020 2020 2074 656d 706f 5f54 673d         tempo_Tg=
-0000d4d0: 666c 6f61 7428 662e 7265 6164 6c69 6e65  float(f.readline
-0000d4e0: 2829 2e73 706c 6974 2829 5b30 5d29 0a20  ().split()[0]). 
-0000d4f0: 2020 2020 2020 2074 656d 706f 5f54 643d         tempo_Td=
-0000d500: 666c 6f61 7428 662e 7265 6164 6c69 6e65  float(f.readline
-0000d510: 2829 2e73 706c 6974 2829 5b30 5d29 0a20  ().split()[0]). 
-0000d520: 2020 2020 2020 2069 6620 7368 6f72 745f         if short_
-0000d530: 666f 726d 6174 3a0a 2020 2020 2020 2020  format:.        
-0000d540: 2020 2020 666f 7220 6a20 696e 2072 616e      for j in ran
-0000d550: 6765 286e 7370 6563 6965 7329 3a0a 2020  ge(nspecies):.  
-0000d560: 2020 2020 2020 2020 2020 2020 2020 7465                te
-0000d570: 6d70 6f3d 736c 6162 2829 0a20 2020 2020  mpo=slab().     
-0000d580: 2020 2020 2020 2020 2020 2074 656d 706f             tempo
-0000d590: 2e6d 6f64 656c 5f6e 756d 6265 723d 7465  .model_number=te
-0000d5a0: 6d70 6f5f 6d6f 6465 6c5f 6e75 6d62 6572  mpo_model_number
-0000d5b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d5c0: 2074 656d 706f 2e4e 483d 7465 6d70 6f5f   tempo.NH=tempo_
-0000d5d0: 6e48 746f 740a 2020 2020 2020 2020 2020  nHtot.          
-0000d5e0: 2020 2020 2020 7465 6d70 6f2e 6e43 6f6c        tempo.nCol
-0000d5f0: 6c3d 7465 6d70 6f5f 6761 7344 656e 730a  l=tempo_gasDens.
-0000d600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d610: 7465 6d70 6f2e 6e65 3d74 656d 706f 5f6e  tempo.ne=tempo_n
-0000d620: 656c 6563 0a20 2020 2020 2020 2020 2020  elec.           
-0000d630: 2020 2020 2074 656d 706f 2e6e 4865 3d74       tempo.nHe=t
-0000d640: 656d 706f 5f6e 4865 0a20 2020 2020 2020  empo_nHe.       
-0000d650: 2020 2020 2020 2020 2074 656d 706f 2e6e           tempo.n
-0000d660: 4849 493d 7465 6d70 6f5f 6e48 4949 0a20  HII=tempo_nHII. 
-0000d670: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000d680: 656d 706f 2e6e 4849 3d74 656d 706f 5f6e  empo.nHI=tempo_n
-0000d690: 4849 0a20 2020 2020 2020 2020 2020 2020  HI.             
-0000d6a0: 2020 2074 656d 706f 2e6e 4832 3d74 656d     tempo.nH2=tem
-0000d6b0: 706f 5f6e 4832 0a20 2020 2020 2020 2020  po_nH2.         
-0000d6c0: 2020 2020 2020 2074 656d 706f 2e64 7573         tempo.dus
-0000d6d0: 745f 746f 5f67 6173 3d74 656d 706f 5f64  t_to_gas=tempo_d
-0000d6e0: 7573 745f 746f 5f67 6173 0a20 2020 2020  ust_to_gas.     
-0000d6f0: 2020 2020 2020 2020 2020 2074 656d 706f             tempo
-0000d700: 2e76 7475 7262 3d74 656d 706f 5f76 7475  .vturb=tempo_vtu
-0000d710: 7262 0a20 2020 2020 2020 2020 2020 2020  rb.             
-0000d720: 2020 2074 656d 706f 2e54 673d 7465 6d70     tempo.Tg=temp
-0000d730: 6f5f 5467 0a20 2020 2020 2020 2020 2020  o_Tg.           
-0000d740: 2020 2020 2074 656d 706f 2e54 643d 7465       tempo.Td=te
-0000d750: 6d70 6f5f 5464 0a0a 2020 2020 2020 2020  mpo_Td..        
-0000d760: 2020 2020 2020 2020 7465 6d70 6f2e 7370          tempo.sp
-0000d770: 6563 6965 735f 696e 6465 783d 696e 7428  ecies_index=int(
-0000d780: 662e 7265 6164 6c69 6e65 2829 2e73 706c  f.readline().spl
-0000d790: 6974 2829 5b30 5d29 0a20 2020 2020 2020  it()[0]).       
-0000d7a0: 2020 2020 2020 2020 2074 656d 706f 2e73           tempo.s
-0000d7b0: 7065 6369 6573 5f6e 756d 6265 723d 6a2b  pecies_number=j+
-0000d7c0: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
-0000d7d0: 2020 7465 6d70 6f2e 7370 6563 6965 735f    tempo.species_
-0000d7e0: 6e61 6d65 3d66 2e72 6561 646c 696e 6528  name=f.readline(
-0000d7f0: 292e 7370 6c69 7428 295b 305d 0a20 2020  ).split()[0].   
-0000d800: 2020 2020 2020 2020 2020 2020 2074 656d               tem
-0000d810: 706f 2e61 6275 6e64 616e 6365 3d66 6c6f  po.abundance=flo
-0000d820: 6174 2866 2e72 6561 646c 696e 6528 292e  at(f.readline().
-0000d830: 7370 6c69 7428 295b 305d 290a 2020 2020  split()[0]).    
-0000d840: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-0000d850: 6f2e 6476 3d66 6c6f 6174 2866 2e72 6561  o.dv=float(f.rea
-0000d860: 646c 696e 6528 292e 7370 6c69 7428 295b  dline().split()[
-0000d870: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
-0000d880: 2020 2020 7465 6d70 6f2e 6e6c 696e 6573      tempo.nlines
-0000d890: 3d69 6e74 2866 2e72 6561 646c 696e 6528  =int(f.readline(
-0000d8a0: 292e 7370 6c69 7428 295b 305d 290a 2020  ).split()[0]).  
-0000d8b0: 2020 2020 2020 2020 2020 2020 2020 6c69                li
-0000d8c0: 6e65 733d 662e 7265 6164 6c69 6e65 2829  nes=f.readline()
-0000d8d0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d8e0: 2020 2320 7465 6d70 6f2e 6e6c 696e 6573    # tempo.nlines
-0000d8f0: 3d4e 6f6e 650a 2020 2020 2020 2020 2020  =None.          
-0000d900: 2020 2020 2020 7465 6d70 6f2e 6c69 6e65        tempo.line
-0000d910: 6461 7461 3d4e 6f6e 650a 2020 2020 2020  data=None.      
-0000d920: 2020 2020 2020 2020 2020 7465 6d70 6f2e            tempo.
-0000d930: 6c65 7665 6c64 6174 613d 4e6f 6e65 0a20  leveldata=None. 
-0000d940: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000d950: 656d 706f 2e63 6f6e 7657 6176 656c 656e  empo.convWavelen
-0000d960: 6774 683d 4e6f 6e65 0a20 2020 2020 2020  gth=None.       
-0000d970: 2020 2020 2020 2020 2074 656d 706f 2e63           tempo.c
-0000d980: 6f6e 764c 5445 666c 7578 3d4e 6f6e 650a  onvLTEflux=None.
-0000d990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9a0: 7465 6d70 6f2e 636f 6e76 4e4c 5445 666c  tempo.convNLTEfl
-0000d9b0: 7578 3d4e 6f6e 650a 2020 2020 2020 2020  ux=None.        
-0000d9c0: 2020 2020 2020 2020 7465 6d70 6f2e 636f          tempo.co
-0000d9d0: 6e76 5479 7065 3d4e 6f6e 650a 2020 2020  nvType=None.    
-0000d9e0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-0000d9f0: 6f2e 636f 6e76 523d 4e6f 6e65 0a0a 2020  o.convR=None..  
-0000da00: 2020 2020 2020 2020 2020 2020 2020 6461                da
-0000da10: 743d 5b5d 0a20 2020 2020 2020 2020 2020  t=[].           
-0000da20: 2020 2020 2023 2066 6f72 206b 2069 6e20       # for k in 
-0000da30: 7261 6e67 6528 7465 6d70 6f2e 6e6c 6576  range(tempo.nlev
-0000da40: 656c 7329 3a0a 2020 2020 2020 2020 2020  els):.          
-0000da50: 2020 2020 2020 2320 2020 2020 6461 745b        #     dat[
-0000da60: 305d 5b6b 2c3a 5d3d 6e70 2e61 7361 7272  0][k,:]=np.asarr
-0000da70: 6179 285b 666c 6f61 7428 7829 2066 6f72  ay([float(x) for
-0000da80: 2078 2069 6e20 662e 7265 6164 6c69 6e65   x in f.readline
-0000da90: 2829 2e73 706c 6974 2829 5d29 0a0a 2020  ().split()])..  
-0000daa0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000dab0: 6c69 6e65 733d 662e 7265 6164 6c69 6e65  lines=f.readline
-0000dac0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-0000dad0: 2020 2023 206c 696e 6573 3d66 2e72 6561     # lines=f.rea
-0000dae0: 646c 696e 6528 290a 2020 2020 2020 2020  dline().        
-0000daf0: 2020 2020 2020 2020 6461 743d 6e70 2e7a          dat=np.z
-0000db00: 6572 6f73 2828 7465 6d70 6f2e 6e6c 696e  eros((tempo.nlin
-0000db10: 6573 2c34 2929 0a20 2020 2020 2020 2020  es,4)).         
-0000db20: 2020 2020 2020 2073 6c61 624f 7574 466f         slabOutFo
-0000db30: 726d 6174 3d5b 382c 3134 2c31 352c 3135  rmat=[8,14,15,15
-0000db40: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0000db50: 2020 666f 7220 6b20 696e 2072 616e 6765    for k in range
-0000db60: 2874 656d 706f 2e6e 6c69 6e65 7329 3a0a  (tempo.nlines):.
-0000db70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db80: 2020 2020 6c69 6e65 5265 6164 3d5b 5d0a      lineRead=[].
-0000db90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dba0: 2020 2020 6c69 6e65 733d 662e 7265 6164      lines=f.read
-0000dbb0: 6c69 6e65 2829 0a20 2020 2020 2020 2020  line().         
-0000dbc0: 2020 2020 2020 2020 2020 206c 3d30 0a20             l=0. 
-0000dbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dbe0: 2020 2066 6f72 206c 656e 6774 6820 696e     for length in
-0000dbf0: 2073 6c61 624f 7574 466f 726d 6174 3a0a   slabOutFormat:.
-0000dc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc10: 2020 2020 2020 2020 6c69 6e65 5265 6164          lineRead
-0000dc20: 2e61 7070 656e 6428 6c69 6e65 735b 6c3a  .append(lines[l:
-0000dc30: 6c2b 6c65 6e67 7468 5d29 0a20 2020 2020  l+length]).     
-0000dc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc50: 2020 206c 2b3d 6c65 6e67 7468 0a20 2020     l+=length.   
-0000dc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc70: 2064 6174 5b6b 2c3a 5d3d 6e70 2e61 7361   dat[k,:]=np.asa
-0000dc80: 7272 6179 285b 666c 6f61 7428 7829 2066  rray([float(x) f
-0000dc90: 6f72 2078 2069 6e20 6c69 6e65 5265 6164  or x in lineRead
-0000dca0: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-0000dcb0: 2020 206c 696e 6544 6174 613d 7064 2e44     lineData=pd.D
-0000dcc0: 6174 6146 7261 6d65 2864 6174 2c63 6f6c  ataFrame(dat,col
-0000dcd0: 756d 6e73 3d5b 2769 272c 2747 487a 272c  umns=['i','GHz',
-0000dce0: 2746 4e4c 5445 272c 2746 4c54 4527 5d29  'FNLTE','FLTE'])
-0000dcf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dd00: 2074 656d 706f 2e6c 696e 6564 6174 613d   tempo.linedata=
-0000dd10: 6c69 6e65 4461 7461 0a20 2020 2020 2020  lineData.       
-0000dd20: 2020 2020 2020 2020 2064 6174 612e 6164           data.ad
-0000dd30: 645f 6d6f 6465 6c28 7465 6d70 6f29 0a20  d_model(tempo). 
-0000dd40: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000dd50: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
-0000dd60: 6e20 7261 6e67 6528 6e73 7065 6369 6573  n range(nspecies
-0000dd70: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000dd80: 2020 2074 656d 706f 3d73 6c61 6228 290a     tempo=slab().
-0000dd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dda0: 7465 6d70 6f2e 6d6f 6465 6c5f 6e75 6d62  tempo.model_numb
-0000ddb0: 6572 3d74 656d 706f 5f6d 6f64 656c 5f6e  er=tempo_model_n
-0000ddc0: 756d 6265 720a 2020 2020 2020 2020 2020  umber.          
-0000ddd0: 2020 2020 2020 7465 6d70 6f2e 4e48 3d74        tempo.NH=t
-0000dde0: 656d 706f 5f6e 4874 6f74 0a20 2020 2020  empo_nHtot.     
-0000ddf0: 2020 2020 2020 2020 2020 2074 656d 706f             tempo
-0000de00: 2e6e 436f 6c6c 3d74 656d 706f 5f67 6173  .nColl=tempo_gas
-0000de10: 4465 6e73 0a20 2020 2020 2020 2020 2020  Dens.           
-0000de20: 2020 2020 2074 656d 706f 2e6e 653d 7465       tempo.ne=te
-0000de30: 6d70 6f5f 6e65 6c65 630a 2020 2020 2020  mpo_nelec.      
-0000de40: 2020 2020 2020 2020 2020 7465 6d70 6f2e            tempo.
-0000de50: 6e48 653d 7465 6d70 6f5f 6e48 650a 2020  nHe=tempo_nHe.  
-0000de60: 2020 2020 2020 2020 2020 2020 2020 7465                te
-0000de70: 6d70 6f2e 6e48 4949 3d74 656d 706f 5f6e  mpo.nHII=tempo_n
-0000de80: 4849 490a 2020 2020 2020 2020 2020 2020  HII.            
-0000de90: 2020 2020 7465 6d70 6f2e 6e48 493d 7465      tempo.nHI=te
-0000dea0: 6d70 6f5f 6e48 490a 2020 2020 2020 2020  mpo_nHI.        
-0000deb0: 2020 2020 2020 2020 7465 6d70 6f2e 6e48          tempo.nH
-0000dec0: 323d 7465 6d70 6f5f 6e48 320a 2020 2020  2=tempo_nH2.    
-0000ded0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-0000dee0: 6f2e 6475 7374 5f74 6f5f 6761 733d 7465  o.dust_to_gas=te
-0000def0: 6d70 6f5f 6475 7374 5f74 6f5f 6761 730a  mpo_dust_to_gas.
-0000df00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df10: 7465 6d70 6f2e 7674 7572 623d 7465 6d70  tempo.vturb=temp
-0000df20: 6f5f 7674 7572 620a 2020 2020 2020 2020  o_vturb.        
-0000df30: 2020 2020 2020 2020 7465 6d70 6f2e 5467          tempo.Tg
-0000df40: 3d74 656d 706f 5f54 670a 2020 2020 2020  =tempo_Tg.      
-0000df50: 2020 2020 2020 2020 2020 7465 6d70 6f2e            tempo.
-0000df60: 5464 3d74 656d 706f 5f54 640a 0a20 2020  Td=tempo_Td..   
-0000df70: 2020 2020 2020 2020 2020 2020 2074 656d               tem
-0000df80: 706f 2e73 7065 6369 6573 5f69 6e64 6578  po.species_index
-0000df90: 3d69 6e74 2866 2e72 6561 646c 696e 6528  =int(f.readline(
-0000dfa0: 292e 7370 6c69 7428 295b 305d 290a 2020  ).split()[0]).  
-0000dfb0: 2020 2020 2020 2020 2020 2020 2020 7465                te
-0000dfc0: 6d70 6f2e 7370 6563 6965 735f 6e75 6d62  mpo.species_numb
-0000dfd0: 6572 3d6a 2b31 0a20 2020 2020 2020 2020  er=j+1.         
-0000dfe0: 2020 2020 2020 2074 656d 706f 2e73 7065         tempo.spe
-0000dff0: 6369 6573 5f6e 616d 653d 662e 7265 6164  cies_name=f.read
-0000e000: 6c69 6e65 2829 2e73 706c 6974 2829 5b30  line().split()[0
-0000e010: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0000e020: 2020 7465 6d70 6f2e 6162 756e 6461 6e63    tempo.abundanc
-0000e030: 653d 666c 6f61 7428 662e 7265 6164 6c69  e=float(f.readli
-0000e040: 6e65 2829 2e73 706c 6974 2829 5b30 5d29  ne().split()[0])
-0000e050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e060: 2074 656d 706f 2e64 763d 666c 6f61 7428   tempo.dv=float(
-0000e070: 662e 7265 6164 6c69 6e65 2829 2e73 706c  f.readline().spl
-0000e080: 6974 2829 5b30 5d29 0a20 2020 2020 2020  it()[0]).       
-0000e090: 2020 2020 2020 2020 2074 656d 706f 2e6e           tempo.n
-0000e0a0: 6c65 7665 6c73 3d69 6e74 2866 2e72 6561  levels=int(f.rea
-0000e0b0: 646c 696e 6528 292e 7370 6c69 7428 295b  dline().split()[
-0000e0c0: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
-0000e0d0: 2020 2020 6c69 6e65 733d 662e 7265 6164      lines=f.read
-0000e0e0: 6c69 6e65 2829 0a0a 2020 2020 2020 2020  line()..        
-0000e0f0: 2020 2020 2020 2020 7465 6d70 6f2e 6e6c          tempo.nl
-0000e100: 696e 6573 3d4e 6f6e 650a 2020 2020 2020  ines=None.      
-0000e110: 2020 2020 2020 2020 2020 7465 6d70 6f2e            tempo.
-0000e120: 6c69 6e65 6461 7461 3d4e 6f6e 650a 2020  linedata=None.  
-0000e130: 2020 2020 2020 2020 2020 2020 2020 7465                te
-0000e140: 6d70 6f2e 6c65 7665 6c64 6174 613d 4e6f  mpo.leveldata=No
-0000e150: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
-0000e160: 2020 2074 656d 706f 2e63 6f6e 7657 6176     tempo.convWav
-0000e170: 656c 656e 6774 683d 4e6f 6e65 0a20 2020  elength=None.   
-0000e180: 2020 2020 2020 2020 2020 2020 2074 656d               tem
-0000e190: 706f 2e63 6f6e 764c 5445 666c 7578 3d4e  po.convLTEflux=N
-0000e1a0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-0000e1b0: 2020 2020 7465 6d70 6f2e 636f 6e76 4e4c      tempo.convNL
-0000e1c0: 5445 666c 7578 3d4e 6f6e 650a 2020 2020  TEflux=None.    
-0000e1d0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-0000e1e0: 6f2e 636f 6e76 5479 7065 3d4e 6f6e 650a  o.convType=None.
-0000e1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e200: 7465 6d70 6f2e 636f 6e76 523d 4e6f 6e65  tempo.convR=None
-0000e210: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000e220: 2020 6461 743d 5b6e 702e 7a65 726f 7328    dat=[np.zeros(
-0000e230: 2874 656d 706f 2e6e 6c65 7665 6c73 2c38  (tempo.nlevels,8
-0000e240: 2929 2c5b 5d2c 5b5d 5d0a 2020 2020 2020  )),[],[]].      
-0000e250: 2020 2020 2020 2020 2020 666f 7220 6b20            for k 
-0000e260: 696e 2072 616e 6765 2874 656d 706f 2e6e  in range(tempo.n
-0000e270: 6c65 7665 6c73 293a 0a20 2020 2020 2020  levels):.       
-0000e280: 2020 2020 2020 2020 2020 2020 2064 6174               dat
-0000e290: 5b30 5d5b 6b2c 3a5d 3d6e 702e 6173 6172  [0][k,:]=np.asar
-0000e2a0: 7261 7928 5b66 6c6f 6174 2878 2920 666f  ray([float(x) fo
-0000e2b0: 7220 7820 696e 2066 2e72 6561 646c 696e  r x in f.readlin
-0000e2c0: 6528 292e 7370 6c69 7428 295d 290a 2020  e().split()]).  
-0000e2d0: 2020 2020 2020 2020 2020 2020 2020 7465                te
-0000e2e0: 6d70 6f2e 6e6c 696e 6573 3d69 6e74 2866  mpo.nlines=int(f
-0000e2f0: 2e72 6561 646c 696e 6528 292e 7370 6c69  .readline().spli
-0000e300: 7428 295b 305d 290a 2020 2020 2020 2020  t()[0]).        
-0000e310: 2020 2020 2020 2020 6c69 6e65 733d 662e          lines=f.
-0000e320: 7265 6164 6c69 6e65 2829 0a20 2020 2020  readline().     
-0000e330: 2020 2020 2020 2020 2020 206c 696e 6573             lines
-0000e340: 3d66 2e72 6561 646c 696e 6528 290a 2020  =f.readline().  
-0000e350: 2020 2020 2020 2020 2020 2020 2020 6461                da
-0000e360: 745b 315d 3d6e 702e 7a65 726f 7328 2874  t[1]=np.zeros((t
-0000e370: 656d 706f 2e6e 6c69 6e65 732c 3233 2929  empo.nlines,23))
+0000b350: 7374 7228 7365 6c66 2e6e 4849 292b 275c  str(self.nHI)+'\
+0000b360: 6e5c 6e27 0a20 2020 2020 2020 206f 7574  n\n'.        out
+0000b370: 7075 742b 3d27 6e48 3220 2020 2020 2020  put+='nH2       
+0000b380: 2020 2020 3d20 270a 2020 2020 2020 2020      = '.        
+0000b390: 6f75 7470 7574 2b3d 7374 7228 7365 6c66  output+=str(self
+0000b3a0: 2e6e 4832 292b 275c 6e5c 6e27 0a20 2020  .nH2)+'\n\n'.   
+0000b3b0: 2020 2020 206f 7574 7075 742b 3d27 6475       output+='du
+0000b3c0: 7374 5f74 6f5f 6761 7320 2020 3d20 270a  st_to_gas   = '.
+0000b3d0: 2020 2020 2020 2020 6f75 7470 7574 2b3d          output+=
+0000b3e0: 7374 7228 7365 6c66 2e64 7573 745f 746f  str(self.dust_to
+0000b3f0: 5f67 6173 292b 275c 6e5c 6e27 0a20 2020  _gas)+'\n\n'.   
+0000b400: 2020 2020 206f 7574 7075 742b 3d27 7674       output+='vt
+0000b410: 7572 6220 2020 2020 2020 2020 3d20 270a  urb         = '.
+0000b420: 2020 2020 2020 2020 6f75 7470 7574 2b3d          output+=
+0000b430: 7374 7228 7365 6c66 2e76 7475 7262 292b  str(self.vturb)+
+0000b440: 275c 6e5c 6e27 0a20 2020 2020 2020 206f  '\n\n'.        o
+0000b450: 7574 7075 742b 3d27 5467 2020 2020 2020  utput+='Tg      
+0000b460: 2020 2020 2020 3d20 270a 2020 2020 2020        = '.      
+0000b470: 2020 6f75 7470 7574 2b3d 7374 7228 7365    output+=str(se
+0000b480: 6c66 2e54 6729 2b27 5c6e 5c6e 270a 2020  lf.Tg)+'\n\n'.  
+0000b490: 2020 2020 2020 6f75 7470 7574 2b3d 2754        output+='T
+0000b4a0: 6420 2020 2020 2020 2020 2020 203d 2027  d            = '
+0000b4b0: 0a20 2020 2020 2020 206f 7574 7075 742b  .        output+
+0000b4c0: 3d73 7472 2873 656c 662e 5464 292b 275c  =str(self.Td)+'\
+0000b4d0: 6e5c 6e27 0a20 2020 2020 2020 206f 7574  n\n'.        out
+0000b4e0: 7075 742b 3d27 7370 6563 6965 735f 6e61  put+='species_na
+0000b4f0: 6d65 2020 203d 2027 0a20 2020 2020 2020  me   = '.       
+0000b500: 206f 7574 7075 742b 3d73 656c 662e 7370   output+=self.sp
+0000b510: 6563 6965 735f 6e61 6d65 2b27 5c6e 5c6e  ecies_name+'\n\n
+0000b520: 270a 2020 2020 2020 2020 6f75 7470 7574  '.        output
+0000b530: 2b3d 2761 6275 6e64 616e 6365 2020 2020  +='abundance    
+0000b540: 203d 2027 0a20 2020 2020 2020 206f 7574   = '.        out
+0000b550: 7075 742b 3d73 7472 2873 656c 662e 6162  put+=str(self.ab
+0000b560: 756e 6461 6e63 6529 2b27 5c6e 5c6e 270a  undance)+'\n\n'.
+0000b570: 2020 2020 2020 2020 6f75 7470 7574 2b3d          output+=
+0000b580: 2764 7620 2020 2020 2020 2020 2020 203d  'dv            =
+0000b590: 2027 0a20 2020 2020 2020 206f 7574 7075   '.        outpu
+0000b5a0: 742b 3d73 7472 2873 656c 662e 6476 292b  t+=str(self.dv)+
+0000b5b0: 275c 6e5c 6e27 0a20 2020 2020 2020 206f  '\n\n'.        o
+0000b5c0: 7574 7075 742b 3d27 6e6c 6576 656c 7320  utput+='nlevels 
+0000b5d0: 2020 2020 2020 3d20 270a 2020 2020 2020        = '.      
+0000b5e0: 2020 6f75 7470 7574 2b3d 7374 7228 7365    output+=str(se
+0000b5f0: 6c66 2e6e 6c65 7665 6c73 292b 275c 6e5c  lf.nlevels)+'\n\
+0000b600: 6e27 0a20 2020 2020 2020 206f 7574 7075  n'.        outpu
+0000b610: 742b 3d27 6e6c 696e 6573 2020 2020 2020  t+='nlines      
+0000b620: 2020 3d20 270a 2020 2020 2020 2020 6f75    = '.        ou
+0000b630: 7470 7574 2b3d 7374 7228 7365 6c66 2e6e  tput+=str(self.n
+0000b640: 6c69 6e65 7329 2b27 5c6e 5c6e 270a 2020  lines)+'\n\n'.  
+0000b650: 2020 2020 2020 6f75 7470 7574 2b3d 2763        output+='c
+0000b660: 6f6e 7654 7970 6520 2020 2020 2020 3d20  onvType       = 
+0000b670: 270a 2020 2020 2020 2020 6f75 7470 7574  '.        output
+0000b680: 2b3d 7374 7228 7365 6c66 2e63 6f6e 7654  +=str(self.convT
+0000b690: 7970 6529 2b27 5c6e 5c6e 270a 2020 2020  ype)+'\n\n'.    
+0000b6a0: 2020 2020 6f75 7470 7574 2b3d 2763 6f6e      output+='con
+0000b6b0: 7652 2020 2020 2020 2020 3d20 270a 2020  vR        = '.  
+0000b6c0: 2020 2020 2020 6f75 7470 7574 2b3d 7374        output+=st
+0000b6d0: 7228 7365 6c66 2e63 6f6e 7652 292b 275c  r(self.convR)+'\
+0000b6e0: 6e5c 6e27 0a20 2020 2020 2020 2072 6574  n\n'.        ret
+0000b6f0: 7572 6e20 6f75 7470 7574 0a0a 2020 2020  urn output..    
+0000b700: 6465 6620 636f 6e76 6f6c 7665 2873 656c  def convolve(sel
+0000b710: 662c 6672 6571 5f62 696e 733d 4e6f 6e65  f,freq_bins=None
+0000b720: 2c52 3d31 2c6c 616d 6264 615f 303d 312c  ,R=1,lambda_0=1,
+0000b730: 6c61 6d62 6461 5f6e 3d31 2c76 723d 3133  lambda_n=1,vr=13
+0000b740: 3030 2c4e 4c54 453d 4661 6c73 652c 636f  00,NLTE=False,co
+0000b750: 6e76 5f74 7970 653d 312c 6f76 6572 6c61  nv_type=1,overla
+0000b760: 703d 4661 6c73 6529 3a0a 2020 2020 2020  p=False):.      
+0000b770: 2020 6966 206f 7665 726c 6170 3a0a 2020    if overlap:.  
+0000b780: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000b790: 6f6e 766f 6c76 655f 6f76 6572 6c61 7028  onvolve_overlap(
+0000b7a0: 523d 522c 6c61 6d62 6461 5f30 3d6c 616d  R=R,lambda_0=lam
+0000b7b0: 6264 615f 302c 6c61 6d62 6461 5f6e 3d6c  bda_0,lambda_n=l
+0000b7c0: 616d 6264 615f 6e29 0a20 2020 2020 2020  ambda_n).       
+0000b7d0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+0000b7e0: 2020 2020 743d 2746 4c54 4527 0a20 2020      t='FLTE'.   
+0000b7f0: 2020 2020 2069 6620 4e4c 5445 3a0a 2020       if NLTE:.  
+0000b800: 2020 2020 2020 2020 2020 743d 2746 4e4c            t='FNL
+0000b810: 5445 270a 2020 2020 2020 2020 6461 3d73  TE'.        da=s
+0000b820: 656c 662e 6c69 6e65 6461 7461 0a20 2020  elf.linedata.   
+0000b830: 2020 2020 2069 6620 6c61 6d62 6461 5f30       if lambda_0
+0000b840: 3d3d 6c61 6d62 6461 5f6e 3a0a 2020 2020  ==lambda_n:.    
+0000b850: 2020 2020 2020 2020 6c61 6d62 6461 5f30          lambda_0
+0000b860: 3d6e 702e 616d 696e 2864 615b 2747 487a  =np.amin(da['GHz
+0000b870: 275d 3e63 2f6c 616d 6264 615f 6e2a 3165  ']>c/lambda_n*1e
+0000b880: 2d33 290a 2020 2020 2020 2020 2020 2020  -3).            
+0000b890: 6c61 6d62 6461 5f6e 3d6e 702e 616d 6178  lambda_n=np.amax
+0000b8a0: 2864 615b 2747 487a 275d 3e63 2f6c 616d  (da['GHz']>c/lam
+0000b8b0: 6264 615f 6e2a 3165 2d33 290a 2020 2020  bda_n*1e-3).    
+0000b8c0: 2020 2020 2020 2020 6c61 6d62 6461 5f30          lambda_0
+0000b8d0: 3d6c 616d 6264 615f 302a 3130 2a2a 2d30  =lambda_0*10**-0
+0000b8e0: 2e30 350a 2020 2020 2020 2020 2020 2020  .05.            
+0000b8f0: 6c61 6d62 6461 5f6e 3d6c 616d 6264 615f  lambda_n=lambda_
+0000b900: 6e2a 3130 2a2a 302e 3035 0a20 2020 2020  n*10**0.05.     
+0000b910: 2020 2064 615f 7265 713d 6461 5b28 6461     da_req=da[(da
+0000b920: 5b27 4748 7a27 5d3e 632f 6c61 6d62 6461  ['GHz']>c/lambda
+0000b930: 5f6e 2a31 652d 3329 2628 6461 5b27 4748  _n*1e-3)&(da['GH
+0000b940: 7a27 5d3c 632f 6c61 6d62 6461 5f30 2a31  z']<c/lambda_0*1
+0000b950: 652d 3329 5d0a 2020 2020 2020 2020 6461  e-3)].        da
+0000b960: 5f72 6571 2e72 6573 6574 5f69 6e64 6578  _req.reset_index
+0000b970: 2864 726f 703d 5472 7565 2c69 6e70 6c61  (drop=True,inpla
+0000b980: 6365 3d54 7275 6529 0a20 2020 2020 2020  ce=True).       
+0000b990: 2069 6620 636f 6e76 5f74 7970 653d 3d31   if conv_type==1
+0000b9a0: 3a0a 2020 2020 2020 2020 2020 2020 6c2c  :.            l,
+0000b9b0: 663d 6765 6e65 7261 6c43 6f6e 766f 6c76  f=generalConvolv
+0000b9c0: 6528 6461 5f72 6571 5b74 5d2c 6461 5f72  e(da_req[t],da_r
+0000b9d0: 6571 5b27 4748 7a27 5d2c 523d 522c 6c61  eq['GHz'],R=R,la
+0000b9e0: 6d62 6461 5f30 3d6c 616d 6264 615f 302c  mbda_0=lambda_0,
+0000b9f0: 6c61 6d62 6461 5f6e 3d6c 616d 6264 615f  lambda_n=lambda_
+0000ba00: 6e29 0a20 2020 2020 2020 2065 6c73 653a  n).        else:
+0000ba10: 0a20 2020 2020 2020 2020 2020 206c 2c66  .            l,f
+0000ba20: 3d73 7065 6343 6f6e 766f 6c76 6528 6461  =specConvolve(da
+0000ba30: 5f72 6571 5b74 5d2c 6461 5f72 6571 5b27  _req[t],da_req['
+0000ba40: 4748 7a27 5d2c 6672 6571 5f62 696e 733d  GHz'],freq_bins=
+0000ba50: 6672 6571 5f62 696e 732c 523d 522c 6c61  freq_bins,R=R,la
+0000ba60: 6d62 6461 5f30 3d6c 616d 6264 615f 302c  mbda_0=lambda_0,
+0000ba70: 6c61 6d62 6461 5f6e 3d6c 616d 6264 615f  lambda_n=lambda_
+0000ba80: 6e2c 7672 3d76 7229 0a20 2020 2020 2020  n,vr=vr).       
+0000ba90: 2073 656c 662e 636f 6e76 5761 7665 6c65   self.convWavele
+0000baa0: 6e67 7468 3d6c 0a20 2020 2020 2020 2073  ngth=l.        s
+0000bab0: 656c 662e 636f 6e76 5479 7065 3d63 6f6e  elf.convType=con
+0000bac0: 765f 7479 7065 0a20 2020 2020 2020 2073  v_type.        s
+0000bad0: 656c 662e 636f 6e76 523d 520a 2020 2020  elf.convR=R.    
+0000bae0: 2020 2020 6966 204e 4c54 453a 0a20 2020      if NLTE:.   
+0000baf0: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+0000bb00: 6e76 4e4c 5445 666c 7578 3d66 0a20 2020  nvNLTEflux=f.   
+0000bb10: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000bb20: 2020 2020 2020 2073 656c 662e 636f 6e76         self.conv
+0000bb30: 4c54 4566 6c75 783d 660a 0a20 2020 2064  LTEflux=f..    d
+0000bb40: 6566 2063 6f6e 766f 6c76 655f 6f76 6572  ef convolve_over
+0000bb50: 6c61 7028 7365 6c66 2c52 3d31 2c6c 616d  lap(self,R=1,lam
+0000bb60: 6264 615f 303d 312c 6c61 6d62 6461 5f6e  bda_0=1,lambda_n
+0000bb70: 3d31 293a 0a20 2020 2020 2020 2069 6620  =1):.        if 
+0000bb80: 6c61 6d62 6461 5f30 3d3d 6c61 6d62 6461  lambda_0==lambda
+0000bb90: 5f6e 3a0a 2020 2020 2020 2020 2020 2020  _n:.            
+0000bba0: 6c61 6d62 6461 5f30 3d6e 702e 616d 696e  lambda_0=np.amin
+0000bbb0: 2863 2f73 656c 662e 6f76 6572 6c61 7046  (c/self.overlapF
+0000bbc0: 7265 712a 3165 2d33 290a 2020 2020 2020  req*1e-3).      
+0000bbd0: 2020 2020 2020 6c61 6d62 6461 5f6e 3d6e        lambda_n=n
+0000bbe0: 702e 616d 6178 2863 2f73 656c 662e 6f76  p.amax(c/self.ov
+0000bbf0: 6572 6c61 7046 7265 712a 3165 2d33 290a  erlapFreq*1e-3).
+0000bc00: 2020 2020 2020 2020 2020 2020 6c61 6d62              lamb
+0000bc10: 6461 5f30 3d6c 616d 6264 615f 302a 3130  da_0=lambda_0*10
+0000bc20: 2a2a 2d30 2e30 350a 2020 2020 2020 2020  **-0.05.        
+0000bc30: 2020 2020 6c61 6d62 6461 5f6e 3d6c 616d      lambda_n=lam
+0000bc40: 6264 615f 6e2a 3130 2a2a 302e 3035 0a20  bda_n*10**0.05. 
+0000bc50: 2020 2020 2020 206d 6173 6b3d 2873 656c         mask=(sel
+0000bc60: 662e 6f76 6572 6c61 7046 7265 713e 632f  f.overlapFreq>c/
+0000bc70: 6c61 6d62 6461 5f6e 2a31 652d 3329 2628  lambda_n*1e-3)&(
+0000bc80: 7365 6c66 2e6f 7665 726c 6170 4672 6571  self.overlapFreq
+0000bc90: 3c63 2f6c 616d 6264 615f 302a 3165 2d33  <c/lambda_0*1e-3
+0000bca0: 290a 2020 2020 2020 2020 4657 484d 3d73  ).        FWHM=s
+0000bcb0: 656c 662e 6f76 6572 6c61 7052 2f52 2f32  elf.overlapR/R/2
+0000bcc0: 2e33 3535 0a20 2020 2020 2020 2067 3d47  .355.        g=G
+0000bcd0: 6175 7373 6961 6e31 444b 6572 6e65 6c28  aussian1DKernel(
+0000bce0: 7374 6464 6576 3d46 5748 4d2c 6661 6374  stddev=FWHM,fact
+0000bcf0: 6f72 3d37 290a 2020 2020 2020 2020 7365  or=7).        se
+0000bd00: 6c66 2e63 6f6e 764f 7665 726c 6170 4c54  lf.convOverlapLT
+0000bd10: 453d 6170 795f 636f 6e76 6f6c 7665 2873  E=apy_convolve(s
+0000bd20: 656c 662e 6f76 6572 6c61 704c 5445 5b6d  elf.overlapLTE[m
+0000bd30: 6173 6b5d 2c67 290a 2020 2020 2020 2020  ask],g).        
+0000bd40: 7365 6c66 2e63 6f6e 764f 7665 726c 6170  self.convOverlap
+0000bd50: 4e4c 5445 3d61 7079 5f63 6f6e 766f 6c76  NLTE=apy_convolv
+0000bd60: 6528 7365 6c66 2e6f 7665 726c 6170 4e4c  e(self.overlapNL
+0000bd70: 5445 5b6d 6173 6b5d 2c67 290a 2020 2020  TE[mask],g).    
+0000bd80: 2020 2020 7365 6c66 2e63 6f6e 764f 7665      self.convOve
+0000bd90: 726c 6170 4672 6571 3d73 656c 662e 6f76  rlapFreq=self.ov
+0000bda0: 6572 6c61 7046 7265 715b 6d61 736b 5d2a  erlapFreq[mask]*
+0000bdb0: 312e 300a 2020 2020 2020 2020 7365 6c66  1.0.        self
+0000bdc0: 2e63 6f6e 764f 7665 726c 6170 5761 7665  .convOverlapWave
+0000bdd0: 3d63 2f73 656c 662e 636f 6e76 4f76 6572  =c/self.convOver
+0000bde0: 6c61 7046 7265 712a 3165 2d33 0a20 2020  lapFreq*1e-3.   
+0000bdf0: 2020 2020 2073 656c 662e 636f 6e76 4f76       self.convOv
+0000be00: 6572 6c61 7052 3d52 0a0a 2020 2020 6465  erlapR=R..    de
+0000be10: 6620 7368 6f77 2873 656c 6629 3a0a 2020  f show(self):.  
+0000be20: 2020 2020 2020 7072 696e 7428 7365 6c66        print(self
+0000be30: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
+0000be40: 276c 696e 6544 6174 6120 2020 203d 2027  'lineData    = '
+0000be50: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
+0000be60: 7365 6c66 2e6c 696e 6564 6174 6129 0a20  self.linedata). 
+0000be70: 2020 2020 2020 2070 7269 6e74 2827 6c65         print('le
+0000be80: 7665 6c44 6174 6120 2020 3d20 2729 0a20  velData   = '). 
+0000be90: 2020 2020 2020 2070 7269 6e74 2873 656c         print(sel
+0000bea0: 662e 6c65 7665 6c64 6174 6129 0a0a 0a63  f.leveldata)...c
+0000beb0: 6c61 7373 2073 6c61 6231 443a 0a20 2020  lass slab1D:.   
+0000bec0: 2022 2222 0a20 2020 2063 6c61 7373 3a3a   """.    class::
+0000bed0: 2073 6c61 6231 440a 2020 2020 436c 6173   slab1D.    Clas
+0000bee0: 7320 746f 2068 6f6c 6420 7468 6520 6461  s to hold the da
+0000bef0: 7461 206f 6620 3144 2073 6c61 6220 6d6f  ta of 1D slab mo
+0000bf00: 6465 6c73 0a20 2020 2022 2222 0a0a 2020  dels.    """..  
+0000bf10: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+0000bf20: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
+0000bf30: 6c66 2e64 6972 6563 746f 7279 3d4e 6f6e  lf.directory=Non
+0000bf40: 650a 2020 2020 2020 2020 7365 6c66 2e66  e.        self.f
+0000bf50: 6c75 783d 4e6f 6e65 0a20 2020 2020 2020  lux=None.       
+0000bf60: 2073 656c 662e 6672 6571 7565 6e63 793d   self.frequency=
+0000bf70: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
+0000bf80: 662e 4e73 7065 6369 6573 3d4e 6f6e 650a  f.Nspecies=None.
+0000bf90: 2020 2020 2020 2020 7365 6c66 2e73 7065          self.spe
+0000bfa0: 6369 6573 3d5b 5d0a 2020 2020 2020 2020  cies=[].        
+0000bfb0: 7365 6c66 2e4e 6772 6964 3d4e 6f6e 650a  self.Ngrid=None.
+0000bfc0: 2020 2020 2020 2020 7365 6c66 2e52 3d4e          self.R=N
+0000bfd0: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+0000bfe0: 2e67 7269 643d 7064 2e44 6174 6146 7261  .grid=pd.DataFra
+0000bff0: 6d65 2829 0a20 2020 2020 2020 2073 656c  me().        sel
+0000c000: 662e 736f 7572 6365 5f66 756e 6374 696f  f.source_functio
+0000c010: 6e3d 4e6f 6e65 0a20 2020 2020 2020 2073  n=None.        s
+0000c020: 656c 662e 736f 7572 6365 5f66 756e 6374  elf.source_funct
+0000c030: 696f 6e5f 6761 733d 4e6f 6e65 0a20 2020  ion_gas=None.   
+0000c040: 2020 2020 2073 656c 662e 7461 755f 6475       self.tau_du
+0000c050: 7374 3d4e 6f6e 650a 2020 2020 2020 2020  st=None.        
+0000c060: 7365 6c66 2e74 6175 5f67 6173 3d4e 6f6e  self.tau_gas=Non
+0000c070: 650a 2020 2020 2020 2020 7365 6c66 2e63  e.        self.c
+0000c080: 6f6e 7657 6176 656c 656e 6774 683d 4e6f  onvWavelength=No
+0000c090: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
+0000c0a0: 636f 6e76 4672 6571 7565 6e63 793d 4e6f  convFrequency=No
+0000c0b0: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
+0000c0c0: 636f 6e76 5f66 6c75 783d 4e6f 6e65 0a20  conv_flux=None. 
+0000c0d0: 2020 2020 2020 2073 656c 662e 636f 6e76         self.conv
+0000c0e0: 523d 4e6f 6e65 0a0a 2020 2020 6465 6620  R=None..    def 
+0000c0f0: 5f5f 7374 725f 5f28 7365 6c66 293a 0a20  __str__(self):. 
+0000c100: 2020 2020 2020 206f 7574 7075 743d 2249         output="I
+0000c110: 6e66 6f20 4d6f 6465 6c3a 205c 6e22 0a20  nfo Model: \n". 
+0000c120: 2020 2020 2020 206f 7574 7075 742b 3d27         output+='
+0000c130: 4e75 6d62 6572 206f 6620 7370 6563 6965  Number of specie
+0000c140: 7320 2020 2020 2020 2020 203d 2027 0a20  s          = '. 
+0000c150: 2020 2020 2020 206f 7574 7075 742b 3d73         output+=s
+0000c160: 7472 2873 656c 662e 4e73 7065 6369 6573  tr(self.Nspecies
+0000c170: 292b 275c 6e5c 6e27 0a20 2020 2020 2020  )+'\n\n'.       
+0000c180: 206f 7574 7075 742b 3d27 4772 6964 2073   output+='Grid s
+0000c190: 697a 6520 2020 2020 2020 2020 2020 2020  ize             
+0000c1a0: 2020 2020 203d 2027 0a20 2020 2020 2020       = '.       
+0000c1b0: 206f 7574 7075 742b 3d73 7472 2873 656c   output+=str(sel
+0000c1c0: 662e 4e67 7269 6429 2b27 5c6e 5c6e 270a  f.Ngrid)+'\n\n'.
+0000c1d0: 2020 2020 2020 2020 6f75 7470 7574 2b3d          output+=
+0000c1e0: 2752 6573 6f6c 7669 6e67 2070 6f77 6572  'Resolving power
+0000c1f0: 206f 6620 7370 6563 7472 6120 3d20 270a   of spectra = '.
+0000c200: 2020 2020 2020 2020 6f75 7470 7574 2b3d          output+=
+0000c210: 7374 7228 7365 6c66 2e52 292b 275c 6e5c  str(self.R)+'\n\
+0000c220: 6e27 0a20 2020 2020 2020 206f 7574 7075  n'.        outpu
+0000c230: 742b 3d27 4f75 7470 7574 2066 696c 6520  t+='Output file 
+0000c240: 7061 7468 203d 2027 0a20 2020 2020 2020  path = '.       
+0000c250: 206f 7574 7075 742b 3d73 7472 2873 656c   output+=str(sel
+0000c260: 662e 6469 7265 6374 6f72 7929 2b27 5c6e  f.directory)+'\n
+0000c270: 5c6e 270a 2020 2020 2020 2020 7265 7475  \n'.        retu
+0000c280: 726e 206f 7574 7075 740a 0a20 2020 2064  rn output..    d
+0000c290: 6566 2063 6f6e 766f 6c76 6528 7365 6c66  ef convolve(self
+0000c2a0: 2c52 3d31 2c6c 616d 6264 615f 303d 312c  ,R=1,lambda_0=1,
+0000c2b0: 6c61 6d62 6461 5f6e 3d31 2c76 6572 626f  lambda_n=1,verbo
+0000c2c0: 7365 3d54 7275 6529 3a0a 2020 2020 2020  se=True):.      
+0000c2d0: 2020 6966 2076 6572 626f 7365 3a20 7072    if verbose: pr
+0000c2e0: 696e 7428 2243 6f6e 766f 6c76 696e 6720  int("Convolving 
+0000c2f0: 746f 2022 2c52 290a 2020 2020 2020 2020  to ",R).        
+0000c300: 6966 206c 616d 6264 615f 303d 3d6c 616d  if lambda_0==lam
+0000c310: 6264 615f 6e3a 0a20 2020 2020 2020 2020  bda_n:.         
+0000c320: 2020 206c 616d 6264 615f 303d 6e70 2e61     lambda_0=np.a
+0000c330: 6d69 6e28 632f 7365 6c66 2e66 7265 7175  min(c/self.frequ
+0000c340: 656e 6379 2a31 652d 3329 0a20 2020 2020  ency*1e-3).     
+0000c350: 2020 2020 2020 206c 616d 6264 615f 6e3d         lambda_n=
+0000c360: 6e70 2e61 6d61 7828 632f 7365 6c66 2e66  np.amax(c/self.f
+0000c370: 7265 7175 656e 6379 2a31 652d 3329 0a20  requency*1e-3). 
+0000c380: 2020 2020 2020 2020 2020 206c 616d 6264             lambd
+0000c390: 615f 303d 6c61 6d62 6461 5f30 2a31 302a  a_0=lambda_0*10*
+0000c3a0: 2a2d 302e 3035 0a20 2020 2020 2020 2020  *-0.05.         
+0000c3b0: 2020 206c 616d 6264 615f 6e3d 6c61 6d62     lambda_n=lamb
+0000c3c0: 6461 5f6e 2a31 302a 2a30 2e30 350a 2020  da_n*10**0.05.  
+0000c3d0: 2020 2020 2020 6d61 736b 3d28 7365 6c66        mask=(self
+0000c3e0: 2e66 7265 7175 656e 6379 3e63 2f6c 616d  .frequency>c/lam
+0000c3f0: 6264 615f 6e2a 3165 2d33 2926 2873 656c  bda_n*1e-3)&(sel
+0000c400: 662e 6672 6571 7565 6e63 793c 632f 6c61  f.frequency<c/la
+0000c410: 6d62 6461 5f30 2a31 652d 3329 0a20 2020  mbda_0*1e-3).   
+0000c420: 2020 2020 2046 5748 4d3d 7365 6c66 2e52       FWHM=self.R
+0000c430: 2f52 2f32 2e33 3535 0a20 2020 2020 2020  /R/2.355.       
+0000c440: 2067 3d47 6175 7373 6961 6e31 444b 6572   g=Gaussian1DKer
+0000c450: 6e65 6c28 7374 6464 6576 3d46 5748 4d2c  nel(stddev=FWHM,
+0000c460: 6661 6374 6f72 3d37 290a 2020 2020 2020  factor=7).      
+0000c470: 2020 7365 6c66 2e63 6f6e 765f 666c 7578    self.conv_flux
+0000c480: 3d61 7079 5f63 6f6e 766f 6c76 6528 7365  =apy_convolve(se
+0000c490: 6c66 2e66 6c75 785b 6d61 736b 5d2c 6729  lf.flux[mask],g)
+0000c4a0: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+0000c4b0: 6e76 4672 6571 7565 6e63 793d 7365 6c66  nvFrequency=self
+0000c4c0: 2e66 7265 7175 656e 6379 5b6d 6173 6b5d  .frequency[mask]
+0000c4d0: 2a31 2e30 0a20 2020 2020 2020 2073 656c  *1.0.        sel
+0000c4e0: 662e 636f 6e76 523d 520a 2020 2020 2020  f.convR=R.      
+0000c4f0: 2020 7365 6c66 2e63 6f6e 7657 6176 656c    self.convWavel
+0000c500: 656e 6774 683d 632f 7365 6c66 2e63 6f6e  ength=c/self.con
+0000c510: 7646 7265 7175 656e 6379 2a31 652d 330a  vFrequency*1e-3.
+0000c520: 0a20 2020 2064 6566 2073 686f 7728 7365  .    def show(se
+0000c530: 6c66 293a 0a20 2020 2020 2020 2070 7269  lf):.        pri
+0000c540: 6e74 2873 656c 6629 0a20 2020 2020 2020  nt(self).       
+0000c550: 2070 7269 6e74 2827 4772 6964 2020 2020   print('Grid    
+0000c560: 3d20 2729 0a20 2020 2020 2020 2070 7269  = ').        pri
+0000c570: 6e74 2873 656c 662e 6772 6964 290a 2020  nt(self.grid).  
+0000c580: 2020 2020 2020 7072 696e 7428 2753 6f75        print('Sou
+0000c590: 7263 6520 6675 6e63 7469 6f6e 2020 203d  rce function   =
+0000c5a0: 2027 290a 2020 2020 2020 2020 7072 696e   ').        prin
+0000c5b0: 7428 7365 6c66 2e73 6f75 7263 655f 6675  t(self.source_fu
+0000c5c0: 6e63 7469 6f6e 290a 2020 2020 2020 2020  nction).        
+0000c5d0: 7072 696e 7428 2747 6173 206f 6e6c 7920  print('Gas only 
+0000c5e0: 736f 7572 6365 2066 756e 6374 696f 6e20  source function 
+0000c5f0: 2020 3d20 2729 0a20 2020 2020 2020 2070    = ').        p
+0000c600: 7269 6e74 2873 656c 662e 736f 7572 6365  rint(self.source
+0000c610: 5f66 756e 6374 696f 6e5f 6761 7329 0a20  _function_gas). 
+0000c620: 2020 2020 2020 2070 7269 6e74 2827 4475         print('Du
+0000c630: 7374 206f 7074 6963 616c 2064 6570 7468  st optical depth
+0000c640: 2020 203d 2027 290a 2020 2020 2020 2020     = ').        
+0000c650: 7072 696e 7428 7365 6c66 2e74 6175 5f64  print(self.tau_d
+0000c660: 7573 7429 0a20 2020 2020 2020 2070 7269  ust).        pri
+0000c670: 6e74 2827 4761 7320 6f70 7469 6361 6c20  nt('Gas optical 
+0000c680: 6465 7074 6820 2020 3d20 2729 0a20 2020  depth   = ').   
+0000c690: 2020 2020 2070 7269 6e74 2873 656c 662e       print(self.
+0000c6a0: 7461 755f 6761 7329 0a0a 0a63 6c61 7373  tau_gas)...class
+0000c6b0: 2066 6974 3a0a 2020 2020 6465 6620 5f5f   fit:.    def __
+0000c6c0: 696e 6974 5f5f 2873 656c 6629 3a0a 2020  init__(self):.  
+0000c6d0: 2020 2020 2020 7365 6c66 2e6e 616d 6520        self.name 
+0000c6e0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
+0000c6f0: 656c 662e 7220 3d20 4e6f 6e65 0a20 2020  elf.r = None.   
+0000c700: 2020 2020 2073 656c 662e 4e20 3d20 4e6f       self.N = No
+0000c710: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
+0000c720: 5420 3d20 4e6f 6e65 0a20 2020 2020 2020  T = None.       
+0000c730: 2073 656c 662e 6265 7374 5f66 6974 203d   self.best_fit =
+0000c740: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
+0000c750: 6c66 2e62 6573 745f 6669 745f 6669 6c65  lf.best_fit_file
+0000c760: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+0000c770: 7365 6c66 2e63 6869 3220 3d20 4e6f 6e65  self.chi2 = None
+0000c780: 0a20 2020 2020 2020 2073 656c 662e 6669  .        self.fi
+0000c790: 745f 7769 6e64 6f77 203d 204e 6f6e 650a  t_window = None.
+0000c7a0: 2020 2020 2020 2020 7365 6c66 2e66 6974          self.fit
+0000c7b0: 5f73 6574 7469 6e67 7320 3d20 4e6f 6e65  _settings = None
+0000c7c0: 0a20 2020 2020 2020 2073 656c 662e 6368  .        self.ch
+0000c7d0: 6932 5f6d 6170 203d 204e 6f6e 650a 2020  i2_map = None.  
+0000c7e0: 2020 2020 2020 7365 6c66 2e72 5f6d 6170        self.r_map
+0000c7f0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+0000c800: 0a20 2020 2064 6566 205f 5f73 7472 5f5f  .    def __str__
+0000c810: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000c820: 6f75 7470 7574 203d 2027 4669 743a 205c  output = 'Fit: \
+0000c830: 6e27 0a20 2020 2020 2020 206f 7574 7075  n'.        outpu
+0000c840: 7420 2b3d 2027 4e61 6d65 3a20 272b 7374  t += 'Name: '+st
+0000c850: 7228 7365 6c66 2e6e 616d 6529 2b27 205c  r(self.name)+' \
+0000c860: 6e27 0a20 2020 2020 2020 206f 7574 7075  n'.        outpu
+0000c870: 7420 2b3d 2027 4265 7374 2066 6974 2070  t += 'Best fit p
+0000c880: 6172 616d 6574 6572 733a 205c 6e27 0a20  arameters: \n'. 
+0000c890: 2020 2020 2020 206f 7574 7075 7420 2b3d         output +=
+0000c8a0: 2066 274e 203d 207b 3130 2a2a 7365 6c66   f'N = {10**self
+0000c8b0: 2e4e 3a2e 3265 7d20 636d 2d32 2c20 5420  .N:.2e} cm-2, T 
+0000c8c0: 3d20 7b73 656c 662e 543a 2e31 667d 204b  = {self.T:.1f} K
+0000c8d0: 2c20 5220 3d20 7b73 656c 662e 723a 2e35  , R = {self.r:.5
+0000c8e0: 667d 2061 752c 2063 6869 3220 3d20 7b73  f} au, chi2 = {s
+0000c8f0: 656c 662e 6368 6932 3a2e 3265 7d20 5c6e  elf.chi2:.2e} \n
+0000c900: 270a 2020 2020 2020 2020 6f75 7470 7574  '.        output
+0000c910: 202b 3d20 2742 6573 7420 6669 7420 6669   += 'Best fit fi
+0000c920: 6c65 3a20 272b 7374 7228 7365 6c66 2e62  le: '+str(self.b
+0000c930: 6573 745f 6669 745f 6669 6c65 292b 275c  est_fit_file)+'\
+0000c940: 6e27 0a20 2020 2020 2020 206f 7574 7075  n'.        outpu
+0000c950: 7420 2b3d 2027 4669 7420 7769 6e64 6f77  t += 'Fit window
+0000c960: 3a20 270a 2020 2020 2020 2020 6966 206e  : '.        if n
+0000c970: 6f74 2073 656c 662e 6669 745f 7769 6e64  ot self.fit_wind
+0000c980: 6f77 2069 7320 4e6f 6e65 3a0a 2020 2020  ow is None:.    
+0000c990: 2020 2020 2020 2020 666f 7220 7769 6e64          for wind
+0000c9a0: 2069 6e20 7365 6c66 2e66 6974 5f77 696e   in self.fit_win
+0000c9b0: 646f 773a 0a20 2020 2020 2020 2020 2020  dow:.           
+0000c9c0: 2020 2020 206f 7574 7075 7420 2b3d 2066       output += f
+0000c9d0: 277b 7769 6e64 5b30 5d3a 2e33 667d 206d  '{wind[0]:.3f} m
+0000c9e0: 6963 2c20 7b77 696e 645b 315d 3a2e 3366  ic, {wind[1]:.3f
+0000c9f0: 7d20 6d69 635c 6e27 0a20 2020 2020 2020  } mic\n'.       
+0000ca00: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000ca10: 2020 206f 7574 7075 7420 2b3d 2027 4e6f     output += 'No
+0000ca20: 6e65 205c 6e27 0a20 2020 2020 2020 2072  ne \n'.        r
+0000ca30: 6574 7572 6e28 6f75 7470 7574 290a 0a20  eturn(output).. 
+0000ca40: 2020 2020 2020 200a 636c 6173 7320 6669         .class fi
+0000ca50: 745f 7365 7474 696e 6773 3a0a 2020 2020  t_settings:.    
+0000ca60: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+0000ca70: 662c 4e4d 4f4c 3d4e 6f6e 652c 4e6c 696d  f,NMOL=None,Nlim
+0000ca80: 7320 3d20 5b5d 2c54 6c69 6d73 203d 205b  s = [],Tlims = [
+0000ca90: 5d2c 6772 6964 203d 204e 6f6e 652c 6772  ],grid = None,gr
+0000caa0: 6964 5f6d 6173 6b20 3d20 4e6f 6e65 2c66  id_mask = None,f
+0000cab0: 6974 5f77 696e 646f 7720 3d20 4e6f 6e65  it_window = None
+0000cac0: 2c52 6469 736b 3d4e 6f6e 652c 6469 7374  ,Rdisk=None,dist
+0000cad0: 616e 6365 3d4e 6f6e 652c 523d 4e6f 6e65  ance=None,R=None
+0000cae0: 2c6e 6f69 7365 5f6c 6576 656c 203d 204e  ,noise_level = N
+0000caf0: 6f6e 6529 3a0a 2020 2020 2020 2020 7365  one):.        se
+0000cb00: 6c66 2e4e 4d4f 4c20 3d20 4e4d 4f4c 0a20  lf.NMOL = NMOL. 
+0000cb10: 2020 2020 2020 2073 656c 662e 4e6c 696d         self.Nlim
+0000cb20: 7320 3d20 4e6c 696d 730a 2020 2020 2020  s = Nlims.      
+0000cb30: 2020 7365 6c66 2e54 6c69 6d73 203d 2054    self.Tlims = T
+0000cb40: 6c69 6d73 0a20 2020 2020 2020 2073 656c  lims.        sel
+0000cb50: 662e 6772 6964 203d 2067 7269 640a 2020  f.grid = grid.  
+0000cb60: 2020 2020 2020 7365 6c66 2e67 7269 645f        self.grid_
+0000cb70: 6d61 736b 203d 2067 7269 645f 6d61 736b  mask = grid_mask
+0000cb80: 0a20 2020 2020 2020 2073 656c 662e 6669  .        self.fi
+0000cb90: 745f 7769 6e64 6f77 203d 2066 6974 5f77  t_window = fit_w
+0000cba0: 696e 646f 770a 2020 2020 2020 2020 7365  indow.        se
+0000cbb0: 6c66 2e52 6469 736b 203d 2052 6469 736b  lf.Rdisk = Rdisk
+0000cbc0: 0a20 2020 2020 2020 2073 656c 662e 6469  .        self.di
+0000cbd0: 7374 616e 6365 203d 2064 6973 7461 6e63  stance = distanc
+0000cbe0: 650a 2020 2020 2020 2020 7365 6c66 2e52  e.        self.R
+0000cbf0: 203d 2052 0a20 2020 2020 2020 2073 656c   = R.        sel
+0000cc00: 662e 6e6f 6973 655f 6c65 7665 6c20 3d20  f.noise_level = 
+0000cc10: 6e6f 6973 655f 6c65 7665 6c0a 2020 2020  noise_level.    
+0000cc20: 2020 2020 0a20 2020 2064 6566 205f 5f73      .    def __s
+0000cc30: 7472 5f5f 2873 656c 6629 3a0a 2020 2020  tr__(self):.    
+0000cc40: 2020 2020 6f75 7470 7574 203d 2027 4669      output = 'Fi
+0000cc50: 7420 7365 7474 696e 6773 3a20 5c6e 270a  t settings: \n'.
+0000cc60: 2020 2020 2020 2020 6f75 7470 7574 202b          output +
+0000cc70: 3d20 6627 4e4d 4f4c 203d 207b 7365 6c66  = f'NMOL = {self
+0000cc80: 2e4e 4d4f 4c7d 205c 6e27 0a20 2020 2020  .NMOL} \n'.     
+0000cc90: 2020 206f 7574 7075 7420 2b3d 2066 274e     output += f'N
+0000cca0: 6c69 6d73 203d 207b 7365 6c66 2e4e 6c69  lims = {self.Nli
+0000ccb0: 6d73 7d20 5c6e 270a 2020 2020 2020 2020  ms} \n'.        
+0000ccc0: 6f75 7470 7574 202b 3d20 6627 546c 696d  output += f'Tlim
+0000ccd0: 7320 3d20 7b73 656c 662e 546c 696d 737d  s = {self.Tlims}
+0000cce0: 205c 6e27 0a20 2020 2020 2020 206f 7574   \n'.        out
+0000ccf0: 7075 7420 2b3d 2066 2767 7269 642e 7368  put += f'grid.sh
+0000cd00: 6170 6520 3d20 7b6e 702e 6172 7261 7928  ape = {np.array(
+0000cd10: 7365 6c66 2e67 7269 6429 2e73 6861 7065  self.grid).shape
+0000cd20: 7d20 5c6e 270a 2020 2020 2020 2020 6f75  } \n'.        ou
+0000cd30: 7470 7574 202b 3d20 6627 6772 6964 5f6d  tput += f'grid_m
+0000cd40: 6173 6b20 3d20 7b73 656c 662e 6772 6964  ask = {self.grid
+0000cd50: 5f6d 6173 6b7d 205c 6e27 0a20 2020 2020  _mask} \n'.     
+0000cd60: 2020 206f 7574 7075 7420 2b3d 2066 2766     output += f'f
+0000cd70: 6974 5f77 696e 646f 7720 3d20 7b73 656c  it_window = {sel
+0000cd80: 662e 6669 745f 7769 6e64 6f77 7d20 5c6e  f.fit_window} \n
+0000cd90: 270a 2020 2020 2020 2020 6f75 7470 7574  '.        output
+0000cda0: 202b 3d20 6627 6c65 6e28 5264 6973 6b29   += f'len(Rdisk)
+0000cdb0: 203d 207b 6c65 6e28 7365 6c66 2e52 6469   = {len(self.Rdi
+0000cdc0: 736b 297d 205c 6e27 0a20 2020 2020 2020  sk)} \n'.       
+0000cdd0: 206f 7574 7075 7420 2b3d 2066 2764 6973   output += f'dis
+0000cde0: 7461 6e63 6520 3d20 7b73 656c 662e 6469  tance = {self.di
+0000cdf0: 7374 616e 6365 7d20 5c6e 270a 2020 2020  stance} \n'.    
+0000ce00: 2020 2020 6f75 7470 7574 202b 3d20 6627      output += f'
+0000ce10: 5220 3d20 7b73 656c 662e 527d 205c 6e27  R = {self.R} \n'
+0000ce20: 0a20 2020 2020 2020 206f 7574 7075 7420  .        output 
+0000ce30: 2b3d 2066 276e 6f69 7365 5f6c 6576 656c  += f'noise_level
+0000ce40: 203d 207b 7365 6c66 2e6e 6f69 7365 5f6c   = {self.noise_l
+0000ce50: 6576 656c 7d20 5c6e 270a 2020 2020 2020  evel} \n'.      
+0000ce60: 2020 7265 7475 726e 286f 7574 7075 7429    return(output)
+0000ce70: 0a0a 2020 2020 2020 2020 0a64 6566 2072  ..        .def r
+0000ce80: 6561 645f 3144 5f73 6c61 6228 6d6f 6465  ead_1D_slab(mode
+0000ce90: 6c5f 7061 7468 3d27 536c 6162 5265 7375  l_path='SlabResu
+0000cea0: 6c74 732e 6669 7473 2e67 7a27 2c76 6572  lts.fits.gz',ver
+0000ceb0: 626f 7365 3d54 7275 6529 3a0a 2020 2020  bose=True):.    
+0000cec0: 2222 220a 2020 2020 4675 6e63 7469 6f6e  """.    Function
+0000ced0: 2074 6f20 7265 6164 2031 4420 7072 6f64   to read 1D prod
+0000cee0: 696d 6f20 736c 6162 206d 6f64 656c 206f  imo slab model o
+0000cef0: 7574 7075 740a 2020 2020 2222 220a 2020  utput.    """.  
+0000cf00: 2020 6966 2076 6572 626f 7365 3a20 7072    if verbose: pr
+0000cf10: 696e 7428 2252 6561 6469 6e67 2031 4420  int("Reading 1D 
+0000cf20: 736c 6162 206d 6f64 656c 206f 7574 7075  slab model outpu
+0000cf30: 7420 6672 6f6d 3a20 222c 6d6f 6465 6c5f  t from: ",model_
+0000cf40: 7061 7468 290a 2020 2020 6966 2027 2e66  path).    if '.f
+0000cf50: 6974 732e 677a 2720 696e 206d 6f64 656c  its.gz' in model
+0000cf60: 5f70 6174 683a 0a20 2020 2020 2020 2068  _path:.        h
+0000cf70: 6475 6c3d 6669 7473 2e6f 7065 6e28 6d6f  dul=fits.open(mo
+0000cf80: 6465 6c5f 7061 7468 290a 2020 2020 2020  del_path).      
+0000cf90: 2020 6461 7461 3d73 6c61 6231 4428 290a    data=slab1D().
+0000cfa0: 2020 2020 2020 2020 6461 7461 2e64 6972          data.dir
+0000cfb0: 6563 746f 7279 3d6d 6f64 656c 5f70 6174  ectory=model_pat
+0000cfc0: 680a 2020 2020 2020 2020 6461 7461 2e66  h.        data.f
+0000cfd0: 6c75 783d 6864 756c 5b30 5d2e 6461 7461  lux=hdul[0].data
+0000cfe0: 2e54 5b3a 2c31 5d0a 2020 2020 2020 2020  .T[:,1].        
+0000cff0: 6461 7461 2e66 7265 7175 656e 6379 3d68  data.frequency=h
+0000d000: 6475 6c5b 305d 2e64 6174 612e 545b 3a2c  dul[0].data.T[:,
+0000d010: 305d 0a20 2020 2020 2020 2064 6174 612e  0].        data.
+0000d020: 4e73 7065 6369 6573 3d68 6475 6c5b 305d  Nspecies=hdul[0]
+0000d030: 2e68 6561 6465 725b 274e 5350 4543 4945  .header['NSPECIE
+0000d040: 5327 5d0a 2020 2020 2020 2020 6461 7461  S'].        data
+0000d050: 2e73 7065 6369 6573 3d68 6475 6c5b 305d  .species=hdul[0]
+0000d060: 2e68 6561 6465 722e 636f 6d6d 656e 7473  .header.comments
+0000d070: 5b27 4e53 5045 4349 4553 275d 2e73 706c  ['NSPECIES'].spl
+0000d080: 6974 2827 2c27 290a 2020 2020 2020 2020  it(',').        
+0000d090: 6461 7461 2e4e 6772 6964 3d68 6475 6c5b  data.Ngrid=hdul[
+0000d0a0: 305d 2e68 6561 6465 725b 274e 4752 4944  0].header['NGRID
+0000d0b0: 275d 0a20 2020 2020 2020 2064 6174 612e  '].        data.
+0000d0c0: 523d 6864 756c 5b30 5d2e 6865 6164 6572  R=hdul[0].header
+0000d0d0: 5b27 525f 4f56 4c50 275d 0a20 2020 2020  ['R_OVLP'].     
+0000d0e0: 2020 2069 6620 2828 392b 6461 7461 2e4e     if ((9+data.N
+0000d0f0: 7370 6563 6965 732a 3229 2c64 6174 612e  species*2),data.
+0000d100: 4e67 7269 6429 3d3d 6864 756c 5b31 5d2e  Ngrid)==hdul[1].
+0000d110: 6461 7461 2e54 2e73 6861 7065 3a0a 2020  data.T.shape:.  
+0000d120: 2020 2020 2020 2020 2020 6772 6964 3d68            grid=h
+0000d130: 6475 6c5b 315d 2e64 6174 610a 2020 2020  dul[1].data.    
+0000d140: 2020 2020 2020 2020 6461 7461 2e67 7269          data.gri
+0000d150: 645b 2764 7a27 5d3d 6772 6964 5b3a 2c30  d['dz']=grid[:,0
+0000d160: 5d0a 2020 2020 2020 2020 2020 2020 6461  ].            da
+0000d170: 7461 2e67 7269 645b 2776 7475 7262 275d  ta.grid['vturb']
+0000d180: 3d67 7269 645b 3a2c 315d 0a20 2020 2020  =grid[:,1].     
+0000d190: 2020 2020 2020 2064 6174 612e 6772 6964         data.grid
+0000d1a0: 5b27 6e64 275d 3d67 7269 645b 3a2c 325d  ['nd']=grid[:,2]
+0000d1b0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+0000d1c0: 612e 6772 6964 5b27 5464 275d 3d67 7269  a.grid['Td']=gri
+0000d1d0: 645b 3a2c 335d 0a20 2020 2020 2020 2020  d[:,3].         
+0000d1e0: 2020 2064 6174 612e 6772 6964 5b27 6e48     data.grid['nH
+0000d1f0: 3227 5d3d 6772 6964 5b3a 2c34 5d0a 2020  2']=grid[:,4].  
+0000d200: 2020 2020 2020 2020 2020 6461 7461 2e67            data.g
+0000d210: 7269 645b 276e 4849 275d 3d67 7269 645b  rid['nHI']=grid[
+0000d220: 3a2c 355d 0a20 2020 2020 2020 2020 2020  :,5].           
+0000d230: 2064 6174 612e 6772 6964 5b27 6e48 4949   data.grid['nHII
+0000d240: 275d 3d67 7269 645b 3a2c 365d 0a20 2020  ']=grid[:,6].   
+0000d250: 2020 2020 2020 2020 2064 6174 612e 6772           data.gr
+0000d260: 6964 5b27 6e48 6527 5d3d 6772 6964 5b3a  id['nHe']=grid[:
+0000d270: 2c37 5d0a 2020 2020 2020 2020 2020 2020  ,7].            
+0000d280: 6461 7461 2e67 7269 645b 276e 656c 6563  data.grid['nelec
+0000d290: 275d 3d67 7269 645b 3a2c 385d 0a20 2020  ']=grid[:,8].   
+0000d2a0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+0000d2b0: 6e20 7261 6e67 6528 6461 7461 2e4e 7370  n range(data.Nsp
+0000d2c0: 6563 6965 7329 3a0a 2020 2020 2020 2020  ecies):.        
+0000d2d0: 2020 2020 2020 2020 6b65 793d 276e 272b          key='n'+
+0000d2e0: 6461 7461 2e73 7065 6369 6573 5b69 5d0a  data.species[i].
+0000d2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d300: 6461 7461 2e67 7269 645b 6b65 795d 3d67  data.grid[key]=g
+0000d310: 7269 645b 3a2c 392b 695d 0a20 2020 2020  rid[:,9+i].     
+0000d320: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+0000d330: 7261 6e67 6528 6461 7461 2e4e 7370 6563  range(data.Nspec
+0000d340: 6965 7329 3a0a 2020 2020 2020 2020 2020  ies):.          
+0000d350: 2020 2020 2020 6b65 793d 2754 675f 272b        key='Tg_'+
+0000d360: 6461 7461 2e73 7065 6369 6573 5b69 5d0a  data.species[i].
+0000d370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d380: 6461 7461 2e67 7269 645b 6b65 795d 3d67  data.grid[key]=g
+0000d390: 7269 645b 3a2c 392b 6461 7461 2e4e 7370  rid[:,9+data.Nsp
+0000d3a0: 6563 6965 732b 695d 0a20 2020 2020 2020  ecies+i].       
+0000d3b0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000d3c0: 2020 2072 6169 7365 2041 7373 6572 7469     raise Asserti
+0000d3d0: 6f6e 4572 726f 7228 2747 7269 6420 696e  onError('Grid in
+0000d3e0: 206f 7574 7075 7420 6669 6c65 2064 6f65   output file doe
+0000d3f0: 7320 6e6f 7420 6d61 7463 6820 7468 6520  s not match the 
+0000d400: 6163 7475 616c 2067 7269 6420 6f75 7470  actual grid outp
+0000d410: 7574 2061 7272 6179 2729 0a0a 2020 2020  ut array')..    
+0000d420: 2020 2020 6966 2028 6c65 6e28 6461 7461      if (len(data
+0000d430: 2e66 7265 7175 656e 6379 292c 6461 7461  .frequency),data
+0000d440: 2e4e 6772 6964 293d 3d68 6475 6c5b 325d  .Ngrid)==hdul[2]
+0000d450: 2e64 6174 612e 542e 7368 6170 653a 0a20  .data.T.shape:. 
+0000d460: 2020 2020 2020 2020 2020 2064 6174 612e             data.
+0000d470: 736f 7572 6365 5f66 756e 6374 696f 6e3d  source_function=
+0000d480: 6864 756c 5b32 5d2e 6461 7461 0a20 2020  hdul[2].data.   
+0000d490: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000d4a0: 2020 2020 2020 2072 6169 7365 2041 7373         raise Ass
+0000d4b0: 6572 7469 6f6e 4572 726f 7228 2753 6f75  ertionError('Sou
+0000d4c0: 7263 6520 6675 6e63 7469 6f6e 2067 7269  rce function gri
+0000d4d0: 6420 696e 206f 7574 7075 7420 6669 6c65  d in output file
+0000d4e0: 2064 6f65 7320 6e6f 7420 6d61 7463 6820   does not match 
+0000d4f0: 7468 6520 7370 6174 6961 6c20 616e 6420  the spatial and 
+0000d500: 6672 6571 7565 6e63 7920 6772 6964 2073  frequency grid s
+0000d510: 697a 6527 290a 0a20 2020 2020 2020 2069  ize')..        i
+0000d520: 6620 286c 656e 2864 6174 612e 6672 6571  f (len(data.freq
+0000d530: 7565 6e63 7929 2c64 6174 612e 4e67 7269  uency),data.Ngri
+0000d540: 6429 3d3d 6864 756c 5b33 5d2e 6461 7461  d)==hdul[3].data
+0000d550: 2e54 2e73 6861 7065 3a0a 2020 2020 2020  .T.shape:.      
+0000d560: 2020 2020 2020 6461 7461 2e73 6f75 7263        data.sourc
+0000d570: 655f 6675 6e63 7469 6f6e 5f67 6173 3d68  e_function_gas=h
+0000d580: 6475 6c5b 335d 2e64 6174 610a 2020 2020  dul[3].data.    
+0000d590: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000d5a0: 2020 2020 2020 7261 6973 6520 4173 7365        raise Asse
+0000d5b0: 7274 696f 6e45 7272 6f72 2827 4761 7320  rtionError('Gas 
+0000d5c0: 736f 7572 6365 2066 756e 6374 696f 6e20  source function 
+0000d5d0: 6772 6964 2069 6e20 6f75 7470 7574 2066  grid in output f
+0000d5e0: 696c 6520 646f 6573 206e 6f74 206d 6174  ile does not mat
+0000d5f0: 6368 2074 6865 2073 7061 7469 616c 2061  ch the spatial a
+0000d600: 6e64 2066 7265 7175 656e 6379 2067 7269  nd frequency gri
+0000d610: 6420 7369 7a65 2729 0a0a 2020 2020 2020  d size')..      
+0000d620: 2020 6966 2028 6c65 6e28 6461 7461 2e66    if (len(data.f
+0000d630: 7265 7175 656e 6379 292c 6461 7461 2e4e  requency),data.N
+0000d640: 6772 6964 293d 3d68 6475 6c5b 345d 2e64  grid)==hdul[4].d
+0000d650: 6174 612e 542e 7368 6170 653a 0a20 2020  ata.T.shape:.   
+0000d660: 2020 2020 2020 2020 2064 6174 612e 7461           data.ta
+0000d670: 755f 6475 7374 3d68 6475 6c5b 345d 2e64  u_dust=hdul[4].d
+0000d680: 6174 610a 2020 2020 2020 2020 656c 7365  ata.        else
+0000d690: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+0000d6a0: 6973 6520 4173 7365 7274 696f 6e45 7272  ise AssertionErr
+0000d6b0: 6f72 2827 4475 7374 206f 7074 6963 616c  or('Dust optical
+0000d6c0: 2064 6570 7468 2067 7269 6420 696e 206f   depth grid in o
+0000d6d0: 7574 7075 7420 6669 6c65 2064 6f65 7320  utput file does 
+0000d6e0: 6e6f 7420 6d61 7463 6820 7468 6520 7370  not match the sp
+0000d6f0: 6174 6961 6c20 616e 6420 6672 6571 7565  atial and freque
+0000d700: 6e63 7920 6772 6964 2073 697a 6527 290a  ncy grid size').
+0000d710: 0a20 2020 2020 2020 2069 6620 286c 656e  .        if (len
+0000d720: 2864 6174 612e 6672 6571 7565 6e63 7929  (data.frequency)
+0000d730: 2c64 6174 612e 4e67 7269 6429 3d3d 6864  ,data.Ngrid)==hd
+0000d740: 756c 5b35 5d2e 6461 7461 2e54 2e73 6861  ul[5].data.T.sha
+0000d750: 7065 3a0a 2020 2020 2020 2020 2020 2020  pe:.            
+0000d760: 6461 7461 2e74 6175 5f67 6173 3d68 6475  data.tau_gas=hdu
+0000d770: 6c5b 355d 2e64 6174 610a 2020 2020 2020  l[5].data.      
+0000d780: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000d790: 2020 2020 7261 6973 6520 4173 7365 7274      raise Assert
+0000d7a0: 696f 6e45 7272 6f72 2827 4761 7320 6f70  ionError('Gas op
+0000d7b0: 7469 6361 6c20 6465 7074 6820 6772 6964  tical depth grid
+0000d7c0: 2069 6e20 6f75 7470 7574 2066 696c 6520   in output file 
+0000d7d0: 646f 6573 206e 6f74 206d 6174 6368 2074  does not match t
+0000d7e0: 6865 2073 7061 7469 616c 2061 6e64 2066  he spatial and f
+0000d7f0: 7265 7175 656e 6379 2067 7269 6420 7369  requency grid si
+0000d800: 7a65 2729 0a20 2020 2065 6c73 653a 0a20  ze').    else:. 
+0000d810: 2020 2020 2020 2064 6174 615f 7265 6164         data_read
+0000d820: 3d6e 702e 6c6f 6164 7478 7428 6d6f 6465  =np.loadtxt(mode
+0000d830: 6c5f 7061 7468 2c73 6b69 7072 6f77 733d  l_path,skiprows=
+0000d840: 3129 0a20 2020 2020 2020 2064 6174 613d  1).        data=
+0000d850: 736c 6162 3144 2829 0a20 2020 2020 2020  slab1D().       
+0000d860: 2064 6174 612e 6469 7265 6374 6f72 793d   data.directory=
+0000d870: 6d6f 6465 6c5f 7061 7468 0a20 2020 2020  model_path.     
+0000d880: 2020 2064 6174 612e 666c 7578 3d64 6174     data.flux=dat
+0000d890: 615f 7265 6164 5b3a 2c31 5d0a 2020 2020  a_read[:,1].    
+0000d8a0: 2020 2020 6461 7461 2e66 7265 7175 656e      data.frequen
+0000d8b0: 6379 3d64 6174 615f 7265 6164 5b3a 2c30  cy=data_read[:,0
+0000d8c0: 5d0a 2020 2020 7265 7475 726e 2864 6174  ].    return(dat
+0000d8d0: 6129 0a0a 0a64 6566 2072 6561 645f 736c  a)...def read_sl
+0000d8e0: 6162 286d 6f64 656c 5f70 6174 683d 2753  ab(model_path='S
+0000d8f0: 6c61 6252 6573 756c 7473 2e6f 7574 272c  labResults.out',
+0000d900: 7665 7262 6f73 653d 5472 7565 2c73 686f  verbose=True,sho
+0000d910: 7274 5f66 6f72 6d61 743d 4661 6c73 652c  rt_format=False,
+0000d920: 6f76 6572 6c61 703d 4661 6c73 6529 3a0a  overlap=False):.
+0000d930: 2020 2020 2222 220a 2020 2020 4675 6e63      """.    Func
+0000d940: 7469 6f6e 2074 6f20 7265 6164 2073 6c61  tion to read sla
+0000d950: 6220 6d6f 6465 6c20 6f75 7470 7574 0a20  b model output. 
+0000d960: 2020 2022 2222 0a20 2020 2069 6620 6f76     """.    if ov
+0000d970: 6572 6c61 703a 2072 6574 7572 6e28 7265  erlap: return(re
+0000d980: 6164 5f6f 7665 726c 6170 5f73 7065 6374  ad_overlap_spect
+0000d990: 7261 2870 6174 683d 6d6f 6465 6c5f 7061  ra(path=model_pa
+0000d9a0: 7468 2c76 6572 626f 7365 3d76 6572 626f  th,verbose=verbo
+0000d9b0: 7365 2929 0a0a 2020 2020 6966 2069 7369  se))..    if isi
+0000d9c0: 6e73 7461 6e63 6528 6d6f 6465 6c5f 7061  nstance(model_pa
+0000d9d0: 7468 2c6c 6973 7429 3a0a 2020 2020 2020  th,list):.      
+0000d9e0: 2020 6461 7461 3d73 6c61 625f 6461 7461    data=slab_data
+0000d9f0: 2829 0a20 2020 2020 2020 2064 6174 612e  ().        data.
+0000da00: 6469 7265 6374 6f72 793d 6d6f 6465 6c5f  directory=model_
+0000da10: 7061 7468 0a20 2020 2020 2020 2066 6f72  path.        for
+0000da20: 2069 2069 6e20 6d6f 6465 6c5f 7061 7468   i in model_path
+0000da30: 3a0a 2020 2020 2020 2020 2020 2020 7264  :.            rd
+0000da40: 6174 613d 7265 6164 5f73 6c61 6228 692c  ata=read_slab(i,
+0000da50: 7665 7262 6f73 653d 7665 7262 6f73 652c  verbose=verbose,
+0000da60: 7368 6f72 745f 666f 726d 6174 3d73 686f  short_format=sho
+0000da70: 7274 5f66 6f72 6d61 7429 0a20 2020 2020  rt_format).     
+0000da80: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
+0000da90: 7261 6e67 6528 7264 6174 612e 6e6d 6f64  range(rdata.nmod
+0000daa0: 656c 7329 3a0a 2020 2020 2020 2020 2020  els):.          
+0000dab0: 2020 2020 2020 6461 7461 2e61 6464 5f6d        data.add_m
+0000dac0: 6f64 656c 2872 6461 7461 2e6d 6f64 656c  odel(rdata.model
+0000dad0: 735b 6a5d 290a 2020 2020 2020 2020 7265  s[j]).        re
+0000dae0: 7475 726e 2864 6174 6129 0a20 2020 200a  turn(data).    .
+0000daf0: 2020 2020 0a20 2020 2069 6620 7665 7262      .    if verb
+0000db00: 6f73 653a 2070 7269 6e74 2822 5265 6164  ose: print("Read
+0000db10: 696e 6720 736c 6162 206d 6f64 656c 206f  ing slab model o
+0000db20: 7574 7075 7420 6672 6f6d 3a20 222c 6d6f  utput from: ",mo
+0000db30: 6465 6c5f 7061 7468 290a 2020 2020 663d  del_path).    f=
+0000db40: 6f70 656e 286d 6f64 656c 5f70 6174 6829  open(model_path)
+0000db50: 0a20 2020 2064 6174 613d 736c 6162 5f64  .    data=slab_d
+0000db60: 6174 6128 290a 2020 2020 6e6d 6f64 656c  ata().    nmodel
+0000db70: 733d 696e 7428 662e 7265 6164 6c69 6e65  s=int(f.readline
+0000db80: 2829 2e73 706c 6974 2829 5b30 5d29 0a20  ().split()[0]). 
+0000db90: 2020 2064 6174 612e 6469 7265 6374 6f72     data.director
+0000dba0: 793d 6d6f 6465 6c5f 7061 7468 0a20 2020  y=model_path.   
+0000dbb0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+0000dbc0: 6e6d 6f64 656c 7329 3a0a 2020 2020 2020  nmodels):.      
+0000dbd0: 2020 2374 656d 706f 2020 2020 2020 2020    #tempo        
+0000dbe0: 2020 2020 2020 2020 3d20 2020 736c 6162          =   slab
+0000dbf0: 2829 0a20 2020 2020 2020 2074 656d 706f  ().        tempo
+0000dc00: 5f6d 6f64 656c 5f6e 756d 6265 723d 696e  _model_number=in
+0000dc10: 7428 662e 7265 6164 6c69 6e65 2829 2e73  t(f.readline().s
+0000dc20: 706c 6974 2829 5b30 5d29 0a20 2020 2020  plit()[0]).     
+0000dc30: 2020 206e 7370 6563 6965 733d 696e 7428     nspecies=int(
+0000dc40: 662e 7265 6164 6c69 6e65 2829 2e73 706c  f.readline().spl
+0000dc50: 6974 2829 5b30 5d29 0a20 2020 2020 2020  it()[0]).       
+0000dc60: 2023 7465 6d70 6f2e 7370 6563 6965 735f   #tempo.species_
+0000dc70: 6e75 6d62 6572 203d 2020 2069 6e74 2866  number =   int(f
+0000dc80: 2e72 6561 646c 696e 6528 292e 7370 6c69  .readline().spli
+0000dc90: 7428 295b 305d 290a 2020 2020 2020 2020  t()[0]).        
+0000dca0: 7465 6d70 6f5f 6e48 746f 743d 666c 6f61  tempo_nHtot=floa
+0000dcb0: 7428 662e 7265 6164 6c69 6e65 2829 2e73  t(f.readline().s
+0000dcc0: 706c 6974 2829 5b30 5d29 0a20 2020 2020  plit()[0]).     
+0000dcd0: 2020 2074 656d 706f 5f67 6173 4465 6e73     tempo_gasDens
+0000dce0: 3d66 6c6f 6174 2866 2e72 6561 646c 696e  =float(f.readlin
+0000dcf0: 6528 292e 7370 6c69 7428 295b 305d 290a  e().split()[0]).
+0000dd00: 2020 2020 2020 2020 7465 6d70 6f5f 6e65          tempo_ne
+0000dd10: 6c65 633d 666c 6f61 7428 662e 7265 6164  lec=float(f.read
+0000dd20: 6c69 6e65 2829 2e73 706c 6974 2829 5b30  line().split()[0
+0000dd30: 5d29 0a20 2020 2020 2020 2074 656d 706f  ]).        tempo
+0000dd40: 5f6e 4865 3d66 6c6f 6174 2866 2e72 6561  _nHe=float(f.rea
+0000dd50: 646c 696e 6528 292e 7370 6c69 7428 295b  dline().split()[
+0000dd60: 305d 290a 2020 2020 2020 2020 7465 6d70  0]).        temp
+0000dd70: 6f5f 6e48 4949 3d66 6c6f 6174 2866 2e72  o_nHII=float(f.r
+0000dd80: 6561 646c 696e 6528 292e 7370 6c69 7428  eadline().split(
+0000dd90: 295b 305d 290a 2020 2020 2020 2020 7465  )[0]).        te
+0000dda0: 6d70 6f5f 6e48 493d 666c 6f61 7428 662e  mpo_nHI=float(f.
+0000ddb0: 7265 6164 6c69 6e65 2829 2e73 706c 6974  readline().split
+0000ddc0: 2829 5b30 5d29 0a20 2020 2020 2020 2074  ()[0]).        t
+0000ddd0: 656d 706f 5f6e 4832 3d66 6c6f 6174 2866  empo_nH2=float(f
+0000dde0: 2e72 6561 646c 696e 6528 292e 7370 6c69  .readline().spli
+0000ddf0: 7428 295b 305d 290a 2020 2020 2020 2020  t()[0]).        
+0000de00: 7465 6d70 6f5f 6475 7374 5f74 6f5f 6761  tempo_dust_to_ga
+0000de10: 733d 666c 6f61 7428 662e 7265 6164 6c69  s=float(f.readli
+0000de20: 6e65 2829 2e73 706c 6974 2829 5b30 5d29  ne().split()[0])
+0000de30: 0a20 2020 2020 2020 2074 656d 706f 5f76  .        tempo_v
+0000de40: 7475 7262 3d66 6c6f 6174 2866 2e72 6561  turb=float(f.rea
+0000de50: 646c 696e 6528 292e 7370 6c69 7428 295b  dline().split()[
+0000de60: 305d 290a 2020 2020 2020 2020 7465 6d70  0]).        temp
+0000de70: 6f5f 5467 3d66 6c6f 6174 2866 2e72 6561  o_Tg=float(f.rea
+0000de80: 646c 696e 6528 292e 7370 6c69 7428 295b  dline().split()[
+0000de90: 305d 290a 2020 2020 2020 2020 7465 6d70  0]).        temp
+0000dea0: 6f5f 5464 3d66 6c6f 6174 2866 2e72 6561  o_Td=float(f.rea
+0000deb0: 646c 696e 6528 292e 7370 6c69 7428 295b  dline().split()[
+0000dec0: 305d 290a 2020 2020 2020 2020 6966 2073  0]).        if s
+0000ded0: 686f 7274 5f66 6f72 6d61 743a 0a20 2020  hort_format:.   
+0000dee0: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
+0000def0: 6e20 7261 6e67 6528 6e73 7065 6369 6573  n range(nspecies
+0000df00: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000df10: 2020 2074 656d 706f 3d73 6c61 6228 290a     tempo=slab().
+0000df20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df30: 7465 6d70 6f2e 6d6f 6465 6c5f 6e75 6d62  tempo.model_numb
+0000df40: 6572 3d74 656d 706f 5f6d 6f64 656c 5f6e  er=tempo_model_n
+0000df50: 756d 6265 720a 2020 2020 2020 2020 2020  umber.          
+0000df60: 2020 2020 2020 7465 6d70 6f2e 4e48 3d74        tempo.NH=t
+0000df70: 656d 706f 5f6e 4874 6f74 0a20 2020 2020  empo_nHtot.     
+0000df80: 2020 2020 2020 2020 2020 2074 656d 706f             tempo
+0000df90: 2e6e 436f 6c6c 3d74 656d 706f 5f67 6173  .nColl=tempo_gas
+0000dfa0: 4465 6e73 0a20 2020 2020 2020 2020 2020  Dens.           
+0000dfb0: 2020 2020 2074 656d 706f 2e6e 653d 7465       tempo.ne=te
+0000dfc0: 6d70 6f5f 6e65 6c65 630a 2020 2020 2020  mpo_nelec.      
+0000dfd0: 2020 2020 2020 2020 2020 7465 6d70 6f2e            tempo.
+0000dfe0: 6e48 653d 7465 6d70 6f5f 6e48 650a 2020  nHe=tempo_nHe.  
+0000dff0: 2020 2020 2020 2020 2020 2020 2020 7465                te
+0000e000: 6d70 6f2e 6e48 4949 3d74 656d 706f 5f6e  mpo.nHII=tempo_n
+0000e010: 4849 490a 2020 2020 2020 2020 2020 2020  HII.            
+0000e020: 2020 2020 7465 6d70 6f2e 6e48 493d 7465      tempo.nHI=te
+0000e030: 6d70 6f5f 6e48 490a 2020 2020 2020 2020  mpo_nHI.        
+0000e040: 2020 2020 2020 2020 7465 6d70 6f2e 6e48          tempo.nH
+0000e050: 323d 7465 6d70 6f5f 6e48 320a 2020 2020  2=tempo_nH2.    
+0000e060: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+0000e070: 6f2e 6475 7374 5f74 6f5f 6761 733d 7465  o.dust_to_gas=te
+0000e080: 6d70 6f5f 6475 7374 5f74 6f5f 6761 730a  mpo_dust_to_gas.
+0000e090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e0a0: 7465 6d70 6f2e 7674 7572 623d 7465 6d70  tempo.vturb=temp
+0000e0b0: 6f5f 7674 7572 620a 2020 2020 2020 2020  o_vturb.        
+0000e0c0: 2020 2020 2020 2020 7465 6d70 6f2e 5467          tempo.Tg
+0000e0d0: 3d74 656d 706f 5f54 670a 2020 2020 2020  =tempo_Tg.      
+0000e0e0: 2020 2020 2020 2020 2020 7465 6d70 6f2e            tempo.
+0000e0f0: 5464 3d74 656d 706f 5f54 640a 0a20 2020  Td=tempo_Td..   
+0000e100: 2020 2020 2020 2020 2020 2020 2074 656d               tem
+0000e110: 706f 2e73 7065 6369 6573 5f69 6e64 6578  po.species_index
+0000e120: 3d69 6e74 2866 2e72 6561 646c 696e 6528  =int(f.readline(
+0000e130: 292e 7370 6c69 7428 295b 305d 290a 2020  ).split()[0]).  
+0000e140: 2020 2020 2020 2020 2020 2020 2020 7465                te
+0000e150: 6d70 6f2e 7370 6563 6965 735f 6e75 6d62  mpo.species_numb
+0000e160: 6572 3d6a 2b31 0a20 2020 2020 2020 2020  er=j+1.         
+0000e170: 2020 2020 2020 2074 656d 706f 2e73 7065         tempo.spe
+0000e180: 6369 6573 5f6e 616d 653d 662e 7265 6164  cies_name=f.read
+0000e190: 6c69 6e65 2829 2e73 706c 6974 2829 5b30  line().split()[0
+0000e1a0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0000e1b0: 2020 7465 6d70 6f2e 6162 756e 6461 6e63    tempo.abundanc
+0000e1c0: 653d 666c 6f61 7428 662e 7265 6164 6c69  e=float(f.readli
+0000e1d0: 6e65 2829 2e73 706c 6974 2829 5b30 5d29  ne().split()[0])
+0000e1e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e1f0: 2074 656d 706f 2e64 763d 666c 6f61 7428   tempo.dv=float(
+0000e200: 662e 7265 6164 6c69 6e65 2829 2e73 706c  f.readline().spl
+0000e210: 6974 2829 5b30 5d29 0a20 2020 2020 2020  it()[0]).       
+0000e220: 2020 2020 2020 2020 2074 656d 706f 2e6e           tempo.n
+0000e230: 6c69 6e65 733d 696e 7428 662e 7265 6164  lines=int(f.read
+0000e240: 6c69 6e65 2829 2e73 706c 6974 2829 5b30  line().split()[0
+0000e250: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+0000e260: 2020 206c 696e 6573 3d66 2e72 6561 646c     lines=f.readl
+0000e270: 696e 6528 290a 0a20 2020 2020 2020 2020  ine()..         
+0000e280: 2020 2020 2020 2023 2074 656d 706f 2e6e         # tempo.n
+0000e290: 6c69 6e65 733d 4e6f 6e65 0a20 2020 2020  lines=None.     
+0000e2a0: 2020 2020 2020 2020 2020 2074 656d 706f             tempo
+0000e2b0: 2e6c 696e 6564 6174 613d 4e6f 6e65 0a20  .linedata=None. 
+0000e2c0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000e2d0: 656d 706f 2e6c 6576 656c 6461 7461 3d4e  empo.leveldata=N
+0000e2e0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+0000e2f0: 2020 2020 7465 6d70 6f2e 636f 6e76 5761      tempo.convWa
+0000e300: 7665 6c65 6e67 7468 3d4e 6f6e 650a 2020  velength=None.  
+0000e310: 2020 2020 2020 2020 2020 2020 2020 7465                te
+0000e320: 6d70 6f2e 636f 6e76 4c54 4566 6c75 783d  mpo.convLTEflux=
+0000e330: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+0000e340: 2020 2020 2074 656d 706f 2e63 6f6e 764e       tempo.convN
+0000e350: 4c54 4566 6c75 783d 4e6f 6e65 0a20 2020  LTEflux=None.   
+0000e360: 2020 2020 2020 2020 2020 2020 2074 656d               tem
+0000e370: 706f 2e63 6f6e 7654 7970 653d 4e6f 6e65  po.convType=None
 0000e380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e390: 2073 6c61 624f 7574 466f 726d 6174 3d5b   slabOutFormat=[
-0000e3a0: 392c 392c 392c 352c 352c 352c 3135 2c31  9,9,9,5,5,5,15,1
-0000e3b0: 352c 3135 2c31 352c 3135 2c31 352c 3135  5,15,15,15,15,15
-0000e3c0: 2c31 352c 3135 2c31 352c 3135 2c31 352c  ,15,15,15,15,15,
-0000e3d0: 3135 2c31 352c 3135 2c31 352c 3135 2c32  15,15,15,15,15,2
-0000e3e0: 312c 3231 2c32 312c 3231 5d0a 2020 2020  1,21,21,21].    
-0000e3f0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000e400: 6b20 696e 2072 616e 6765 2874 656d 706f  k in range(tempo
-0000e410: 2e6e 6c69 6e65 7329 3a0a 2020 2020 2020  .nlines):.      
-0000e420: 2020 2020 2020 2020 2020 2020 2020 6c69                li
-0000e430: 6e65 5265 6164 3d5b 5d0a 2020 2020 2020  neRead=[].      
-0000e440: 2020 2020 2020 2020 2020 2020 2020 6c69                li
-0000e450: 6e65 733d 662e 7265 6164 6c69 6e65 2829  nes=f.readline()
-0000e460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e470: 2020 2020 206c 3d30 0a20 2020 2020 2020       l=0.       
-0000e480: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000e490: 206c 656e 6774 6820 696e 2073 6c61 624f   length in slabO
-0000e4a0: 7574 466f 726d 6174 3a0a 2020 2020 2020  utFormat:.      
-0000e4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4c0: 2020 6c69 6e65 5265 6164 2e61 7070 656e    lineRead.appen
-0000e4d0: 6428 6c69 6e65 735b 6c3a 6c2b 6c65 6e67  d(lines[l:l+leng
-0000e4e0: 7468 5d29 0a20 2020 2020 2020 2020 2020  th]).           
-0000e4f0: 2020 2020 2020 2020 2020 2020 206c 2b3d               l+=
-0000e500: 6c65 6e67 7468 0a20 2020 2020 2020 2020  length.         
-0000e510: 2020 2020 2020 2020 2020 2064 6174 5b31             dat[1
-0000e520: 5d5b 6b2c 3a5d 3d6e 702e 6173 6172 7261  ][k,:]=np.asarra
-0000e530: 7928 5b66 6c6f 6174 2878 2920 666f 7220  y([float(x) for 
-0000e540: 7820 696e 206c 696e 6552 6561 645b 303a  x in lineRead[0:
-0000e550: 2d34 5d5d 290a 2020 2020 2020 2020 2020  -4]]).          
-0000e560: 2020 2020 2020 2020 2020 6461 745b 325d            dat[2]
-0000e570: 2e61 7070 656e 6428 5b61 2e73 7472 6970  .append([a.strip
-0000e580: 2829 2066 6f72 2061 2069 6e20 6c69 6e65  () for a in line
-0000e590: 5265 6164 5b2d 343a 5d5d 290a 0a20 2020  Read[-4:]])..   
-0000e5a0: 2020 2020 2020 2020 2020 2020 206c 696e               lin
-0000e5b0: 6544 6174 613d 7064 2e44 6174 6146 7261  eData=pd.DataFra
-0000e5c0: 6d65 2864 6174 5b31 5d2c 636f 6c75 6d6e  me(dat[1],column
-0000e5d0: 733d 5b27 6927 2c27 7527 2c27 6c27 2c27  s=['i','u','l','
-0000e5e0: 6527 2c27 7627 2c27 4a27 2c27 6775 272c  e','v','J','gu',
-0000e5f0: 2745 7527 2c27 4127 2c27 4227 2c27 4748  'Eu','A','B','GH
-0000e600: 7a27 2c27 7461 7544 272c 274a 6261 636b  z','tauD','Jback
-0000e610: 272c 2770 6f70 272c 276c 7465 706f 7027  ','pop','ltepop'
-0000e620: 2c27 7461 754e 4c54 4527 2c27 7461 754c  ,'tauNLTE','tauL
-0000e630: 5445 272c 2762 4e4c 5445 272c 2762 4c54  TE','bNLTE','bLT
-0000e640: 4527 2c27 704e 4c54 4527 2c27 704c 5445  E','pNLTE','pLTE
-0000e650: 272c 2746 4e4c 5445 272c 2746 4c54 4527  ','FNLTE','FLTE'
-0000e660: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-0000e670: 2020 206c 696e 6544 6174 615b 2767 6c6f     lineData['glo
-0000e680: 6261 6c5f 7527 5d3d 5b61 5b30 5d20 666f  bal_u']=[a[0] fo
-0000e690: 7220 6120 696e 2064 6174 5b32 5d5d 0a20  r a in dat[2]]. 
-0000e6a0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0000e6b0: 696e 6544 6174 615b 2767 6c6f 6261 6c5f  ineData['global_
-0000e6c0: 6c27 5d3d 5b61 5b31 5d20 666f 7220 6120  l']=[a[1] for a 
-0000e6d0: 696e 2064 6174 5b32 5d5d 0a20 2020 2020  in dat[2]].     
-0000e6e0: 2020 2020 2020 2020 2020 206c 696e 6544             lineD
-0000e6f0: 6174 615b 276c 6f63 616c 5f75 275d 3d5b  ata['local_u']=[
-0000e700: 615b 325d 2066 6f72 2061 2069 6e20 6461  a[2] for a in da
-0000e710: 745b 325d 5d0a 2020 2020 2020 2020 2020  t[2]].          
-0000e720: 2020 2020 2020 6c69 6e65 4461 7461 5b27        lineData['
-0000e730: 6c6f 6361 6c5f 6c27 5d3d 5b61 5b33 5d20  local_l']=[a[3] 
-0000e740: 666f 7220 6120 696e 2064 6174 5b32 5d5d  for a in dat[2]]
-0000e750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e760: 206c 6576 4461 7461 3d70 642e 4461 7461   levData=pd.Data
-0000e770: 4672 616d 6528 6461 745b 305d 2c63 6f6c  Frame(dat[0],col
-0000e780: 756d 6e73 3d5b 2769 272c 2767 272c 2745  umns=['i','g','E
-0000e790: 272c 2770 6f70 272c 276c 7465 706f 7027  ','pop','ltepop'
-0000e7a0: 2c27 6527 2c27 7627 2c27 4a27 5d29 0a20  ,'e','v','J']). 
-0000e7b0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000e7c0: 656d 706f 2e6c 696e 6564 6174 613d 6c69  empo.linedata=li
-0000e7d0: 6e65 4461 7461 0a20 2020 2020 2020 2020  neData.         
-0000e7e0: 2020 2020 2020 2074 656d 706f 2e6c 6576         tempo.lev
-0000e7f0: 656c 6461 7461 3d6c 6576 4461 7461 0a20  eldata=levData. 
-0000e800: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0000e810: 6174 612e 6164 645f 6d6f 6465 6c28 7465  ata.add_model(te
-0000e820: 6d70 6f29 0a20 2020 2072 6574 7572 6e28  mpo).    return(
-0000e830: 6461 7461 290a 0a0a 6465 6620 7265 6164  data)...def read
-0000e840: 5f6f 7665 726c 6170 5f73 7065 6374 7261  _overlap_spectra
-0000e850: 2870 6174 683d 2753 6c61 624f 7665 726c  (path='SlabOverl
-0000e860: 6170 2e6f 7574 272c 7665 7262 6f73 653d  ap.out',verbose=
-0000e870: 5472 7565 293a 0a20 2020 2022 2222 0a20  True):.    """. 
-0000e880: 2020 2046 756e 6374 696f 6e20 746f 2072     Function to r
-0000e890: 6561 6420 3044 2070 726f 6469 6d6f 2073  ead 0D prodimo s
-0000e8a0: 6c61 6220 6d6f 6465 6c20 6f75 7470 7574  lab model output
-0000e8b0: 2077 6974 6820 6c69 6e65 206f 7665 726c   with line overl
-0000e8c0: 6170 0a20 2020 2022 2222 0a0a 2020 2020  ap.    """..    
-0000e8d0: 6966 2069 7369 6e73 7461 6e63 6528 7061  if isinstance(pa
-0000e8e0: 7468 2c6c 6973 7429 3a0a 2020 2020 2020  th,list):.      
-0000e8f0: 2020 6461 7461 3d73 6c61 625f 6461 7461    data=slab_data
-0000e900: 2829 0a20 2020 2020 2020 2064 6174 612e  ().        data.
-0000e910: 6469 7265 6374 6f72 793d 7061 7468 0a20  directory=path. 
-0000e920: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-0000e930: 7061 7468 3a0a 2020 2020 2020 2020 2020  path:.          
-0000e940: 2020 7264 6174 613d 7265 6164 5f6f 7665    rdata=read_ove
-0000e950: 726c 6170 5f73 7065 6374 7261 2869 2c76  rlap_spectra(i,v
-0000e960: 6572 626f 7365 3d76 6572 626f 7365 290a  erbose=verbose).
-0000e970: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000e980: 6a20 696e 2072 616e 6765 2872 6461 7461  j in range(rdata
-0000e990: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
-0000e9a0: 2020 2020 2020 2020 2020 2064 6174 612e             data.
-0000e9b0: 6164 645f 6d6f 6465 6c28 7264 6174 612e  add_model(rdata.
-0000e9c0: 6d6f 6465 6c73 5b6a 5d29 0a20 2020 2020  models[j]).     
-0000e9d0: 2020 2072 6574 7572 6e28 6461 7461 290a     return(data).
-0000e9e0: 0a20 2020 2069 6620 7665 7262 6f73 653a  .    if verbose:
-0000e9f0: 2070 7269 6e74 2822 5265 6164 696e 6720   print("Reading 
-0000ea00: 736c 6162 206c 696e 6520 6f76 6572 6c61  slab line overla
-0000ea10: 7020 6d6f 6465 6c20 6f75 7470 7574 2066  p model output f
-0000ea20: 726f 6d3a 2022 2c70 6174 6829 0a20 2020  rom: ",path).   
-0000ea30: 2069 6620 272e 6669 7473 2e67 7a27 2069   if '.fits.gz' i
-0000ea40: 6e20 7061 7468 3a0a 2020 2020 2020 2020  n path:.        
-0000ea50: 6864 756c 3d66 6974 732e 6f70 656e 2870  hdul=fits.open(p
-0000ea60: 6174 6829 0a20 2020 2020 2020 2064 6174  ath).        dat
-0000ea70: 613d 736c 6162 5f64 6174 6128 290a 2020  a=slab_data().  
-0000ea80: 2020 2020 2020 6e6d 6f64 656c 733d 6864        nmodels=hd
-0000ea90: 756c 5b30 5d2e 6865 6164 6572 5b27 4e4d  ul[0].header['NM
-0000eaa0: 4f44 454c 5327 5d0a 2020 2020 2020 2020  ODELS'].        
-0000eab0: 6461 7461 2e64 6972 6563 746f 7279 3d70  data.directory=p
-0000eac0: 6174 680a 2020 2020 2020 2020 666f 7220  ath.        for 
-0000ead0: 6920 696e 2072 616e 6765 286e 6d6f 6465  i in range(nmode
-0000eae0: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
-0000eaf0: 2074 656d 706f 3d73 6c61 6228 290a 2020   tempo=slab().  
-0000eb00: 2020 2020 2020 2020 2020 7465 6d70 6f5f            tempo_
-0000eb10: 6d6f 6465 6c5f 6e75 6d62 6572 3d68 6475  model_number=hdu
-0000eb20: 6c5b 692b 315d 2e68 6561 6465 725b 274d  l[i+1].header['M
-0000eb30: 4f44 454c 275d 0a20 2020 2020 2020 2020  ODEL'].         
-0000eb40: 2020 2074 656d 706f 5f4e 6c69 6e65 3d68     tempo_Nline=h
-0000eb50: 6475 6c5b 692b 315d 2e68 6561 6465 725b  dul[i+1].header[
-0000eb60: 274e 4c49 4e45 275d 0a20 2020 2020 2020  'NLINE'].       
-0000eb70: 2020 2020 2074 656d 706f 5f52 3d68 6475       tempo_R=hdu
-0000eb80: 6c5b 692b 315d 2e68 6561 6465 725b 2752  l[i+1].header['R
-0000eb90: 5f4f 564c 5027 5d0a 2020 2020 2020 2020  _OVLP'].        
-0000eba0: 2020 2020 6461 7474 613d 5b5d 0a20 2020      datta=[].   
-0000ebb0: 2020 2020 2020 2020 2074 656d 706f 2e6f           tempo.o
-0000ebc0: 7665 726c 6170 4672 6571 3d68 6475 6c5b  verlapFreq=hdul[
-0000ebd0: 692b 315d 2e64 6174 615b 3a2c 2d31 5d0a  i+1].data[:,-1].
-0000ebe0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-0000ebf0: 6f2e 6f76 6572 6c61 704c 5445 3d68 6475  o.overlapLTE=hdu
-0000ec00: 6c5b 692b 315d 2e64 6174 615b 3a2c 305d  l[i+1].data[:,0]
-0000ec10: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
-0000ec20: 706f 2e6f 7665 726c 6170 5461 754c 5445  po.overlapTauLTE
-0000ec30: 3d68 6475 6c5b 692b 315d 2e64 6174 615b  =hdul[i+1].data[
-0000ec40: 3a2c 315d 0a20 2020 2020 2020 2020 2020  :,1].           
-0000ec50: 2074 656d 706f 2e6f 7665 726c 6170 4e4c   tempo.overlapNL
-0000ec60: 5445 3d68 6475 6c5b 692b 315d 2e64 6174  TE=hdul[i+1].dat
-0000ec70: 615b 3a2c 325d 0a20 2020 2020 2020 2020  a[:,2].         
-0000ec80: 2020 2074 656d 706f 2e6f 7665 726c 6170     tempo.overlap
-0000ec90: 5461 754e 4c54 453d 6864 756c 5b69 2b31  TauNLTE=hdul[i+1
-0000eca0: 5d2e 6461 7461 5b3a 2c33 5d0a 2020 2020  ].data[:,3].    
-0000ecb0: 2020 2020 2020 2020 7465 6d70 6f2e 6f76          tempo.ov
-0000ecc0: 6572 6c61 7052 3d74 656d 706f 5f52 0a20  erlapR=tempo_R. 
-0000ecd0: 2020 2020 2020 2020 2020 2074 656d 706f             tempo
-0000ece0: 2e6d 6f64 656c 5f6e 756d 6265 723d 6864  .model_number=hd
-0000ecf0: 756c 5b69 2b31 5d2e 6865 6164 6572 5b27  ul[i+1].header['
-0000ed00: 4d4f 4445 4c27 5d0a 2020 2020 2020 2020  MODEL'].        
-0000ed10: 2020 2020 7465 6d70 6f2e 5467 3d68 6475      tempo.Tg=hdu
-0000ed20: 6c5b 692b 315d 2e68 6561 6465 725b 2754  l[i+1].header['T
-0000ed30: 4727 5d0a 2020 2020 2020 2020 2020 2020  G'].            
-0000ed40: 7465 6d70 6f2e 5464 3d68 6475 6c5b 692b  tempo.Td=hdul[i+
-0000ed50: 315d 2e68 6561 6465 725b 2754 4427 5d0a  1].header['TD'].
-0000ed60: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-0000ed70: 6f2e 7674 7572 623d 6864 756c 5b69 2b31  o.vturb=hdul[i+1
-0000ed80: 5d2e 6865 6164 6572 5b27 5654 5552 4227  ].header['VTURB'
-0000ed90: 5d0a 2020 2020 2020 2020 2020 2020 7465  ].            te
-0000eda0: 6d70 6f2e 4e48 3d68 6475 6c5b 692b 315d  mpo.NH=hdul[i+1]
-0000edb0: 2e68 6561 6465 725b 274e 4854 4f54 275d  .header['NHTOT']
-0000edc0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-0000edd0: 612e 6164 645f 6d6f 6465 6c28 7465 6d70  a.add_model(temp
-0000ede0: 6f29 0a20 2020 2020 2020 2020 2020 2023  o).            #
-0000edf0: 2070 7269 6e74 2827 7265 6164 2027 2c69   print('read ',i
-0000ee00: 2c27 206d 6f64 656c 2729 0a20 2020 2065  ,' model').    e
-0000ee10: 6c73 653a 0a20 2020 2020 2020 2066 3d6f  lse:.        f=o
-0000ee20: 7065 6e28 7061 7468 290a 2020 2020 2020  pen(path).      
-0000ee30: 2020 6461 7461 3d73 6c61 625f 6461 7461    data=slab_data
-0000ee40: 2829 0a20 2020 2020 2020 206e 6d6f 6465  ().        nmode
-0000ee50: 6c73 3d69 6e74 2866 2e72 6561 646c 696e  ls=int(f.readlin
-0000ee60: 6528 292e 7370 6c69 7428 295b 305d 290a  e().split()[0]).
-0000ee70: 2020 2020 2020 2020 6461 7461 2e64 6972          data.dir
-0000ee80: 6563 746f 7279 3d70 6174 680a 2020 2020  ectory=path.    
-0000ee90: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-0000eea0: 6765 286e 6d6f 6465 6c73 293a 0a20 2020  ge(nmodels):.   
-0000eeb0: 2020 2020 2020 2020 2074 656d 706f 3d73           tempo=s
-0000eec0: 6c61 6228 290a 2020 2020 2020 2020 2020  lab().          
-0000eed0: 2020 7465 6d70 6f5f 6d6f 6465 6c5f 6e75    tempo_model_nu
-0000eee0: 6d62 6572 3d69 6e74 2866 2e72 6561 646c  mber=int(f.readl
-0000eef0: 696e 6528 292e 7370 6c69 7428 295b 305d  ine().split()[0]
-0000ef00: 290a 2020 2020 2020 2020 2020 2020 7465  ).            te
-0000ef10: 6d70 6f5f 4e6c 696e 653d 696e 7428 662e  mpo_Nline=int(f.
-0000ef20: 7265 6164 6c69 6e65 2829 2e73 706c 6974  readline().split
-0000ef30: 2829 5b30 5d29 0a20 2020 2020 2020 2020  ()[0]).         
-0000ef40: 2020 2074 656d 706f 5f52 3d66 6c6f 6174     tempo_R=float
-0000ef50: 2866 2e72 6561 646c 696e 6528 292e 7370  (f.readline().sp
-0000ef60: 6c69 7428 295b 305d 290a 2020 2020 2020  lit()[0]).      
-0000ef70: 2020 2020 2020 6461 7474 613d 5b5d 0a20        datta=[]. 
-0000ef80: 2020 2020 2020 2020 2020 206c 696e 6573             lines
-0000ef90: 3d66 2e72 6561 646c 696e 6528 290a 2020  =f.readline().  
-0000efa0: 2020 2020 2020 2020 2020 666f 7220 6a20            for j 
-0000efb0: 696e 2072 616e 6765 2874 656d 706f 5f4e  in range(tempo_N
-0000efc0: 6c69 6e65 293a 0a20 2020 2020 2020 2020  line):.         
-0000efd0: 2020 2020 2020 206c 696e 6573 3d66 2e72         lines=f.r
-0000efe0: 6561 646c 696e 6528 290a 2020 2020 2020  eadline().      
-0000eff0: 2020 2020 2020 2020 2020 6461 7474 612e            datta.
-0000f000: 6170 7065 6e64 286e 702e 6172 7261 7928  append(np.array(
-0000f010: 6c69 6e65 732e 7370 6c69 7428 292c 6474  lines.split(),dt
-0000f020: 7970 653d 666c 6f61 7429 290a 2020 2020  ype=float)).    
-0000f030: 2020 2020 2020 2020 6461 7474 613d 6e70          datta=np
-0000f040: 2e61 7272 6179 2864 6174 7461 290a 2020  .array(datta).  
-0000f050: 2020 2020 2020 2020 2020 7465 6d70 6f2e            tempo.
-0000f060: 6f76 6572 6c61 7046 7265 713d 6461 7474  overlapFreq=datt
-0000f070: 615b 3a2c 305d 0a20 2020 2020 2020 2020  a[:,0].         
-0000f080: 2020 2074 656d 706f 2e6f 7665 726c 6170     tempo.overlap
-0000f090: 4c54 453d 6461 7474 615b 3a2c 315d 0a20  LTE=datta[:,1]. 
-0000f0a0: 2020 2020 2020 2020 2020 2074 656d 706f             tempo
-0000f0b0: 2e6f 7665 726c 6170 5461 754c 5445 3d64  .overlapTauLTE=d
-0000f0c0: 6174 7461 5b3a 2c32 5d0a 2020 2020 2020  atta[:,2].      
-0000f0d0: 2020 2020 2020 7465 6d70 6f2e 6f76 6572        tempo.over
-0000f0e0: 6c61 704e 4c54 453d 6461 7474 615b 3a2c  lapNLTE=datta[:,
-0000f0f0: 335d 0a20 2020 2020 2020 2020 2020 2074  3].            t
-0000f100: 656d 706f 2e6f 7665 726c 6170 5461 754e  empo.overlapTauN
-0000f110: 4c54 453d 6461 7474 615b 3a2c 345d 0a20  LTE=datta[:,4]. 
-0000f120: 2020 2020 2020 2020 2020 2074 656d 706f             tempo
-0000f130: 2e6f 7665 726c 6170 523d 7465 6d70 6f5f  .overlapR=tempo_
-0000f140: 520a 2020 2020 2020 2020 2020 2020 6461  R.            da
-0000f150: 7461 2e61 6464 5f6d 6f64 656c 2874 656d  ta.add_model(tem
-0000f160: 706f 290a 2020 2020 2020 2020 2020 2020  po).            
-0000f170: 6c69 6e65 733d 662e 7265 6164 6c69 6e65  lines=f.readline
-0000f180: 2829 0a20 2020 2020 2020 2020 2020 2023  ().            #
-0000f190: 2070 7269 6e74 2827 7265 6164 2027 2c69   print('read ',i
-0000f1a0: 2c27 206d 6f64 656c 2729 0a20 2020 200a  ,' model').    .
-0000f1b0: 2020 2020 7265 7475 726e 2864 6174 6129      return(data)
-0000f1c0: 0a0a 0a64 6566 2073 7065 6343 6f6e 766f  ...def specConvo
-0000f1d0: 6c76 6528 6c69 6e65 5374 7265 6e67 7468  lve(lineStrength
-0000f1e0: 732c 6c69 6e65 4672 6571 2c66 7265 715f  s,lineFreq,freq_
-0000f1f0: 6269 6e73 3d4e 6f6e 652c 523d 312c 6c61  bins=None,R=1,la
-0000f200: 6d62 6461 5f30 3d31 2c6c 616d 6264 615f  mbda_0=1,lambda_
-0000f210: 6e3d 312c 7672 3d31 3330 3029 3a0a 2020  n=1,vr=1300):.  
-0000f220: 2020 2222 220a 2020 2020 4e4f 5420 5553    """.    NOT US
-0000f230: 4544 2041 4e59 4d4f 5245 0a20 2020 2046  ED ANYMORE.    F
-0000f240: 756e 6374 696f 6e20 746f 2063 6f6e 766f  unction to convo
-0000f250: 6c76 6520 6c69 6e65 7320 696e 746f 2073  lve lines into s
-0000f260: 7065 6374 7261 2062 7920 7369 6d70 6c79  pectra by simply
-0000f270: 2062 696e 6e69 6e67 2074 6865 6d20 696e   binning them in
-0000f280: 746f 2061 2077 6176 656c 656e 6774 6820  to a wavelength 
-0000f290: 6772 6964 0a20 2020 2022 2222 0a20 2020  grid.    """.   
-0000f2a0: 2067 5065 7263 3d6c 616d 6264 6120 782c   gPerc=lambda x,
-0000f2b0: 6d2c 733a 2073 6572 6628 2878 2d6d 292f  m,s: serf((x-m)/
-0000f2c0: 7329 2a30 2e35 2b30 2e35 0a20 2020 206e  s)*0.5+0.5.    n
-0000f2d0: 755f 696a 3d6c 696e 6546 7265 712a 3165  u_ij=lineFreq*1e
-0000f2e0: 390a 2020 2020 6966 206c 616d 6264 615f  9.    if lambda_
-0000f2f0: 6e3d 3d6c 616d 6264 615f 303a 0a20 2020  n==lambda_0:.   
-0000f300: 2020 2020 206c 616d 6264 615f 6e3d 6e70       lambda_n=np
-0000f310: 2e61 6d61 7828 632f 6e75 5f69 6a2a 3165  .amax(c/nu_ij*1e
-0000f320: 3629 2a32 0a20 2020 2069 6620 7479 7065  6)*2.    if type
-0000f330: 2866 7265 715f 6269 6e73 293d 3d74 7970  (freq_bins)==typ
-0000f340: 6528 4e6f 6e65 293a 0a20 2020 2020 2020  e(None):.       
-0000f350: 206e 753d 6765 6e65 7261 7465 5f67 7269   nu=generate_gri
-0000f360: 6428 523d 522c 6c61 6d62 6461 5f30 3d6c  d(R=R,lambda_0=l
-0000f370: 616d 6264 615f 302c 6c61 6d62 6461 5f6e  ambda_0,lambda_n
-0000f380: 3d6c 616d 6264 615f 6e29 2a31 6539 0a20  =lambda_n)*1e9. 
-0000f390: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000f3a0: 2066 7265 715f 6269 6e73 3d6e 702e 636f   freq_bins=np.co
-0000f3b0: 6e63 6174 656e 6174 6528 2866 7265 715f  ncatenate((freq_
-0000f3c0: 6269 6e73 2c6e 702e 6172 7261 7928 5b28  bins,np.array([(
-0000f3d0: 6672 6571 5f62 696e 735b 2d31 5d2d 6672  freq_bins[-1]-fr
-0000f3e0: 6571 5f62 696e 735b 2d32 5d29 2b66 7265  eq_bins[-2])+fre
-0000f3f0: 715f 6269 6e73 5b2d 315d 5d29 2929 0a20  q_bins[-1]]))). 
-0000f400: 2020 2020 2020 206e 753d 6672 6571 5f62         nu=freq_b
-0000f410: 696e 732a 3165 390a 2020 2020 6e75 5f69  ins*1e9.    nu_i
-0000f420: 6a5f 7469 6c65 3d6e 702e 7469 6c65 286e  j_tile=np.tile(n
-0000f430: 755f 696a 2c5b 6c65 6e28 6e75 292c 315d  u_ij,[len(nu),1]
-0000f440: 290a 2020 2020 6e75 5f74 696c 653d 6e70  ).    nu_tile=np
-0000f450: 2e74 696c 6528 6e75 2c5b 6c65 6e28 6e75  .tile(nu,[len(nu
-0000f460: 5f69 6a29 2c31 5d29 0a20 2020 206c 696e  _ij),1]).    lin
-0000f470: 6553 7472 656e 6774 6873 5f74 696c 653d  eStrengths_tile=
-0000f480: 6e70 2e74 696c 6528 6c69 6e65 5374 7265  np.tile(lineStre
-0000f490: 6e67 7468 732c 5b6c 656e 286e 7529 2c31  ngths,[len(nu),1
-0000f4a0: 5d29 0a20 2020 2070 6572 635f 7469 6c65  ]).    perc_tile
-0000f4b0: 3d67 5065 7263 286e 755f 7469 6c65 2c6e  =gPerc(nu_tile,n
-0000f4c0: 755f 696a 5f74 696c 652e 542c 6e75 5f69  u_ij_tile.T,nu_i
-0000f4d0: 6a5f 7469 6c65 2e54 2f63 2a76 7229 0a20  j_tile.T/c*vr). 
-0000f4e0: 2020 2078 3d70 6572 635f 7469 6c65 5b3a     x=perc_tile[:
-0000f4f0: 2c3a 2d31 5d2d 7065 7263 5f74 696c 655b  ,:-1]-perc_tile[
-0000f500: 3a2c 313a 5d0a 2020 2020 7761 7665 6c65  :,1:].    wavele
-0000f510: 6e67 7468 2c66 6c75 783d 632f 6e75 5b3a  ngth,flux=c/nu[:
-0000f520: 2d31 5d2a 3165 362c 6e70 2e73 756d 2878  -1]*1e6,np.sum(x
-0000f530: 2a6c 696e 6553 7472 656e 6774 6873 5f74  *lineStrengths_t
-0000f540: 696c 655b 3a2d 312c 3a5d 2e54 2c61 7869  ile[:-1,:].T,axi
-0000f550: 733d 3029 2f28 6e75 5b3a 2d31 5d2d 6e75  s=0)/(nu[:-1]-nu
-0000f560: 5b31 3a5d 290a 2020 2020 7265 7475 726e  [1:]).    return
-0000f570: 2077 6176 656c 656e 6774 682c 666c 7578   wavelength,flux
-0000f580: 0a0a 0a64 6566 2067 656e 6572 616c 436f  ...def generalCo
-0000f590: 6e76 6f6c 7665 286c 696e 6553 7472 656e  nvolve(lineStren
-0000f5a0: 6774 6873 2c6c 696e 6546 7265 712c 523d  gths,lineFreq,R=
-0000f5b0: 312c 6c61 6d62 6461 5f30 3d31 2c6c 616d  1,lambda_0=1,lam
-0000f5c0: 6264 615f 6e3d 312c 525f 6261 636b 3d31  bda_n=1,R_back=1
-0000f5d0: 6536 293a 0a20 2020 2022 2222 0a20 2020  e6):.    """.   
-0000f5e0: 2046 756e 6374 696f 6e20 746f 2063 6f6e   Function to con
-0000f5f0: 766f 6c76 6520 6c69 6e65 2066 6c75 7865  volve line fluxe
-0000f600: 7320 696e 746f 206c 696e 6520 7370 6563  s into line spec
-0000f610: 7472 6120 6261 7365 6420 6f6e 2061 2075  tra based on a u
-0000f620: 7365 7220 6465 6669 6e65 6420 7370 6563  ser defined spec
-0000f630: 7472 616c 2072 6573 6f6c 7669 6e67 2070  tral resolving p
-0000f640: 6f77 6572 2052 0a20 2020 2022 2222 0a20  ower R.    """. 
-0000f650: 2020 2069 6620 6c61 6d62 6461 5f6e 3d3d     if lambda_n==
-0000f660: 6c61 6d62 6461 5f30 3a0a 2020 2020 2020  lambda_0:.      
-0000f670: 2020 6c61 6d62 6461 5f6e 3d63 2f6e 702e    lambda_n=c/np.
-0000f680: 616d 696e 286c 696e 6546 7265 7129 2a31  amin(lineFreq)*1
-0000f690: 652d 332a 320a 2020 2020 6672 6571 5f62  e-3*2.    freq_b
-0000f6a0: 696e 733d 6765 6e65 7261 7465 5f67 7269  ins=generate_gri
-0000f6b0: 6428 525f 6261 636b 2c6c 616d 6264 615f  d(R_back,lambda_
-0000f6c0: 302c 6c61 6d62 6461 5f6e 290a 2020 2020  0,lambda_n).    
-0000f6d0: 7761 7665 5f62 696e 733d 632f 6672 6571  wave_bins=c/freq
-0000f6e0: 5f62 696e 732a 3165 2d33 0a20 2020 2066  _bins*1e-3.    f
-0000f6f0: 6c75 785f 6269 6e73 3d77 6176 655f 6269  lux_bins=wave_bi
-0000f700: 6e73 2a30 2e30 0a20 2020 2069 3d36 0a20  ns*0.0.    i=6. 
-0000f710: 2020 2053 3d6c 696e 6553 7472 656e 6774     S=lineStrengt
-0000f720: 6873 0a20 2020 2046 3d6c 696e 6546 7265  hs.    F=lineFre
-0000f730: 710a 2020 2020 696e 643d 6e70 2e64 6967  q.    ind=np.dig
-0000f740: 6974 697a 6528 462c 6e70 2e66 6c69 7028  itize(F,np.flip(
-0000f750: 6672 6571 5f62 696e 7329 5b3a 2d31 5d29  freq_bins)[:-1])
-0000f760: 0a20 2020 2066 6f72 2069 2c69 6478 2069  .    for i,idx i
-0000f770: 6e20 656e 756d 6572 6174 6528 696e 6429  n enumerate(ind)
-0000f780: 3a0a 2020 2020 2020 2020 666c 7578 5f62  :.        flux_b
-0000f790: 696e 735b 6964 785d 2b3d 535b 695d 0a0a  ins[idx]+=S[i]..
-0000f7a0: 2020 2020 4657 484d 3d52 5f62 6163 6b2f      FWHM=R_back/
-0000f7b0: 522f 322e 3335 350a 2020 2020 673d 4761  R/2.355.    g=Ga
-0000f7c0: 7573 7369 616e 3144 4b65 726e 656c 2873  ussian1DKernel(s
-0000f7d0: 7464 6465 763d 4657 484d 2c66 6163 746f  tddev=FWHM,facto
-0000f7e0: 723d 3729 0a20 2020 2041 3d61 7079 5f63  r=7).    A=apy_c
-0000f7f0: 6f6e 766f 6c76 6528 666c 7578 5f62 696e  onvolve(flux_bin
-0000f800: 732c 6729 0a20 2020 2041 3d41 5b31 3a5d  s,g).    A=A[1:]
-0000f810: 2f28 6e70 2e66 6c69 7028 6672 6571 5f62  /(np.flip(freq_b
-0000f820: 696e 7329 5b31 3a5d 2d6e 702e 666c 6970  ins)[1:]-np.flip
-0000f830: 2866 7265 715f 6269 6e73 295b 3a2d 315d  (freq_bins)[:-1]
-0000f840: 292a 3165 2d39 0a20 2020 2057 3d6e 702e  )*1e-9.    W=np.
-0000f850: 666c 6970 2877 6176 655f 6269 6e73 5b31  flip(wave_bins[1
-0000f860: 3a5d 290a 2020 2020 7265 7475 726e 206e  :]).    return n
-0000f870: 702e 666c 6970 2857 292c 6e70 2e66 6c69  p.flip(W),np.fli
-0000f880: 7028 4129 0a0a 0a64 6566 2067 656e 6572  p(A)...def gener
-0000f890: 6174 655f 6772 6964 2852 3d31 2c6c 616d  ate_grid(R=1,lam
-0000f8a0: 6264 615f 303d 312c 6c61 6d62 6461 5f6e  bda_0=1,lambda_n
-0000f8b0: 3d31 2c73 616d 706c 696e 673d 3129 3a0a  =1,sampling=1):.
-0000f8c0: 2020 2020 2222 220a 2020 2020 4765 6e65      """.    Gene
-0000f8d0: 7261 7465 2061 2073 7065 6374 7261 6c20  rate a spectral 
-0000f8e0: 6772 6964 2069 6e20 4748 7a0a 2020 2020  grid in GHz.    
-0000f8f0: 2222 220a 2020 2020 6465 6c5f 6c6f 676c  """.    del_logl
-0000f900: 616d 3d6e 702e 6c6f 6731 3028 312e 302b  am=np.log10(1.0+
-0000f910: 312e 302f 5229 0a20 2020 204e 3d31 2b69  1.0/R).    N=1+i
-0000f920: 6e74 286e 702e 6c6f 6731 3028 6c61 6d62  nt(np.log10(lamb
-0000f930: 6461 5f6e 2f6c 616d 6264 615f 3029 2f64  da_n/lambda_0)/d
-0000f940: 656c 5f6c 6f67 6c61 6d29 0a20 2020 206d  el_loglam).    m
-0000f950: 776c 736c 696e 653d 6e70 2e6c 6f67 7370  wlsline=np.logsp
-0000f960: 6163 6528 6e70 2e6c 6f67 3130 286c 616d  ace(np.log10(lam
-0000f970: 6264 615f 3029 2c6e 702e 6c6f 6731 3028  bda_0),np.log10(
-0000f980: 6c61 6d62 6461 5f6e 292c 696e 7428 4e2a  lambda_n),int(N*
-0000f990: 7361 6d70 6c69 6e67 2929 0a20 2020 206e  sampling)).    n
-0000f9a0: 753d 632f 6d77 6c73 6c69 6e65 2a31 6536  u=c/mwlsline*1e6
-0000f9b0: 0a20 2020 2072 6574 7572 6e28 6e75 2a31  .    return(nu*1
-0000f9c0: 652d 3929 0a0a 0a64 6566 2063 6f6e 766f  e-9)...def convo
-0000f9d0: 6c76 6528 6d6f 6465 6c73 2c66 7265 715f  lve(models,freq_
-0000f9e0: 6269 6e73 3d4e 6f6e 652c 523d 312c 6c61  bins=None,R=1,la
-0000f9f0: 6d62 6461 5f30 3d31 2c6c 616d 6264 615f  mbda_0=1,lambda_
-0000fa00: 6e3d 312c 7672 3d31 3330 302c 4e4c 5445  n=1,vr=1300,NLTE
-0000fa10: 3d46 616c 7365 2c63 6f6e 765f 7479 7065  =False,conv_type
-0000fa20: 3d31 2c76 6572 626f 7365 3d54 7275 6529  =1,verbose=True)
-0000fa30: 3a0a 2020 2020 2222 220a 2020 2020 5361  :.    """.    Sa
-0000fa40: 6d65 2061 7320 2e63 6f6e 766f 6c76 6528  me as .convolve(
-0000fa50: 2920 6d65 7468 6f64 0a20 2020 2022 2222  ) method.    """
-0000fa60: 0a20 2020 2066 6f72 2069 2c64 2069 6e20  .    for i,d in 
-0000fa70: 656e 756d 6572 6174 6528 6d6f 6465 6c73  enumerate(models
-0000fa80: 293a 0a20 2020 2020 2020 2069 6620 7665  ):.        if ve
-0000fa90: 7262 6f73 653a 2070 7269 6e74 2827 5c6e  rbose: print('\n
-0000faa0: 5c6e 4d6f 6465 6c20 272c 692b 3129 0a20  \nModel ',i+1). 
-0000fab0: 2020 2020 2020 2064 2e63 6f6e 766f 6c76         d.convolv
-0000fac0: 6528 6672 6571 5f62 696e 733d 6672 6571  e(freq_bins=freq
-0000fad0: 5f62 696e 732c 523d 522c 6c61 6d62 6461  _bins,R=R,lambda
-0000fae0: 5f30 3d6c 616d 6264 615f 302c 6c61 6d62  _0=lambda_0,lamb
-0000faf0: 6461 5f6e 3d6c 616d 6264 615f 6e2c 7672  da_n=lambda_n,vr
-0000fb00: 3d76 722c 4e4c 5445 3d4e 4c54 452c 636f  =vr,NLTE=NLTE,co
-0000fb10: 6e76 5f74 7970 653d 636f 6e76 5f74 7970  nv_type=conv_typ
-0000fb20: 6529 0a20 2020 2072 6574 7572 6e20 6d6f  e).    return mo
-0000fb30: 6465 6c73 0a0a 0a64 6566 2067 656e 6572  dels...def gener
-0000fb40: 6174 655f 736c 6162 5f67 7269 6428 6469  ate_slab_grid(di
-0000fb50: 7265 6374 6f72 793d 272e 272c 6772 6964  rectory='.',grid
-0000fb60: 5f70 6172 616d 6574 6572 733d 7b7d 2c63  _parameters={},c
-0000fb70: 6f6d 6269 6e61 7469 6f6e 3d46 616c 7365  ombination=False
-0000fb80: 2c4e 746f 743d 4e6f 6e65 2c54 673d 4e6f  ,Ntot=None,Tg=No
-0000fb90: 6e65 2c6e 4870 6c75 733d 4e6f 6e65 2c6e  ne,nHplus=None,n
-0000fba0: 4831 3d4e 6f6e 652c 6e48 323d 4e6f 6e65  H1=None,nH2=None
-0000fbb0: 2c6e 4865 3d4e 6f6e 652c 6e65 6c65 633d  ,nHe=None,nelec=
-0000fbc0: 4e6f 6e65 2c54 643d 4e6f 6e65 2c76 7475  None,Td=None,vtu
-0000fbd0: 7262 3d4e 6f6e 652c 6475 7374 5f74 6f5f  rb=None,dust_to_
-0000fbe0: 6761 733d 4e6f 6e65 2c52 5f6f 7665 726c  gas=None,R_overl
-0000fbf0: 6170 3d4e 6f6e 652c 6c69 6e65 5f6f 7665  ap=None,line_ove
-0000fc00: 726c 6170 3d4e 6f6e 652c 7370 6563 6965  rlap=None,specie
-0000fc10: 735f 6c69 7374 3d7b 7d2c 6f75 7470 7574  s_list={},output
-0000fc20: 5f66 696c 656e 616d 653d 2753 6c61 6252  _filename='SlabR
-0000fc30: 6573 756c 7473 2e6f 7574 272c 6f76 6572  esults.out',over
-0000fc40: 6c61 705f 6669 6c65 6e61 6d65 3d27 536c  lap_filename='Sl
-0000fc50: 6162 4f76 6572 6c61 702e 6f75 7427 2c73  abOverlap.out',s
-0000fc60: 6570 6172 6174 655f 6f70 5f66 696c 6573  eparate_op_files
-0000fc70: 3d54 7275 652c 736c 6162 5f52 543d 5472  =True,slab_RT=Tr
-0000fc80: 7565 2c73 686f 7274 5f66 6f72 6d61 743d  ue,short_format=
-0000fc90: 4661 6c73 652c 6e6f 5f69 6e64 6976 6964  False,no_individ
-0000fca0: 7561 6c5f 6c69 6e65 733d 4661 6c73 652c  ual_lines=False,
-0000fcb0: 6669 7473 5f6f 705f 6669 6c65 733d 4661  fits_op_files=Fa
-0000fcc0: 6c73 6529 3a0a 2020 2020 2222 220a 2020  lse):.    """.  
-0000fcd0: 2020 4675 6e63 7469 6f6e 2074 6f20 6765    Function to ge
-0000fce0: 6e65 7261 7465 2053 6c61 6249 6e70 7574  nerate SlabInput
-0000fcf0: 2e69 6e20 696e 7075 7420 6669 6c65 2063  .in input file c
-0000fd00: 6f6e 7461 696e 696e 6720 7468 6520 6465  ontaining the de
-0000fd10: 7461 696c 7320 6f66 2074 6865 2073 6c61  tails of the sla
-0000fd20: 6220 6d6f 6465 6c20 6772 6964 0a20 2020  b model grid.   
-0000fd30: 2022 2222 0a20 2020 206e 6d6f 6465 6c73   """.    nmodels
-0000fd40: 3d31 0a20 2020 2063 6f6d 6269 6e61 7469  =1.    combinati
-0000fd50: 6f6e 3d46 616c 7365 0a20 2020 2069 6620  on=False.    if 
-0000fd60: 6c65 6e28 6772 6964 5f70 6172 616d 6574  len(grid_paramet
-0000fd70: 6572 7329 3e30 3a0a 2020 2020 2020 2020  ers)>0:.        
-0000fd80: 6966 206e 6f74 2063 6f6d 6269 6e61 7469  if not combinati
-0000fd90: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
-0000fda0: 6e6d 6f64 656c 733d 6c65 6e28 6772 6964  nmodels=len(grid
-0000fdb0: 5f70 6172 616d 6574 6572 735b 6c69 7374  _parameters[list
-0000fdc0: 2867 7269 645f 7061 7261 6d65 7465 7273  (grid_parameters
-0000fdd0: 2e6b 6579 7328 2929 5b30 5d5d 290a 2020  .keys())[0]]).  
-0000fde0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000fdf0: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-0000fe00: 2072 616e 6765 286c 656e 2867 7269 645f   range(len(grid_
-0000fe10: 7061 7261 6d65 7465 7273 2929 3a0a 2020  parameters)):.  
-0000fe20: 2020 2020 2020 2020 2020 2020 2020 6e6d                nm
-0000fe30: 6f64 656c 732a 3d6c 656e 2867 7269 645f  odels*=len(grid_
-0000fe40: 7061 7261 6d65 7465 7273 5b6c 6973 7428  parameters[list(
-0000fe50: 6772 6964 5f70 6172 616d 6574 6572 732e  grid_parameters.
-0000fe60: 6b65 7973 2829 295b 695d 5d29 0a0a 2020  keys())[i]])..  
-0000fe70: 2020 4e74 6f74 5f6c 6973 743d 6e70 2e6f    Ntot_list=np.o
-0000fe80: 6e65 7328 286e 6d6f 6465 6c73 2929 0a20  nes((nmodels)). 
-0000fe90: 2020 2054 675f 6c69 7374 3d6e 702e 6f6e     Tg_list=np.on
-0000fea0: 6573 2828 6e6d 6f64 656c 7329 290a 2020  es((nmodels)).  
-0000feb0: 2020 6e48 706c 7573 5f6c 6973 743d 6e70    nHplus_list=np
-0000fec0: 2e6f 6e65 7328 286e 6d6f 6465 6c73 2929  .ones((nmodels))
-0000fed0: 0a20 2020 206e 4831 5f6c 6973 743d 6e70  .    nH1_list=np
-0000fee0: 2e6f 6e65 7328 286e 6d6f 6465 6c73 2929  .ones((nmodels))
-0000fef0: 0a20 2020 206e 4832 5f6c 6973 743d 6e70  .    nH2_list=np
-0000ff00: 2e6f 6e65 7328 286e 6d6f 6465 6c73 2929  .ones((nmodels))
-0000ff10: 0a20 2020 206e 4865 5f6c 6973 743d 6e70  .    nHe_list=np
-0000ff20: 2e6f 6e65 7328 286e 6d6f 6465 6c73 2929  .ones((nmodels))
-0000ff30: 0a20 2020 206e 656c 6563 5f6c 6973 743d  .    nelec_list=
-0000ff40: 6e70 2e6f 6e65 7328 286e 6d6f 6465 6c73  np.ones((nmodels
-0000ff50: 2929 0a20 2020 2054 645f 6c69 7374 3d6e  )).    Td_list=n
-0000ff60: 702e 6f6e 6573 2828 6e6d 6f64 656c 7329  p.ones((nmodels)
-0000ff70: 290a 2020 2020 7674 7572 625f 6c69 7374  ).    vturb_list
-0000ff80: 3d6e 702e 6f6e 6573 2828 6e6d 6f64 656c  =np.ones((nmodel
-0000ff90: 7329 290a 2020 2020 6475 7374 5f74 6f5f  s)).    dust_to_
-0000ffa0: 6761 735f 6c69 7374 3d6e 702e 6f6e 6573  gas_list=np.ones
-0000ffb0: 2828 6e6d 6f64 656c 7329 290a 2020 2020  ((nmodels)).    
-0000ffc0: 525f 6f76 6572 6c61 705f 6c69 7374 3d6e  R_overlap_list=n
-0000ffd0: 702e 6f6e 6573 2828 6e6d 6f64 656c 7329  p.ones((nmodels)
-0000ffe0: 290a 2020 2020 6c69 6e65 5f6f 7665 726c  ).    line_overl
-0000fff0: 6170 5f6c 6973 743d 6e70 2e6f 6e65 7328  ap_list=np.ones(
-00010000: 286e 6d6f 6465 6c73 2c32 2929 0a20 2020  (nmodels,2)).   
-00010010: 2069 6620 6c65 6e28 7370 6563 6965 735f   if len(species_
-00010020: 6c69 7374 293c 313a 2072 6169 7365 2056  list)<1: raise V
-00010030: 616c 7565 4572 726f 7228 2754 6865 2073  alueError('The s
-00010040: 7065 6369 6573 5f6c 6973 7420 6361 6e6e  pecies_list cann
-00010050: 6f74 2062 6520 656d 7074 7927 290a 0a20  ot be empty').. 
-00010060: 2020 2069 6620 6e6f 7420 636f 6d62 696e     if not combin
-00010070: 6174 696f 6e3a 0a20 2020 2020 2020 2066  ation:.        f
-00010080: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
-00010090: 6e28 6772 6964 5f70 6172 616d 6574 6572  n(grid_parameter
-000100a0: 7329 293a 0a20 2020 2020 2020 2020 2020  s)):.           
-000100b0: 2069 6620 6c69 7374 2867 7269 645f 7061   if list(grid_pa
-000100c0: 7261 6d65 7465 7273 2e6b 6579 7328 2929  rameters.keys())
-000100d0: 5b69 5d3d 3d27 4e74 6f74 273a 0a20 2020  [i]=='Ntot':.   
-000100e0: 2020 2020 2020 2020 2020 2020 204e 746f               Nto
-000100f0: 745f 6c69 7374 2a3d 6772 6964 5f70 6172  t_list*=grid_par
-00010100: 616d 6574 6572 735b 274e 746f 7427 5d0a  ameters['Ntot'].
-00010110: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00010120: 206c 6973 7428 6772 6964 5f70 6172 616d   list(grid_param
-00010130: 6574 6572 732e 6b65 7973 2829 295b 695d  eters.keys())[i]
-00010140: 3d3d 2754 6727 3a0a 2020 2020 2020 2020  =='Tg':.        
-00010150: 2020 2020 2020 2020 5467 5f6c 6973 742a          Tg_list*
-00010160: 3d67 7269 645f 7061 7261 6d65 7465 7273  =grid_parameters
-00010170: 5b27 5467 275d 0a20 2020 2020 2020 2020  ['Tg'].         
-00010180: 2020 2065 6c69 6620 6c69 7374 2867 7269     elif list(gri
-00010190: 645f 7061 7261 6d65 7465 7273 2e6b 6579  d_parameters.key
-000101a0: 7328 2929 5b69 5d3d 3d27 6e48 706c 7573  s())[i]=='nHplus
-000101b0: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
-000101c0: 2020 206e 4870 6c75 735f 6c69 7374 2a3d     nHplus_list*=
-000101d0: 6772 6964 5f70 6172 616d 6574 6572 735b  grid_parameters[
-000101e0: 276e 4870 6c75 7327 5d0a 2020 2020 2020  'nHplus'].      
-000101f0: 2020 2020 2020 656c 6966 206c 6973 7428        elif list(
-00010200: 6772 6964 5f70 6172 616d 6574 6572 732e  grid_parameters.
-00010210: 6b65 7973 2829 295b 695d 3d3d 276e 4831  keys())[i]=='nH1
-00010220: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
-00010230: 2020 206e 4831 5f6c 6973 742a 3d67 7269     nH1_list*=gri
-00010240: 645f 7061 7261 6d65 7465 7273 5b27 6e48  d_parameters['nH
-00010250: 3127 5d0a 2020 2020 2020 2020 2020 2020  1'].            
-00010260: 656c 6966 206c 6973 7428 6772 6964 5f70  elif list(grid_p
-00010270: 6172 616d 6574 6572 732e 6b65 7973 2829  arameters.keys()
-00010280: 295b 695d 3d3d 276e 4832 273a 0a20 2020  )[i]=='nH2':.   
-00010290: 2020 2020 2020 2020 2020 2020 206e 4832               nH2
-000102a0: 5f6c 6973 742a 3d67 7269 645f 7061 7261  _list*=grid_para
-000102b0: 6d65 7465 7273 5b27 6e48 3227 5d0a 2020  meters['nH2'].  
-000102c0: 2020 2020 2020 2020 2020 656c 6966 206c            elif l
-000102d0: 6973 7428 6772 6964 5f70 6172 616d 6574  ist(grid_paramet
-000102e0: 6572 732e 6b65 7973 2829 295b 695d 3d3d  ers.keys())[i]==
-000102f0: 276e 4865 273a 0a20 2020 2020 2020 2020  'nHe':.         
-00010300: 2020 2020 2020 206e 4865 5f6c 6973 742a         nHe_list*
-00010310: 3d67 7269 645f 7061 7261 6d65 7465 7273  =grid_parameters
-00010320: 5b27 6e48 6527 5d0a 2020 2020 2020 2020  ['nHe'].        
-00010330: 2020 2020 656c 6966 206c 6973 7428 6772      elif list(gr
-00010340: 6964 5f70 6172 616d 6574 6572 732e 6b65  id_parameters.ke
-00010350: 7973 2829 295b 695d 3d3d 276e 656c 6563  ys())[i]=='nelec
-00010360: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
-00010370: 2020 206e 656c 6563 5f6c 6973 742a 3d67     nelec_list*=g
-00010380: 7269 645f 7061 7261 6d65 7465 7273 5b27  rid_parameters['
-00010390: 6e65 6c65 6327 5d0a 2020 2020 2020 2020  nelec'].        
-000103a0: 2020 2020 656c 6966 206c 6973 7428 6772      elif list(gr
-000103b0: 6964 5f70 6172 616d 6574 6572 732e 6b65  id_parameters.ke
-000103c0: 7973 2829 295b 695d 3d3d 2754 6427 3a0a  ys())[i]=='Td':.
-000103d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103e0: 5464 5f6c 6973 742a 3d67 7269 645f 7061  Td_list*=grid_pa
-000103f0: 7261 6d65 7465 7273 5b27 5464 275d 0a20  rameters['Td']. 
-00010400: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00010410: 6c69 7374 2867 7269 645f 7061 7261 6d65  list(grid_parame
-00010420: 7465 7273 2e6b 6579 7328 2929 5b69 5d3d  ters.keys())[i]=
-00010430: 3d27 7674 7572 6227 3a0a 2020 2020 2020  ='vturb':.      
-00010440: 2020 2020 2020 2020 2020 7674 7572 625f            vturb_
-00010450: 6c69 7374 2a3d 6772 6964 5f70 6172 616d  list*=grid_param
-00010460: 6574 6572 735b 2776 7475 7262 275d 0a20  eters['vturb']. 
-00010470: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00010480: 6c69 7374 2867 7269 645f 7061 7261 6d65  list(grid_parame
-00010490: 7465 7273 2e6b 6579 7328 2929 5b69 5d3d  ters.keys())[i]=
-000104a0: 3d27 6475 7374 5f74 6f5f 6761 7327 3a0a  ='dust_to_gas':.
-000104b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104c0: 6475 7374 5f74 6f5f 6761 735f 6c69 7374  dust_to_gas_list
-000104d0: 2a3d 6772 6964 5f70 6172 616d 6574 6572  *=grid_parameter
-000104e0: 735b 2764 7573 745f 746f 5f67 6173 275d  s['dust_to_gas']
-000104f0: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-00010500: 6620 6c69 7374 2867 7269 645f 7061 7261  f list(grid_para
-00010510: 6d65 7465 7273 2e6b 6579 7328 2929 5b69  meters.keys())[i
-00010520: 5d3d 3d27 525f 6f76 6572 6c61 7027 3a0a  ]=='R_overlap':.
-00010530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010540: 525f 6f76 6572 6c61 705f 6c69 7374 2a3d  R_overlap_list*=
-00010550: 6772 6964 5f70 6172 616d 6574 6572 735b  grid_parameters[
-00010560: 2752 5f6f 7665 726c 6170 275d 0a20 2020  'R_overlap'].   
-00010570: 2020 2020 2020 2020 2065 6c69 6620 6c69           elif li
-00010580: 7374 2867 7269 645f 7061 7261 6d65 7465  st(grid_paramete
-00010590: 7273 2e6b 6579 7328 2929 5b69 5d3d 3d27  rs.keys())[i]=='
-000105a0: 6c69 6e65 5f6f 7665 726c 6170 273a 0a20  line_overlap':. 
-000105b0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000105c0: 6f72 206a 2069 6e20 7261 6e67 6528 6c65  or j in range(le
-000105d0: 6e28 6772 6964 5f70 6172 616d 6574 6572  n(grid_parameter
-000105e0: 735b 276c 696e 655f 6f76 6572 6c61 7027  s['line_overlap'
-000105f0: 5d29 293a 0a20 2020 2020 2020 2020 2020  ])):.           
-00010600: 2020 2020 2020 2020 206c 696e 655f 6f76           line_ov
-00010610: 6572 6c61 705f 6c69 7374 5b6a 2c3a 5d3d  erlap_list[j,:]=
-00010620: 6e70 2e61 7272 6179 2867 7269 645f 7061  np.array(grid_pa
-00010630: 7261 6d65 7465 7273 5b27 6c69 6e65 5f6f  rameters['line_o
-00010640: 7665 726c 6170 275d 5b6a 5d29 0a20 2020  verlap'][j]).   
-00010650: 2020 2020 2020 2020 2065 6c73 653a 2072           else: r
-00010660: 6169 7365 204b 6579 4572 726f 7228 6627  aise KeyError(f'
-00010670: 556e 6964 656e 7469 6669 6564 2067 7269  Unidentified gri
-00010680: 6420 7061 7261 6d65 7465 7220 7b6c 6973  d parameter {lis
-00010690: 7428 6772 6964 5f70 6172 616d 6574 6572  t(grid_parameter
-000106a0: 732e 6b65 7973 2829 295b 695d 7d27 290a  s.keys())[i]}').
-000106b0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000106c0: 2020 7261 6973 6520 4b65 7945 7272 6f72    raise KeyError
-000106d0: 2827 436f 6d62 696e 6174 696f 6e20 6973  ('Combination is
-000106e0: 2073 7469 6c6c 206e 6f74 2073 7570 706f   still not suppo
-000106f0: 7274 6564 2729 0a0a 2020 2020 6966 206e  rted')..    if n
-00010700: 702e 7375 6d28 4e74 6f74 5f6c 6973 7429  p.sum(Ntot_list)
-00010710: 3d3d 6e6d 6f64 656c 733a 0a20 2020 2020  ==nmodels:.     
-00010720: 2020 2069 6620 6e6f 7420 284e 746f 7420     if not (Ntot 
-00010730: 2020 2020 2020 2069 7320 4e6f 6e65 293a         is None):
-00010740: 0a20 2020 2020 2020 2020 2020 204e 746f  .            Nto
-00010750: 745f 6c69 7374 2a3d 4e74 6f74 0a20 2020  t_list*=Ntot.   
-00010760: 2020 2020 2023 2065 6c73 653a 0a20 2020       # else:.   
-00010770: 2020 2020 2023 2020 2020 204e 746f 745f       #     Ntot_
-00010780: 6c69 7374 2a3d 3165 3135 0a20 2020 2069  list*=1e15.    i
-00010790: 6620 6e70 2e73 756d 2854 675f 6c69 7374  f np.sum(Tg_list
-000107a0: 293d 3d6e 6d6f 6465 6c73 3a0a 2020 2020  )==nmodels:.    
-000107b0: 2020 2020 6966 206e 6f74 2028 5467 2020      if not (Tg  
-000107c0: 2020 2020 2020 2020 6973 204e 6f6e 6529          is None)
-000107d0: 3a0a 2020 2020 2020 2020 2020 2020 5467  :.            Tg
-000107e0: 5f6c 6973 742a 3d54 670a 2020 2020 2020  _list*=Tg.      
-000107f0: 2020 2320 656c 7365 3a0a 2020 2020 2020    # else:.      
-00010800: 2020 2320 2020 2020 5467 5f6c 6973 742a    #     Tg_list*
-00010810: 3d31 3030 0a20 2020 2069 6620 6e70 2e73  =100.    if np.s
-00010820: 756d 286e 4870 6c75 735f 6c69 7374 293d  um(nHplus_list)=
-00010830: 3d6e 6d6f 6465 6c73 3a0a 2020 2020 2020  =nmodels:.      
-00010840: 2020 6966 206e 6f74 2028 6e48 706c 7573    if not (nHplus
-00010850: 2020 2020 2020 6973 204e 6f6e 6529 3a0a        is None):.
-00010860: 2020 2020 2020 2020 2020 2020 6e48 706c              nHpl
-00010870: 7573 5f6c 6973 742a 3d6e 4870 6c75 730a  us_list*=nHplus.
-00010880: 2020 2020 2020 2020 2320 656c 7365 3a0a          # else:.
-00010890: 2020 2020 2020 2020 2320 2020 2020 6e48          #     nH
-000108a0: 706c 7573 5f6c 6973 742a 3d31 6531 0a20  plus_list*=1e1. 
-000108b0: 2020 2069 6620 6e70 2e73 756d 286e 4831     if np.sum(nH1
-000108c0: 5f6c 6973 7429 3d3d 6e6d 6f64 656c 733a  _list)==nmodels:
-000108d0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-000108e0: 286e 4831 2020 2020 2020 2020 2069 7320  (nH1         is 
-000108f0: 4e6f 6e65 293a 0a20 2020 2020 2020 2020  None):.         
-00010900: 2020 206e 4831 5f6c 6973 742a 3d6e 4831     nH1_list*=nH1
-00010910: 0a20 2020 2020 2020 2023 2065 6c73 653a  .        # else:
-00010920: 0a20 2020 2020 2020 2023 2020 2020 206e  .        #     n
-00010930: 4831 5f6c 6973 742a 3d31 6531 320a 2020  H1_list*=1e12.  
-00010940: 2020 6966 206e 702e 7375 6d28 6e48 325f    if np.sum(nH2_
-00010950: 6c69 7374 293d 3d6e 6d6f 6465 6c73 3a0a  list)==nmodels:.
-00010960: 2020 2020 2020 2020 6966 206e 6f74 2028          if not (
-00010970: 6e48 3220 2020 2020 2020 2020 6973 204e  nH2         is N
-00010980: 6f6e 6529 3a0a 2020 2020 2020 2020 2020  one):.          
-00010990: 2020 6e48 325f 6c69 7374 2a3d 6e48 320a    nH2_list*=nH2.
-000109a0: 2020 2020 2020 2020 2320 656c 7365 3a0a          # else:.
-000109b0: 2020 2020 2020 2020 2320 2020 2020 6e48          #     nH
-000109c0: 325f 6c69 7374 2a3d 3165 3132 0a20 2020  2_list*=1e12.   
-000109d0: 2069 6620 6e70 2e73 756d 286e 4865 5f6c   if np.sum(nHe_l
-000109e0: 6973 7429 3d3d 6e6d 6f64 656c 733a 0a20  ist)==nmodels:. 
-000109f0: 2020 2020 2020 2069 6620 6e6f 7420 286e         if not (n
-00010a00: 4865 2020 2020 2020 2020 2069 7320 4e6f  He         is No
-00010a10: 6e65 293a 0a20 2020 2020 2020 2020 2020  ne):.           
-00010a20: 206e 4865 5f6c 6973 742a 3d6e 4865 0a20   nHe_list*=nHe. 
-00010a30: 2020 2020 2020 2023 2065 6c73 653a 0a20         # else:. 
-00010a40: 2020 2020 2020 2023 2020 2020 206e 4865         #     nHe
-00010a50: 5f6c 6973 742a 3d31 6531 310a 2020 2020  _list*=1e11.    
-00010a60: 6966 206e 702e 7375 6d28 6e65 6c65 635f  if np.sum(nelec_
-00010a70: 6c69 7374 293d 3d6e 6d6f 6465 6c73 3a0a  list)==nmodels:.
-00010a80: 2020 2020 2020 2020 6966 206e 6f74 2028          if not (
-00010a90: 6e65 6c65 6320 2020 2020 2020 6973 204e  nelec       is N
-00010aa0: 6f6e 6529 3a0a 2020 2020 2020 2020 2020  one):.          
-00010ab0: 2020 6e65 6c65 635f 6c69 7374 2a3d 6e65    nelec_list*=ne
-00010ac0: 6c65 630a 2020 2020 2020 2020 2320 656c  lec.        # el
-00010ad0: 7365 3a0a 2020 2020 2020 2020 2320 2020  se:.        #   
-00010ae0: 2020 6e65 6c65 635f 6c69 7374 2a3d 3165    nelec_list*=1e
-00010af0: 380a 2020 2020 6966 206e 702e 7375 6d28  8.    if np.sum(
-00010b00: 5464 5f6c 6973 7429 3d3d 6e6d 6f64 656c  Td_list)==nmodel
-00010b10: 733a 0a20 2020 2020 2020 2069 6620 6e6f  s:.        if no
-00010b20: 7420 2854 6420 2020 2020 2020 2020 2069  t (Td          i
-00010b30: 7320 4e6f 6e65 293a 0a20 2020 2020 2020  s None):.       
-00010b40: 2020 2020 2054 645f 6c69 7374 2a3d 5464       Td_list*=Td
-00010b50: 0a20 2020 2020 2020 2023 2065 6c73 653a  .        # else:
-00010b60: 0a20 2020 2020 2020 2023 2020 2020 2054  .        #     T
-00010b70: 645f 6c69 7374 2a3d 3130 0a20 2020 2069  d_list*=10.    i
-00010b80: 6620 6e70 2e73 756d 2876 7475 7262 5f6c  f np.sum(vturb_l
-00010b90: 6973 7429 3d3d 6e6d 6f64 656c 733a 0a20  ist)==nmodels:. 
-00010ba0: 2020 2020 2020 2069 6620 6e6f 7420 2876         if not (v
-00010bb0: 7475 7262 2020 2020 2020 2069 7320 4e6f  turb       is No
-00010bc0: 6e65 293a 0a20 2020 2020 2020 2020 2020  ne):.           
-00010bd0: 2076 7475 7262 5f6c 6973 742a 3d76 7475   vturb_list*=vtu
-00010be0: 7262 0a20 2020 2020 2020 2023 2065 6c73  rb.        # els
-00010bf0: 653a 0a20 2020 2020 2020 2023 2020 2020  e:.        #    
-00010c00: 2076 7475 7262 5f6c 6973 742a 3d31 2e34   vturb_list*=1.4
-00010c10: 0a20 2020 2069 6620 6e70 2e73 756d 2864  .    if np.sum(d
-00010c20: 7573 745f 746f 5f67 6173 5f6c 6973 7429  ust_to_gas_list)
-00010c30: 3d3d 6e6d 6f64 656c 733a 0a20 2020 2020  ==nmodels:.     
-00010c40: 2020 2069 6620 6e6f 7420 2864 7573 745f     if not (dust_
-00010c50: 746f 5f67 6173 2069 7320 4e6f 6e65 293a  to_gas is None):
-00010c60: 0a20 2020 2020 2020 2020 2020 2064 7573  .            dus
-00010c70: 745f 746f 5f67 6173 5f6c 6973 742a 3d64  t_to_gas_list*=d
-00010c80: 7573 745f 746f 5f67 6173 0a20 2020 2020  ust_to_gas.     
-00010c90: 2020 2023 2065 6c73 653a 0a20 2020 2020     # else:.     
-00010ca0: 2020 2023 2020 2020 2064 7573 745f 746f     #     dust_to
-00010cb0: 5f67 6173 5f6c 6973 742a 3d31 652d 3231  _gas_list*=1e-21
-00010cc0: 0a20 2020 2069 6620 6e70 2e73 756d 2852  .    if np.sum(R
-00010cd0: 5f6f 7665 726c 6170 5f6c 6973 7429 3d3d  _overlap_list)==
-00010ce0: 6e6d 6f64 656c 733a 0a20 2020 2020 2020  nmodels:.       
-00010cf0: 2069 6620 6e6f 7420 2852 5f6f 7665 726c   if not (R_overl
-00010d00: 6170 2069 7320 4e6f 6e65 293a 0a20 2020  ap is None):.   
-00010d10: 2020 2020 2020 2020 2052 5f6f 7665 726c           R_overl
-00010d20: 6170 5f6c 6973 742a 3d52 5f6f 7665 726c  ap_list*=R_overl
-00010d30: 6170 0a20 2020 2020 2020 2023 2065 6c73  ap.        # els
-00010d40: 653a 0a20 2020 2020 2020 2023 2020 2020  e:.        #    
-00010d50: 2052 5f6f 7665 726c 6170 5f6c 6973 742a   R_overlap_list*
-00010d60: 3d31 6535 0a20 2020 2069 6620 6e70 2e73  =1e5.    if np.s
-00010d70: 756d 286c 696e 655f 6f76 6572 6c61 705f  um(line_overlap_
-00010d80: 6c69 7374 293d 3d32 2a6e 6d6f 6465 6c73  list)==2*nmodels
-00010d90: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
-00010da0: 2028 6c69 6e65 5f6f 7665 726c 6170 2069   (line_overlap i
-00010db0: 7320 4e6f 6e65 293a 0a20 2020 2020 2020  s None):.       
-00010dc0: 2020 2020 206c 696e 655f 6f76 6572 6c61       line_overla
-00010dd0: 705f 6c69 7374 2a3d 6e70 2e61 7272 6179  p_list*=np.array
-00010de0: 286c 696e 655f 6f76 6572 6c61 7029 0a20  (line_overlap). 
-00010df0: 2020 2020 2020 2023 2065 6c73 653a 0a20         # else:. 
-00010e00: 2020 2020 2020 2023 2020 2020 206c 696e         #     lin
-00010e10: 655f 6f76 6572 6c61 705f 6c69 7374 2a3d  e_overlap_list*=
-00010e20: 6e70 2e61 7272 6179 2828 342c 3330 2929  np.array((4,30))
-00010e30: 0a0a 2020 2020 6f73 2e73 7973 7465 6d28  ..    os.system(
-00010e40: 6627 746f 7563 6820 7b64 6972 6563 746f  f'touch {directo
-00010e50: 7279 2b22 2f53 6c61 6249 6e70 7574 2e69  ry+"/SlabInput.i
-00010e60: 6e22 7d27 290a 2020 2020 663d 6f70 656e  n"}').    f=open
-00010e70: 2864 6972 6563 746f 7279 2b27 2f53 6c61  (directory+'/Sla
-00010e80: 6249 6e70 7574 2e69 6e27 2c27 7727 290a  bInput.in','w').
-00010e90: 2020 2020 662e 7772 6974 6528 222a 2a2a      f.write("***
-00010ea0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00010eb0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00010ec0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00010ed0: 2a2a 2a2a 2a2a 2a2a 5c6e 2229 0a20 2020  ********\n").   
-00010ee0: 2066 2e77 7269 7465 2822 2a2a 2a20 496e   f.write("*** In
-00010ef0: 7075 7420 6669 6c65 2066 6f72 2073 6c61  put file for sla
-00010f00: 6220 6573 6361 7065 2070 726f 6261 6269  b escape probabi
-00010f10: 6c69 7479 2077 6974 6820 5072 6f44 694d  lity with ProDiM
-00010f20: 6f20 2a2a 2a5c 6e22 290a 2020 2020 662e  o ***\n").    f.
-00010f30: 7772 6974 6528 222a 2a2a 2a2a 2a2a 2a2a  write("*********
-00010f40: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00010f50: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00010f60: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00010f70: 2a2a 5c6e 2229 0a20 2020 2066 2e77 7269  **\n").    f.wri
-00010f80: 7465 2822 2a2a 2a20 6e6d 6f64 656c 7320  te("*** nmodels 
-00010f90: 7368 6f75 6c64 2066 6f6c 6c6f 7720 6f75  should follow ou
-00010fa0: 7470 7574 5f66 696c 656e 616d 6520 2a2a  tput_filename **
-00010fb0: 2a5c 6e22 290a 2020 2020 662e 7772 6974  *\n").    f.writ
-00010fc0: 6528 6627 7b6f 7574 7075 745f 6669 6c65  e(f'{output_file
-00010fd0: 6e61 6d65 7d20 2120 6f75 7470 7574 5f66  name} ! output_f
-00010fe0: 696c 656e 616d 655c 6e27 290a 2020 2020  ilename\n').    
-00010ff0: 662e 7772 6974 6528 6627 7b6f 7665 726c  f.write(f'{overl
-00011000: 6170 5f66 696c 656e 616d 657d 2021 206f  ap_filename} ! o
-00011010: 7665 726c 6170 5f66 696c 656e 616d 655c  verlap_filename\
-00011020: 6e27 290a 2020 2020 6966 2073 6570 6172  n').    if separ
-00011030: 6174 655f 6f70 5f66 696c 6573 3a0a 2020  ate_op_files:.  
-00011040: 2020 2020 2020 662e 7772 6974 6528 272e        f.write('.
-00011050: 7472 7565 2e20 2020 2021 2073 6570 6172  true.    ! separ
-00011060: 6174 655f 6f70 5f66 696c 6573 5c6e 2729  ate_op_files\n')
-00011070: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-00011080: 2020 2066 2e77 7269 7465 2827 2e66 616c     f.write('.fal
-00011090: 7365 2e20 2020 2120 7365 7061 7261 7465  se.   ! separate
-000110a0: 5f6f 705f 6669 6c65 735c 6e27 290a 2020  _op_files\n').  
-000110b0: 2020 6966 2066 6974 735f 6f70 5f66 696c    if fits_op_fil
-000110c0: 6573 3a0a 2020 2020 2020 2020 662e 7772  es:.        f.wr
-000110d0: 6974 6528 272e 7472 7565 2e20 2020 2021  ite('.true.    !
-000110e0: 2066 6974 735f 6f70 5f66 696c 6573 5c6e   fits_op_files\n
-000110f0: 2729 0a20 2020 2065 6c73 653a 0a20 2020  ').    else:.   
-00011100: 2020 2020 2066 2e77 7269 7465 2827 2e66       f.write('.f
-00011110: 616c 7365 2e20 2020 2120 6669 7473 5f6f  alse.   ! fits_o
-00011120: 705f 6669 6c65 735c 6e27 290a 2020 2020  p_files\n').    
-00011130: 6966 206e 6f5f 696e 6469 7669 6475 616c  if no_individual
-00011140: 5f6c 696e 6573 3a0a 2020 2020 2020 2020  _lines:.        
-00011150: 662e 7772 6974 6528 272e 7472 7565 2e20  f.write('.true. 
-00011160: 2020 2021 206e 6f5f 696e 6469 7669 6475     ! no_individu
-00011170: 616c 5f6c 696e 6573 5c6e 2729 0a20 2020  al_lines\n').   
-00011180: 2065 6c73 653a 0a20 2020 2020 2020 2066   else:.        f
-00011190: 2e77 7269 7465 2827 2e66 616c 7365 2e20  .write('.false. 
-000111a0: 2020 2120 6e6f 5f69 6e64 6976 6964 7561    ! no_individua
-000111b0: 6c5f 6c69 6e65 735c 6e27 290a 2020 2020  l_lines\n').    
-000111c0: 6966 2073 6c61 625f 5254 3a0a 2020 2020  if slab_RT:.    
-000111d0: 2020 2020 662e 7772 6974 6528 272e 7472      f.write('.tr
-000111e0: 7565 2e20 2020 2021 2073 6c61 625f 5254  ue.    ! slab_RT
-000111f0: 205c 6e27 290a 2020 2020 656c 7365 3a0a   \n').    else:.
-00011200: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
-00011210: 272e 6661 6c73 652e 2020 2021 2073 6c61  '.false.   ! sla
-00011220: 625f 5254 205c 6e27 290a 2020 2020 6966  b_RT \n').    if
-00011230: 2073 686f 7274 5f66 6f72 6d61 743a 0a20   short_format:. 
-00011240: 2020 2020 2020 2066 2e77 7269 7465 2827         f.write('
-00011250: 2e74 7275 652e 2020 2020 2120 7368 6f72  .true.    ! shor
-00011260: 745f 666f 726d 6174 5c6e 2729 0a20 2020  t_format\n').   
-00011270: 2065 6c73 653a 0a20 2020 2020 2020 2066   else:.        f
-00011280: 2e77 7269 7465 2827 2e66 616c 7365 2e20  .write('.false. 
-00011290: 2020 2120 7368 6f72 745f 666f 726d 6174    ! short_format
-000112a0: 5c6e 2729 0a20 2020 2066 2e77 7269 7465  \n').    f.write
-000112b0: 2866 277b 6e6d 6f64 656c 737d 2020 2020  (f'{nmodels}    
-000112c0: 2020 2020 2020 2020 2021 206e 6d6f 6465           ! nmode
-000112d0: 6c73 5c6e 2729 0a20 2020 2066 2e77 7269  ls\n').    f.wri
-000112e0: 7465 2827 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  te('------------
-000112f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00011300: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00011310: 2d2d 2d2d 2d2d 2d2d 2d2d 2d27 290a 2020  -----------').  
-00011320: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-00011330: 286e 6d6f 6465 6c73 293a 0a20 2020 2020  (nmodels):.     
-00011340: 2020 2066 2e77 7269 7465 2866 275c 6e2a     f.write(f'\n*
-00011350: 2a2a 206d 6f64 656c 207b 692b 317d 202a  ** model {i+1} *
-00011360: 2a2a 5c6e 2729 0a20 2020 2020 2020 2069  **\n').        i
-00011370: 6620 6e70 2e73 756d 284e 746f 745f 6c69  f np.sum(Ntot_li
-00011380: 7374 2921 3d6e 6d6f 6465 6c73 3a0a 2020  st)!=nmodels:.  
-00011390: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
-000113a0: 6528 666d 742e 666f 726d 6174 2827 7b3a  e(fmt.format('{:
-000113b0: 2e33 6d7d 272c 4e74 6f74 5f6c 6973 745b  .3m}',Ntot_list[
-000113c0: 695d 2929 0a20 2020 2020 2020 2020 2020  i])).           
-000113d0: 2066 2e77 7269 7465 2827 0920 2020 2120   f.write('.   ! 
-000113e0: 4e48 746f 7420 205b 636d 5e2d 325d 2074  NHtot  [cm^-2] t
-000113f0: 6f74 616c 2067 6173 2063 6f6c 756d 6e20  otal gas column 
-00011400: 6465 6e73 6974 795c 6e27 290a 2020 2020  density\n').    
-00011410: 2020 2020 6966 206e 702e 7375 6d28 6e48      if np.sum(nH
-00011420: 706c 7573 5f6c 6973 7429 213d 6e6d 6f64  plus_list)!=nmod
-00011430: 656c 733a 0a20 2020 2020 2020 2020 2020  els:.           
-00011440: 2066 2e77 7269 7465 2866 6d74 2e66 6f72   f.write(fmt.for
-00011450: 6d61 7428 277b 3a2e 336d 7d27 2c6e 4870  mat('{:.3m}',nHp
-00011460: 6c75 735f 6c69 7374 5b69 5d29 290a 2020  lus_list[i])).  
-00011470: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
-00011480: 6528 2709 2020 2021 206e 482b 2020 2020  e('.   ! nH+    
-00011490: 5b63 6d5e 2d33 5d20 2070 726f 746f 6e20  [cm^-3]  proton 
-000114a0: 6e75 6d62 6572 2064 656e 7369 7479 5c6e  number density\n
-000114b0: 2729 0a20 2020 2020 2020 2069 6620 6e70  ').        if np
-000114c0: 2e73 756d 286e 4831 5f6c 6973 7429 213d  .sum(nH1_list)!=
-000114d0: 6e6d 6f64 656c 733a 0a20 2020 2020 2020  nmodels:.       
-000114e0: 2020 2020 2066 2e77 7269 7465 2866 6d74       f.write(fmt
-000114f0: 2e66 6f72 6d61 7428 277b 3a2e 336d 7d27  .format('{:.3m}'
-00011500: 2c6e 4831 5f6c 6973 745b 695d 2929 0a20  ,nH1_list[i])). 
-00011510: 2020 2020 2020 2020 2020 2066 2e77 7269             f.wri
-00011520: 7465 2827 0920 2020 2120 6e48 4909 205b  te('.   ! nHI. [
-00011530: 636d 5e2d 335d 2061 746f 6d69 6320 6879  cm^-3] atomic hy
-00011540: 6472 6f67 656e 5c6e 2729 0a20 2020 2020  drogen\n').     
-00011550: 2020 2069 6620 6e70 2e73 756d 286e 4832     if np.sum(nH2
-00011560: 5f6c 6973 7429 213d 6e6d 6f64 656c 733a  _list)!=nmodels:
-00011570: 0a20 2020 2020 2020 2020 2020 2066 2e77  .            f.w
-00011580: 7269 7465 2866 6d74 2e66 6f72 6d61 7428  rite(fmt.format(
-00011590: 277b 3a2e 336d 7d27 2c6e 4832 5f6c 6973  '{:.3m}',nH2_lis
-000115a0: 745b 695d 2929 0a20 2020 2020 2020 2020  t[i])).         
-000115b0: 2020 2066 2e77 7269 7465 2827 0920 2020     f.write('.   
-000115c0: 2120 6e48 3220 2020 205b 636d 5e2d 335d  ! nH2    [cm^-3]
-000115d0: 2020 206d 6f6c 6563 756c 6172 2068 7964     molecular hyd
-000115e0: 726f 6765 6e5c 6e27 290a 2020 2020 2020  rogen\n').      
-000115f0: 2020 6966 206e 702e 7375 6d28 6e48 655f    if np.sum(nHe_
-00011600: 6c69 7374 2921 3d6e 6d6f 6465 6c73 3a0a  list)!=nmodels:.
-00011610: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
-00011620: 6974 6528 666d 742e 666f 726d 6174 2827  ite(fmt.format('
-00011630: 7b3a 2e33 6d7d 272c 6e48 655f 6c69 7374  {:.3m}',nHe_list
-00011640: 5b69 5d29 290a 2020 2020 2020 2020 2020  [i])).          
-00011650: 2020 662e 7772 6974 6528 2709 2020 2021    f.write('.   !
-00011660: 206e 4865 2020 2020 5b63 6d5e 2d33 5d20   nHe    [cm^-3] 
-00011670: 2020 4865 6c69 756d 5c6e 2729 0a20 2020    Helium\n').   
-00011680: 2020 2020 2069 6620 6e70 2e73 756d 286e       if np.sum(n
-00011690: 656c 6563 5f6c 6973 7429 213d 6e6d 6f64  elec_list)!=nmod
-000116a0: 656c 733a 0a20 2020 2020 2020 2020 2020  els:.           
-000116b0: 2066 2e77 7269 7465 2866 6d74 2e66 6f72   f.write(fmt.for
-000116c0: 6d61 7428 277b 3a2e 336d 7d27 2c6e 656c  mat('{:.3m}',nel
-000116d0: 6563 5f6c 6973 745b 695d 2929 0a20 2020  ec_list[i])).   
-000116e0: 2020 2020 2020 2020 2066 2e77 7269 7465           f.write
-000116f0: 2827 0920 2020 2120 6e65 6c65 6320 205b  ('.   ! nelec  [
-00011700: 636d 5e2d 335d 2020 2065 6c65 6374 726f  cm^-3]   electro
-00011710: 6e20 6e75 6d62 6572 2064 656e 7369 7479  n number density
-00011720: 5c6e 2729 0a20 2020 2020 2020 2069 6620  \n').        if 
-00011730: 6e70 2e73 756d 2854 675f 6c69 7374 2921  np.sum(Tg_list)!
-00011740: 3d6e 6d6f 6465 6c73 3a0a 2020 2020 2020  =nmodels:.      
-00011750: 2020 2020 2020 662e 7772 6974 6528 666d        f.write(fm
-00011760: 742e 666f 726d 6174 2827 7b3a 2e33 6d7d  t.format('{:.3m}
-00011770: 272c 5467 5f6c 6973 745b 695d 2929 0a20  ',Tg_list[i])). 
-00011780: 2020 2020 2020 2020 2020 2066 2e77 7269             f.wri
-00011790: 7465 2827 0920 2020 2120 5467 6173 205b  te('.   ! Tgas [
-000117a0: 4b5d 2020 2020 2020 2020 2020 2067 6173  K]           gas
-000117b0: 2074 656d 7065 7261 7475 7265 5c6e 2729   temperature\n')
-000117c0: 0a20 2020 2020 2020 2069 6620 6e70 2e73  .        if np.s
-000117d0: 756d 2854 645f 6c69 7374 2921 3d6e 6d6f  um(Td_list)!=nmo
-000117e0: 6465 6c73 3a0a 2020 2020 2020 2020 2020  dels:.          
-000117f0: 2020 662e 7772 6974 6528 666d 742e 666f    f.write(fmt.fo
-00011800: 726d 6174 2827 7b3a 2e33 6d7d 272c 5464  rmat('{:.3m}',Td
-00011810: 5f6c 6973 745b 695d 2929 0a20 2020 2020  _list[i])).     
-00011820: 2020 2020 2020 2066 2e77 7269 7465 2827         f.write('
-00011830: 0920 2020 2120 5464 7573 7420 5b4b 5d20  .   ! Tdust [K] 
-00011840: 2020 2020 2020 2020 2020 6475 7374 2074            dust t
-00011850: 656d 7065 7261 7475 7265 5c6e 2729 0a20  emperature\n'). 
-00011860: 2020 2020 2020 2069 6620 6e70 2e73 756d         if np.sum
-00011870: 2876 7475 7262 5f6c 6973 7429 213d 6e6d  (vturb_list)!=nm
-00011880: 6f64 656c 733a 0a20 2020 2020 2020 2020  odels:.         
-00011890: 2020 2066 2e77 7269 7465 2866 6d74 2e66     f.write(fmt.f
-000118a0: 6f72 6d61 7428 277b 3a2e 336d 7d27 2c76  ormat('{:.3m}',v
-000118b0: 7475 7262 5f6c 6973 745b 695d 2929 0a20  turb_list[i])). 
-000118c0: 2020 2020 2020 2020 2020 2066 2e77 7269             f.wri
-000118d0: 7465 2827 0920 2020 2120 7674 7572 6220  te('.   ! vturb 
-000118e0: 205b 6b6d 732f 735d 2020 2020 7475 7262   [kms/s]    turb
-000118f0: 756c 656e 7420 7665 6c6f 6369 7479 5c6e  ulent velocity\n
-00011900: 2729 0a20 2020 2020 2020 2069 6620 6e70  ').        if np
-00011910: 2e73 756d 2864 7573 745f 746f 5f67 6173  .sum(dust_to_gas
-00011920: 5f6c 6973 7429 213d 6e6d 6f64 656c 733a  _list)!=nmodels:
-00011930: 0a20 2020 2020 2020 2020 2020 2066 2e77  .            f.w
-00011940: 7269 7465 2866 6d74 2e66 6f72 6d61 7428  rite(fmt.format(
-00011950: 277b 3a2e 336d 7d27 2c64 7573 745f 746f  '{:.3m}',dust_to
-00011960: 5f67 6173 5f6c 6973 745b 695d 2929 0a20  _gas_list[i])). 
-00011970: 2020 2020 2020 2020 2020 2066 2e77 7269             f.wri
-00011980: 7465 2827 0920 2020 2120 6475 7374 5f74  te('.   ! dust_t
-00011990: 6f5f 6761 735c 6e27 290a 2020 2020 2020  o_gas\n').      
-000119a0: 2020 6966 206e 702e 7375 6d28 6c69 6e65    if np.sum(line
-000119b0: 5f6f 7665 726c 6170 5f6c 6973 7429 213d  _overlap_list)!=
-000119c0: 322a 6e6d 6f64 656c 733a 0a20 2020 2020  2*nmodels:.     
-000119d0: 2020 2020 2020 2066 2e77 7269 7465 2866         f.write(f
-000119e0: 6d74 2e66 6f72 6d61 7428 277b 3a2e 3366  mt.format('{:.3f
-000119f0: 7d27 2c6c 696e 655f 6f76 6572 6c61 705f  }',line_overlap_
-00011a00: 6c69 7374 5b69 2c30 5d29 2b27 2027 2b66  list[i,0])+' '+f
-00011a10: 6d74 2e66 6f72 6d61 7428 277b 3a2e 3366  mt.format('{:.3f
-00011a20: 7d27 2c6c 696e 655f 6f76 6572 6c61 705f  }',line_overlap_
-00011a30: 6c69 7374 5b69 2c31 5d29 290a 2020 2020  list[i,1])).    
-00011a40: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
-00011a50: 2709 2020 2021 206c 696e 655f 6f76 6572  '.   ! line_over
-00011a60: 6c61 7020 205b 6d69 6372 6f6e 735d 2020  lap  [microns]  
-00011a70: 6d69 6e69 6d75 6d20 616e 6420 6d61 7869  minimum and maxi
-00011a80: 6d75 6d20 7761 7665 6c65 6e67 7468 7320  mum wavelengths 
-00011a90: 666f 7220 6c69 6e65 206f 7665 726c 6170  for line overlap
-00011aa0: 5c6e 2729 0a20 2020 2020 2020 2069 6620  \n').        if 
-00011ab0: 6e70 2e73 756d 2852 5f6f 7665 726c 6170  np.sum(R_overlap
-00011ac0: 5f6c 6973 7429 213d 6e6d 6f64 656c 733a  _list)!=nmodels:
-00011ad0: 0a20 2020 2020 2020 2020 2020 2066 2e77  .            f.w
-00011ae0: 7269 7465 2866 6d74 2e66 6f72 6d61 7428  rite(fmt.format(
-00011af0: 277b 3a2e 336d 7d27 2c52 5f6f 7665 726c  '{:.3m}',R_overl
-00011b00: 6170 5f6c 6973 745b 695d 2929 0a20 2020  ap_list[i])).   
-00011b10: 2020 2020 2020 2020 2066 2e77 7269 7465           f.write
-00011b20: 2827 0920 2020 2120 525f 6f76 6572 6c61  ('.   ! R_overla
-00011b30: 7020 2073 616d 706c 696e 6720 6772 6964  p  sampling grid
-00011b40: 2072 6573 6f6c 7574 696f 6e20 666f 7220   resolution for 
-00011b50: 6c69 6e65 206f 7665 726c 6170 5c6e 2729  line overlap\n')
-00011b60: 0a20 2020 2020 2020 2066 2e77 7269 7465  .        f.write
-00011b70: 2866 277b 6c65 6e28 7370 6563 6965 735f  (f'{len(species_
-00011b80: 6c69 7374 297d 0920 2020 2120 4e73 7065  list)}.   ! Nspe
-00011b90: 6369 6573 2020 2020 2020 2020 2020 2020  cies            
-00011ba0: 6e75 6d62 6572 206f 6620 7370 6563 6965  number of specie
-00011bb0: 7320 666f 7220 7468 6174 206d 6f64 656c  s for that model
-00011bc0: 5c6e 2729 0a20 2020 2020 2020 2066 6f72  \n').        for
-00011bd0: 206a 2069 6e20 7261 6e67 6528 6c65 6e28   j in range(len(
-00011be0: 7370 6563 6965 735f 6c69 7374 2929 3a0a  species_list)):.
-00011bf0: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
-00011c00: 6974 6528 6627 7b6c 6973 7428 7370 6563  ite(f'{list(spec
-00011c10: 6965 735f 6c69 7374 2e6b 6579 7328 2929  ies_list.keys())
-00011c20: 5b6a 5d7d 2020 2020 2020 7b73 7065 6369  [j]}      {speci
-00011c30: 6573 5f6c 6973 745b 6c69 7374 2873 7065  es_list[list(spe
-00011c40: 6369 6573 5f6c 6973 742e 6b65 7973 2829  cies_list.keys()
-00011c50: 295b 6a5d 5d7d 5c6e 2729 0a20 2020 2020  )[j]]}\n').     
-00011c60: 2020 2066 2e77 7269 7465 2827 2020 2020     f.write('    
-00011c70: 2020 2020 2020 2021 2065 6e64 5c6e 2729         ! end\n')
-00011c80: 0a20 2020 2020 2020 2066 2e77 7269 7465  .        f.write
-00011c90: 2827 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ('--------------
+0000e390: 2074 656d 706f 2e63 6f6e 7652 3d4e 6f6e   tempo.convR=Non
+0000e3a0: 650a 0a20 2020 2020 2020 2020 2020 2020  e..             
+0000e3b0: 2020 2064 6174 3d5b 5d0a 2020 2020 2020     dat=[].      
+0000e3c0: 2020 2020 2020 2020 2020 2320 666f 7220            # for 
+0000e3d0: 6b20 696e 2072 616e 6765 2874 656d 706f  k in range(tempo
+0000e3e0: 2e6e 6c65 7665 6c73 293a 0a20 2020 2020  .nlevels):.     
+0000e3f0: 2020 2020 2020 2020 2020 2023 2020 2020             #    
+0000e400: 2064 6174 5b30 5d5b 6b2c 3a5d 3d6e 702e   dat[0][k,:]=np.
+0000e410: 6173 6172 7261 7928 5b66 6c6f 6174 2878  asarray([float(x
+0000e420: 2920 666f 7220 7820 696e 2066 2e72 6561  ) for x in f.rea
+0000e430: 646c 696e 6528 292e 7370 6c69 7428 295d  dline().split()]
+0000e440: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000e450: 2020 2023 206c 696e 6573 3d66 2e72 6561     # lines=f.rea
+0000e460: 646c 696e 6528 290a 2020 2020 2020 2020  dline().        
+0000e470: 2020 2020 2020 2020 2320 6c69 6e65 733d          # lines=
+0000e480: 662e 7265 6164 6c69 6e65 2829 0a20 2020  f.readline().   
+0000e490: 2020 2020 2020 2020 2020 2020 2064 6174               dat
+0000e4a0: 3d6e 702e 7a65 726f 7328 2874 656d 706f  =np.zeros((tempo
+0000e4b0: 2e6e 6c69 6e65 732c 3429 290a 2020 2020  .nlines,4)).    
+0000e4c0: 2020 2020 2020 2020 2020 2020 736c 6162              slab
+0000e4d0: 4f75 7446 6f72 6d61 743d 5b38 2c31 342c  OutFormat=[8,14,
+0000e4e0: 3135 2c31 355d 0a20 2020 2020 2020 2020  15,15].         
+0000e4f0: 2020 2020 2020 2066 6f72 206b 2069 6e20         for k in 
+0000e500: 7261 6e67 6528 7465 6d70 6f2e 6e6c 696e  range(tempo.nlin
+0000e510: 6573 293a 0a20 2020 2020 2020 2020 2020  es):.           
+0000e520: 2020 2020 2020 2020 206c 696e 6552 6561           lineRea
+0000e530: 643d 5b5d 0a20 2020 2020 2020 2020 2020  d=[].           
+0000e540: 2020 2020 2020 2020 206c 696e 6573 3d66           lines=f
+0000e550: 2e72 6561 646c 696e 6528 290a 2020 2020  .readline().    
+0000e560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e570: 6c3d 300a 2020 2020 2020 2020 2020 2020  l=0.            
+0000e580: 2020 2020 2020 2020 666f 7220 6c65 6e67          for leng
+0000e590: 7468 2069 6e20 736c 6162 4f75 7446 6f72  th in slabOutFor
+0000e5a0: 6d61 743a 0a20 2020 2020 2020 2020 2020  mat:.           
+0000e5b0: 2020 2020 2020 2020 2020 2020 206c 696e               lin
+0000e5c0: 6552 6561 642e 6170 7065 6e64 286c 696e  eRead.append(lin
+0000e5d0: 6573 5b6c 3a6c 2b6c 656e 6774 685d 290a  es[l:l+length]).
+0000e5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5f0: 2020 2020 2020 2020 6c2b 3d6c 656e 6774          l+=lengt
+0000e600: 680a 2020 2020 2020 2020 2020 2020 2020  h.              
+0000e610: 2020 2020 2020 6461 745b 6b2c 3a5d 3d6e        dat[k,:]=n
+0000e620: 702e 6173 6172 7261 7928 5b66 6c6f 6174  p.asarray([float
+0000e630: 2878 2920 666f 7220 7820 696e 206c 696e  (x) for x in lin
+0000e640: 6552 6561 645d 290a 2020 2020 2020 2020  eRead]).        
+0000e650: 2020 2020 2020 2020 6c69 6e65 4461 7461          lineData
+0000e660: 3d70 642e 4461 7461 4672 616d 6528 6461  =pd.DataFrame(da
+0000e670: 742c 636f 6c75 6d6e 733d 5b27 6927 2c27  t,columns=['i','
+0000e680: 4748 7a27 2c27 464e 4c54 4527 2c27 464c  GHz','FNLTE','FL
+0000e690: 5445 275d 290a 2020 2020 2020 2020 2020  TE']).          
+0000e6a0: 2020 2020 2020 7465 6d70 6f2e 6c69 6e65        tempo.line
+0000e6b0: 6461 7461 3d6c 696e 6544 6174 610a 2020  data=lineData.  
+0000e6c0: 2020 2020 2020 2020 2020 2020 2020 6461                da
+0000e6d0: 7461 2e61 6464 5f6d 6f64 656c 2874 656d  ta.add_model(tem
+0000e6e0: 706f 290a 2020 2020 2020 2020 656c 7365  po).        else
+0000e6f0: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+0000e700: 7220 6a20 696e 2072 616e 6765 286e 7370  r j in range(nsp
+0000e710: 6563 6965 7329 3a0a 2020 2020 2020 2020  ecies):.        
+0000e720: 2020 2020 2020 2020 7465 6d70 6f3d 736c          tempo=sl
+0000e730: 6162 2829 0a20 2020 2020 2020 2020 2020  ab().           
+0000e740: 2020 2020 2074 656d 706f 2e6d 6f64 656c       tempo.model
+0000e750: 5f6e 756d 6265 723d 7465 6d70 6f5f 6d6f  _number=tempo_mo
+0000e760: 6465 6c5f 6e75 6d62 6572 0a20 2020 2020  del_number.     
+0000e770: 2020 2020 2020 2020 2020 2074 656d 706f             tempo
+0000e780: 2e4e 483d 7465 6d70 6f5f 6e48 746f 740a  .NH=tempo_nHtot.
+0000e790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e7a0: 7465 6d70 6f2e 6e43 6f6c 6c3d 7465 6d70  tempo.nColl=temp
+0000e7b0: 6f5f 6761 7344 656e 730a 2020 2020 2020  o_gasDens.      
+0000e7c0: 2020 2020 2020 2020 2020 7465 6d70 6f2e            tempo.
+0000e7d0: 6e65 3d74 656d 706f 5f6e 656c 6563 0a20  ne=tempo_nelec. 
+0000e7e0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000e7f0: 656d 706f 2e6e 4865 3d74 656d 706f 5f6e  empo.nHe=tempo_n
+0000e800: 4865 0a20 2020 2020 2020 2020 2020 2020  He.             
+0000e810: 2020 2074 656d 706f 2e6e 4849 493d 7465     tempo.nHII=te
+0000e820: 6d70 6f5f 6e48 4949 0a20 2020 2020 2020  mpo_nHII.       
+0000e830: 2020 2020 2020 2020 2074 656d 706f 2e6e           tempo.n
+0000e840: 4849 3d74 656d 706f 5f6e 4849 0a20 2020  HI=tempo_nHI.   
+0000e850: 2020 2020 2020 2020 2020 2020 2074 656d               tem
+0000e860: 706f 2e6e 4832 3d74 656d 706f 5f6e 4832  po.nH2=tempo_nH2
+0000e870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e880: 2074 656d 706f 2e64 7573 745f 746f 5f67   tempo.dust_to_g
+0000e890: 6173 3d74 656d 706f 5f64 7573 745f 746f  as=tempo_dust_to
+0000e8a0: 5f67 6173 0a20 2020 2020 2020 2020 2020  _gas.           
+0000e8b0: 2020 2020 2074 656d 706f 2e76 7475 7262       tempo.vturb
+0000e8c0: 3d74 656d 706f 5f76 7475 7262 0a20 2020  =tempo_vturb.   
+0000e8d0: 2020 2020 2020 2020 2020 2020 2074 656d               tem
+0000e8e0: 706f 2e54 673d 7465 6d70 6f5f 5467 0a20  po.Tg=tempo_Tg. 
+0000e8f0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000e900: 656d 706f 2e54 643d 7465 6d70 6f5f 5464  empo.Td=tempo_Td
+0000e910: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e920: 2020 7465 6d70 6f2e 7370 6563 6965 735f    tempo.species_
+0000e930: 696e 6465 783d 696e 7428 662e 7265 6164  index=int(f.read
+0000e940: 6c69 6e65 2829 2e73 706c 6974 2829 5b30  line().split()[0
+0000e950: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+0000e960: 2020 2074 656d 706f 2e73 7065 6369 6573     tempo.species
+0000e970: 5f6e 756d 6265 723d 6a2b 310a 2020 2020  _number=j+1.    
+0000e980: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+0000e990: 6f2e 7370 6563 6965 735f 6e61 6d65 3d66  o.species_name=f
+0000e9a0: 2e72 6561 646c 696e 6528 292e 7370 6c69  .readline().spli
+0000e9b0: 7428 295b 305d 0a20 2020 2020 2020 2020  t()[0].         
+0000e9c0: 2020 2020 2020 2074 656d 706f 2e61 6275         tempo.abu
+0000e9d0: 6e64 616e 6365 3d66 6c6f 6174 2866 2e72  ndance=float(f.r
+0000e9e0: 6561 646c 696e 6528 292e 7370 6c69 7428  eadline().split(
+0000e9f0: 295b 305d 290a 2020 2020 2020 2020 2020  )[0]).          
+0000ea00: 2020 2020 2020 7465 6d70 6f2e 6476 3d66        tempo.dv=f
+0000ea10: 6c6f 6174 2866 2e72 6561 646c 696e 6528  loat(f.readline(
+0000ea20: 292e 7370 6c69 7428 295b 305d 290a 2020  ).split()[0]).  
+0000ea30: 2020 2020 2020 2020 2020 2020 2020 7465                te
+0000ea40: 6d70 6f2e 6e6c 6576 656c 733d 696e 7428  mpo.nlevels=int(
+0000ea50: 662e 7265 6164 6c69 6e65 2829 2e73 706c  f.readline().spl
+0000ea60: 6974 2829 5b30 5d29 0a20 2020 2020 2020  it()[0]).       
+0000ea70: 2020 2020 2020 2020 206c 696e 6573 3d66           lines=f
+0000ea80: 2e72 6561 646c 696e 6528 290a 0a20 2020  .readline()..   
+0000ea90: 2020 2020 2020 2020 2020 2020 2074 656d               tem
+0000eaa0: 706f 2e6e 6c69 6e65 733d 4e6f 6e65 0a20  po.nlines=None. 
+0000eab0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000eac0: 656d 706f 2e6c 696e 6564 6174 613d 4e6f  empo.linedata=No
+0000ead0: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
+0000eae0: 2020 2074 656d 706f 2e6c 6576 656c 6461     tempo.levelda
+0000eaf0: 7461 3d4e 6f6e 650a 2020 2020 2020 2020  ta=None.        
+0000eb00: 2020 2020 2020 2020 7465 6d70 6f2e 636f          tempo.co
+0000eb10: 6e76 5761 7665 6c65 6e67 7468 3d4e 6f6e  nvWavelength=Non
+0000eb20: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000eb30: 2020 7465 6d70 6f2e 636f 6e76 4c54 4566    tempo.convLTEf
+0000eb40: 6c75 783d 4e6f 6e65 0a20 2020 2020 2020  lux=None.       
+0000eb50: 2020 2020 2020 2020 2074 656d 706f 2e63           tempo.c
+0000eb60: 6f6e 764e 4c54 4566 6c75 783d 4e6f 6e65  onvNLTEflux=None
+0000eb70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000eb80: 2074 656d 706f 2e63 6f6e 7654 7970 653d   tempo.convType=
+0000eb90: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+0000eba0: 2020 2020 2074 656d 706f 2e63 6f6e 7652       tempo.convR
+0000ebb0: 3d4e 6f6e 650a 0a20 2020 2020 2020 2020  =None..         
+0000ebc0: 2020 2020 2020 2064 6174 3d5b 6e70 2e7a         dat=[np.z
+0000ebd0: 6572 6f73 2828 7465 6d70 6f2e 6e6c 6576  eros((tempo.nlev
+0000ebe0: 656c 732c 3829 292c 5b5d 2c5b 5d5d 0a20  els,8)),[],[]]. 
+0000ebf0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000ec00: 6f72 206b 2069 6e20 7261 6e67 6528 7465  or k in range(te
+0000ec10: 6d70 6f2e 6e6c 6576 656c 7329 3a0a 2020  mpo.nlevels):.  
+0000ec20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec30: 2020 6461 745b 305d 5b6b 2c3a 5d3d 6e70    dat[0][k,:]=np
+0000ec40: 2e61 7361 7272 6179 285b 666c 6f61 7428  .asarray([float(
+0000ec50: 7829 2066 6f72 2078 2069 6e20 662e 7265  x) for x in f.re
+0000ec60: 6164 6c69 6e65 2829 2e73 706c 6974 2829  adline().split()
+0000ec70: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+0000ec80: 2020 2074 656d 706f 2e6e 6c69 6e65 733d     tempo.nlines=
+0000ec90: 696e 7428 662e 7265 6164 6c69 6e65 2829  int(f.readline()
+0000eca0: 2e73 706c 6974 2829 5b30 5d29 0a20 2020  .split()[0]).   
+0000ecb0: 2020 2020 2020 2020 2020 2020 206c 696e               lin
+0000ecc0: 6573 3d66 2e72 6561 646c 696e 6528 290a  es=f.readline().
+0000ecd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ece0: 6c69 6e65 733d 662e 7265 6164 6c69 6e65  lines=f.readline
+0000ecf0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+0000ed00: 2020 2064 6174 5b31 5d3d 6e70 2e7a 6572     dat[1]=np.zer
+0000ed10: 6f73 2828 7465 6d70 6f2e 6e6c 696e 6573  os((tempo.nlines
+0000ed20: 2c32 3329 290a 2020 2020 2020 2020 2020  ,23)).          
+0000ed30: 2020 2020 2020 736c 6162 4f75 7446 6f72        slabOutFor
+0000ed40: 6d61 743d 5b39 2c39 2c39 2c35 2c35 2c35  mat=[9,9,9,5,5,5
+0000ed50: 2c31 352c 3135 2c31 352c 3135 2c31 352c  ,15,15,15,15,15,
+0000ed60: 3135 2c31 352c 3135 2c31 352c 3135 2c31  15,15,15,15,15,1
+0000ed70: 352c 3135 2c31 352c 3135 2c31 352c 3135  5,15,15,15,15,15
+0000ed80: 2c31 352c 3231 2c32 312c 3231 2c32 315d  ,15,21,21,21,21]
+0000ed90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000eda0: 2066 6f72 206b 2069 6e20 7261 6e67 6528   for k in range(
+0000edb0: 7465 6d70 6f2e 6e6c 696e 6573 293a 0a20  tempo.nlines):. 
+0000edc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000edd0: 2020 206c 696e 6552 6561 643d 5b5d 0a20     lineRead=[]. 
+0000ede0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000edf0: 2020 206c 696e 6573 3d66 2e72 6561 646c     lines=f.readl
+0000ee00: 696e 6528 290a 2020 2020 2020 2020 2020  ine().          
+0000ee10: 2020 2020 2020 2020 2020 6c3d 300a 2020            l=0.  
+0000ee20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee30: 2020 666f 7220 6c65 6e67 7468 2069 6e20    for length in 
+0000ee40: 736c 6162 4f75 7446 6f72 6d61 743a 0a20  slabOutFormat:. 
+0000ee50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee60: 2020 2020 2020 206c 696e 6552 6561 642e         lineRead.
+0000ee70: 6170 7065 6e64 286c 696e 6573 5b6c 3a6c  append(lines[l:l
+0000ee80: 2b6c 656e 6774 685d 290a 2020 2020 2020  +length]).      
+0000ee90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eea0: 2020 6c2b 3d6c 656e 6774 680a 2020 2020    l+=length.    
+0000eeb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eec0: 6461 745b 315d 5b6b 2c3a 5d3d 6e70 2e61  dat[1][k,:]=np.a
+0000eed0: 7361 7272 6179 285b 666c 6f61 7428 7829  sarray([float(x)
+0000eee0: 2066 6f72 2078 2069 6e20 6c69 6e65 5265   for x in lineRe
+0000eef0: 6164 5b30 3a2d 345d 5d29 0a20 2020 2020  ad[0:-4]]).     
+0000ef00: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0000ef10: 6174 5b32 5d2e 6170 7065 6e64 285b 612e  at[2].append([a.
+0000ef20: 7374 7269 7028 2920 666f 7220 6120 696e  strip() for a in
+0000ef30: 206c 696e 6552 6561 645b 2d34 3a5d 5d29   lineRead[-4:]])
+0000ef40: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000ef50: 2020 6c69 6e65 4461 7461 3d70 642e 4461    lineData=pd.Da
+0000ef60: 7461 4672 616d 6528 6461 745b 315d 2c63  taFrame(dat[1],c
+0000ef70: 6f6c 756d 6e73 3d5b 2769 272c 2775 272c  olumns=['i','u',
+0000ef80: 276c 272c 2765 272c 2776 272c 274a 272c  'l','e','v','J',
+0000ef90: 2767 7527 2c27 4575 272c 2741 272c 2742  'gu','Eu','A','B
+0000efa0: 272c 2747 487a 272c 2774 6175 4427 2c27  ','GHz','tauD','
+0000efb0: 4a62 6163 6b27 2c27 706f 7027 2c27 6c74  Jback','pop','lt
+0000efc0: 6570 6f70 272c 2774 6175 4e4c 5445 272c  epop','tauNLTE',
+0000efd0: 2774 6175 4c54 4527 2c27 624e 4c54 4527  'tauLTE','bNLTE'
+0000efe0: 2c27 624c 5445 272c 2770 4e4c 5445 272c  ,'bLTE','pNLTE',
+0000eff0: 2770 4c54 4527 2c27 464e 4c54 4527 2c27  'pLTE','FNLTE','
+0000f000: 464c 5445 275d 290a 2020 2020 2020 2020  FLTE']).        
+0000f010: 2020 2020 2020 2020 6c69 6e65 4461 7461          lineData
+0000f020: 5b27 676c 6f62 616c 5f75 275d 3d5b 615b  ['global_u']=[a[
+0000f030: 305d 2066 6f72 2061 2069 6e20 6461 745b  0] for a in dat[
+0000f040: 325d 5d0a 2020 2020 2020 2020 2020 2020  2]].            
+0000f050: 2020 2020 6c69 6e65 4461 7461 5b27 676c      lineData['gl
+0000f060: 6f62 616c 5f6c 275d 3d5b 615b 315d 2066  obal_l']=[a[1] f
+0000f070: 6f72 2061 2069 6e20 6461 745b 325d 5d0a  or a in dat[2]].
+0000f080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f090: 6c69 6e65 4461 7461 5b27 6c6f 6361 6c5f  lineData['local_
+0000f0a0: 7527 5d3d 5b61 5b32 5d20 666f 7220 6120  u']=[a[2] for a 
+0000f0b0: 696e 2064 6174 5b32 5d5d 0a20 2020 2020  in dat[2]].     
+0000f0c0: 2020 2020 2020 2020 2020 206c 696e 6544             lineD
+0000f0d0: 6174 615b 276c 6f63 616c 5f6c 275d 3d5b  ata['local_l']=[
+0000f0e0: 615b 335d 2066 6f72 2061 2069 6e20 6461  a[3] for a in da
+0000f0f0: 745b 325d 5d0a 2020 2020 2020 2020 2020  t[2]].          
+0000f100: 2020 2020 2020 6c65 7644 6174 613d 7064        levData=pd
+0000f110: 2e44 6174 6146 7261 6d65 2864 6174 5b30  .DataFrame(dat[0
+0000f120: 5d2c 636f 6c75 6d6e 733d 5b27 6927 2c27  ],columns=['i','
+0000f130: 6727 2c27 4527 2c27 706f 7027 2c27 6c74  g','E','pop','lt
+0000f140: 6570 6f70 272c 2765 272c 2776 272c 274a  epop','e','v','J
+0000f150: 275d 290a 2020 2020 2020 2020 2020 2020  ']).            
+0000f160: 2020 2020 7465 6d70 6f2e 6c69 6e65 6461      tempo.lineda
+0000f170: 7461 3d6c 696e 6544 6174 610a 2020 2020  ta=lineData.    
+0000f180: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+0000f190: 6f2e 6c65 7665 6c64 6174 613d 6c65 7644  o.leveldata=levD
+0000f1a0: 6174 610a 2020 2020 2020 2020 2020 2020  ata.            
+0000f1b0: 2020 2020 6461 7461 2e61 6464 5f6d 6f64      data.add_mod
+0000f1c0: 656c 2874 656d 706f 290a 2020 2020 7265  el(tempo).    re
+0000f1d0: 7475 726e 2864 6174 6129 0a0a 0a64 6566  turn(data)...def
+0000f1e0: 2072 6561 645f 6f76 6572 6c61 705f 7370   read_overlap_sp
+0000f1f0: 6563 7472 6128 7061 7468 3d27 536c 6162  ectra(path='Slab
+0000f200: 4f76 6572 6c61 702e 6f75 7427 2c76 6572  Overlap.out',ver
+0000f210: 626f 7365 3d54 7275 6529 3a0a 2020 2020  bose=True):.    
+0000f220: 2222 220a 2020 2020 4675 6e63 7469 6f6e  """.    Function
+0000f230: 2074 6f20 7265 6164 2030 4420 7072 6f64   to read 0D prod
+0000f240: 696d 6f20 736c 6162 206d 6f64 656c 206f  imo slab model o
+0000f250: 7574 7075 7420 7769 7468 206c 696e 6520  utput with line 
+0000f260: 6f76 6572 6c61 700a 2020 2020 2222 220a  overlap.    """.
+0000f270: 0a20 2020 2069 6620 6973 696e 7374 616e  .    if isinstan
+0000f280: 6365 2870 6174 682c 6c69 7374 293a 0a20  ce(path,list):. 
+0000f290: 2020 2020 2020 2064 6174 613d 736c 6162         data=slab
+0000f2a0: 5f64 6174 6128 290a 2020 2020 2020 2020  _data().        
+0000f2b0: 6461 7461 2e64 6972 6563 746f 7279 3d70  data.directory=p
+0000f2c0: 6174 680a 2020 2020 2020 2020 666f 7220  ath.        for 
+0000f2d0: 6920 696e 2070 6174 683a 0a20 2020 2020  i in path:.     
+0000f2e0: 2020 2020 2020 2072 6461 7461 3d72 6561         rdata=rea
+0000f2f0: 645f 6f76 6572 6c61 705f 7370 6563 7472  d_overlap_spectr
+0000f300: 6128 692c 7665 7262 6f73 653d 7665 7262  a(i,verbose=verb
+0000f310: 6f73 6529 0a20 2020 2020 2020 2020 2020  ose).           
+0000f320: 2066 6f72 206a 2069 6e20 7261 6e67 6528   for j in range(
+0000f330: 7264 6174 612e 6e6d 6f64 656c 7329 3a0a  rdata.nmodels):.
+0000f340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f350: 6461 7461 2e61 6464 5f6d 6f64 656c 2872  data.add_model(r
+0000f360: 6461 7461 2e6d 6f64 656c 735b 6a5d 290a  data.models[j]).
+0000f370: 2020 2020 2020 2020 7265 7475 726e 2864          return(d
+0000f380: 6174 6129 0a0a 2020 2020 6966 2076 6572  ata)..    if ver
+0000f390: 626f 7365 3a20 7072 696e 7428 2252 6561  bose: print("Rea
+0000f3a0: 6469 6e67 2073 6c61 6220 6c69 6e65 206f  ding slab line o
+0000f3b0: 7665 726c 6170 206d 6f64 656c 206f 7574  verlap model out
+0000f3c0: 7075 7420 6672 6f6d 3a20 222c 7061 7468  put from: ",path
+0000f3d0: 290a 2020 2020 6966 2027 2e66 6974 732e  ).    if '.fits.
+0000f3e0: 677a 2720 696e 2070 6174 683a 0a20 2020  gz' in path:.   
+0000f3f0: 2020 2020 2068 6475 6c3d 6669 7473 2e6f       hdul=fits.o
+0000f400: 7065 6e28 7061 7468 290a 2020 2020 2020  pen(path).      
+0000f410: 2020 6461 7461 3d73 6c61 625f 6461 7461    data=slab_data
+0000f420: 2829 0a20 2020 2020 2020 206e 6d6f 6465  ().        nmode
+0000f430: 6c73 3d68 6475 6c5b 305d 2e68 6561 6465  ls=hdul[0].heade
+0000f440: 725b 274e 4d4f 4445 4c53 275d 0a20 2020  r['NMODELS'].   
+0000f450: 2020 2020 2064 6174 612e 6469 7265 6374       data.direct
+0000f460: 6f72 793d 7061 7468 0a20 2020 2020 2020  ory=path.       
+0000f470: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+0000f480: 6e6d 6f64 656c 7329 3a0a 2020 2020 2020  nmodels):.      
+0000f490: 2020 2020 2020 7465 6d70 6f3d 736c 6162        tempo=slab
+0000f4a0: 2829 0a20 2020 2020 2020 2020 2020 2074  ().            t
+0000f4b0: 656d 706f 5f6d 6f64 656c 5f6e 756d 6265  empo_model_numbe
+0000f4c0: 723d 6864 756c 5b69 2b31 5d2e 6865 6164  r=hdul[i+1].head
+0000f4d0: 6572 5b27 4d4f 4445 4c27 5d0a 2020 2020  er['MODEL'].    
+0000f4e0: 2020 2020 2020 2020 7465 6d70 6f5f 4e6c          tempo_Nl
+0000f4f0: 696e 653d 6864 756c 5b69 2b31 5d2e 6865  ine=hdul[i+1].he
+0000f500: 6164 6572 5b27 4e4c 494e 4527 5d0a 2020  ader['NLINE'].  
+0000f510: 2020 2020 2020 2020 2020 7465 6d70 6f5f            tempo_
+0000f520: 523d 6864 756c 5b69 2b31 5d2e 6865 6164  R=hdul[i+1].head
+0000f530: 6572 5b27 525f 4f56 4c50 275d 0a20 2020  er['R_OVLP'].   
+0000f540: 2020 2020 2020 2020 2064 6174 7461 3d5b           datta=[
+0000f550: 5d0a 2020 2020 2020 2020 2020 2020 7465  ].            te
+0000f560: 6d70 6f2e 6f76 6572 6c61 7046 7265 713d  mpo.overlapFreq=
+0000f570: 6864 756c 5b69 2b31 5d2e 6461 7461 5b3a  hdul[i+1].data[:
+0000f580: 2c2d 315d 0a20 2020 2020 2020 2020 2020  ,-1].           
+0000f590: 2074 656d 706f 2e6f 7665 726c 6170 4c54   tempo.overlapLT
+0000f5a0: 453d 6864 756c 5b69 2b31 5d2e 6461 7461  E=hdul[i+1].data
+0000f5b0: 5b3a 2c30 5d0a 2020 2020 2020 2020 2020  [:,0].          
+0000f5c0: 2020 7465 6d70 6f2e 6f76 6572 6c61 7054    tempo.overlapT
+0000f5d0: 6175 4c54 453d 6864 756c 5b69 2b31 5d2e  auLTE=hdul[i+1].
+0000f5e0: 6461 7461 5b3a 2c31 5d0a 2020 2020 2020  data[:,1].      
+0000f5f0: 2020 2020 2020 7465 6d70 6f2e 6f76 6572        tempo.over
+0000f600: 6c61 704e 4c54 453d 6864 756c 5b69 2b31  lapNLTE=hdul[i+1
+0000f610: 5d2e 6461 7461 5b3a 2c32 5d0a 2020 2020  ].data[:,2].    
+0000f620: 2020 2020 2020 2020 7465 6d70 6f2e 6f76          tempo.ov
+0000f630: 6572 6c61 7054 6175 4e4c 5445 3d68 6475  erlapTauNLTE=hdu
+0000f640: 6c5b 692b 315d 2e64 6174 615b 3a2c 335d  l[i+1].data[:,3]
+0000f650: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
+0000f660: 706f 2e6f 7665 726c 6170 523d 7465 6d70  po.overlapR=temp
+0000f670: 6f5f 520a 2020 2020 2020 2020 2020 2020  o_R.            
+0000f680: 7465 6d70 6f2e 6d6f 6465 6c5f 6e75 6d62  tempo.model_numb
+0000f690: 6572 3d68 6475 6c5b 692b 315d 2e68 6561  er=hdul[i+1].hea
+0000f6a0: 6465 725b 274d 4f44 454c 275d 0a20 2020  der['MODEL'].   
+0000f6b0: 2020 2020 2020 2020 2074 656d 706f 2e54           tempo.T
+0000f6c0: 673d 6864 756c 5b69 2b31 5d2e 6865 6164  g=hdul[i+1].head
+0000f6d0: 6572 5b27 5447 275d 0a20 2020 2020 2020  er['TG'].       
+0000f6e0: 2020 2020 2074 656d 706f 2e54 643d 6864       tempo.Td=hd
+0000f6f0: 756c 5b69 2b31 5d2e 6865 6164 6572 5b27  ul[i+1].header['
+0000f700: 5444 275d 0a20 2020 2020 2020 2020 2020  TD'].           
+0000f710: 2074 656d 706f 2e76 7475 7262 3d68 6475   tempo.vturb=hdu
+0000f720: 6c5b 692b 315d 2e68 6561 6465 725b 2756  l[i+1].header['V
+0000f730: 5455 5242 275d 0a20 2020 2020 2020 2020  TURB'].         
+0000f740: 2020 2074 656d 706f 2e4e 483d 6864 756c     tempo.NH=hdul
+0000f750: 5b69 2b31 5d2e 6865 6164 6572 5b27 4e48  [i+1].header['NH
+0000f760: 544f 5427 5d0a 2020 2020 2020 2020 2020  TOT'].          
+0000f770: 2020 6461 7461 2e61 6464 5f6d 6f64 656c    data.add_model
+0000f780: 2874 656d 706f 290a 2020 2020 2020 2020  (tempo).        
+0000f790: 2020 2020 2320 7072 696e 7428 2772 6561      # print('rea
+0000f7a0: 6420 272c 692c 2720 6d6f 6465 6c27 290a  d ',i,' model').
+0000f7b0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000f7c0: 2020 663d 6f70 656e 2870 6174 6829 0a20    f=open(path). 
+0000f7d0: 2020 2020 2020 2064 6174 613d 736c 6162         data=slab
+0000f7e0: 5f64 6174 6128 290a 2020 2020 2020 2020  _data().        
+0000f7f0: 6e6d 6f64 656c 733d 696e 7428 662e 7265  nmodels=int(f.re
+0000f800: 6164 6c69 6e65 2829 2e73 706c 6974 2829  adline().split()
+0000f810: 5b30 5d29 0a20 2020 2020 2020 2064 6174  [0]).        dat
+0000f820: 612e 6469 7265 6374 6f72 793d 7061 7468  a.directory=path
+0000f830: 0a20 2020 2020 2020 2066 6f72 2069 2069  .        for i i
+0000f840: 6e20 7261 6e67 6528 6e6d 6f64 656c 7329  n range(nmodels)
+0000f850: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
+0000f860: 6d70 6f3d 736c 6162 2829 0a20 2020 2020  mpo=slab().     
+0000f870: 2020 2020 2020 2074 656d 706f 5f6d 6f64         tempo_mod
+0000f880: 656c 5f6e 756d 6265 723d 696e 7428 662e  el_number=int(f.
+0000f890: 7265 6164 6c69 6e65 2829 2e73 706c 6974  readline().split
+0000f8a0: 2829 5b30 5d29 0a20 2020 2020 2020 2020  ()[0]).         
+0000f8b0: 2020 2074 656d 706f 5f4e 6c69 6e65 3d69     tempo_Nline=i
+0000f8c0: 6e74 2866 2e72 6561 646c 696e 6528 292e  nt(f.readline().
+0000f8d0: 7370 6c69 7428 295b 305d 290a 2020 2020  split()[0]).    
+0000f8e0: 2020 2020 2020 2020 7465 6d70 6f5f 523d          tempo_R=
+0000f8f0: 666c 6f61 7428 662e 7265 6164 6c69 6e65  float(f.readline
+0000f900: 2829 2e73 706c 6974 2829 5b30 5d29 0a20  ().split()[0]). 
+0000f910: 2020 2020 2020 2020 2020 2064 6174 7461             datta
+0000f920: 3d5b 5d0a 2020 2020 2020 2020 2020 2020  =[].            
+0000f930: 6c69 6e65 733d 662e 7265 6164 6c69 6e65  lines=f.readline
+0000f940: 2829 0a20 2020 2020 2020 2020 2020 2066  ().            f
+0000f950: 6f72 206a 2069 6e20 7261 6e67 6528 7465  or j in range(te
+0000f960: 6d70 6f5f 4e6c 696e 6529 3a0a 2020 2020  mpo_Nline):.    
+0000f970: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
+0000f980: 733d 662e 7265 6164 6c69 6e65 2829 0a20  s=f.readline(). 
+0000f990: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0000f9a0: 6174 7461 2e61 7070 656e 6428 6e70 2e61  atta.append(np.a
+0000f9b0: 7272 6179 286c 696e 6573 2e73 706c 6974  rray(lines.split
+0000f9c0: 2829 2c64 7479 7065 3d66 6c6f 6174 2929  (),dtype=float))
+0000f9d0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+0000f9e0: 7461 3d6e 702e 6172 7261 7928 6461 7474  ta=np.array(datt
+0000f9f0: 6129 0a20 2020 2020 2020 2020 2020 2074  a).            t
+0000fa00: 656d 706f 2e6f 7665 726c 6170 4672 6571  empo.overlapFreq
+0000fa10: 3d64 6174 7461 5b3a 2c30 5d0a 2020 2020  =datta[:,0].    
+0000fa20: 2020 2020 2020 2020 7465 6d70 6f2e 6f76          tempo.ov
+0000fa30: 6572 6c61 704c 5445 3d64 6174 7461 5b3a  erlapLTE=datta[:
+0000fa40: 2c31 5d0a 2020 2020 2020 2020 2020 2020  ,1].            
+0000fa50: 7465 6d70 6f2e 6f76 6572 6c61 7054 6175  tempo.overlapTau
+0000fa60: 4c54 453d 6461 7474 615b 3a2c 325d 0a20  LTE=datta[:,2]. 
+0000fa70: 2020 2020 2020 2020 2020 2074 656d 706f             tempo
+0000fa80: 2e6f 7665 726c 6170 4e4c 5445 3d64 6174  .overlapNLTE=dat
+0000fa90: 7461 5b3a 2c33 5d0a 2020 2020 2020 2020  ta[:,3].        
+0000faa0: 2020 2020 7465 6d70 6f2e 6f76 6572 6c61      tempo.overla
+0000fab0: 7054 6175 4e4c 5445 3d64 6174 7461 5b3a  pTauNLTE=datta[:
+0000fac0: 2c34 5d0a 2020 2020 2020 2020 2020 2020  ,4].            
+0000fad0: 7465 6d70 6f2e 6f76 6572 6c61 7052 3d74  tempo.overlapR=t
+0000fae0: 656d 706f 5f52 0a20 2020 2020 2020 2020  empo_R.         
+0000faf0: 2020 2064 6174 612e 6164 645f 6d6f 6465     data.add_mode
+0000fb00: 6c28 7465 6d70 6f29 0a20 2020 2020 2020  l(tempo).       
+0000fb10: 2020 2020 206c 696e 6573 3d66 2e72 6561       lines=f.rea
+0000fb20: 646c 696e 6528 290a 2020 2020 2020 2020  dline().        
+0000fb30: 2020 2020 2320 7072 696e 7428 2772 6561      # print('rea
+0000fb40: 6420 272c 692c 2720 6d6f 6465 6c27 290a  d ',i,' model').
+0000fb50: 2020 2020 0a20 2020 2072 6574 7572 6e28      .    return(
+0000fb60: 6461 7461 290a 0a0a 6465 6620 7370 6563  data)...def spec
+0000fb70: 436f 6e76 6f6c 7665 286c 696e 6553 7472  Convolve(lineStr
+0000fb80: 656e 6774 6873 2c6c 696e 6546 7265 712c  engths,lineFreq,
+0000fb90: 6672 6571 5f62 696e 733d 4e6f 6e65 2c52  freq_bins=None,R
+0000fba0: 3d31 2c6c 616d 6264 615f 303d 312c 6c61  =1,lambda_0=1,la
+0000fbb0: 6d62 6461 5f6e 3d31 2c76 723d 3133 3030  mbda_n=1,vr=1300
+0000fbc0: 293a 0a20 2020 2022 2222 0a20 2020 204e  ):.    """.    N
+0000fbd0: 4f54 2055 5345 4420 414e 594d 4f52 450a  OT USED ANYMORE.
+0000fbe0: 2020 2020 4675 6e63 7469 6f6e 2074 6f20      Function to 
+0000fbf0: 636f 6e76 6f6c 7665 206c 696e 6573 2069  convolve lines i
+0000fc00: 6e74 6f20 7370 6563 7472 6120 6279 2073  nto spectra by s
+0000fc10: 696d 706c 7920 6269 6e6e 696e 6720 7468  imply binning th
+0000fc20: 656d 2069 6e74 6f20 6120 7761 7665 6c65  em into a wavele
+0000fc30: 6e67 7468 2067 7269 640a 2020 2020 2222  ngth grid.    ""
+0000fc40: 220a 2020 2020 6750 6572 633d 6c61 6d62  ".    gPerc=lamb
+0000fc50: 6461 2078 2c6d 2c73 3a20 7365 7266 2828  da x,m,s: serf((
+0000fc60: 782d 6d29 2f73 292a 302e 352b 302e 350a  x-m)/s)*0.5+0.5.
+0000fc70: 2020 2020 6e75 5f69 6a3d 6c69 6e65 4672      nu_ij=lineFr
+0000fc80: 6571 2a31 6539 0a20 2020 2069 6620 6c61  eq*1e9.    if la
+0000fc90: 6d62 6461 5f6e 3d3d 6c61 6d62 6461 5f30  mbda_n==lambda_0
+0000fca0: 3a0a 2020 2020 2020 2020 6c61 6d62 6461  :.        lambda
+0000fcb0: 5f6e 3d6e 702e 616d 6178 2863 2f6e 755f  _n=np.amax(c/nu_
+0000fcc0: 696a 2a31 6536 292a 320a 2020 2020 6966  ij*1e6)*2.    if
+0000fcd0: 2074 7970 6528 6672 6571 5f62 696e 7329   type(freq_bins)
+0000fce0: 3d3d 7479 7065 284e 6f6e 6529 3a0a 2020  ==type(None):.  
+0000fcf0: 2020 2020 2020 6e75 3d67 656e 6572 6174        nu=generat
+0000fd00: 655f 6772 6964 2852 3d52 2c6c 616d 6264  e_grid(R=R,lambd
+0000fd10: 615f 303d 6c61 6d62 6461 5f30 2c6c 616d  a_0=lambda_0,lam
+0000fd20: 6264 615f 6e3d 6c61 6d62 6461 5f6e 292a  bda_n=lambda_n)*
+0000fd30: 3165 390a 2020 2020 656c 7365 3a0a 2020  1e9.    else:.  
+0000fd40: 2020 2020 2020 6672 6571 5f62 696e 733d        freq_bins=
+0000fd50: 6e70 2e63 6f6e 6361 7465 6e61 7465 2828  np.concatenate((
+0000fd60: 6672 6571 5f62 696e 732c 6e70 2e61 7272  freq_bins,np.arr
+0000fd70: 6179 285b 2866 7265 715f 6269 6e73 5b2d  ay([(freq_bins[-
+0000fd80: 315d 2d66 7265 715f 6269 6e73 5b2d 325d  1]-freq_bins[-2]
+0000fd90: 292b 6672 6571 5f62 696e 735b 2d31 5d5d  )+freq_bins[-1]]
+0000fda0: 2929 290a 2020 2020 2020 2020 6e75 3d66  ))).        nu=f
+0000fdb0: 7265 715f 6269 6e73 2a31 6539 0a20 2020  req_bins*1e9.   
+0000fdc0: 206e 755f 696a 5f74 696c 653d 6e70 2e74   nu_ij_tile=np.t
+0000fdd0: 696c 6528 6e75 5f69 6a2c 5b6c 656e 286e  ile(nu_ij,[len(n
+0000fde0: 7529 2c31 5d29 0a20 2020 206e 755f 7469  u),1]).    nu_ti
+0000fdf0: 6c65 3d6e 702e 7469 6c65 286e 752c 5b6c  le=np.tile(nu,[l
+0000fe00: 656e 286e 755f 696a 292c 315d 290a 2020  en(nu_ij),1]).  
+0000fe10: 2020 6c69 6e65 5374 7265 6e67 7468 735f    lineStrengths_
+0000fe20: 7469 6c65 3d6e 702e 7469 6c65 286c 696e  tile=np.tile(lin
+0000fe30: 6553 7472 656e 6774 6873 2c5b 6c65 6e28  eStrengths,[len(
+0000fe40: 6e75 292c 315d 290a 2020 2020 7065 7263  nu),1]).    perc
+0000fe50: 5f74 696c 653d 6750 6572 6328 6e75 5f74  _tile=gPerc(nu_t
+0000fe60: 696c 652c 6e75 5f69 6a5f 7469 6c65 2e54  ile,nu_ij_tile.T
+0000fe70: 2c6e 755f 696a 5f74 696c 652e 542f 632a  ,nu_ij_tile.T/c*
+0000fe80: 7672 290a 2020 2020 783d 7065 7263 5f74  vr).    x=perc_t
+0000fe90: 696c 655b 3a2c 3a2d 315d 2d70 6572 635f  ile[:,:-1]-perc_
+0000fea0: 7469 6c65 5b3a 2c31 3a5d 0a20 2020 2077  tile[:,1:].    w
+0000feb0: 6176 656c 656e 6774 682c 666c 7578 3d63  avelength,flux=c
+0000fec0: 2f6e 755b 3a2d 315d 2a31 6536 2c6e 702e  /nu[:-1]*1e6,np.
+0000fed0: 7375 6d28 782a 6c69 6e65 5374 7265 6e67  sum(x*lineStreng
+0000fee0: 7468 735f 7469 6c65 5b3a 2d31 2c3a 5d2e  ths_tile[:-1,:].
+0000fef0: 542c 6178 6973 3d30 292f 286e 755b 3a2d  T,axis=0)/(nu[:-
+0000ff00: 315d 2d6e 755b 313a 5d29 0a20 2020 2072  1]-nu[1:]).    r
+0000ff10: 6574 7572 6e20 7761 7665 6c65 6e67 7468  eturn wavelength
+0000ff20: 2c66 6c75 780a 0a0a 6465 6620 6765 6e65  ,flux...def gene
+0000ff30: 7261 6c43 6f6e 766f 6c76 6528 6c69 6e65  ralConvolve(line
+0000ff40: 5374 7265 6e67 7468 732c 6c69 6e65 4672  Strengths,lineFr
+0000ff50: 6571 2c52 3d31 2c6c 616d 6264 615f 303d  eq,R=1,lambda_0=
+0000ff60: 312c 6c61 6d62 6461 5f6e 3d31 2c52 5f62  1,lambda_n=1,R_b
+0000ff70: 6163 6b3d 3165 3629 3a0a 2020 2020 2222  ack=1e6):.    ""
+0000ff80: 220a 2020 2020 4675 6e63 7469 6f6e 2074  ".    Function t
+0000ff90: 6f20 636f 6e76 6f6c 7665 206c 696e 6520  o convolve line 
+0000ffa0: 666c 7578 6573 2069 6e74 6f20 6c69 6e65  fluxes into line
+0000ffb0: 2073 7065 6374 7261 2062 6173 6564 206f   spectra based o
+0000ffc0: 6e20 6120 7573 6572 2064 6566 696e 6564  n a user defined
+0000ffd0: 2073 7065 6374 7261 6c20 7265 736f 6c76   spectral resolv
+0000ffe0: 696e 6720 706f 7765 7220 520a 2020 2020  ing power R.    
+0000fff0: 2222 220a 2020 2020 6966 206c 616d 6264  """.    if lambd
+00010000: 615f 6e3d 3d6c 616d 6264 615f 303a 0a20  a_n==lambda_0:. 
+00010010: 2020 2020 2020 206c 616d 6264 615f 6e3d         lambda_n=
+00010020: 632f 6e70 2e61 6d69 6e28 6c69 6e65 4672  c/np.amin(lineFr
+00010030: 6571 292a 3165 2d33 2a32 0a20 2020 2066  eq)*1e-3*2.    f
+00010040: 7265 715f 6269 6e73 3d67 656e 6572 6174  req_bins=generat
+00010050: 655f 6772 6964 2852 5f62 6163 6b2c 6c61  e_grid(R_back,la
+00010060: 6d62 6461 5f30 2c6c 616d 6264 615f 6e29  mbda_0,lambda_n)
+00010070: 0a20 2020 2077 6176 655f 6269 6e73 3d63  .    wave_bins=c
+00010080: 2f66 7265 715f 6269 6e73 2a31 652d 330a  /freq_bins*1e-3.
+00010090: 2020 2020 666c 7578 5f62 696e 733d 7761      flux_bins=wa
+000100a0: 7665 5f62 696e 732a 302e 300a 2020 2020  ve_bins*0.0.    
+000100b0: 693d 360a 2020 2020 533d 6c69 6e65 5374  i=6.    S=lineSt
+000100c0: 7265 6e67 7468 730a 2020 2020 463d 6c69  rengths.    F=li
+000100d0: 6e65 4672 6571 0a20 2020 2069 6e64 3d6e  neFreq.    ind=n
+000100e0: 702e 6469 6769 7469 7a65 2846 2c6e 702e  p.digitize(F,np.
+000100f0: 666c 6970 2866 7265 715f 6269 6e73 295b  flip(freq_bins)[
+00010100: 3a2d 315d 290a 2020 2020 666f 7220 692c  :-1]).    for i,
+00010110: 6964 7820 696e 2065 6e75 6d65 7261 7465  idx in enumerate
+00010120: 2869 6e64 293a 0a20 2020 2020 2020 2066  (ind):.        f
+00010130: 6c75 785f 6269 6e73 5b69 6478 5d2b 3d53  lux_bins[idx]+=S
+00010140: 5b69 5d0a 0a20 2020 2046 5748 4d3d 525f  [i]..    FWHM=R_
+00010150: 6261 636b 2f52 2f32 2e33 3535 0a20 2020  back/R/2.355.   
+00010160: 2067 3d47 6175 7373 6961 6e31 444b 6572   g=Gaussian1DKer
+00010170: 6e65 6c28 7374 6464 6576 3d46 5748 4d2c  nel(stddev=FWHM,
+00010180: 6661 6374 6f72 3d37 290a 2020 2020 413d  factor=7).    A=
+00010190: 6170 795f 636f 6e76 6f6c 7665 2866 6c75  apy_convolve(flu
+000101a0: 785f 6269 6e73 2c67 290a 2020 2020 413d  x_bins,g).    A=
+000101b0: 415b 313a 5d2f 286e 702e 666c 6970 2866  A[1:]/(np.flip(f
+000101c0: 7265 715f 6269 6e73 295b 313a 5d2d 6e70  req_bins)[1:]-np
+000101d0: 2e66 6c69 7028 6672 6571 5f62 696e 7329  .flip(freq_bins)
+000101e0: 5b3a 2d31 5d29 2a31 652d 390a 2020 2020  [:-1])*1e-9.    
+000101f0: 573d 6e70 2e66 6c69 7028 7761 7665 5f62  W=np.flip(wave_b
+00010200: 696e 735b 313a 5d29 0a20 2020 2072 6574  ins[1:]).    ret
+00010210: 7572 6e20 6e70 2e66 6c69 7028 5729 2c6e  urn np.flip(W),n
+00010220: 702e 666c 6970 2841 290a 0a0a 6465 6620  p.flip(A)...def 
+00010230: 6765 6e65 7261 7465 5f67 7269 6428 523d  generate_grid(R=
+00010240: 312c 6c61 6d62 6461 5f30 3d31 2c6c 616d  1,lambda_0=1,lam
+00010250: 6264 615f 6e3d 312c 7361 6d70 6c69 6e67  bda_n=1,sampling
+00010260: 3d31 293a 0a20 2020 2022 2222 0a20 2020  =1):.    """.   
+00010270: 2047 656e 6572 6174 6520 6120 7370 6563   Generate a spec
+00010280: 7472 616c 2067 7269 6420 696e 2047 487a  tral grid in GHz
+00010290: 0a20 2020 2022 2222 0a20 2020 2064 656c  .    """.    del
+000102a0: 5f6c 6f67 6c61 6d3d 6e70 2e6c 6f67 3130  _loglam=np.log10
+000102b0: 2831 2e30 2b31 2e30 2f52 290a 2020 2020  (1.0+1.0/R).    
+000102c0: 4e3d 312b 696e 7428 6e70 2e6c 6f67 3130  N=1+int(np.log10
+000102d0: 286c 616d 6264 615f 6e2f 6c61 6d62 6461  (lambda_n/lambda
+000102e0: 5f30 292f 6465 6c5f 6c6f 676c 616d 290a  _0)/del_loglam).
+000102f0: 2020 2020 6d77 6c73 6c69 6e65 3d6e 702e      mwlsline=np.
+00010300: 6c6f 6773 7061 6365 286e 702e 6c6f 6731  logspace(np.log1
+00010310: 3028 6c61 6d62 6461 5f30 292c 6e70 2e6c  0(lambda_0),np.l
+00010320: 6f67 3130 286c 616d 6264 615f 6e29 2c69  og10(lambda_n),i
+00010330: 6e74 284e 2a73 616d 706c 696e 6729 290a  nt(N*sampling)).
+00010340: 2020 2020 6e75 3d63 2f6d 776c 736c 696e      nu=c/mwlslin
+00010350: 652a 3165 360a 2020 2020 7265 7475 726e  e*1e6.    return
+00010360: 286e 752a 3165 2d39 290a 0a0a 6465 6620  (nu*1e-9)...def 
+00010370: 636f 6e76 6f6c 7665 286d 6f64 656c 732c  convolve(models,
+00010380: 6672 6571 5f62 696e 733d 4e6f 6e65 2c52  freq_bins=None,R
+00010390: 3d31 2c6c 616d 6264 615f 303d 312c 6c61  =1,lambda_0=1,la
+000103a0: 6d62 6461 5f6e 3d31 2c76 723d 3133 3030  mbda_n=1,vr=1300
+000103b0: 2c4e 4c54 453d 4661 6c73 652c 636f 6e76  ,NLTE=False,conv
+000103c0: 5f74 7970 653d 312c 7665 7262 6f73 653d  _type=1,verbose=
+000103d0: 5472 7565 293a 0a20 2020 2022 2222 0a20  True):.    """. 
+000103e0: 2020 2053 616d 6520 6173 202e 636f 6e76     Same as .conv
+000103f0: 6f6c 7665 2829 206d 6574 686f 640a 2020  olve() method.  
+00010400: 2020 2222 220a 2020 2020 666f 7220 692c    """.    for i,
+00010410: 6420 696e 2065 6e75 6d65 7261 7465 286d  d in enumerate(m
+00010420: 6f64 656c 7329 3a0a 2020 2020 2020 2020  odels):.        
+00010430: 6966 2076 6572 626f 7365 3a20 7072 696e  if verbose: prin
+00010440: 7428 275c 6e5c 6e4d 6f64 656c 2027 2c69  t('\n\nModel ',i
+00010450: 2b31 290a 2020 2020 2020 2020 642e 636f  +1).        d.co
+00010460: 6e76 6f6c 7665 2866 7265 715f 6269 6e73  nvolve(freq_bins
+00010470: 3d66 7265 715f 6269 6e73 2c52 3d52 2c6c  =freq_bins,R=R,l
+00010480: 616d 6264 615f 303d 6c61 6d62 6461 5f30  ambda_0=lambda_0
+00010490: 2c6c 616d 6264 615f 6e3d 6c61 6d62 6461  ,lambda_n=lambda
+000104a0: 5f6e 2c76 723d 7672 2c4e 4c54 453d 4e4c  _n,vr=vr,NLTE=NL
+000104b0: 5445 2c63 6f6e 765f 7479 7065 3d63 6f6e  TE,conv_type=con
+000104c0: 765f 7479 7065 290a 2020 2020 7265 7475  v_type).    retu
+000104d0: 726e 206d 6f64 656c 730a 0a0a 6465 6620  rn models...def 
+000104e0: 6765 6e65 7261 7465 5f73 6c61 625f 6772  generate_slab_gr
+000104f0: 6964 2864 6972 6563 746f 7279 3d27 2e27  id(directory='.'
+00010500: 2c67 7269 645f 7061 7261 6d65 7465 7273  ,grid_parameters
+00010510: 3d7b 7d2c 636f 6d62 696e 6174 696f 6e3d  ={},combination=
+00010520: 4661 6c73 652c 4e74 6f74 3d4e 6f6e 652c  False,Ntot=None,
+00010530: 5467 3d4e 6f6e 652c 6e48 706c 7573 3d4e  Tg=None,nHplus=N
+00010540: 6f6e 652c 6e48 313d 4e6f 6e65 2c6e 4832  one,nH1=None,nH2
+00010550: 3d4e 6f6e 652c 6e48 653d 4e6f 6e65 2c6e  =None,nHe=None,n
+00010560: 656c 6563 3d4e 6f6e 652c 5464 3d4e 6f6e  elec=None,Td=Non
+00010570: 652c 7674 7572 623d 4e6f 6e65 2c64 7573  e,vturb=None,dus
+00010580: 745f 746f 5f67 6173 3d4e 6f6e 652c 525f  t_to_gas=None,R_
+00010590: 6f76 6572 6c61 703d 4e6f 6e65 2c6c 696e  overlap=None,lin
+000105a0: 655f 6f76 6572 6c61 703d 4e6f 6e65 2c73  e_overlap=None,s
+000105b0: 7065 6369 6573 5f6c 6973 743d 7b7d 2c6f  pecies_list={},o
+000105c0: 7574 7075 745f 6669 6c65 6e61 6d65 3d27  utput_filename='
+000105d0: 536c 6162 5265 7375 6c74 732e 6f75 7427  SlabResults.out'
+000105e0: 2c6f 7665 726c 6170 5f66 696c 656e 616d  ,overlap_filenam
+000105f0: 653d 2753 6c61 624f 7665 726c 6170 2e6f  e='SlabOverlap.o
+00010600: 7574 272c 7365 7061 7261 7465 5f6f 705f  ut',separate_op_
+00010610: 6669 6c65 733d 5472 7565 2c73 6c61 625f  files=True,slab_
+00010620: 5254 3d54 7275 652c 7368 6f72 745f 666f  RT=True,short_fo
+00010630: 726d 6174 3d46 616c 7365 2c6e 6f5f 696e  rmat=False,no_in
+00010640: 6469 7669 6475 616c 5f6c 696e 6573 3d46  dividual_lines=F
+00010650: 616c 7365 2c66 6974 735f 6f70 5f66 696c  alse,fits_op_fil
+00010660: 6573 3d46 616c 7365 293a 0a20 2020 2022  es=False):.    "
+00010670: 2222 0a20 2020 2046 756e 6374 696f 6e20  "".    Function 
+00010680: 746f 2067 656e 6572 6174 6520 536c 6162  to generate Slab
+00010690: 496e 7075 742e 696e 2069 6e70 7574 2066  Input.in input f
+000106a0: 696c 6520 636f 6e74 6169 6e69 6e67 2074  ile containing t
+000106b0: 6865 2064 6574 6169 6c73 206f 6620 7468  he details of th
+000106c0: 6520 736c 6162 206d 6f64 656c 2067 7269  e slab model gri
+000106d0: 640a 2020 2020 2222 220a 2020 2020 6e6d  d.    """.    nm
+000106e0: 6f64 656c 733d 310a 2020 2020 636f 6d62  odels=1.    comb
+000106f0: 696e 6174 696f 6e3d 4661 6c73 650a 2020  ination=False.  
+00010700: 2020 6966 206c 656e 2867 7269 645f 7061    if len(grid_pa
+00010710: 7261 6d65 7465 7273 293e 303a 0a20 2020  rameters)>0:.   
+00010720: 2020 2020 2069 6620 6e6f 7420 636f 6d62       if not comb
+00010730: 696e 6174 696f 6e3a 0a20 2020 2020 2020  ination:.       
+00010740: 2020 2020 206e 6d6f 6465 6c73 3d6c 656e       nmodels=len
+00010750: 2867 7269 645f 7061 7261 6d65 7465 7273  (grid_parameters
+00010760: 5b6c 6973 7428 6772 6964 5f70 6172 616d  [list(grid_param
+00010770: 6574 6572 732e 6b65 7973 2829 295b 305d  eters.keys())[0]
+00010780: 5d29 0a20 2020 2020 2020 2065 6c73 653a  ]).        else:
+00010790: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+000107a0: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
+000107b0: 6772 6964 5f70 6172 616d 6574 6572 7329  grid_parameters)
+000107c0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000107d0: 2020 206e 6d6f 6465 6c73 2a3d 6c65 6e28     nmodels*=len(
+000107e0: 6772 6964 5f70 6172 616d 6574 6572 735b  grid_parameters[
+000107f0: 6c69 7374 2867 7269 645f 7061 7261 6d65  list(grid_parame
+00010800: 7465 7273 2e6b 6579 7328 2929 5b69 5d5d  ters.keys())[i]]
+00010810: 290a 0a20 2020 204e 746f 745f 6c69 7374  )..    Ntot_list
+00010820: 3d6e 702e 6f6e 6573 2828 6e6d 6f64 656c  =np.ones((nmodel
+00010830: 7329 290a 2020 2020 5467 5f6c 6973 743d  s)).    Tg_list=
+00010840: 6e70 2e6f 6e65 7328 286e 6d6f 6465 6c73  np.ones((nmodels
+00010850: 2929 0a20 2020 206e 4870 6c75 735f 6c69  )).    nHplus_li
+00010860: 7374 3d6e 702e 6f6e 6573 2828 6e6d 6f64  st=np.ones((nmod
+00010870: 656c 7329 290a 2020 2020 6e48 315f 6c69  els)).    nH1_li
+00010880: 7374 3d6e 702e 6f6e 6573 2828 6e6d 6f64  st=np.ones((nmod
+00010890: 656c 7329 290a 2020 2020 6e48 325f 6c69  els)).    nH2_li
+000108a0: 7374 3d6e 702e 6f6e 6573 2828 6e6d 6f64  st=np.ones((nmod
+000108b0: 656c 7329 290a 2020 2020 6e48 655f 6c69  els)).    nHe_li
+000108c0: 7374 3d6e 702e 6f6e 6573 2828 6e6d 6f64  st=np.ones((nmod
+000108d0: 656c 7329 290a 2020 2020 6e65 6c65 635f  els)).    nelec_
+000108e0: 6c69 7374 3d6e 702e 6f6e 6573 2828 6e6d  list=np.ones((nm
+000108f0: 6f64 656c 7329 290a 2020 2020 5464 5f6c  odels)).    Td_l
+00010900: 6973 743d 6e70 2e6f 6e65 7328 286e 6d6f  ist=np.ones((nmo
+00010910: 6465 6c73 2929 0a20 2020 2076 7475 7262  dels)).    vturb
+00010920: 5f6c 6973 743d 6e70 2e6f 6e65 7328 286e  _list=np.ones((n
+00010930: 6d6f 6465 6c73 2929 0a20 2020 2064 7573  models)).    dus
+00010940: 745f 746f 5f67 6173 5f6c 6973 743d 6e70  t_to_gas_list=np
+00010950: 2e6f 6e65 7328 286e 6d6f 6465 6c73 2929  .ones((nmodels))
+00010960: 0a20 2020 2052 5f6f 7665 726c 6170 5f6c  .    R_overlap_l
+00010970: 6973 743d 6e70 2e6f 6e65 7328 286e 6d6f  ist=np.ones((nmo
+00010980: 6465 6c73 2929 0a20 2020 206c 696e 655f  dels)).    line_
+00010990: 6f76 6572 6c61 705f 6c69 7374 3d6e 702e  overlap_list=np.
+000109a0: 6f6e 6573 2828 6e6d 6f64 656c 732c 3229  ones((nmodels,2)
+000109b0: 290a 2020 2020 6966 206c 656e 2873 7065  ).    if len(spe
+000109c0: 6369 6573 5f6c 6973 7429 3c31 3a20 7261  cies_list)<1: ra
+000109d0: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
+000109e0: 5468 6520 7370 6563 6965 735f 6c69 7374  The species_list
+000109f0: 2063 616e 6e6f 7420 6265 2065 6d70 7479   cannot be empty
+00010a00: 2729 0a0a 2020 2020 6966 206e 6f74 2063  ')..    if not c
+00010a10: 6f6d 6269 6e61 7469 6f6e 3a0a 2020 2020  ombination:.    
+00010a20: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00010a30: 6765 286c 656e 2867 7269 645f 7061 7261  ge(len(grid_para
+00010a40: 6d65 7465 7273 2929 3a0a 2020 2020 2020  meters)):.      
+00010a50: 2020 2020 2020 6966 206c 6973 7428 6772        if list(gr
+00010a60: 6964 5f70 6172 616d 6574 6572 732e 6b65  id_parameters.ke
+00010a70: 7973 2829 295b 695d 3d3d 274e 746f 7427  ys())[i]=='Ntot'
+00010a80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00010a90: 2020 4e74 6f74 5f6c 6973 742a 3d67 7269    Ntot_list*=gri
+00010aa0: 645f 7061 7261 6d65 7465 7273 5b27 4e74  d_parameters['Nt
+00010ab0: 6f74 275d 0a20 2020 2020 2020 2020 2020  ot'].           
+00010ac0: 2065 6c69 6620 6c69 7374 2867 7269 645f   elif list(grid_
+00010ad0: 7061 7261 6d65 7465 7273 2e6b 6579 7328  parameters.keys(
+00010ae0: 2929 5b69 5d3d 3d27 5467 273a 0a20 2020  ))[i]=='Tg':.   
+00010af0: 2020 2020 2020 2020 2020 2020 2054 675f               Tg_
+00010b00: 6c69 7374 2a3d 6772 6964 5f70 6172 616d  list*=grid_param
+00010b10: 6574 6572 735b 2754 6727 5d0a 2020 2020  eters['Tg'].    
+00010b20: 2020 2020 2020 2020 656c 6966 206c 6973          elif lis
+00010b30: 7428 6772 6964 5f70 6172 616d 6574 6572  t(grid_parameter
+00010b40: 732e 6b65 7973 2829 295b 695d 3d3d 276e  s.keys())[i]=='n
+00010b50: 4870 6c75 7327 3a0a 2020 2020 2020 2020  Hplus':.        
+00010b60: 2020 2020 2020 2020 6e48 706c 7573 5f6c          nHplus_l
+00010b70: 6973 742a 3d67 7269 645f 7061 7261 6d65  ist*=grid_parame
+00010b80: 7465 7273 5b27 6e48 706c 7573 275d 0a20  ters['nHplus']. 
+00010b90: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00010ba0: 6c69 7374 2867 7269 645f 7061 7261 6d65  list(grid_parame
+00010bb0: 7465 7273 2e6b 6579 7328 2929 5b69 5d3d  ters.keys())[i]=
+00010bc0: 3d27 6e48 3127 3a0a 2020 2020 2020 2020  ='nH1':.        
+00010bd0: 2020 2020 2020 2020 6e48 315f 6c69 7374          nH1_list
+00010be0: 2a3d 6772 6964 5f70 6172 616d 6574 6572  *=grid_parameter
+00010bf0: 735b 276e 4831 275d 0a20 2020 2020 2020  s['nH1'].       
+00010c00: 2020 2020 2065 6c69 6620 6c69 7374 2867       elif list(g
+00010c10: 7269 645f 7061 7261 6d65 7465 7273 2e6b  rid_parameters.k
+00010c20: 6579 7328 2929 5b69 5d3d 3d27 6e48 3227  eys())[i]=='nH2'
+00010c30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00010c40: 2020 6e48 325f 6c69 7374 2a3d 6772 6964    nH2_list*=grid
+00010c50: 5f70 6172 616d 6574 6572 735b 276e 4832  _parameters['nH2
+00010c60: 275d 0a20 2020 2020 2020 2020 2020 2065  '].            e
+00010c70: 6c69 6620 6c69 7374 2867 7269 645f 7061  lif list(grid_pa
+00010c80: 7261 6d65 7465 7273 2e6b 6579 7328 2929  rameters.keys())
+00010c90: 5b69 5d3d 3d27 6e48 6527 3a0a 2020 2020  [i]=='nHe':.    
+00010ca0: 2020 2020 2020 2020 2020 2020 6e48 655f              nHe_
+00010cb0: 6c69 7374 2a3d 6772 6964 5f70 6172 616d  list*=grid_param
+00010cc0: 6574 6572 735b 276e 4865 275d 0a20 2020  eters['nHe'].   
+00010cd0: 2020 2020 2020 2020 2065 6c69 6620 6c69           elif li
+00010ce0: 7374 2867 7269 645f 7061 7261 6d65 7465  st(grid_paramete
+00010cf0: 7273 2e6b 6579 7328 2929 5b69 5d3d 3d27  rs.keys())[i]=='
+00010d00: 6e65 6c65 6327 3a0a 2020 2020 2020 2020  nelec':.        
+00010d10: 2020 2020 2020 2020 6e65 6c65 635f 6c69          nelec_li
+00010d20: 7374 2a3d 6772 6964 5f70 6172 616d 6574  st*=grid_paramet
+00010d30: 6572 735b 276e 656c 6563 275d 0a20 2020  ers['nelec'].   
+00010d40: 2020 2020 2020 2020 2065 6c69 6620 6c69           elif li
+00010d50: 7374 2867 7269 645f 7061 7261 6d65 7465  st(grid_paramete
+00010d60: 7273 2e6b 6579 7328 2929 5b69 5d3d 3d27  rs.keys())[i]=='
+00010d70: 5464 273a 0a20 2020 2020 2020 2020 2020  Td':.           
+00010d80: 2020 2020 2054 645f 6c69 7374 2a3d 6772       Td_list*=gr
+00010d90: 6964 5f70 6172 616d 6574 6572 735b 2754  id_parameters['T
+00010da0: 6427 5d0a 2020 2020 2020 2020 2020 2020  d'].            
+00010db0: 656c 6966 206c 6973 7428 6772 6964 5f70  elif list(grid_p
+00010dc0: 6172 616d 6574 6572 732e 6b65 7973 2829  arameters.keys()
+00010dd0: 295b 695d 3d3d 2776 7475 7262 273a 0a20  )[i]=='vturb':. 
+00010de0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+00010df0: 7475 7262 5f6c 6973 742a 3d67 7269 645f  turb_list*=grid_
+00010e00: 7061 7261 6d65 7465 7273 5b27 7674 7572  parameters['vtur
+00010e10: 6227 5d0a 2020 2020 2020 2020 2020 2020  b'].            
+00010e20: 656c 6966 206c 6973 7428 6772 6964 5f70  elif list(grid_p
+00010e30: 6172 616d 6574 6572 732e 6b65 7973 2829  arameters.keys()
+00010e40: 295b 695d 3d3d 2764 7573 745f 746f 5f67  )[i]=='dust_to_g
+00010e50: 6173 273a 0a20 2020 2020 2020 2020 2020  as':.           
+00010e60: 2020 2020 2064 7573 745f 746f 5f67 6173       dust_to_gas
+00010e70: 5f6c 6973 742a 3d67 7269 645f 7061 7261  _list*=grid_para
+00010e80: 6d65 7465 7273 5b27 6475 7374 5f74 6f5f  meters['dust_to_
+00010e90: 6761 7327 5d0a 2020 2020 2020 2020 2020  gas'].          
+00010ea0: 2020 656c 6966 206c 6973 7428 6772 6964    elif list(grid
+00010eb0: 5f70 6172 616d 6574 6572 732e 6b65 7973  _parameters.keys
+00010ec0: 2829 295b 695d 3d3d 2752 5f6f 7665 726c  ())[i]=='R_overl
+00010ed0: 6170 273a 0a20 2020 2020 2020 2020 2020  ap':.           
+00010ee0: 2020 2020 2052 5f6f 7665 726c 6170 5f6c       R_overlap_l
+00010ef0: 6973 742a 3d67 7269 645f 7061 7261 6d65  ist*=grid_parame
+00010f00: 7465 7273 5b27 525f 6f76 6572 6c61 7027  ters['R_overlap'
+00010f10: 5d0a 2020 2020 2020 2020 2020 2020 656c  ].            el
+00010f20: 6966 206c 6973 7428 6772 6964 5f70 6172  if list(grid_par
+00010f30: 616d 6574 6572 732e 6b65 7973 2829 295b  ameters.keys())[
+00010f40: 695d 3d3d 276c 696e 655f 6f76 6572 6c61  i]=='line_overla
+00010f50: 7027 3a0a 2020 2020 2020 2020 2020 2020  p':.            
+00010f60: 2020 2020 666f 7220 6a20 696e 2072 616e      for j in ran
+00010f70: 6765 286c 656e 2867 7269 645f 7061 7261  ge(len(grid_para
+00010f80: 6d65 7465 7273 5b27 6c69 6e65 5f6f 7665  meters['line_ove
+00010f90: 726c 6170 275d 2929 3a0a 2020 2020 2020  rlap'])):.      
+00010fa0: 2020 2020 2020 2020 2020 2020 2020 6c69                li
+00010fb0: 6e65 5f6f 7665 726c 6170 5f6c 6973 745b  ne_overlap_list[
+00010fc0: 6a2c 3a5d 3d6e 702e 6172 7261 7928 6772  j,:]=np.array(gr
+00010fd0: 6964 5f70 6172 616d 6574 6572 735b 276c  id_parameters['l
+00010fe0: 696e 655f 6f76 6572 6c61 7027 5d5b 6a5d  ine_overlap'][j]
+00010ff0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+00011000: 7365 3a20 7261 6973 6520 4b65 7945 7272  se: raise KeyErr
+00011010: 6f72 2866 2755 6e69 6465 6e74 6966 6965  or(f'Unidentifie
+00011020: 6420 6772 6964 2070 6172 616d 6574 6572  d grid parameter
+00011030: 207b 6c69 7374 2867 7269 645f 7061 7261   {list(grid_para
+00011040: 6d65 7465 7273 2e6b 6579 7328 2929 5b69  meters.keys())[i
+00011050: 5d7d 2729 0a20 2020 2065 6c73 653a 0a20  ]}').    else:. 
+00011060: 2020 2020 2020 2072 6169 7365 204b 6579         raise Key
+00011070: 4572 726f 7228 2743 6f6d 6269 6e61 7469  Error('Combinati
+00011080: 6f6e 2069 7320 7374 696c 6c20 6e6f 7420  on is still not 
+00011090: 7375 7070 6f72 7465 6427 290a 0a20 2020  supported')..   
+000110a0: 2069 6620 6e70 2e73 756d 284e 746f 745f   if np.sum(Ntot_
+000110b0: 6c69 7374 293d 3d6e 6d6f 6465 6c73 3a0a  list)==nmodels:.
+000110c0: 2020 2020 2020 2020 6966 206e 6f74 2028          if not (
+000110d0: 4e74 6f74 2020 2020 2020 2020 6973 204e  Ntot        is N
+000110e0: 6f6e 6529 3a0a 2020 2020 2020 2020 2020  one):.          
+000110f0: 2020 4e74 6f74 5f6c 6973 742a 3d4e 746f    Ntot_list*=Nto
+00011100: 740a 2020 2020 2020 2020 2320 656c 7365  t.        # else
+00011110: 3a0a 2020 2020 2020 2020 2320 2020 2020  :.        #     
+00011120: 4e74 6f74 5f6c 6973 742a 3d31 6531 350a  Ntot_list*=1e15.
+00011130: 2020 2020 6966 206e 702e 7375 6d28 5467      if np.sum(Tg
+00011140: 5f6c 6973 7429 3d3d 6e6d 6f64 656c 733a  _list)==nmodels:
+00011150: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00011160: 2854 6720 2020 2020 2020 2020 2069 7320  (Tg          is 
+00011170: 4e6f 6e65 293a 0a20 2020 2020 2020 2020  None):.         
+00011180: 2020 2054 675f 6c69 7374 2a3d 5467 0a20     Tg_list*=Tg. 
+00011190: 2020 2020 2020 2023 2065 6c73 653a 0a20         # else:. 
+000111a0: 2020 2020 2020 2023 2020 2020 2054 675f         #     Tg_
+000111b0: 6c69 7374 2a3d 3130 300a 2020 2020 6966  list*=100.    if
+000111c0: 206e 702e 7375 6d28 6e48 706c 7573 5f6c   np.sum(nHplus_l
+000111d0: 6973 7429 3d3d 6e6d 6f64 656c 733a 0a20  ist)==nmodels:. 
+000111e0: 2020 2020 2020 2069 6620 6e6f 7420 286e         if not (n
+000111f0: 4870 6c75 7320 2020 2020 2069 7320 4e6f  Hplus      is No
+00011200: 6e65 293a 0a20 2020 2020 2020 2020 2020  ne):.           
+00011210: 206e 4870 6c75 735f 6c69 7374 2a3d 6e48   nHplus_list*=nH
+00011220: 706c 7573 0a20 2020 2020 2020 2023 2065  plus.        # e
+00011230: 6c73 653a 0a20 2020 2020 2020 2023 2020  lse:.        #  
+00011240: 2020 206e 4870 6c75 735f 6c69 7374 2a3d     nHplus_list*=
+00011250: 3165 310a 2020 2020 6966 206e 702e 7375  1e1.    if np.su
+00011260: 6d28 6e48 315f 6c69 7374 293d 3d6e 6d6f  m(nH1_list)==nmo
+00011270: 6465 6c73 3a0a 2020 2020 2020 2020 6966  dels:.        if
+00011280: 206e 6f74 2028 6e48 3120 2020 2020 2020   not (nH1       
+00011290: 2020 6973 204e 6f6e 6529 3a0a 2020 2020    is None):.    
+000112a0: 2020 2020 2020 2020 6e48 315f 6c69 7374          nH1_list
+000112b0: 2a3d 6e48 310a 2020 2020 2020 2020 2320  *=nH1.        # 
+000112c0: 656c 7365 3a0a 2020 2020 2020 2020 2320  else:.        # 
+000112d0: 2020 2020 6e48 315f 6c69 7374 2a3d 3165      nH1_list*=1e
+000112e0: 3132 0a20 2020 2069 6620 6e70 2e73 756d  12.    if np.sum
+000112f0: 286e 4832 5f6c 6973 7429 3d3d 6e6d 6f64  (nH2_list)==nmod
+00011300: 656c 733a 0a20 2020 2020 2020 2069 6620  els:.        if 
+00011310: 6e6f 7420 286e 4832 2020 2020 2020 2020  not (nH2        
+00011320: 2069 7320 4e6f 6e65 293a 0a20 2020 2020   is None):.     
+00011330: 2020 2020 2020 206e 4832 5f6c 6973 742a         nH2_list*
+00011340: 3d6e 4832 0a20 2020 2020 2020 2023 2065  =nH2.        # e
+00011350: 6c73 653a 0a20 2020 2020 2020 2023 2020  lse:.        #  
+00011360: 2020 206e 4832 5f6c 6973 742a 3d31 6531     nH2_list*=1e1
+00011370: 320a 2020 2020 6966 206e 702e 7375 6d28  2.    if np.sum(
+00011380: 6e48 655f 6c69 7374 293d 3d6e 6d6f 6465  nHe_list)==nmode
+00011390: 6c73 3a0a 2020 2020 2020 2020 6966 206e  ls:.        if n
+000113a0: 6f74 2028 6e48 6520 2020 2020 2020 2020  ot (nHe         
+000113b0: 6973 204e 6f6e 6529 3a0a 2020 2020 2020  is None):.      
+000113c0: 2020 2020 2020 6e48 655f 6c69 7374 2a3d        nHe_list*=
+000113d0: 6e48 650a 2020 2020 2020 2020 2320 656c  nHe.        # el
+000113e0: 7365 3a0a 2020 2020 2020 2020 2320 2020  se:.        #   
+000113f0: 2020 6e48 655f 6c69 7374 2a3d 3165 3131    nHe_list*=1e11
+00011400: 0a20 2020 2069 6620 6e70 2e73 756d 286e  .    if np.sum(n
+00011410: 656c 6563 5f6c 6973 7429 3d3d 6e6d 6f64  elec_list)==nmod
+00011420: 656c 733a 0a20 2020 2020 2020 2069 6620  els:.        if 
+00011430: 6e6f 7420 286e 656c 6563 2020 2020 2020  not (nelec      
+00011440: 2069 7320 4e6f 6e65 293a 0a20 2020 2020   is None):.     
+00011450: 2020 2020 2020 206e 656c 6563 5f6c 6973         nelec_lis
+00011460: 742a 3d6e 656c 6563 0a20 2020 2020 2020  t*=nelec.       
+00011470: 2023 2065 6c73 653a 0a20 2020 2020 2020   # else:.       
+00011480: 2023 2020 2020 206e 656c 6563 5f6c 6973   #     nelec_lis
+00011490: 742a 3d31 6538 0a20 2020 2069 6620 6e70  t*=1e8.    if np
+000114a0: 2e73 756d 2854 645f 6c69 7374 293d 3d6e  .sum(Td_list)==n
+000114b0: 6d6f 6465 6c73 3a0a 2020 2020 2020 2020  models:.        
+000114c0: 6966 206e 6f74 2028 5464 2020 2020 2020  if not (Td      
+000114d0: 2020 2020 6973 204e 6f6e 6529 3a0a 2020      is None):.  
+000114e0: 2020 2020 2020 2020 2020 5464 5f6c 6973            Td_lis
+000114f0: 742a 3d54 640a 2020 2020 2020 2020 2320  t*=Td.        # 
+00011500: 656c 7365 3a0a 2020 2020 2020 2020 2320  else:.        # 
+00011510: 2020 2020 5464 5f6c 6973 742a 3d31 300a      Td_list*=10.
+00011520: 2020 2020 6966 206e 702e 7375 6d28 7674      if np.sum(vt
+00011530: 7572 625f 6c69 7374 293d 3d6e 6d6f 6465  urb_list)==nmode
+00011540: 6c73 3a0a 2020 2020 2020 2020 6966 206e  ls:.        if n
+00011550: 6f74 2028 7674 7572 6220 2020 2020 2020  ot (vturb       
+00011560: 6973 204e 6f6e 6529 3a0a 2020 2020 2020  is None):.      
+00011570: 2020 2020 2020 7674 7572 625f 6c69 7374        vturb_list
+00011580: 2a3d 7674 7572 620a 2020 2020 2020 2020  *=vturb.        
+00011590: 2320 656c 7365 3a0a 2020 2020 2020 2020  # else:.        
+000115a0: 2320 2020 2020 7674 7572 625f 6c69 7374  #     vturb_list
+000115b0: 2a3d 312e 340a 2020 2020 6966 206e 702e  *=1.4.    if np.
+000115c0: 7375 6d28 6475 7374 5f74 6f5f 6761 735f  sum(dust_to_gas_
+000115d0: 6c69 7374 293d 3d6e 6d6f 6465 6c73 3a0a  list)==nmodels:.
+000115e0: 2020 2020 2020 2020 6966 206e 6f74 2028          if not (
+000115f0: 6475 7374 5f74 6f5f 6761 7320 6973 204e  dust_to_gas is N
+00011600: 6f6e 6529 3a0a 2020 2020 2020 2020 2020  one):.          
+00011610: 2020 6475 7374 5f74 6f5f 6761 735f 6c69    dust_to_gas_li
+00011620: 7374 2a3d 6475 7374 5f74 6f5f 6761 730a  st*=dust_to_gas.
+00011630: 2020 2020 2020 2020 2320 656c 7365 3a0a          # else:.
+00011640: 2020 2020 2020 2020 2320 2020 2020 6475          #     du
+00011650: 7374 5f74 6f5f 6761 735f 6c69 7374 2a3d  st_to_gas_list*=
+00011660: 3165 2d32 310a 2020 2020 6966 206e 702e  1e-21.    if np.
+00011670: 7375 6d28 525f 6f76 6572 6c61 705f 6c69  sum(R_overlap_li
+00011680: 7374 293d 3d6e 6d6f 6465 6c73 3a0a 2020  st)==nmodels:.  
+00011690: 2020 2020 2020 6966 206e 6f74 2028 525f        if not (R_
+000116a0: 6f76 6572 6c61 7020 6973 204e 6f6e 6529  overlap is None)
+000116b0: 3a0a 2020 2020 2020 2020 2020 2020 525f  :.            R_
+000116c0: 6f76 6572 6c61 705f 6c69 7374 2a3d 525f  overlap_list*=R_
+000116d0: 6f76 6572 6c61 700a 2020 2020 2020 2020  overlap.        
+000116e0: 2320 656c 7365 3a0a 2020 2020 2020 2020  # else:.        
+000116f0: 2320 2020 2020 525f 6f76 6572 6c61 705f  #     R_overlap_
+00011700: 6c69 7374 2a3d 3165 350a 2020 2020 6966  list*=1e5.    if
+00011710: 206e 702e 7375 6d28 6c69 6e65 5f6f 7665   np.sum(line_ove
+00011720: 726c 6170 5f6c 6973 7429 3d3d 322a 6e6d  rlap_list)==2*nm
+00011730: 6f64 656c 733a 0a20 2020 2020 2020 2069  odels:.        i
+00011740: 6620 6e6f 7420 286c 696e 655f 6f76 6572  f not (line_over
+00011750: 6c61 7020 6973 204e 6f6e 6529 3a0a 2020  lap is None):.  
+00011760: 2020 2020 2020 2020 2020 6c69 6e65 5f6f            line_o
+00011770: 7665 726c 6170 5f6c 6973 742a 3d6e 702e  verlap_list*=np.
+00011780: 6172 7261 7928 6c69 6e65 5f6f 7665 726c  array(line_overl
+00011790: 6170 290a 2020 2020 2020 2020 2320 656c  ap).        # el
+000117a0: 7365 3a0a 2020 2020 2020 2020 2320 2020  se:.        #   
+000117b0: 2020 6c69 6e65 5f6f 7665 726c 6170 5f6c    line_overlap_l
+000117c0: 6973 742a 3d6e 702e 6172 7261 7928 2834  ist*=np.array((4
+000117d0: 2c33 3029 290a 0a20 2020 206f 732e 7379  ,30))..    os.sy
+000117e0: 7374 656d 2866 2774 6f75 6368 207b 6469  stem(f'touch {di
+000117f0: 7265 6374 6f72 792b 222f 536c 6162 496e  rectory+"/SlabIn
+00011800: 7075 742e 696e 227d 2729 0a20 2020 2066  put.in"}').    f
+00011810: 3d6f 7065 6e28 6469 7265 6374 6f72 792b  =open(directory+
+00011820: 272f 536c 6162 496e 7075 742e 696e 272c  '/SlabInput.in',
+00011830: 2777 2729 0a20 2020 2066 2e77 7269 7465  'w').    f.write
+00011840: 2822 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ("**************
+00011850: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00011860: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00011870: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a5c 6e22  *************\n"
+00011880: 290a 2020 2020 662e 7772 6974 6528 222a  ).    f.write("*
+00011890: 2a2a 2049 6e70 7574 2066 696c 6520 666f  ** Input file fo
+000118a0: 7220 736c 6162 2065 7363 6170 6520 7072  r slab escape pr
+000118b0: 6f62 6162 696c 6974 7920 7769 7468 2050  obability with P
+000118c0: 726f 4469 4d6f 202a 2a2a 5c6e 2229 0a20  roDiMo ***\n"). 
+000118d0: 2020 2066 2e77 7269 7465 2822 2a2a 2a2a     f.write("****
+000118e0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+000118f0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00011900: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00011910: 2a2a 2a2a 2a2a 2a5c 6e22 290a 2020 2020  *******\n").    
+00011920: 662e 7772 6974 6528 222a 2a2a 206e 6d6f  f.write("*** nmo
+00011930: 6465 6c73 2073 686f 756c 6420 666f 6c6c  dels should foll
+00011940: 6f77 206f 7574 7075 745f 6669 6c65 6e61  ow output_filena
+00011950: 6d65 202a 2a2a 5c6e 2229 0a20 2020 2066  me ***\n").    f
+00011960: 2e77 7269 7465 2866 277b 6f75 7470 7574  .write(f'{output
+00011970: 5f66 696c 656e 616d 657d 2021 206f 7574  _filename} ! out
+00011980: 7075 745f 6669 6c65 6e61 6d65 5c6e 2729  put_filename\n')
+00011990: 0a20 2020 2066 2e77 7269 7465 2866 277b  .    f.write(f'{
+000119a0: 6f76 6572 6c61 705f 6669 6c65 6e61 6d65  overlap_filename
+000119b0: 7d20 2120 6f76 6572 6c61 705f 6669 6c65  } ! overlap_file
+000119c0: 6e61 6d65 5c6e 2729 0a20 2020 2069 6620  name\n').    if 
+000119d0: 7365 7061 7261 7465 5f6f 705f 6669 6c65  separate_op_file
+000119e0: 733a 0a20 2020 2020 2020 2066 2e77 7269  s:.        f.wri
+000119f0: 7465 2827 2e74 7275 652e 2020 2020 2120  te('.true.    ! 
+00011a00: 7365 7061 7261 7465 5f6f 705f 6669 6c65  separate_op_file
+00011a10: 735c 6e27 290a 2020 2020 656c 7365 3a0a  s\n').    else:.
+00011a20: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
+00011a30: 272e 6661 6c73 652e 2020 2021 2073 6570  '.false.   ! sep
+00011a40: 6172 6174 655f 6f70 5f66 696c 6573 5c6e  arate_op_files\n
+00011a50: 2729 0a20 2020 2069 6620 6669 7473 5f6f  ').    if fits_o
+00011a60: 705f 6669 6c65 733a 0a20 2020 2020 2020  p_files:.       
+00011a70: 2066 2e77 7269 7465 2827 2e74 7275 652e   f.write('.true.
+00011a80: 2020 2020 2120 6669 7473 5f6f 705f 6669      ! fits_op_fi
+00011a90: 6c65 735c 6e27 290a 2020 2020 656c 7365  les\n').    else
+00011aa0: 3a0a 2020 2020 2020 2020 662e 7772 6974  :.        f.writ
+00011ab0: 6528 272e 6661 6c73 652e 2020 2021 2066  e('.false.   ! f
+00011ac0: 6974 735f 6f70 5f66 696c 6573 5c6e 2729  its_op_files\n')
+00011ad0: 0a20 2020 2069 6620 6e6f 5f69 6e64 6976  .    if no_indiv
+00011ae0: 6964 7561 6c5f 6c69 6e65 733a 0a20 2020  idual_lines:.   
+00011af0: 2020 2020 2066 2e77 7269 7465 2827 2e74       f.write('.t
+00011b00: 7275 652e 2020 2020 2120 6e6f 5f69 6e64  rue.    ! no_ind
+00011b10: 6976 6964 7561 6c5f 6c69 6e65 735c 6e27  ividual_lines\n'
+00011b20: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
+00011b30: 2020 2020 662e 7772 6974 6528 272e 6661      f.write('.fa
+00011b40: 6c73 652e 2020 2021 206e 6f5f 696e 6469  lse.   ! no_indi
+00011b50: 7669 6475 616c 5f6c 696e 6573 5c6e 2729  vidual_lines\n')
+00011b60: 0a20 2020 2069 6620 736c 6162 5f52 543a  .    if slab_RT:
+00011b70: 0a20 2020 2020 2020 2066 2e77 7269 7465  .        f.write
+00011b80: 2827 2e74 7275 652e 2020 2020 2120 736c  ('.true.    ! sl
+00011b90: 6162 5f52 5420 5c6e 2729 0a20 2020 2065  ab_RT \n').    e
+00011ba0: 6c73 653a 0a20 2020 2020 2020 2066 2e77  lse:.        f.w
+00011bb0: 7269 7465 2827 2e66 616c 7365 2e20 2020  rite('.false.   
+00011bc0: 2120 736c 6162 5f52 5420 5c6e 2729 0a20  ! slab_RT \n'). 
+00011bd0: 2020 2069 6620 7368 6f72 745f 666f 726d     if short_form
+00011be0: 6174 3a0a 2020 2020 2020 2020 662e 7772  at:.        f.wr
+00011bf0: 6974 6528 272e 7472 7565 2e20 2020 2021  ite('.true.    !
+00011c00: 2073 686f 7274 5f66 6f72 6d61 745c 6e27   short_format\n'
+00011c10: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
+00011c20: 2020 2020 662e 7772 6974 6528 272e 6661      f.write('.fa
+00011c30: 6c73 652e 2020 2021 2073 686f 7274 5f66  lse.   ! short_f
+00011c40: 6f72 6d61 745c 6e27 290a 2020 2020 662e  ormat\n').    f.
+00011c50: 7772 6974 6528 6627 7b6e 6d6f 6465 6c73  write(f'{nmodels
+00011c60: 7d20 2020 2020 2020 2020 2020 2020 2120  }             ! 
+00011c70: 6e6d 6f64 656c 735c 6e27 290a 2020 2020  nmodels\n').    
+00011c80: 662e 7772 6974 6528 272d 2d2d 2d2d 2d2d  f.write('-------
+00011c90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00011ca0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00011cb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00011cc0: 2d2d 2d2d 2d2d 2d2d 2d27 290a 2020 2020  ---------').    
-00011cd0: 662e 636c 6f73 6528 290a 2020 2020 7265  f.close().    re
-00011ce0: 7475 726e 0a0a 0a64 6566 2067 656e 6572  turn...def gener
-00011cf0: 6174 655f 3144 5f73 7472 7563 7475 7265  ate_1D_structure
-00011d00: 2864 7a2c 7370 6563 6965 735f 6c69 7374  (dz,species_list
-00011d10: 2c76 7475 7262 2c6e 642c 5464 2c6e 5f73  ,vturb,nd,Td,n_s
-00011d20: 7065 6369 6573 2c54 5f73 7065 6369 6573  pecies,T_species
-00011d30: 2c6e 4832 3d30 2c6e 4849 3d30 2c6e 4849  ,nH2=0,nHI=0,nHI
-00011d40: 493d 302c 6e48 653d 302c 6e65 6c65 633d  I=0,nHe=0,nelec=
-00011d50: 302c 6669 6c65 6e61 6d65 3d27 3144 5f73  0,filename='1D_s
-00011d60: 7472 7563 7475 7265 2729 3a0a 2020 2020  tructure'):.    
-00011d70: 2222 220a 2020 2020 4765 6e65 7261 7465  """.    Generate
-00011d80: 7320 3144 2073 7472 7563 7475 7265 2066  s 1D structure f
-00011d90: 696c 6520 7265 7175 6972 6564 2066 6f72  ile required for
-00011da0: 2031 4420 736c 6162 206d 6f64 656c 730a   1D slab models.
-00011db0: 2020 2020 2222 220a 2020 2020 6966 2069      """.    if i
-00011dc0: 7369 6e73 7461 6e63 6528 647a 2c66 6c6f  sinstance(dz,flo
-00011dd0: 6174 2920 6f72 2069 7369 6e73 7461 6e63  at) or isinstanc
-00011de0: 6528 647a 2c69 6e74 293a 2064 7a3d 6e70  e(dz,int): dz=np
-00011df0: 2e61 7272 6179 285b 647a 5d29 0a20 2020  .array([dz]).   
-00011e00: 2069 6620 6973 696e 7374 616e 6365 2864   if isinstance(d
-00011e10: 7a2c 6c69 7374 293a 2064 7a3d 6e70 2e61  z,list): dz=np.a
-00011e20: 7272 6179 2864 7a29 0a20 2020 2069 6620  rray(dz).    if 
-00011e30: 6973 696e 7374 616e 6365 2873 7065 6369  isinstance(speci
-00011e40: 6573 5f6c 6973 742c 7374 7229 3a20 7370  es_list,str): sp
-00011e50: 6563 6965 735f 6c69 7374 3d5b 7370 6563  ecies_list=[spec
-00011e60: 6965 735f 6c69 7374 5d0a 2020 2020 6966  ies_list].    if
-00011e70: 2069 7369 6e73 7461 6e63 6528 7674 7572   isinstance(vtur
-00011e80: 622c 666c 6f61 7429 206f 7220 6973 696e  b,float) or isin
-00011e90: 7374 616e 6365 2876 7475 7262 2c69 6e74  stance(vturb,int
-00011ea0: 293a 2076 7475 7262 3d6e 702e 6f6e 6573  ): vturb=np.ones
-00011eb0: 5f6c 696b 6528 647a 292a 7674 7572 620a  _like(dz)*vturb.
-00011ec0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00011ed0: 6528 6e64 2c66 6c6f 6174 2920 6f72 2069  e(nd,float) or i
-00011ee0: 7369 6e73 7461 6e63 6528 6e64 2c69 6e74  sinstance(nd,int
-00011ef0: 293a 206e 643d 6e70 2e6f 6e65 735f 6c69  ): nd=np.ones_li
-00011f00: 6b65 2864 7a29 2a6e 640a 2020 2020 6966  ke(dz)*nd.    if
-00011f10: 2069 7369 6e73 7461 6e63 6528 5464 2c66   isinstance(Td,f
-00011f20: 6c6f 6174 2920 6f72 2069 7369 6e73 7461  loat) or isinsta
-00011f30: 6e63 6528 5464 2c69 6e74 293a 2054 643d  nce(Td,int): Td=
-00011f40: 6e70 2e6f 6e65 735f 6c69 6b65 2864 7a29  np.ones_like(dz)
-00011f50: 2a54 640a 2020 2020 6966 2069 7369 6e73  *Td.    if isins
-00011f60: 7461 6e63 6528 6e48 322c 666c 6f61 7429  tance(nH2,float)
-00011f70: 206f 7220 6973 696e 7374 616e 6365 286e   or isinstance(n
-00011f80: 4832 2c69 6e74 293a 206e 4832 3d6e 702e  H2,int): nH2=np.
-00011f90: 6f6e 6573 5f6c 696b 6528 647a 292a 6e48  ones_like(dz)*nH
-00011fa0: 320a 2020 2020 6966 2069 7369 6e73 7461  2.    if isinsta
-00011fb0: 6e63 6528 6e48 492c 666c 6f61 7429 206f  nce(nHI,float) o
-00011fc0: 7220 6973 696e 7374 616e 6365 286e 4849  r isinstance(nHI
-00011fd0: 2c69 6e74 293a 206e 4849 3d6e 702e 6f6e  ,int): nHI=np.on
-00011fe0: 6573 5f6c 696b 6528 647a 292a 6e48 490a  es_like(dz)*nHI.
-00011ff0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00012000: 6528 6e48 4949 2c66 6c6f 6174 2920 6f72  e(nHII,float) or
-00012010: 2069 7369 6e73 7461 6e63 6528 6e48 4949   isinstance(nHII
-00012020: 2c69 6e74 293a 206e 4849 493d 6e70 2e6f  ,int): nHII=np.o
-00012030: 6e65 735f 6c69 6b65 2864 7a29 2a6e 4849  nes_like(dz)*nHI
-00012040: 490a 2020 2020 6966 2069 7369 6e73 7461  I.    if isinsta
-00012050: 6e63 6528 6e48 652c 666c 6f61 7429 206f  nce(nHe,float) o
-00012060: 7220 6973 696e 7374 616e 6365 286e 4865  r isinstance(nHe
-00012070: 2c69 6e74 293a 206e 4865 3d6e 702e 6f6e  ,int): nHe=np.on
-00012080: 6573 5f6c 696b 6528 647a 292a 6e48 650a  es_like(dz)*nHe.
-00012090: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-000120a0: 6528 6e65 6c65 632c 666c 6f61 7429 206f  e(nelec,float) o
-000120b0: 7220 6973 696e 7374 616e 6365 286e 656c  r isinstance(nel
-000120c0: 6563 2c69 6e74 293a 206e 656c 6563 3d6e  ec,int): nelec=n
-000120d0: 702e 6f6e 6573 5f6c 696b 6528 647a 292a  p.ones_like(dz)*
-000120e0: 6e65 6c65 630a 2020 2020 6966 2069 7369  nelec.    if isi
-000120f0: 6e73 7461 6e63 6528 6e5f 7370 6563 6965  nstance(n_specie
-00012100: 732c 666c 6f61 7429 206f 7220 6973 696e  s,float) or isin
-00012110: 7374 616e 6365 286e 5f73 7065 6369 6573  stance(n_species
-00012120: 2c69 6e74 293a 206e 5f73 7065 6369 6573  ,int): n_species
-00012130: 3d6e 702e 6f6e 6573 2828 647a 2e73 6861  =np.ones((dz.sha
-00012140: 7065 5b30 5d2c 6c65 6e28 7370 6563 6965  pe[0],len(specie
-00012150: 735f 6c69 7374 2929 292a 6e5f 7370 6563  s_list)))*n_spec
-00012160: 6965 730a 2020 2020 6966 2069 7369 6e73  ies.    if isins
-00012170: 7461 6e63 6528 545f 7370 6563 6965 732c  tance(T_species,
-00012180: 666c 6f61 7429 206f 7220 6973 696e 7374  float) or isinst
-00012190: 616e 6365 2854 5f73 7065 6369 6573 2c69  ance(T_species,i
-000121a0: 6e74 293a 2054 5f73 7065 6369 6573 3d6e  nt): T_species=n
-000121b0: 702e 6f6e 6573 2828 647a 2e73 6861 7065  p.ones((dz.shape
-000121c0: 5b30 5d2c 6c65 6e28 7370 6563 6965 735f  [0],len(species_
-000121d0: 6c69 7374 2929 292a 545f 7370 6563 6965  list)))*T_specie
-000121e0: 730a 2020 2020 6966 2069 7369 6e73 7461  s.    if isinsta
-000121f0: 6e63 6528 545f 7370 6563 6965 732c 6c69  nce(T_species,li
-00012200: 7374 293a 2054 5f73 7065 6369 6573 3d6e  st): T_species=n
-00012210: 702e 6172 7261 7928 545f 7370 6563 6965  p.array(T_specie
-00012220: 7329 0a20 2020 2069 6620 6973 696e 7374  s).    if isinst
-00012230: 616e 6365 286e 5f73 7065 6369 6573 2c6c  ance(n_species,l
-00012240: 6973 7429 3a20 6e5f 7370 6563 6965 733d  ist): n_species=
-00012250: 6e70 2e61 7272 6179 286e 5f73 7065 6369  np.array(n_speci
-00012260: 6573 290a 2020 2020 6966 206e 702e 6172  es).    if np.ar
-00012270: 7261 7928 545f 7370 6563 6965 7329 2e73  ray(T_species).s
-00012280: 697a 653d 3d6c 656e 2873 7065 6369 6573  ize==len(species
-00012290: 5f6c 6973 7429 3a0a 2020 2020 2020 2020  _list):.        
-000122a0: 545f 7370 6563 6965 735f 7465 6d70 3d6e  T_species_temp=n
-000122b0: 702e 6f6e 6573 2828 647a 2e73 6861 7065  p.ones((dz.shape
-000122c0: 5b30 5d2c 6c65 6e28 7370 6563 6965 735f  [0],len(species_
-000122d0: 6c69 7374 2929 290a 2020 2020 2020 2020  list))).        
-000122e0: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
-000122f0: 656e 2873 7065 6369 6573 5f6c 6973 7429  en(species_list)
-00012300: 293a 0a20 2020 2020 2020 2020 2020 2054  ):.            T
-00012310: 5f73 7065 6369 6573 5f74 656d 705b 3a2c  _species_temp[:,
-00012320: 695d 3d54 5f73 7065 6369 6573 5b69 5d0a  i]=T_species[i].
-00012330: 2020 2020 2020 2020 545f 7370 6563 6965          T_specie
-00012340: 733d 545f 7370 6563 6965 735f 7465 6d70  s=T_species_temp
-00012350: 2a31 2e30 300a 2020 2020 6966 206e 702e  *1.00.    if np.
-00012360: 6172 7261 7928 6e5f 7370 6563 6965 7329  array(n_species)
-00012370: 2e73 697a 653d 3d6c 656e 2873 7065 6369  .size==len(speci
-00012380: 6573 5f6c 6973 7429 3a0a 2020 2020 2020  es_list):.      
-00012390: 2020 6e5f 7370 6563 6965 735f 7465 6d70    n_species_temp
-000123a0: 3d6e 702e 6f6e 6573 2828 647a 2e73 6861  =np.ones((dz.sha
-000123b0: 7065 5b30 5d2c 6c65 6e28 7370 6563 6965  pe[0],len(specie
-000123c0: 735f 6c69 7374 2929 290a 2020 2020 2020  s_list))).      
-000123d0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-000123e0: 286c 656e 2873 7065 6369 6573 5f6c 6973  (len(species_lis
-000123f0: 7429 293a 0a20 2020 2020 2020 2020 2020  t)):.           
-00012400: 206e 5f73 7065 6369 6573 5f74 656d 705b   n_species_temp[
-00012410: 3a2c 695d 3d6e 5f73 7065 6369 6573 5b69  :,i]=n_species[i
-00012420: 5d0a 2020 2020 2020 2020 6e5f 7370 6563  ].        n_spec
-00012430: 6965 733d 6e5f 7370 6563 6965 735f 7465  ies=n_species_te
-00012440: 6d70 2a31 2e30 300a 0a20 2020 2077 6974  mp*1.00..    wit
-00012450: 6820 6f70 656e 2866 696c 656e 616d 652c  h open(filename,
-00012460: 2777 2729 2061 7320 663a 0a20 2020 2020  'w') as f:.     
-00012470: 2020 2066 2e77 7269 7465 2866 277b 6c65     f.write(f'{le
-00012480: 6e28 647a 293a 647d 5c6e 2729 0a20 2020  n(dz):d}\n').   
-00012490: 2020 2020 2066 2e77 7269 7465 2866 277b       f.write(f'{
-000124a0: 6c65 6e28 7370 6563 6965 735f 6c69 7374  len(species_list
-000124b0: 293a 647d 5c6e 2729 0a20 2020 2020 2020  ):d}\n').       
-000124c0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-000124d0: 6c65 6e28 7370 6563 6965 735f 6c69 7374  len(species_list
-000124e0: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-000124f0: 662e 7772 6974 6528 7370 6563 6965 735f  f.write(species_
-00012500: 6c69 7374 5b69 5d2b 275c 6e27 290a 2020  list[i]+'\n').  
-00012510: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-00012520: 616e 6765 286c 656e 2864 7a29 293a 0a20  ange(len(dz)):. 
-00012530: 2020 2020 2020 2020 2020 2073 7472 696e             strin
-00012540: 673d 2727 0a20 2020 2020 2020 2020 2020  g=''.           
-00012550: 2073 7472 696e 672b 3d66 277b 692b 313a   string+=f'{i+1:
-00012560: 647d 2020 270a 2020 2020 2020 2020 2020  d}  '.          
-00012570: 2020 7374 7269 6e67 2b3d 6627 7b64 7a5b    string+=f'{dz[
-00012580: 695d 3a2e 3365 7d20 2027 0a20 2020 2020  i]:.3e}  '.     
-00012590: 2020 2020 2020 2073 7472 696e 672b 3d66         string+=f
-000125a0: 277b 7674 7572 625b 695d 3a2e 3366 7d20  '{vturb[i]:.3f} 
-000125b0: 2027 0a20 2020 2020 2020 2020 2020 2073   '.            s
-000125c0: 7472 696e 672b 3d66 277b 6e64 5b69 5d3a  tring+=f'{nd[i]:
-000125d0: 2e33 657d 2020 270a 2020 2020 2020 2020  .3e}  '.        
-000125e0: 2020 2020 7374 7269 6e67 2b3d 6627 7b54      string+=f'{T
-000125f0: 645b 695d 3a2e 3366 7d20 2027 0a20 2020  d[i]:.3f}  '.   
-00012600: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
-00012610: 6e20 7261 6e67 6528 6c65 6e28 7370 6563  n range(len(spec
-00012620: 6965 735f 6c69 7374 2929 3a0a 2020 2020  ies_list)):.    
-00012630: 2020 2020 2020 2020 2020 2020 7374 7269              stri
-00012640: 6e67 2b3d 6627 7b6e 5f73 7065 6369 6573  ng+=f'{n_species
-00012650: 5b69 2c6a 5d3a 2e33 657d 2020 270a 2020  [i,j]:.3e}  '.  
-00012660: 2020 2020 2020 2020 2020 666f 7220 6a20            for j 
-00012670: 696e 2072 616e 6765 286c 656e 2873 7065  in range(len(spe
-00012680: 6369 6573 5f6c 6973 7429 293a 0a20 2020  cies_list)):.   
-00012690: 2020 2020 2020 2020 2020 2020 2073 7472               str
-000126a0: 696e 672b 3d66 277b 545f 7370 6563 6965  ing+=f'{T_specie
-000126b0: 735b 692c 6a5d 3a2e 3366 7d20 2027 0a20  s[i,j]:.3f}  '. 
-000126c0: 2020 2020 2020 2020 2020 2073 7472 696e             strin
-000126d0: 672b 3d66 277b 6e48 325b 695d 3a2e 3365  g+=f'{nH2[i]:.3e
-000126e0: 7d20 2027 0a20 2020 2020 2020 2020 2020  }  '.           
-000126f0: 2073 7472 696e 672b 3d66 277b 6e48 495b   string+=f'{nHI[
-00012700: 695d 3a2e 3365 7d20 2027 0a20 2020 2020  i]:.3e}  '.     
-00012710: 2020 2020 2020 2073 7472 696e 672b 3d66         string+=f
-00012720: 277b 6e48 4949 5b69 5d3a 2e33 657d 2020  '{nHII[i]:.3e}  
-00012730: 270a 2020 2020 2020 2020 2020 2020 7374  '.            st
-00012740: 7269 6e67 2b3d 6627 7b6e 4865 5b69 5d3a  ring+=f'{nHe[i]:
-00012750: 2e33 657d 2020 270a 2020 2020 2020 2020  .3e}  '.        
-00012760: 2020 2020 7374 7269 6e67 2b3d 6627 7b6e      string+=f'{n
-00012770: 656c 6563 5b69 5d3a 2e33 657d 2020 270a  elec[i]:.3e}  '.
-00012780: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
-00012790: 6974 6528 7374 7269 6e67 2b27 5c6e 2729  ite(string+'\n')
-000127a0: 0a20 2020 2020 2020 2066 2e63 6c6f 7365  .        f.close
-000127b0: 2829 0a0a 0a63 6c61 7373 204d 7946 6f72  ()...class MyFor
-000127c0: 6d61 7474 6572 2873 7472 696e 672e 466f  matter(string.Fo
-000127d0: 726d 6174 7465 7229 3a0a 2020 2020 2222  rmatter):.    ""
-000127e0: 220a 2020 2020 5374 7269 6e67 2066 6f72  ".    String for
-000127f0: 6d61 7474 6572 2066 6f72 2070 726f 6475  matter for produ
-00012800: 6369 6e67 2069 6e70 7574 2066 696c 6573  cing input files
-00012810: 0a20 2020 2022 2222 0a0a 2020 2020 6465  .    """..    de
-00012820: 6620 666f 726d 6174 5f66 6965 6c64 2873  f format_field(s
-00012830: 656c 662c 7661 6c75 652c 666f 726d 6174  elf,value,format
-00012840: 5f73 7065 6329 3a0a 2020 2020 2020 2020  _spec):.        
-00012850: 6966 2066 6f72 6d61 745f 7370 6563 5b2d  if format_spec[-
-00012860: 315d 3d3d 276d 273a 0a20 2020 2020 2020  1]=='m':.       
-00012870: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
-00012880: 7228 292e 666f 726d 6174 5f66 6965 6c64  r().format_field
-00012890: 2876 616c 7565 2c66 6f72 6d61 745f 7370  (value,format_sp
-000128a0: 6563 5b3a 2d31 5d2b 2765 2729 2e72 6570  ec[:-1]+'e').rep
-000128b0: 6c61 6365 2827 652b 272c 2765 2729 0a20  lace('e+','e'). 
-000128c0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000128d0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000128e0: 7375 7065 7228 292e 666f 726d 6174 5f66  super().format_f
-000128f0: 6965 6c64 2876 616c 7565 2c66 6f72 6d61  ield(value,forma
-00012900: 745f 7370 6563 290a 0a0a 666d 743d 4d79  t_spec)...fmt=My
-00012910: 466f 726d 6174 7465 7228 290a 0a0a 6465  Formatter()...de
-00012920: 6620 6c69 6e65 5f66 6c75 7828 6c31 2c6c  f line_flux(l1,l
-00012930: 322c 7761 7665 6c65 6e67 7468 2c66 6c75  2,wavelength,flu
-00012940: 7829 3a0a 2020 2020 2727 270a 2020 2020  x):.    '''.    
-00012950: 556e 6974 733a 2052 6574 7572 6e20 6973  Units: Return is
-00012960: 2069 6e20 7468 6520 7361 6d65 2075 6e69   in the same uni
-00012970: 7420 6173 2069 6e70 7574 2e20 5b41 7373  t as input. [Ass
-00012980: 756d 6564 2074 6f20 6265 2069 6e20 6572  umed to be in er
-00012990: 672f 732f 636d 322f 7372 5d20 6c31 2061  g/s/cm2/sr] l1 a
-000129a0: 6e64 206c 3220 7361 6d65 2075 6e69 7420  nd l2 same unit 
-000129b0: 6173 2077 6176 656c 656e 6774 680a 0a20  as wavelength.. 
-000129c0: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
-000129d0: 2d2d 2d2d 2d2d 0a20 2020 2066 6c6f 6174  ------.    float
-000129e0: 3a0a 2020 2020 2020 5375 6d20 6f66 2069  :.      Sum of i
-000129f0: 6e74 6567 7261 7465 6420 6c69 6e65 2066  ntegrated line f
-00012a00: 6c75 7820 6265 7477 6565 6e20 7761 7665  lux between wave
-00012a10: 6c65 6e67 7468 7320 6c31 2061 6e64 206c  lengths l1 and l
-00012a20: 322e 0a0a 2020 2020 2727 270a 2020 2020  2...    '''.    
-00012a30: 6d61 736b 3d28 7761 7665 6c65 6e67 7468  mask=(wavelength
-00012a40: 3e6c 3129 2628 7761 7665 6c65 6e67 7468  >l1)&(wavelength
-00012a50: 3c3d 6c32 290a 2020 2020 7265 7475 726e  <=l2).    return
-00012a60: 206e 702e 7375 6d28 666c 7578 5b6d 6173   np.sum(flux[mas
-00012a70: 6b5d 290a 0a0a 6465 6620 6c69 6e65 5f66  k])...def line_f
-00012a80: 6c75 7865 7328 7769 6e64 6f77 732c 7761  luxes(windows,wa
-00012a90: 7665 6c65 6e67 7468 2c66 6c75 7829 3a0a  velength,flux):.
-00012aa0: 2020 2020 2727 270a 2020 2020 5265 7475      '''.    Retu
-00012ab0: 726e 3a20 6172 7261 7920 6f66 2073 756d  rn: array of sum
-00012ac0: 206f 6620 696e 7465 6772 6174 6564 206c   of integrated l
-00012ad0: 696e 6520 666c 7578 2069 6e20 7761 7665  ine flux in wave
-00012ae0: 6c65 6e67 7468 2077 696e 646f 7773 2e0a  length windows..
-00012af0: 0a20 2020 2055 6e69 7473 3a20 5265 7475  .    Units: Retu
-00012b00: 726e 2069 7320 696e 2074 6865 2073 616d  rn is in the sam
-00012b10: 6520 756e 6974 2061 7320 696e 7075 742e  e unit as input.
-00012b20: 205b 4173 7375 6d65 6420 746f 2062 6520   [Assumed to be 
-00012b30: 696e 2065 7267 2f73 2f63 6d32 2f73 725d  in erg/s/cm2/sr]
-00012b40: 0a0a 2020 2020 7769 6e64 6f77 733a 206c  ..    windows: l
-00012b50: 6973 7420 6f66 2077 6176 656c 656e 6774  ist of wavelengt
-00012b60: 6820 6c69 6d69 7473 206f 6620 7769 6e64  h limits of wind
-00012b70: 6f77 732e 2045 7861 6d70 6c65 3a20 5b5b  ows. Example: [[
-00012b80: 3134 2c31 342e 355d 2c5b 3135 2c31 362e  14,14.5],[15,16.
-00012b90: 325d 2c5b 3132 2e35 2c31 342e 315d 5d0a  2],[12.5,14.1]].
-00012ba0: 2020 2020 2727 270a 2020 2020 463d 5b5d      '''.    F=[]
-00012bb0: 0a20 2020 2066 6f72 2057 2069 6e20 7769  .    for W in wi
-00012bc0: 6e64 6f77 733a 0a20 2020 2020 2020 2046  ndows:.        F
-00012bd0: 2e61 7070 656e 6428 6c69 6e65 5f66 6c75  .append(line_flu
-00012be0: 7828 575b 305d 2c57 5b31 5d2c 7761 7665  x(W[0],W[1],wave
-00012bf0: 6c65 6e67 7468 2c66 6c75 7829 290a 2020  length,flux)).  
-00012c00: 2020 7265 7475 726e 286e 702e 6172 7261    return(np.arra
-00012c10: 7928 4629 290a 0a0a 6465 6620 6c69 6e65  y(F))...def line
-00012c20: 5f66 6c75 785f 7261 7469 6f73 2872 6174  _flux_ratios(rat
-00012c30: 696f 5f77 696e 646f 7773 2c77 6176 656c  io_windows,wavel
-00012c40: 656e 6774 682c 666c 7578 293a 0a20 2020  ength,flux):.   
-00012c50: 2027 2727 0a20 2020 2052 6574 7572 6e3a   '''.    Return:
-00012c60: 2049 6e74 6567 7261 7465 6420 6c69 6e65   Integrated line
-00012c70: 2066 6c75 7820 7261 7469 6f73 2062 6574   flux ratios bet
-00012c80: 7765 656e 2077 6176 656c 656e 6774 6873  ween wavelengths
-00012c90: 206c 3120 616e 6420 6c32 2e0a 0a20 2020   l1 and l2...   
-00012ca0: 2055 6e69 743a 2052 6574 7572 6e20 6861   Unit: Return ha
-00012cb0: 7320 6e6f 2075 6e69 742e 205b 496e 7075  s no unit. [Inpu
-00012cc0: 7420 6973 2061 7373 756d 6564 2074 6f20  t is assumed to 
-00012cd0: 6265 2069 6e20 6572 672f 732f 636d 322f  be in erg/s/cm2/
-00012ce0: 7372 5d0a 0a20 2020 2072 6174 696f 5f77  sr]..    ratio_w
-00012cf0: 696e 646f 7773 3a20 6c69 7374 206f 6620  indows: list of 
-00012d00: 7761 7665 6c65 6e67 7468 2077 696e 646f  wavelength windo
-00012d10: 7773 2e20 4578 616d 706c 653a 205b 5b5b  ws. Example: [[[
-00012d20: 3134 2c31 342e 355d 2c5b 3135 2c31 362e  14,14.5],[15,16.
-00012d30: 325d 5d2c 5b5b 3132 2e35 2c31 342e 315d  2]],[[12.5,14.1]
-00012d40: 2c5b 3133 2e34 2c31 332e 385d 5d5d 0a20  ,[13.4,13.8]]]. 
-00012d50: 2020 2027 2727 0a20 2020 2052 3d5b 5d0a     '''.    R=[].
-00012d60: 2020 2020 666f 7220 7769 6e64 6f77 2069      for window i
-00012d70: 6e20 7261 7469 6f5f 7769 6e64 6f77 733a  n ratio_windows:
-00012d80: 0a20 2020 2020 2020 2046 3d6c 696e 655f  .        F=line_
-00012d90: 666c 7578 6573 285b 7769 6e64 6f77 5b30  fluxes([window[0
-00012da0: 5d2c 7769 6e64 6f77 5b31 5d5d 2c77 6176  ],window[1]],wav
-00012db0: 656c 656e 6774 682c 666c 7578 290a 2020  elength,flux).  
-00012dc0: 2020 2020 2020 522e 6170 7065 6e64 2846        R.append(F
-00012dd0: 5b31 5d2f 465b 305d 290a 2020 2020 7265  [1]/F[0]).    re
-00012de0: 7475 726e 286e 702e 6172 7261 7928 5229  turn(np.array(R)
-00012df0: 290a 0a0a 6465 6620 6c69 6e65 5f66 6c75  )...def line_flu
-00012e00: 785f 7072 6f64 7563 7473 2870 726f 6475  x_products(produ
-00012e10: 6374 5f77 696e 646f 7773 2c77 6176 656c  ct_windows,wavel
-00012e20: 656e 6774 682c 666c 7578 293a 0a20 2020  ength,flux):.   
-00012e30: 2027 2727 0a20 2020 2052 6574 7572 6e3a   '''.    Return:
-00012e40: 2049 6e74 6567 7261 7465 6420 6c69 6e65   Integrated line
-00012e50: 2066 6c75 7820 7072 6f64 7563 7473 2062   flux products b
-00012e60: 6574 7765 656e 2077 6176 656c 656e 6774  etween wavelengt
-00012e70: 6873 206c 3120 616e 6420 6c32 2e0a 0a20  hs l1 and l2... 
-00012e80: 2020 2055 6e69 743a 2052 6574 7572 6e20     Unit: Return 
-00012e90: 756e 6974 2069 7320 6f75 7470 7574 2075  unit is output u
-00012ea0: 6e69 7473 2073 7175 6172 6564 2e20 5b49  nits squared. [I
-00012eb0: 6e70 7574 2069 7320 6173 7375 6d65 6420  nput is assumed 
-00012ec0: 746f 2062 6520 696e 2065 7267 2f73 2f63  to be in erg/s/c
-00012ed0: 6d32 2f73 725d 0a0a 2020 2020 7072 6f64  m2/sr]..    prod
-00012ee0: 7563 745f 7769 6e64 6f77 733a 206c 6973  uct_windows: lis
-00012ef0: 7420 6f66 2077 6176 656c 656e 6774 6820  t of wavelength 
-00012f00: 7769 6e64 6f77 732e 2045 7861 6d70 6c65  windows. Example
-00012f10: 3a20 5b5b 5b31 342c 3134 2e35 5d2c 5b31  : [[[14,14.5],[1
-00012f20: 352c 3136 2e32 5d5d 2c5b 5b31 322e 352c  5,16.2]],[[12.5,
-00012f30: 3134 2e31 5d2c 5b31 332e 342c 3133 2e38  14.1],[13.4,13.8
-00012f40: 5d5d 5d0a 2020 2020 2727 270a 2020 2020  ]]].    '''.    
-00012f50: 523d 5b5d 0a20 2020 2066 6f72 2077 696e  R=[].    for win
-00012f60: 646f 7720 696e 2070 726f 6475 6374 5f77  dow in product_w
-00012f70: 696e 646f 7773 3a0a 2020 2020 2020 2020  indows:.        
-00012f80: 463d 6c69 6e65 5f66 6c75 7865 7328 5b77  F=line_fluxes([w
-00012f90: 696e 646f 775b 305d 2c77 696e 646f 775b  indow[0],window[
-00012fa0: 315d 5d2c 7761 7665 6c65 6e67 7468 2c66  1]],wavelength,f
-00012fb0: 6c75 7829 0a20 2020 2020 2020 2052 2e61  lux).        R.a
-00012fc0: 7070 656e 6428 465b 315d 2a46 5b30 5d29  ppend(F[1]*F[0])
-00012fd0: 0a20 2020 2072 6574 7572 6e28 6e70 2e61  .    return(np.a
-00012fe0: 7272 6179 2852 2929 0a0a 0a64 6566 2073  rray(R))...def s
-00012ff0: 7065 6374 7261 6c5f 666c 7578 286c 312c  pectral_flux(l1,
-00013000: 6c32 2c77 6176 656c 656e 6774 682c 666c  l2,wavelength,fl
-00013010: 7578 293a 0a20 2020 2027 2727 0a20 2020  ux):.    '''.   
-00013020: 2055 6e69 743a 2052 6574 7572 6e20 696e   Unit: Return in
-00013030: 205b 6572 672f 732f 636d 325d 2061 6e64   [erg/s/cm2] and
-00013040: 2069 6e70 7574 2069 7320 696e 205b 4a79   input is in [Jy
-00013050: 5d20 6c31 2c20 6c32 2c20 616e 6420 7761  ] l1, l2, and wa
-00013060: 7665 6c65 6e67 7468 2069 6e20 6d69 6372  velength in micr
-00013070: 6f6e 730a 0a20 2020 2052 6574 7572 6e73  ons..    Returns
-00013080: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
-00013090: 2066 6c6f 6174 3a0a 2020 2020 2020 5375   float:.      Su
-000130a0: 6d20 6f66 2069 6e74 6567 7261 7465 6420  m of integrated 
-000130b0: 6c69 6e65 2066 6c75 7820 6265 7477 6565  line flux betwee
-000130c0: 6e20 7761 7665 6c65 6e67 7468 7320 6c31  n wavelengths l1
-000130d0: 2061 6e64 206c 322e 0a0a 2020 2020 2727   and l2...    ''
-000130e0: 270a 2020 2020 666c 7578 3d66 6c75 782a  '.    flux=flux*
-000130f0: 3165 2d32 3320 2023 2043 6f6e 7665 7274  1e-23  # Convert
-00013100: 696e 6720 4a79 2074 6f20 6572 672e 73e2  ing Jy to erg.s.
-00013110: 8892 312e 636d e288 9232 2e48 7ae2 8892  ..1.cm...2.Hz...
-00013120: 310a 2020 2020 7761 7665 6c65 6e67 7468  1.    wavelength
-00013130: 3d77 6176 656c 656e 6774 682a 3165 2d34  =wavelength*1e-4
-00013140: 2020 2320 436f 6e76 6572 7469 6e67 206d    # Converting m
-00013150: 6963 726f 6e73 2074 6f20 636d 0a20 2020  icrons to cm.   
-00013160: 2066 6c75 783d 666c 7578 5b6e 702e 6172   flux=flux[np.ar
-00013170: 6773 6f72 7428 7761 7665 6c65 6e67 7468  gsort(wavelength
-00013180: 295d 0a20 2020 2077 6176 656c 656e 6774  )].    wavelengt
-00013190: 683d 7761 7665 6c65 6e67 7468 5b6e 702e  h=wavelength[np.
-000131a0: 6172 6773 6f72 7428 7761 7665 6c65 6e67  argsort(waveleng
-000131b0: 7468 295d 0a20 2020 206c 313d 6c31 2a31  th)].    l1=l1*1
-000131c0: 652d 3420 2023 2043 6f6e 7665 7274 696e  e-4  # Convertin
-000131d0: 6720 6d69 6372 6f6e 7320 746f 2063 6d0a  g microns to cm.
-000131e0: 2020 2020 6c32 3d6c 322a 3165 2d34 2020      l2=l2*1e-4  
-000131f0: 2320 436f 6e76 6572 7469 6e67 206d 6963  # Converting mic
-00013200: 726f 6e73 2074 6f20 636d 0a20 2020 2063  rons to cm.    c
-00013210: 5f63 6d73 3d63 2a31 6532 2020 2320 436f  _cms=c*1e2  # Co
-00013220: 6e76 6572 7469 6e67 206d 2f73 2074 6f20  nverting m/s to 
-00013230: 636d 2f73 0a20 2020 206d 6173 6b3d 2877  cm/s.    mask=(w
-00013240: 6176 656c 656e 6774 683e 6c31 2926 2877  avelength>l1)&(w
-00013250: 6176 656c 656e 6774 683c 3d6c 3229 0a20  avelength<=l2). 
-00013260: 2020 2077 6176 653d 7761 7665 6c65 6e67     wave=waveleng
-00013270: 7468 5b6d 6173 6b5d 0a20 2020 2023 2077  th[mask].    # w
-00013280: 6176 6531 2020 2020 2020 3d20 6e70 2e72  ave1      = np.r
-00013290: 6f6c 6c28 7761 7665 6c65 6e67 7468 2c31  oll(wavelength,1
-000132a0: 295b 6d61 736b 5d0a 2020 2020 2320 7761  )[mask].    # wa
-000132b0: 7665 3120 2020 2020 203d 2031 302a 2a28  ve1      = 10**(
-000132c0: 286e 702e 6c6f 6731 3028 7761 7665 292b  (np.log10(wave)+
-000132d0: 6e70 2e6c 6f67 3130 2877 6176 6531 2929  np.log10(wave1))
-000132e0: 2f32 290a 2020 2020 2320 7761 7665 3220  /2).    # wave2 
-000132f0: 2020 2020 203d 206e 702e 726f 6c6c 2877       = np.roll(w
-00013300: 6176 656c 656e 6774 682c 2d31 295b 6d61  avelength,-1)[ma
-00013310: 736b 5d0a 2020 2020 2320 7761 7665 3220  sk].    # wave2 
-00013320: 2020 2020 203d 2031 302a 2a28 286e 702e       = 10**((np.
-00013330: 6c6f 6731 3028 7761 7665 292b 6e70 2e6c  log10(wave)+np.l
-00013340: 6f67 3130 2877 6176 6532 2929 2f32 290a  og10(wave2))/2).
-00013350: 2020 2020 2320 646e 7520 2020 2020 2020      # dnu       
-00013360: 203d 2063 2a28 7761 7665 322d 7761 7665   = c*(wave2-wave
-00013370: 3129 2f77 6176 652a 2a32 2a31 6532 0a20  1)/wave**2*1e2. 
-00013380: 2020 2077 6176 6531 3d6e 702e 726f 6c6c     wave1=np.roll
-00013390: 2877 6176 656c 656e 6774 682c 3129 5b6d  (wavelength,1)[m
-000133a0: 6173 6b5d 0a20 2020 2077 6176 6532 3d6e  ask].    wave2=n
-000133b0: 702e 726f 6c6c 2877 6176 656c 656e 6774  p.roll(wavelengt
-000133c0: 682c 2d31 295b 6d61 736b 5d0a 2020 2020  h,-1)[mask].    
-000133d0: 646e 753d 2863 5f63 6d73 2a28 312f 7761  dnu=(c_cms*(1/wa
-000133e0: 7665 312d 312f 7761 7665 3229 2f32 290a  ve1-1/wave2)/2).
-000133f0: 2020 2020 7265 7475 726e 286e 702e 7375      return(np.su
-00013400: 6d28 666c 7578 5b6d 6173 6b5d 2a64 6e75  m(flux[mask]*dnu
-00013410: 2929 0a0a 0a64 6566 2073 7065 6374 7261  ))...def spectra
-00013420: 6c5f 666c 7578 6573 2877 696e 646f 7773  l_fluxes(windows
-00013430: 2c77 6176 656c 656e 6774 682c 666c 7578  ,wavelength,flux
-00013440: 293a 0a20 2020 2027 2727 0a20 2020 2052  ):.    '''.    R
-00013450: 6574 7572 6e3a 2053 756d 206f 6620 696e  eturn: Sum of in
-00013460: 7465 6772 6174 6564 206c 696e 6520 666c  tegrated line fl
-00013470: 7578 2062 6574 7765 656e 2077 6176 656c  ux between wavel
-00013480: 656e 6774 6820 7769 6e64 6f77 732e 0a0a  ength windows...
-00013490: 2020 2020 556e 6974 3a20 7265 7475 726e      Unit: return
-000134a0: 2069 7320 696e 205b 6572 672f 732f 636d   is in [erg/s/cm
-000134b0: 325d 2061 6e64 2069 6e70 7574 2069 7320  2] and input is 
-000134c0: 696e 205b 4a79 5d0a 0a20 2020 2077 696e  in [Jy]..    win
-000134d0: 646f 7773 3a20 6c69 7374 206f 6620 7761  dows: list of wa
-000134e0: 7665 6c65 6e67 7468 206c 696d 6974 7320  velength limits 
-000134f0: 286d 6963 726f 6e73 2920 6f66 2077 696e  (microns) of win
-00013500: 646f 7773 2e20 4578 616d 706c 653a 205b  dows. Example: [
-00013510: 5b31 342c 3134 2e35 5d2c 5b31 352c 3136  [14,14.5],[15,16
-00013520: 2e32 5d2c 5b31 322e 352c 3134 2e31 5d5d  .2],[12.5,14.1]]
-00013530: 0a20 2020 2027 2727 0a20 2020 2046 3d5b  .    '''.    F=[
-00013540: 5d0a 2020 2020 666f 7220 5720 696e 2077  ].    for W in w
-00013550: 696e 646f 7773 3a0a 2020 2020 2020 2020  indows:.        
-00013560: 462e 6170 7065 6e64 2873 7065 6374 7261  F.append(spectra
-00013570: 6c5f 666c 7578 2857 5b30 5d2c 575b 315d  l_flux(W[0],W[1]
-00013580: 2c77 6176 656c 656e 6774 682c 666c 7578  ,wavelength,flux
-00013590: 2929 0a20 2020 2072 6574 7572 6e28 6e70  )).    return(np
-000135a0: 2e61 7272 6179 2846 2929 0a0a 0a64 6566  .array(F))...def
-000135b0: 2073 7065 6374 7261 6c5f 666c 7578 5f72   spectral_flux_r
-000135c0: 6174 696f 7328 7261 7469 6f5f 7769 6e64  atios(ratio_wind
-000135d0: 6f77 732c 7761 7665 6c65 6e67 7468 2c66  ows,wavelength,f
-000135e0: 6c75 7829 3a0a 2020 2020 2727 270a 2020  lux):.    '''.  
-000135f0: 2020 5265 7475 726e 3a20 5370 6563 7472    Return: Spectr
-00013600: 616c 2069 6e74 6567 7261 7465 6420 666c  al integrated fl
-00013610: 7578 2072 6174 696f 7320 6265 7477 6565  ux ratios betwee
-00013620: 6e20 7761 7665 6c65 6e67 7468 2077 696e  n wavelength win
-00013630: 646f 7773 2e0a 0a20 2020 2055 6e69 7473  dows...    Units
-00013640: 3a20 5265 7475 726e 2069 7320 7769 7468  : Return is with
-00013650: 6f75 7420 756e 6974 7320 616e 6420 696e  out units and in
-00013660: 7075 7420 6973 2069 6e20 5b4a 795d 0a0a  put is in [Jy]..
-00013670: 2020 2020 7261 7469 6f5f 7769 6e64 6f77      ratio_window
-00013680: 733a 206c 6973 7420 6f66 2077 6176 656c  s: list of wavel
-00013690: 656e 6774 6820 286d 6963 726f 6e73 2920  ength (microns) 
-000136a0: 7769 6e64 6f77 732e 2045 7861 6d70 6c65  windows. Example
-000136b0: 3a20 5b5b 5b31 342c 3134 2e35 5d2c 5b31  : [[[14,14.5],[1
-000136c0: 352c 3136 2e32 5d5d 2c5b 5b31 322e 352c  5,16.2]],[[12.5,
-000136d0: 3134 2e31 5d2c 5b31 332e 342c 3133 2e38  14.1],[13.4,13.8
-000136e0: 5d5d 5d0a 2020 2020 2727 270a 2020 2020  ]]].    '''.    
-000136f0: 523d 5b5d 0a20 2020 2066 6f72 2077 696e  R=[].    for win
-00013700: 646f 7720 696e 2072 6174 696f 5f77 696e  dow in ratio_win
-00013710: 646f 7773 3a0a 2020 2020 2020 2020 463d  dows:.        F=
-00013720: 7370 6563 7472 616c 5f66 6c75 7865 7328  spectral_fluxes(
-00013730: 5b77 696e 646f 775b 305d 2c77 696e 646f  [window[0],windo
-00013740: 775b 315d 5d2c 7761 7665 6c65 6e67 7468  w[1]],wavelength
-00013750: 2c66 6c75 7829 0a20 2020 2020 2020 2052  ,flux).        R
-00013760: 2e61 7070 656e 6428 465b 315d 2f46 5b30  .append(F[1]/F[0
-00013770: 5d29 0a20 2020 2072 6574 7572 6e28 6e70  ]).    return(np
-00013780: 2e61 7272 6179 2852 2929 0a0a 0a64 6566  .array(R))...def
-00013790: 2073 7065 6374 7261 6c5f 666c 7578 5f70   spectral_flux_p
-000137a0: 726f 6475 6374 7328 7072 6f64 7563 745f  roducts(product_
-000137b0: 7769 6e64 6f77 732c 7761 7665 6c65 6e67  windows,waveleng
-000137c0: 7468 2c66 6c75 7829 3a0a 2020 2020 2727  th,flux):.    ''
-000137d0: 270a 2020 2020 5265 7475 726e 3a20 5072  '.    Return: Pr
-000137e0: 6f64 7563 7473 206f 6620 7370 6563 7472  oducts of spectr
-000137f0: 616c 2069 6e74 6567 7261 7465 6420 666c  al integrated fl
-00013800: 7578 6573 2062 6574 7765 656e 2077 6176  uxes between wav
-00013810: 656c 656e 6774 6820 7769 6e64 6f77 732e  elength windows.
-00013820: 0a0a 2020 2020 556e 6974 733a 2052 6574  ..    Units: Ret
-00013830: 7572 6e20 756e 6974 2069 7320 6f75 7470  urn unit is outp
-00013840: 7574 2075 6e69 7473 2073 7175 6172 6564  ut units squared
-00013850: 2061 6e64 2069 6e70 7574 2069 7320 696e   and input is in
-00013860: 205b 4a79 5d0a 0a20 2020 2070 726f 6475   [Jy]..    produ
-00013870: 6374 5f77 696e 646f 7773 3a20 6c69 7374  ct_windows: list
-00013880: 206f 6620 7761 7665 6c65 6e67 7468 2028   of wavelength (
-00013890: 6d69 6372 6f6e 7329 2077 696e 646f 7773  microns) windows
-000138a0: 2e20 4578 616d 706c 653a 205b 5b5b 3134  . Example: [[[14
-000138b0: 2c31 342e 355d 2c5b 3135 2c31 362e 325d  ,14.5],[15,16.2]
-000138c0: 5d2c 5b5b 3132 2e35 2c31 342e 315d 2c5b  ],[[12.5,14.1],[
-000138d0: 3133 2e34 2c31 332e 385d 5d5d 0a20 2020  13.4,13.8]]].   
-000138e0: 2027 2727 0a20 2020 2052 3d5b 5d0a 2020   '''.    R=[].  
-000138f0: 2020 666f 7220 7769 6e64 6f77 2069 6e20    for window in 
-00013900: 7072 6f64 7563 745f 7769 6e64 6f77 733a  product_windows:
-00013910: 0a20 2020 2020 2020 2046 3d73 7065 6374  .        F=spect
-00013920: 7261 6c5f 666c 7578 6573 285b 7769 6e64  ral_fluxes([wind
-00013930: 6f77 5b30 5d2c 7769 6e64 6f77 5b31 5d5d  ow[0],window[1]]
-00013940: 2c77 6176 656c 656e 6774 682c 666c 7578  ,wavelength,flux
-00013950: 290a 2020 2020 2020 2020 522e 6170 7065  ).        R.appe
-00013960: 6e64 2846 5b31 5d2a 465b 305d 290a 2020  nd(F[1]*F[0]).  
-00013970: 2020 7265 7475 726e 286e 702e 6172 7261    return(np.arra
-00013980: 7928 5229 290a 0a0a 6465 6620 6368 6932  y(R))...def chi2
-00013990: 5f73 6c61 6228 736c 6162 5f64 6174 612c  _slab(slab_data,
-000139a0: 7370 6563 7472 612c 7769 6e64 6f77 733d  spectra,windows=
-000139b0: 5b5d 2c72 6174 696f 5f77 696e 646f 7773  [],ratio_windows
-000139c0: 3d5b 5d2c 7072 6f64 7563 745f 7769 6e64  =[],product_wind
-000139d0: 6f77 733d 5b5d 2c52 6469 736b 3d6e 702e  ows=[],Rdisk=np.
-000139e0: 6c6f 6773 7061 6365 282d 322c 322c 3130  logspace(-2,2,10
-000139f0: 292c 6469 7374 616e 6365 3d31 3230 2c63  ),distance=120,c
-00013a00: 6f6e 766f 6c76 653d 4661 6c73 652c 4e4c  onvolve=False,NL
-00013a10: 5445 3d46 616c 7365 2c73 686f 7274 5f66  TE=False,short_f
-00013a20: 6f72 6d61 743d 4661 6c73 6529 3a0a 2020  ormat=False):.  
-00013a30: 2020 2727 270a 2020 2020 5265 7475 726e    '''.    Return
-00013a40: 7320 6368 6932 2062 6173 6564 206f 6e20  s chi2 based on 
-00013a50: 7365 6c65 6374 6564 2073 7065 6374 7261  selected spectra
-00013a60: 6c20 7769 6e64 6f77 7320 6163 726f 7373  l windows across
-00013a70: 2064 6966 6665 7265 6e74 2065 6d69 7474   different emitt
-00013a80: 696e 6720 6469 736b 2072 6164 6975 730a  ing disk radius.
-00013a90: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
-00013aa0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00013ab0: 2020 2073 6c61 625f 6461 7461 203a 2073     slab_data : s
-00013ac0: 7472 696e 6720 6f72 2073 6c61 625f 6d6f  tring or slab_mo
-00013ad0: 6465 6c20 696e 7374 616e 6365 0a20 2020  del instance.   
-00013ae0: 2020 2070 6174 6820 636f 7272 6573 706f     path correspo
-00013af0: 6e64 696e 6720 746f 2061 2073 696e 676c  nding to a singl
-00013b00: 6520 736c 6162 206d 6f64 656c 206f 7220  e slab model or 
-00013b10: 6120 7369 6e67 6c65 2073 6c61 625f 6d6f  a single slab_mo
-00013b20: 6465 6c20 696e 7374 616e 6365 0a0a 2020  del instance..  
-00013b30: 2020 7370 6563 7472 6120 3a20 6e75 6d70    spectra : nump
-00013b40: 792e 6172 7261 790a 2020 2020 2020 6e75  y.array.      nu
-00013b50: 6d70 7920 6172 7261 7920 7769 7468 2066  mpy array with f
-00013b60: 6972 7374 2063 6f6c 756d 6e20 7468 6520  irst column the 
-00013b70: 7761 7665 6c65 6e67 7468 2069 6e20 5b6d  wavelength in [m
-00013b80: 6963 726f 6e73 5d20 616e 6420 7365 636f  icrons] and seco
-00013b90: 6e64 2063 6f6c 756d 6e20 666c 7578 2069  nd column flux i
-00013ba0: 6e20 5b4a 795d 0a0a 2020 2020 7769 6e64  n [Jy]..    wind
-00013bb0: 6f77 7320 3a20 6172 7261 795f 6c69 6b65  ows : array_like
-00013bc0: 0a20 2020 2020 204c 6973 7420 6f66 2073  .      List of s
-00013bd0: 7065 6374 7261 6c20 7769 6e64 6f77 7320  pectral windows 
-00013be0: 666f 7220 6368 6932 2063 616c 6375 6c61  for chi2 calcula
-00013bf0: 7469 6f6e 2028 7765 6967 6874 7320 6f70  tion (weights op
-00013c00: 7469 6f6e 616c 292e 2046 6f72 6d61 7420  tional). Format 
-00013c10: 3a20 5b77 696e 646f 7731 2c77 696e 646f  : [window1,windo
-00013c20: 7732 2c2e 2e2e 2e5d 0a20 2020 2020 2057  w2,....].      W
-00013c30: 696e 646f 7720 666f 726d 6174 3a20 5b6c  indow format: [l
-00013c40: 616d 6264 615f 302c 206c 616d 6264 615f  ambda_0, lambda_
-00013c50: 312c 2077 6569 6768 745d 2077 6569 6768  1, weight] weigh
-00013c60: 7420 6973 206f 7074 696f 6e61 6c2c 2075  t is optional, u
-00013c70: 7365 6420 666f 7220 7765 6967 6874 6564  sed for weighted
-00013c80: 2063 6869 320a 2020 2020 2020 4578 616d   chi2.      Exam
-00013c90: 706c 6520 7769 7468 6f75 7420 7765 6967  ple without weig
-00013ca0: 6874 3a20 5b5b 3134 2c31 342e 355d 2c5b  ht: [[14,14.5],[
-00013cb0: 3135 2c31 362e 325d 2c5b 3132 2e35 2c31  15,16.2],[12.5,1
-00013cc0: 342e 315d 5d0a 2020 2020 2020 4578 616d  4.1]].      Exam
-00013cd0: 706c 6520 7769 7468 2077 6569 6768 743a  ple with weight:
-00013ce0: 205b 5b31 342c 3134 2e35 2c32 5d2c 5b31   [[14,14.5,2],[1
-00013cf0: 352c 3136 2e32 2c35 5d2c 5b31 322e 352c  5,16.2,5],[12.5,
-00013d00: 3134 2e31 2c31 5d5d 0a20 2020 2020 2057  14.1,1]].      W
-00013d10: 6569 6768 7473 2061 7265 2061 7574 6f6d  eights are autom
-00013d20: 6174 6963 616c 6c79 206e 6f72 6d61 6c69  atically normali
-00013d30: 7365 642c 2073 6f20 7375 6d20 6f66 2077  sed, so sum of w
-00013d40: 6569 6768 7473 206e 6565 6420 6e6f 7420  eights need not 
-00013d50: 6265 2031 0a0a 2020 2020 5264 6973 6b20  be 1..    Rdisk 
-00013d60: 3a20 6172 7261 795f 6c69 6b65 0a20 2020  : array_like.   
-00013d70: 2020 2052 6164 6975 7320 636f 7272 6573     Radius corres
-00013d80: 706f 6e64 696e 6720 746f 2065 6d69 7474  ponding to emitt
-00013d90: 696e 6720 6172 6561 2069 6e20 6173 7472  ing area in astr
-00013da0: 6f6e 6f6d 6963 616c 2075 6e69 7473 0a0a  onomical units..
-00013db0: 2020 2020 6469 7374 616e 6365 203a 2066      distance : f
-00013dc0: 6c6f 6174 0a20 2020 2020 2064 6973 7461  loat.      dista
-00013dd0: 6e63 6520 6f66 2064 6973 6b20 696e 2070  nce of disk in p
-00013de0: 6172 7365 630a 0a20 2020 2063 6f6e 766f  arsec..    convo
-00013df0: 6c76 6520 3a20 626f 6f6c 6561 6e0a 2020  lve : boolean.  
-00013e00: 2020 2020 4966 2054 7275 652c 2074 6865      If True, the
-00013e10: 2063 6869 3220 6973 2070 6572 666f 726d   chi2 is perform
-00013e20: 6564 206f 6e20 636f 6e76 6f6c 7665 6420  ed on convolved 
-00013e30: 7370 6563 7472 6120 616e 6420 6e6f 7420  spectra and not 
-00013e40: 6f6e 2069 6e64 6976 6964 7561 6c20 6c69  on individual li
-00013e50: 6e65 730a 0a20 2020 204e 4c54 4520 3a20  nes..    NLTE : 
-00013e60: 626f 6f6c 6561 6e0a 2020 2020 2020 6966  boolean.      if
-00013e70: 2054 7275 652c 204e 4c54 4520 666c 7578   True, NLTE flux
-00013e80: 2069 7320 7461 6b65 6e20 6672 6f6d 2074   is taken from t
-00013e90: 6865 2073 6c61 6220 6d6f 6465 6c2e 0a20  he slab model.. 
-00013ea0: 2020 2027 2727 0a20 2020 2061 7265 613d     '''.    area=
-00013eb0: 6e70 2e70 692a 2852 6469 736b 2a61 752f  np.pi*(Rdisk*au/
-00013ec0: 6469 7374 616e 6365 2f70 6329 2a2a 320a  distance/pc)**2.
-00013ed0: 2020 2020 6368 695f 6172 6561 3d6e 702e      chi_area=np.
-00013ee0: 7a65 726f 7328 286c 656e 2861 7265 6129  zeros((len(area)
-00013ef0: 2929 0a20 2020 2069 6620 6973 696e 7374  )).    if isinst
-00013f00: 616e 6365 2873 6c61 625f 6461 7461 2c73  ance(slab_data,s
-00013f10: 7472 293a 2073 6c61 625f 6461 7461 3d72  tr): slab_data=r
-00013f20: 6561 645f 736c 6162 2873 6c61 625f 6461  ead_slab(slab_da
-00013f30: 7461 2c76 6572 626f 7365 3d46 616c 7365  ta,verbose=False
-00013f40: 2c73 686f 7274 5f66 6f72 6d61 743d 7368  ,short_format=sh
-00013f50: 6f72 745f 666f 726d 6174 290a 2020 2020  ort_format).    
-00013f60: 6966 206c 656e 2877 696e 646f 7773 293c  if len(windows)<
-00013f70: 3020 616e 6420 6c65 6e28 7261 7469 6f5f  0 and len(ratio_
-00013f80: 7769 6e64 6f77 7329 3c30 2061 6e64 206c  windows)<0 and l
-00013f90: 656e 2870 726f 6475 6374 5f77 696e 646f  en(product_windo
-00013fa0: 7773 293c 303a 2072 6574 7572 6e20 6368  ws)<0: return ch
-00013fb0: 695f 6172 6561 0a20 2020 2069 6620 636f  i_area.    if co
-00013fc0: 6e76 6f6c 7665 3a20 2023 2074 6f20 6573  nvolve:  # to es
-00013fd0: 7469 6d61 7465 2066 6c75 7820 6672 6f6d  timate flux from
-00013fe0: 2063 6f6e 766f 6c76 6564 2073 7065 6374   convolved spect
-00013ff0: 7261 0a20 2020 2020 2020 206c 6d69 6e2c  ra.        lmin,
-00014000: 6c6d 6178 3d5b 5d2c 5b5d 0a20 2020 2020  lmax=[],[].     
-00014010: 2020 2069 6620 6c65 6e28 7769 6e64 6f77     if len(window
-00014020: 7329 3e30 3a0a 2020 2020 2020 2020 2020  s)>0:.          
-00014030: 2020 6c6d 696e 2e61 7070 656e 6428 6e70    lmin.append(np
-00014040: 2e61 6d69 6e28 6e70 2e61 7272 6179 285b  .amin(np.array([
-00014050: 5b69 5b30 5d2c 695b 315d 5d20 666f 7220  [i[0],i[1]] for 
-00014060: 6920 696e 2077 696e 646f 7773 5d29 2e66  i in windows]).f
-00014070: 6c61 7474 656e 2829 2929 0a20 2020 2020  latten())).     
-00014080: 2020 2020 2020 206c 6d61 782e 6170 7065         lmax.appe
-00014090: 6e64 286e 702e 616d 6178 286e 702e 6172  nd(np.amax(np.ar
-000140a0: 7261 7928 5b5b 695b 305d 2c69 5b31 5d5d  ray([[i[0],i[1]]
-000140b0: 2066 6f72 2069 2069 6e20 7769 6e64 6f77   for i in window
-000140c0: 735d 292e 666c 6174 7465 6e28 2929 290a  s]).flatten())).
-000140d0: 2020 2020 2020 2020 6966 206c 656e 2872          if len(r
-000140e0: 6174 696f 5f77 696e 646f 7773 293e 303a  atio_windows)>0:
-000140f0: 0a20 2020 2020 2020 2020 2020 206c 6d69  .            lmi
-00014100: 6e2e 6170 7065 6e64 286e 702e 616d 696e  n.append(np.amin
-00014110: 286e 702e 6172 7261 7928 5b5b 695b 305d  (np.array([[i[0]
-00014120: 2c69 5b31 5d5d 2066 6f72 2069 2069 6e20  ,i[1]] for i in 
-00014130: 7261 7469 6f5f 7769 6e64 6f77 735d 292e  ratio_windows]).
-00014140: 666c 6174 7465 6e28 2929 290a 2020 2020  flatten())).    
-00014150: 2020 2020 2020 2020 6c6d 6178 2e61 7070          lmax.app
-00014160: 656e 6428 6e70 2e61 6d61 7828 6e70 2e61  end(np.amax(np.a
-00014170: 7272 6179 285b 5b69 5b30 5d2c 695b 315d  rray([[i[0],i[1]
-00014180: 5d20 666f 7220 6920 696e 2072 6174 696f  ] for i in ratio
-00014190: 5f77 696e 646f 7773 5d29 2e66 6c61 7474  _windows]).flatt
-000141a0: 656e 2829 2929 0a20 2020 2020 2020 2069  en())).        i
-000141b0: 6620 6c65 6e28 7072 6f64 7563 745f 7769  f len(product_wi
-000141c0: 6e64 6f77 7329 3e30 3a0a 2020 2020 2020  ndows)>0:.      
-000141d0: 2020 2020 2020 6c6d 696e 2e61 7070 656e        lmin.appen
-000141e0: 6428 6e70 2e61 6d69 6e28 6e70 2e61 7272  d(np.amin(np.arr
-000141f0: 6179 285b 5b69 5b30 5d2c 695b 315d 5d20  ay([[i[0],i[1]] 
-00014200: 666f 7220 6920 696e 2070 726f 6475 6374  for i in product
-00014210: 5f77 696e 646f 7773 5d29 2e66 6c61 7474  _windows]).flatt
-00014220: 656e 2829 2929 0a20 2020 2020 2020 2020  en())).         
-00014230: 2020 206c 6d61 782e 6170 7065 6e64 286e     lmax.append(n
-00014240: 702e 616d 6178 286e 702e 6172 7261 7928  p.amax(np.array(
-00014250: 5b5b 695b 305d 2c69 5b31 5d5d 2066 6f72  [[i[0],i[1]] for
-00014260: 2069 2069 6e20 7072 6f64 7563 745f 7769   i in product_wi
-00014270: 6e64 6f77 735d 292e 666c 6174 7465 6e28  ndows]).flatten(
-00014280: 2929 290a 2020 2020 2020 2020 6c6d 696e  ))).        lmin
-00014290: 3d6e 702e 616d 696e 286c 6d69 6e29 0a20  =np.amin(lmin). 
-000142a0: 2020 2020 2020 206c 6d61 783d 6e70 2e61         lmax=np.a
-000142b0: 6d61 7828 6c6d 6178 290a 2020 2020 2020  max(lmax).      
-000142c0: 2020 736c 6162 5f64 6174 612e 636f 6e76    slab_data.conv
-000142d0: 6f6c 7665 2852 3d32 3030 302c 6c61 6d62  olve(R=2000,lamb
-000142e0: 6461 5f30 3d6c 6d69 6e2a 302e 392c 6c61  da_0=lmin*0.9,la
-000142f0: 6d62 6461 5f6e 3d6c 6d61 782a 312e 312c  mbda_n=lmax*1.1,
-00014300: 4e4c 5445 3d4e 4c54 452c 7665 7262 6f73  NLTE=NLTE,verbos
-00014310: 653d 4661 6c73 6529 0a20 2020 2020 2020  e=False).       
-00014320: 2069 6620 4e4c 5445 3a0a 2020 2020 2020   if NLTE:.      
-00014330: 2020 2020 2020 466d 6f64 656c 3d73 7065        Fmodel=spe
-00014340: 6374 7261 6c5f 666c 7578 6573 2877 696e  ctral_fluxes(win
-00014350: 646f 7773 2c73 6c61 625f 6461 7461 2e63  dows,slab_data.c
-00014360: 6f6e 7657 6176 656c 656e 6774 682c 736c  onvWavelength,sl
-00014370: 6162 5f64 6174 612e 636f 6e76 4e4c 5445  ab_data.convNLTE
-00014380: 666c 7578 2a31 6532 3329 0a20 2020 2020  flux*1e23).     
-00014390: 2020 2020 2020 2052 6d6f 6465 6c3d 7370         Rmodel=sp
-000143a0: 6563 7472 616c 5f66 6c75 785f 7261 7469  ectral_flux_rati
-000143b0: 6f73 2872 6174 696f 5f77 696e 646f 7773  os(ratio_windows
-000143c0: 2c73 6c61 625f 6461 7461 2e63 6f6e 7657  ,slab_data.convW
-000143d0: 6176 656c 656e 6774 682c 736c 6162 5f64  avelength,slab_d
-000143e0: 6174 612e 636f 6e76 4e4c 5445 666c 7578  ata.convNLTEflux
-000143f0: 2a31 6532 3329 0a20 2020 2020 2020 2020  *1e23).         
-00014400: 2020 2050 6d6f 6465 6c3d 7370 6563 7472     Pmodel=spectr
-00014410: 616c 5f66 6c75 785f 7072 6f64 7563 7473  al_flux_products
-00014420: 2870 726f 6475 6374 5f77 696e 646f 7773  (product_windows
-00014430: 2c73 6c61 625f 6461 7461 2e63 6f6e 7657  ,slab_data.convW
-00014440: 6176 656c 656e 6774 682c 736c 6162 5f64  avelength,slab_d
-00014450: 6174 612e 636f 6e76 4e4c 5445 666c 7578  ata.convNLTEflux
-00014460: 2a31 6532 3329 0a20 2020 2020 2020 2065  *1e23).        e
-00014470: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00014480: 2046 6d6f 6465 6c3d 7370 6563 7472 616c   Fmodel=spectral
-00014490: 5f66 6c75 7865 7328 7769 6e64 6f77 732c  _fluxes(windows,
-000144a0: 736c 6162 5f64 6174 612e 636f 6e76 5761  slab_data.convWa
-000144b0: 7665 6c65 6e67 7468 2c73 6c61 625f 6461  velength,slab_da
-000144c0: 7461 2e63 6f6e 764c 5445 666c 7578 2a31  ta.convLTEflux*1
-000144d0: 6532 3329 0a20 2020 2020 2020 2020 2020  e23).           
-000144e0: 2052 6d6f 6465 6c3d 7370 6563 7472 616c   Rmodel=spectral
-000144f0: 5f66 6c75 785f 7261 7469 6f73 2872 6174  _flux_ratios(rat
-00014500: 696f 5f77 696e 646f 7773 2c73 6c61 625f  io_windows,slab_
-00014510: 6461 7461 2e63 6f6e 7657 6176 656c 656e  data.convWavelen
-00014520: 6774 682c 736c 6162 5f64 6174 612e 636f  gth,slab_data.co
-00014530: 6e76 4c54 4566 6c75 782a 3165 3233 290a  nvLTEflux*1e23).
-00014540: 2020 2020 2020 2020 2020 2020 506d 6f64              Pmod
-00014550: 656c 3d73 7065 6374 7261 6c5f 666c 7578  el=spectral_flux
-00014560: 5f70 726f 6475 6374 7328 7072 6f64 7563  _products(produc
-00014570: 745f 7769 6e64 6f77 732c 736c 6162 5f64  t_windows,slab_d
-00014580: 6174 612e 636f 6e76 5761 7665 6c65 6e67  ata.convWaveleng
-00014590: 7468 2c73 6c61 625f 6461 7461 2e63 6f6e  th,slab_data.con
-000145a0: 764c 5445 666c 7578 2a31 6532 3329 0a20  vLTEflux*1e23). 
-000145b0: 2020 2065 6c73 653a 2020 2320 746f 2065     else:  # to e
-000145c0: 7374 696d 6174 6520 666c 7578 2066 726f  stimate flux fro
-000145d0: 6d20 6c69 6e65 206c 6973 740a 2020 2020  m line list.    
-000145e0: 2020 2020 6966 204e 4c54 453a 0a20 2020      if NLTE:.   
-000145f0: 2020 2020 2020 2020 2074 3d27 464e 4c54           t='FNLT
-00014600: 4527 0a20 2020 2020 2020 2065 6c73 653a  E'.        else:
-00014610: 0a20 2020 2020 2020 2020 2020 2074 3d27  .            t='
-00014620: 464c 5445 270a 2020 2020 2020 2020 6c69  FLTE'.        li
-00014630: 6e65 6461 7461 3d73 6c61 625f 6461 7461  nedata=slab_data
-00014640: 2e6c 696e 6564 6174 610a 2020 2020 2020  .linedata.      
-00014650: 2020 6c69 6e65 6461 7461 2e73 6f72 745f    linedata.sort_
-00014660: 7661 6c75 6573 2862 793d 5b27 4748 7a27  values(by=['GHz'
-00014670: 5d2c 6173 6365 6e64 696e 673d 4661 6c73  ],ascending=Fals
-00014680: 652c 696e 706c 6163 653d 5472 7565 2c69  e,inplace=True,i
-00014690: 676e 6f72 655f 696e 6465 783d 5472 7565  gnore_index=True
-000146a0: 290a 2020 2020 2020 2020 466d 6f64 656c  ).        Fmodel
-000146b0: 3d6c 696e 655f 666c 7578 6573 2877 696e  =line_fluxes(win
-000146c0: 646f 7773 2c63 2f6c 696e 6564 6174 615b  dows,c/linedata[
-000146d0: 2747 487a 275d 2a31 652d 332c 6c69 6e65  'GHz']*1e-3,line
-000146e0: 6461 7461 5b74 5d29 0a20 2020 2020 2020  data[t]).       
-000146f0: 2052 6d6f 6465 6c3d 6c69 6e65 5f66 6c75   Rmodel=line_flu
-00014700: 785f 7261 7469 6f73 2872 6174 696f 5f77  x_ratios(ratio_w
-00014710: 696e 646f 7773 2c63 2f6c 696e 6564 6174  indows,c/linedat
-00014720: 615b 2747 487a 275d 2a31 652d 332c 6c69  a['GHz']*1e-3,li
-00014730: 6e65 6461 7461 5b74 5d29 0a20 2020 2020  nedata[t]).     
-00014740: 2020 2050 6d6f 6465 6c3d 6c69 6e65 5f66     Pmodel=line_f
-00014750: 6c75 785f 7261 7469 6f73 2870 726f 6475  lux_ratios(produ
-00014760: 6374 5f77 696e 646f 7773 2c63 2f6c 696e  ct_windows,c/lin
-00014770: 6564 6174 615b 2747 487a 275d 2a31 652d  edata['GHz']*1e-
-00014780: 332c 6c69 6e65 6461 7461 5b74 5d29 0a20  3,linedata[t]). 
-00014790: 2020 2046 6f62 7365 7276 6564 3d73 7065     Fobserved=spe
-000147a0: 6374 7261 6c5f 666c 7578 6573 2877 696e  ctral_fluxes(win
-000147b0: 646f 7773 2c73 7065 6374 7261 5b3a 2c30  dows,spectra[:,0
-000147c0: 5d2c 7370 6563 7472 615b 3a2c 315d 290a  ],spectra[:,1]).
-000147d0: 2020 2020 526f 6273 6572 7665 643d 7370      Robserved=sp
-000147e0: 6563 7472 616c 5f66 6c75 785f 7261 7469  ectral_flux_rati
-000147f0: 6f73 2872 6174 696f 5f77 696e 646f 7773  os(ratio_windows
-00014800: 2c73 7065 6374 7261 5b3a 2c30 5d2c 7370  ,spectra[:,0],sp
-00014810: 6563 7472 615b 3a2c 315d 290a 2020 2020  ectra[:,1]).    
-00014820: 506f 6273 6572 7665 643d 7370 6563 7472  Pobserved=spectr
-00014830: 616c 5f66 6c75 785f 7072 6f64 7563 7473  al_flux_products
-00014840: 2870 726f 6475 6374 5f77 696e 646f 7773  (product_windows
-00014850: 2c73 7065 6374 7261 5b3a 2c30 5d2c 7370  ,spectra[:,0],sp
-00014860: 6563 7472 615b 3a2c 315d 290a 2020 2020  ectra[:,1]).    
-00014870: 6e6f 726d 5f66 6163 746f 723d 300a 2020  norm_factor=0.  
-00014880: 2020 6966 206c 656e 2877 696e 646f 7773    if len(windows
-00014890: 293e 303a 0a20 2020 2020 2020 2061 7265  )>0:.        are
-000148a0: 615f 3264 3d6e 702e 6473 7461 636b 285b  a_2d=np.dstack([
-000148b0: 6172 6561 2066 6f72 2069 2069 6e20 7261  area for i in ra
-000148c0: 6e67 6528 6c65 6e28 7769 6e64 6f77 7329  nge(len(windows)
-000148d0: 295d 292e 7371 7565 657a 6528 292e 7265  )]).squeeze().re
-000148e0: 7368 6170 6528 286c 656e 2861 7265 6129  shape((len(area)
-000148f0: 2c6c 656e 2877 696e 646f 7773 2929 290a  ,len(windows))).
-00014900: 2020 2020 2020 2020 466d 6f64 656c 5f32          Fmodel_2
-00014910: 643d 6e70 2e64 7374 6163 6b28 5b46 6d6f  d=np.dstack([Fmo
-00014920: 6465 6c20 666f 7220 6920 696e 2072 616e  del for i in ran
-00014930: 6765 286c 656e 2861 7265 6129 295d 292e  ge(len(area))]).
-00014940: 7371 7565 657a 6528 292e 542e 7265 7368  squeeze().T.resh
-00014950: 6170 6528 286c 656e 2861 7265 6129 2c6c  ape((len(area),l
-00014960: 656e 2877 696e 646f 7773 2929 290a 2020  en(windows))).  
-00014970: 2020 2020 2020 466f 6273 6572 7665 645f        Fobserved_
-00014980: 3264 3d6e 702e 6473 7461 636b 285b 466f  2d=np.dstack([Fo
-00014990: 6273 6572 7665 6420 666f 7220 6920 696e  bserved for i in
-000149a0: 2072 616e 6765 286c 656e 2861 7265 6129   range(len(area)
-000149b0: 295d 292e 7371 7565 657a 6528 292e 542e  )]).squeeze().T.
-000149c0: 7265 7368 6170 6528 286c 656e 2861 7265  reshape((len(are
-000149d0: 6129 2c6c 656e 2877 696e 646f 7773 2929  a),len(windows))
-000149e0: 290a 2020 2020 2020 2020 6966 206c 656e  ).        if len
-000149f0: 2877 696e 646f 7773 5b30 5d29 3d3d 333a  (windows[0])==3:
-00014a00: 2020 2320 7765 6967 6874 6564 2063 6869    # weighted chi
-00014a10: 320a 2020 2020 2020 2020 2020 2020 7769  2.            wi
-00014a20: 6e64 6f77 735f 7765 6967 6874 733d 6e70  ndows_weights=np
-00014a30: 2e61 7272 6179 285b 7769 6e64 6f77 735b  .array([windows[
-00014a40: 6b5d 5b32 5d20 666f 7220 6b20 696e 2072  k][2] for k in r
-00014a50: 616e 6765 286c 656e 2877 696e 646f 7773  ange(len(windows
-00014a60: 2929 5d29 0a20 2020 2020 2020 2020 2020  ))]).           
-00014a70: 2077 696e 646f 7773 5f77 6569 6768 7473   windows_weights
-00014a80: 5f32 643d 6e70 2e64 7374 6163 6b28 5b77  _2d=np.dstack([w
-00014a90: 696e 646f 7773 5f77 6569 6768 7473 2066  indows_weights f
-00014aa0: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
-00014ab0: 6e28 6172 6561 2929 5d29 2e73 7175 6565  n(area))]).squee
-00014ac0: 7a65 2829 2e54 2e72 6573 6861 7065 2828  ze().T.reshape((
-00014ad0: 6c65 6e28 6172 6561 292c 6c65 6e28 7769  len(area),len(wi
-00014ae0: 6e64 6f77 735f 7765 6967 6874 7329 2929  ndows_weights)))
-00014af0: 0a20 2020 2020 2020 2020 2020 2063 6869  .            chi
-00014b00: 5f61 7265 612b 3d6e 702e 7375 6d28 2828  _area+=np.sum(((
-00014b10: 466d 6f64 656c 5f32 642a 6172 6561 5f32  Fmodel_2d*area_2
-00014b20: 642d 466f 6273 6572 7665 645f 3264 292f  d-Fobserved_2d)/
-00014b30: 466f 6273 6572 7665 645f 3264 292a 2a32  Fobserved_2d)**2
-00014b40: 2a77 696e 646f 7773 5f77 6569 6768 7473  *windows_weights
-00014b50: 5f32 642c 6178 6973 3d31 290a 2020 2020  _2d,axis=1).    
-00014b60: 2020 2020 2020 2020 6e6f 726d 5f66 6163          norm_fac
-00014b70: 746f 722b 3d6e 702e 7375 6d28 7769 6e64  tor+=np.sum(wind
-00014b80: 6f77 735f 7765 6967 6874 7329 0a20 2020  ows_weights).   
-00014b90: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00014ba0: 2020 2020 2020 2063 6869 5f61 7265 612b         chi_area+
-00014bb0: 3d6e 702e 7375 6d28 2828 466d 6f64 656c  =np.sum(((Fmodel
-00014bc0: 5f32 642a 6172 6561 5f32 642d 466f 6273  _2d*area_2d-Fobs
-00014bd0: 6572 7665 645f 3264 292f 466f 6273 6572  erved_2d)/Fobser
-00014be0: 7665 645f 3264 292a 2a32 2c61 7869 733d  ved_2d)**2,axis=
-00014bf0: 3129 0a20 2020 2020 2020 2020 2020 206e  1).            n
-00014c00: 6f72 6d5f 6661 6374 6f72 2b3d 6c65 6e28  orm_factor+=len(
-00014c10: 7769 6e64 6f77 7329 0a20 2020 2069 6620  windows).    if 
-00014c20: 6c65 6e28 7261 7469 6f5f 7769 6e64 6f77  len(ratio_window
-00014c30: 7329 3e30 3a0a 2020 2020 2020 2020 526d  s)>0:.        Rm
-00014c40: 6f64 656c 5f32 643d 6e70 2e64 7374 6163  odel_2d=np.dstac
-00014c50: 6b28 5b52 6d6f 6465 6c20 666f 7220 6920  k([Rmodel for i 
-00014c60: 696e 2072 616e 6765 286c 656e 2861 7265  in range(len(are
-00014c70: 6129 295d 292e 7371 7565 657a 6528 292e  a))]).squeeze().
-00014c80: 542e 7265 7368 6170 6528 286c 656e 2861  T.reshape((len(a
-00014c90: 7265 6129 2c6c 656e 2872 6174 696f 5f77  rea),len(ratio_w
-00014ca0: 696e 646f 7773 2929 290a 2020 2020 2020  indows))).      
-00014cb0: 2020 526f 6273 6572 7665 645f 3264 3d6e    Robserved_2d=n
-00014cc0: 702e 6473 7461 636b 285b 526f 6273 6572  p.dstack([Robser
-00014cd0: 7665 6420 666f 7220 6920 696e 2072 616e  ved for i in ran
-00014ce0: 6765 286c 656e 2861 7265 6129 295d 292e  ge(len(area))]).
-00014cf0: 7371 7565 657a 6528 292e 542e 7265 7368  squeeze().T.resh
-00014d00: 6170 6528 286c 656e 2861 7265 6129 2c6c  ape((len(area),l
-00014d10: 656e 2872 6174 696f 5f77 696e 646f 7773  en(ratio_windows
-00014d20: 2929 290a 2020 2020 2020 2020 6966 2028  ))).        if (
-00014d30: 6c65 6e28 7261 7469 6f5f 7769 6e64 6f77  len(ratio_window
-00014d40: 735b 305d 293d 3d33 293a 2020 2320 7765  s[0])==3):  # we
-00014d50: 6967 6874 6564 2063 6869 320a 2020 2020  ighted chi2.    
-00014d60: 2020 2020 2020 2020 7261 7469 6f5f 7769          ratio_wi
-00014d70: 6e64 6f77 735f 7765 6967 6874 733d 6e70  ndows_weights=np
-00014d80: 2e61 7272 6179 285b 7261 7469 6f5f 7769  .array([ratio_wi
-00014d90: 6e64 6f77 735b 6b5d 5b32 5d20 666f 7220  ndows[k][2] for 
-00014da0: 6b20 696e 2072 616e 6765 286c 656e 2872  k in range(len(r
-00014db0: 6174 696f 5f77 696e 646f 7773 2929 5d29  atio_windows))])
-00014dc0: 0a20 2020 2020 2020 2020 2020 2072 6174  .            rat
-00014dd0: 696f 5f77 696e 646f 7773 5f77 6569 6768  io_windows_weigh
-00014de0: 7473 5f32 643d 6e70 2e64 7374 6163 6b28  ts_2d=np.dstack(
-00014df0: 5b72 6174 696f 5f77 696e 646f 7773 5f77  [ratio_windows_w
-00014e00: 6569 6768 7473 2066 6f72 2069 2069 6e20  eights for i in 
-00014e10: 7261 6e67 6528 6c65 6e28 6172 6561 2929  range(len(area))
-00014e20: 5d29 2e73 7175 6565 7a65 2829 2e54 2e72  ]).squeeze().T.r
-00014e30: 6573 6861 7065 2828 6c65 6e28 6172 6561  eshape((len(area
-00014e40: 292c 6c65 6e28 7261 7469 6f5f 7769 6e64  ),len(ratio_wind
-00014e50: 6f77 735f 7765 6967 6874 7329 2929 0a20  ows_weights))). 
-00014e60: 2020 2020 2020 2020 2020 2063 6869 5f61             chi_a
-00014e70: 7265 612b 3d6e 702e 7375 6d28 2828 526d  rea+=np.sum(((Rm
-00014e80: 6f64 656c 5f32 642d 526f 6273 6572 7665  odel_2d-Robserve
-00014e90: 645f 3264 292f 526f 6273 6572 7665 645f  d_2d)/Robserved_
-00014ea0: 3264 292a 2a32 2a72 6174 696f 5f77 696e  2d)**2*ratio_win
-00014eb0: 646f 7773 5f77 6569 6768 7473 5f32 642c  dows_weights_2d,
-00014ec0: 6178 6973 3d31 290a 2020 2020 2020 2020  axis=1).        
-00014ed0: 2020 2020 6e6f 726d 5f66 6163 746f 722b      norm_factor+
-00014ee0: 3d6e 702e 7375 6d28 7261 7469 6f5f 7769  =np.sum(ratio_wi
-00014ef0: 6e64 6f77 735f 7765 6967 6874 7329 0a20  ndows_weights). 
-00014f00: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00014f10: 2020 2020 2020 2020 2063 6869 5f61 7265           chi_are
-00014f20: 612b 3d6e 702e 7375 6d28 2828 526d 6f64  a+=np.sum(((Rmod
-00014f30: 656c 5f32 642d 526f 6273 6572 7665 645f  el_2d-Robserved_
-00014f40: 3264 292f 526f 6273 6572 7665 645f 3264  2d)/Robserved_2d
-00014f50: 292a 2a32 2c61 7869 733d 3129 0a20 2020  )**2,axis=1).   
-00014f60: 2020 2020 2020 2020 206e 6f72 6d5f 6661           norm_fa
-00014f70: 6374 6f72 2b3d 6c65 6e28 7261 7469 6f5f  ctor+=len(ratio_
-00014f80: 7769 6e64 6f77 7329 0a20 2020 2069 6620  windows).    if 
-00014f90: 6c65 6e28 7072 6f64 7563 745f 7769 6e64  len(product_wind
-00014fa0: 6f77 7329 3e30 3a0a 2020 2020 2020 2020  ows)>0:.        
-00014fb0: 6172 6561 5f32 643d 6e70 2e64 7374 6163  area_2d=np.dstac
-00014fc0: 6b28 5b61 7265 6120 666f 7220 6920 696e  k([area for i in
-00014fd0: 2072 616e 6765 286c 656e 2870 726f 6475   range(len(produ
-00014fe0: 6374 5f77 696e 646f 7773 2929 5d29 2e73  ct_windows))]).s
-00014ff0: 7175 6565 7a65 2829 2e72 6573 6861 7065  queeze().reshape
-00015000: 2828 6c65 6e28 6172 6561 292c 6c65 6e28  ((len(area),len(
-00015010: 7072 6f64 7563 745f 7769 6e64 6f77 7329  product_windows)
-00015020: 2929 0a20 2020 2020 2020 2050 6d6f 6465  )).        Pmode
-00015030: 6c5f 3264 3d6e 702e 6473 7461 636b 285b  l_2d=np.dstack([
-00015040: 506d 6f64 656c 2066 6f72 2069 2069 6e20  Pmodel for i in 
-00015050: 7261 6e67 6528 6c65 6e28 6172 6561 2929  range(len(area))
-00015060: 5d29 2e73 7175 6565 7a65 2829 2e54 2e72  ]).squeeze().T.r
-00015070: 6573 6861 7065 2828 6c65 6e28 6172 6561  eshape((len(area
-00015080: 292c 6c65 6e28 7072 6f64 7563 745f 7769  ),len(product_wi
-00015090: 6e64 6f77 7329 2929 0a20 2020 2020 2020  ndows))).       
-000150a0: 2050 6f62 7365 7276 6564 5f32 643d 6e70   Pobserved_2d=np
-000150b0: 2e64 7374 6163 6b28 5b50 6f62 7365 7276  .dstack([Pobserv
-000150c0: 6564 2066 6f72 2069 2069 6e20 7261 6e67  ed for i in rang
-000150d0: 6528 6c65 6e28 6172 6561 2929 5d29 2e73  e(len(area))]).s
-000150e0: 7175 6565 7a65 2829 2e54 2e72 6573 6861  queeze().T.resha
-000150f0: 7065 2828 6c65 6e28 6172 6561 292c 6c65  pe((len(area),le
-00015100: 6e28 7072 6f64 7563 745f 7769 6e64 6f77  n(product_window
-00015110: 7329 2929 0a20 2020 2020 2020 2069 6620  s))).        if 
-00015120: 286c 656e 2870 726f 6475 6374 5f77 696e  (len(product_win
-00015130: 646f 7773 5b30 5d29 3d3d 3329 3a20 2023  dows[0])==3):  #
-00015140: 2077 6569 6768 7465 6420 6368 6932 0a20   weighted chi2. 
-00015150: 2020 2020 2020 2020 2020 2070 726f 6475             produ
-00015160: 6374 5f77 696e 646f 7773 5f77 6569 6768  ct_windows_weigh
-00015170: 7473 3d6e 702e 6172 7261 7928 5b70 726f  ts=np.array([pro
-00015180: 6475 6374 5f77 696e 646f 7773 5b6b 5d5b  duct_windows[k][
-00015190: 325d 2066 6f72 206b 2069 6e20 7261 6e67  2] for k in rang
-000151a0: 6528 6c65 6e28 7072 6f64 7563 745f 7769  e(len(product_wi
-000151b0: 6e64 6f77 7329 295d 290a 2020 2020 2020  ndows))]).      
-000151c0: 2020 2020 2020 7072 6f64 7563 745f 7769        product_wi
-000151d0: 6e64 6f77 735f 7765 6967 6874 735f 3264  ndows_weights_2d
-000151e0: 3d6e 702e 6473 7461 636b 285b 7072 6f64  =np.dstack([prod
-000151f0: 7563 745f 7769 6e64 6f77 735f 7765 6967  uct_windows_weig
-00015200: 6874 7320 666f 7220 6920 696e 2072 616e  hts for i in ran
-00015210: 6765 286c 656e 2861 7265 6129 295d 292e  ge(len(area))]).
-00015220: 7371 7565 657a 6528 292e 542e 7265 7368  squeeze().T.resh
-00015230: 6170 6528 286c 656e 2861 7265 6129 2c6c  ape((len(area),l
-00015240: 656e 2870 726f 6475 6374 5f77 696e 646f  en(product_windo
-00015250: 7773 5f77 6569 6768 7473 2929 290a 2020  ws_weights))).  
-00015260: 2020 2020 2020 2020 2020 6368 695f 6172            chi_ar
-00015270: 6561 2b3d 6e70 2e73 756d 2828 2828 506d  ea+=np.sum((((Pm
-00015280: 6f64 656c 5f32 642a 6172 6561 5f32 642a  odel_2d*area_2d*
-00015290: 2a32 292a 2a30 2e35 2d28 506f 6273 6572  *2)**0.5-(Pobser
-000152a0: 7665 645f 3264 292a 2a30 2e35 292f 2850  ved_2d)**0.5)/(P
-000152b0: 6f62 7365 7276 6564 5f32 6429 2a2a 302e  observed_2d)**0.
-000152c0: 3529 2a2a 322a 7072 6f64 7563 745f 7769  5)**2*product_wi
-000152d0: 6e64 6f77 735f 7765 6967 6874 735f 3264  ndows_weights_2d
-000152e0: 2c61 7869 733d 3129 0a20 2020 2020 2020  ,axis=1).       
-000152f0: 2020 2020 206e 6f72 6d5f 6661 6374 6f72       norm_factor
-00015300: 2b3d 6e70 2e73 756d 2870 726f 6475 6374  +=np.sum(product
-00015310: 5f77 696e 646f 7773 5f77 6569 6768 7473  _windows_weights
-00015320: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00015330: 2020 2020 2020 2020 2020 2020 6368 695f              chi_
-00015340: 6172 6561 2b3d 6e70 2e73 756d 2828 2828  area+=np.sum((((
-00015350: 506d 6f64 656c 5f32 642a 6172 6561 5f32  Pmodel_2d*area_2
-00015360: 642a 2a32 292a 2a30 2e35 2d28 506f 6273  d**2)**0.5-(Pobs
-00015370: 6572 7665 645f 3264 292a 2a30 2e35 292f  erved_2d)**0.5)/
-00015380: 2850 6f62 7365 7276 6564 5f32 6429 2a2a  (Pobserved_2d)**
-00015390: 302e 3529 2a2a 322c 6178 6973 3d31 290a  0.5)**2,axis=1).
-000153a0: 2020 2020 2020 2020 2020 2020 6e6f 726d              norm
-000153b0: 5f66 6163 746f 722b 3d6c 656e 2870 726f  _factor+=len(pro
-000153c0: 6475 6374 5f77 696e 646f 7773 290a 2020  duct_windows).  
-000153d0: 2020 6966 206e 6f72 6d5f 6661 6374 6f72    if norm_factor
-000153e0: 3e30 3a20 6368 695f 6172 6561 2f3d 6e6f  >0: chi_area/=no
-000153f0: 726d 5f66 6163 746f 720a 2020 2020 7265  rm_factor.    re
-00015400: 7475 726e 2863 6869 5f61 7265 6129 0a0a  turn(chi_area)..
-00015410: 0a64 6566 2072 6564 5f63 6869 325f 736c  .def red_chi2_sl
-00015420: 6162 2873 6c61 625f 6461 7461 2c73 7065  ab(slab_data,spe
-00015430: 6374 7261 2c6d 6173 6b2c 5264 6973 6b3d  ctra,mask,Rdisk=
-00015440: 6e70 2e6c 6f67 7370 6163 6528 2d32 2c32  np.logspace(-2,2
-00015450: 2c31 3029 2c64 6973 7461 6e63 653d 3132  ,10),distance=12
-00015460: 302c 4e4c 5445 3d46 616c 7365 2c52 3d33  0,NLTE=False,R=3
-00015470: 3030 302c 7368 6f72 745f 666f 726d 6174  000,short_format
-00015480: 3d46 616c 7365 2c6f 7665 726c 6170 3d46  =False,overlap=F
-00015490: 616c 7365 2c6e 6f69 7365 5f6c 6576 656c  alse,noise_level
-000154a0: 3d31 293a 0a20 2020 2027 2727 0a20 2020  =1):.    '''.   
-000154b0: 2052 6574 7572 6e73 2072 6564 7563 6564   Returns reduced
-000154c0: 2063 6869 3220 6261 7365 6420 6f6e 2073   chi2 based on s
-000154d0: 656c 6563 7465 6420 7370 6563 7472 616c  elected spectral
-000154e0: 2077 696e 646f 7773 2061 6372 6f73 7320   windows across 
-000154f0: 6469 6666 6572 656e 7420 656d 6974 7469  different emitti
-00015500: 6e67 2064 6973 6b20 7261 6469 7573 0a0a  ng disk radius..
-00015510: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-00015520: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00015530: 2020 736c 6162 5f64 6174 6120 3a20 7374    slab_data : st
-00015540: 7269 6e67 206f 7220 736c 6162 5f6d 6f64  ring or slab_mod
-00015550: 656c 2069 6e73 7461 6e63 650a 2020 2020  el instance.    
-00015560: 2020 7061 7468 2063 6f72 7265 7370 6f6e    path correspon
-00015570: 6469 6e67 2074 6f20 6120 7369 6e67 6c65  ding to a single
-00015580: 2073 6c61 6220 6d6f 6465 6c20 6f72 2061   slab model or a
-00015590: 2073 696e 676c 6520 736c 6162 5f6d 6f64   single slab_mod
-000155a0: 656c 2069 6e73 7461 6e63 650a 2020 2020  el instance.    
-000155b0: 0a20 2020 2073 7065 6374 7261 203a 206e  .    spectra : n
-000155c0: 756d 7079 2e61 7272 6179 0a20 2020 2020  umpy.array.     
-000155d0: 206e 756d 7079 2061 7272 6179 2077 6974   numpy array wit
-000155e0: 6820 6669 7273 7420 636f 6c75 6d6e 2074  h first column t
-000155f0: 6865 2077 6176 656c 656e 6774 6820 696e  he wavelength in
-00015600: 205b 6d69 6372 6f6e 735d 2061 6e64 2073   [microns] and s
-00015610: 6563 6f6e 6420 636f 6c75 6d6e 2066 6c75  econd column flu
-00015620: 7820 696e 205b 4a79 5d0a 2020 2020 0a20  x in [Jy].    . 
-00015630: 2020 2052 6469 736b 203a 2066 6c6f 6174     Rdisk : float
-00015640: 0a20 2020 2020 2052 6164 6975 7320 636f  .      Radius co
-00015650: 7272 6573 706f 6e64 696e 6720 746f 2065  rresponding to e
-00015660: 6d69 7474 696e 6720 6172 6561 2069 6e20  mitting area in 
-00015670: 6173 7472 6f6e 6f6d 6963 616c 2075 6e69  astronomical uni
-00015680: 7473 0a20 2020 200a 2020 2020 6469 7374  ts.    .    dist
-00015690: 616e 6365 203a 2066 6c6f 6174 0a20 2020  ance : float.   
-000156a0: 2020 2064 6973 7461 6e63 6520 6f66 2064     distance of d
-000156b0: 6973 6b20 696e 2070 6172 7365 630a 2020  isk in parsec.  
-000156c0: 2020 0a20 2020 204e 4c54 4520 3a20 626f    .    NLTE : bo
-000156d0: 6f6c 6561 6e0a 2020 2020 2020 6966 2054  olean.      if T
-000156e0: 7275 652c 204e 4c54 4520 666c 7578 2069  rue, NLTE flux i
-000156f0: 7320 7461 6b65 6e20 6672 6f6d 2074 6865  s taken from the
-00015700: 2073 6c61 6220 6d6f 6465 6c20 696e 2063   slab model in c
-00015710: 6173 6520 6f66 206f 7665 726c 6170 3d46  ase of overlap=F
-00015720: 616c 7365 2e0a 2020 2020 2727 270a 2020  alse..    '''.  
-00015730: 2020 6172 6561 3d28 6e70 2e70 692a 2852    area=(np.pi*(R
-00015740: 6469 736b 2a61 752f 6469 7374 616e 6365  disk*au/distance
-00015750: 2f70 6329 2a2a 3229 2e72 6573 6861 7065  /pc)**2).reshape
-00015760: 2852 6469 736b 2e73 6861 7065 5b30 5d2c  (Rdisk.shape[0],
-00015770: 3129 0a0a 2020 2020 6966 206e 6f74 206f  1)..    if not o
-00015780: 7665 726c 6170 3a0a 2020 2020 2020 2020  verlap:.        
-00015790: 6966 2069 7369 6e73 7461 6e63 6528 736c  if isinstance(sl
-000157a0: 6162 5f64 6174 612c 7374 7229 3a20 736c  ab_data,str): sl
-000157b0: 6162 5f64 6174 613d 7265 6164 5f73 6c61  ab_data=read_sla
-000157c0: 6228 736c 6162 5f64 6174 612c 7665 7262  b(slab_data,verb
-000157d0: 6f73 653d 4661 6c73 652c 7368 6f72 745f  ose=False,short_
-000157e0: 666f 726d 6174 3d73 686f 7274 5f66 6f72  format=short_for
-000157f0: 6d61 7429 0a20 2020 2020 2020 206c 6d69  mat).        lmi
-00015800: 6e3d 6e70 2e61 6d69 6e28 7370 6563 7472  n=np.amin(spectr
-00015810: 615b 3a2c 305d 290a 2020 2020 2020 2020  a[:,0]).        
-00015820: 6c6d 6178 3d6e 702e 616d 6178 2873 7065  lmax=np.amax(spe
-00015830: 6374 7261 5b3a 2c30 5d29 0a20 2020 2020  ctra[:,0]).     
-00015840: 2020 2073 6c61 625f 6461 7461 2e63 6f6e     slab_data.con
-00015850: 766f 6c76 6528 523d 522c 6c61 6d62 6461  volve(R=R,lambda
-00015860: 5f30 3d6c 6d69 6e2a 302e 392c 6c61 6d62  _0=lmin*0.9,lamb
-00015870: 6461 5f6e 3d6c 6d61 782a 312e 312c 4e4c  da_n=lmax*1.1,NL
-00015880: 5445 3d4e 4c54 452c 7665 7262 6f73 653d  TE=NLTE,verbose=
-00015890: 4661 6c73 6529 0a20 2020 2020 2020 2069  False).        i
-000158a0: 6620 4e4c 5445 3a0a 2020 2020 2020 2020  f NLTE:.        
-000158b0: 2020 2020 6d6f 6465 6c53 7065 633d 7370      modelSpec=sp
-000158c0: 6563 7472 6573 2e73 7065 6374 7265 7328  ectres.spectres(
-000158d0: 7370 6563 7472 615b 3a2c 305d 2c73 6c61  spectra[:,0],sla
-000158e0: 625f 6461 7461 2e63 6f6e 7657 6176 656c  b_data.convWavel
-000158f0: 656e 6774 682c 736c 6162 5f64 6174 612e  ength,slab_data.
-00015900: 636f 6e76 4e4c 5445 666c 7578 2a31 6532  convNLTEflux*1e2
-00015910: 332c 7665 7262 6f73 653d 4661 6c73 652c  3,verbose=False,
-00015920: 6669 6c6c 3d30 2e30 290a 2020 2020 2020  fill=0.0).      
-00015930: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00015940: 2020 2020 6d6f 6465 6c53 7065 633d 7370      modelSpec=sp
-00015950: 6563 7472 6573 2e73 7065 6374 7265 7328  ectres.spectres(
-00015960: 7370 6563 7472 615b 3a2c 305d 2c73 6c61  spectra[:,0],sla
-00015970: 625f 6461 7461 2e63 6f6e 7657 6176 656c  b_data.convWavel
-00015980: 656e 6774 682c 736c 6162 5f64 6174 612e  ength,slab_data.
-00015990: 636f 6e76 4c54 4566 6c75 782a 3165 3233  convLTEflux*1e23
-000159a0: 2c76 6572 626f 7365 3d46 616c 7365 2c66  ,verbose=False,f
-000159b0: 696c 6c3d 302e 3029 0a20 2020 2065 6c73  ill=0.0).    els
-000159c0: 653a 0a20 2020 2020 2020 2069 6620 6973  e:.        if is
-000159d0: 696e 7374 616e 6365 2873 6c61 625f 6461  instance(slab_da
-000159e0: 7461 2c73 7472 293a 2073 6c61 625f 6461  ta,str): slab_da
-000159f0: 7461 3d72 6561 645f 6f76 6572 6c61 705f  ta=read_overlap_
-00015a00: 7370 6563 7472 6128 736c 6162 5f64 6174  spectra(slab_dat
-00015a10: 612c 7665 7262 6f73 653d 4661 6c73 6529  a,verbose=False)
-00015a20: 0a20 2020 2020 2020 206c 6d69 6e3d 6e70  .        lmin=np
-00015a30: 2e61 6d69 6e28 7370 6563 7472 615b 3a2c  .amin(spectra[:,
-00015a40: 305d 290a 2020 2020 2020 2020 6c6d 6178  0]).        lmax
-00015a50: 3d6e 702e 616d 6178 2873 7065 6374 7261  =np.amax(spectra
-00015a60: 5b3a 2c30 5d29 0a20 2020 2020 2020 2073  [:,0]).        s
-00015a70: 6c61 625f 6461 7461 2e63 6f6e 766f 6c76  lab_data.convolv
-00015a80: 655f 6f76 6572 6c61 7028 523d 522c 6c61  e_overlap(R=R,la
-00015a90: 6d62 6461 5f30 3d6c 6d69 6e2a 302e 392c  mbda_0=lmin*0.9,
-00015aa0: 6c61 6d62 6461 5f6e 3d6c 6d61 782a 312e  lambda_n=lmax*1.
-00015ab0: 312c 7665 7262 6f73 653d 4661 6c73 6529  1,verbose=False)
-00015ac0: 0a20 2020 2020 2020 206d 6f64 656c 5370  .        modelSp
-00015ad0: 6563 3d73 7065 6374 7265 732e 7370 6563  ec=spectres.spec
-00015ae0: 7472 6573 2873 7065 6374 7261 5b3a 2c30  tres(spectra[:,0
-00015af0: 5d2c 632f 736c 6162 5f64 6174 612e 636f  ],c/slab_data.co
-00015b00: 6e76 4f76 6572 6c61 7046 7265 715b 3a3a  nvOverlapFreq[::
-00015b10: 2d31 5d2a 3165 2d33 2c73 6c61 625f 6461  -1]*1e-3,slab_da
-00015b20: 7461 2e63 6f6e 764f 7665 726c 6170 4c54  ta.convOverlapLT
-00015b30: 455b 3a3a 2d31 5d2a 3165 3233 2c76 6572  E[::-1]*1e23,ver
-00015b40: 626f 7365 3d46 616c 7365 2c66 696c 6c3d  bose=False,fill=
-00015b50: 302e 3029 0a20 2020 2073 7065 6374 7261  0.0).    spectra
-00015b60: 5f32 643d 7370 6563 7472 615b 6d61 736b  _2d=spectra[mask
-00015b70: 2c31 5d2e 7265 7368 6170 6528 312c 7370  ,1].reshape(1,sp
-00015b80: 6563 7472 615b 6d61 736b 2c2d 315d 2e73  ectra[mask,-1].s
-00015b90: 6861 7065 5b30 5d29 2a6e 702e 6f6e 6573  hape[0])*np.ones
-00015ba0: 5f6c 696b 6528 6172 6561 290a 2020 2020  _like(area).    
-00015bb0: 6d6f 6465 6c53 7065 635f 3264 3d6d 6f64  modelSpec_2d=mod
-00015bc0: 656c 5370 6563 5b6d 6173 6b5d 2e72 6573  elSpec[mask].res
-00015bd0: 6861 7065 2831 2c6d 6f64 656c 5370 6563  hape(1,modelSpec
-00015be0: 5b6d 6173 6b5d 2e73 6861 7065 5b30 5d29  [mask].shape[0])
-00015bf0: 2a6e 702e 6f6e 6573 5f6c 696b 6528 6172  *np.ones_like(ar
-00015c00: 6561 290a 2020 2020 6172 6561 5f32 643d  ea).    area_2d=
-00015c10: 6172 6561 2e72 6573 6861 7065 2861 7265  area.reshape(are
-00015c20: 612e 7368 6170 655b 305d 2c31 290a 2020  a.shape[0],1).  
-00015c30: 2020 6368 695f 6172 6561 3d6e 702e 7375    chi_area=np.su
-00015c40: 6d28 2873 7065 6374 7261 5f32 642d 6d6f  m((spectra_2d-mo
-00015c50: 6465 6c53 7065 635f 3264 2a61 7265 615f  delSpec_2d*area_
-00015c60: 3264 292a 2a32 2c61 7869 733d 3129 2f6c  2d)**2,axis=1)/l
-00015c70: 656e 2873 7065 6374 7261 5b6d 6173 6b2c  en(spectra[mask,
-00015c80: 305d 292f 6e6f 6973 655f 6c65 7665 6c2a  0])/noise_level*
-00015c90: 2a32 0a0a 2020 2020 7265 7475 726e 2863  *2..    return(c
-00015ca0: 6869 5f61 7265 6129 0a                   hi_area).
+00011cc0: 2729 0a20 2020 2066 6f72 2069 2069 6e20  ').    for i in 
+00011cd0: 7261 6e67 6528 6e6d 6f64 656c 7329 3a0a  range(nmodels):.
+00011ce0: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
+00011cf0: 6627 5c6e 2a2a 2a20 6d6f 6465 6c20 7b69  f'\n*** model {i
+00011d00: 2b31 7d20 2a2a 2a5c 6e27 290a 2020 2020  +1} ***\n').    
+00011d10: 2020 2020 6966 206e 702e 7375 6d28 4e74      if np.sum(Nt
+00011d20: 6f74 5f6c 6973 7429 213d 6e6d 6f64 656c  ot_list)!=nmodel
+00011d30: 733a 0a20 2020 2020 2020 2020 2020 2066  s:.            f
+00011d40: 2e77 7269 7465 2866 6d74 2e66 6f72 6d61  .write(fmt.forma
+00011d50: 7428 277b 3a2e 336d 7d27 2c4e 746f 745f  t('{:.3m}',Ntot_
+00011d60: 6c69 7374 5b69 5d29 290a 2020 2020 2020  list[i])).      
+00011d70: 2020 2020 2020 662e 7772 6974 6528 2709        f.write('.
+00011d80: 2020 2021 204e 4874 6f74 2020 5b63 6d5e     ! NHtot  [cm^
+00011d90: 2d32 5d20 746f 7461 6c20 6761 7320 636f  -2] total gas co
+00011da0: 6c75 6d6e 2064 656e 7369 7479 5c6e 2729  lumn density\n')
+00011db0: 0a20 2020 2020 2020 2069 6620 6e70 2e73  .        if np.s
+00011dc0: 756d 286e 4870 6c75 735f 6c69 7374 2921  um(nHplus_list)!
+00011dd0: 3d6e 6d6f 6465 6c73 3a0a 2020 2020 2020  =nmodels:.      
+00011de0: 2020 2020 2020 662e 7772 6974 6528 666d        f.write(fm
+00011df0: 742e 666f 726d 6174 2827 7b3a 2e33 6d7d  t.format('{:.3m}
+00011e00: 272c 6e48 706c 7573 5f6c 6973 745b 695d  ',nHplus_list[i]
+00011e10: 2929 0a20 2020 2020 2020 2020 2020 2066  )).            f
+00011e20: 2e77 7269 7465 2827 0920 2020 2120 6e48  .write('.   ! nH
+00011e30: 2b20 2020 205b 636d 5e2d 335d 2020 7072  +    [cm^-3]  pr
+00011e40: 6f74 6f6e 206e 756d 6265 7220 6465 6e73  oton number dens
+00011e50: 6974 795c 6e27 290a 2020 2020 2020 2020  ity\n').        
+00011e60: 6966 206e 702e 7375 6d28 6e48 315f 6c69  if np.sum(nH1_li
+00011e70: 7374 2921 3d6e 6d6f 6465 6c73 3a0a 2020  st)!=nmodels:.  
+00011e80: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
+00011e90: 6528 666d 742e 666f 726d 6174 2827 7b3a  e(fmt.format('{:
+00011ea0: 2e33 6d7d 272c 6e48 315f 6c69 7374 5b69  .3m}',nH1_list[i
+00011eb0: 5d29 290a 2020 2020 2020 2020 2020 2020  ])).            
+00011ec0: 662e 7772 6974 6528 2709 2020 2021 206e  f.write('.   ! n
+00011ed0: 4849 0920 5b63 6d5e 2d33 5d20 6174 6f6d  HI. [cm^-3] atom
+00011ee0: 6963 2068 7964 726f 6765 6e5c 6e27 290a  ic hydrogen\n').
+00011ef0: 2020 2020 2020 2020 6966 206e 702e 7375          if np.su
+00011f00: 6d28 6e48 325f 6c69 7374 2921 3d6e 6d6f  m(nH2_list)!=nmo
+00011f10: 6465 6c73 3a0a 2020 2020 2020 2020 2020  dels:.          
+00011f20: 2020 662e 7772 6974 6528 666d 742e 666f    f.write(fmt.fo
+00011f30: 726d 6174 2827 7b3a 2e33 6d7d 272c 6e48  rmat('{:.3m}',nH
+00011f40: 325f 6c69 7374 5b69 5d29 290a 2020 2020  2_list[i])).    
+00011f50: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
+00011f60: 2709 2020 2021 206e 4832 2020 2020 5b63  '.   ! nH2    [c
+00011f70: 6d5e 2d33 5d20 2020 6d6f 6c65 6375 6c61  m^-3]   molecula
+00011f80: 7220 6879 6472 6f67 656e 5c6e 2729 0a20  r hydrogen\n'). 
+00011f90: 2020 2020 2020 2069 6620 6e70 2e73 756d         if np.sum
+00011fa0: 286e 4865 5f6c 6973 7429 213d 6e6d 6f64  (nHe_list)!=nmod
+00011fb0: 656c 733a 0a20 2020 2020 2020 2020 2020  els:.           
+00011fc0: 2066 2e77 7269 7465 2866 6d74 2e66 6f72   f.write(fmt.for
+00011fd0: 6d61 7428 277b 3a2e 336d 7d27 2c6e 4865  mat('{:.3m}',nHe
+00011fe0: 5f6c 6973 745b 695d 2929 0a20 2020 2020  _list[i])).     
+00011ff0: 2020 2020 2020 2066 2e77 7269 7465 2827         f.write('
+00012000: 0920 2020 2120 6e48 6520 2020 205b 636d  .   ! nHe    [cm
+00012010: 5e2d 335d 2020 2048 656c 6975 6d5c 6e27  ^-3]   Helium\n'
+00012020: 290a 2020 2020 2020 2020 6966 206e 702e  ).        if np.
+00012030: 7375 6d28 6e65 6c65 635f 6c69 7374 2921  sum(nelec_list)!
+00012040: 3d6e 6d6f 6465 6c73 3a0a 2020 2020 2020  =nmodels:.      
+00012050: 2020 2020 2020 662e 7772 6974 6528 666d        f.write(fm
+00012060: 742e 666f 726d 6174 2827 7b3a 2e33 6d7d  t.format('{:.3m}
+00012070: 272c 6e65 6c65 635f 6c69 7374 5b69 5d29  ',nelec_list[i])
+00012080: 290a 2020 2020 2020 2020 2020 2020 662e  ).            f.
+00012090: 7772 6974 6528 2709 2020 2021 206e 656c  write('.   ! nel
+000120a0: 6563 2020 5b63 6d5e 2d33 5d20 2020 656c  ec  [cm^-3]   el
+000120b0: 6563 7472 6f6e 206e 756d 6265 7220 6465  ectron number de
+000120c0: 6e73 6974 795c 6e27 290a 2020 2020 2020  nsity\n').      
+000120d0: 2020 6966 206e 702e 7375 6d28 5467 5f6c    if np.sum(Tg_l
+000120e0: 6973 7429 213d 6e6d 6f64 656c 733a 0a20  ist)!=nmodels:. 
+000120f0: 2020 2020 2020 2020 2020 2066 2e77 7269             f.wri
+00012100: 7465 2866 6d74 2e66 6f72 6d61 7428 277b  te(fmt.format('{
+00012110: 3a2e 336d 7d27 2c54 675f 6c69 7374 5b69  :.3m}',Tg_list[i
+00012120: 5d29 290a 2020 2020 2020 2020 2020 2020  ])).            
+00012130: 662e 7772 6974 6528 2709 2020 2021 2054  f.write('.   ! T
+00012140: 6761 7320 5b4b 5d20 2020 2020 2020 2020  gas [K]         
+00012150: 2020 6761 7320 7465 6d70 6572 6174 7572    gas temperatur
+00012160: 655c 6e27 290a 2020 2020 2020 2020 6966  e\n').        if
+00012170: 206e 702e 7375 6d28 5464 5f6c 6973 7429   np.sum(Td_list)
+00012180: 213d 6e6d 6f64 656c 733a 0a20 2020 2020  !=nmodels:.     
+00012190: 2020 2020 2020 2066 2e77 7269 7465 2866         f.write(f
+000121a0: 6d74 2e66 6f72 6d61 7428 277b 3a2e 336d  mt.format('{:.3m
+000121b0: 7d27 2c54 645f 6c69 7374 5b69 5d29 290a  }',Td_list[i])).
+000121c0: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
+000121d0: 6974 6528 2709 2020 2021 2054 6475 7374  ite('.   ! Tdust
+000121e0: 205b 4b5d 2020 2020 2020 2020 2020 2064   [K]           d
+000121f0: 7573 7420 7465 6d70 6572 6174 7572 655c  ust temperature\
+00012200: 6e27 290a 2020 2020 2020 2020 6966 206e  n').        if n
+00012210: 702e 7375 6d28 7674 7572 625f 6c69 7374  p.sum(vturb_list
+00012220: 2921 3d6e 6d6f 6465 6c73 3a0a 2020 2020  )!=nmodels:.    
+00012230: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
+00012240: 666d 742e 666f 726d 6174 2827 7b3a 2e33  fmt.format('{:.3
+00012250: 6d7d 272c 7674 7572 625f 6c69 7374 5b69  m}',vturb_list[i
+00012260: 5d29 290a 2020 2020 2020 2020 2020 2020  ])).            
+00012270: 662e 7772 6974 6528 2709 2020 2021 2076  f.write('.   ! v
+00012280: 7475 7262 2020 5b6b 6d73 2f73 5d20 2020  turb  [kms/s]   
+00012290: 2074 7572 6275 6c65 6e74 2076 656c 6f63   turbulent veloc
+000122a0: 6974 795c 6e27 290a 2020 2020 2020 2020  ity\n').        
+000122b0: 6966 206e 702e 7375 6d28 6475 7374 5f74  if np.sum(dust_t
+000122c0: 6f5f 6761 735f 6c69 7374 2921 3d6e 6d6f  o_gas_list)!=nmo
+000122d0: 6465 6c73 3a0a 2020 2020 2020 2020 2020  dels:.          
+000122e0: 2020 662e 7772 6974 6528 666d 742e 666f    f.write(fmt.fo
+000122f0: 726d 6174 2827 7b3a 2e33 6d7d 272c 6475  rmat('{:.3m}',du
+00012300: 7374 5f74 6f5f 6761 735f 6c69 7374 5b69  st_to_gas_list[i
+00012310: 5d29 290a 2020 2020 2020 2020 2020 2020  ])).            
+00012320: 662e 7772 6974 6528 2709 2020 2021 2064  f.write('.   ! d
+00012330: 7573 745f 746f 5f67 6173 5c6e 2729 0a20  ust_to_gas\n'). 
+00012340: 2020 2020 2020 2069 6620 6e70 2e73 756d         if np.sum
+00012350: 286c 696e 655f 6f76 6572 6c61 705f 6c69  (line_overlap_li
+00012360: 7374 2921 3d32 2a6e 6d6f 6465 6c73 3a0a  st)!=2*nmodels:.
+00012370: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
+00012380: 6974 6528 666d 742e 666f 726d 6174 2827  ite(fmt.format('
+00012390: 7b3a 2e33 667d 272c 6c69 6e65 5f6f 7665  {:.3f}',line_ove
+000123a0: 726c 6170 5f6c 6973 745b 692c 305d 292b  rlap_list[i,0])+
+000123b0: 2720 272b 666d 742e 666f 726d 6174 2827  ' '+fmt.format('
+000123c0: 7b3a 2e33 667d 272c 6c69 6e65 5f6f 7665  {:.3f}',line_ove
+000123d0: 726c 6170 5f6c 6973 745b 692c 315d 2929  rlap_list[i,1]))
+000123e0: 0a20 2020 2020 2020 2020 2020 2066 2e77  .            f.w
+000123f0: 7269 7465 2827 0920 2020 2120 6c69 6e65  rite('.   ! line
+00012400: 5f6f 7665 726c 6170 2020 5b6d 6963 726f  _overlap  [micro
+00012410: 6e73 5d20 206d 696e 696d 756d 2061 6e64  ns]  minimum and
+00012420: 206d 6178 696d 756d 2077 6176 656c 656e   maximum wavelen
+00012430: 6774 6873 2066 6f72 206c 696e 6520 6f76  gths for line ov
+00012440: 6572 6c61 705c 6e27 290a 2020 2020 2020  erlap\n').      
+00012450: 2020 6966 206e 702e 7375 6d28 525f 6f76    if np.sum(R_ov
+00012460: 6572 6c61 705f 6c69 7374 2921 3d6e 6d6f  erlap_list)!=nmo
+00012470: 6465 6c73 3a0a 2020 2020 2020 2020 2020  dels:.          
+00012480: 2020 662e 7772 6974 6528 666d 742e 666f    f.write(fmt.fo
+00012490: 726d 6174 2827 7b3a 2e33 6d7d 272c 525f  rmat('{:.3m}',R_
+000124a0: 6f76 6572 6c61 705f 6c69 7374 5b69 5d29  overlap_list[i])
+000124b0: 290a 2020 2020 2020 2020 2020 2020 662e  ).            f.
+000124c0: 7772 6974 6528 2709 2020 2021 2052 5f6f  write('.   ! R_o
+000124d0: 7665 726c 6170 2020 7361 6d70 6c69 6e67  verlap  sampling
+000124e0: 2067 7269 6420 7265 736f 6c75 7469 6f6e   grid resolution
+000124f0: 2066 6f72 206c 696e 6520 6f76 6572 6c61   for line overla
+00012500: 705c 6e27 290a 2020 2020 2020 2020 662e  p\n').        f.
+00012510: 7772 6974 6528 6627 7b6c 656e 2873 7065  write(f'{len(spe
+00012520: 6369 6573 5f6c 6973 7429 7d09 2020 2021  cies_list)}.   !
+00012530: 204e 7370 6563 6965 7320 2020 2020 2020   Nspecies       
+00012540: 2020 2020 206e 756d 6265 7220 6f66 2073       number of s
+00012550: 7065 6369 6573 2066 6f72 2074 6861 7420  pecies for that 
+00012560: 6d6f 6465 6c5c 6e27 290a 2020 2020 2020  model\n').      
+00012570: 2020 666f 7220 6a20 696e 2072 616e 6765    for j in range
+00012580: 286c 656e 2873 7065 6369 6573 5f6c 6973  (len(species_lis
+00012590: 7429 293a 0a20 2020 2020 2020 2020 2020  t)):.           
+000125a0: 2066 2e77 7269 7465 2866 277b 6c69 7374   f.write(f'{list
+000125b0: 2873 7065 6369 6573 5f6c 6973 742e 6b65  (species_list.ke
+000125c0: 7973 2829 295b 6a5d 7d20 2020 2020 207b  ys())[j]}      {
+000125d0: 7370 6563 6965 735f 6c69 7374 5b6c 6973  species_list[lis
+000125e0: 7428 7370 6563 6965 735f 6c69 7374 2e6b  t(species_list.k
+000125f0: 6579 7328 2929 5b6a 5d5d 7d5c 6e27 290a  eys())[j]]}\n').
+00012600: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
+00012610: 2720 2020 2020 2020 2020 2020 2120 656e  '           ! en
+00012620: 645c 6e27 290a 2020 2020 2020 2020 662e  d\n').        f.
+00012630: 7772 6974 6528 272d 2d2d 2d2d 2d2d 2d2d  write('---------
+00012640: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00012650: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00012660: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2729  --------------')
+00012670: 0a20 2020 2066 2e63 6c6f 7365 2829 0a20  .    f.close(). 
+00012680: 2020 2072 6574 7572 6e0a 0a0a 6465 6620     return...def 
+00012690: 6765 6e65 7261 7465 5f31 445f 7374 7275  generate_1D_stru
+000126a0: 6374 7572 6528 647a 2c73 7065 6369 6573  cture(dz,species
+000126b0: 5f6c 6973 742c 7674 7572 622c 6e64 2c54  _list,vturb,nd,T
+000126c0: 642c 6e5f 7370 6563 6965 732c 545f 7370  d,n_species,T_sp
+000126d0: 6563 6965 732c 6e48 323d 302c 6e48 493d  ecies,nH2=0,nHI=
+000126e0: 302c 6e48 4949 3d30 2c6e 4865 3d30 2c6e  0,nHII=0,nHe=0,n
+000126f0: 656c 6563 3d30 2c66 696c 656e 616d 653d  elec=0,filename=
+00012700: 2731 445f 7374 7275 6374 7572 6527 293a  '1D_structure'):
+00012710: 0a20 2020 2022 2222 0a20 2020 2047 656e  .    """.    Gen
+00012720: 6572 6174 6573 2031 4420 7374 7275 6374  erates 1D struct
+00012730: 7572 6520 6669 6c65 2072 6571 7569 7265  ure file require
+00012740: 6420 666f 7220 3144 2073 6c61 6220 6d6f  d for 1D slab mo
+00012750: 6465 6c73 0a20 2020 2022 2222 0a20 2020  dels.    """.   
+00012760: 2069 6620 6973 696e 7374 616e 6365 2864   if isinstance(d
+00012770: 7a2c 666c 6f61 7429 206f 7220 6973 696e  z,float) or isin
+00012780: 7374 616e 6365 2864 7a2c 696e 7429 3a20  stance(dz,int): 
+00012790: 647a 3d6e 702e 6172 7261 7928 5b64 7a5d  dz=np.array([dz]
+000127a0: 290a 2020 2020 6966 2069 7369 6e73 7461  ).    if isinsta
+000127b0: 6e63 6528 647a 2c6c 6973 7429 3a20 647a  nce(dz,list): dz
+000127c0: 3d6e 702e 6172 7261 7928 647a 290a 2020  =np.array(dz).  
+000127d0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+000127e0: 7370 6563 6965 735f 6c69 7374 2c73 7472  species_list,str
+000127f0: 293a 2073 7065 6369 6573 5f6c 6973 743d  ): species_list=
+00012800: 5b73 7065 6369 6573 5f6c 6973 745d 0a20  [species_list]. 
+00012810: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00012820: 2876 7475 7262 2c66 6c6f 6174 2920 6f72  (vturb,float) or
+00012830: 2069 7369 6e73 7461 6e63 6528 7674 7572   isinstance(vtur
+00012840: 622c 696e 7429 3a20 7674 7572 623d 6e70  b,int): vturb=np
+00012850: 2e6f 6e65 735f 6c69 6b65 2864 7a29 2a76  .ones_like(dz)*v
+00012860: 7475 7262 0a20 2020 2069 6620 6973 696e  turb.    if isin
+00012870: 7374 616e 6365 286e 642c 666c 6f61 7429  stance(nd,float)
+00012880: 206f 7220 6973 696e 7374 616e 6365 286e   or isinstance(n
+00012890: 642c 696e 7429 3a20 6e64 3d6e 702e 6f6e  d,int): nd=np.on
+000128a0: 6573 5f6c 696b 6528 647a 292a 6e64 0a20  es_like(dz)*nd. 
+000128b0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+000128c0: 2854 642c 666c 6f61 7429 206f 7220 6973  (Td,float) or is
+000128d0: 696e 7374 616e 6365 2854 642c 696e 7429  instance(Td,int)
+000128e0: 3a20 5464 3d6e 702e 6f6e 6573 5f6c 696b  : Td=np.ones_lik
+000128f0: 6528 647a 292a 5464 0a20 2020 2069 6620  e(dz)*Td.    if 
+00012900: 6973 696e 7374 616e 6365 286e 4832 2c66  isinstance(nH2,f
+00012910: 6c6f 6174 2920 6f72 2069 7369 6e73 7461  loat) or isinsta
+00012920: 6e63 6528 6e48 322c 696e 7429 3a20 6e48  nce(nH2,int): nH
+00012930: 323d 6e70 2e6f 6e65 735f 6c69 6b65 2864  2=np.ones_like(d
+00012940: 7a29 2a6e 4832 0a20 2020 2069 6620 6973  z)*nH2.    if is
+00012950: 696e 7374 616e 6365 286e 4849 2c66 6c6f  instance(nHI,flo
+00012960: 6174 2920 6f72 2069 7369 6e73 7461 6e63  at) or isinstanc
+00012970: 6528 6e48 492c 696e 7429 3a20 6e48 493d  e(nHI,int): nHI=
+00012980: 6e70 2e6f 6e65 735f 6c69 6b65 2864 7a29  np.ones_like(dz)
+00012990: 2a6e 4849 0a20 2020 2069 6620 6973 696e  *nHI.    if isin
+000129a0: 7374 616e 6365 286e 4849 492c 666c 6f61  stance(nHII,floa
+000129b0: 7429 206f 7220 6973 696e 7374 616e 6365  t) or isinstance
+000129c0: 286e 4849 492c 696e 7429 3a20 6e48 4949  (nHII,int): nHII
+000129d0: 3d6e 702e 6f6e 6573 5f6c 696b 6528 647a  =np.ones_like(dz
+000129e0: 292a 6e48 4949 0a20 2020 2069 6620 6973  )*nHII.    if is
+000129f0: 696e 7374 616e 6365 286e 4865 2c66 6c6f  instance(nHe,flo
+00012a00: 6174 2920 6f72 2069 7369 6e73 7461 6e63  at) or isinstanc
+00012a10: 6528 6e48 652c 696e 7429 3a20 6e48 653d  e(nHe,int): nHe=
+00012a20: 6e70 2e6f 6e65 735f 6c69 6b65 2864 7a29  np.ones_like(dz)
+00012a30: 2a6e 4865 0a20 2020 2069 6620 6973 696e  *nHe.    if isin
+00012a40: 7374 616e 6365 286e 656c 6563 2c66 6c6f  stance(nelec,flo
+00012a50: 6174 2920 6f72 2069 7369 6e73 7461 6e63  at) or isinstanc
+00012a60: 6528 6e65 6c65 632c 696e 7429 3a20 6e65  e(nelec,int): ne
+00012a70: 6c65 633d 6e70 2e6f 6e65 735f 6c69 6b65  lec=np.ones_like
+00012a80: 2864 7a29 2a6e 656c 6563 0a20 2020 2069  (dz)*nelec.    i
+00012a90: 6620 6973 696e 7374 616e 6365 286e 5f73  f isinstance(n_s
+00012aa0: 7065 6369 6573 2c66 6c6f 6174 2920 6f72  pecies,float) or
+00012ab0: 2069 7369 6e73 7461 6e63 6528 6e5f 7370   isinstance(n_sp
+00012ac0: 6563 6965 732c 696e 7429 3a20 6e5f 7370  ecies,int): n_sp
+00012ad0: 6563 6965 733d 6e70 2e6f 6e65 7328 2864  ecies=np.ones((d
+00012ae0: 7a2e 7368 6170 655b 305d 2c6c 656e 2873  z.shape[0],len(s
+00012af0: 7065 6369 6573 5f6c 6973 7429 2929 2a6e  pecies_list)))*n
+00012b00: 5f73 7065 6369 6573 0a20 2020 2069 6620  _species.    if 
+00012b10: 6973 696e 7374 616e 6365 2854 5f73 7065  isinstance(T_spe
+00012b20: 6369 6573 2c66 6c6f 6174 2920 6f72 2069  cies,float) or i
+00012b30: 7369 6e73 7461 6e63 6528 545f 7370 6563  sinstance(T_spec
+00012b40: 6965 732c 696e 7429 3a20 545f 7370 6563  ies,int): T_spec
+00012b50: 6965 733d 6e70 2e6f 6e65 7328 2864 7a2e  ies=np.ones((dz.
+00012b60: 7368 6170 655b 305d 2c6c 656e 2873 7065  shape[0],len(spe
+00012b70: 6369 6573 5f6c 6973 7429 2929 2a54 5f73  cies_list)))*T_s
+00012b80: 7065 6369 6573 0a20 2020 2069 6620 6973  pecies.    if is
+00012b90: 696e 7374 616e 6365 2854 5f73 7065 6369  instance(T_speci
+00012ba0: 6573 2c6c 6973 7429 3a20 545f 7370 6563  es,list): T_spec
+00012bb0: 6965 733d 6e70 2e61 7272 6179 2854 5f73  ies=np.array(T_s
+00012bc0: 7065 6369 6573 290a 2020 2020 6966 2069  pecies).    if i
+00012bd0: 7369 6e73 7461 6e63 6528 6e5f 7370 6563  sinstance(n_spec
+00012be0: 6965 732c 6c69 7374 293a 206e 5f73 7065  ies,list): n_spe
+00012bf0: 6369 6573 3d6e 702e 6172 7261 7928 6e5f  cies=np.array(n_
+00012c00: 7370 6563 6965 7329 0a20 2020 2069 6620  species).    if 
+00012c10: 6e70 2e61 7272 6179 2854 5f73 7065 6369  np.array(T_speci
+00012c20: 6573 292e 7369 7a65 3d3d 6c65 6e28 7370  es).size==len(sp
+00012c30: 6563 6965 735f 6c69 7374 293a 0a20 2020  ecies_list):.   
+00012c40: 2020 2020 2054 5f73 7065 6369 6573 5f74       T_species_t
+00012c50: 656d 703d 6e70 2e6f 6e65 7328 2864 7a2e  emp=np.ones((dz.
+00012c60: 7368 6170 655b 305d 2c6c 656e 2873 7065  shape[0],len(spe
+00012c70: 6369 6573 5f6c 6973 7429 2929 0a20 2020  cies_list))).   
+00012c80: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+00012c90: 6e67 6528 6c65 6e28 7370 6563 6965 735f  nge(len(species_
+00012ca0: 6c69 7374 2929 3a0a 2020 2020 2020 2020  list)):.        
+00012cb0: 2020 2020 545f 7370 6563 6965 735f 7465      T_species_te
+00012cc0: 6d70 5b3a 2c69 5d3d 545f 7370 6563 6965  mp[:,i]=T_specie
+00012cd0: 735b 695d 0a20 2020 2020 2020 2054 5f73  s[i].        T_s
+00012ce0: 7065 6369 6573 3d54 5f73 7065 6369 6573  pecies=T_species
+00012cf0: 5f74 656d 702a 312e 3030 0a20 2020 2069  _temp*1.00.    i
+00012d00: 6620 6e70 2e61 7272 6179 286e 5f73 7065  f np.array(n_spe
+00012d10: 6369 6573 292e 7369 7a65 3d3d 6c65 6e28  cies).size==len(
+00012d20: 7370 6563 6965 735f 6c69 7374 293a 0a20  species_list):. 
+00012d30: 2020 2020 2020 206e 5f73 7065 6369 6573         n_species
+00012d40: 5f74 656d 703d 6e70 2e6f 6e65 7328 2864  _temp=np.ones((d
+00012d50: 7a2e 7368 6170 655b 305d 2c6c 656e 2873  z.shape[0],len(s
+00012d60: 7065 6369 6573 5f6c 6973 7429 2929 0a20  pecies_list))). 
+00012d70: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+00012d80: 7261 6e67 6528 6c65 6e28 7370 6563 6965  range(len(specie
+00012d90: 735f 6c69 7374 2929 3a0a 2020 2020 2020  s_list)):.      
+00012da0: 2020 2020 2020 6e5f 7370 6563 6965 735f        n_species_
+00012db0: 7465 6d70 5b3a 2c69 5d3d 6e5f 7370 6563  temp[:,i]=n_spec
+00012dc0: 6965 735b 695d 0a20 2020 2020 2020 206e  ies[i].        n
+00012dd0: 5f73 7065 6369 6573 3d6e 5f73 7065 6369  _species=n_speci
+00012de0: 6573 5f74 656d 702a 312e 3030 0a0a 2020  es_temp*1.00..  
+00012df0: 2020 7769 7468 206f 7065 6e28 6669 6c65    with open(file
+00012e00: 6e61 6d65 2c27 7727 2920 6173 2066 3a0a  name,'w') as f:.
+00012e10: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
+00012e20: 6627 7b6c 656e 2864 7a29 3a64 7d5c 6e27  f'{len(dz):d}\n'
+00012e30: 290a 2020 2020 2020 2020 662e 7772 6974  ).        f.writ
+00012e40: 6528 6627 7b6c 656e 2873 7065 6369 6573  e(f'{len(species
+00012e50: 5f6c 6973 7429 3a64 7d5c 6e27 290a 2020  _list):d}\n').  
+00012e60: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+00012e70: 616e 6765 286c 656e 2873 7065 6369 6573  ange(len(species
+00012e80: 5f6c 6973 7429 293a 0a20 2020 2020 2020  _list)):.       
+00012e90: 2020 2020 2066 2e77 7269 7465 2873 7065       f.write(spe
+00012ea0: 6369 6573 5f6c 6973 745b 695d 2b27 5c6e  cies_list[i]+'\n
+00012eb0: 2729 0a20 2020 2020 2020 2066 6f72 2069  ').        for i
+00012ec0: 2069 6e20 7261 6e67 6528 6c65 6e28 647a   in range(len(dz
+00012ed0: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+00012ee0: 7374 7269 6e67 3d27 270a 2020 2020 2020  string=''.      
+00012ef0: 2020 2020 2020 7374 7269 6e67 2b3d 6627        string+=f'
+00012f00: 7b69 2b31 3a64 7d20 2027 0a20 2020 2020  {i+1:d}  '.     
+00012f10: 2020 2020 2020 2073 7472 696e 672b 3d66         string+=f
+00012f20: 277b 647a 5b69 5d3a 2e33 657d 2020 270a  '{dz[i]:.3e}  '.
+00012f30: 2020 2020 2020 2020 2020 2020 7374 7269              stri
+00012f40: 6e67 2b3d 6627 7b76 7475 7262 5b69 5d3a  ng+=f'{vturb[i]:
+00012f50: 2e33 667d 2020 270a 2020 2020 2020 2020  .3f}  '.        
+00012f60: 2020 2020 7374 7269 6e67 2b3d 6627 7b6e      string+=f'{n
+00012f70: 645b 695d 3a2e 3365 7d20 2027 0a20 2020  d[i]:.3e}  '.   
+00012f80: 2020 2020 2020 2020 2073 7472 696e 672b           string+
+00012f90: 3d66 277b 5464 5b69 5d3a 2e33 667d 2020  =f'{Td[i]:.3f}  
+00012fa0: 270a 2020 2020 2020 2020 2020 2020 666f  '.            fo
+00012fb0: 7220 6a20 696e 2072 616e 6765 286c 656e  r j in range(len
+00012fc0: 2873 7065 6369 6573 5f6c 6973 7429 293a  (species_list)):
+00012fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012fe0: 2073 7472 696e 672b 3d66 277b 6e5f 7370   string+=f'{n_sp
+00012ff0: 6563 6965 735b 692c 6a5d 3a2e 3365 7d20  ecies[i,j]:.3e} 
+00013000: 2027 0a20 2020 2020 2020 2020 2020 2066   '.            f
+00013010: 6f72 206a 2069 6e20 7261 6e67 6528 6c65  or j in range(le
+00013020: 6e28 7370 6563 6965 735f 6c69 7374 2929  n(species_list))
+00013030: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00013040: 2020 7374 7269 6e67 2b3d 6627 7b54 5f73    string+=f'{T_s
+00013050: 7065 6369 6573 5b69 2c6a 5d3a 2e33 667d  pecies[i,j]:.3f}
+00013060: 2020 270a 2020 2020 2020 2020 2020 2020    '.            
+00013070: 7374 7269 6e67 2b3d 6627 7b6e 4832 5b69  string+=f'{nH2[i
+00013080: 5d3a 2e33 657d 2020 270a 2020 2020 2020  ]:.3e}  '.      
+00013090: 2020 2020 2020 7374 7269 6e67 2b3d 6627        string+=f'
+000130a0: 7b6e 4849 5b69 5d3a 2e33 657d 2020 270a  {nHI[i]:.3e}  '.
+000130b0: 2020 2020 2020 2020 2020 2020 7374 7269              stri
+000130c0: 6e67 2b3d 6627 7b6e 4849 495b 695d 3a2e  ng+=f'{nHII[i]:.
+000130d0: 3365 7d20 2027 0a20 2020 2020 2020 2020  3e}  '.         
+000130e0: 2020 2073 7472 696e 672b 3d66 277b 6e48     string+=f'{nH
+000130f0: 655b 695d 3a2e 3365 7d20 2027 0a20 2020  e[i]:.3e}  '.   
+00013100: 2020 2020 2020 2020 2073 7472 696e 672b           string+
+00013110: 3d66 277b 6e65 6c65 635b 695d 3a2e 3365  =f'{nelec[i]:.3e
+00013120: 7d20 2027 0a20 2020 2020 2020 2020 2020  }  '.           
+00013130: 2066 2e77 7269 7465 2873 7472 696e 672b   f.write(string+
+00013140: 275c 6e27 290a 2020 2020 2020 2020 662e  '\n').        f.
+00013150: 636c 6f73 6528 290a 0a0a 6465 6620 6c69  close()...def li
+00013160: 6e65 5f66 6c75 7828 6c31 2c6c 322c 7761  ne_flux(l1,l2,wa
+00013170: 7665 6c65 6e67 7468 2c66 6c75 7829 3a0a  velength,flux):.
+00013180: 2020 2020 2727 270a 2020 2020 556e 6974      '''.    Unit
+00013190: 733a 2052 6574 7572 6e20 6973 2069 6e20  s: Return is in 
+000131a0: 7468 6520 7361 6d65 2075 6e69 7420 6173  the same unit as
+000131b0: 2069 6e70 7574 2e20 5b41 7373 756d 6564   input. [Assumed
+000131c0: 2074 6f20 6265 2069 6e20 6572 672f 732f   to be in erg/s/
+000131d0: 636d 322f 7372 5d20 6c31 2061 6e64 206c  cm2/sr] l1 and l
+000131e0: 3220 7361 6d65 2075 6e69 7420 6173 2077  2 same unit as w
+000131f0: 6176 656c 656e 6774 680a 0a20 2020 2052  avelength..    R
+00013200: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
+00013210: 2d2d 0a20 2020 2066 6c6f 6174 3a0a 2020  --.    float:.  
+00013220: 2020 2020 5375 6d20 6f66 2069 6e74 6567      Sum of integ
+00013230: 7261 7465 6420 6c69 6e65 2066 6c75 7820  rated line flux 
+00013240: 6265 7477 6565 6e20 7761 7665 6c65 6e67  between waveleng
+00013250: 7468 7320 6c31 2061 6e64 206c 322e 0a0a  ths l1 and l2...
+00013260: 2020 2020 2727 270a 2020 2020 6d61 736b      '''.    mask
+00013270: 3d28 7761 7665 6c65 6e67 7468 3e6c 3129  =(wavelength>l1)
+00013280: 2628 7761 7665 6c65 6e67 7468 3c3d 6c32  &(wavelength<=l2
+00013290: 290a 2020 2020 7265 7475 726e 206e 702e  ).    return np.
+000132a0: 7375 6d28 666c 7578 5b6d 6173 6b5d 290a  sum(flux[mask]).
+000132b0: 0a0a 6465 6620 6c69 6e65 5f66 6c75 7865  ..def line_fluxe
+000132c0: 7328 7769 6e64 6f77 732c 7761 7665 6c65  s(windows,wavele
+000132d0: 6e67 7468 2c66 6c75 7829 3a0a 2020 2020  ngth,flux):.    
+000132e0: 2727 270a 2020 2020 5265 7475 726e 3a20  '''.    Return: 
+000132f0: 6172 7261 7920 6f66 2073 756d 206f 6620  array of sum of 
+00013300: 696e 7465 6772 6174 6564 206c 696e 6520  integrated line 
+00013310: 666c 7578 2069 6e20 7761 7665 6c65 6e67  flux in waveleng
+00013320: 7468 2077 696e 646f 7773 2e0a 0a20 2020  th windows...   
+00013330: 2055 6e69 7473 3a20 5265 7475 726e 2069   Units: Return i
+00013340: 7320 696e 2074 6865 2073 616d 6520 756e  s in the same un
+00013350: 6974 2061 7320 696e 7075 742e 205b 4173  it as input. [As
+00013360: 7375 6d65 6420 746f 2062 6520 696e 2065  sumed to be in e
+00013370: 7267 2f73 2f63 6d32 2f73 725d 0a0a 2020  rg/s/cm2/sr]..  
+00013380: 2020 7769 6e64 6f77 733a 206c 6973 7420    windows: list 
+00013390: 6f66 2077 6176 656c 656e 6774 6820 6c69  of wavelength li
+000133a0: 6d69 7473 206f 6620 7769 6e64 6f77 732e  mits of windows.
+000133b0: 2045 7861 6d70 6c65 3a20 5b5b 3134 2c31   Example: [[14,1
+000133c0: 342e 355d 2c5b 3135 2c31 362e 325d 2c5b  4.5],[15,16.2],[
+000133d0: 3132 2e35 2c31 342e 315d 5d0a 2020 2020  12.5,14.1]].    
+000133e0: 2727 270a 2020 2020 463d 5b5d 0a20 2020  '''.    F=[].   
+000133f0: 2066 6f72 2057 2069 6e20 7769 6e64 6f77   for W in window
+00013400: 733a 0a20 2020 2020 2020 2046 2e61 7070  s:.        F.app
+00013410: 656e 6428 6c69 6e65 5f66 6c75 7828 575b  end(line_flux(W[
+00013420: 305d 2c57 5b31 5d2c 7761 7665 6c65 6e67  0],W[1],waveleng
+00013430: 7468 2c66 6c75 7829 290a 2020 2020 7265  th,flux)).    re
+00013440: 7475 726e 286e 702e 6172 7261 7928 4629  turn(np.array(F)
+00013450: 290a 0a0a 6465 6620 6c69 6e65 5f66 6c75  )...def line_flu
+00013460: 785f 7261 7469 6f73 2872 6174 696f 5f77  x_ratios(ratio_w
+00013470: 696e 646f 7773 2c77 6176 656c 656e 6774  indows,wavelengt
+00013480: 682c 666c 7578 293a 0a20 2020 2027 2727  h,flux):.    '''
+00013490: 0a20 2020 2052 6574 7572 6e3a 2049 6e74  .    Return: Int
+000134a0: 6567 7261 7465 6420 6c69 6e65 2066 6c75  egrated line flu
+000134b0: 7820 7261 7469 6f73 2062 6574 7765 656e  x ratios between
+000134c0: 2077 6176 656c 656e 6774 6873 206c 3120   wavelengths l1 
+000134d0: 616e 6420 6c32 2e0a 0a20 2020 2055 6e69  and l2...    Uni
+000134e0: 743a 2052 6574 7572 6e20 6861 7320 6e6f  t: Return has no
+000134f0: 2075 6e69 742e 205b 496e 7075 7420 6973   unit. [Input is
+00013500: 2061 7373 756d 6564 2074 6f20 6265 2069   assumed to be i
+00013510: 6e20 6572 672f 732f 636d 322f 7372 5d0a  n erg/s/cm2/sr].
+00013520: 0a20 2020 2072 6174 696f 5f77 696e 646f  .    ratio_windo
+00013530: 7773 3a20 6c69 7374 206f 6620 7761 7665  ws: list of wave
+00013540: 6c65 6e67 7468 2077 696e 646f 7773 2e20  length windows. 
+00013550: 4578 616d 706c 653a 205b 5b5b 3134 2c31  Example: [[[14,1
+00013560: 342e 355d 2c5b 3135 2c31 362e 325d 5d2c  4.5],[15,16.2]],
+00013570: 5b5b 3132 2e35 2c31 342e 315d 2c5b 3133  [[12.5,14.1],[13
+00013580: 2e34 2c31 332e 385d 5d5d 0a20 2020 2027  .4,13.8]]].    '
+00013590: 2727 0a20 2020 2052 3d5b 5d0a 2020 2020  ''.    R=[].    
+000135a0: 666f 7220 7769 6e64 6f77 2069 6e20 7261  for window in ra
+000135b0: 7469 6f5f 7769 6e64 6f77 733a 0a20 2020  tio_windows:.   
+000135c0: 2020 2020 2046 3d6c 696e 655f 666c 7578       F=line_flux
+000135d0: 6573 285b 7769 6e64 6f77 5b30 5d2c 7769  es([window[0],wi
+000135e0: 6e64 6f77 5b31 5d5d 2c77 6176 656c 656e  ndow[1]],wavelen
+000135f0: 6774 682c 666c 7578 290a 2020 2020 2020  gth,flux).      
+00013600: 2020 522e 6170 7065 6e64 2846 5b31 5d2f    R.append(F[1]/
+00013610: 465b 305d 290a 2020 2020 7265 7475 726e  F[0]).    return
+00013620: 286e 702e 6172 7261 7928 5229 290a 0a0a  (np.array(R))...
+00013630: 6465 6620 6c69 6e65 5f66 6c75 785f 7072  def line_flux_pr
+00013640: 6f64 7563 7473 2870 726f 6475 6374 5f77  oducts(product_w
+00013650: 696e 646f 7773 2c77 6176 656c 656e 6774  indows,wavelengt
+00013660: 682c 666c 7578 293a 0a20 2020 2027 2727  h,flux):.    '''
+00013670: 0a20 2020 2052 6574 7572 6e3a 2049 6e74  .    Return: Int
+00013680: 6567 7261 7465 6420 6c69 6e65 2066 6c75  egrated line flu
+00013690: 7820 7072 6f64 7563 7473 2062 6574 7765  x products betwe
+000136a0: 656e 2077 6176 656c 656e 6774 6873 206c  en wavelengths l
+000136b0: 3120 616e 6420 6c32 2e0a 0a20 2020 2055  1 and l2...    U
+000136c0: 6e69 743a 2052 6574 7572 6e20 756e 6974  nit: Return unit
+000136d0: 2069 7320 6f75 7470 7574 2075 6e69 7473   is output units
+000136e0: 2073 7175 6172 6564 2e20 5b49 6e70 7574   squared. [Input
+000136f0: 2069 7320 6173 7375 6d65 6420 746f 2062   is assumed to b
+00013700: 6520 696e 2065 7267 2f73 2f63 6d32 2f73  e in erg/s/cm2/s
+00013710: 725d 0a0a 2020 2020 7072 6f64 7563 745f  r]..    product_
+00013720: 7769 6e64 6f77 733a 206c 6973 7420 6f66  windows: list of
+00013730: 2077 6176 656c 656e 6774 6820 7769 6e64   wavelength wind
+00013740: 6f77 732e 2045 7861 6d70 6c65 3a20 5b5b  ows. Example: [[
+00013750: 5b31 342c 3134 2e35 5d2c 5b31 352c 3136  [14,14.5],[15,16
+00013760: 2e32 5d5d 2c5b 5b31 322e 352c 3134 2e31  .2]],[[12.5,14.1
+00013770: 5d2c 5b31 332e 342c 3133 2e38 5d5d 5d0a  ],[13.4,13.8]]].
+00013780: 2020 2020 2727 270a 2020 2020 523d 5b5d      '''.    R=[]
+00013790: 0a20 2020 2066 6f72 2077 696e 646f 7720  .    for window 
+000137a0: 696e 2070 726f 6475 6374 5f77 696e 646f  in product_windo
+000137b0: 7773 3a0a 2020 2020 2020 2020 463d 6c69  ws:.        F=li
+000137c0: 6e65 5f66 6c75 7865 7328 5b77 696e 646f  ne_fluxes([windo
+000137d0: 775b 305d 2c77 696e 646f 775b 315d 5d2c  w[0],window[1]],
+000137e0: 7761 7665 6c65 6e67 7468 2c66 6c75 7829  wavelength,flux)
+000137f0: 0a20 2020 2020 2020 2052 2e61 7070 656e  .        R.appen
+00013800: 6428 465b 315d 2a46 5b30 5d29 0a20 2020  d(F[1]*F[0]).   
+00013810: 2072 6574 7572 6e28 6e70 2e61 7272 6179   return(np.array
+00013820: 2852 2929 0a0a 0a64 6566 2073 7065 6374  (R))...def spect
+00013830: 7261 6c5f 666c 7578 286c 312c 6c32 2c77  ral_flux(l1,l2,w
+00013840: 6176 656c 656e 6774 682c 666c 7578 293a  avelength,flux):
+00013850: 0a20 2020 2027 2727 0a20 2020 2055 6e69  .    '''.    Uni
+00013860: 743a 2052 6574 7572 6e20 696e 205b 6572  t: Return in [er
+00013870: 672f 732f 636d 325d 2061 6e64 2069 6e70  g/s/cm2] and inp
+00013880: 7574 2069 7320 696e 205b 4a79 5d20 6c31  ut is in [Jy] l1
+00013890: 2c20 6c32 2c20 616e 6420 7761 7665 6c65  , l2, and wavele
+000138a0: 6e67 7468 2069 6e20 6d69 6372 6f6e 730a  ngth in microns.
+000138b0: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
+000138c0: 202d 2d2d 2d2d 2d2d 0a20 2020 2066 6c6f   -------.    flo
+000138d0: 6174 3a0a 2020 2020 2020 5375 6d20 6f66  at:.      Sum of
+000138e0: 2069 6e74 6567 7261 7465 6420 6c69 6e65   integrated line
+000138f0: 2066 6c75 7820 6265 7477 6565 6e20 7761   flux between wa
+00013900: 7665 6c65 6e67 7468 7320 6c31 2061 6e64  velengths l1 and
+00013910: 206c 322e 0a0a 2020 2020 2727 270a 2020   l2...    '''.  
+00013920: 2020 666c 7578 3d66 6c75 782a 3165 2d32    flux=flux*1e-2
+00013930: 3320 2023 2043 6f6e 7665 7274 696e 6720  3  # Converting 
+00013940: 4a79 2074 6f20 6572 672e 73e2 8892 312e  Jy to erg.s...1.
+00013950: 636d e288 9232 2e48 7ae2 8892 310a 2020  cm...2.Hz...1.  
+00013960: 2020 7761 7665 6c65 6e67 7468 3d77 6176    wavelength=wav
+00013970: 656c 656e 6774 682a 3165 2d34 2020 2320  elength*1e-4  # 
+00013980: 436f 6e76 6572 7469 6e67 206d 6963 726f  Converting micro
+00013990: 6e73 2074 6f20 636d 0a20 2020 2066 6c75  ns to cm.    flu
+000139a0: 783d 666c 7578 5b6e 702e 6172 6773 6f72  x=flux[np.argsor
+000139b0: 7428 7761 7665 6c65 6e67 7468 295d 0a20  t(wavelength)]. 
+000139c0: 2020 2077 6176 656c 656e 6774 683d 7761     wavelength=wa
+000139d0: 7665 6c65 6e67 7468 5b6e 702e 6172 6773  velength[np.args
+000139e0: 6f72 7428 7761 7665 6c65 6e67 7468 295d  ort(wavelength)]
+000139f0: 0a20 2020 206c 313d 6c31 2a31 652d 3420  .    l1=l1*1e-4 
+00013a00: 2023 2043 6f6e 7665 7274 696e 6720 6d69   # Converting mi
+00013a10: 6372 6f6e 7320 746f 2063 6d0a 2020 2020  crons to cm.    
+00013a20: 6c32 3d6c 322a 3165 2d34 2020 2320 436f  l2=l2*1e-4  # Co
+00013a30: 6e76 6572 7469 6e67 206d 6963 726f 6e73  nverting microns
+00013a40: 2074 6f20 636d 0a20 2020 2063 5f63 6d73   to cm.    c_cms
+00013a50: 3d63 2a31 6532 2020 2320 436f 6e76 6572  =c*1e2  # Conver
+00013a60: 7469 6e67 206d 2f73 2074 6f20 636d 2f73  ting m/s to cm/s
+00013a70: 0a20 2020 206d 6173 6b3d 2877 6176 656c  .    mask=(wavel
+00013a80: 656e 6774 683e 6c31 2926 2877 6176 656c  ength>l1)&(wavel
+00013a90: 656e 6774 683c 3d6c 3229 0a20 2020 2077  ength<=l2).    w
+00013aa0: 6176 653d 7761 7665 6c65 6e67 7468 5b6d  ave=wavelength[m
+00013ab0: 6173 6b5d 0a20 2020 2023 2077 6176 6531  ask].    # wave1
+00013ac0: 2020 2020 2020 3d20 6e70 2e72 6f6c 6c28        = np.roll(
+00013ad0: 7761 7665 6c65 6e67 7468 2c31 295b 6d61  wavelength,1)[ma
+00013ae0: 736b 5d0a 2020 2020 2320 7761 7665 3120  sk].    # wave1 
+00013af0: 2020 2020 203d 2031 302a 2a28 286e 702e       = 10**((np.
+00013b00: 6c6f 6731 3028 7761 7665 292b 6e70 2e6c  log10(wave)+np.l
+00013b10: 6f67 3130 2877 6176 6531 2929 2f32 290a  og10(wave1))/2).
+00013b20: 2020 2020 2320 7761 7665 3220 2020 2020      # wave2     
+00013b30: 203d 206e 702e 726f 6c6c 2877 6176 656c   = np.roll(wavel
+00013b40: 656e 6774 682c 2d31 295b 6d61 736b 5d0a  ength,-1)[mask].
+00013b50: 2020 2020 2320 7761 7665 3220 2020 2020      # wave2     
+00013b60: 203d 2031 302a 2a28 286e 702e 6c6f 6731   = 10**((np.log1
+00013b70: 3028 7761 7665 292b 6e70 2e6c 6f67 3130  0(wave)+np.log10
+00013b80: 2877 6176 6532 2929 2f32 290a 2020 2020  (wave2))/2).    
+00013b90: 2320 646e 7520 2020 2020 2020 203d 2063  # dnu        = c
+00013ba0: 2a28 7761 7665 322d 7761 7665 3129 2f77  *(wave2-wave1)/w
+00013bb0: 6176 652a 2a32 2a31 6532 0a20 2020 2077  ave**2*1e2.    w
+00013bc0: 6176 6531 3d6e 702e 726f 6c6c 2877 6176  ave1=np.roll(wav
+00013bd0: 656c 656e 6774 682c 3129 5b6d 6173 6b5d  elength,1)[mask]
+00013be0: 0a20 2020 2077 6176 6532 3d6e 702e 726f  .    wave2=np.ro
+00013bf0: 6c6c 2877 6176 656c 656e 6774 682c 2d31  ll(wavelength,-1
+00013c00: 295b 6d61 736b 5d0a 2020 2020 646e 753d  )[mask].    dnu=
+00013c10: 2863 5f63 6d73 2a28 312f 7761 7665 312d  (c_cms*(1/wave1-
+00013c20: 312f 7761 7665 3229 2f32 290a 2020 2020  1/wave2)/2).    
+00013c30: 7265 7475 726e 286e 702e 7375 6d28 666c  return(np.sum(fl
+00013c40: 7578 5b6d 6173 6b5d 2a64 6e75 2929 0a0a  ux[mask]*dnu))..
+00013c50: 0a64 6566 2073 7065 6374 7261 6c5f 666c  .def spectral_fl
+00013c60: 7578 6573 2877 696e 646f 7773 2c77 6176  uxes(windows,wav
+00013c70: 656c 656e 6774 682c 666c 7578 293a 0a20  elength,flux):. 
+00013c80: 2020 2027 2727 0a20 2020 2052 6574 7572     '''.    Retur
+00013c90: 6e3a 2053 756d 206f 6620 696e 7465 6772  n: Sum of integr
+00013ca0: 6174 6564 206c 696e 6520 666c 7578 2062  ated line flux b
+00013cb0: 6574 7765 656e 2077 6176 656c 656e 6774  etween wavelengt
+00013cc0: 6820 7769 6e64 6f77 732e 0a0a 2020 2020  h windows...    
+00013cd0: 556e 6974 3a20 7265 7475 726e 2069 7320  Unit: return is 
+00013ce0: 696e 205b 6572 672f 732f 636d 325d 2061  in [erg/s/cm2] a
+00013cf0: 6e64 2069 6e70 7574 2069 7320 696e 205b  nd input is in [
+00013d00: 4a79 5d0a 0a20 2020 2077 696e 646f 7773  Jy]..    windows
+00013d10: 3a20 6c69 7374 206f 6620 7761 7665 6c65  : list of wavele
+00013d20: 6e67 7468 206c 696d 6974 7320 286d 6963  ngth limits (mic
+00013d30: 726f 6e73 2920 6f66 2077 696e 646f 7773  rons) of windows
+00013d40: 2e20 4578 616d 706c 653a 205b 5b31 342c  . Example: [[14,
+00013d50: 3134 2e35 5d2c 5b31 352c 3136 2e32 5d2c  14.5],[15,16.2],
+00013d60: 5b31 322e 352c 3134 2e31 5d5d 0a20 2020  [12.5,14.1]].   
+00013d70: 2027 2727 0a20 2020 2046 3d5b 5d0a 2020   '''.    F=[].  
+00013d80: 2020 666f 7220 5720 696e 2077 696e 646f    for W in windo
+00013d90: 7773 3a0a 2020 2020 2020 2020 462e 6170  ws:.        F.ap
+00013da0: 7065 6e64 2873 7065 6374 7261 6c5f 666c  pend(spectral_fl
+00013db0: 7578 2857 5b30 5d2c 575b 315d 2c77 6176  ux(W[0],W[1],wav
+00013dc0: 656c 656e 6774 682c 666c 7578 2929 0a20  elength,flux)). 
+00013dd0: 2020 2072 6574 7572 6e28 6e70 2e61 7272     return(np.arr
+00013de0: 6179 2846 2929 0a0a 0a64 6566 2073 7065  ay(F))...def spe
+00013df0: 6374 7261 6c5f 666c 7578 5f72 6174 696f  ctral_flux_ratio
+00013e00: 7328 7261 7469 6f5f 7769 6e64 6f77 732c  s(ratio_windows,
+00013e10: 7761 7665 6c65 6e67 7468 2c66 6c75 7829  wavelength,flux)
+00013e20: 3a0a 2020 2020 2727 270a 2020 2020 5265  :.    '''.    Re
+00013e30: 7475 726e 3a20 5370 6563 7472 616c 2069  turn: Spectral i
+00013e40: 6e74 6567 7261 7465 6420 666c 7578 2072  ntegrated flux r
+00013e50: 6174 696f 7320 6265 7477 6565 6e20 7761  atios between wa
+00013e60: 7665 6c65 6e67 7468 2077 696e 646f 7773  velength windows
+00013e70: 2e0a 0a20 2020 2055 6e69 7473 3a20 5265  ...    Units: Re
+00013e80: 7475 726e 2069 7320 7769 7468 6f75 7420  turn is without 
+00013e90: 756e 6974 7320 616e 6420 696e 7075 7420  units and input 
+00013ea0: 6973 2069 6e20 5b4a 795d 0a0a 2020 2020  is in [Jy]..    
+00013eb0: 7261 7469 6f5f 7769 6e64 6f77 733a 206c  ratio_windows: l
+00013ec0: 6973 7420 6f66 2077 6176 656c 656e 6774  ist of wavelengt
+00013ed0: 6820 286d 6963 726f 6e73 2920 7769 6e64  h (microns) wind
+00013ee0: 6f77 732e 2045 7861 6d70 6c65 3a20 5b5b  ows. Example: [[
+00013ef0: 5b31 342c 3134 2e35 5d2c 5b31 352c 3136  [14,14.5],[15,16
+00013f00: 2e32 5d5d 2c5b 5b31 322e 352c 3134 2e31  .2]],[[12.5,14.1
+00013f10: 5d2c 5b31 332e 342c 3133 2e38 5d5d 5d0a  ],[13.4,13.8]]].
+00013f20: 2020 2020 2727 270a 2020 2020 523d 5b5d      '''.    R=[]
+00013f30: 0a20 2020 2066 6f72 2077 696e 646f 7720  .    for window 
+00013f40: 696e 2072 6174 696f 5f77 696e 646f 7773  in ratio_windows
+00013f50: 3a0a 2020 2020 2020 2020 463d 7370 6563  :.        F=spec
+00013f60: 7472 616c 5f66 6c75 7865 7328 5b77 696e  tral_fluxes([win
+00013f70: 646f 775b 305d 2c77 696e 646f 775b 315d  dow[0],window[1]
+00013f80: 5d2c 7761 7665 6c65 6e67 7468 2c66 6c75  ],wavelength,flu
+00013f90: 7829 0a20 2020 2020 2020 2052 2e61 7070  x).        R.app
+00013fa0: 656e 6428 465b 315d 2f46 5b30 5d29 0a20  end(F[1]/F[0]). 
+00013fb0: 2020 2072 6574 7572 6e28 6e70 2e61 7272     return(np.arr
+00013fc0: 6179 2852 2929 0a0a 0a64 6566 2073 7065  ay(R))...def spe
+00013fd0: 6374 7261 6c5f 666c 7578 5f70 726f 6475  ctral_flux_produ
+00013fe0: 6374 7328 7072 6f64 7563 745f 7769 6e64  cts(product_wind
+00013ff0: 6f77 732c 7761 7665 6c65 6e67 7468 2c66  ows,wavelength,f
+00014000: 6c75 7829 3a0a 2020 2020 2727 270a 2020  lux):.    '''.  
+00014010: 2020 5265 7475 726e 3a20 5072 6f64 7563    Return: Produc
+00014020: 7473 206f 6620 7370 6563 7472 616c 2069  ts of spectral i
+00014030: 6e74 6567 7261 7465 6420 666c 7578 6573  ntegrated fluxes
+00014040: 2062 6574 7765 656e 2077 6176 656c 656e   between wavelen
+00014050: 6774 6820 7769 6e64 6f77 732e 0a0a 2020  gth windows...  
+00014060: 2020 556e 6974 733a 2052 6574 7572 6e20    Units: Return 
+00014070: 756e 6974 2069 7320 6f75 7470 7574 2075  unit is output u
+00014080: 6e69 7473 2073 7175 6172 6564 2061 6e64  nits squared and
+00014090: 2069 6e70 7574 2069 7320 696e 205b 4a79   input is in [Jy
+000140a0: 5d0a 0a20 2020 2070 726f 6475 6374 5f77  ]..    product_w
+000140b0: 696e 646f 7773 3a20 6c69 7374 206f 6620  indows: list of 
+000140c0: 7761 7665 6c65 6e67 7468 2028 6d69 6372  wavelength (micr
+000140d0: 6f6e 7329 2077 696e 646f 7773 2e20 4578  ons) windows. Ex
+000140e0: 616d 706c 653a 205b 5b5b 3134 2c31 342e  ample: [[[14,14.
+000140f0: 355d 2c5b 3135 2c31 362e 325d 5d2c 5b5b  5],[15,16.2]],[[
+00014100: 3132 2e35 2c31 342e 315d 2c5b 3133 2e34  12.5,14.1],[13.4
+00014110: 2c31 332e 385d 5d5d 0a20 2020 2027 2727  ,13.8]]].    '''
+00014120: 0a20 2020 2052 3d5b 5d0a 2020 2020 666f  .    R=[].    fo
+00014130: 7220 7769 6e64 6f77 2069 6e20 7072 6f64  r window in prod
+00014140: 7563 745f 7769 6e64 6f77 733a 0a20 2020  uct_windows:.   
+00014150: 2020 2020 2046 3d73 7065 6374 7261 6c5f       F=spectral_
+00014160: 666c 7578 6573 285b 7769 6e64 6f77 5b30  fluxes([window[0
+00014170: 5d2c 7769 6e64 6f77 5b31 5d5d 2c77 6176  ],window[1]],wav
+00014180: 656c 656e 6774 682c 666c 7578 290a 2020  elength,flux).  
+00014190: 2020 2020 2020 522e 6170 7065 6e64 2846        R.append(F
+000141a0: 5b31 5d2a 465b 305d 290a 2020 2020 7265  [1]*F[0]).    re
+000141b0: 7475 726e 286e 702e 6172 7261 7928 5229  turn(np.array(R)
+000141c0: 290a 0a0a 6465 6620 6368 6932 5f73 6c61  )...def chi2_sla
+000141d0: 6228 736c 6162 5f64 6174 612c 7370 6563  b(slab_data,spec
+000141e0: 7472 612c 7769 6e64 6f77 733d 5b5d 2c72  tra,windows=[],r
+000141f0: 6174 696f 5f77 696e 646f 7773 3d5b 5d2c  atio_windows=[],
+00014200: 7072 6f64 7563 745f 7769 6e64 6f77 733d  product_windows=
+00014210: 5b5d 2c52 6469 736b 3d6e 702e 6c6f 6773  [],Rdisk=np.logs
+00014220: 7061 6365 282d 322c 322c 3130 292c 6469  pace(-2,2,10),di
+00014230: 7374 616e 6365 3d31 3230 2c63 6f6e 766f  stance=120,convo
+00014240: 6c76 653d 4661 6c73 652c 4e4c 5445 3d46  lve=False,NLTE=F
+00014250: 616c 7365 2c73 686f 7274 5f66 6f72 6d61  alse,short_forma
+00014260: 743d 4661 6c73 6529 3a0a 2020 2020 2727  t=False):.    ''
+00014270: 270a 2020 2020 5265 7475 726e 7320 6368  '.    Returns ch
+00014280: 6932 2062 6173 6564 206f 6e20 7365 6c65  i2 based on sele
+00014290: 6374 6564 2073 7065 6374 7261 6c20 7769  cted spectral wi
+000142a0: 6e64 6f77 7320 6163 726f 7373 2064 6966  ndows across dif
+000142b0: 6665 7265 6e74 2065 6d69 7474 696e 6720  ferent emitting 
+000142c0: 6469 736b 2072 6164 6975 730a 0a20 2020  disk radius..   
+000142d0: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+000142e0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2073  ----------.    s
+000142f0: 6c61 625f 6461 7461 203a 2073 7472 696e  lab_data : strin
+00014300: 6720 6f72 2073 6c61 625f 6d6f 6465 6c20  g or slab_model 
+00014310: 696e 7374 616e 6365 0a20 2020 2020 2070  instance.      p
+00014320: 6174 6820 636f 7272 6573 706f 6e64 696e  ath correspondin
+00014330: 6720 746f 2061 2073 696e 676c 6520 736c  g to a single sl
+00014340: 6162 206d 6f64 656c 206f 7220 6120 7369  ab model or a si
+00014350: 6e67 6c65 2073 6c61 625f 6d6f 6465 6c20  ngle slab_model 
+00014360: 696e 7374 616e 6365 0a0a 2020 2020 7370  instance..    sp
+00014370: 6563 7472 6120 3a20 6e75 6d70 792e 6172  ectra : numpy.ar
+00014380: 7261 790a 2020 2020 2020 6e75 6d70 7920  ray.      numpy 
+00014390: 6172 7261 7920 7769 7468 2066 6972 7374  array with first
+000143a0: 2063 6f6c 756d 6e20 7468 6520 7761 7665   column the wave
+000143b0: 6c65 6e67 7468 2069 6e20 5b6d 6963 726f  length in [micro
+000143c0: 6e73 5d20 616e 6420 7365 636f 6e64 2063  ns] and second c
+000143d0: 6f6c 756d 6e20 666c 7578 2069 6e20 5b4a  olumn flux in [J
+000143e0: 795d 0a0a 2020 2020 7769 6e64 6f77 7320  y]..    windows 
+000143f0: 3a20 6172 7261 795f 6c69 6b65 0a20 2020  : array_like.   
+00014400: 2020 204c 6973 7420 6f66 2073 7065 6374     List of spect
+00014410: 7261 6c20 7769 6e64 6f77 7320 666f 7220  ral windows for 
+00014420: 6368 6932 2063 616c 6375 6c61 7469 6f6e  chi2 calculation
+00014430: 2028 7765 6967 6874 7320 6f70 7469 6f6e   (weights option
+00014440: 616c 292e 2046 6f72 6d61 7420 3a20 5b77  al). Format : [w
+00014450: 696e 646f 7731 2c77 696e 646f 7732 2c2e  indow1,window2,.
+00014460: 2e2e 2e5d 0a20 2020 2020 2057 696e 646f  ...].      Windo
+00014470: 7720 666f 726d 6174 3a20 5b6c 616d 6264  w format: [lambd
+00014480: 615f 302c 206c 616d 6264 615f 312c 2077  a_0, lambda_1, w
+00014490: 6569 6768 745d 2077 6569 6768 7420 6973  eight] weight is
+000144a0: 206f 7074 696f 6e61 6c2c 2075 7365 6420   optional, used 
+000144b0: 666f 7220 7765 6967 6874 6564 2063 6869  for weighted chi
+000144c0: 320a 2020 2020 2020 4578 616d 706c 6520  2.      Example 
+000144d0: 7769 7468 6f75 7420 7765 6967 6874 3a20  without weight: 
+000144e0: 5b5b 3134 2c31 342e 355d 2c5b 3135 2c31  [[14,14.5],[15,1
+000144f0: 362e 325d 2c5b 3132 2e35 2c31 342e 315d  6.2],[12.5,14.1]
+00014500: 5d0a 2020 2020 2020 4578 616d 706c 6520  ].      Example 
+00014510: 7769 7468 2077 6569 6768 743a 205b 5b31  with weight: [[1
+00014520: 342c 3134 2e35 2c32 5d2c 5b31 352c 3136  4,14.5,2],[15,16
+00014530: 2e32 2c35 5d2c 5b31 322e 352c 3134 2e31  .2,5],[12.5,14.1
+00014540: 2c31 5d5d 0a20 2020 2020 2057 6569 6768  ,1]].      Weigh
+00014550: 7473 2061 7265 2061 7574 6f6d 6174 6963  ts are automatic
+00014560: 616c 6c79 206e 6f72 6d61 6c69 7365 642c  ally normalised,
+00014570: 2073 6f20 7375 6d20 6f66 2077 6569 6768   so sum of weigh
+00014580: 7473 206e 6565 6420 6e6f 7420 6265 2031  ts need not be 1
+00014590: 0a0a 2020 2020 5264 6973 6b20 3a20 6172  ..    Rdisk : ar
+000145a0: 7261 795f 6c69 6b65 0a20 2020 2020 2052  ray_like.      R
+000145b0: 6164 6975 7320 636f 7272 6573 706f 6e64  adius correspond
+000145c0: 696e 6720 746f 2065 6d69 7474 696e 6720  ing to emitting 
+000145d0: 6172 6561 2069 6e20 6173 7472 6f6e 6f6d  area in astronom
+000145e0: 6963 616c 2075 6e69 7473 0a0a 2020 2020  ical units..    
+000145f0: 6469 7374 616e 6365 203a 2066 6c6f 6174  distance : float
+00014600: 0a20 2020 2020 2064 6973 7461 6e63 6520  .      distance 
+00014610: 6f66 2064 6973 6b20 696e 2070 6172 7365  of disk in parse
+00014620: 630a 0a20 2020 2063 6f6e 766f 6c76 6520  c..    convolve 
+00014630: 3a20 626f 6f6c 6561 6e0a 2020 2020 2020  : boolean.      
+00014640: 4966 2054 7275 652c 2074 6865 2063 6869  If True, the chi
+00014650: 3220 6973 2070 6572 666f 726d 6564 206f  2 is performed o
+00014660: 6e20 636f 6e76 6f6c 7665 6420 7370 6563  n convolved spec
+00014670: 7472 6120 616e 6420 6e6f 7420 6f6e 2069  tra and not on i
+00014680: 6e64 6976 6964 7561 6c20 6c69 6e65 730a  ndividual lines.
+00014690: 0a20 2020 204e 4c54 4520 3a20 626f 6f6c  .    NLTE : bool
+000146a0: 6561 6e0a 2020 2020 2020 6966 2054 7275  ean.      if Tru
+000146b0: 652c 204e 4c54 4520 666c 7578 2069 7320  e, NLTE flux is 
+000146c0: 7461 6b65 6e20 6672 6f6d 2074 6865 2073  taken from the s
+000146d0: 6c61 6220 6d6f 6465 6c2e 0a20 2020 2027  lab model..    '
+000146e0: 2727 0a20 2020 2061 7265 613d 6e70 2e70  ''.    area=np.p
+000146f0: 692a 2852 6469 736b 2a61 752f 6469 7374  i*(Rdisk*au/dist
+00014700: 616e 6365 2f70 6329 2a2a 320a 2020 2020  ance/pc)**2.    
+00014710: 6368 695f 6172 6561 3d6e 702e 7a65 726f  chi_area=np.zero
+00014720: 7328 286c 656e 2861 7265 6129 2929 0a20  s((len(area))). 
+00014730: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00014740: 2873 6c61 625f 6461 7461 2c73 7472 293a  (slab_data,str):
+00014750: 2073 6c61 625f 6461 7461 3d72 6561 645f   slab_data=read_
+00014760: 736c 6162 2873 6c61 625f 6461 7461 2c76  slab(slab_data,v
+00014770: 6572 626f 7365 3d46 616c 7365 2c73 686f  erbose=False,sho
+00014780: 7274 5f66 6f72 6d61 743d 7368 6f72 745f  rt_format=short_
+00014790: 666f 726d 6174 290a 2020 2020 6966 206c  format).    if l
+000147a0: 656e 2877 696e 646f 7773 293c 3020 616e  en(windows)<0 an
+000147b0: 6420 6c65 6e28 7261 7469 6f5f 7769 6e64  d len(ratio_wind
+000147c0: 6f77 7329 3c30 2061 6e64 206c 656e 2870  ows)<0 and len(p
+000147d0: 726f 6475 6374 5f77 696e 646f 7773 293c  roduct_windows)<
+000147e0: 303a 2072 6574 7572 6e20 6368 695f 6172  0: return chi_ar
+000147f0: 6561 0a20 2020 2069 6620 636f 6e76 6f6c  ea.    if convol
+00014800: 7665 3a20 2023 2074 6f20 6573 7469 6d61  ve:  # to estima
+00014810: 7465 2066 6c75 7820 6672 6f6d 2063 6f6e  te flux from con
+00014820: 766f 6c76 6564 2073 7065 6374 7261 0a20  volved spectra. 
+00014830: 2020 2020 2020 206c 6d69 6e2c 6c6d 6178         lmin,lmax
+00014840: 3d5b 5d2c 5b5d 0a20 2020 2020 2020 2069  =[],[].        i
+00014850: 6620 6c65 6e28 7769 6e64 6f77 7329 3e30  f len(windows)>0
+00014860: 3a0a 2020 2020 2020 2020 2020 2020 6c6d  :.            lm
+00014870: 696e 2e61 7070 656e 6428 6e70 2e61 6d69  in.append(np.ami
+00014880: 6e28 6e70 2e61 7272 6179 285b 5b69 5b30  n(np.array([[i[0
+00014890: 5d2c 695b 315d 5d20 666f 7220 6920 696e  ],i[1]] for i in
+000148a0: 2077 696e 646f 7773 5d29 2e66 6c61 7474   windows]).flatt
+000148b0: 656e 2829 2929 0a20 2020 2020 2020 2020  en())).         
+000148c0: 2020 206c 6d61 782e 6170 7065 6e64 286e     lmax.append(n
+000148d0: 702e 616d 6178 286e 702e 6172 7261 7928  p.amax(np.array(
+000148e0: 5b5b 695b 305d 2c69 5b31 5d5d 2066 6f72  [[i[0],i[1]] for
+000148f0: 2069 2069 6e20 7769 6e64 6f77 735d 292e   i in windows]).
+00014900: 666c 6174 7465 6e28 2929 290a 2020 2020  flatten())).    
+00014910: 2020 2020 6966 206c 656e 2872 6174 696f      if len(ratio
+00014920: 5f77 696e 646f 7773 293e 303a 0a20 2020  _windows)>0:.   
+00014930: 2020 2020 2020 2020 206c 6d69 6e2e 6170           lmin.ap
+00014940: 7065 6e64 286e 702e 616d 696e 286e 702e  pend(np.amin(np.
+00014950: 6172 7261 7928 5b5b 695b 305d 2c69 5b31  array([[i[0],i[1
+00014960: 5d5d 2066 6f72 2069 2069 6e20 7261 7469  ]] for i in rati
+00014970: 6f5f 7769 6e64 6f77 735d 292e 666c 6174  o_windows]).flat
+00014980: 7465 6e28 2929 290a 2020 2020 2020 2020  ten())).        
+00014990: 2020 2020 6c6d 6178 2e61 7070 656e 6428      lmax.append(
+000149a0: 6e70 2e61 6d61 7828 6e70 2e61 7272 6179  np.amax(np.array
+000149b0: 285b 5b69 5b30 5d2c 695b 315d 5d20 666f  ([[i[0],i[1]] fo
+000149c0: 7220 6920 696e 2072 6174 696f 5f77 696e  r i in ratio_win
+000149d0: 646f 7773 5d29 2e66 6c61 7474 656e 2829  dows]).flatten()
+000149e0: 2929 0a20 2020 2020 2020 2069 6620 6c65  )).        if le
+000149f0: 6e28 7072 6f64 7563 745f 7769 6e64 6f77  n(product_window
+00014a00: 7329 3e30 3a0a 2020 2020 2020 2020 2020  s)>0:.          
+00014a10: 2020 6c6d 696e 2e61 7070 656e 6428 6e70    lmin.append(np
+00014a20: 2e61 6d69 6e28 6e70 2e61 7272 6179 285b  .amin(np.array([
+00014a30: 5b69 5b30 5d2c 695b 315d 5d20 666f 7220  [i[0],i[1]] for 
+00014a40: 6920 696e 2070 726f 6475 6374 5f77 696e  i in product_win
+00014a50: 646f 7773 5d29 2e66 6c61 7474 656e 2829  dows]).flatten()
+00014a60: 2929 0a20 2020 2020 2020 2020 2020 206c  )).            l
+00014a70: 6d61 782e 6170 7065 6e64 286e 702e 616d  max.append(np.am
+00014a80: 6178 286e 702e 6172 7261 7928 5b5b 695b  ax(np.array([[i[
+00014a90: 305d 2c69 5b31 5d5d 2066 6f72 2069 2069  0],i[1]] for i i
+00014aa0: 6e20 7072 6f64 7563 745f 7769 6e64 6f77  n product_window
+00014ab0: 735d 292e 666c 6174 7465 6e28 2929 290a  s]).flatten())).
+00014ac0: 2020 2020 2020 2020 6c6d 696e 3d6e 702e          lmin=np.
+00014ad0: 616d 696e 286c 6d69 6e29 0a20 2020 2020  amin(lmin).     
+00014ae0: 2020 206c 6d61 783d 6e70 2e61 6d61 7828     lmax=np.amax(
+00014af0: 6c6d 6178 290a 2020 2020 2020 2020 736c  lmax).        sl
+00014b00: 6162 5f64 6174 612e 636f 6e76 6f6c 7665  ab_data.convolve
+00014b10: 2852 3d32 3030 302c 6c61 6d62 6461 5f30  (R=2000,lambda_0
+00014b20: 3d6c 6d69 6e2a 302e 392c 6c61 6d62 6461  =lmin*0.9,lambda
+00014b30: 5f6e 3d6c 6d61 782a 312e 312c 4e4c 5445  _n=lmax*1.1,NLTE
+00014b40: 3d4e 4c54 452c 7665 7262 6f73 653d 4661  =NLTE,verbose=Fa
+00014b50: 6c73 6529 0a20 2020 2020 2020 2069 6620  lse).        if 
+00014b60: 4e4c 5445 3a0a 2020 2020 2020 2020 2020  NLTE:.          
+00014b70: 2020 466d 6f64 656c 3d73 7065 6374 7261    Fmodel=spectra
+00014b80: 6c5f 666c 7578 6573 2877 696e 646f 7773  l_fluxes(windows
+00014b90: 2c73 6c61 625f 6461 7461 2e63 6f6e 7657  ,slab_data.convW
+00014ba0: 6176 656c 656e 6774 682c 736c 6162 5f64  avelength,slab_d
+00014bb0: 6174 612e 636f 6e76 4e4c 5445 666c 7578  ata.convNLTEflux
+00014bc0: 2a31 6532 3329 0a20 2020 2020 2020 2020  *1e23).         
+00014bd0: 2020 2052 6d6f 6465 6c3d 7370 6563 7472     Rmodel=spectr
+00014be0: 616c 5f66 6c75 785f 7261 7469 6f73 2872  al_flux_ratios(r
+00014bf0: 6174 696f 5f77 696e 646f 7773 2c73 6c61  atio_windows,sla
+00014c00: 625f 6461 7461 2e63 6f6e 7657 6176 656c  b_data.convWavel
+00014c10: 656e 6774 682c 736c 6162 5f64 6174 612e  ength,slab_data.
+00014c20: 636f 6e76 4e4c 5445 666c 7578 2a31 6532  convNLTEflux*1e2
+00014c30: 3329 0a20 2020 2020 2020 2020 2020 2050  3).            P
+00014c40: 6d6f 6465 6c3d 7370 6563 7472 616c 5f66  model=spectral_f
+00014c50: 6c75 785f 7072 6f64 7563 7473 2870 726f  lux_products(pro
+00014c60: 6475 6374 5f77 696e 646f 7773 2c73 6c61  duct_windows,sla
+00014c70: 625f 6461 7461 2e63 6f6e 7657 6176 656c  b_data.convWavel
+00014c80: 656e 6774 682c 736c 6162 5f64 6174 612e  ength,slab_data.
+00014c90: 636f 6e76 4e4c 5445 666c 7578 2a31 6532  convNLTEflux*1e2
+00014ca0: 3329 0a20 2020 2020 2020 2065 6c73 653a  3).        else:
+00014cb0: 0a20 2020 2020 2020 2020 2020 2046 6d6f  .            Fmo
+00014cc0: 6465 6c3d 7370 6563 7472 616c 5f66 6c75  del=spectral_flu
+00014cd0: 7865 7328 7769 6e64 6f77 732c 736c 6162  xes(windows,slab
+00014ce0: 5f64 6174 612e 636f 6e76 5761 7665 6c65  _data.convWavele
+00014cf0: 6e67 7468 2c73 6c61 625f 6461 7461 2e63  ngth,slab_data.c
+00014d00: 6f6e 764c 5445 666c 7578 2a31 6532 3329  onvLTEflux*1e23)
+00014d10: 0a20 2020 2020 2020 2020 2020 2052 6d6f  .            Rmo
+00014d20: 6465 6c3d 7370 6563 7472 616c 5f66 6c75  del=spectral_flu
+00014d30: 785f 7261 7469 6f73 2872 6174 696f 5f77  x_ratios(ratio_w
+00014d40: 696e 646f 7773 2c73 6c61 625f 6461 7461  indows,slab_data
+00014d50: 2e63 6f6e 7657 6176 656c 656e 6774 682c  .convWavelength,
+00014d60: 736c 6162 5f64 6174 612e 636f 6e76 4c54  slab_data.convLT
+00014d70: 4566 6c75 782a 3165 3233 290a 2020 2020  Eflux*1e23).    
+00014d80: 2020 2020 2020 2020 506d 6f64 656c 3d73          Pmodel=s
+00014d90: 7065 6374 7261 6c5f 666c 7578 5f70 726f  pectral_flux_pro
+00014da0: 6475 6374 7328 7072 6f64 7563 745f 7769  ducts(product_wi
+00014db0: 6e64 6f77 732c 736c 6162 5f64 6174 612e  ndows,slab_data.
+00014dc0: 636f 6e76 5761 7665 6c65 6e67 7468 2c73  convWavelength,s
+00014dd0: 6c61 625f 6461 7461 2e63 6f6e 764c 5445  lab_data.convLTE
+00014de0: 666c 7578 2a31 6532 3329 0a20 2020 2065  flux*1e23).    e
+00014df0: 6c73 653a 2020 2320 746f 2065 7374 696d  lse:  # to estim
+00014e00: 6174 6520 666c 7578 2066 726f 6d20 6c69  ate flux from li
+00014e10: 6e65 206c 6973 740a 2020 2020 2020 2020  ne list.        
+00014e20: 6966 204e 4c54 453a 0a20 2020 2020 2020  if NLTE:.       
+00014e30: 2020 2020 2074 3d27 464e 4c54 4527 0a20       t='FNLTE'. 
+00014e40: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00014e50: 2020 2020 2020 2020 2074 3d27 464c 5445           t='FLTE
+00014e60: 270a 2020 2020 2020 2020 6c69 6e65 6461  '.        lineda
+00014e70: 7461 3d73 6c61 625f 6461 7461 2e6c 696e  ta=slab_data.lin
+00014e80: 6564 6174 610a 2020 2020 2020 2020 6c69  edata.        li
+00014e90: 6e65 6461 7461 2e73 6f72 745f 7661 6c75  nedata.sort_valu
+00014ea0: 6573 2862 793d 5b27 4748 7a27 5d2c 6173  es(by=['GHz'],as
+00014eb0: 6365 6e64 696e 673d 4661 6c73 652c 696e  cending=False,in
+00014ec0: 706c 6163 653d 5472 7565 2c69 676e 6f72  place=True,ignor
+00014ed0: 655f 696e 6465 783d 5472 7565 290a 2020  e_index=True).  
+00014ee0: 2020 2020 2020 466d 6f64 656c 3d6c 696e        Fmodel=lin
+00014ef0: 655f 666c 7578 6573 2877 696e 646f 7773  e_fluxes(windows
+00014f00: 2c63 2f6c 696e 6564 6174 615b 2747 487a  ,c/linedata['GHz
+00014f10: 275d 2a31 652d 332c 6c69 6e65 6461 7461  ']*1e-3,linedata
+00014f20: 5b74 5d29 0a20 2020 2020 2020 2052 6d6f  [t]).        Rmo
+00014f30: 6465 6c3d 6c69 6e65 5f66 6c75 785f 7261  del=line_flux_ra
+00014f40: 7469 6f73 2872 6174 696f 5f77 696e 646f  tios(ratio_windo
+00014f50: 7773 2c63 2f6c 696e 6564 6174 615b 2747  ws,c/linedata['G
+00014f60: 487a 275d 2a31 652d 332c 6c69 6e65 6461  Hz']*1e-3,lineda
+00014f70: 7461 5b74 5d29 0a20 2020 2020 2020 2050  ta[t]).        P
+00014f80: 6d6f 6465 6c3d 6c69 6e65 5f66 6c75 785f  model=line_flux_
+00014f90: 7261 7469 6f73 2870 726f 6475 6374 5f77  ratios(product_w
+00014fa0: 696e 646f 7773 2c63 2f6c 696e 6564 6174  indows,c/linedat
+00014fb0: 615b 2747 487a 275d 2a31 652d 332c 6c69  a['GHz']*1e-3,li
+00014fc0: 6e65 6461 7461 5b74 5d29 0a20 2020 2046  nedata[t]).    F
+00014fd0: 6f62 7365 7276 6564 3d73 7065 6374 7261  observed=spectra
+00014fe0: 6c5f 666c 7578 6573 2877 696e 646f 7773  l_fluxes(windows
+00014ff0: 2c73 7065 6374 7261 5b3a 2c30 5d2c 7370  ,spectra[:,0],sp
+00015000: 6563 7472 615b 3a2c 315d 290a 2020 2020  ectra[:,1]).    
+00015010: 526f 6273 6572 7665 643d 7370 6563 7472  Robserved=spectr
+00015020: 616c 5f66 6c75 785f 7261 7469 6f73 2872  al_flux_ratios(r
+00015030: 6174 696f 5f77 696e 646f 7773 2c73 7065  atio_windows,spe
+00015040: 6374 7261 5b3a 2c30 5d2c 7370 6563 7472  ctra[:,0],spectr
+00015050: 615b 3a2c 315d 290a 2020 2020 506f 6273  a[:,1]).    Pobs
+00015060: 6572 7665 643d 7370 6563 7472 616c 5f66  erved=spectral_f
+00015070: 6c75 785f 7072 6f64 7563 7473 2870 726f  lux_products(pro
+00015080: 6475 6374 5f77 696e 646f 7773 2c73 7065  duct_windows,spe
+00015090: 6374 7261 5b3a 2c30 5d2c 7370 6563 7472  ctra[:,0],spectr
+000150a0: 615b 3a2c 315d 290a 2020 2020 6e6f 726d  a[:,1]).    norm
+000150b0: 5f66 6163 746f 723d 300a 2020 2020 6966  _factor=0.    if
+000150c0: 206c 656e 2877 696e 646f 7773 293e 303a   len(windows)>0:
+000150d0: 0a20 2020 2020 2020 2061 7265 615f 3264  .        area_2d
+000150e0: 3d6e 702e 6473 7461 636b 285b 6172 6561  =np.dstack([area
+000150f0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00015100: 6c65 6e28 7769 6e64 6f77 7329 295d 292e  len(windows))]).
+00015110: 7371 7565 657a 6528 292e 7265 7368 6170  squeeze().reshap
+00015120: 6528 286c 656e 2861 7265 6129 2c6c 656e  e((len(area),len
+00015130: 2877 696e 646f 7773 2929 290a 2020 2020  (windows))).    
+00015140: 2020 2020 466d 6f64 656c 5f32 643d 6e70      Fmodel_2d=np
+00015150: 2e64 7374 6163 6b28 5b46 6d6f 6465 6c20  .dstack([Fmodel 
+00015160: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
+00015170: 656e 2861 7265 6129 295d 292e 7371 7565  en(area))]).sque
+00015180: 657a 6528 292e 542e 7265 7368 6170 6528  eze().T.reshape(
+00015190: 286c 656e 2861 7265 6129 2c6c 656e 2877  (len(area),len(w
+000151a0: 696e 646f 7773 2929 290a 2020 2020 2020  indows))).      
+000151b0: 2020 466f 6273 6572 7665 645f 3264 3d6e    Fobserved_2d=n
+000151c0: 702e 6473 7461 636b 285b 466f 6273 6572  p.dstack([Fobser
+000151d0: 7665 6420 666f 7220 6920 696e 2072 616e  ved for i in ran
+000151e0: 6765 286c 656e 2861 7265 6129 295d 292e  ge(len(area))]).
+000151f0: 7371 7565 657a 6528 292e 542e 7265 7368  squeeze().T.resh
+00015200: 6170 6528 286c 656e 2861 7265 6129 2c6c  ape((len(area),l
+00015210: 656e 2877 696e 646f 7773 2929 290a 2020  en(windows))).  
+00015220: 2020 2020 2020 6966 206c 656e 2877 696e        if len(win
+00015230: 646f 7773 5b30 5d29 3d3d 333a 2020 2320  dows[0])==3:  # 
+00015240: 7765 6967 6874 6564 2063 6869 320a 2020  weighted chi2.  
+00015250: 2020 2020 2020 2020 2020 7769 6e64 6f77            window
+00015260: 735f 7765 6967 6874 733d 6e70 2e61 7272  s_weights=np.arr
+00015270: 6179 285b 7769 6e64 6f77 735b 6b5d 5b32  ay([windows[k][2
+00015280: 5d20 666f 7220 6b20 696e 2072 616e 6765  ] for k in range
+00015290: 286c 656e 2877 696e 646f 7773 2929 5d29  (len(windows))])
+000152a0: 0a20 2020 2020 2020 2020 2020 2077 696e  .            win
+000152b0: 646f 7773 5f77 6569 6768 7473 5f32 643d  dows_weights_2d=
+000152c0: 6e70 2e64 7374 6163 6b28 5b77 696e 646f  np.dstack([windo
+000152d0: 7773 5f77 6569 6768 7473 2066 6f72 2069  ws_weights for i
+000152e0: 2069 6e20 7261 6e67 6528 6c65 6e28 6172   in range(len(ar
+000152f0: 6561 2929 5d29 2e73 7175 6565 7a65 2829  ea))]).squeeze()
+00015300: 2e54 2e72 6573 6861 7065 2828 6c65 6e28  .T.reshape((len(
+00015310: 6172 6561 292c 6c65 6e28 7769 6e64 6f77  area),len(window
+00015320: 735f 7765 6967 6874 7329 2929 0a20 2020  s_weights))).   
+00015330: 2020 2020 2020 2020 2063 6869 5f61 7265           chi_are
+00015340: 612b 3d6e 702e 7375 6d28 2828 466d 6f64  a+=np.sum(((Fmod
+00015350: 656c 5f32 642a 6172 6561 5f32 642d 466f  el_2d*area_2d-Fo
+00015360: 6273 6572 7665 645f 3264 292f 466f 6273  bserved_2d)/Fobs
+00015370: 6572 7665 645f 3264 292a 2a32 2a77 696e  erved_2d)**2*win
+00015380: 646f 7773 5f77 6569 6768 7473 5f32 642c  dows_weights_2d,
+00015390: 6178 6973 3d31 290a 2020 2020 2020 2020  axis=1).        
+000153a0: 2020 2020 6e6f 726d 5f66 6163 746f 722b      norm_factor+
+000153b0: 3d6e 702e 7375 6d28 7769 6e64 6f77 735f  =np.sum(windows_
+000153c0: 7765 6967 6874 7329 0a20 2020 2020 2020  weights).       
+000153d0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000153e0: 2020 2063 6869 5f61 7265 612b 3d6e 702e     chi_area+=np.
+000153f0: 7375 6d28 2828 466d 6f64 656c 5f32 642a  sum(((Fmodel_2d*
+00015400: 6172 6561 5f32 642d 466f 6273 6572 7665  area_2d-Fobserve
+00015410: 645f 3264 292f 466f 6273 6572 7665 645f  d_2d)/Fobserved_
+00015420: 3264 292a 2a32 2c61 7869 733d 3129 0a20  2d)**2,axis=1). 
+00015430: 2020 2020 2020 2020 2020 206e 6f72 6d5f             norm_
+00015440: 6661 6374 6f72 2b3d 6c65 6e28 7769 6e64  factor+=len(wind
+00015450: 6f77 7329 0a20 2020 2069 6620 6c65 6e28  ows).    if len(
+00015460: 7261 7469 6f5f 7769 6e64 6f77 7329 3e30  ratio_windows)>0
+00015470: 3a0a 2020 2020 2020 2020 526d 6f64 656c  :.        Rmodel
+00015480: 5f32 643d 6e70 2e64 7374 6163 6b28 5b52  _2d=np.dstack([R
+00015490: 6d6f 6465 6c20 666f 7220 6920 696e 2072  model for i in r
+000154a0: 616e 6765 286c 656e 2861 7265 6129 295d  ange(len(area))]
+000154b0: 292e 7371 7565 657a 6528 292e 542e 7265  ).squeeze().T.re
+000154c0: 7368 6170 6528 286c 656e 2861 7265 6129  shape((len(area)
+000154d0: 2c6c 656e 2872 6174 696f 5f77 696e 646f  ,len(ratio_windo
+000154e0: 7773 2929 290a 2020 2020 2020 2020 526f  ws))).        Ro
+000154f0: 6273 6572 7665 645f 3264 3d6e 702e 6473  bserved_2d=np.ds
+00015500: 7461 636b 285b 526f 6273 6572 7665 6420  tack([Robserved 
+00015510: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
+00015520: 656e 2861 7265 6129 295d 292e 7371 7565  en(area))]).sque
+00015530: 657a 6528 292e 542e 7265 7368 6170 6528  eze().T.reshape(
+00015540: 286c 656e 2861 7265 6129 2c6c 656e 2872  (len(area),len(r
+00015550: 6174 696f 5f77 696e 646f 7773 2929 290a  atio_windows))).
+00015560: 2020 2020 2020 2020 6966 2028 6c65 6e28          if (len(
+00015570: 7261 7469 6f5f 7769 6e64 6f77 735b 305d  ratio_windows[0]
+00015580: 293d 3d33 293a 2020 2320 7765 6967 6874  )==3):  # weight
+00015590: 6564 2063 6869 320a 2020 2020 2020 2020  ed chi2.        
+000155a0: 2020 2020 7261 7469 6f5f 7769 6e64 6f77      ratio_window
+000155b0: 735f 7765 6967 6874 733d 6e70 2e61 7272  s_weights=np.arr
+000155c0: 6179 285b 7261 7469 6f5f 7769 6e64 6f77  ay([ratio_window
+000155d0: 735b 6b5d 5b32 5d20 666f 7220 6b20 696e  s[k][2] for k in
+000155e0: 2072 616e 6765 286c 656e 2872 6174 696f   range(len(ratio
+000155f0: 5f77 696e 646f 7773 2929 5d29 0a20 2020  _windows))]).   
+00015600: 2020 2020 2020 2020 2072 6174 696f 5f77           ratio_w
+00015610: 696e 646f 7773 5f77 6569 6768 7473 5f32  indows_weights_2
+00015620: 643d 6e70 2e64 7374 6163 6b28 5b72 6174  d=np.dstack([rat
+00015630: 696f 5f77 696e 646f 7773 5f77 6569 6768  io_windows_weigh
+00015640: 7473 2066 6f72 2069 2069 6e20 7261 6e67  ts for i in rang
+00015650: 6528 6c65 6e28 6172 6561 2929 5d29 2e73  e(len(area))]).s
+00015660: 7175 6565 7a65 2829 2e54 2e72 6573 6861  queeze().T.resha
+00015670: 7065 2828 6c65 6e28 6172 6561 292c 6c65  pe((len(area),le
+00015680: 6e28 7261 7469 6f5f 7769 6e64 6f77 735f  n(ratio_windows_
+00015690: 7765 6967 6874 7329 2929 0a20 2020 2020  weights))).     
+000156a0: 2020 2020 2020 2063 6869 5f61 7265 612b         chi_area+
+000156b0: 3d6e 702e 7375 6d28 2828 526d 6f64 656c  =np.sum(((Rmodel
+000156c0: 5f32 642d 526f 6273 6572 7665 645f 3264  _2d-Robserved_2d
+000156d0: 292f 526f 6273 6572 7665 645f 3264 292a  )/Robserved_2d)*
+000156e0: 2a32 2a72 6174 696f 5f77 696e 646f 7773  *2*ratio_windows
+000156f0: 5f77 6569 6768 7473 5f32 642c 6178 6973  _weights_2d,axis
+00015700: 3d31 290a 2020 2020 2020 2020 2020 2020  =1).            
+00015710: 6e6f 726d 5f66 6163 746f 722b 3d6e 702e  norm_factor+=np.
+00015720: 7375 6d28 7261 7469 6f5f 7769 6e64 6f77  sum(ratio_window
+00015730: 735f 7765 6967 6874 7329 0a20 2020 2020  s_weights).     
+00015740: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00015750: 2020 2020 2063 6869 5f61 7265 612b 3d6e       chi_area+=n
+00015760: 702e 7375 6d28 2828 526d 6f64 656c 5f32  p.sum(((Rmodel_2
+00015770: 642d 526f 6273 6572 7665 645f 3264 292f  d-Robserved_2d)/
+00015780: 526f 6273 6572 7665 645f 3264 292a 2a32  Robserved_2d)**2
+00015790: 2c61 7869 733d 3129 0a20 2020 2020 2020  ,axis=1).       
+000157a0: 2020 2020 206e 6f72 6d5f 6661 6374 6f72       norm_factor
+000157b0: 2b3d 6c65 6e28 7261 7469 6f5f 7769 6e64  +=len(ratio_wind
+000157c0: 6f77 7329 0a20 2020 2069 6620 6c65 6e28  ows).    if len(
+000157d0: 7072 6f64 7563 745f 7769 6e64 6f77 7329  product_windows)
+000157e0: 3e30 3a0a 2020 2020 2020 2020 6172 6561  >0:.        area
+000157f0: 5f32 643d 6e70 2e64 7374 6163 6b28 5b61  _2d=np.dstack([a
+00015800: 7265 6120 666f 7220 6920 696e 2072 616e  rea for i in ran
+00015810: 6765 286c 656e 2870 726f 6475 6374 5f77  ge(len(product_w
+00015820: 696e 646f 7773 2929 5d29 2e73 7175 6565  indows))]).squee
+00015830: 7a65 2829 2e72 6573 6861 7065 2828 6c65  ze().reshape((le
+00015840: 6e28 6172 6561 292c 6c65 6e28 7072 6f64  n(area),len(prod
+00015850: 7563 745f 7769 6e64 6f77 7329 2929 0a20  uct_windows))). 
+00015860: 2020 2020 2020 2050 6d6f 6465 6c5f 3264         Pmodel_2d
+00015870: 3d6e 702e 6473 7461 636b 285b 506d 6f64  =np.dstack([Pmod
+00015880: 656c 2066 6f72 2069 2069 6e20 7261 6e67  el for i in rang
+00015890: 6528 6c65 6e28 6172 6561 2929 5d29 2e73  e(len(area))]).s
+000158a0: 7175 6565 7a65 2829 2e54 2e72 6573 6861  queeze().T.resha
+000158b0: 7065 2828 6c65 6e28 6172 6561 292c 6c65  pe((len(area),le
+000158c0: 6e28 7072 6f64 7563 745f 7769 6e64 6f77  n(product_window
+000158d0: 7329 2929 0a20 2020 2020 2020 2050 6f62  s))).        Pob
+000158e0: 7365 7276 6564 5f32 643d 6e70 2e64 7374  served_2d=np.dst
+000158f0: 6163 6b28 5b50 6f62 7365 7276 6564 2066  ack([Pobserved f
+00015900: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
+00015910: 6e28 6172 6561 2929 5d29 2e73 7175 6565  n(area))]).squee
+00015920: 7a65 2829 2e54 2e72 6573 6861 7065 2828  ze().T.reshape((
+00015930: 6c65 6e28 6172 6561 292c 6c65 6e28 7072  len(area),len(pr
+00015940: 6f64 7563 745f 7769 6e64 6f77 7329 2929  oduct_windows)))
+00015950: 0a20 2020 2020 2020 2069 6620 286c 656e  .        if (len
+00015960: 2870 726f 6475 6374 5f77 696e 646f 7773  (product_windows
+00015970: 5b30 5d29 3d3d 3329 3a20 2023 2077 6569  [0])==3):  # wei
+00015980: 6768 7465 6420 6368 6932 0a20 2020 2020  ghted chi2.     
+00015990: 2020 2020 2020 2070 726f 6475 6374 5f77         product_w
+000159a0: 696e 646f 7773 5f77 6569 6768 7473 3d6e  indows_weights=n
+000159b0: 702e 6172 7261 7928 5b70 726f 6475 6374  p.array([product
+000159c0: 5f77 696e 646f 7773 5b6b 5d5b 325d 2066  _windows[k][2] f
+000159d0: 6f72 206b 2069 6e20 7261 6e67 6528 6c65  or k in range(le
+000159e0: 6e28 7072 6f64 7563 745f 7769 6e64 6f77  n(product_window
+000159f0: 7329 295d 290a 2020 2020 2020 2020 2020  s))]).          
+00015a00: 2020 7072 6f64 7563 745f 7769 6e64 6f77    product_window
+00015a10: 735f 7765 6967 6874 735f 3264 3d6e 702e  s_weights_2d=np.
+00015a20: 6473 7461 636b 285b 7072 6f64 7563 745f  dstack([product_
+00015a30: 7769 6e64 6f77 735f 7765 6967 6874 7320  windows_weights 
+00015a40: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
+00015a50: 656e 2861 7265 6129 295d 292e 7371 7565  en(area))]).sque
+00015a60: 657a 6528 292e 542e 7265 7368 6170 6528  eze().T.reshape(
+00015a70: 286c 656e 2861 7265 6129 2c6c 656e 2870  (len(area),len(p
+00015a80: 726f 6475 6374 5f77 696e 646f 7773 5f77  roduct_windows_w
+00015a90: 6569 6768 7473 2929 290a 2020 2020 2020  eights))).      
+00015aa0: 2020 2020 2020 6368 695f 6172 6561 2b3d        chi_area+=
+00015ab0: 6e70 2e73 756d 2828 2828 506d 6f64 656c  np.sum((((Pmodel
+00015ac0: 5f32 642a 6172 6561 5f32 642a 2a32 292a  _2d*area_2d**2)*
+00015ad0: 2a30 2e35 2d28 506f 6273 6572 7665 645f  *0.5-(Pobserved_
+00015ae0: 3264 292a 2a30 2e35 292f 2850 6f62 7365  2d)**0.5)/(Pobse
+00015af0: 7276 6564 5f32 6429 2a2a 302e 3529 2a2a  rved_2d)**0.5)**
+00015b00: 322a 7072 6f64 7563 745f 7769 6e64 6f77  2*product_window
+00015b10: 735f 7765 6967 6874 735f 3264 2c61 7869  s_weights_2d,axi
+00015b20: 733d 3129 0a20 2020 2020 2020 2020 2020  s=1).           
+00015b30: 206e 6f72 6d5f 6661 6374 6f72 2b3d 6e70   norm_factor+=np
+00015b40: 2e73 756d 2870 726f 6475 6374 5f77 696e  .sum(product_win
+00015b50: 646f 7773 5f77 6569 6768 7473 290a 2020  dows_weights).  
+00015b60: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00015b70: 2020 2020 2020 2020 6368 695f 6172 6561          chi_area
+00015b80: 2b3d 6e70 2e73 756d 2828 2828 506d 6f64  +=np.sum((((Pmod
+00015b90: 656c 5f32 642a 6172 6561 5f32 642a 2a32  el_2d*area_2d**2
+00015ba0: 292a 2a30 2e35 2d28 506f 6273 6572 7665  )**0.5-(Pobserve
+00015bb0: 645f 3264 292a 2a30 2e35 292f 2850 6f62  d_2d)**0.5)/(Pob
+00015bc0: 7365 7276 6564 5f32 6429 2a2a 302e 3529  served_2d)**0.5)
+00015bd0: 2a2a 322c 6178 6973 3d31 290a 2020 2020  **2,axis=1).    
+00015be0: 2020 2020 2020 2020 6e6f 726d 5f66 6163          norm_fac
+00015bf0: 746f 722b 3d6c 656e 2870 726f 6475 6374  tor+=len(product
+00015c00: 5f77 696e 646f 7773 290a 2020 2020 6966  _windows).    if
+00015c10: 206e 6f72 6d5f 6661 6374 6f72 3e30 3a20   norm_factor>0: 
+00015c20: 6368 695f 6172 6561 2f3d 6e6f 726d 5f66  chi_area/=norm_f
+00015c30: 6163 746f 720a 2020 2020 7265 7475 726e  actor.    return
+00015c40: 2863 6869 5f61 7265 6129 0a0a 0a64 6566  (chi_area)...def
+00015c50: 2072 6564 5f63 6869 325f 736c 6162 2873   red_chi2_slab(s
+00015c60: 6c61 625f 6461 7461 2c73 7065 6374 7261  lab_data,spectra
+00015c70: 2c6d 6173 6b2c 5264 6973 6b3d 6e70 2e6c  ,mask,Rdisk=np.l
+00015c80: 6f67 7370 6163 6528 2d32 2c32 2c31 3029  ogspace(-2,2,10)
+00015c90: 2c64 6973 7461 6e63 653d 3132 302c 4e4c  ,distance=120,NL
+00015ca0: 5445 3d46 616c 7365 2c52 3d33 3030 302c  TE=False,R=3000,
+00015cb0: 7368 6f72 745f 666f 726d 6174 3d46 616c  short_format=Fal
+00015cc0: 7365 2c6f 7665 726c 6170 3d46 616c 7365  se,overlap=False
+00015cd0: 2c6e 6f69 7365 5f6c 6576 656c 3d31 293a  ,noise_level=1):
+00015ce0: 0a20 2020 2027 2727 0a20 2020 2052 6574  .    '''.    Ret
+00015cf0: 7572 6e73 2072 6564 7563 6564 2063 6869  urns reduced chi
+00015d00: 3220 6261 7365 6420 6f6e 2073 656c 6563  2 based on selec
+00015d10: 7465 6420 7370 6563 7472 616c 2077 696e  ted spectral win
+00015d20: 646f 7773 2061 6372 6f73 7320 6469 6666  dows across diff
+00015d30: 6572 656e 7420 656d 6974 7469 6e67 2064  erent emitting d
+00015d40: 6973 6b20 7261 6469 7573 0a0a 2020 2020  isk radius..    
+00015d50: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+00015d60: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 736c  ---------.    sl
+00015d70: 6162 5f64 6174 6120 3a20 7374 7269 6e67  ab_data : string
+00015d80: 206f 7220 736c 6162 5f6d 6f64 656c 2069   or slab_model i
+00015d90: 6e73 7461 6e63 650a 2020 2020 2020 7061  nstance.      pa
+00015da0: 7468 2063 6f72 7265 7370 6f6e 6469 6e67  th corresponding
+00015db0: 2074 6f20 6120 7369 6e67 6c65 2073 6c61   to a single sla
+00015dc0: 6220 6d6f 6465 6c20 6f72 2061 2073 696e  b model or a sin
+00015dd0: 676c 6520 736c 6162 5f6d 6f64 656c 2069  gle slab_model i
+00015de0: 6e73 7461 6e63 650a 2020 2020 0a20 2020  nstance.    .   
+00015df0: 2073 7065 6374 7261 203a 206e 756d 7079   spectra : numpy
+00015e00: 2e61 7272 6179 0a20 2020 2020 206e 756d  .array.      num
+00015e10: 7079 2061 7272 6179 2077 6974 6820 6669  py array with fi
+00015e20: 7273 7420 636f 6c75 6d6e 2074 6865 2077  rst column the w
+00015e30: 6176 656c 656e 6774 6820 696e 205b 6d69  avelength in [mi
+00015e40: 6372 6f6e 735d 2061 6e64 2073 6563 6f6e  crons] and secon
+00015e50: 6420 636f 6c75 6d6e 2066 6c75 7820 696e  d column flux in
+00015e60: 205b 4a79 5d0a 0a20 2020 206d 6173 6b20   [Jy]..    mask 
+00015e70: 3a20 6e75 6d70 792e 6172 7261 790a 2020  : numpy.array.  
+00015e80: 2020 2020 6e75 6d70 7920 626f 6f6c 6561      numpy boolea
+00015e90: 6e20 6172 7261 7920 7468 6174 206d 6173  n array that mas
+00015ea0: 6b73 2063 6572 7461 696e 2070 6172 7473  ks certain parts
+00015eb0: 206f 6620 7468 6520 7370 6563 7472 6120   of the spectra 
+00015ec0: 6672 6f6d 2074 6865 2066 6974 2020 0a20  from the fit  . 
+00015ed0: 2020 200a 2020 2020 5264 6973 6b20 3a20     .    Rdisk : 
+00015ee0: 666c 6f61 740a 2020 2020 2020 5261 6469  float.      Radi
+00015ef0: 7573 2063 6f72 7265 7370 6f6e 6469 6e67  us corresponding
+00015f00: 2074 6f20 656d 6974 7469 6e67 2061 7265   to emitting are
+00015f10: 6120 696e 2061 7374 726f 6e6f 6d69 6361  a in astronomica
+00015f20: 6c20 756e 6974 730a 2020 2020 0a20 2020  l units.    .   
+00015f30: 2064 6973 7461 6e63 6520 3a20 666c 6f61   distance : floa
+00015f40: 740a 2020 2020 2020 6469 7374 616e 6365  t.      distance
+00015f50: 206f 6620 6469 736b 2069 6e20 7061 7273   of disk in pars
+00015f60: 6563 0a20 2020 200a 2020 2020 4e4c 5445  ec.    .    NLTE
+00015f70: 203a 2062 6f6f 6c65 616e 0a20 2020 2020   : boolean.     
+00015f80: 2069 6620 5472 7565 2c20 4e4c 5445 2066   if True, NLTE f
+00015f90: 6c75 7820 6973 2074 616b 656e 2066 726f  lux is taken fro
+00015fa0: 6d20 7468 6520 736c 6162 206d 6f64 656c  m the slab model
+00015fb0: 2069 6e20 6361 7365 206f 6620 6f76 6572   in case of over
+00015fc0: 6c61 703d 4661 6c73 652e 0a0a 2020 2020  lap=False...    
+00015fd0: 5220 3a20 666c 6f61 740a 2020 2020 2020  R : float.      
+00015fe0: 5370 6563 7472 616c 2072 6573 6f6c 7669  Spectral resolvi
+00015ff0: 6e67 2070 6f77 6572 206f 6620 7468 6520  ng power of the 
+00016000: 6f62 7365 7276 6564 2073 7065 6374 7275  observed spectru
+00016010: 6d20 666f 7220 636f 6e76 6f6c 7669 6e67  m for convolving
+00016020: 2074 6865 2073 6c61 6220 6d6f 6465 6c0a   the slab model.
+00016030: 2020 2020 0a20 2020 2073 686f 7274 5f66      .    short_f
+00016040: 6f72 6d61 7420 3a20 626f 6f6c 6561 6e0a  ormat : boolean.
+00016050: 2020 2020 2020 5479 7065 206f 6620 736c        Type of sl
+00016060: 6162 206d 6f64 656c 206f 7574 7075 7420  ab model output 
+00016070: 6669 6c65 2c20 7368 6f72 7420 7673 206c  file, short vs l
+00016080: 6f6e 670a 2020 2020 0a20 2020 206f 7665  ong.    .    ove
+00016090: 726c 6170 203a 2062 6f6f 6c65 616e 0a20  rlap : boolean. 
+000160a0: 2020 2020 204d 6f6c 6563 756c 6172 206f       Molecular o
+000160b0: 7061 6369 7479 206f 7665 726c 6170 2063  pacity overlap c
+000160c0: 6f6e 7369 6465 7265 6420 696e 2074 6865  onsidered in the
+000160d0: 2073 6c61 6220 6d6f 6465 6c0a 2020 2020   slab model.    
+000160e0: 2020 0a20 2020 206e 6f69 7365 5f6c 6576    .    noise_lev
+000160f0: 656c 203a 2066 6c6f 6174 0a20 2020 2020  el : float.     
+00016100: 204e 6f69 7365 206c 6576 656c 2069 6e20   Noise level in 
+00016110: 7468 6520 7370 6563 7472 756d 2c20 696e  the spectrum, in
+00016120: 2074 6865 2073 616d 6520 756e 6974 7320   the same units 
+00016130: 6173 2074 6865 2066 6c75 7820 7061 7373  as the flux pass
+00016140: 6564 2069 6e20 7468 6520 6172 6775 6d65  ed in the argume
+00016150: 6e74 2073 7065 6374 7261 0a20 2020 2027  nt spectra.    '
+00016160: 2727 0a20 2020 2061 7265 613d 286e 702e  ''.    area=(np.
+00016170: 7069 2a28 5264 6973 6b2a 6175 2f64 6973  pi*(Rdisk*au/dis
+00016180: 7461 6e63 652f 7063 292a 2a32 292e 7265  tance/pc)**2).re
+00016190: 7368 6170 6528 5264 6973 6b2e 7368 6170  shape(Rdisk.shap
+000161a0: 655b 305d 2c31 290a 0a20 2020 2069 6620  e[0],1)..    if 
+000161b0: 6973 696e 7374 616e 6365 2873 6c61 625f  isinstance(slab_
+000161c0: 6461 7461 2c73 7472 293a 2073 6c61 625f  data,str): slab_
+000161d0: 6461 7461 3d72 6561 645f 736c 6162 2873  data=read_slab(s
+000161e0: 6c61 625f 6461 7461 2c76 6572 626f 7365  lab_data,verbose
+000161f0: 3d46 616c 7365 2c73 686f 7274 5f66 6f72  =False,short_for
+00016200: 6d61 743d 7368 6f72 745f 666f 726d 6174  mat=short_format
+00016210: 2c6f 7665 726c 6170 3d6f 7665 726c 6170  ,overlap=overlap
+00016220: 290a 2020 2020 6c6d 696e 3d6e 702e 616d  ).    lmin=np.am
+00016230: 696e 2873 7065 6374 7261 5b3a 2c30 5d29  in(spectra[:,0])
+00016240: 0a20 2020 206c 6d61 783d 6e70 2e61 6d61  .    lmax=np.ama
+00016250: 7828 7370 6563 7472 615b 3a2c 305d 290a  x(spectra[:,0]).
+00016260: 2020 2020 736c 6162 5f64 6174 612e 636f      slab_data.co
+00016270: 6e76 6f6c 7665 2852 3d52 2c6c 616d 6264  nvolve(R=R,lambd
+00016280: 615f 303d 6c6d 696e 2a30 2e39 2c6c 616d  a_0=lmin*0.9,lam
+00016290: 6264 615f 6e3d 6c6d 6178 2a31 2e31 2c4e  bda_n=lmax*1.1,N
+000162a0: 4c54 453d 4e4c 5445 2c76 6572 626f 7365  LTE=NLTE,verbose
+000162b0: 3d46 616c 7365 2c6f 7665 726c 6170 3d6f  =False,overlap=o
+000162c0: 7665 726c 6170 290a 2020 2020 6966 206e  verlap).    if n
+000162d0: 6f74 206f 7665 726c 6170 3a0a 2020 2020  ot overlap:.    
+000162e0: 2020 2020 6966 204e 4c54 453a 0a20 2020      if NLTE:.   
+000162f0: 2020 2020 2020 2020 206d 6f64 656c 5370           modelSp
+00016300: 6563 3d73 7065 6374 7265 7328 7370 6563  ec=spectres(spec
+00016310: 7472 615b 3a2c 305d 2c73 6c61 625f 6461  tra[:,0],slab_da
+00016320: 7461 2e63 6f6e 7657 6176 656c 656e 6774  ta.convWavelengt
+00016330: 682c 736c 6162 5f64 6174 612e 636f 6e76  h,slab_data.conv
+00016340: 4e4c 5445 666c 7578 2a31 6532 332c 7665  NLTEflux*1e23,ve
+00016350: 7262 6f73 653d 4661 6c73 652c 6669 6c6c  rbose=False,fill
+00016360: 3d30 2e30 290a 2020 2020 2020 2020 656c  =0.0).        el
+00016370: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00016380: 6d6f 6465 6c53 7065 633d 7370 6563 7472  modelSpec=spectr
+00016390: 6573 2873 7065 6374 7261 5b3a 2c30 5d2c  es(spectra[:,0],
+000163a0: 736c 6162 5f64 6174 612e 636f 6e76 5761  slab_data.convWa
+000163b0: 7665 6c65 6e67 7468 2c73 6c61 625f 6461  velength,slab_da
+000163c0: 7461 2e63 6f6e 764c 5445 666c 7578 2a31  ta.convLTEflux*1
+000163d0: 6532 332c 7665 7262 6f73 653d 4661 6c73  e23,verbose=Fals
+000163e0: 652c 6669 6c6c 3d30 2e30 290a 2020 2020  e,fill=0.0).    
+000163f0: 656c 7365 3a0a 2020 2020 2020 2020 6d6f  else:.        mo
+00016400: 6465 6c53 7065 633d 7370 6563 7472 6573  delSpec=spectres
+00016410: 2873 7065 6374 7261 5b3a 2c30 5d2c 632f  (spectra[:,0],c/
+00016420: 736c 6162 5f64 6174 612e 636f 6e76 4f76  slab_data.convOv
+00016430: 6572 6c61 7046 7265 715b 3a3a 2d31 5d2a  erlapFreq[::-1]*
+00016440: 3165 2d33 2c73 6c61 625f 6461 7461 2e63  1e-3,slab_data.c
+00016450: 6f6e 764f 7665 726c 6170 4c54 455b 3a3a  onvOverlapLTE[::
+00016460: 2d31 5d2a 3165 3233 2c76 6572 626f 7365  -1]*1e23,verbose
+00016470: 3d46 616c 7365 2c66 696c 6c3d 302e 3029  =False,fill=0.0)
+00016480: 0a20 2020 2073 7065 6374 7261 5f32 643d  .    spectra_2d=
+00016490: 7370 6563 7472 615b 6d61 736b 2c31 5d2e  spectra[mask,1].
+000164a0: 7265 7368 6170 6528 312c 7370 6563 7472  reshape(1,spectr
+000164b0: 615b 6d61 736b 2c2d 315d 2e73 6861 7065  a[mask,-1].shape
+000164c0: 5b30 5d29 2a6e 702e 6f6e 6573 5f6c 696b  [0])*np.ones_lik
+000164d0: 6528 6172 6561 290a 2020 2020 6d6f 6465  e(area).    mode
+000164e0: 6c53 7065 635f 3264 3d6d 6f64 656c 5370  lSpec_2d=modelSp
+000164f0: 6563 5b6d 6173 6b5d 2e72 6573 6861 7065  ec[mask].reshape
+00016500: 2831 2c6d 6f64 656c 5370 6563 5b6d 6173  (1,modelSpec[mas
+00016510: 6b5d 2e73 6861 7065 5b30 5d29 2a6e 702e  k].shape[0])*np.
+00016520: 6f6e 6573 5f6c 696b 6528 6172 6561 290a  ones_like(area).
+00016530: 2020 2020 6172 6561 5f32 643d 6172 6561      area_2d=area
+00016540: 2e72 6573 6861 7065 2861 7265 612e 7368  .reshape(area.sh
+00016550: 6170 655b 305d 2c31 290a 2020 2020 6368  ape[0],1).    ch
+00016560: 695f 6172 6561 3d6e 702e 7375 6d28 2873  i_area=np.sum((s
+00016570: 7065 6374 7261 5f32 642d 6d6f 6465 6c53  pectra_2d-modelS
+00016580: 7065 635f 3264 2a61 7265 615f 3264 292a  pec_2d*area_2d)*
+00016590: 2a32 2c61 7869 733d 3129 2f6c 656e 2873  *2,axis=1)/len(s
+000165a0: 7065 6374 7261 5b6d 6173 6b2c 305d 292f  pectra[mask,0])/
+000165b0: 6e6f 6973 655f 6c65 7665 6c2a 2a32 0a0a  noise_level**2..
+000165c0: 2020 2020 7265 7475 726e 2863 6869 5f61      return(chi_a
+000165d0: 7265 6129 0a0a 0a64 6566 2072 6564 5f63  rea)...def red_c
+000165e0: 6869 325f 736c 6162 5f6d 756c 7469 2873  hi2_slab_multi(s
+000165f0: 6c61 625f 6461 7461 2c73 7065 6374 7261  lab_data,spectra
+00016600: 2c6d 6173 6b2c 5264 6973 6b3d 6e70 2e6c  ,mask,Rdisk=np.l
+00016610: 6f67 7370 6163 6528 2d32 2c32 2c31 3029  ogspace(-2,2,10)
+00016620: 2c64 6973 7461 6e63 653d 3132 302c 4e4c  ,distance=120,NL
+00016630: 5445 3d46 616c 7365 2c52 3d33 3030 302c  TE=False,R=3000,
+00016640: 7368 6f72 745f 666f 726d 6174 3d46 616c  short_format=Fal
+00016650: 7365 2c6f 7665 726c 6170 3d46 616c 7365  se,overlap=False
+00016660: 2c6e 6f69 7365 5f6c 6576 656c 3d31 293a  ,noise_level=1):
+00016670: 0a20 2020 2027 2727 0a20 2020 2052 6574  .    '''.    Ret
+00016680: 7572 6e73 2072 6564 7563 6564 2063 6869  urns reduced chi
+00016690: 3220 666f 7220 7477 6f20 736c 6162 206d  2 for two slab m
+000166a0: 6f64 656c 7320 6261 7365 6420 6f6e 2073  odels based on s
+000166b0: 656c 6563 7465 6420 7370 6563 7472 616c  elected spectral
+000166c0: 2077 696e 646f 7773 2061 6372 6f73 7320   windows across 
+000166d0: 6469 6666 6572 656e 7420 656d 6974 7469  different emitti
+000166e0: 6e67 2064 6973 6b20 7261 6469 7573 0a0a  ng disk radius..
+000166f0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00016700: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00016710: 2020 736c 6162 5f64 6174 6120 3a20 6c69    slab_data : li
+00016720: 7374 206f 6620 7374 7269 6e67 730a 2020  st of strings.  
+00016730: 2020 2020 7061 7468 7320 636f 7272 6573      paths corres
+00016740: 706f 6e64 696e 6720 746f 2074 776f 2073  ponding to two s
+00016750: 6c61 6220 6d6f 6465 6c0a 2020 2020 7370  lab model.    sp
+00016760: 6563 7472 6120 3a20 6e75 6d70 792e 6172  ectra : numpy.ar
+00016770: 7261 790a 2020 2020 2020 6e75 6d70 7920  ray.      numpy 
+00016780: 6172 7261 7920 7769 7468 2066 6972 7374  array with first
+00016790: 2063 6f6c 756d 6e20 7468 6520 7761 7665   column the wave
+000167a0: 6c65 6e67 7468 2069 6e20 5b6d 6963 726f  length in [micro
+000167b0: 6e73 5d20 616e 6420 7365 636f 6e64 2063  ns] and second c
+000167c0: 6f6c 756d 6e20 666c 7578 2069 6e20 5b4a  olumn flux in [J
+000167d0: 795d 0a0a 2020 2020 6d61 736b 203a 206e  y]..    mask : n
+000167e0: 756d 7079 2e61 7272 6179 0a20 2020 2020  umpy.array.     
+000167f0: 206e 756d 7079 2062 6f6f 6c65 616e 2061   numpy boolean a
+00016800: 7272 6179 2074 6861 7420 6d61 736b 7320  rray that masks 
+00016810: 6365 7274 6169 6e20 7061 7274 7320 6f66  certain parts of
+00016820: 2074 6865 2073 7065 6374 7261 2066 726f   the spectra fro
+00016830: 6d20 7468 6520 6669 7420 200a 2020 2020  m the fit  .    
+00016840: 0a20 2020 2052 6469 736b 203a 2066 6c6f  .    Rdisk : flo
+00016850: 6174 0a20 2020 2020 2052 6164 6975 7320  at.      Radius 
+00016860: 636f 7272 6573 706f 6e64 696e 6720 746f  corresponding to
+00016870: 2065 6d69 7474 696e 6720 6172 6561 2069   emitting area i
+00016880: 6e20 6173 7472 6f6e 6f6d 6963 616c 2075  n astronomical u
+00016890: 6e69 7473 0a20 2020 200a 2020 2020 6469  nits.    .    di
+000168a0: 7374 616e 6365 203a 2066 6c6f 6174 0a20  stance : float. 
+000168b0: 2020 2020 2064 6973 7461 6e63 6520 6f66       distance of
+000168c0: 2064 6973 6b20 696e 2070 6172 7365 630a   disk in parsec.
+000168d0: 2020 2020 0a20 2020 204e 4c54 4520 3a20      .    NLTE : 
+000168e0: 626f 6f6c 6561 6e0a 2020 2020 2020 6966  boolean.      if
+000168f0: 2054 7275 652c 204e 4c54 4520 666c 7578   True, NLTE flux
+00016900: 2069 7320 7461 6b65 6e20 6672 6f6d 2074   is taken from t
+00016910: 6865 2073 6c61 6220 6d6f 6465 6c20 696e  he slab model in
+00016920: 2063 6173 6520 6f66 206f 7665 726c 6170   case of overlap
+00016930: 3d46 616c 7365 2e0a 0a20 2020 2052 203a  =False...    R :
+00016940: 2066 6c6f 6174 0a20 2020 2020 2053 7065   float.      Spe
+00016950: 6374 7261 6c20 7265 736f 6c76 696e 6720  ctral resolving 
+00016960: 706f 7765 7220 6f66 2074 6865 206f 6273  power of the obs
+00016970: 6572 7665 6420 7370 6563 7472 756d 2066  erved spectrum f
+00016980: 6f72 2063 6f6e 766f 6c76 696e 6720 7468  or convolving th
+00016990: 6520 736c 6162 206d 6f64 656c 0a20 2020  e slab model.   
+000169a0: 200a 2020 2020 7368 6f72 745f 666f 726d   .    short_form
+000169b0: 6174 203a 2062 6f6f 6c65 616e 0a20 2020  at : boolean.   
+000169c0: 2020 2054 7970 6520 6f66 2073 6c61 6220     Type of slab 
+000169d0: 6d6f 6465 6c20 6f75 7470 7574 2066 696c  model output fil
+000169e0: 652c 2073 686f 7274 2076 7320 6c6f 6e67  e, short vs long
+000169f0: 0a20 2020 200a 2020 2020 6f76 6572 6c61  .    .    overla
+00016a00: 7020 3a20 626f 6f6c 6561 6e0a 2020 2020  p : boolean.    
+00016a10: 2020 4d6f 6c65 6375 6c61 7220 6f70 6163    Molecular opac
+00016a20: 6974 7920 6f76 6572 6c61 7020 636f 6e73  ity overlap cons
+00016a30: 6964 6572 6564 2069 6e20 7468 6520 736c  idered in the sl
+00016a40: 6162 206d 6f64 656c 0a20 2020 2020 200a  ab model.      .
+00016a50: 2020 2020 6e6f 6973 655f 6c65 7665 6c20      noise_level 
+00016a60: 3a20 666c 6f61 740a 2020 2020 2020 4e6f  : float.      No
+00016a70: 6973 6520 6c65 7665 6c20 696e 2074 6865  ise level in the
+00016a80: 2073 7065 6374 7275 6d2c 2069 6e20 7468   spectrum, in th
+00016a90: 6520 7361 6d65 2075 6e69 7473 2061 7320  e same units as 
+00016aa0: 7468 6520 666c 7578 2070 6173 7365 6420  the flux passed 
+00016ab0: 696e 2074 6865 2061 7267 756d 656e 7420  in the argument 
+00016ac0: 7370 6563 7472 610a 2020 2020 2727 270a  spectra.    '''.
+00016ad0: 2020 2020 6172 6561 203d 2028 6e70 2e70      area = (np.p
+00016ae0: 692a 2852 6469 736b 2a61 752f 6469 7374  i*(Rdisk*au/dist
+00016af0: 616e 6365 2f70 6329 2a2a 3229 2e72 6573  ance/pc)**2).res
+00016b00: 6861 7065 2852 6469 736b 2e73 6861 7065  hape(Rdisk.shape
+00016b10: 5b30 5d2c 312c 3129 0a20 2020 2066 7261  [0],1,1).    fra
+00016b20: 6374 696f 6e20 3d20 6e70 2e6c 696e 7370  ction = np.linsp
+00016b30: 6163 6528 302c 312c 3130 3029 2e72 6573  ace(0,1,100).res
+00016b40: 6861 7065 2831 2c31 3030 2c31 290a 2020  hape(1,100,1).  
+00016b50: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00016b60: 736c 6162 5f64 6174 612c 7374 7229 3a20  slab_data,str): 
+00016b70: 0a20 2020 2020 2020 2073 6c61 625f 6461  .        slab_da
+00016b80: 7461 3d72 6561 645f 736c 6162 2873 6c61  ta=read_slab(sla
+00016b90: 625f 6461 7461 2c76 6572 626f 7365 3d46  b_data,verbose=F
+00016ba0: 616c 7365 2c73 686f 7274 5f66 6f72 6d61  alse,short_forma
+00016bb0: 743d 7368 6f72 745f 666f 726d 6174 2c6f  t=short_format,o
+00016bc0: 7665 726c 6170 3d6f 7665 726c 6170 290a  verlap=overlap).
+00016bd0: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
+00016be0: 6e63 6528 736c 6162 5f64 6174 612c 6c69  nce(slab_data,li
+00016bf0: 7374 293a 0a20 2020 2020 2020 2073 6c61  st):.        sla
+00016c00: 625f 6461 7461 3d72 6561 645f 736c 6162  b_data=read_slab
+00016c10: 2873 6c61 625f 6461 7461 2c76 6572 626f  (slab_data,verbo
+00016c20: 7365 3d46 616c 7365 2c73 686f 7274 5f66  se=False,short_f
+00016c30: 6f72 6d61 743d 7368 6f72 745f 666f 726d  ormat=short_form
+00016c40: 6174 2c6f 7665 726c 6170 3d6f 7665 726c  at,overlap=overl
+00016c50: 6170 290a 2020 2020 2020 2020 0a20 2020  ap).        .   
+00016c60: 206c 6d69 6e3d 6e70 2e61 6d69 6e28 7370   lmin=np.amin(sp
+00016c70: 6563 7472 615b 3a2c 305d 290a 2020 2020  ectra[:,0]).    
+00016c80: 6c6d 6178 3d6e 702e 616d 6178 2873 7065  lmax=np.amax(spe
+00016c90: 6374 7261 5b3a 2c30 5d29 0a20 2020 2073  ctra[:,0]).    s
+00016ca0: 6c61 625f 6461 7461 2e63 6f6e 766f 6c76  lab_data.convolv
+00016cb0: 6528 523d 522c 6c61 6d62 6461 5f30 3d6c  e(R=R,lambda_0=l
+00016cc0: 6d69 6e2a 302e 392c 6c61 6d62 6461 5f6e  min*0.9,lambda_n
+00016cd0: 3d6c 6d61 782a 312e 312c 4e4c 5445 3d4e  =lmax*1.1,NLTE=N
+00016ce0: 4c54 452c 7665 7262 6f73 653d 4661 6c73  LTE,verbose=Fals
+00016cf0: 652c 6f76 6572 6c61 703d 6f76 6572 6c61  e,overlap=overla
+00016d00: 7029 0a20 2020 2069 6620 6e6f 7420 6f76  p).    if not ov
+00016d10: 6572 6c61 703a 0a20 2020 2020 2020 2069  erlap:.        i
+00016d20: 6620 4e4c 5445 3a0a 2020 2020 2020 2020  f NLTE:.        
+00016d30: 2020 2020 636f 6e74 5370 6563 203d 2073      contSpec = s
+00016d40: 7065 6374 7265 7328 7370 6563 7472 615b  pectres(spectra[
+00016d50: 3a2c 305d 2c20 736c 6162 5f64 6174 615b  :,0], slab_data[
+00016d60: 305d 2e63 6f6e 7657 6176 656c 656e 6774  0].convWavelengt
+00016d70: 682c 736c 6162 5f64 6174 615b 305d 2e63  h,slab_data[0].c
+00016d80: 6f6e 764e 4c54 4566 6c75 782a 3165 3233  onvNLTEflux*1e23
+00016d90: 2c76 6572 626f 7365 3d46 616c 7365 2c66  ,verbose=False,f
+00016da0: 696c 6c3d 302e 3029 0a20 2020 2020 2020  ill=0.0).       
+00016db0: 2020 2020 2066 6561 7453 7065 6320 3d20       featSpec = 
+00016dc0: 7370 6563 7472 6573 2873 7065 6374 7261  spectres(spectra
+00016dd0: 5b3a 2c30 5d2c 2073 6c61 625f 6461 7461  [:,0], slab_data
+00016de0: 5b31 5d2e 636f 6e76 5761 7665 6c65 6e67  [1].convWaveleng
+00016df0: 7468 2c73 6c61 625f 6461 7461 5b31 5d2e  th,slab_data[1].
+00016e00: 636f 6e76 4e4c 5445 666c 7578 2a31 6532  convNLTEflux*1e2
+00016e10: 332c 7665 7262 6f73 653d 4661 6c73 652c  3,verbose=False,
+00016e20: 6669 6c6c 3d30 2e30 290a 2020 2020 2020  fill=0.0).      
+00016e30: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00016e40: 2020 2020 636f 6e74 5370 6563 203d 2073      contSpec = s
+00016e50: 7065 6374 7265 7328 7370 6563 7472 615b  pectres(spectra[
+00016e60: 3a2c 305d 2c20 736c 6162 5f64 6174 615b  :,0], slab_data[
+00016e70: 305d 2e63 6f6e 7657 6176 656c 656e 6774  0].convWavelengt
+00016e80: 682c 736c 6162 5f64 6174 615b 305d 2e63  h,slab_data[0].c
+00016e90: 6f6e 764c 5445 666c 7578 2a31 6532 332c  onvLTEflux*1e23,
+00016ea0: 7665 7262 6f73 653d 4661 6c73 652c 6669  verbose=False,fi
+00016eb0: 6c6c 3d30 2e30 290a 2020 2020 2020 2020  ll=0.0).        
+00016ec0: 2020 2020 6665 6174 5370 6563 203d 2073      featSpec = s
+00016ed0: 7065 6374 7265 7328 7370 6563 7472 615b  pectres(spectra[
+00016ee0: 3a2c 305d 2c20 736c 6162 5f64 6174 615b  :,0], slab_data[
+00016ef0: 315d 2e63 6f6e 7657 6176 656c 656e 6774  1].convWavelengt
+00016f00: 682c 736c 6162 5f64 6174 615b 315d 2e63  h,slab_data[1].c
+00016f10: 6f6e 764c 5445 666c 7578 2a31 6532 332c  onvLTEflux*1e23,
+00016f20: 7665 7262 6f73 653d 4661 6c73 652c 6669  verbose=False,fi
+00016f30: 6c6c 3d30 2e30 290a 2020 2020 656c 7365  ll=0.0).    else
+00016f40: 3a0a 2020 2020 2020 2020 636f 6e74 5370  :.        contSp
+00016f50: 6563 203d 2073 7065 6374 7265 7328 7370  ec = spectres(sp
+00016f60: 6563 7472 615b 3a2c 305d 2c20 736c 6162  ectra[:,0], slab
+00016f70: 5f64 6174 615b 305d 2e63 6f6e 764f 7665  _data[0].convOve
+00016f80: 726c 6170 5761 7665 5b3a 3a2d 315d 2c73  rlapWave[::-1],s
+00016f90: 6c61 625f 6461 7461 5b30 5d2e 636f 6e76  lab_data[0].conv
+00016fa0: 4f76 6572 6c61 704c 5445 5b3a 3a2d 315d  OverlapLTE[::-1]
+00016fb0: 2a31 6532 332c 2076 6572 626f 7365 3d46  *1e23, verbose=F
+00016fc0: 616c 7365 2c66 696c 6c3d 302e 3029 0a20  alse,fill=0.0). 
+00016fd0: 2020 2020 2020 2066 6561 7453 7065 6320         featSpec 
+00016fe0: 3d20 7370 6563 7472 6573 2873 7065 6374  = spectres(spect
+00016ff0: 7261 5b3a 2c30 5d2c 2073 6c61 625f 6461  ra[:,0], slab_da
+00017000: 7461 5b31 5d2e 636f 6e76 4f76 6572 6c61  ta[1].convOverla
+00017010: 7057 6176 655b 3a3a 2d31 5d2c 736c 6162  pWave[::-1],slab
+00017020: 5f64 6174 615b 315d 2e63 6f6e 764f 7665  _data[1].convOve
+00017030: 726c 6170 4c54 455b 3a3a 2d31 5d2a 3165  rlapLTE[::-1]*1e
+00017040: 3233 2c20 7665 7262 6f73 653d 4661 6c73  23, verbose=Fals
+00017050: 652c 6669 6c6c 3d30 2e30 290a 2020 2020  e,fill=0.0).    
+00017060: 0a20 2020 2073 7065 6374 7261 2020 3d20  .    spectra  = 
+00017070: 7370 6563 7472 615b 6d61 736b 2c31 5d2e  spectra[mask,1].
+00017080: 7265 7368 6170 6528 312c 312c 7370 6563  reshape(1,1,spec
+00017090: 7472 615b 6d61 736b 2c2d 315d 2e73 6861  tra[mask,-1].sha
+000170a0: 7065 5b30 5d29 0a20 2020 2063 6f6e 7453  pe[0]).    contS
+000170b0: 7065 6320 3d20 2063 6f6e 7453 7065 635b  pec =  contSpec[
+000170c0: 6d61 736b 5d2e 7265 7368 6170 6528 312c  mask].reshape(1,
+000170d0: 312c 636f 6e74 5370 6563 5b6d 6173 6b5d  1,contSpec[mask]
+000170e0: 2e73 6861 7065 5b30 5d29 0a20 2020 2066  .shape[0]).    f
+000170f0: 6561 7453 7065 6320 3d20 2066 6561 7453  eatSpec =  featS
+00017100: 7065 635b 6d61 736b 5d2e 7265 7368 6170  pec[mask].reshap
+00017110: 6528 312c 312c 6665 6174 5370 6563 5b6d  e(1,1,featSpec[m
+00017120: 6173 6b5d 2e73 6861 7065 5b30 5d29 0a20  ask].shape[0]). 
+00017130: 2020 200a 2020 2020 6669 6e61 6c53 7065     .    finalSpe
+00017140: 6320 3d20 6172 6561 2a28 6672 6163 7469  c = area*(fracti
+00017150: 6f6e 2a63 6f6e 7453 7065 632b 2831 2d66  on*contSpec+(1-f
+00017160: 7261 6374 696f 6e29 2a66 6561 7453 7065  raction)*featSpe
+00017170: 6329 0a20 2020 2063 6869 5f61 7265 6120  c).    chi_area 
+00017180: 3d20 6e70 2e73 756d 2828 7370 6563 7472  = np.sum((spectr
+00017190: 612d 6669 6e61 6c53 7065 6329 2a2a 322c  a-finalSpec)**2,
+000171a0: 6178 6973 3d32 292f 7370 6563 7472 612e  axis=2)/spectra.
+000171b0: 7369 7a65 2f6e 6f69 7365 5f6c 6576 656c  size/noise_level
+000171c0: 2a2a 320a 2020 2020 0a20 2020 2072 6574  **2.    .    ret
+000171d0: 7572 6e28 6368 695f 6172 6561 290a 0a    urn(chi_area)..
```

### Comparing `prodimopy-2.2.1/prodimopy/run_slab.py` & `prodimopy-2.3/prodimopy/run_slab.py`

 * *Files 6% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 # C4H2,  HC3N,                                  H2,            CS,                        SO3, 
 5000.,   5000.,5000.,5000.,5000.,5000.,5000.,   6000.,6000.,   5000.,5000.,5000.,5000.,   3500.,
 # C2N2,        COCl2,        SO,                 CH3F    GeH4                          
 5000.,5000.,   5000.,5000.,  5000.,5000.,5000.,  5000.,  5000.,5000.,5000.,5000.,5000.,
 # CS2                       CH3I,         NF3     C3H4,    CH3,  
   5000.,5000.,5000.,5000.,  5000.,5000.,  5000.,  5000.,   5000.]
 
-def fetch_QT(mol,iso,T,QTpath):
+def fetch_QT(mol,iso,T,QTpath,T_limit='warn',verbose=True):
     '''
     Retrieve the partition sum from HITRAN QTpy files
 
     Parameters
     ----------
 
     mol : string
@@ -148,28 +148,53 @@
     QTpath : string
         Path pointing to directory containing the directory QTpy provided by HITRAN (see hitran.org)
     '''
     mol = int(QT_mol_id[mol])
     iso = int(iso)
     if not (iso>0 and iso<=QT_niso[mol]):
         raise ValueError('the range is',1,' to', QT_niso[mol],' try again')  
-    file = QTpath+'QTpy/'+str(mol)+'_'+str(iso)+'.QTpy'
+    file = QTpath+str(mol)+'_'+str(iso)+'.QTpy'
     QTdict = {}
     with open(file, 'rb') as handle:
         QTdict = pickle.loads(handle.read())
-    if (type(T) is int) or (type(T) is float):
+    if (type(T) is int) or (type(T) is float) or (type(T) is np.float64):
         if not (T>=1. and T<=QT_Tmax[np.sum(QT_niso[1:mol],dtype=int)+iso]):
-            raise ValueError('the temperature range is',1,' to', QT_Tmax[np.sum(QT_niso[1:mol],dtype=int)+iso],' try again')  
+            if T_limit=='warn':
+                if(T<1.):
+                    if verbose:
+                        print('WARNING: ',T,' falls below the temperature range ',1,' to', QT_Tmax[np.sum(QT_niso[1:mol],dtype=int)+iso])
+                        print('resetting T = 1')
+                    T = 1.
+                else:
+                    if verbose:
+                        print('WARNING: ',T,' falls above the temperature range ',1,' to', QT_Tmax[np.sum(QT_niso[1:mol],dtype=int)+iso])
+                        print('resetting T = ',QT_Tmax[np.sum(QT_niso[1:mol],dtype=int)+iso])
+                    T = QT_Tmax[np.sum(QT_niso[1:mol],dtype=int)+iso]
+            else:
+                raise ValueError('the temperature range is',1,' to', QT_Tmax[np.sum(QT_niso[1:mol],dtype=int)+iso],' try again')  
         Q1 = float(QTdict[str(int(T))])
-        Q2 = float(QTdict[str(int(T)+1)])
+        if T==QT_Tmax[np.sum(QT_niso[1:mol],dtype=int)+iso]:
+            Q2 = Q1
+        else:
+            Q2 = float(QTdict[str(int(T)+1)])
         QT = Q1+(Q2-Q1)*(T-int(T))
     else:
         T = np.array(T)
         if not (np.amin(T)>=1. and np.amax(T)<=QT_Tmax[np.sum(QT_niso[1:mol],dtype=int)+iso]):
-            raise ValueError('the temperature range is',1,' to', QT_Tmax[np.sum(QT_niso[1:mol],dtype=int)+iso],' try again')  
+            if T_limit=='warn':
+                if(T<1.):
+                    print('WARNING: ',T,' falls below the temperature range ',1,' to', QT_Tmax[np.sum(QT_niso[1:mol],dtype=int)+iso])
+                    print('resetting T = 1')
+                    T = 1.
+                else:
+                    print('WARNING: ',T,' falls above the temperature range ',1,' to', QT_Tmax[np.sum(QT_niso[1:mol],dtype=int)+iso])
+                    print('resetting T = ',QT_Tmax[np.sum(QT_niso[1:mol],dtype=int)+iso])
+                    T = QT_Tmax[np.sum(QT_niso[1:mol],dtype=int)+iso]
+            else:
+                raise ValueError('the temperature range is',1,' to', QT_Tmax[np.sum(QT_niso[1:mol],dtype=int)+iso],' try again')  
         QT = np.array([float(QTdict[str(int(t))])+(float(QTdict[str(int(t)+1)])-float(QTdict[str(int(t))]))*(t-int(t)) for t in T])
     return(QT)
 
 
 def run_0D_slab(Ng,Tg,vturb,molecule,mol_mass,HITRANfile,R_grid,QTpath,output_filename,isotopolog=[1],wave_mol=[4,30],wave_spec=[4.9,28]):
     '''
     This is a python implementation of 0D slab models, based on the FORTRAN version of 0D slab models in ProDiMo (https://prodimo.iwf.oeaw.ac.at/)
```

### Comparing `prodimopy-2.2.1/prodimopy/script_compare.py` & `prodimopy-2.3/prodimopy/script_compare.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 import argparse
 import os
 
 import prodimopy.compare as pcomp
 import prodimopy.read as pread
 import prodimopy.read_mc as pread_mc
+import prodimopy.read_slab as pread_slab
 
 
 # The main routine is require to have an entry point.
 # It is not necessary if you want to write your own script.
 def main(args=None):
   parser=argparse.ArgumentParser(description='Compares two ProDiMo models')
   parser.add_argument('model1',help='The directory/path of the first model used for the comparison.')
@@ -45,14 +46,19 @@
       print("\nRead model "+args.model2+"...")
       model2=pread_mc.read_mc("MC_Results.out",directory=args.model2)
     else:
       print("ERROR: Could not find MC outputfile.")
       return
 
     compare=pcomp.CompareMc(model1,model2)
+  elif pcomp.eval_model_type(args.model1)=="slab":
+    # FIXME: might not always be SlabResults.out ?! but I don't know
+    model1=pread_slab.read_slab(os.path.join(args.model1,"SlabResults.out"))
+    model2=pread_slab.read_slab(os.path.join(args.model2,"SlabResults.out"))
+    compare=pcomp.CompareSlab(model1,model2)
   else:
     print("\nRead model "+args.model1+"...")
     model1=pread.read_prodimo(args.model1,readlineEstimates=True,td_fileIdx=args.tdIdx1)
     print("\nRead model "+args.model2+"...")
     model2=pread.read_prodimo(args.model2,readlineEstimates=True,td_fileIdx=args.tdIdx1)
     compare=pcomp.Compare(model1,model2)
```

### Comparing `prodimopy-2.2.1/prodimopy/script_params.py` & `prodimopy-2.3/prodimopy/script_params.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.2.1/prodimopy/script_plot.py` & `prodimopy-2.3/prodimopy/script_plot.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.2.1/prodimopy/script_plot_models.py` & `prodimopy-2.3/prodimopy/script_plot_models.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.2.1/prodimopy/utils.py` & `prodimopy-2.3/prodimopy/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -72,28 +72,37 @@
   list
     the paramFileList
 
   _todo: This is quick and dirty ... maybe it is worth to make this more elegant and more flexible (e.g. its own class, allow to set comments etc.)
 
   """
 
+  # figure out if we can skip the line from the Parameter file
+  skipline=lambda pline: pline.strip()=="" or pline.strip().startswith("***") or pline.strip().startswith("---")
+  # find the Parameter in line from he Parameter file
+  findparam=lambda pline,param: (pline.strip()+" ").find(param)
+
+  # add a space to param
+  param=param.strip()+" "
+
   # delete the parameter
   if value.strip()=="DELETEPARAM":
     for i in range(len(paramFileList)):
-      if paramFileList[i].find(param)>-1:
+      if skipline(paramFileList[i]): continue
+      if findparam(paramFileList[i],param)>-1:
         print("delete line : "+paramFileList[i])
         paramFileList.pop(i)
         return paramFileList
     print("Parameter '"+param+"' not found.")
     return paramFileList
 
   replaced=False
   for i in range(len(paramFileList)):
-    # FIXME shouln"t that be `"! "+param
-    ip=paramFileList[i].find(param)
+    if skipline(paramFileList[i]): continue
+    ip=findparam(paramFileList[i],param)
     if ip>-1:
       val=paramFileList[i][0:ip-1]
       rest=paramFileList[i][ip:]
       lval=len(val)
       lnewval=len(value)
       if lval>lnewval:
         newval=value+" "*(lval-lnewval)+" "
```

### Comparing `prodimopy-2.2.1/prodimopy/utils_casasim.py` & `prodimopy-2.3/prodimopy/utils_casasim.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.2.1/prodimopy.egg-info/SOURCES.txt` & `prodimopy-2.3/prodimopy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 prodimopy/hitran.py
 prodimopy/movie.py
 prodimopy/plot.py
 prodimopy/plot_casasim.py
 prodimopy/plot_mc.py
 prodimopy/plot_models.py
 prodimopy/plot_slab.py
+prodimopy/postprocessing.py
 prodimopy/read.py
 prodimopy/read_casasim.py
 prodimopy/read_mc.py
 prodimopy/read_slab.py
 prodimopy/run_slab.py
 prodimopy/script_compare.py
 prodimopy/script_params.py
```

### Comparing `prodimopy-2.2.1/setup.py` & `prodimopy-2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 setup(
     name='prodimopy',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='2.2.1',
+    version='2.3',
 
     description='Python tools for ProDiMo.',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     # The project's main homepage.
     url='https://gitlab.astro.rug.nl/prodimo/prodimopy/',
```

