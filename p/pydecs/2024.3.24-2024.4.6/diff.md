# Comparing `tmp/pydecs-2024.3.24.tar.gz` & `tmp/pydecs-2024.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydecs-2024.3.24.tar", last modified: Sun Mar 24 08:47:52 2024, max compression
+gzip compressed data, was "pydecs-2024.4.6.tar", last modified: Sat Apr  6 08:01:57 2024, max compression
```

## Comparing `pydecs-2024.3.24.tar` & `pydecs-2024.4.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        0 2024-03-24 08:47:52.936966 pydecs-2024.3.24/
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    11357 2024-03-24 02:21:06.000000 pydecs-2024.3.24/LICENSE.txt
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      647 2024-03-24 08:47:52.927911 pydecs-2024.3.24/PKG-INFO
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      484 2024-03-24 02:21:06.000000 pydecs-2024.3.24/README.md
-drwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        0 2024-03-24 08:47:52.477366 pydecs-2024.3.24/pydecs/
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      257 2024-03-24 02:21:08.000000 pydecs-2024.3.24/pydecs/__init__.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    36214 2024-03-24 02:21:08.000000 pydecs-2024.3.24/pydecs/aux_EdefCorrection_VASP.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     2258 2024-03-24 02:21:08.000000 pydecs-2024.3.24/pydecs/aux_check_equilibrium_phases.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     6569 2024-03-24 02:21:08.000000 pydecs-2024.3.24/pydecs/aux_convDOS.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     1343 2024-03-24 02:21:08.000000 pydecs-2024.3.24/pydecs/aux_convGasEne.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     1855 2024-03-24 02:21:08.000000 pydecs-2024.3.24/pydecs/aux_plot_defectdata.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      671 2024-03-24 02:21:08.000000 pydecs-2024.3.24/pydecs/common.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    13630 2024-03-24 03:34:53.000000 pydecs-2024.3.24/pydecs/defects.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    22348 2024-03-24 02:21:08.000000 pydecs-2024.3.24/pydecs/eqcond.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     7104 2024-03-24 03:35:14.000000 pydecs-2024.3.24/pydecs/host.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    67472 2024-03-24 08:38:42.000000 pydecs-2024.3.24/pydecs/inout.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     4681 2024-03-24 02:21:08.000000 pydecs-2024.3.24/pydecs/pydecs.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     9491 2024-03-24 02:21:08.000000 pydecs-2024.3.24/pydecs/reference_phases.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    32689 2024-03-24 02:21:08.000000 pydecs-2024.3.24/pydecs/solver.py
-drwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        0 2024-03-24 08:47:52.889670 pydecs-2024.3.24/pydecs.egg-info/
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      647 2024-03-24 08:47:51.000000 pydecs-2024.3.24/pydecs.egg-info/PKG-INFO
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      570 2024-03-24 08:47:51.000000 pydecs-2024.3.24/pydecs.egg-info/SOURCES.txt
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        1 2024-03-24 08:47:51.000000 pydecs-2024.3.24/pydecs.egg-info/dependency_links.txt
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      420 2024-03-24 08:47:51.000000 pydecs-2024.3.24/pydecs.egg-info/entry_points.txt
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        1 2024-03-24 08:47:51.000000 pydecs-2024.3.24/pydecs.egg-info/not-zip-safe
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)       35 2024-03-24 08:47:51.000000 pydecs-2024.3.24/pydecs.egg-info/requires.txt
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        7 2024-03-24 08:47:51.000000 pydecs-2024.3.24/pydecs.egg-info/top_level.txt
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)       91 2024-03-24 02:21:08.000000 pydecs-2024.3.24/pyproject.toml
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     1098 2024-03-24 08:47:52.950051 pydecs-2024.3.24/setup.cfg
+drwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        0 2024-04-06 08:01:57.842695 pydecs-2024.4.6/
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    11357 2024-04-06 07:44:30.000000 pydecs-2024.4.6/LICENSE.txt
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      646 2024-04-06 08:01:57.834600 pydecs-2024.4.6/PKG-INFO
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      484 2024-04-06 07:44:30.000000 pydecs-2024.4.6/README.md
+drwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        0 2024-04-06 08:01:57.596332 pydecs-2024.4.6/pydecs/
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      257 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/__init__.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    36214 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/aux_EdefCorrection_VASP.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     2700 2024-04-06 07:59:58.000000 pydecs-2024.4.6/pydecs/aux_check_equilibrium_phases.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     6569 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/aux_convDOS.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     1343 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/aux_convGasEne.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     1855 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/aux_plot_defectdata.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      671 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/common.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    13630 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/defects.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    22348 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/eqcond.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     7104 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/host.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    67472 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/inout.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     4681 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/pydecs.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     9491 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/reference_phases.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    32689 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/solver.py
+drwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        0 2024-04-06 08:01:57.816057 pydecs-2024.4.6/pydecs.egg-info/
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      646 2024-04-06 08:01:56.000000 pydecs-2024.4.6/pydecs.egg-info/PKG-INFO
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      570 2024-04-06 08:01:57.000000 pydecs-2024.4.6/pydecs.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        1 2024-04-06 08:01:56.000000 pydecs-2024.4.6/pydecs.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      420 2024-04-06 08:01:56.000000 pydecs-2024.4.6/pydecs.egg-info/entry_points.txt
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        1 2024-04-06 08:01:56.000000 pydecs-2024.4.6/pydecs.egg-info/not-zip-safe
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)       35 2024-04-06 08:01:56.000000 pydecs-2024.4.6/pydecs.egg-info/requires.txt
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        7 2024-04-06 08:01:56.000000 pydecs-2024.4.6/pydecs.egg-info/top_level.txt
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)       91 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pyproject.toml
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     1098 2024-04-06 08:01:57.853235 pydecs-2024.4.6/setup.cfg
```

### Comparing `pydecs-2024.3.24/LICENSE.txt` & `pydecs-2024.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydecs-2024.3.24/PKG-INFO` & `pydecs-2024.4.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydecs
-Version: 2024.3.24
+Version: 2024.4.6
 Summary: This tool enables us to analyze equilibrium concentrations of point and complex defects in crystalline solids
 Home-page: https://gitlab.com/tkog/pydecs
 Author: Takafumi Ogawa
 Author-email: takafumi.ogawa.1+pydecs@gmail.com
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `pydecs-2024.3.24/pydecs/aux_EdefCorrection_VASP.py` & `pydecs-2024.4.6/pydecs/aux_EdefCorrection_VASP.py`

 * *Files identical despite different names*

