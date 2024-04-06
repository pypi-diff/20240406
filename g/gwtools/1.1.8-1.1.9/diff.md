# Comparing `tmp/gwtools-1.1.8.tar.gz` & `tmp/gwtools-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwtools-1.1.8.tar", last modified: Sat Feb 24 14:05:59 2024, max compression
+gzip compressed data, was "gwtools-1.1.9.tar", last modified: Sat Apr  6 14:33:28 2024, max compression
```

## Comparing `gwtools-1.1.8.tar` & `gwtools-1.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 balzani57  (1000) balzani57  (1000)        0 2024-02-24 14:05:59.638455 gwtools-1.1.8/
--rw-r--r--   0 balzani57  (1000) balzani57  (1000)     1155 2018-08-24 21:42:03.000000 gwtools-1.1.8/LICENSE
--rw-r--r--   0 balzani57  (1000) balzani57  (1000)      166 2018-08-24 21:42:03.000000 gwtools-1.1.8/MANIFEST.in
--rw-rw-r--   0 balzani57  (1000) balzani57  (1000)     1052 2024-02-24 14:05:59.638455 gwtools-1.1.8/PKG-INFO
--rw-rw-r--   0 balzani57  (1000) balzani57  (1000)      441 2023-11-17 16:39:55.000000 gwtools-1.1.8/README.md
-drwxrwxr-x   0 balzani57  (1000) balzani57  (1000)        0 2024-02-24 14:05:59.634455 gwtools-1.1.8/docs/
--rw-r--r--   0 balzani57  (1000) balzani57  (1000)     6666 2017-07-03 01:39:34.000000 gwtools-1.1.8/docs/mismatch.tex
-drwxrwxr-x   0 balzani57  (1000) balzani57  (1000)        0 2024-02-24 14:05:59.638455 gwtools-1.1.8/gwtools/
--rw-rw-r--   0 balzani57  (1000) balzani57  (1000)       85 2022-09-30 22:46:55.000000 gwtools-1.1.8/gwtools/__init__.py
--rw-r--r--   0 balzani57  (1000) balzani57  (1000)     2143 2020-02-11 05:01:09.000000 gwtools-1.1.8/gwtools/const.py
--rw-r--r--   0 balzani57  (1000) balzani57  (1000)    58678 2024-02-24 13:58:23.000000 gwtools-1.1.8/gwtools/gwtools.py
--rw-r--r--   0 balzani57  (1000) balzani57  (1000)    12361 2019-11-17 17:26:04.000000 gwtools-1.1.8/gwtools/gwutils.py
--rw-r--r--   0 balzani57  (1000) balzani57  (1000)     1636 2017-07-31 19:01:07.000000 gwtools-1.1.8/gwtools/harmonics.py
--rw-r--r--   0 balzani57  (1000) balzani57  (1000)    12538 2019-10-21 16:14:54.000000 gwtools-1.1.8/gwtools/mismatch.py
--rw-r--r--   0 balzani57  (1000) balzani57  (1000)    19691 2017-07-31 19:01:07.000000 gwtools-1.1.8/gwtools/rotations.py
-drwxrwxr-x   0 balzani57  (1000) balzani57  (1000)        0 2024-02-24 14:05:59.638455 gwtools-1.1.8/gwtools.egg-info/
--rw-r--r--   0 balzani57  (1000) balzani57  (1000)     1052 2024-02-24 14:05:59.000000 gwtools-1.1.8/gwtools.egg-info/PKG-INFO
--rw-r--r--   0 balzani57  (1000) balzani57  (1000)      317 2024-02-24 14:05:59.000000 gwtools-1.1.8/gwtools.egg-info/SOURCES.txt
--rw-r--r--   0 balzani57  (1000) balzani57  (1000)        1 2024-02-24 14:05:59.000000 gwtools-1.1.8/gwtools.egg-info/dependency_links.txt
--rw-r--r--   0 balzani57  (1000) balzani57  (1000)        8 2024-02-24 14:05:59.000000 gwtools-1.1.8/gwtools.egg-info/top_level.txt
--rw-rw-r--   0 balzani57  (1000) balzani57  (1000)       38 2024-02-24 14:05:59.638455 gwtools-1.1.8/setup.cfg
--rw-rw-r--   0 balzani57  (1000) balzani57  (1000)     1466 2024-02-24 14:03:02.000000 gwtools-1.1.8/setup.py
+drwxrwxr-x   0 balzani57  (1000) balzani57  (1000)        0 2024-04-06 14:33:28.230347 gwtools-1.1.9/
+-rw-r--r--   0 balzani57  (1000) balzani57  (1000)     1155 2018-08-24 21:42:03.000000 gwtools-1.1.9/LICENSE
+-rw-r--r--   0 balzani57  (1000) balzani57  (1000)      166 2018-08-24 21:42:03.000000 gwtools-1.1.9/MANIFEST.in
+-rw-rw-r--   0 balzani57  (1000) balzani57  (1000)     1052 2024-04-06 14:33:28.230347 gwtools-1.1.9/PKG-INFO
+-rw-rw-r--   0 balzani57  (1000) balzani57  (1000)      441 2023-11-17 16:39:55.000000 gwtools-1.1.9/README.md
+drwxrwxr-x   0 balzani57  (1000) balzani57  (1000)        0 2024-04-06 14:33:28.226347 gwtools-1.1.9/docs/
+-rw-r--r--   0 balzani57  (1000) balzani57  (1000)     6666 2017-07-03 01:39:34.000000 gwtools-1.1.9/docs/mismatch.tex
+drwxrwxr-x   0 balzani57  (1000) balzani57  (1000)        0 2024-04-06 14:33:28.230347 gwtools-1.1.9/gwtools/
+-rw-rw-r--   0 balzani57  (1000) balzani57  (1000)       85 2022-09-30 22:46:55.000000 gwtools-1.1.9/gwtools/__init__.py
+-rw-r--r--   0 balzani57  (1000) balzani57  (1000)     2143 2020-02-11 05:01:09.000000 gwtools-1.1.9/gwtools/const.py
+-rw-r--r--   0 balzani57  (1000) balzani57  (1000)    58642 2024-04-06 13:44:54.000000 gwtools-1.1.9/gwtools/gwtools.py
+-rw-r--r--   0 balzani57  (1000) balzani57  (1000)    12924 2024-02-27 21:45:52.000000 gwtools-1.1.9/gwtools/gwutils.py
+-rw-r--r--   0 balzani57  (1000) balzani57  (1000)     1636 2017-07-31 19:01:07.000000 gwtools-1.1.9/gwtools/harmonics.py
+-rw-r--r--   0 balzani57  (1000) balzani57  (1000)    12538 2019-10-21 16:14:54.000000 gwtools-1.1.9/gwtools/mismatch.py
+-rw-r--r--   0 balzani57  (1000) balzani57  (1000)    19691 2017-07-31 19:01:07.000000 gwtools-1.1.9/gwtools/rotations.py
+drwxrwxr-x   0 balzani57  (1000) balzani57  (1000)        0 2024-04-06 14:33:28.230347 gwtools-1.1.9/gwtools.egg-info/
+-rw-r--r--   0 balzani57  (1000) balzani57  (1000)     1052 2024-04-06 14:33:28.000000 gwtools-1.1.9/gwtools.egg-info/PKG-INFO
+-rw-r--r--   0 balzani57  (1000) balzani57  (1000)      317 2024-04-06 14:33:28.000000 gwtools-1.1.9/gwtools.egg-info/SOURCES.txt
+-rw-r--r--   0 balzani57  (1000) balzani57  (1000)        1 2024-04-06 14:33:28.000000 gwtools-1.1.9/gwtools.egg-info/dependency_links.txt
+-rw-r--r--   0 balzani57  (1000) balzani57  (1000)        8 2024-04-06 14:33:28.000000 gwtools-1.1.9/gwtools.egg-info/top_level.txt
+-rw-rw-r--   0 balzani57  (1000) balzani57  (1000)       38 2024-04-06 14:33:28.230347 gwtools-1.1.9/setup.cfg
+-rw-rw-r--   0 balzani57  (1000) balzani57  (1000)     1466 2024-04-06 14:31:52.000000 gwtools-1.1.9/setup.py
```

### Comparing `gwtools-1.1.8/LICENSE` & `gwtools-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gwtools-1.1.8/PKG-INFO` & `gwtools-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwtools
-Version: 1.1.8
+Version: 1.1.9
 Summary: A collection of gravitational wave tools
 Author: Jonathan Blackman, Scott Field, Chad Galley
 Author-email: sfield@umassd.edu
 License: MIT
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `gwtools-1.1.8/docs/mismatch.tex` & `gwtools-1.1.9/docs/mismatch.tex`

 * *Files identical despite different names*

