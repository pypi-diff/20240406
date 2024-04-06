# Comparing `tmp/pyrestoolbox-1.4.3.tar.gz` & `tmp/pyrestoolbox-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrestoolbox-1.4.3.tar", last modified: Sat Feb  3 23:36:06 2024, max compression
+gzip compressed data, was "pyrestoolbox-1.4.4.tar", last modified: Sat Apr  6 01:34:07 2024, max compression
```

## Comparing `pyrestoolbox-1.4.3.tar` & `pyrestoolbox-1.4.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-02-03 23:36:06.671030 pyrestoolbox-1.4.3/
--rw-rw-rw-   0        0        0    33092 2021-12-19 10:23:37.000000 pyrestoolbox-1.4.3/LICENSE
--rw-rw-rw-   0        0        0       37 2022-01-30 04:13:11.000000 pyrestoolbox-1.4.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6078 2024-02-03 23:36:06.671030 pyrestoolbox-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0    20534 2023-08-05 05:24:37.000000 pyrestoolbox-1.4.3/README.rst
--rw-rw-rw-   0        0        0      121 2022-01-07 02:09:05.000000 pyrestoolbox-1.4.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-02-03 23:36:06.623653 pyrestoolbox-1.4.3/pyrestoolbox/
--rw-rw-rw-   0        0        0        0 2022-01-07 01:15:07.000000 pyrestoolbox-1.4.3/pyrestoolbox/__init__.py
--rw-rw-rw-   0        0        0    42056 2023-09-12 04:37:21.000000 pyrestoolbox-1.4.3/pyrestoolbox/component_library.xlsx
--rw-rw-rw-   0        0        0   173692 2024-02-03 23:30:41.000000 pyrestoolbox-1.4.3/pyrestoolbox/pyrestoolbox.py
-drwxrwxrwx   0        0        0        0 2024-02-03 23:36:06.662014 pyrestoolbox-1.4.3/pyrestoolbox/simtools/
--rw-rw-rw-   0        0        0        0 2022-01-07 01:15:07.000000 pyrestoolbox-1.4.3/pyrestoolbox/simtools/__init__.py
--rw-rw-rw-   0        0        0    37326 2022-04-19 07:29:27.000000 pyrestoolbox-1.4.3/pyrestoolbox/simtools/simtools.py
-drwxrwxrwx   0        0        0        0 2024-02-03 23:36:06.671030 pyrestoolbox-1.4.3/pyrestoolbox.egg-info/
--rw-rw-rw-   0        0        0     6078 2024-02-03 23:36:06.000000 pyrestoolbox-1.4.3/pyrestoolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      401 2024-02-03 23:36:06.000000 pyrestoolbox-1.4.3/pyrestoolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-03 23:36:06.000000 pyrestoolbox-1.4.3/pyrestoolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-02-03 23:36:06.000000 pyrestoolbox-1.4.3/pyrestoolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-02-03 23:36:06.000000 pyrestoolbox-1.4.3/pyrestoolbox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      635 2024-02-03 23:36:06.671030 pyrestoolbox-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1205 2024-02-03 23:32:13.000000 pyrestoolbox-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 01:34:07.901225 pyrestoolbox-1.4.4/
+-rw-rw-rw-   0        0        0    33092 2021-12-19 10:23:37.000000 pyrestoolbox-1.4.4/LICENSE
+-rw-rw-rw-   0        0        0       37 2022-01-30 04:13:11.000000 pyrestoolbox-1.4.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     6247 2024-04-06 01:34:07.900225 pyrestoolbox-1.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0    20534 2023-08-05 05:24:37.000000 pyrestoolbox-1.4.4/README.rst
+-rw-rw-rw-   0        0        0      121 2022-01-07 02:09:05.000000 pyrestoolbox-1.4.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-06 01:34:07.871313 pyrestoolbox-1.4.4/pyrestoolbox/
+-rw-rw-rw-   0        0        0        0 2022-01-07 01:15:07.000000 pyrestoolbox-1.4.4/pyrestoolbox/__init__.py
+-rw-rw-rw-   0        0        0    42056 2023-09-12 04:37:21.000000 pyrestoolbox-1.4.4/pyrestoolbox/component_library.xlsx
+-rw-rw-rw-   0        0        0   176609 2024-04-04 21:51:20.000000 pyrestoolbox-1.4.4/pyrestoolbox/pyrestoolbox.py
+drwxrwxrwx   0        0        0        0 2024-04-06 01:34:07.894699 pyrestoolbox-1.4.4/pyrestoolbox/simtools/
+-rw-rw-rw-   0        0        0        0 2022-01-07 01:15:07.000000 pyrestoolbox-1.4.4/pyrestoolbox/simtools/__init__.py
+-rw-rw-rw-   0        0        0    37326 2022-04-19 07:29:27.000000 pyrestoolbox-1.4.4/pyrestoolbox/simtools/simtools.py
+drwxrwxrwx   0        0        0        0 2024-04-06 01:34:07.898225 pyrestoolbox-1.4.4/pyrestoolbox.egg-info/
+-rw-rw-rw-   0        0        0     6247 2024-04-06 01:34:07.000000 pyrestoolbox-1.4.4/pyrestoolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      401 2024-04-06 01:34:07.000000 pyrestoolbox-1.4.4/pyrestoolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 01:34:07.000000 pyrestoolbox-1.4.4/pyrestoolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2024-04-06 01:34:07.000000 pyrestoolbox-1.4.4/pyrestoolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-06 01:34:07.000000 pyrestoolbox-1.4.4/pyrestoolbox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      648 2024-04-06 01:34:07.903409 pyrestoolbox-1.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1228 2024-04-06 01:08:57.000000 pyrestoolbox-1.4.4/setup.py
```

### Comparing `pyrestoolbox-1.4.3/LICENSE` & `pyrestoolbox-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrestoolbox-1.4.3/PKG-INFO` & `pyrestoolbox-1.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrestoolbox
-Version: 1.4.3
+Version: 1.4.4
 Summary: pyResToolbox - A collection of Reservoir Engineering Utilities
 Home-page: https://github.com/mwburgoyne/pyResToolbox
 Author: Mark W. Burgoyne
 Author-email: mark.w.burgoyne@gmail.com
 Keywords: restoolbox,petroleum,reservoir
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -15,14 +15,15 @@
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: tabulate
 Requires-Dist: gwr_inversion
 Requires-Dist: mpmath
 Requires-Dist: openpyxl