### Comparing `pydecs-2024.3.24/pydecs/aux_check_equilibrium_phases.py` & `pydecs-2024.4.6/pydecs/aux_check_equilibrium_phases.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,31 +9,38 @@
 import numpy as np
 import datetime
 from scipy.spatial import ConvexHull
 
 from pydecs.reference_phases import ReferencePhases
 
 def check_equilibrium_phases_0K():
+    fout_rp = open("outpydecs_checked_EqPhase.txt","w")
     print("-"*60)
     print(" Checking equilibrium phases")
     print(" Parsed files: inpydecs_phases.csv")
-    refPhase=ReferencePhases()
+    fout_rp.write("-"*60+"\n")
+    fout_rp.write(" Checking equilibrium phases\n")
+    fout_rp.write(" Parsed files: inpydecs_phases.csv\n")
+    refPhase=ReferencePhases("host",["./"],fout_rp)
     phaseList=refPhase.get_phaseList()
     print("-"*60)
+    fout_rp.write("-"*60+"\n")
     ph_host=refPhase.get_host(phaseList)
     comp_host=ph_host["composition"]
     atoms_host=ph_host["composition_dict"]
     elems_host=list(atoms_host.keys())
     num_elems=len(elems_host)
     pointsList = []
     compList=[]
     print(" Accounted compounds")
+    fout_rp.write(" Accounted compounds\n")
     for ph1 in phaseList:
         c1=ph1["composition"]
         print("  "+c1)