### Comparing `gwtools-1.1.8/gwtools/const.py` & `gwtools-1.1.9/gwtools/const.py`

 * *Files identical despite different names*

### Comparing `gwtools-1.1.8/gwtools/gwtools.py` & `gwtools-1.1.9/gwtools/gwtools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1144,53 +1144,51 @@
     if dtype == 'complex':
       return splev(t, interp_real) + 1j*splev(t, interp_imag)
     elif dtype == 'double':
       return splev(t, interp)
 
   return f_sp
 
-
-  # add to gwtools
-def orbital_phase_from_h2m(h2m,m):
+def orbital_phase_from_hlm(hlm,m):
     """ Compute orbital phase from GW mode h_{ell,m}.
     
     Input
     =====
     h2m: numpy array
     m:   spherical harmonic index m for mode h_{ell,m}
 
     orbital_phase = - \frac{1}{m} arg(h_{ell,m})"""
     
-    return -gwtools.phase(h2m) / m
+    return -phase(hlm) / m
 
-def orbital_frequency_from_h2m(h2m,t,m,deg=3,spline_smooth=0.001):
+def orbital_frequency_from_hlm(hlm,t,m,deg=3,spline_smooth=0.001):
     """ Compute orbital frequency from GW mode h_{ell,m}.
     
     computed as a time derivative of orbital_phase. The derivative
     is computed by (i) building a smoothing spline of the phase data
     (ii) taking a derivative of the spline.
     
     spline degree(=3) and smoothing factor(=0.001) have been set to reasonable
     defaults for SXS waveforms. noisier waveforms should use a larger smoothing 
     factor and/or lower degre.
     """
     
     from scipy.interpolate import splev