+Requires-Dist: setuptools
 
 `pyrestoolbox`
 ==============
 
 \-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\--
 A collection of Reservoir Engineering Utilities
 \-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\--
@@ -49,14 +50,17 @@
 -   Creation of Corey and LET relative permeability tables in Eclipse
     format
 -   Calculation of Methane and CO2 saturated brine properties
 
 Apologies in advance that it is only in oilfield
 units with no current plans to add universal multi-unit support.
 
+Changelist in 1.4.4:
+- Added in new Z-Factor method, 'PR', which is a tuned single component Peng Robinson method that is fast and stable
+
 Changelist in 1.4.2:
 - Corrected CO2 solubility calculations when two roots in CO2 liquid phase
 
 Changelist in 1.4.1:
 - Added calculation of Ezrokhi coefficients for brine density and viscosity with dissolved CO2
 
 Changelist in 1.4.0:
```

### Comparing `pyrestoolbox-1.4.3/README.rst` & `pyrestoolbox-1.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `pyrestoolbox-1.4.3/pyrestoolbox/component_library.xlsx` & `pyrestoolbox-1.4.4/pyrestoolbox/component_library.xlsx`

 * *Files identical despite different names*

### Comparing `pyrestoolbox-1.4.3/pyrestoolbox/pyrestoolbox.py` & `pyrestoolbox-1.4.4/pyrestoolbox/pyrestoolbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 scf_per_mol = R * tscr / psc  # scf/lb-mol (V = ZnRT/P, Z = 1, n = 1)
 
 
 class z_method(Enum):  # Gas Z-Factor calculation model
     DAK = 0
     HY = 1
     WYW = 2
+    PR = 3
 
 
 class c_method(Enum):  # Gas critical properties calculation method
     PMC = 0
     SUT = 1
 
 