+        fout_rp.write("  "+c1+"\n")
         compList.append(c1)
         atoms=ph1["composition_dict"]
         ene0K=ph1["energy_0K"]
         ntot=0
         for n1 in atoms.values():
             ntot+=n1
         point1=np.zeros(num_elems)
@@ -52,20 +59,23 @@
             for is1 in simp1:
                 c1=compList[is1]
                 if c1!=comp_host:
                     comp_simp.append(c1)
             simpList.append(comp_simp)
     print("-"*60)
     print(" Simpleces list")
+    fout_rp.write("-"*60+"\n")
+    fout_rp.write(" Simpleces list\n")
     for simp1 in simpList:
         str1="  "
         for comp1 in simp1:
             str1+=comp1+" + "
         str1=str1[:-2]
         print(str1)
+        fout_rp.write(str1+"\n")
 
 
 if __name__=="__main__":
     check_equilibrium_phases_0K()
```

### Comparing `pydecs-2024.3.24/pydecs/aux_convDOS.py` & `pydecs-2024.4.6/pydecs/aux_convDOS.py`

 * *Files identical despite different names*

### Comparing `pydecs-2024.3.24/pydecs/aux_convGasEne.py` & `pydecs-2024.4.6/pydecs/aux_convGasEne.py`

 * *Files identical despite different names*

### Comparing `pydecs-2024.3.24/pydecs/aux_plot_defectdata.py` & `pydecs-2024.4.6/pydecs/aux_plot_defectdata.py`

 * *Files identical despite different names*

### Comparing `pydecs-2024.3.24/pydecs/common.py` & `pydecs-2024.4.6/pydecs/common.py`

 * *Files identical despite different names*

### Comparing `pydecs-2024.3.24/pydecs/defects.py` & `pydecs-2024.4.6/pydecs/defects.py`

 * *Files identical despite different names*

### Comparing `pydecs-2024.3.24/pydecs/eqcond.py` & `pydecs-2024.4.6/pydecs/eqcond.py`

 * *Files identical despite different names*

### Comparing `pydecs-2024.3.24/pydecs/host.py` & `pydecs-2024.4.6/pydecs/host.py`

 * *Files identical despite different names*

### Comparing `pydecs-2024.3.24/pydecs/inout.py` & `pydecs-2024.4.6/pydecs/inout.py`

 * *Files identical despite different names*

### Comparing `pydecs-2024.3.24/pydecs/pydecs.py` & `pydecs-2024.4.6/pydecs/pydecs.py`

 * *Files identical despite different names*

### Comparing `pydecs-2024.3.24/pydecs/reference_phases.py` & `pydecs-2024.4.6/pydecs/reference_phases.py`

 * *Files identical despite different names*

### Comparing `pydecs-2024.3.24/pydecs/solver.py` & `pydecs-2024.4.6/pydecs/solver.py`

 * *Files identical despite different names*

### Comparing `pydecs-2024.3.24/pydecs.egg-info/PKG-INFO` & `pydecs-2024.4.6/pydecs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydecs
-Version: 2024.3.24
+Version: 2024.4.6
 Summary: This tool enables us to analyze equilibrium concentrations of point and complex defects in crystalline solids
 Home-page: https://gitlab.com/tkog/pydecs
 Author: Takafumi Ogawa
 Author-email: takafumi.ogawa.1+pydecs@gmail.com
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `pydecs-2024.3.24/pydecs.egg-info/SOURCES.txt` & `pydecs-2024.4.6/pydecs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydecs-2024.3.24/setup.cfg` & `pydecs-2024.4.6/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pydecs
-version = 2024.03.24
+version = 2024.04.06
 description = This tool enables us to analyze equilibrium concentrations of point and complex defects in crystalline solids
 author = Takafumi Ogawa
 author_email = takafumi.ogawa.1+pydecs@gmail.com
 url = https://gitlab.com/tkog/pydecs
 lisense_file = LICENSE.txt
 classifiers = 
 	Intended Audience :: Science/Research
```