-    orbital_phase = orbital_phase_from_h2m(h2m,m)
-    tmp = gwtools.interpolant_h(t, orbital_phase, deg=deg, s=spline_smooth)
+    orbital_phase = orbital_phase_from_hlm(hlm,m)
+    tmp = interpolant_h(t, orbital_phase, deg=deg, s=spline_smooth)
     orbital_freq = splev(t,tmp,der=1)
     return orbital_freq
 
-def orbital_phase_frequency_from_h2m(h2m,t,m,deg=3,spline_smooth=0.001):
+def orbital_phase_frequency_from_hlm(hlm,t,m,deg=3,spline_smooth=0.001):
     """ Compute orbital phase and frequency from  GW mode h_{\ell,m)}.
     
     The phase is computed from a smoothing spline. Please see the documentation 
-    of orbital_phase_from_h2m and orbital_frequency_from_h2m for more information.
+    of orbital_phase_from_hlm and orbital_frequency_from_hlm for more information.
     """
-    return orbital_phase_from_h2m(h2m,m), orbital_frequency_from_h2m(h2m,t,m,deg,spline_smooth)
+    return orbital_phase_from_hlm(hlm,m), orbital_frequency_from_hlm(hlm,t,m,deg,spline_smooth)
 
 
 
 def energy_flux_from_modes(h, time, q, M=1., tend=100.):
   """ Computes the radiated energy and flux from each mode (E_modes), and 
     total energy (E_tot) as described in Eq.(2) of arXiv:1802.04276v2 and E0_over_M (Eq. 3).
```

### Comparing `gwtools-1.1.8/gwtools/gwutils.py` & `gwtools-1.1.9/gwtools/gwutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,33 @@
            If None, only pad up to a power of 2.
     padLocation  --- 'start', 'center', 'end', 'random', and
                      determines where the zeros are placed
 
     OUTPUT
     =====
     frequencies: An array of monotonically increasing frequencies
-    hf: The frequency domain waveform"""
+    hf: The frequency domain waveform
+
+
+
+    EXAMPLE
+    =======
+
+    The following code will show peak at 10 
+
+    omega = 10
+    times = np.linspace(-10,10,1000)
+    y = np.cos(omega*times) + 1.0j*np.sin(omega*times)
+    y_tapered = gwutils.windowWaveform(times, y, times[0], times[0] + 100, times[-1] -100, times[-1], windowType='planck')
+
+    dt = times[1] - times[0]
+    freqs_ringdown, hFreq_tapered_y = gwutils.freqDomainWaveform(y_tapered, dt, dfMax=None, padLocation='end')
+    freqs_ringdown = freqs_ringdown*2*np.pi
+
+    plt.semilogy(freqs_ringdown*2*np.pi, np.abs(hFreq_tapered_y),'k--') """
 
     # Find a power of 2 that achieves dfMax
     minLength = len(h)
     if dfMax is not None:
         minLength = max(len(h), 1./(dt*dfMax))
     pow2 = 0
     while 2**pow2 < minLength:
```

### Comparing `gwtools-1.1.8/gwtools/harmonics.py` & `gwtools-1.1.9/gwtools/harmonics.py`

 * *Files identical despite different names*

### Comparing `gwtools-1.1.8/gwtools/mismatch.py` & `gwtools-1.1.9/gwtools/mismatch.py`

 * *Files identical despite different names*

### Comparing `gwtools-1.1.8/gwtools/rotations.py` & `gwtools-1.1.9/gwtools/rotations.py`

 * *Files identical despite different names*

### Comparing `gwtools-1.1.8/gwtools.egg-info/PKG-INFO` & `gwtools-1.1.9/gwtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwtools
-Version: 1.1.8
+Version: 1.1.9
 Summary: A collection of gravitational wave tools
 Author: Jonathan Blackman, Scott Field, Chad Galley
 Author-email: sfield@umassd.edu
 License: MIT
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `gwtools-1.1.8/setup.py` & `gwtools-1.1.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     import pypandoc
     long_description = pypandoc.convert('README.md', 'rst')
 except ImportError:
     long_description = open('README.md').read()
 
 
 setup(name='gwtools',
-      version='1.1.8',
+      version='1.1.9',
       author='Jonathan Blackman, Scott Field, Chad Galley',
       author_email='sfield@umassd.edu',
       packages=['gwtools'],
       license='MIT',
       include_package_data=True,
       contributors=[
       # Alphabetical by last name.
```