@@ -178,14 +179,15 @@
         r_w: Wellbore Radius (ft)
         r_ext: External Reservoir Radius (ft)
         degf: Reservoir Temperature (deg F)
         zmethod: Method for calculating Z-Factor
                  'DAK' Dranchuk & Abou-Kassem (1975) using from Equations 2.7-2.8 from 'Petroleum Reservoir Fluid Property Correlations' by W. McCain et al.
                  'HY' Hall & Yarborough (1973)
                  'WYW' Wang, Ye & Wu (2021)
+                 'PR' Tuned single component Peng Robinson EOS model (Unpublished, created by M. Burgoyne 2024)
                  defaults to 'DAK' if not specified
         cmethod: Method for calculating critical properties
                'SUT' for Sutton with Wichert & Aziz non-hydrocarbon corrections, or
                'PMC' for Piper, McCain & Corredor (1999) correlation, using equations 2.4 - 2.6 from 'Petroleum Reservoir Fluid Property Correlations' by W. McCain et al.
                Defaults to 'PMC'
         tc: Critical gas temperature (deg R). Uses cmethod correlation if not specified
         pc: Critical gas pressure (psia). Uses cmethod correlation if not specified
@@ -302,14 +304,15 @@
         pwf: BHFP (psia)
         area: Net cross sectional area perpendicular to direction of flow (ft2).
         length: Length over which flow takes place (ft)
         zmethod: Method for calculating Z-Factor
                  'DAK' Dranchuk & Abou-Kassem (1975) using from Equations 2.7-2.8 from 'Petroleum Reservoir Fluid Property Correlations' by W. McCain et al.
                  'HY' Hall & Yarborough (1973)
                  'WYW' Wang, Ye & Wu (2021)
+                 'PR' Tuned single component Peng Robinson EOS model (Unpublished, created by M. Burgoyne 2024)
                  defaults to 'DAK' if not specified
         cmethod: Method for calculting critical properties
                'SUT' for Sutton with Wichert & Aziz non-hydrocarbon corrections, or
                'PMC' for Piper, McCain & Corredor (1999) correlation, using equations 2.4 - 2.6 from 'Petroleum Reservoir Fluid Property Correlations' by W. McCain et al.
                Defaults to 'PMC' if not specified
         tc: Critical gas temperature (deg R). Uses cmethod correlation if not specified
         pc: Critical gas pressure (psia). Uses cmethod correlation if not specified
@@ -550,14 +553,15 @@
         p: Gas pressure (psia). Takes a single float, 1D list or 1D Numpy array
         sg: Gas SG relative to air. Single float only
         degf: Gas Temperature (deg F). Single float only
         zmethod: Method for calculating Z-Factor
                  'DAK' Dranchuk & Abou-Kassem (1975) using from Equations 2.7-2.8 from 'Petroleum Reservoir Fluid Property Correlations' by W. McCain et al.
                  'HY' Hall & Yarborough (1973)
                  'WYW' Wang, Ye & Wu (2021)
+                 'PR' Tuned single component Peng Robinson EOS model (Unpublished, created by M. Burgoyne 2024)
                  defaults to 'DAK' if not specified
         cmethod: Method for calculting critical properties
                'SUT' for Sutton with Wichert & Aziz non-hydrocarbon corrections, or
                'PMC' for Piper, McCain & Corredor (1999) correlation, using equations 2.4 - 2.6 from 'Petroleum Reservoir Fluid Property Correlations' by W. McCain et al.
                Defaults to 'PMC'
         tc: Critical gas temperature (deg R). Uses cmethod correlation if not specified
         pc: Critical gas pressure (psia). Uses cmethod correlation if not specified
@@ -631,23 +635,23 @@
             z2 = (1 + c1*rhor + c2*rhor**2 - c3 * rhor**5 + c4)
             return z2 - z        
             
         def z_dak_calc(pr, tr, tol = 1e-6):
             niter = 0
             minppr = min_ppr(tr)
             
-            if abs(pr - minppr) > 0.05: # If Ppr is further from calculated minimum Ppr than 0.05, use Netwon solver
+            if abs(pr - minppr) > 0.05: # If Ppr is further from calculated minimum Ppr than 0.05, use Newton solver
                 newton_solve = True
             else:
                 newton_solve = False    # Else, use bisection solver, and setup Z bounds to search within
                 minz = fit_minz(tr)
                 bounds = (minz - 0.02, minz + 0.02)
     
             if newton_solve:
-                midz = min(max(0.1, z_wyw(pr, tr)),3) # First guess using explict calculation method
+                midz = min(max(0.1, z_pr([pr], tr)),3) # First guess using explicit calculation method
                 mid_err = 1
                 while abs(mid_err) > tol and niter < 100:
                     midz, mid_err = new_dak_z(midz, pr, tr)
                     niter += 1
             else:
                 midz = brentq(z_err, bounds[0], bounds[1], args=(pr))  
             return midz
@@ -702,15 +706,68 @@
         zs = numerators/denominators
 
         if single_p:
             return float(zs)
         else:
             return zs
 
-    zfuncs = {"DAK": zdak, "HY": z_hy, "WYW": z_wyw}
+    def z_pr(pprs, tr):
+        
+        # Analytic solution for maximum real root of cubic polynomial
+        # a[0] * Z^3 + a[1]*Z^2 + a[2]*Z + a[3] = 0
+        def max_root(a):
+            p = (3 * a[2]- a[1]**2)/3
+            q = (2 * a[1]**3 - 9 * a[1] * a[2] + 27 * a[3])/27
+            root_diagnostic = q**2/4 + p**3/27
+
+            if root_diagnostic < 0:
+                m = 2*np.sqrt(-p/3)
+                qpm = 3*q/p/m
+                theta1 = np.arccos(qpm)/3
+                roots = np.array([m*np.cos(theta1), m*np.cos(theta1+4*np.pi/3), m*np.cos(theta1+2*np.pi/3)])
+                Zs = roots - a[1] / 3
+            else:
+                P = (-q/2 + np.sqrt(root_diagnostic))
+                if P >= 0:
+                    P = P **(1/3)
+                else:
+                    P = -(-P)**(1/3)
+            
+                Q = (-q/2 - np.sqrt(root_diagnostic))
+                if Q >=0:
+                    Q = Q **(1/3)
+                else:
+                    Q = -(-Q)**(1/3)
+                Zs = np.array([P + Q]) - a[1] / 3
+            return max(Zs)
+    
+        w, s = -0.048964, -0.394899
+        m = 0.37464 + 1.54226 * w - 0.26992 * w**2
+        alpha = (1 + m * (1 - np.sqrt(tr)))**2    
+        
+        zout = []
+        for pr in pprs:
+            A = 0.429188 * alpha * pr / tr**2
+            B = 0.0692551 * pr / tr
+    
+            # Coefficients of Cubic: a[0] * Z^3 + a[1]*Z^2 + a[2]*Z + a[3] = 0
+            a = [1, -(1 - B), A - 3 * B**2 - 2 * B, -(A * B - B**2 - B**3)]  
+            zout.append(max_root(a) - s * B) # Volume translated Z          
+                
+        if single_p:
+            return zout[0]
+        else:
+            return np.array(zout)
+            
+        if single_p:
+            return float(zs)
+        else:
+            return zs
+            
+    zfuncs = {"DAK": zdak, "HY": z_hy, "WYW": z_wyw, "PR": z_pr}
 
     return zfuncs[zmethod.name](pprs, tr)
 
 
 def gas_ug(
     p: npt.ArrayLike,
     sg: float,
@@ -729,14 +786,15 @@
           p: Gas pressure (psia)
           sg: Gas SG relative to air
           degf: Reservoir Temperature (deg F).
           zmethod: Method for calculating Z-Factor
                    'DAK' Dranchuk & Abou-Kassem (1975) using from Equations 2.7-2.8 from 'Petroleum Reservoir Fluid Property Correlations' by W. McCain et al.
                    'HY' Hall & Yarborough (1973)
                    'WYW' Wang, Ye & Wu (2021)
+                   'PR' Tuned single component Peng Robinson EOS model (Unpublished, created by M. Burgoyne 2024)
                    defaults to 'DAK' if not specified
           cmethod: Method for calculting critical properties
                    'SUT' for Sutton with Wichert & Aziz non-hydrocarbon corrections, or
                    'PMC' for Piper, McCain & Corredor (1999) correlation, using equations 2.4 - 2.6 from 'Petroleum Reservoir Fluid Property Correlations' by W. McCain et al.
                    Defaults to 'PMC'
           tc: Critical gas temperature (deg R). Calculates using cmethod if not specified
           pc: Critical gas pressure (psia). Calculates using cmethod if not specified
@@ -874,14 +932,15 @@
     pc: float = 0,
 ) -> np.ndarray:
     """ Returns Bg (gas formation volume factor) for natural gas (rcf/scf)
         zmethod: Method for calculating Z-Factor
                  'DAK' Dranchuk & Abou-Kassem (1975) using from Equations 2.7-2.8 from 'Petroleum Reservoir Fluid Property Correlations' by W. McCain et al.
                  'HY' Hall & Yarborough (1973)
                  'WYW' Wang, Ye & Wu (2021)
+                 'PR' Tuned single component Peng Robinson EOS model (Unpublished, created by M. Burgoyne 2024)
                  defaults to 'DAK' if not specified
         cmethod: Method for calculting critical properties
                  'SUT' for Sutton with Wichert & Aziz non-hydrocarbon corrections, or
                  'PMC' for Piper, McCain & Corredor (1999) correlation, using equations 2.4 - 2.6 from 'Petroleum Reservoir Fluid Property Correlations' by W. McCain et al.
                  Defaults to 'PMC'
           p: Gas pressure (psia)
           tc: Critical gas temperature (deg R). Calculates using cmethod if not specified
@@ -926,14 +985,15 @@
 ) -> np.ndarray:
     """ Returns gas density for natural gas (lb/cuft)
 
           zmethod: Method for calculating Z-Factor
                    'DAK' Dranchuk & Abou-Kassem (1975) using from Equations 2.7-2.8 from 'Petroleum Reservoir Fluid Property Correlations' by W. McCain et al.
                    'HY' Hall & Yarborough (1973)
                    'WYW' Wang, Ye & Wu (2021)
+                   'PR' Tuned single component Peng Robinson EOS model (Unpublished, created by M. Burgoyne 2024)
                    defaults to 'DAK' if not specified
           cmethod: Method for calculting critical properties
                    'sut' for Sutton with Wichert & Aziz non-hydrocarbon corrections, or
                    'pmc' for Piper, McCain & Corredor (1999) correlation, using equations 2.4 - 2.6 from 'Petroleum Reservoir Fluid Property Correlations' by W. McCain et al.
                    Defaults to 'pmc'
           p: Gas pressure (psia)
           tc: Critical gas temperature (deg R). Calculates using cmethod if not specified
@@ -984,14 +1044,15 @@
         Calculated through iterative solution method
         poverz: Gas pressure / Z-Factor (psia)
 
         zmethod: Method for calculating Z-Factor
                  'DAK' Dranchuk & Abou-Kassem (1975) using from Equations 2.7-2.8 from 'Petroleum Reservoir Fluid Property Correlations' by W. McCain et al.
                  'HY' Hall & Yarborough (1973)
                  'WYW' Wang, Ye & Wu (2021)
+                 'PR' Tuned single component Peng Robinson EOS model (Unpublished, created by M. Burgoyne 2024)
                  defaults to 'DAK' if not specified
         cmethod: Method for calculting critical properties
                  'SUT' for Sutton with Wichert & Aziz non-hydrocarbon corrections, or
                  'PMC' for Piper, McCain & Corredor (1999) correlation, using equations 2.4 - 2.6 from 'Petroleum Reservoir Fluid Property Correlations' by W. McCain et al.
                  Defaults to 'PMC'
           tc: Critical gas temperature (deg R). Calculates using cmethod if not specified
           pc: Critical gas pressure (psia). Calculates using cmethod if not specified
@@ -1060,14 +1121,15 @@
         grad: Observed gas gradient (psi/ft)
         p: Pressure at observation (psia)
         degf: Reservoir Temperature (deg F). Defaults to False if undefined
         zmethod: Method for calculating Z-Factor
                  'DAK' Dranchuk & Abou-Kassem (1975) using from Equations 2.7-2.8 from 'Petroleum Reservoir Fluid Property Correlations' by W. McCain et al.
                  'HY' Hall & Yarborough (1973)
                  'WYW' Wang, Ye & Wu (2021)
+                 'PR' Tuned single component Peng Robinson EOS model (Unpublished, created by M. Burgoyne 2024)
                  defaults to 'DAK' if not specified
         cmethod: Method for calculting critical properties
                  'SUT' for Sutton with Wichert & Aziz non-hydrocarbon corrections, or
                  'PMC' for Piper, McCain & Corredor (1999) correlation, using equations 2.4 - 2.6 from 'Petroleum Reservoir Fluid Property Correlations' by W. McCain et al.
                  Defaults to 'PMC'
           tc: Critical gas temperature (deg R). Calculates using cmethod if not specified
           pc: Critical gas pressure (psia). Calculates using cmethod if not specified
@@ -1126,14 +1188,15 @@
         p2: Ending (upper) pressure (psia)
         t: Gas Temperature (deg F)
         sg: Specific gravity of  gas (relative to air)
         zmethod: Method for calculating Z-Factor
                    'DAK' Dranchuk & Abou-Kassem (1975) using from Equations 2.7-2.8 from 'Petroleum Reservoir Fluid Property Correlations' by W. McCain et al.
                    'HY' Hall & Yarborough (1973)
                    'WYW' Wang, Ye & Wu (2021)
+                   'PR' Tuned single component Peng Robinson EOS model (Unpublished, created by M. Burgoyne 2024)
                    defaults to 'DAK' if not specified
         cmethod: Method for calculting critical properties
                  'sut' for Sutton with Wichert & Aziz non-hydrocarbon corrections, or
                  'pmc' for Piper, McCain & Corredor (1999) correlation, using equations 2.4 - 2.6 from 'Petroleum Reservoir Fluid Property Correlations' by W. McCain et al.
                  Defaults to 'pmc'
         tc: Critical gas temperature (deg R). Calculates using cmethod if not specified
         pc: Critical gas pressure (psia). Calculates using cmethod if not specified
```

### Comparing `pyrestoolbox-1.4.3/pyrestoolbox/simtools/simtools.py` & `pyrestoolbox-1.4.4/pyrestoolbox/simtools/simtools.py`

 * *Files identical despite different names*

### Comparing `pyrestoolbox-1.4.3/pyrestoolbox.egg-info/PKG-INFO` & `pyrestoolbox-1.4.4/pyrestoolbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrestoolbox
-Version: 1.4.3
+Version: 1.4.4
 Summary: pyResToolbox - A collection of Reservoir Engineering Utilities
 Home-page: https://github.com/mwburgoyne/pyResToolbox
 Author: Mark W. Burgoyne
 Author-email: mark.w.burgoyne@gmail.com
 Keywords: restoolbox,petroleum,reservoir
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -15,14 +15,15 @@
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: tabulate
 Requires-Dist: gwr_inversion
 Requires-Dist: mpmath
 Requires-Dist: openpyxl
+Requires-Dist: setuptools
 
 `pyrestoolbox`
 ==============
 
 \-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\--
 A collection of Reservoir Engineering Utilities
 \-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\--
@@ -49,14 +50,17 @@
 -   Creation of Corey and LET relative permeability tables in Eclipse
     format
 -   Calculation of Methane and CO2 saturated brine properties
 
 Apologies in advance that it is only in oilfield
 units with no current plans to add universal multi-unit support.
 
+Changelist in 1.4.4:
+- Added in new Z-Factor method, 'PR', which is a tuned single component Peng Robinson method that is fast and stable
+
 Changelist in 1.4.2:
 - Corrected CO2 solubility calculations when two roots in CO2 liquid phase
 
 Changelist in 1.4.1:
 - Added calculation of Ezrokhi coefficients for brine density and viscosity with dissolved CO2
 
 Changelist in 1.4.0:
```

### Comparing `pyrestoolbox-1.4.3/setup.cfg` & `pyrestoolbox-1.4.4/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6465 7363  [metadata]..desc
 00000010: 7269 7074 696f 6e5f 6669 6c65 203d 2052  ription_file = R
 00000020: 4541 444d 452e 6d64 0d0a 6e61 6d65 203d  EADME.md..name =
 00000030: 2070 7972 6573 746f 6f6c 626f 780d 0a76   pyrestoolbox..v
-00000040: 6572 7369 6f6e 203d 2031 2e34 2e33 0d0a  ersion = 1.4.3..
+00000040: 6572 7369 6f6e 203d 2031 2e34 2e34 0d0a  ersion = 1.4.4..
 00000050: 6175 7468 6f72 203d 204d 6172 6b20 572e  author = Mark W.
 00000060: 2042 7572 676f 796e 650d 0a61 7574 686f   Burgoyne..autho
 00000070: 725f 656d 6169 6c20 3d20 6d61 726b 2e77  r_email = mark.w
 00000080: 2e62 7572 676f 796e 6540 676d 6169 6c2e  .burgoyne@gmail.
 00000090: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 000000a0: 203d 2070 7952 6573 546f 6f6c 626f 7820   = pyResToolbox 
 000000b0: 2d20 4120 636f 6c6c 6563 7469 6f6e 206f  - A collection o
@@ -30,11 +30,12 @@
 000001d0: 6573 203d 205b 2770 7972 6573 746f 6f6c  es = ['pyrestool
 000001e0: 626f 7827 5d0d 0a69 6e73 7461 6c6c 5f72  box']..install_r
 000001f0: 6571 7569 7265 7320 3d20 0d0a 0972 6571  equires = ...req
 00000200: 7565 7374 730d 0a09 6e75 6d70 790d 0a09  uests...numpy...
 00000210: 7363 6970 790d 0a09 7061 6e64 6173 0d0a  scipy...pandas..
 00000220: 0974 6162 756c 6174 650d 0a09 6777 725f  .tabulate...gwr_
 00000230: 696e 7665 7273 696f 6e0d 0a09 6d70 6d61  inversion...mpma
-00000240: 7468 0d0a 096f 7065 6e70 7978 6c0d 0a0d  th...openpyxl...
-00000250: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
-00000260: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
-00000270: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
+00000240: 7468 0d0a 096f 7065 6e70 7978 6c0d 0a09  th...openpyxl...
+00000250: 7365 7475 7074 6f6f 6c73 0d0a 0d0a 5b65  setuptools....[e
+00000260: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
+00000270: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
+00000280: 203d 2030 0d0a 0d0a                       = 0....
```

### Comparing `pyrestoolbox-1.4.3/setup.py` & `pyrestoolbox-1.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 f = open('C:\\Users\\vinom\OneDrive - Santos\\Work in progress\\Python\\0-ResEng\\pyResToolbox\\source_dir\\README.md', 'r').read()
 long_description= f #markdown.markdown( f.read() )
 
 setup(
     name = 'pyrestoolbox',
     packages = find_packages(),
     include_package_data=True,
-    version = '1.4.3',  # Ideally should be same as your GitHub release tag varsion
+    version = '1.4.4',  # Ideally should be same as your GitHub release tag varsion
     description = 'pyResToolbox - A collection of Reservoir Engineering Utilities',
     long_description= long_description,
     long_description_content_type = 'text/markdown',
     author = 'Mark W. Burgoyne',
     author_email = 'mark.w.burgoyne@gmail.com',
     url = 'https://github.com/mwburgoyne/pyResToolbox',
     keywords = ['restoolbox', 'petroleum', 'reservoir'],
@@ -29,10 +29,11 @@
         'requests',
         'numpy',
         'scipy',
         'pandas',
         'tabulate',
         'gwr_inversion',
         'mpmath',
-        'openpyxl'
+        'openpyxl',
+        'setuptools'
     ]
 )
```

