# Comparing `tmp/AstroToolkit-1.3.5.tar.gz` & `tmp/AstroToolkit-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AstroToolkit-1.3.5.tar", last modified: Tue Apr  2 12:45:58 2024, max compression
+gzip compressed data, was "AstroToolkit-1.4.0.tar", last modified: Sat Apr  6 13:59:17 2024, max compression
```

## Comparing `AstroToolkit-1.3.5.tar` & `AstroToolkit-1.4.0.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 12:45:58.447382 AstroToolkit-1.3.5/
--rw-rw-rw-   0        0        0        0 2024-01-11 16:40:26.000000 AstroToolkit-1.3.5/LICENSE
--rw-rw-rw-   0        0        0      297 2024-02-04 17:52:40.000000 AstroToolkit-1.3.5/MANIFEST.in
--rw-rw-rw-   0        0        0    39258 2024-04-02 12:45:58.446382 AstroToolkit-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0    38214 2024-03-24 21:49:15.000000 AstroToolkit-1.3.5/README.md
--rw-rw-rw-   0        0        0     1058 2024-04-02 12:45:39.000000 AstroToolkit-1.3.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-02 12:45:58.447382 AstroToolkit-1.3.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-02 12:45:58.067297 AstroToolkit-1.3.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-02 12:45:58.076299 AstroToolkit-1.3.5/src/AstroToolkit/
-drwxrwxrwx   0        0        0        0 2024-04-02 12:45:58.222269 AstroToolkit-1.3.5/src/AstroToolkit/Data/
--rw-rw-rw-   0        0        0    14952 2024-03-28 11:05:05.000000 AstroToolkit-1.3.5/src/AstroToolkit/Data/data.py
--rw-rw-rw-   0        0        0     6292 2024-03-24 13:18:55.000000 AstroToolkit-1.3.5/src/AstroToolkit/Data/imaging.py
--rw-rw-rw-   0        0        0     3489 2024-03-15 17:17:57.000000 AstroToolkit-1.3.5/src/AstroToolkit/Data/lightcurve_sigma_clip.py
--rw-rw-rw-   0        0        0    23058 2024-03-30 19:21:54.000000 AstroToolkit-1.3.5/src/AstroToolkit/Data/lightcurves.py
--rw-rw-rw-   0        0        0    10503 2024-03-24 13:13:06.000000 AstroToolkit-1.3.5/src/AstroToolkit/Data/overlays.py
--rw-rw-rw-   0        0        0     2763 2024-01-17 19:10:24.000000 AstroToolkit-1.3.5/src/AstroToolkit/Data/photometry.py
--rw-rw-rw-   0        0        0     2534 2024-03-24 15:05:20.000000 AstroToolkit-1.3.5/src/AstroToolkit/Data/reddening.py
--rw-rw-rw-   0        0        0     4300 2024-01-18 17:10:19.000000 AstroToolkit-1.3.5/src/AstroToolkit/Data/sed.py
--rw-rw-rw-   0        0        0     1974 2024-03-29 17:46:17.000000 AstroToolkit-1.3.5/src/AstroToolkit/Data/spectra.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:45:58.249274 AstroToolkit-1.3.5/src/AstroToolkit/Datapages/
--rw-rw-rw-   0        0        0     2747 2024-01-17 22:56:29.000000 AstroToolkit-1.3.5/src/AstroToolkit/Datapages/buttons.py
--rw-rw-rw-   0        0        0     3785 2024-03-24 00:14:23.000000 AstroToolkit-1.3.5/src/AstroToolkit/Datapages/grid.py
--rw-rw-rw-   0        0        0     8232 2024-01-17 22:58:42.000000 AstroToolkit-1.3.5/src/AstroToolkit/Datapages/metadata.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:45:58.257276 AstroToolkit-1.3.5/src/AstroToolkit/Examples/
--rw-rw-rw-   0        0        0     3135 2024-03-24 00:18:21.000000 AstroToolkit-1.3.5/src/AstroToolkit/Examples/datapage_creation.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:45:58.308053 AstroToolkit-1.3.5/src/AstroToolkit/Misc/
--rw-rw-rw-   0        0        0     2388 2024-02-07 17:32:05.000000 AstroToolkit-1.3.5/src/AstroToolkit/Misc/ProperMotionCorrection.py
--rw-rw-rw-   0        0        0     2540 2024-02-21 13:02:49.000000 AstroToolkit-1.3.5/src/AstroToolkit/Misc/coord_conversion.py
--rw-rw-rw-   0        0        0    18188 2024-03-28 16:04:31.000000 AstroToolkit-1.3.5/src/AstroToolkit/Misc/file_handling.py
--rw-rw-rw-   0        0        0     4207 2024-03-24 13:13:35.000000 AstroToolkit-1.3.5/src/AstroToolkit/Misc/file_naming.py
--rw-rw-rw-   0        0        0     2764 2024-03-09 16:01:36.000000 AstroToolkit-1.3.5/src/AstroToolkit/Misc/input_validation.py
--rw-rw-rw-   0        0        0     3244 2024-03-15 18:39:31.000000 AstroToolkit-1.3.5/src/AstroToolkit/Misc/read_fits.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:45:58.373365 AstroToolkit-1.3.5/src/AstroToolkit/Plotting/
--rw-rw-rw-   0        0        0     4697 2024-03-31 16:17:17.000000 AstroToolkit-1.3.5/src/AstroToolkit/Plotting/HRD.py
--rw-rw-rw-   0        0        0  1224000 2024-01-11 16:40:26.000000 AstroToolkit-1.3.5/src/AstroToolkit/Plotting/backdrop_hrd_allmags.fits
--rw-rw-rw-   0        0        0     4576 2024-03-24 13:19:53.000000 AstroToolkit-1.3.5/src/AstroToolkit/Plotting/imaging.py
--rw-rw-rw-   0        0        0     5609 2024-03-23 23:37:51.000000 AstroToolkit-1.3.5/src/AstroToolkit/Plotting/lightcurves.py
--rw-rw-rw-   0        0        0     2647 2024-03-23 23:44:35.000000 AstroToolkit-1.3.5/src/AstroToolkit/Plotting/powspec.py
--rw-rw-rw-   0        0        0     2629 2024-02-27 18:54:15.000000 AstroToolkit-1.3.5/src/AstroToolkit/Plotting/sed.py
--rw-rw-rw-   0        0        0     3676 2024-03-23 22:29:45.000000 AstroToolkit-1.3.5/src/AstroToolkit/Plotting/spectra.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:45:58.374365 AstroToolkit-1.3.5/src/AstroToolkit/Settings/
--rw-rw-rw-   0        0        0        0 2024-02-04 19:17:29.000000 AstroToolkit-1.3.5/src/AstroToolkit/Settings/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:45:58.443381 AstroToolkit-1.3.5/src/AstroToolkit/Timeseries/
--rw-rw-rw-   0        0        0     3780 2024-01-11 16:40:26.000000 AstroToolkit-1.3.5/src/AstroToolkit/Timeseries/README - Windows.txt
--rw-rw-rw-   0        0        0     3269 2024-01-11 16:40:26.000000 AstroToolkit-1.3.5/src/AstroToolkit/Timeseries/README.txt
--rw-rw-rw-   0        0        0        0 2024-01-11 16:40:26.000000 AstroToolkit-1.3.5/src/AstroToolkit/Timeseries/__init__.py
--rw-rw-rw-   0        0        0   167936 2024-01-14 17:57:05.000000 AstroToolkit-1.3.5/src/AstroToolkit/Timeseries/aov.cp38-win_amd64.pyd
--rw-rw-rw-   0        0        0    33000 2024-01-11 16:40:26.000000 AstroToolkit-1.3.5/src/AstroToolkit/Timeseries/aov.f90
--rw-rw-rw-   0        0        0      554 2024-01-11 16:40:26.000000 AstroToolkit-1.3.5/src/AstroToolkit/Timeseries/aovconst.f90
--rw-rw-rw-   0        0        0    36089 2024-01-11 16:40:26.000000 AstroToolkit-1.3.5/src/AstroToolkit/Timeseries/aovsub.f90
--rw-rw-rw-   0        0        0      577 2024-01-11 16:40:26.000000 AstroToolkit-1.3.5/src/AstroToolkit/Timeseries/build.sh
--rwxrwxrwx   0        0        0      635 2024-01-11 16:40:26.000000 AstroToolkit-1.3.5/src/AstroToolkit/Timeseries/buildwin.bat
--rw-rw-rw-   0        0        0   256433 2024-01-11 16:40:26.000000 AstroToolkit-1.3.5/src/AstroToolkit/Timeseries/pyaov.pdf
--rw-rw-rw-   0        0        0    24550 2024-01-11 16:40:26.000000 AstroToolkit-1.3.5/src/AstroToolkit/Timeseries/pyaov.py
--rw-rw-rw-   0        0        0    31600 2024-04-02 12:42:59.000000 AstroToolkit-1.3.5/src/AstroToolkit/Timeseries/ztfanalysis.py
--rw-rw-rw-   0        0        0    33123 2024-03-31 16:18:16.000000 AstroToolkit-1.3.5/src/AstroToolkit/Tools.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:45:58.444381 AstroToolkit-1.3.5/src/AstroToolkit.egg-info/
--rw-rw-rw-   0        0        0    39258 2024-04-02 12:45:58.000000 AstroToolkit-1.3.5/src/AstroToolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1784 2024-04-02 12:45:58.000000 AstroToolkit-1.3.5/src/AstroToolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 12:45:58.000000 AstroToolkit-1.3.5/src/AstroToolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      265 2024-04-02 12:45:58.000000 AstroToolkit-1.3.5/src/AstroToolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-02 12:45:58.000000 AstroToolkit-1.3.5/src/AstroToolkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 13:59:17.929451 AstroToolkit-1.4.0/
+-rw-rw-rw-   0        0        0        0 2024-01-11 16:40:26.000000 AstroToolkit-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0      297 2024-02-04 17:52:40.000000 AstroToolkit-1.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    40407 2024-04-06 13:59:17.928451 AstroToolkit-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0    39363 2024-04-06 00:56:04.000000 AstroToolkit-1.4.0/README.md
+-rw-rw-rw-   0        0        0     1058 2024-04-06 13:58:43.000000 AstroToolkit-1.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-06 13:59:17.930451 AstroToolkit-1.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-06 13:59:17.738862 AstroToolkit-1.4.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-06 13:59:17.755423 AstroToolkit-1.4.0/src/AstroToolkit/
+drwxrwxrwx   0        0        0        0 2024-04-06 13:59:17.826170 AstroToolkit-1.4.0/src/AstroToolkit/Data/
+-rw-rw-rw-   0        0        0    14952 2024-03-28 11:05:05.000000 AstroToolkit-1.4.0/src/AstroToolkit/Data/data.py
+-rw-rw-rw-   0        0        0     6296 2024-04-05 17:18:50.000000 AstroToolkit-1.4.0/src/AstroToolkit/Data/imaging.py
+-rw-rw-rw-   0        0        0     3489 2024-03-15 17:17:57.000000 AstroToolkit-1.4.0/src/AstroToolkit/Data/lightcurve_sigma_clip.py
+-rw-rw-rw-   0        0        0    23062 2024-04-05 17:22:00.000000 AstroToolkit-1.4.0/src/AstroToolkit/Data/lightcurves.py
+-rw-rw-rw-   0        0        0    10534 2024-04-05 17:25:55.000000 AstroToolkit-1.4.0/src/AstroToolkit/Data/overlays.py
+-rw-rw-rw-   0        0        0     2763 2024-01-17 19:10:24.000000 AstroToolkit-1.4.0/src/AstroToolkit/Data/photometry.py
+-rw-rw-rw-   0        0        0     2618 2024-04-05 17:44:53.000000 AstroToolkit-1.4.0/src/AstroToolkit/Data/reddening.py
+-rw-rw-rw-   0        0        0     4300 2024-04-05 17:17:38.000000 AstroToolkit-1.4.0/src/AstroToolkit/Data/sed.py
+-rw-rw-rw-   0        0        0     1978 2024-04-05 17:27:41.000000 AstroToolkit-1.4.0/src/AstroToolkit/Data/spectra.py
+drwxrwxrwx   0        0        0        0 2024-04-06 13:59:17.830217 AstroToolkit-1.4.0/src/AstroToolkit/Datapages/
+-rw-rw-rw-   0        0        0     2751 2024-04-05 17:28:09.000000 AstroToolkit-1.4.0/src/AstroToolkit/Datapages/buttons.py
+-rw-rw-rw-   0        0        0     3785 2024-03-24 00:14:23.000000 AstroToolkit-1.4.0/src/AstroToolkit/Datapages/grid.py
+-rw-rw-rw-   0        0        0     8244 2024-04-05 17:28:31.000000 AstroToolkit-1.4.0/src/AstroToolkit/Datapages/metadata.py
+drwxrwxrwx   0        0        0        0 2024-04-06 13:59:17.838219 AstroToolkit-1.4.0/src/AstroToolkit/Examples/
+-rw-rw-rw-   0        0        0     3072 2024-04-06 09:17:47.000000 AstroToolkit-1.4.0/src/AstroToolkit/Examples/datapage_creation.py
+drwxrwxrwx   0        0        0        0 2024-04-06 13:59:17.848981 AstroToolkit-1.4.0/src/AstroToolkit/Misc/
+-rw-rw-rw-   0        0        0     2388 2024-02-07 17:32:05.000000 AstroToolkit-1.4.0/src/AstroToolkit/Misc/ProperMotionCorrection.py
+-rw-rw-rw-   0        0        0     2540 2024-02-21 13:02:49.000000 AstroToolkit-1.4.0/src/AstroToolkit/Misc/coord_conversion.py
+-rw-rw-rw-   0        0        0     1625 2024-04-05 17:29:14.000000 AstroToolkit-1.4.0/src/AstroToolkit/Misc/database_queries.py
+-rw-rw-rw-   0        0        0    18188 2024-03-28 16:04:31.000000 AstroToolkit-1.4.0/src/AstroToolkit/Misc/file_handling.py
+-rw-rw-rw-   0        0        0     4308 2024-04-05 22:43:02.000000 AstroToolkit-1.4.0/src/AstroToolkit/Misc/file_naming.py
+-rw-rw-rw-   0        0        0     2937 2024-04-05 17:40:17.000000 AstroToolkit-1.4.0/src/AstroToolkit/Misc/input_validation.py
+-rw-rw-rw-   0        0        0     3244 2024-03-15 18:39:31.000000 AstroToolkit-1.4.0/src/AstroToolkit/Misc/read_fits.py
+drwxrwxrwx   0        0        0        0 2024-04-06 13:59:17.858984 AstroToolkit-1.4.0/src/AstroToolkit/Plotting/
+-rw-rw-rw-   0        0        0     4533 2024-04-05 22:49:09.000000 AstroToolkit-1.4.0/src/AstroToolkit/Plotting/HRD.py
+-rw-rw-rw-   0        0        0  1224000 2024-01-11 16:40:26.000000 AstroToolkit-1.4.0/src/AstroToolkit/Plotting/backdrop_hrd_allmags.fits
+-rw-rw-rw-   0        0        0     4576 2024-03-24 13:19:53.000000 AstroToolkit-1.4.0/src/AstroToolkit/Plotting/imaging.py
+-rw-rw-rw-   0        0        0     5609 2024-03-23 23:37:51.000000 AstroToolkit-1.4.0/src/AstroToolkit/Plotting/lightcurves.py
+-rw-rw-rw-   0        0        0     2647 2024-03-23 23:44:35.000000 AstroToolkit-1.4.0/src/AstroToolkit/Plotting/powspec.py
+-rw-rw-rw-   0        0        0     2629 2024-02-27 18:54:15.000000 AstroToolkit-1.4.0/src/AstroToolkit/Plotting/sed.py
+-rw-rw-rw-   0        0        0     3676 2024-03-23 22:29:45.000000 AstroToolkit-1.4.0/src/AstroToolkit/Plotting/spectra.py
+drwxrwxrwx   0        0        0        0 2024-04-06 13:59:17.860984 AstroToolkit-1.4.0/src/AstroToolkit/Settings/
+-rw-rw-rw-   0        0        0        0 2024-02-04 19:17:29.000000 AstroToolkit-1.4.0/src/AstroToolkit/Settings/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 13:59:17.926451 AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/
+-rw-rw-rw-   0        0        0     3780 2024-01-11 16:40:26.000000 AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/README - Windows.txt
+-rw-rw-rw-   0        0        0     3269 2024-01-11 16:40:26.000000 AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/README.txt
+-rw-rw-rw-   0        0        0        0 2024-01-11 16:40:26.000000 AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/__init__.py
+-rw-rw-rw-   0        0        0   167936 2024-01-14 17:57:05.000000 AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/aov.cp38-win_amd64.pyd
+-rw-rw-rw-   0        0        0    33000 2024-01-11 16:40:26.000000 AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/aov.f90
+-rw-rw-rw-   0        0        0      554 2024-01-11 16:40:26.000000 AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/aovconst.f90
+-rw-rw-rw-   0        0        0    36089 2024-01-11 16:40:26.000000 AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/aovsub.f90
+-rw-rw-rw-   0        0        0      577 2024-01-11 16:40:26.000000 AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/build.sh
+-rwxrwxrwx   0        0        0      635 2024-01-11 16:40:26.000000 AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/buildwin.bat
+-rw-rw-rw-   0        0        0   256433 2024-01-11 16:40:26.000000 AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/pyaov.pdf
+-rw-rw-rw-   0        0        0    24550 2024-01-11 16:40:26.000000 AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/pyaov.py
+-rw-rw-rw-   0        0        0    31600 2024-04-02 12:42:59.000000 AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/ztfanalysis.py
+-rw-rw-rw-   0        0        0    33302 2024-04-06 09:19:55.000000 AstroToolkit-1.4.0/src/AstroToolkit/Tools.py
+drwxrwxrwx   0        0        0        0 2024-04-06 13:59:17.927451 AstroToolkit-1.4.0/src/AstroToolkit.egg-info/
+-rw-rw-rw-   0        0        0    40407 2024-04-06 13:59:17.000000 AstroToolkit-1.4.0/src/AstroToolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1826 2024-04-06 13:59:17.000000 AstroToolkit-1.4.0/src/AstroToolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 13:59:17.000000 AstroToolkit-1.4.0/src/AstroToolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      265 2024-04-06 13:59:17.000000 AstroToolkit-1.4.0/src/AstroToolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-06 13:59:17.000000 AstroToolkit-1.4.0/src/AstroToolkit.egg-info/top_level.txt
```

### Comparing `AstroToolkit-1.3.5/PKG-INFO` & `AstroToolkit-1.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,89 +1,26 @@
-Metadata-Version: 2.1
-Name: AstroToolkit
-Version: 1.3.5
-Summary: A package for the gathering and plotting of astronomical data.
-Author-email: Ethan Moorfield <ethan.moorfield@hotmail.co.uk>
-Project-URL: Homepage, https://github.com/WD-planets/AstroToolkit
-Project-URL: Issues, https://github.com/WD-planets/AstroToolkit/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: astropy==5.2.2
-Requires-Dist: astroquery==0.4.7
-Requires-Dist: bokeh==3.1.1
-Requires-Dist: cmasher==1.6.3
-Requires-Dist: importlib_resources==6.4.0
-Requires-Dist: matplotlib==3.7.5
-Requires-Dist: numba==0.58.1
-Requires-Dist: numpy==1.24.4
-Requires-Dist: pandas==2.0.3
-Requires-Dist: Pillow==10.2.0
-Requires-Dist: PyQt5==5.15.10
-Requires-Dist: PyQt5_sip==12.13.0
-Requires-Dist: Requests==2.31.0
-Requires-Dist: scikit_learn==1.3.2
-Requires-Dist: scipy==1.10.1
-Requires-Dist: selenium==4.17.2
-
 # AstroToolkit
 
-AstroToolkit (ATK) is a set of useful tools for fetching, plotting, and analysing astronomical data.
+AstroToolkit (ATK) is a set of tools for fetching, plotting, and analysing astronomical data.
 
 ## Table of Contents
 
 1. [Installation](#installation)
 2. [Introduction](#introduction)
 3. [Configuration](#configuration)
 4. [Tools](#tools)
+5. [Examples](#examples)
 
 ### ATK Tools
 
-- 1 [Raw Data Tools](#1-raw-data-tools)
-	- 1.1 [dataquery](#11-dataquery)
-	- 1.2 [photquery](#12-photquery)
-	- 1.3 [bulkphotquery](#13-bulkphotquery)
-	- 1.4 [getreddening](#14-getreddening)
-- 2 [Imaging Tools](#2-imaging-tools)
-	- 2.1 [imagequery](#21-imagequery)
-	- 2.2 [plotimage](#22-plotimage)
-- 3 [HRD Tools](#3-hrd-tools)
-	- 3.1 [plothrd](#31-plothrd)
-- 4 [Lightcurve Tools](#4-lightcurve-tools)
-	- 4.1 [lightcurvequery](#41-lightcurvequery)
-	- 4.2 [plotlightcurve](#42-plotlightcurve)
-- 5 [SED Tools](#5-sed-tools)
-	- 5.1 [sedquery](#51-sedquery)
-	- 5.2 [plotsed](#52-plotsed)
-- 6 [Spectrum Tools](#6-spectrum-tools)
-	- 6.1 [spectrumquery](#61-spectrumquery)
-	- 6.2 [plotspectrum](#62-plotspectrum)
-- 7 [Timeseries Tools](#7-timeseries-tools)
-	- 7.1 [plotpowspec](#71-plotpowspec)
-	- 7.2 [tsanalysis](#72-tsanalysis)
-- 8 [Datapage Tools](#8-datapage-tools)
-	- 8.1 [gridsetup](#81-gridsetup)
-	- 8.2 [getbuttons](#82-getbuttons)
-	- 8.3 [getmdtable](#83-getmdtable)
-- 9 [File Handling Tools](#9-file-handling-tools)
-	- 9.1 [savedata](#91-savedata)
-	- 9.2 [readdata](#92-readdata)
-	- 9.3 [export](#93-export)
-- 10 [Miscellaneous Tools](#10-miscellaneous-tools)
-	- 10.1 [showplot](#101-showplot)
-	- 10.2 [saveplot](#102-saveplot)
-	- 10.3 [correctpm](#103-correctpm)
-	- 10.4 [getdistance](#104-getdistance)
-	- 10.5 [convfromdeg](#105-convfromdeg)
-	- 10.6 [convtodeg](#106-convtodeg)
-	- 10.7 [getcolumn](#107-getcolumn)
-	- 10.8 [getsources](#108-getsources)
-	- 10.9 [getpositions](#109-getpositions)
+- 1 [Query](#1-query)
+- 2 [Plot](#2-plot)
+- 3 [Datapage Tools](#3-datapage-tools)
+- 4 [File Handling Tools](#4-file-handling-tools)
+- 5 [Other Tools](#5-other-tools)
 
 <br>
 
 ## Installation<a id="installation"></a>
 
 The package can be installed as with any other package, e.g. using pip:
 ```
@@ -138,33 +75,33 @@
 editconfig(options)
 ```
 
 where options is a dictionary containing key : value pairs to set in the config. The list of accepted keys and their default values are shown below:
 - enable_notifications = False
 	- If True, notifications denoting basic information as each ATK tool is executed will be shown in the terminal. Can be useful for tracking the flow of data.
 - dataquery_radius = 3
-	- This sets the default radius (in arcseconds) to use in the [dataquery](#11-dataquery) tool.
+	- This sets the default radius (in arcseconds) to use in [data queries](#11-data-query).
 - photquery_radius = 3
-	- This sets the default radius (in arcseconds) to use in the [photquery](#12-photquery) tool.
+	- This sets the default radius (in arcseconds) to use in [photometry queries](#12-photometry-query).
 - bulkphotquery_radius = 3
-	- This sets the default radius (in arcseconds) to use in the [bulkphotquery](#13-bulkphotquery) tool.
+	- This sets the default radius (in arcseconds) to use in [bulk photometry queries](#13-bulk-photometry-query).
 - imagequery_size = 30
-	- This sets the default radius (in arcseconds) to use in the [imagequery](#21-imagequery) tool.
+	- This sets the default radius (in arcseconds) to use in [image queries](#15-imaging-query).
 - imagequery_overlays = gaia
-	- This sets the default radius (in arcseconds) to use in the [imagequery](#21-imagequery) tool.
+	- This sets the default radius (in arcseconds) to use in [image queries](#15-imaging-query).
 - lightcurvequery_radius = 3
-	- This sets the default radius (in arcseconds) to use in the [lightcurvequery](#31-lightcurvequery) tool.
+	- This sets the default radius (in arcseconds) to use in [lightcurve queries](#16-lightcurve-query).
 - atlas_username = None
-	- This sets the default username to use for ATLAS lightcurve queries in the [lightcurvequery](#31-lightcurvequery) tool.
+	- This sets the default username to use in ATLAS [lightcurve queries](#16-lightcurve-query).
 - atlas_password = None
-	- This sets the default password to use for ATLAS lightcurve queries in the [lightcurvequery](#31-lightcurvequery) tool.
+	- This sets the default password to use in ATLAS [lightcurve queries](#16-lightcurve-query).
 - sed_radius = 3
-	- This sets the default radius to use in the [sedquery](#41-sedquery) tool.
+	- This sets the default radius to use in [SED queries](#17-sed-query).
 - spectrum_radius = 3
-	- This sets the default radius to use in the [spectrumquery](#51-spectrumquery) tool.
+	- This sets the default radius to use in [spectrum queries](#18-spectrum-query).
 - grid_size = 250
 	- This sets the default grid size to use in the [gridsetup](#71-gridsetup) tool.
 - button_simbad_radius = 3
 	- This sets the default radius to use for the SIMBAD button in the [getbuttons](#72-getbuttons) tool.
 - button_vizier_radius = 3
 	- This sets the default radius to use for the Vizier button in the [getbuttons](#72-getbuttons) tool.
 - plot_size = 400
@@ -198,168 +135,153 @@
 parameter = string, name of config parameter from above list
 ```
 
 **Returns**: value of this parameter in the config.
 
 <br><br>
 
-## Tools
+## Tools<a id="tools"></a>
 
 In this section, the available tools will be outlined. Note that if a parameter is listed as having a default parameter CONFIG, this means that this parameter is taken from the config as listed above. These parameters can still be passed to the tool, in which case the config value will be ignored.
 
 **Note:** most data returned from fetching/plotting tools takes the form of a dictionary. This dictionary contains the returned data, as well as basic information such as the pos/source used to acquire the data. This format is then used by other ATK functions (such as file showing/saving/reading).
 
 **Note:** All plots created by ATK can have their legends toggled by double clicking the plot, and individual data can be hidden by clicking them in the legend.
 
 <br>
 
 **In all data returned by querying tools, the value of the 'data' key will be set to None if no data was returned. Likewise, in all plotting tools, the value of the 'plot' key will be set to None.**
 
 <br>
 
-### 1. Raw Data Tools<a id="1-raw-data-tools"></a>
-### 1.1. dataquery<a id="11-dataquery"></a>
-
-Returns all available data for a given survey (e.g. magnitudes, positions, etc.).
-
-<br>
-
-**Supported surveys:** gaia, galex, rosat, panstarrs, skymapper, sdss, twomass, wise, erosita
+## 1. query<a id="1-query"></a>
 
-<br>
+Returns available data of a given type from a given survey.
 
 **Usage:**
 
 ```
-dataquery(survey,pos=None,source=None,radius=CONFIG)
+query(type,survey=None,pos=None,source=None,radius=CONFIG)
 ```
 
 where:
 
 ```
+type = str, type of data to return
+```
+```
 survey = str, name of a supported survey
 ```
 ```
 pos = list, [ra,dec]
 ```
 ```
 source = int/str, Gaia source_id
 ```
 ```
-radius = int/float, radius of query
+radius = int/float, radius of query of given type. If not given, will be taken from config value for given query type.
 ```
 
-**Returns:** dict
+<br>
 
-```
-{
-'survey' : str, survey of data
-'type' : 'data'
-'source' : int/str, source used to get data (None if a pos was used)
-'pos' : [ra,dec], pos used to get data (None if a source was used)
-'data' : dict, the returned data
-}
-```
+**Note:** If no data is returned, the 'data' key of the returned dictionary will be set to None.
 
 <br>
 
-**Example:**
+**Supported query types:** data, phot, bulkphot, image, lightcurve, sed, spectra, reddening
 
-To retrieve the parallax of a system through Gaia, and its WISE data:
+<br>
 
-```
-from AstroToolkit.Tools import dataquery
+Below is an outline of the usage and output of each query type. Note that additonal arguments not listed above may be used, see individual query types below for details.
 
-source = 6050296829033196032
+<br>
 
-parallax = dataquery(survey='gaia',source=source)['data']['parallax']
-wise_data = dataquery(survey='wise',source=source)['data']
-```
+**Shortcuts**:
 
-<br><br>
+[Data Queries](#11-data-query)
 
-### 1.2. photquery<a id="12-photquery"></a>
+[Photometry Queries](#12-photometry-query)
 
-Returns data from a given survey, with columns filtered to only include photometry and other basic information.
+[Bulk Photomety Queries](#13-bulk-photometry-query)
 
-<br>
+[Reddening Queries](#14-reddening-query)
+
+[Imaging Queries](#15-imaging-query)
+
+[Lightcurve Queries](#16-lightcurve-query)
+
+[SED Queries](#17-sed-query)
 
-**Supported surveys:** gaia,panstarrs,skymapper,galex,rosat,sdss,wise,twomass
+[Spectrum Queries](#18-spectrum-query)
+
+[HRD Queries](#19-hrd-query)
 
 <br>
 
-**Usage:**
+### 1.1 Data Query<a id="11-data-query"></a>
 
-```
-photquery(survey,pos=None,source=None,radius=CONFIG)
-```
+Type argument: 'data'
 
-where:
+Description: Returns all available raw data for a given survey
 
-```
-survey = str, name of a supported survey
-```
-```
-pos = list, [ra,dec]
-```
-```
-source = int/str, Gaia source_id
-```
-```
-radius = int/float, radius of query
-```
+Supported Arguments: survey, pos, source, radius (all defined [above](#1-query))
+
+Supported Surveys: gaia, galex, rosat, panstarrs, skymapper, sdss, twomass, wise, erosita
+
+<br>
 
 **Returns:** dict
 
 ```
 {
 'survey' : str, survey of data
 'type' : 'data'
 'source' : int/str, source used to get data (None if a pos was used)
 'pos' : [ra,dec], pos used to get data (None if a source was used)
 'data' : dict, the returned data
 }
 ```
 
-<br>
-
-**Example:**
+<br><br>
 
-To retrieve the 2MASS photometry for an object:
-```
-from AstroToolkit.Tools import photquery
+### 1.2 Photometry Query<a id="12-photometry-query"></a>
 
-data=photquery(survey='twomass',source=6050296829033196032)['data']
-```
+Type argument: 'phot'
 
-<br>
+Description: Returns all photometry available from a given survey, as well as some basic parameters such as coordinates.
 
-### 1.3. bulkphotquery<a id="13-bulkphotquery"></a>
+Supported Arguments: survey, pos, source, radius (all defined [above](#1-query))
 
-Returns available photometry from all surveys supported by [photquery](#12-photquery).
+Supported Surveys: gaia, panstarrs, skymapper, galex, rosat, sdss, wise, twomass
 
 <br>
 
-**Usage:**
+**Returns:** dict
 
 ```
-bulkphotquery(pos=None,source=None,radius=CONFIG)
+{
+'survey' : str, survey of data
+'type' : 'data'
+'source' : int/str, source used to get data (None if a pos was used)
+'pos' : [ra,dec], pos used to get data (None if a source was used)
+'data' : dict, the returned data
+}
 ```
 
-where:
+<br><br>
 
-```
-pos = list, [ra,dec]
-```
-```
-source = int/str, Gaia source_id
-```
-```
-radius = int/float, radius of query
-```
+### 1.3 Bulk Photometry Query<a id="13-bulk-photometry-query"></a>
+
+Type argument: 'bulkphot'
+
+Description: Returns all photometry available from all surveys supported by [photometry queries](#12-photometry-query)
+
+Supported Arguments: pos, source, radius (all defined [above](#1-query))
+
+<br>
 
 **Returns:** dict
 
 ```
 {
 'type' : 'bulkphot'
 'source' : int/str, source used to get data (None if a pos was used)
@@ -371,50 +293,25 @@
           etc. for each survey in surveys supported by photquery
          }
 }
 ```
 
 **Note:** The value of each survey will be set to None if no data was returned. E.g. if no galex data was returned, the value of the ['galex'] key would be None.
 
-<br>
-
-**Example:**
-
-To retrieve the gaia and galex data for an object:
-
-```
-from AstroToolkit.Tools import bulkphotquery
-
-bulk_phot=bulkphotquery(source=6050296829033196032)['data']
-
-gaia_data=bulk_phot['gaia']
-galex_data=bulk_phot['galex']
-```
-
-<br>
-
-### 1.4. getreddening<a id="14-getreddening"></a>
-
-Returns the reddening of a Gaia source.
+<br><br>
 
-Currently supported reddening surveys:
-- STILISM (https://stilism.obspm.fr/)
+### 1.4. Reddening Query<a id="14-reddening-query"></a>
 
-<br>
+Type argument: 'reddening'
 
-**Usage:**
+Description: Returns the reddening for a given Gaia source from a given survey
 
-```
-getreddening(source)
-```
+Supported Arguments: source (defined [above](#1-query))
 
-where:
-```
-source = int/str, Gaia source_id
-```
+Supported Surveys: stilism (https://stilism.obspm.fr/)
 
 <br>
 
 **Returns:** dict
 
 ```
 {
@@ -429,79 +326,56 @@
          'red_lower' : reddening lower limit
          }
 }
 ```
 
 <br><br>
 
-### 2. Imaging Tools<a id="2-imaging-tools"></a>
-
-These functions retrieve and plotimages from supported surveys.
+### 1.5 Imaging Query<a id="15-imaging-query"></a>
 
-**Note:** When using a 'pos' as input, some detections can be missing for high proper motion objects. When instead using a source as input, this is no longer a problem as the detection search radius is increased to account for this proper motion.
+Type argument: 'image'
 
-<br>
-
-### 2.1. imagequery<a id="21-imagequery"></a>
-
-Retrieves an image from a given survey. Overlays  can be used to overlay detections from different surveys. There are two types of overlay: detections and tracers. Detections are proper motion-corrected circles that scale with the magnitude of the detection, and show that there is data available for a given object in a given survey. 
+Description: Returns an image from a given survey. Overlays  can be used to overlay detections from different surveys. There are two types of overlay: detections and tracers. Detections are proper motion-corrected circles that scale with the magnitude of the detection, and show that there is data available for a given object in a given survey. 
 
 Tracers (which are detections created from lightcurve surveys) can be used both to show that lightcurve data is available, but also to trace an object through time.
 
 **Note:** tracing an object through time works best with ZTF and CRTS overlays, as these give data with the necessary coordinate precision. Other tracer overlays are unlikely to work for this, and will hence only be useful to see where lightcurve data is available.
 
 **Note:** In the case of ATLAS overlays, the radius used is very small due to the time taken to perform ATLAS queries. Only data close to the focus of the image (i.e. at the location of the target object) will be shown. 
 
 **Example:**
 
 ![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/tracer_example.png?raw=true)
 
-<br>
-
-Supported surveys:
-- panstarrs, supported bands = g, r, i, z, y
-- skymapper, supported bands = g, r, i, z, u, v
-- dss, supported bands = g
-
-**Note:** Can also use 'any' to perform an image query according to the hierarchy: panstarrs > skymapper > dss
-
-<br>
-
-Supported overlays: gaia, galex_nuv, galex_fuv, rosat,sdss, twomass, wise, ztf, erosita ,atlas, gaia_lc, asassn, crts
-
-**Note:** Can also use 'all', which will enable overlays for all supported surveys.
-
-<br>
-
-**Usage:**
-
-```
-imagequery(survey,pos=None,source=None,size=CONFIG,band='g',overlays=CONFIG)
-```
+Supported Arguments: survey, pos, source, size, band, overlays
 
 where:
 ```
-survey = str, name of a supported survey
-```
-```
-pos = list, [ra,dec]
-```
-```
-source = int/str, Gaia source_id
-```
-```
 size = int/float, size of image in arcsec
 ```
 ```
 band = str, string containing the required bands (e.g. for all panstarrs bands, use band='grizy')
 ```
 ```
 overlays = str, required detection overlays (e.g. for gaia and wise detections, use overlays='gaia,wise') 
 ```
 
+and all other arguments have been defined [above](#1-query).
+
+Supported overlays: gaia, galex_nuv, galex_fuv, rosat,sdss, twomass, wise, ztf, erosita ,atlas, gaia_lc, asassn, crts
+
+**Note:** Can also use 'all', which will enable overlays for all supported surveys.
+
+Supported Surveys:
+- panstarrs, supported bands = g, r, i, z, y
+- skymapper, supported bands = g, r, i, z, u, v
+- dss, supported bands = g
+
+<br>
+
 **Returns:** dict
 
 ```
 {
 'type' : 'image'
 'survey' : str, image survey
 'source' : int/str, source used to get image (None if a pos was used)
@@ -527,159 +401,47 @@
 'radius' : float, radius of detection
 'corrected' : bool, whether or not the detection has been corrected for proper motion
 'mag' : str, name of the magnitude (column heaader) from a given survey
 'marker' : 'circle' or 'cross', detection symbol to overlay. Circles are scaled with radius, crosses are not (e.g. for surveys without a magnitude to scale by)
 }
 ```
 
-<br>
-
-### 2.2. plotimage<a id="22-plotimage"></a>
-
-Plots images in format returned by [imagequery](#21-imagequery).
-
-<br>
-
-**Usage:**
-
-```
-plotimage(data)
-```
-
-where:
-```
-data = dict in format returned by imagequery
-```
-
-**Returns:** dict
-
-```
-{
-'type' : 'image'
-'survey' : str, survey of image
-'source' : int/str, source used to get image (None if a pos was used)
-'pos' : [ra,dec], pos used to get image (None if a source was used)
-'plot' : bokeh figure object, the actual plot
-'ATKfilename' : the default filename given by ATK
-}
-```
-
-**Note:** if a plot is not returned (e.g. if no data was supplied to the plotting tool), the 'plot' key will be set to None.
-
-<br>
-
-**Example:**
-
-To retrieve and plot an image:
-```
-from AstroToolkit.Tools import imagequery,plotimage,showplot
-
-image=imagequery(survey='any',source=6050296829033196032,overlays='gaia')
-plot=plotimage(image)
-showplot(plot)
-```
-
-![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/imaging_example.png?raw=true)
-
 <br><br>
 
-### 3. HRD Tools<a id="3-hrd-tools"></a>
-### 3.1. plothrd<a id="31-plothrd"></a>
+### 1.6 Lightcurve Query<a id="16-lightcurve-query"></a>
 
-Returns a HRD with a source or list of sources overlayed over a Gaia 100pc background sample.
+Type argument: 'lightcurve'
 
-<br>
-
-**Usage:**
+Description: Returns lightcurve data from a given survey.
 
-```
-plothrd(source=None,sources=None)
-```
+Supported Arguments: survey, pos, source, radius, username, password, sigmaclip
 
 where:
-
-```
-source = int/str, Gaia source_id
 ```
+username = str, ATLAS username, hence only used in ATLAS queries
 ```
-sources = list of sources
-```
-
-**Returns:** dict
-
 ```
-{
-'type' : 'hrd'
-'source' : int/str, source overlayed in HRD
-'sources' : list, sources overlayed in HRD if multiple were given
-'plot' : bokeh figure object, the actual plot
-'ATKfilename' : the default filename given by ATK
-}
+password = str, ATLAS password, hence only used in ATLAS queries
 ```
-
-<br>
-
-**Example:**
-To retrieve a HRD with a single source overlayed:
 ```
-from AstroToolkit.Tools import plothrd,showplot
-
-plot=plothrd(source=6050296829033196032)
-showplot(plot)
+sigmaclip = int, performs sigma clipping on the data to this number of standard deviations
 ```
+and all other arguments have been defined [above](#1-query).
 
-![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/hrd_example.png?raw=true)
-
-<br><br>
-
-### 4. Lightcurve Tools<a id="4-lightcurve-tools"></a>
-### 4.1. lightcurvequery<a id="41-lightcurvequery"></a>
-
-Returns lightcurve data for a given survey.
-
-<br>
-
-Supported surveys:
+Supported Surveys (and filter bands):
 - ZTF (ztf) - g, r, i
 - ATLAS (atlas) - o, c, i
 - ASAS-SN (asassn) - g, v
 - Gaia (gaia) - g, bp, rp
 - CRTS (crts) - v
 
 **Note:** CRTS' data server is not designed for scripted queries. As a result, queries are limited in the toolkit to one query per 15 seconds. This cooldown is managed using the CRTS_TIMER.txt file in the Settings directory of the package files, and hence this should not be edited.
 
 <br>
 
-```
-lightcurvequery(survey,pos=None,source=None,radius=CONFIG,username=CONFIG,password=CONFIG,sigmaclip=None)
-```
-
-where:
-```
-survey = str, name of a supported survey
-```
-```
-pos = list, [ra,dec]
-```
-```
-source = int/str, Gaia source_id
-```
-```
-radius = int/float, radius of lightcurve query
-```
-```
-username = str, ATLAS username, hence only used in ATLAS queries
-```
-```
-password = str, ATLAS password, hence only used in ATLAS queries
-```
-```
-sigmaclip = int, performs sigma clipping on the data to this number of standard deviations
-```
-
 **Returns:** list of dicts
 
 list of lightcurve data dictionaries with an entry for each band in that survey (see below). Each entry has the format:
 
 ```
 {
 'type' : 'lightcurve'
@@ -696,340 +458,339 @@
          'hjd_ori'/'mjd_ori' : list of returned hjd/mjd values, unedited
          'mag' : list of returned magnitude values
          'mag_err' : list of returned magnitude error values
          }
 }
 ```
 
-<br>
-
-### 4.2. plotlightcurve<a id="42-plotlightcurve"></a>
+<br><br>
 
-Plots lightcurves in the format returned by [lightcurvequery](#41-lightcurvequery).
+### 1.7 SED Query<a id="17-sed-query"></a>
 
-<br>
+Type argument: 'sed'
 
-**Usage:**
+Description: Queries all supported [photometry surveys](#12-photometry-query) and returns SED data.
 
-```
-plotlightcurve(data,colour='black')
-```
+Supported Arguments: pos, source, radius (all defined [above](#1-query))
 
-where:
-```
-data = dict if passing a single lightcurve, list of dicts if passing multiple lightcurves
-```
-```
-colour = str, name of a supported colour. Only used when passing a single lightcurve
-```
-```
-colours = list of strings denoting supported colours, e.g. ['green','red','blue']. Only used when passing multiple lightcurves
-```
+<br>
 
 **Returns:** dict
 
 ```
 {
-'type' : 'lightcurve'
-'survey' : str, survey of lightcurve
+'type' : 'sed'
 'source' : int/str, source used to get data (None if a pos was used)
 'pos': [ra,dec], pos used to get data (None if a source was used)
-'plot' : bokeh figure object, the actual plot
-'ATKfilename' : the default filename given by ATK
+'data': list of entries with each entry taking the form of a dict:
+	{
+    'survey' : str, survey of data point
+    'wavelength' : filter wavelength of data point
+    'flux' : flux through filter
+    'rel_err' : relative error on flux
+    }
 }
 ```
 
-<br>
-
-**Example**:
-To retrieve and plot lightcurves from ZTF:
-```
-from AstroToolkit.Tools import lightcurvequery,plotlightcurve,showplot
-
-lightcurves=lightcurvequery(survey='ztf',source=6050296829033196032)
-showplot(plotlightcurve(lightcurves,colours=['green','red','blue']))
-```
+<br><br>
 
-![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/lightcurve_example.png?raw=true)
+### 1.8 Spectrum Query<a id="18-spectrum-query"></a>
 
-**Note:** Each band will then be toggleable using the legend.
+Type argument: 'spectra'
 
-<br><br>
+Description: Returns spectrum data for a given survey.
 
-### 5. SED Tools<a id="5-sed-tools"></a>
-### 5.1. sedquery<a id="51-sedquery"></a>
+Supported Arguments: survey, pos, source, radius (all defined [above](#1-query))
 
-Queries all supported photometry surveys and returns SED data.
+Supported Surveys: sdss
 
 <br>
 
-**Usage:**
+**Returns:**
 
 ```
-sedquery(pos=None,source=None,radius=CONFIG)
+{
+'type' : 'spectra'
+'survey' : str, survey of detection
+'source' : int/str, source used to get data (None if a pos was used)
+'pos': [ra,dec], pos used to get data (None if a source was used)
+'data': {
+        'wavelength' : list of wavelength values
+        'flux' : list of flux values
+        }
+}
 ```
 
+<br><br>
+
+### 1.9 HRD Query<a id="19-hrd-query"></a>
+
+Type argument: 'hrd'
+
+Description: Returns data for Gaia HRD creation given a Gaia source/list of Gaia sources.
+
+Supported Arguments: sources
+
 where:
 ```
-pos = list, [ra,dec]
-```
-```
-source = int/str, Gaia source_id
-```
-```
-radius = int/float, radius of data query
+sources = single Gaia source or list of Gaia sources
 ```
 
+<br>
+
 **Returns:** dict
 
 ```
-{
-'type' : 'sed'
-'source' : int/str, source used to get data (None if a pos was used)
-'pos': [ra,dec], pos used to get data (None if a source was used)
-'data': list of entries with each entry taking the form of a dict:
-	{
-    'survey' : str, survey of data point
-    'wavelength' : filter wavelength of data point
-    'flux' : flux through filter
-    'rel_err' : relative error on flux
-    }
-}
+'type' : 'hrd'
+'sources' : list, list of input Gaia sources
+'data': {
+        'absg' : list, absolute g magnitudes of given sources
+        'bp-rp' : list, bp-rp values of given sources
+        }
 ```
 
-<br>
-
-### 5.2. plotsed<a id="52-plotsed"></a>
+<br><br>
 
-Plots SEDs in the format returned by [sedquery](#51-sedquery).
+## 2. plot<a id="2-plot"></a>
 
-<br>
+Interprets and plots data.
 
 **Usage:**
 
 ```
-plotsed(data)
+plot(data,type=None)
 ```
 
 where:
-
 ```
-data = dict in format returned by sedquery
+data = list/dict data in structure returned by the query tool
 ```
 
-**Returns:** dict
+<br>
 
-```
-{
-'type' : 'sed'
-'source' : int/str, source used to get data (None if a pos was used)
-'pos': [ra,dec], pos used to get data (None if a source was used)
-'plot' : bokeh figure object, the actual plot
-'ATKfilename' : the default filename given by ATK
-}
-```
+**Note:** If no plot is returned, the 'plot' key of the returned dictionary will be set to None.
 
 <br>
 
-**Example:** To retrieve and plot an SED:
-```
-from AstroToolkit.Tools import sedquery,plotsed,showplot
+**Supported plot types:** image, lightcurve, sed, spectra, powspec, hrd
 
-data=sedquery(source=6050296829033196032)
-showplot(plotsed(data))
-```
+<br>
 
-![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/sed_example.png?raw=true)
+Below is an outline of the usage and output of each plot type. Note that additonal arguments not listed above may be used, see individual plot types below for details.
 
-<br><br>
+<br>
+
+**Shortcuts**:
+
+[Image Plotting](#21-image-plotting)
 
-### 6. Spectrum Tools<a id="6-spectrum-tools"></a>
-### 6.1. spectrumquery<a id="61-spectrumquery"></a>
+[Lightcurve Plotting](#22-lightcurve-plotting)
 
-Returns spectrum data from a given survey.
+[SED Plotting](#23-sed-plotting)
+
+[Spectrum Plotting](#24-spectrum-plotting)
+
+[HRD Plotting](#25-hrd-plotting)
+
+[Power Spectra Plotting](#26-power-spectra-plotting)
 
 <br>
 
-**Usage:**
+### 2.1 Image Plotting<a id="21-image-plotting"></a>
+
+Type argument: 'image'
+
+Description: Plots images in format returned by [image queries](#15-imaging-query).
+
+<br>
+
+**Returns:** dict
 
 ```
-spectrumquery(survey=None,pos=None,source=None,radius=CONFIG)
+{
+'type' : 'image'
+'survey' : str, survey of image
+'source' : int/str, source used to get image (None if a pos was used)
+'pos' : [ra,dec], pos used to get image (None if a source was used)
+'plot' : bokeh figure object, the actual plot
+'ATKfilename' : the default filename given by ATK
+}
 ```
 
+<br><br>
+
+### 2.2 Lightcurve Plotting<a id="22-lightcurve-plotting"></a>
+
+Type argument: 'lightcurve'
+
+Description: Plots lightcurves in the format returned by [lightcurve queries](#16-lightcurve-query). Here, you can either pass a single lightcurve, or multiple lightcurves (e.g. those returned from [lightcurve queries](#16-lightcurve-query)).
+
+Additional Supported Arguments: colour, colours
+
 where:
 ```
-survey = str, name of a supported survey
-```
-```
-pos = list, [ra,dec]
-```
-```
-source = int/str, Gaia source_id
+colour = str, name of a supported colour. Only used when passing a single lightcurve
 ```
 ```
-radius = int/float, radius of data query
+colours = list of strings denoting supported colours, e.g. ['green','red','blue']. Only used when passing multiple lightcurves
 ```
 
-**Returns:** dict
+**Note:** CRTS' data server is not designed for scripted queries. As a result, queries are limited in the toolkit to one query per 15 seconds. This cooldown is managed using the CRTS_TIMER.txt file in the Settings directory of the package files, and hence the contents of this file should not be edited.
+
+<br>
 
+**Returns:** dict
 ```
 {
-'type' : 'spectra'
-'survey' : str, survey of detection
+'type' : 'lightcurve'
+'survey' : str, survey of lightcurve
 'source' : int/str, source used to get data (None if a pos was used)
 'pos': [ra,dec], pos used to get data (None if a source was used)
-'data': {
-        'wavelength' : list of wavelength values
-        'flux' : list of flux values
-        }
+'plot' : bokeh figure object, the actual plot
+'ATKfilename' : the default filename given by ATK
 }
 ```
 
-<br>
+<br><br>
 
-### 6.2. plotspectrum<a id="62-plotspectrum"></a>
+### 2.3 SED Plotting<a id="23-sed-plotting"></a>
 
-Plots spectra in the format returned by [spectrumquery](#61-spectrumquery).
+Type argument: 'sed'
 
-<br>
+Description: Plots SED data in the format returned by [SED queries](#17-sed-query).
 
-**Usage:**
+<br>
 
+**Returns:** dict
 ```
-plotspectrum(data)
+{
+'type' : 'sed'
+'source' : int/str, source used to get data (None if a pos was used)
+'pos': [ra,dec], pos used to get data (None if a source was used)
+'data': list of entries with each entry taking the form of a dict:
+	{
+    'survey' : str, survey of data point
+    'wavelength' : filter wavelength of data point
+    'flux' : flux through filter
+    'rel_err' : relative error on flux
+    }
+}
 ```
 
-where:
+<br><br>
 
-```
-data = dict in format returned by spectrumquery
-```
+### 2.4 Spectrum Plotting<a id="24-spectrum-plotting"></a>
 
-**Returns:** dict
+Type argument: 'spectra'
 
+Description: Plots spectrum data in the format returned by [spectrum queries](#18-spectrum-query).
+
+<br>
+
+**Returns:** dict
 ```
 {
 'type' : 'spectrum'
 'survey' : str, survey of spectrum
 'source' : int/str, source used to get data (None if a pos was used)
 'pos': [ra,dec], pos used to get data (None if a source was used)
 'plot' : bokeh figure object, the actual plot
 'ATKfilename' : the default filename given by ATK
 }
 ```
 
-<br>
+<br><br>
 
-**Example:**
-To retrieve and plot an SDSS spectrum:
-```
-from AstroToolkit.Tools import spectrumquery,plotspectrum,showplot
+### 2.5 HRD Plotting<a id="25-hrd-plotting"></a>
 
-data=spectrumquery(survey='sdss',source=587316166180416640)
-plot=plotspectrum(data)
-showplot(plot)
-```
+Type argument: 'hrd'
 
-![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/spectrum_example.png?raw=true)
+Description: Plots Gaia HRD data in the format returned by [hrd queries](#19-hrd-query).
 
-<br><br>
+<br>
 
-### 7. Timeseries Tools<a id="7-timeseries-tools"></a>
-### 7.1 plotpowspec<a id="71-plotpowspec"></a>
+**Returns:** dict
+```
+{
+'type' : 'hrd'
+'source' : int/str, source overlayed in HRD
+'sources' : list, sources overlayed in HRD if multiple were given
+'plot' : bokeh figure object, the actual plot
+'ATKfilename' : the default filename given by ATK
+}
+```
 
-Plots a power spectrum from lightcurve data in the format returned by [lightcurvequery](#41-lightcurvequery)
+<br><br>
 
-<br>
+### 2.6 Power Spectra Plotting<a id="26-power-spectra-plotting"></a>
 
-**Usage:**
+Type argument: 'powspec'
 
-```
-plotpowspec(data)
-```
+Description: Plots power spectra from lightcurve data in the format returned by [lightcurve queries](#16-lightcurve-query).
 
-where:
-```
-data = dict or list in format returned by lightcurvequery
-```
+<br>
 
 **Returns:** dict
 
 ```
 {
 'type' : 'powspec'
 'survey' : str, survey of lightcurve data given to the powspec tool
 'source' : int/str, source used to get data (None if a pos was used)
 'pos': [ra,dec], pos used to get data (None if a source was used)
 'plot' : bokeh figure object, the actual plot
 'ATKfilename' : the default filename given by ATK
 }
 ```
 
-<br>
-
-**Example:**
-To retrieve lightcurve data from ZTF and plot a power spectrum:
-```
-from AstroToolkit.Tools import lightcurvequery,plotpowspec,showplot
-
-data=lightcurvequery(survey='ztf',source=6050296829033196032)
-plot=plotpowspec(data)
-showplot(plot)
-```
-
-![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/powspec_example.png?raw=true)
-
 <br><br>
 
-### 7.2 tsanalysis<a id="72-tsanalysis"></a>
+### 2.7 Timeseries Analysis<a id="27-timeseries-analysis"></a>
 
-Runs period analysis on lightcurve data in format returned by [lightcurvequery](#lightcurvequery)
+Description: Not explicitly a plotting function, but included here for completeness. Runs period analysis on lightcurve data in format returned by [lightcurve queries](#16-lightcurve-query).
 
 <br>
 
 **Usage:**
 
 ```
 tsanalysis(data)
 ```
 
 where:
 
 ```
-data = dict or list in format returned by lightcurvequery
-```
-
-<br>
-
-**Example:**
-To retrieve lightcurve data from ZTF and perform timeseries analysis:
-```
-from AstroToolkit.Tools import lightcurvequery,tsanalysis
-
-data=lightcurvequery(survey='ztf',source=6050296829033196032)
-plot=tsanalysis(data)
+data = dict or list in format returned by lightcurve queries
 ```
 
-![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/tsanalysis_example.png?raw=true)
-
 <br><br>
 
-## 8. Datapage Tools<a id="8-datapage-tools"></a>
+## 3. Datapage Tools<a id="3-datapage-tools"></a>
 
 These functions are used to create custom datapages from any plots/data supported by AstroToolkit.
 
 **NOTE:** An example of datapage creation can be found within the packages 'Examples' folder, named 'datapage_creation.py' (within the …/Lib/site-packages/AstroToolkit from earlier). This can be imported from a python terminal using from AstroToolkit.Examples import datapage_creation.
 
 Below is the datapage produced by this example. Once the script to create these has been written, they can be a very powerful way to quickly retrieve and show a wide range of information on a system, with the below example easily being generated in under 30s.
 
 ![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/datapage_example.png?raw=true)
 
 <br>
 
-### 8.1. gridsetup<a id="81-gridsetup"></a>
+Shortcuts:
+
+[Grid Creation](#31-gridsetup)
+
+[SIMBAD/Vizier Buttons](#32-getbuttons)
+
+[Metadata Table Creation](#33-getmdtable)
+
+<br><br>
+
+### 3.1 gridsetup<a id="31-gridsetup"></a>
 
 Formats plots for datapage creation by sizing them to a grid of given dimensions.
 
 <br>
 
 **Usage:**
 
@@ -1067,15 +828,15 @@
 
 where the keys "name ..." are the names given to the plots above, and the values 'plot ...' are the plots to which these names refer.
 
 **NOTE:** Again, see the datapage_creation example as noted [above](#8-datapage-tools) for an example.
 
 <br>
 
-### 8.2. getbuttons<a id="82-getbuttons"></a>
+### 3.2 getbuttons<a id="32-getbuttons"></a>
 
 Returns a Bokeh figure containing SIMBAD and Vizier buttons for use in datapages.
 
 <br>
 
 **Usage:**
 
@@ -1111,15 +872,15 @@
 }
 ```
 
 **NOTE:** Again, see the datapage_creation example as noted [above](#8-datapage-tools) for an example.
 
 <br>
 
-### 8.3. getmdtable<a id="83-getmdtable"></a>
+### 3.3 getmdtable<a id="33-getmdtable"></a>
 
 Creates a table of metadata table using data from supported surveys and/or custom data.
 
 <br>
 
 **Usage:**
 
@@ -1185,20 +946,31 @@
 }
 ```
 
 **NOTE:** Again, see the datapage_creation example as noted [above](#8-datapage-tools) for an example.
 
 <br><br>
 
-## 9. File Handling Tools<a id="9-file-handling-tools"></a>
+## 4. File Handling Tools<a id="4-file-handling-tools"></a>
+
 These tools can be used to transform many returned ATK data structures into local files, and vice versa. This process is designed to be completely lossless, allowing for the exact data structure that was used to create a file to be recreated at a later date.
 
 <br>
 
-### 9.1. savedata<a id="91-savedata"></a>
+Shortcuts:
+
+[Data Saving](#41-savedata)
+
+[Data Reading](#42-readdata)
+
+[Export Plots to PNG](#43-export)
+
+<br><br>
+
+### 4.1 savedata<a id="41-savedata"></a>
 
 This tool allows for the saving of many ATK data structures into local files.
 
 Supported ATK data types: data, phot, bulkphot, image, sed, spectra, lightcurve
 
 <br>
 
@@ -1220,15 +992,15 @@
 
 <br>
 
 **Note:** Created files will contain a tag (e.g. ATKimage for an image). This is necessary, as it tells the readdata function (see below) how to interpret the file to recreate the original data structure.
 
 <br>
 
-### 9.2. readdata<a id="92-readdata"></a>
+### 4.2 readdata<a id="42-readdata"></a>
 
 This tool allows for the lossless recreation of ATK data stuctures from files created using [savedata](#91-savedata).
 
 <br>
 
 **Usage:**
 
@@ -1263,15 +1035,15 @@
 
 ![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/struct_recreation_example.png?raw=true)
 
 **Note:** The above example assumes that you have already set a default ATLAS username / password in the [config](#configuration).
 
 <br>
 
-### 9.3. export<a id="93-export"></a>
+### 4.3 export<a id="43-export"></a>
 
 This allows for ATK figures to be saved as a .png file.
 
 <br>
 
 **Usage:**
 
@@ -1285,59 +1057,79 @@
 ```
 ```
 keephtml = bool. To get the filename for the png, the plot must first be saved as a regular bokeh static html file. This tells ATk whether to delete this file or keep it.
 ```
 
 <br><br>
 
-### 10. Miscellaneous Tools<a id="10-miscellaneous-tools"></a>
+## 5. Other Tools<a id="5-other-tools"></a>
 
-These are tools that do not fit into the above categories, but can still be useful for quickly performing some basic functions.
+Below is a list of the other tools available in ATK.
 
-<br>
+Shortcuts:
+
+[Show Plots](531-showplot)
+
+[Save Plots](532-saveplot)
+
+[Proper Motion Correction](533-correctpm)
+
+[Parallax to Distance](534-getdistance)
+
+[Convert Degrees to HMS/DMS](535-convfromdeg)
+
+[Convert from HMS/DMS to Degrees](536-convtodeg)
+
+[Read fits file columns](#57-getcolumn)
+
+[Read Sources from a fits file](#58-getsources)
+
+[Read Positions from a fits file](#59-getpositions)
+
+[Open object in SIMBAD/Vizier](#510-webquery)
 
-### 10.1. showplot<a id="101-showplot"></a>
+### 5.1 showplot<a id="51-showplot"></a>
 
-This allows for the plot dictionaries returned by ATK to be opened in the browser. Doing so will also save the plot locally as a .html file. Can also be used with the same functionality as show() from bokeh for non-ATK bokeh figures.
+Description: This allows for the plot dictionaries returned by ATK to be opened in the browser. Doing so will also save the plot locally as a .html file. Can also be used with the same functionality as show() from bokeh for non-ATK bokeh figures.
 
 <br>
 
 **Usage:**
 ```
 showplot(plot)
 ```
 
 where:
 ```
-plot = ATK plot dictionary
+plot = ATK plot dictionary or bokeh figure
 ```
 
-<br>
+<br><br>
 
-### 10.2. saveplot<a id="102-saveplot"></a>
+### 5.2 saveplot<a id="52-saveplot"></a>
 
-This allows for the plot dictionaries returned by ATK to be saved to local .html files without opening them in the browser. Can also be used with the same functionality as save() from bokeh for non-ATK bokeh figures.
+Description: This allows for the plot dictionaries returned by ATK to be saved to local .html files without opening them in the browser. Can also be used with the same functionality as save() from bokeh for non-ATK bokeh figures.
 
 <br>
 
 **Usage:**
 ```
 saveplot(plot)
 ```
 
 where:
 ```
-plot = ATK plot dictionary
+plot = ATK plot dictionary or bokeh figure
 ```
 
-<br>
+<br><br>
 
-### 10.3. correctpm<a id="103-correctpm"></a>
+### 5.3 correctpm<a id="53-correctpm"></a>
 
-Corrects for proper motion of an object between an input time and a target time.
+Description: Corrects for proper motion of an object between an input time and a target time.
 
 <br>
 
 **Usage:**
 
 ```
 correctpm(inputtime,targettime,ra,dec,pmra,pmdec)
@@ -1366,30 +1158,17 @@
 
 <br>
 
 **Returns:** list
 
 [ra,dec] of object in degrees, corrected for proper motion.
 
-<br>
-
-**Example:**
-To correct an object for proper motion to the year 2000:
-```
-from AstroToolkit.Tools import dataquery,correctpm
-
-gaia_data=dataquery(survey='gaia',source=6050296829033196032)['data']
-ra,dec,pmra,pmdec=gaia_data['ra'][0],gaia_data['dec'][0],gaia_data['pmra'][0],gaia_data['pmdec'][0]
-
-ra_corrected,dec_corrected=correctpm([2016,0],[2000,0],ra,dec,pmra,pmdec)
-```
-
-<br>
+<br><br>
 
-### 10.4. getdistance<a id="104-getdistance"></a>
+### 5.4 getdistance<a id="54-getdistance"></a>
 
 Simply calculates the distance (1/parallax) of an object given its parallax in mas (the unit of parallax in Gaia).
 
 <br>
 
 **Usage:**
 
@@ -1406,15 +1185,15 @@
 
 **Returns:** float
 
 distance of object in pc
 
 <br>
 
-### 10.5. convfromdeg<a id="105-convfromdeg"></a>
+### 5.5 convfromdeg<a id="55-convfromdeg"></a>
 
 Converts deg coordinates to HMS/DMS format
 
 <br>
 
 **Usage:**
 
@@ -1431,15 +1210,15 @@
 
 **Returns:** list
 
 [ra,dec] of object in [HMS,DMS]
 
 <br>
 
-### 10.6. convtodeg<a id="106-convtodeg"></a>
+### 5.6 convtodeg<a id="56-convtodeg"></a>
 
 Converts HMS/DMS coordinates to deg.
 
 <br>
 
 **Usage:**
 
@@ -1456,15 +1235,15 @@
 
 **Returns:** list
 
 [ra,dec] of object in deg
 
 <br>
 
-### 10.7. getcolumn<a id="107-getcolumn"></a>
+### 5.7 getcolumn<a id="57-getcolumn"></a>
 
 Returns a list of values from a .fits file given a column name.
 
 **Usage:**
 
 ```
 getcolumn(file_name,col_name)
@@ -1480,15 +1259,15 @@
 
 **Returns:** list
 
 list of values for that column
 
 <br>
 
-### 10.8. getsources<a id="108-getsources"></a>
+### 5.8 getsources<a id="58-getsources"></a>
 
 Returns a list of source values from a .fits file given a column name, which can either be set in the tool or in the config.
 
 **Usage:**
 
 ```
 getsources(file_name,col_name=CONFIG)
@@ -1504,15 +1283,15 @@
 
 **Returns:** list
 
 list of Gaia sources
 
 <br>
 
-### 10.9. getpositions<a id="109-getpositions"></a>
+### 5.9 getpositions<a id="59-getpositions"></a>
 
 Returns a list of ra,dec values from a .fits file given ra and dec column names, which can either be set in the tool or in the config.
 
 **Usage:**
 
 ```
 getsources(file_name,col_name=CONFIG)
@@ -1525,7 +1304,177 @@
 ```
 col_name = str, comma separated string containing names of ra and dec columns. e.g. col_name = 'RA_ICRS,'DE_ICRS'. Must be in this order.
 ```
 
 **Returns:** list
 
 list of positions [[ra1,dec1],[ra2,dec2]], etc.
+
+### 5.10 webquery<a id="510-webquery"></a>
+
+Performs SIMBAD/Vizier queries given a source/pos in the web browser.
+
+**Usage:**
+
+```
+webquery(type,source=None,pos=None,radius=CONFIG)
+```
+
+where:
+```
+type = str, type of query from 'simbad' or 'vizier'
+```
+```
+pos = list, [ra,dec]
+```
+```
+source = int/str, Gaia source_id
+```
+```
+radius = int/float, radius of data query. If not given, this is taken from simbad_radius or vizier_radius in the config, depending on the query type
+```
+
+**Returns:** None
+
+<br><br>
+
+## Examples<a id="examples"></a>
+
+### Example 1: Fetching and plotting an image
+
+```
+from AstroToolkit.Tools import query,plot,showplot
+
+image=query(type='image',survey='any',source=6050296829033196032,overlays='gaia')
+figure=plot(image)
+showplot(figure)
+```
+
+![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/imaging_example.png?raw=true)
+
+<br><br>
+
+### Example 2: Fetching and plotting a Gaia HRD
+
+```
+from AstroToolkit.Tools import query,plot,showplot
+
+data=query(type='hrd',sources=[6050296829033196032])
+figure=plot(data)
+showplot(figure)
+```
+
+![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/hrd_example.png?raw=true)
+
+<br><br>
+
+### Example 3: Fetching and plotting a ZTF lightcurve
+
+```
+from AstroToolkit.Tools import query,plot,showplot
+
+data=lightcurvequery(type='lightcurve',survey='ztf',source=6050296829033196032)
+showplot(plot(data,colours=['green','red','blue']))
+```
+
+**Note:** Each band will then be toggleable using the legend.
+
+![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/lightcurve_example.png?raw=true)
+
+<br><br>
+
+### Example 4: Fetching and plotting an SED
+
+```
+from AstroToolkit.Tools import query,plot,showplot
+
+data=query(type='sed',source=6050296829033196032)
+showplot(plot(data))
+```
+
+![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/sed_example.png?raw=true)
+
+<br><br>
+
+### Example 5: Fetching and plotting an SDSS spectrum
+
+```
+from AstroToolkit.Tools import query,plot,showplot
+
+data=query(type='spectra',survey='sdss',source=587316166180416640)
+plot=plot(data)
+showplot(plot)
+```
+
+![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/spectrum_example.png?raw=true)
+
+<br><br>
+
+### Example 6: Fetching ZTF ligthcurve data, and then plotting it as a power spectrum
+
+```
+from AstroToolkit.Tools import lightcurvequery,plotpowspec,showplot
+
+data=lightcurvequery(survey='ztf',source=6050296829033196032)
+plot=plotpowspec(data)
+showplot(plot)
+```
+
+![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/powspec_example.png?raw=true)
+
+<br><br>
+
+### Example 7: Fetching Gaia parallax and WISE data
+
+```
+from AstroToolkit.Tools import query
+
+source = 6050296829033196032
+
+parallax = query(type='data',survey='gaia',source=source)['data']['parallax']
+wise_data = query(type='data',survey='wise',source=source)['data']
+```
+
+### Example 8: Fetching 2MASS photometry for an object
+
+```
+from AstroToolkit.Tools import query
+
+data=query(type='phot',survey='twomass',source=6050296829033196032)['data']
+```
+
+### Example 9: Fetching photometry from all available surveys using a bulk photometry query
+
+```
+from AstroToolkit.Tools import query
+
+bulk_phot=query(type='bulkphot',source=6050296829033196032)['data']
+
+gaia_data=bulk_phot['gaia']
+galex_data=bulk_phot['galex']
+```
+
+<br><br>
+
+### Example 10: Fetching ZTF lightcurve data, and performing timeseries analysis
+
+```
+from AstroToolkit.Tools import query,tsanalysis
+
+data=query(type='lightcurve',survey='ztf',source=6050296829033196032)
+plot=tsanalysis(data)
+```
+
+![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/tsanalysis_example.png?raw=true)
+
+<br><br>
+
+### Example 11: Proper motion correction
+
+```
+from AstroToolkit.Tools import query,correctpm
+
+gaia_data=query(type='data',survey='gaia',source=6050296829033196032)['data']
+ra,dec,pmra,pmdec=gaia_data['ra'][0],gaia_data['dec'][0],gaia_data['pmra'][0],gaia_data['pmdec'][0]
+
+ra_corrected,dec_corrected=correctpm([2016,0],[2000,0],ra,dec,pmra,pmdec)
+```
```

### Comparing `AstroToolkit-1.3.5/README.md` & `AstroToolkit-1.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,60 +1,55 @@
+Metadata-Version: 2.1
+Name: AstroToolkit
+Version: 1.4.0
+Summary: A package for the gathering and plotting of astronomical data.
+Author-email: Ethan Moorfield <ethan.moorfield@hotmail.co.uk>
+Project-URL: Homepage, https://github.com/WD-planets/AstroToolkit
+Project-URL: Issues, https://github.com/WD-planets/AstroToolkit/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: astropy==5.2.2
+Requires-Dist: astroquery==0.4.7
+Requires-Dist: bokeh==3.1.1
+Requires-Dist: cmasher==1.6.3
+Requires-Dist: importlib_resources==6.4.0
+Requires-Dist: matplotlib==3.7.5
+Requires-Dist: numba==0.58.1
+Requires-Dist: numpy==1.24.4
+Requires-Dist: pandas==2.0.3
+Requires-Dist: Pillow==10.2.0
+Requires-Dist: PyQt5==5.15.10
+Requires-Dist: PyQt5_sip==12.13.0
+Requires-Dist: Requests==2.31.0
+Requires-Dist: scikit_learn==1.3.2
+Requires-Dist: scipy==1.10.1
+Requires-Dist: selenium==4.17.2
+
 # AstroToolkit
 
-AstroToolkit (ATK) is a set of useful tools for fetching, plotting, and analysing astronomical data.
+AstroToolkit (ATK) is a set of tools for fetching, plotting, and analysing astronomical data.
 
 ## Table of Contents
 
 1. [Installation](#installation)
 2. [Introduction](#introduction)
 3. [Configuration](#configuration)
 4. [Tools](#tools)
+5. [Examples](#examples)
 
 ### ATK Tools
 
-- 1 [Raw Data Tools](#1-raw-data-tools)
-	- 1.1 [dataquery](#11-dataquery)
-	- 1.2 [photquery](#12-photquery)
-	- 1.3 [bulkphotquery](#13-bulkphotquery)
-	- 1.4 [getreddening](#14-getreddening)
-- 2 [Imaging Tools](#2-imaging-tools)
-	- 2.1 [imagequery](#21-imagequery)
-	- 2.2 [plotimage](#22-plotimage)
-- 3 [HRD Tools](#3-hrd-tools)
-	- 3.1 [plothrd](#31-plothrd)
-- 4 [Lightcurve Tools](#4-lightcurve-tools)
-	- 4.1 [lightcurvequery](#41-lightcurvequery)
-	- 4.2 [plotlightcurve](#42-plotlightcurve)
-- 5 [SED Tools](#5-sed-tools)
-	- 5.1 [sedquery](#51-sedquery)
-	- 5.2 [plotsed](#52-plotsed)
-- 6 [Spectrum Tools](#6-spectrum-tools)
-	- 6.1 [spectrumquery](#61-spectrumquery)
-	- 6.2 [plotspectrum](#62-plotspectrum)
-- 7 [Timeseries Tools](#7-timeseries-tools)
-	- 7.1 [plotpowspec](#71-plotpowspec)
-	- 7.2 [tsanalysis](#72-tsanalysis)
-- 8 [Datapage Tools](#8-datapage-tools)
-	- 8.1 [gridsetup](#81-gridsetup)
-	- 8.2 [getbuttons](#82-getbuttons)
-	- 8.3 [getmdtable](#83-getmdtable)
-- 9 [File Handling Tools](#9-file-handling-tools)
-	- 9.1 [savedata](#91-savedata)
-	- 9.2 [readdata](#92-readdata)
-	- 9.3 [export](#93-export)
-- 10 [Miscellaneous Tools](#10-miscellaneous-tools)
-	- 10.1 [showplot](#101-showplot)
-	- 10.2 [saveplot](#102-saveplot)
-	- 10.3 [correctpm](#103-correctpm)
-	- 10.4 [getdistance](#104-getdistance)
-	- 10.5 [convfromdeg](#105-convfromdeg)
-	- 10.6 [convtodeg](#106-convtodeg)
-	- 10.7 [getcolumn](#107-getcolumn)
-	- 10.8 [getsources](#108-getsources)
-	- 10.9 [getpositions](#109-getpositions)
+- 1 [Query](#1-query)
+- 2 [Plot](#2-plot)
+- 3 [Datapage Tools](#3-datapage-tools)
+- 4 [File Handling Tools](#4-file-handling-tools)
+- 5 [Other Tools](#5-other-tools)
 
 <br>
 
 ## Installation<a id="installation"></a>
 
 The package can be installed as with any other package, e.g. using pip:
 ```
@@ -109,33 +104,33 @@
 editconfig(options)
 ```
 
 where options is a dictionary containing key : value pairs to set in the config. The list of accepted keys and their default values are shown below:
 - enable_notifications = False
 	- If True, notifications denoting basic information as each ATK tool is executed will be shown in the terminal. Can be useful for tracking the flow of data.
 - dataquery_radius = 3
-	- This sets the default radius (in arcseconds) to use in the [dataquery](#11-dataquery) tool.
+	- This sets the default radius (in arcseconds) to use in [data queries](#11-data-query).
 - photquery_radius = 3
-	- This sets the default radius (in arcseconds) to use in the [photquery](#12-photquery) tool.
+	- This sets the default radius (in arcseconds) to use in [photometry queries](#12-photometry-query).
 - bulkphotquery_radius = 3
-	- This sets the default radius (in arcseconds) to use in the [bulkphotquery](#13-bulkphotquery) tool.
+	- This sets the default radius (in arcseconds) to use in [bulk photometry queries](#13-bulk-photometry-query).
 - imagequery_size = 30
-	- This sets the default radius (in arcseconds) to use in the [imagequery](#21-imagequery) tool.
+	- This sets the default radius (in arcseconds) to use in [image queries](#15-imaging-query).
 - imagequery_overlays = gaia
-	- This sets the default radius (in arcseconds) to use in the [imagequery](#21-imagequery) tool.
+	- This sets the default radius (in arcseconds) to use in [image queries](#15-imaging-query).
 - lightcurvequery_radius = 3
-	- This sets the default radius (in arcseconds) to use in the [lightcurvequery](#31-lightcurvequery) tool.
+	- This sets the default radius (in arcseconds) to use in [lightcurve queries](#16-lightcurve-query).
 - atlas_username = None
-	- This sets the default username to use for ATLAS lightcurve queries in the [lightcurvequery](#31-lightcurvequery) tool.
+	- This sets the default username to use in ATLAS [lightcurve queries](#16-lightcurve-query).
 - atlas_password = None
-	- This sets the default password to use for ATLAS lightcurve queries in the [lightcurvequery](#31-lightcurvequery) tool.
+	- This sets the default password to use in ATLAS [lightcurve queries](#16-lightcurve-query).
 - sed_radius = 3
-	- This sets the default radius to use in the [sedquery](#41-sedquery) tool.
+	- This sets the default radius to use in [SED queries](#17-sed-query).
 - spectrum_radius = 3
-	- This sets the default radius to use in the [spectrumquery](#51-spectrumquery) tool.
+	- This sets the default radius to use in [spectrum queries](#18-spectrum-query).
 - grid_size = 250
 	- This sets the default grid size to use in the [gridsetup](#71-gridsetup) tool.
 - button_simbad_radius = 3
 	- This sets the default radius to use for the SIMBAD button in the [getbuttons](#72-getbuttons) tool.
 - button_vizier_radius = 3
 	- This sets the default radius to use for the Vizier button in the [getbuttons](#72-getbuttons) tool.
 - plot_size = 400
@@ -169,168 +164,153 @@
 parameter = string, name of config parameter from above list
 ```
 
 **Returns**: value of this parameter in the config.
 
 <br><br>
 
-## Tools
+## Tools<a id="tools"></a>
 
 In this section, the available tools will be outlined. Note that if a parameter is listed as having a default parameter CONFIG, this means that this parameter is taken from the config as listed above. These parameters can still be passed to the tool, in which case the config value will be ignored.
 
 **Note:** most data returned from fetching/plotting tools takes the form of a dictionary. This dictionary contains the returned data, as well as basic information such as the pos/source used to acquire the data. This format is then used by other ATK functions (such as file showing/saving/reading).
 
 **Note:** All plots created by ATK can have their legends toggled by double clicking the plot, and individual data can be hidden by clicking them in the legend.
 
 <br>
 
 **In all data returned by querying tools, the value of the 'data' key will be set to None if no data was returned. Likewise, in all plotting tools, the value of the 'plot' key will be set to None.**
 
 <br>
 
-### 1. Raw Data Tools<a id="1-raw-data-tools"></a>
-### 1.1. dataquery<a id="11-dataquery"></a>
-
-Returns all available data for a given survey (e.g. magnitudes, positions, etc.).
-
-<br>
-
-**Supported surveys:** gaia, galex, rosat, panstarrs, skymapper, sdss, twomass, wise, erosita
+## 1. query<a id="1-query"></a>
 
-<br>
+Returns available data of a given type from a given survey.
 
 **Usage:**
 
 ```
-dataquery(survey,pos=None,source=None,radius=CONFIG)
+query(type,survey=None,pos=None,source=None,radius=CONFIG)
 ```
 
 where:
 
 ```
+type = str, type of data to return
+```
+```
 survey = str, name of a supported survey
 ```
 ```
 pos = list, [ra,dec]
 ```
 ```
 source = int/str, Gaia source_id
 ```
 ```
-radius = int/float, radius of query
+radius = int/float, radius of query of given type. If not given, will be taken from config value for given query type.
 ```
 
-**Returns:** dict
+<br>
 
-```
-{
-'survey' : str, survey of data
-'type' : 'data'
-'source' : int/str, source used to get data (None if a pos was used)
-'pos' : [ra,dec], pos used to get data (None if a source was used)
-'data' : dict, the returned data
-}
-```
+**Note:** If no data is returned, the 'data' key of the returned dictionary will be set to None.
 
 <br>
 
-**Example:**
+**Supported query types:** data, phot, bulkphot, image, lightcurve, sed, spectra, reddening
 
-To retrieve the parallax of a system through Gaia, and its WISE data:
+<br>
 
-```
-from AstroToolkit.Tools import dataquery
+Below is an outline of the usage and output of each query type. Note that additonal arguments not listed above may be used, see individual query types below for details.
 
-source = 6050296829033196032
+<br>
 
-parallax = dataquery(survey='gaia',source=source)['data']['parallax']
-wise_data = dataquery(survey='wise',source=source)['data']
-```
+**Shortcuts**:
 
-<br><br>
+[Data Queries](#11-data-query)
 
-### 1.2. photquery<a id="12-photquery"></a>
+[Photometry Queries](#12-photometry-query)
 
-Returns data from a given survey, with columns filtered to only include photometry and other basic information.
+[Bulk Photomety Queries](#13-bulk-photometry-query)
 
-<br>
+[Reddening Queries](#14-reddening-query)
+
+[Imaging Queries](#15-imaging-query)
+
+[Lightcurve Queries](#16-lightcurve-query)
+
+[SED Queries](#17-sed-query)
 
-**Supported surveys:** gaia,panstarrs,skymapper,galex,rosat,sdss,wise,twomass
+[Spectrum Queries](#18-spectrum-query)
+
+[HRD Queries](#19-hrd-query)
 
 <br>
 
-**Usage:**
+### 1.1 Data Query<a id="11-data-query"></a>
 
-```
-photquery(survey,pos=None,source=None,radius=CONFIG)
-```
+Type argument: 'data'
 
-where:
+Description: Returns all available raw data for a given survey
 
-```
-survey = str, name of a supported survey
-```
-```
-pos = list, [ra,dec]
-```
-```
-source = int/str, Gaia source_id
-```
-```
-radius = int/float, radius of query
-```
+Supported Arguments: survey, pos, source, radius (all defined [above](#1-query))
+
+Supported Surveys: gaia, galex, rosat, panstarrs, skymapper, sdss, twomass, wise, erosita
+
+<br>
 
 **Returns:** dict
 
 ```
 {
 'survey' : str, survey of data
 'type' : 'data'
 'source' : int/str, source used to get data (None if a pos was used)
 'pos' : [ra,dec], pos used to get data (None if a source was used)
 'data' : dict, the returned data
 }
 ```
 
-<br>
-
-**Example:**
+<br><br>
 
-To retrieve the 2MASS photometry for an object:
-```
-from AstroToolkit.Tools import photquery
+### 1.2 Photometry Query<a id="12-photometry-query"></a>
 
-data=photquery(survey='twomass',source=6050296829033196032)['data']
-```
+Type argument: 'phot'
 
-<br>
+Description: Returns all photometry available from a given survey, as well as some basic parameters such as coordinates.
 
-### 1.3. bulkphotquery<a id="13-bulkphotquery"></a>
+Supported Arguments: survey, pos, source, radius (all defined [above](#1-query))
 
-Returns available photometry from all surveys supported by [photquery](#12-photquery).
+Supported Surveys: gaia, panstarrs, skymapper, galex, rosat, sdss, wise, twomass
 
 <br>
 
-**Usage:**
+**Returns:** dict
 
 ```
-bulkphotquery(pos=None,source=None,radius=CONFIG)
+{
+'survey' : str, survey of data
+'type' : 'data'
+'source' : int/str, source used to get data (None if a pos was used)
+'pos' : [ra,dec], pos used to get data (None if a source was used)
+'data' : dict, the returned data
+}
 ```
 
-where:
+<br><br>
 
-```
-pos = list, [ra,dec]
-```
-```
-source = int/str, Gaia source_id
-```
-```
-radius = int/float, radius of query
-```
+### 1.3 Bulk Photometry Query<a id="13-bulk-photometry-query"></a>
+
+Type argument: 'bulkphot'
+
+Description: Returns all photometry available from all surveys supported by [photometry queries](#12-photometry-query)
+
+Supported Arguments: pos, source, radius (all defined [above](#1-query))
+
+<br>
 
 **Returns:** dict
 
 ```
 {
 'type' : 'bulkphot'
 'source' : int/str, source used to get data (None if a pos was used)
@@ -342,50 +322,25 @@
           etc. for each survey in surveys supported by photquery
          }
 }
 ```
 
 **Note:** The value of each survey will be set to None if no data was returned. E.g. if no galex data was returned, the value of the ['galex'] key would be None.
 
-<br>
-
-**Example:**
-
-To retrieve the gaia and galex data for an object:
-
-```
-from AstroToolkit.Tools import bulkphotquery
-
-bulk_phot=bulkphotquery(source=6050296829033196032)['data']
-
-gaia_data=bulk_phot['gaia']
-galex_data=bulk_phot['galex']
-```
-
-<br>
-
-### 1.4. getreddening<a id="14-getreddening"></a>
-
-Returns the reddening of a Gaia source.
+<br><br>
 
-Currently supported reddening surveys:
-- STILISM (https://stilism.obspm.fr/)
+### 1.4. Reddening Query<a id="14-reddening-query"></a>
 
-<br>
+Type argument: 'reddening'
 
-**Usage:**
+Description: Returns the reddening for a given Gaia source from a given survey
 
-```
-getreddening(source)
-```
+Supported Arguments: source (defined [above](#1-query))
 
-where:
-```
-source = int/str, Gaia source_id
-```
+Supported Surveys: stilism (https://stilism.obspm.fr/)
 
 <br>
 
 **Returns:** dict
 
 ```
 {
@@ -400,79 +355,56 @@
          'red_lower' : reddening lower limit
          }
 }
 ```
 
 <br><br>
 
-### 2. Imaging Tools<a id="2-imaging-tools"></a>
-
-These functions retrieve and plotimages from supported surveys.
+### 1.5 Imaging Query<a id="15-imaging-query"></a>
 
-**Note:** When using a 'pos' as input, some detections can be missing for high proper motion objects. When instead using a source as input, this is no longer a problem as the detection search radius is increased to account for this proper motion.
+Type argument: 'image'
 
-<br>
-
-### 2.1. imagequery<a id="21-imagequery"></a>
-
-Retrieves an image from a given survey. Overlays  can be used to overlay detections from different surveys. There are two types of overlay: detections and tracers. Detections are proper motion-corrected circles that scale with the magnitude of the detection, and show that there is data available for a given object in a given survey. 
+Description: Returns an image from a given survey. Overlays  can be used to overlay detections from different surveys. There are two types of overlay: detections and tracers. Detections are proper motion-corrected circles that scale with the magnitude of the detection, and show that there is data available for a given object in a given survey. 
 
 Tracers (which are detections created from lightcurve surveys) can be used both to show that lightcurve data is available, but also to trace an object through time.
 
 **Note:** tracing an object through time works best with ZTF and CRTS overlays, as these give data with the necessary coordinate precision. Other tracer overlays are unlikely to work for this, and will hence only be useful to see where lightcurve data is available.
 
 **Note:** In the case of ATLAS overlays, the radius used is very small due to the time taken to perform ATLAS queries. Only data close to the focus of the image (i.e. at the location of the target object) will be shown. 
 
 **Example:**
 
 ![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/tracer_example.png?raw=true)
 
-<br>
-
-Supported surveys:
-- panstarrs, supported bands = g, r, i, z, y
-- skymapper, supported bands = g, r, i, z, u, v
-- dss, supported bands = g
-
-**Note:** Can also use 'any' to perform an image query according to the hierarchy: panstarrs > skymapper > dss
-
-<br>
-
-Supported overlays: gaia, galex_nuv, galex_fuv, rosat,sdss, twomass, wise, ztf, erosita ,atlas, gaia_lc, asassn, crts
-
-**Note:** Can also use 'all', which will enable overlays for all supported surveys.
-
-<br>
-
-**Usage:**
-
-```
-imagequery(survey,pos=None,source=None,size=CONFIG,band='g',overlays=CONFIG)
-```
+Supported Arguments: survey, pos, source, size, band, overlays
 
 where:
 ```
-survey = str, name of a supported survey
-```
-```
-pos = list, [ra,dec]
-```
-```
-source = int/str, Gaia source_id
-```
-```
 size = int/float, size of image in arcsec
 ```
 ```
 band = str, string containing the required bands (e.g. for all panstarrs bands, use band='grizy')
 ```
 ```
 overlays = str, required detection overlays (e.g. for gaia and wise detections, use overlays='gaia,wise') 
 ```
 
+and all other arguments have been defined [above](#1-query).
+
+Supported overlays: gaia, galex_nuv, galex_fuv, rosat,sdss, twomass, wise, ztf, erosita ,atlas, gaia_lc, asassn, crts
+
+**Note:** Can also use 'all', which will enable overlays for all supported surveys.
+
+Supported Surveys:
+- panstarrs, supported bands = g, r, i, z, y
+- skymapper, supported bands = g, r, i, z, u, v
+- dss, supported bands = g
+
+<br>
+
 **Returns:** dict
 
 ```
 {
 'type' : 'image'
 'survey' : str, image survey
 'source' : int/str, source used to get image (None if a pos was used)
@@ -498,159 +430,47 @@
 'radius' : float, radius of detection
 'corrected' : bool, whether or not the detection has been corrected for proper motion
 'mag' : str, name of the magnitude (column heaader) from a given survey
 'marker' : 'circle' or 'cross', detection symbol to overlay. Circles are scaled with radius, crosses are not (e.g. for surveys without a magnitude to scale by)
 }
 ```
 
-<br>
-
-### 2.2. plotimage<a id="22-plotimage"></a>
-
-Plots images in format returned by [imagequery](#21-imagequery).
-
-<br>
-
-**Usage:**
-
-```
-plotimage(data)
-```
-
-where:
-```
-data = dict in format returned by imagequery
-```
-
-**Returns:** dict
-
-```
-{
-'type' : 'image'
-'survey' : str, survey of image
-'source' : int/str, source used to get image (None if a pos was used)
-'pos' : [ra,dec], pos used to get image (None if a source was used)
-'plot' : bokeh figure object, the actual plot
-'ATKfilename' : the default filename given by ATK
-}
-```
-
-**Note:** if a plot is not returned (e.g. if no data was supplied to the plotting tool), the 'plot' key will be set to None.
-
-<br>
-
-**Example:**
-
-To retrieve and plot an image:
-```
-from AstroToolkit.Tools import imagequery,plotimage,showplot
-
-image=imagequery(survey='any',source=6050296829033196032,overlays='gaia')
-plot=plotimage(image)
-showplot(plot)
-```
-
-![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/imaging_example.png?raw=true)
-
 <br><br>
 
-### 3. HRD Tools<a id="3-hrd-tools"></a>
-### 3.1. plothrd<a id="31-plothrd"></a>
+### 1.6 Lightcurve Query<a id="16-lightcurve-query"></a>
 
-Returns a HRD with a source or list of sources overlayed over a Gaia 100pc background sample.
+Type argument: 'lightcurve'
 
-<br>
-
-**Usage:**
+Description: Returns lightcurve data from a given survey.
 
-```
-plothrd(source=None,sources=None)
-```
+Supported Arguments: survey, pos, source, radius, username, password, sigmaclip
 
 where:
-
-```
-source = int/str, Gaia source_id
 ```
+username = str, ATLAS username, hence only used in ATLAS queries
 ```
-sources = list of sources
-```
-
-**Returns:** dict
-
 ```
-{
-'type' : 'hrd'
-'source' : int/str, source overlayed in HRD
-'sources' : list, sources overlayed in HRD if multiple were given
-'plot' : bokeh figure object, the actual plot
-'ATKfilename' : the default filename given by ATK
-}
+password = str, ATLAS password, hence only used in ATLAS queries
 ```
-
-<br>
-
-**Example:**
-To retrieve a HRD with a single source overlayed:
 ```
-from AstroToolkit.Tools import plothrd,showplot
-
-plot=plothrd(source=6050296829033196032)
-showplot(plot)
+sigmaclip = int, performs sigma clipping on the data to this number of standard deviations
 ```
+and all other arguments have been defined [above](#1-query).
 
-![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/hrd_example.png?raw=true)
-
-<br><br>
-
-### 4. Lightcurve Tools<a id="4-lightcurve-tools"></a>
-### 4.1. lightcurvequery<a id="41-lightcurvequery"></a>
-
-Returns lightcurve data for a given survey.
-
-<br>
-
-Supported surveys:
+Supported Surveys (and filter bands):
 - ZTF (ztf) - g, r, i
 - ATLAS (atlas) - o, c, i
 - ASAS-SN (asassn) - g, v
 - Gaia (gaia) - g, bp, rp
 - CRTS (crts) - v
 
 **Note:** CRTS' data server is not designed for scripted queries. As a result, queries are limited in the toolkit to one query per 15 seconds. This cooldown is managed using the CRTS_TIMER.txt file in the Settings directory of the package files, and hence this should not be edited.
 
 <br>
 
-```
-lightcurvequery(survey,pos=None,source=None,radius=CONFIG,username=CONFIG,password=CONFIG,sigmaclip=None)
-```
-
-where:
-```
-survey = str, name of a supported survey
-```
-```
-pos = list, [ra,dec]
-```
-```
-source = int/str, Gaia source_id
-```
-```
-radius = int/float, radius of lightcurve query
-```
-```
-username = str, ATLAS username, hence only used in ATLAS queries
-```
-```
-password = str, ATLAS password, hence only used in ATLAS queries
-```
-```
-sigmaclip = int, performs sigma clipping on the data to this number of standard deviations
-```
-
 **Returns:** list of dicts
 
 list of lightcurve data dictionaries with an entry for each band in that survey (see below). Each entry has the format:
 
 ```
 {
 'type' : 'lightcurve'
@@ -667,340 +487,339 @@
          'hjd_ori'/'mjd_ori' : list of returned hjd/mjd values, unedited
          'mag' : list of returned magnitude values
          'mag_err' : list of returned magnitude error values
          }
 }
 ```
 
-<br>
-
-### 4.2. plotlightcurve<a id="42-plotlightcurve"></a>
+<br><br>
 
-Plots lightcurves in the format returned by [lightcurvequery](#41-lightcurvequery).
+### 1.7 SED Query<a id="17-sed-query"></a>
 
-<br>
+Type argument: 'sed'
 
-**Usage:**
+Description: Queries all supported [photometry surveys](#12-photometry-query) and returns SED data.
 
-```
-plotlightcurve(data,colour='black')
-```
+Supported Arguments: pos, source, radius (all defined [above](#1-query))
 
-where:
-```
-data = dict if passing a single lightcurve, list of dicts if passing multiple lightcurves
-```
-```
-colour = str, name of a supported colour. Only used when passing a single lightcurve
-```
-```
-colours = list of strings denoting supported colours, e.g. ['green','red','blue']. Only used when passing multiple lightcurves
-```
+<br>
 
 **Returns:** dict
 
 ```
 {
-'type' : 'lightcurve'
-'survey' : str, survey of lightcurve
+'type' : 'sed'
 'source' : int/str, source used to get data (None if a pos was used)
 'pos': [ra,dec], pos used to get data (None if a source was used)
-'plot' : bokeh figure object, the actual plot
-'ATKfilename' : the default filename given by ATK
+'data': list of entries with each entry taking the form of a dict:
+	{
+    'survey' : str, survey of data point
+    'wavelength' : filter wavelength of data point
+    'flux' : flux through filter
+    'rel_err' : relative error on flux
+    }
 }
 ```
 
-<br>
-
-**Example**:
-To retrieve and plot lightcurves from ZTF:
-```
-from AstroToolkit.Tools import lightcurvequery,plotlightcurve,showplot
-
-lightcurves=lightcurvequery(survey='ztf',source=6050296829033196032)
-showplot(plotlightcurve(lightcurves,colours=['green','red','blue']))
-```
+<br><br>
 
-![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/lightcurve_example.png?raw=true)
+### 1.8 Spectrum Query<a id="18-spectrum-query"></a>
 
-**Note:** Each band will then be toggleable using the legend.
+Type argument: 'spectra'
 
-<br><br>
+Description: Returns spectrum data for a given survey.
 
-### 5. SED Tools<a id="5-sed-tools"></a>
-### 5.1. sedquery<a id="51-sedquery"></a>
+Supported Arguments: survey, pos, source, radius (all defined [above](#1-query))
 
-Queries all supported photometry surveys and returns SED data.
+Supported Surveys: sdss
 
 <br>
 
-**Usage:**
+**Returns:**
 
 ```
-sedquery(pos=None,source=None,radius=CONFIG)
+{
+'type' : 'spectra'
+'survey' : str, survey of detection
+'source' : int/str, source used to get data (None if a pos was used)
+'pos': [ra,dec], pos used to get data (None if a source was used)
+'data': {
+        'wavelength' : list of wavelength values
+        'flux' : list of flux values
+        }
+}
 ```
 
+<br><br>
+
+### 1.9 HRD Query<a id="19-hrd-query"></a>
+
+Type argument: 'hrd'
+
+Description: Returns data for Gaia HRD creation given a Gaia source/list of Gaia sources.
+
+Supported Arguments: sources
+
 where:
 ```
-pos = list, [ra,dec]
-```
-```
-source = int/str, Gaia source_id
-```
-```
-radius = int/float, radius of data query
+sources = single Gaia source or list of Gaia sources
 ```
 
+<br>
+
 **Returns:** dict
 
 ```
-{
-'type' : 'sed'
-'source' : int/str, source used to get data (None if a pos was used)
-'pos': [ra,dec], pos used to get data (None if a source was used)
-'data': list of entries with each entry taking the form of a dict:
-	{
-    'survey' : str, survey of data point
-    'wavelength' : filter wavelength of data point
-    'flux' : flux through filter
-    'rel_err' : relative error on flux
-    }
-}
+'type' : 'hrd'
+'sources' : list, list of input Gaia sources
+'data': {
+        'absg' : list, absolute g magnitudes of given sources
+        'bp-rp' : list, bp-rp values of given sources
+        }
 ```
 
-<br>
-
-### 5.2. plotsed<a id="52-plotsed"></a>
+<br><br>
 
-Plots SEDs in the format returned by [sedquery](#51-sedquery).
+## 2. plot<a id="2-plot"></a>
 
-<br>
+Interprets and plots data.
 
 **Usage:**
 
 ```
-plotsed(data)
+plot(data,type=None)
 ```
 
 where:
-
 ```
-data = dict in format returned by sedquery
+data = list/dict data in structure returned by the query tool
 ```
 
-**Returns:** dict
+<br>
 
-```
-{
-'type' : 'sed'
-'source' : int/str, source used to get data (None if a pos was used)
-'pos': [ra,dec], pos used to get data (None if a source was used)
-'plot' : bokeh figure object, the actual plot
-'ATKfilename' : the default filename given by ATK
-}
-```
+**Note:** If no plot is returned, the 'plot' key of the returned dictionary will be set to None.
 
 <br>
 
-**Example:** To retrieve and plot an SED:
-```
-from AstroToolkit.Tools import sedquery,plotsed,showplot
+**Supported plot types:** image, lightcurve, sed, spectra, powspec, hrd
 
-data=sedquery(source=6050296829033196032)
-showplot(plotsed(data))
-```
+<br>
 
-![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/sed_example.png?raw=true)
+Below is an outline of the usage and output of each plot type. Note that additonal arguments not listed above may be used, see individual plot types below for details.
 
-<br><br>
+<br>
+
+**Shortcuts**:
+
+[Image Plotting](#21-image-plotting)
 
-### 6. Spectrum Tools<a id="6-spectrum-tools"></a>
-### 6.1. spectrumquery<a id="61-spectrumquery"></a>
+[Lightcurve Plotting](#22-lightcurve-plotting)
 
-Returns spectrum data from a given survey.
+[SED Plotting](#23-sed-plotting)
+
+[Spectrum Plotting](#24-spectrum-plotting)
+
+[HRD Plotting](#25-hrd-plotting)
+
+[Power Spectra Plotting](#26-power-spectra-plotting)
 
 <br>
 
-**Usage:**
+### 2.1 Image Plotting<a id="21-image-plotting"></a>
+
+Type argument: 'image'
+
+Description: Plots images in format returned by [image queries](#15-imaging-query).
+
+<br>
+
+**Returns:** dict
 
 ```
-spectrumquery(survey=None,pos=None,source=None,radius=CONFIG)
+{
+'type' : 'image'
+'survey' : str, survey of image
+'source' : int/str, source used to get image (None if a pos was used)
+'pos' : [ra,dec], pos used to get image (None if a source was used)
+'plot' : bokeh figure object, the actual plot
+'ATKfilename' : the default filename given by ATK
+}
 ```
 
+<br><br>
+
+### 2.2 Lightcurve Plotting<a id="22-lightcurve-plotting"></a>
+
+Type argument: 'lightcurve'
+
+Description: Plots lightcurves in the format returned by [lightcurve queries](#16-lightcurve-query). Here, you can either pass a single lightcurve, or multiple lightcurves (e.g. those returned from [lightcurve queries](#16-lightcurve-query)).
+
+Additional Supported Arguments: colour, colours
+
 where:
 ```
-survey = str, name of a supported survey
-```
-```
-pos = list, [ra,dec]
-```
-```
-source = int/str, Gaia source_id
+colour = str, name of a supported colour. Only used when passing a single lightcurve
 ```
 ```
-radius = int/float, radius of data query
+colours = list of strings denoting supported colours, e.g. ['green','red','blue']. Only used when passing multiple lightcurves
 ```
 
-**Returns:** dict
+**Note:** CRTS' data server is not designed for scripted queries. As a result, queries are limited in the toolkit to one query per 15 seconds. This cooldown is managed using the CRTS_TIMER.txt file in the Settings directory of the package files, and hence the contents of this file should not be edited.
+
+<br>
 
+**Returns:** dict
 ```
 {
-'type' : 'spectra'
-'survey' : str, survey of detection
+'type' : 'lightcurve'
+'survey' : str, survey of lightcurve
 'source' : int/str, source used to get data (None if a pos was used)
 'pos': [ra,dec], pos used to get data (None if a source was used)
-'data': {
-        'wavelength' : list of wavelength values
-        'flux' : list of flux values
-        }
+'plot' : bokeh figure object, the actual plot
+'ATKfilename' : the default filename given by ATK
 }
 ```
 
-<br>
+<br><br>
 
-### 6.2. plotspectrum<a id="62-plotspectrum"></a>
+### 2.3 SED Plotting<a id="23-sed-plotting"></a>
 
-Plots spectra in the format returned by [spectrumquery](#61-spectrumquery).
+Type argument: 'sed'
 
-<br>
+Description: Plots SED data in the format returned by [SED queries](#17-sed-query).
 
-**Usage:**
+<br>
 
+**Returns:** dict
 ```
-plotspectrum(data)
+{
+'type' : 'sed'
+'source' : int/str, source used to get data (None if a pos was used)
+'pos': [ra,dec], pos used to get data (None if a source was used)
+'data': list of entries with each entry taking the form of a dict:
+	{
+    'survey' : str, survey of data point
+    'wavelength' : filter wavelength of data point
+    'flux' : flux through filter
+    'rel_err' : relative error on flux
+    }
+}
 ```
 
-where:
+<br><br>
 
-```
-data = dict in format returned by spectrumquery
-```
+### 2.4 Spectrum Plotting<a id="24-spectrum-plotting"></a>
 
-**Returns:** dict
+Type argument: 'spectra'
 
+Description: Plots spectrum data in the format returned by [spectrum queries](#18-spectrum-query).
+
+<br>
+
+**Returns:** dict
 ```
 {
 'type' : 'spectrum'
 'survey' : str, survey of spectrum
 'source' : int/str, source used to get data (None if a pos was used)
 'pos': [ra,dec], pos used to get data (None if a source was used)
 'plot' : bokeh figure object, the actual plot
 'ATKfilename' : the default filename given by ATK
 }
 ```
 
-<br>
+<br><br>
 
-**Example:**
-To retrieve and plot an SDSS spectrum:
-```
-from AstroToolkit.Tools import spectrumquery,plotspectrum,showplot
+### 2.5 HRD Plotting<a id="25-hrd-plotting"></a>
 
-data=spectrumquery(survey='sdss',source=587316166180416640)
-plot=plotspectrum(data)
-showplot(plot)
-```
+Type argument: 'hrd'
 
-![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/spectrum_example.png?raw=true)
+Description: Plots Gaia HRD data in the format returned by [hrd queries](#19-hrd-query).
 
-<br><br>
+<br>
 
-### 7. Timeseries Tools<a id="7-timeseries-tools"></a>
-### 7.1 plotpowspec<a id="71-plotpowspec"></a>
+**Returns:** dict
+```
+{
+'type' : 'hrd'
+'source' : int/str, source overlayed in HRD
+'sources' : list, sources overlayed in HRD if multiple were given
+'plot' : bokeh figure object, the actual plot
+'ATKfilename' : the default filename given by ATK
+}
+```
 
-Plots a power spectrum from lightcurve data in the format returned by [lightcurvequery](#41-lightcurvequery)
+<br><br>
 
-<br>
+### 2.6 Power Spectra Plotting<a id="26-power-spectra-plotting"></a>
 
-**Usage:**
+Type argument: 'powspec'
 
-```
-plotpowspec(data)
-```
+Description: Plots power spectra from lightcurve data in the format returned by [lightcurve queries](#16-lightcurve-query).
 
-where:
-```
-data = dict or list in format returned by lightcurvequery
-```
+<br>
 
 **Returns:** dict
 
 ```
 {
 'type' : 'powspec'
 'survey' : str, survey of lightcurve data given to the powspec tool
 'source' : int/str, source used to get data (None if a pos was used)
 'pos': [ra,dec], pos used to get data (None if a source was used)
 'plot' : bokeh figure object, the actual plot
 'ATKfilename' : the default filename given by ATK
 }
 ```
 
-<br>
-
-**Example:**
-To retrieve lightcurve data from ZTF and plot a power spectrum:
-```
-from AstroToolkit.Tools import lightcurvequery,plotpowspec,showplot
-
-data=lightcurvequery(survey='ztf',source=6050296829033196032)
-plot=plotpowspec(data)
-showplot(plot)
-```
-
-![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/powspec_example.png?raw=true)
-
 <br><br>
 
-### 7.2 tsanalysis<a id="72-tsanalysis"></a>
+### 2.7 Timeseries Analysis<a id="27-timeseries-analysis"></a>
 
-Runs period analysis on lightcurve data in format returned by [lightcurvequery](#lightcurvequery)
+Description: Not explicitly a plotting function, but included here for completeness. Runs period analysis on lightcurve data in format returned by [lightcurve queries](#16-lightcurve-query).
 
 <br>
 
 **Usage:**
 
 ```
 tsanalysis(data)
 ```
 
 where:
 
 ```
-data = dict or list in format returned by lightcurvequery
-```
-
-<br>
-
-**Example:**
-To retrieve lightcurve data from ZTF and perform timeseries analysis:
-```
-from AstroToolkit.Tools import lightcurvequery,tsanalysis
-
-data=lightcurvequery(survey='ztf',source=6050296829033196032)
-plot=tsanalysis(data)
+data = dict or list in format returned by lightcurve queries
 ```
 
-![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/tsanalysis_example.png?raw=true)
-
 <br><br>
 
-## 8. Datapage Tools<a id="8-datapage-tools"></a>
+## 3. Datapage Tools<a id="3-datapage-tools"></a>
 
 These functions are used to create custom datapages from any plots/data supported by AstroToolkit.
 
 **NOTE:** An example of datapage creation can be found within the packages 'Examples' folder, named 'datapage_creation.py' (within the …/Lib/site-packages/AstroToolkit from earlier). This can be imported from a python terminal using from AstroToolkit.Examples import datapage_creation.
 
 Below is the datapage produced by this example. Once the script to create these has been written, they can be a very powerful way to quickly retrieve and show a wide range of information on a system, with the below example easily being generated in under 30s.
 
 ![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/datapage_example.png?raw=true)
 
 <br>
 
-### 8.1. gridsetup<a id="81-gridsetup"></a>
+Shortcuts:
+
+[Grid Creation](#31-gridsetup)
+
+[SIMBAD/Vizier Buttons](#32-getbuttons)
+
+[Metadata Table Creation](#33-getmdtable)
+
+<br><br>
+
+### 3.1 gridsetup<a id="31-gridsetup"></a>
 
 Formats plots for datapage creation by sizing them to a grid of given dimensions.
 
 <br>
 
 **Usage:**
 
@@ -1038,15 +857,15 @@
 
 where the keys "name ..." are the names given to the plots above, and the values 'plot ...' are the plots to which these names refer.
 
 **NOTE:** Again, see the datapage_creation example as noted [above](#8-datapage-tools) for an example.
 
 <br>
 
-### 8.2. getbuttons<a id="82-getbuttons"></a>
+### 3.2 getbuttons<a id="32-getbuttons"></a>
 
 Returns a Bokeh figure containing SIMBAD and Vizier buttons for use in datapages.
 
 <br>
 
 **Usage:**
 
@@ -1082,15 +901,15 @@
 }
 ```
 
 **NOTE:** Again, see the datapage_creation example as noted [above](#8-datapage-tools) for an example.
 
 <br>
 
-### 8.3. getmdtable<a id="83-getmdtable"></a>
+### 3.3 getmdtable<a id="33-getmdtable"></a>
 
 Creates a table of metadata table using data from supported surveys and/or custom data.
 
 <br>
 
 **Usage:**
 
@@ -1156,20 +975,31 @@
 }
 ```
 
 **NOTE:** Again, see the datapage_creation example as noted [above](#8-datapage-tools) for an example.
 
 <br><br>
 
-## 9. File Handling Tools<a id="9-file-handling-tools"></a>
+## 4. File Handling Tools<a id="4-file-handling-tools"></a>
+
 These tools can be used to transform many returned ATK data structures into local files, and vice versa. This process is designed to be completely lossless, allowing for the exact data structure that was used to create a file to be recreated at a later date.
 
 <br>
 
-### 9.1. savedata<a id="91-savedata"></a>
+Shortcuts:
+
+[Data Saving](#41-savedata)
+
+[Data Reading](#42-readdata)
+
+[Export Plots to PNG](#43-export)
+
+<br><br>
+
+### 4.1 savedata<a id="41-savedata"></a>
 
 This tool allows for the saving of many ATK data structures into local files.
 
 Supported ATK data types: data, phot, bulkphot, image, sed, spectra, lightcurve
 
 <br>
 
@@ -1191,15 +1021,15 @@
 
 <br>
 
 **Note:** Created files will contain a tag (e.g. ATKimage for an image). This is necessary, as it tells the readdata function (see below) how to interpret the file to recreate the original data structure.
 
 <br>
 
-### 9.2. readdata<a id="92-readdata"></a>
+### 4.2 readdata<a id="42-readdata"></a>
 
 This tool allows for the lossless recreation of ATK data stuctures from files created using [savedata](#91-savedata).
 
 <br>
 
 **Usage:**
 
@@ -1234,15 +1064,15 @@
 
 ![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/struct_recreation_example.png?raw=true)
 
 **Note:** The above example assumes that you have already set a default ATLAS username / password in the [config](#configuration).
 
 <br>
 
-### 9.3. export<a id="93-export"></a>
+### 4.3 export<a id="43-export"></a>
 
 This allows for ATK figures to be saved as a .png file.
 
 <br>
 
 **Usage:**
 
@@ -1256,59 +1086,79 @@
 ```
 ```
 keephtml = bool. To get the filename for the png, the plot must first be saved as a regular bokeh static html file. This tells ATk whether to delete this file or keep it.
 ```
 
 <br><br>
 
-### 10. Miscellaneous Tools<a id="10-miscellaneous-tools"></a>
+## 5. Other Tools<a id="5-other-tools"></a>
 
-These are tools that do not fit into the above categories, but can still be useful for quickly performing some basic functions.
+Below is a list of the other tools available in ATK.
 
-<br>
+Shortcuts:
+
+[Show Plots](531-showplot)
+
+[Save Plots](532-saveplot)
+
+[Proper Motion Correction](533-correctpm)
+
+[Parallax to Distance](534-getdistance)
+
+[Convert Degrees to HMS/DMS](535-convfromdeg)
+
+[Convert from HMS/DMS to Degrees](536-convtodeg)
+
+[Read fits file columns](#57-getcolumn)
+
+[Read Sources from a fits file](#58-getsources)
+
+[Read Positions from a fits file](#59-getpositions)
+
+[Open object in SIMBAD/Vizier](#510-webquery)
 
-### 10.1. showplot<a id="101-showplot"></a>
+### 5.1 showplot<a id="51-showplot"></a>
 
-This allows for the plot dictionaries returned by ATK to be opened in the browser. Doing so will also save the plot locally as a .html file. Can also be used with the same functionality as show() from bokeh for non-ATK bokeh figures.
+Description: This allows for the plot dictionaries returned by ATK to be opened in the browser. Doing so will also save the plot locally as a .html file. Can also be used with the same functionality as show() from bokeh for non-ATK bokeh figures.
 
 <br>
 
 **Usage:**
 ```
 showplot(plot)
 ```
 
 where:
 ```
-plot = ATK plot dictionary
+plot = ATK plot dictionary or bokeh figure
 ```
 
-<br>
+<br><br>
 
-### 10.2. saveplot<a id="102-saveplot"></a>
+### 5.2 saveplot<a id="52-saveplot"></a>
 
-This allows for the plot dictionaries returned by ATK to be saved to local .html files without opening them in the browser. Can also be used with the same functionality as save() from bokeh for non-ATK bokeh figures.
+Description: This allows for the plot dictionaries returned by ATK to be saved to local .html files without opening them in the browser. Can also be used with the same functionality as save() from bokeh for non-ATK bokeh figures.
 
 <br>
 
 **Usage:**
 ```
 saveplot(plot)
 ```
 
 where:
 ```
-plot = ATK plot dictionary
+plot = ATK plot dictionary or bokeh figure
 ```
 
-<br>
+<br><br>
 
-### 10.3. correctpm<a id="103-correctpm"></a>
+### 5.3 correctpm<a id="53-correctpm"></a>
 
-Corrects for proper motion of an object between an input time and a target time.
+Description: Corrects for proper motion of an object between an input time and a target time.
 
 <br>
 
 **Usage:**
 
 ```
 correctpm(inputtime,targettime,ra,dec,pmra,pmdec)
@@ -1337,30 +1187,17 @@
 
 <br>
 
 **Returns:** list
 
 [ra,dec] of object in degrees, corrected for proper motion.
 
-<br>
-
-**Example:**
-To correct an object for proper motion to the year 2000:
-```
-from AstroToolkit.Tools import dataquery,correctpm
-
-gaia_data=dataquery(survey='gaia',source=6050296829033196032)['data']
-ra,dec,pmra,pmdec=gaia_data['ra'][0],gaia_data['dec'][0],gaia_data['pmra'][0],gaia_data['pmdec'][0]
-
-ra_corrected,dec_corrected=correctpm([2016,0],[2000,0],ra,dec,pmra,pmdec)
-```
-
-<br>
+<br><br>
 
-### 10.4. getdistance<a id="104-getdistance"></a>
+### 5.4 getdistance<a id="54-getdistance"></a>
 
 Simply calculates the distance (1/parallax) of an object given its parallax in mas (the unit of parallax in Gaia).
 
 <br>
 
 **Usage:**
 
@@ -1377,15 +1214,15 @@
 
 **Returns:** float
 
 distance of object in pc
 
 <br>
 
-### 10.5. convfromdeg<a id="105-convfromdeg"></a>
+### 5.5 convfromdeg<a id="55-convfromdeg"></a>
 
 Converts deg coordinates to HMS/DMS format
 
 <br>
 
 **Usage:**
 
@@ -1402,15 +1239,15 @@
 
 **Returns:** list
 
 [ra,dec] of object in [HMS,DMS]
 
 <br>
 
-### 10.6. convtodeg<a id="106-convtodeg"></a>
+### 5.6 convtodeg<a id="56-convtodeg"></a>
 
 Converts HMS/DMS coordinates to deg.
 
 <br>
 
 **Usage:**
 
@@ -1427,15 +1264,15 @@
 
 **Returns:** list
 
 [ra,dec] of object in deg
 
 <br>
 
-### 10.7. getcolumn<a id="107-getcolumn"></a>
+### 5.7 getcolumn<a id="57-getcolumn"></a>
 
 Returns a list of values from a .fits file given a column name.
 
 **Usage:**
 
 ```
 getcolumn(file_name,col_name)
@@ -1451,15 +1288,15 @@
 
 **Returns:** list
 
 list of values for that column
 
 <br>
 
-### 10.8. getsources<a id="108-getsources"></a>
+### 5.8 getsources<a id="58-getsources"></a>
 
 Returns a list of source values from a .fits file given a column name, which can either be set in the tool or in the config.
 
 **Usage:**
 
 ```
 getsources(file_name,col_name=CONFIG)
@@ -1475,15 +1312,15 @@
 
 **Returns:** list
 
 list of Gaia sources
 
 <br>
 
-### 10.9. getpositions<a id="109-getpositions"></a>
+### 5.9 getpositions<a id="59-getpositions"></a>
 
 Returns a list of ra,dec values from a .fits file given ra and dec column names, which can either be set in the tool or in the config.
 
 **Usage:**
 
 ```
 getsources(file_name,col_name=CONFIG)
@@ -1495,8 +1332,178 @@
 ```
 ```
 col_name = str, comma separated string containing names of ra and dec columns. e.g. col_name = 'RA_ICRS,'DE_ICRS'. Must be in this order.
 ```
 
 **Returns:** list
 
-list of positions [[ra1,dec1],[ra2,dec2]], etc.
+list of positions [[ra1,dec1],[ra2,dec2]], etc.
+
+### 5.10 webquery<a id="510-webquery"></a>
+
+Performs SIMBAD/Vizier queries given a source/pos in the web browser.
+
+**Usage:**
+
+```
+webquery(type,source=None,pos=None,radius=CONFIG)
+```
+
+where:
+```
+type = str, type of query from 'simbad' or 'vizier'
+```
+```
+pos = list, [ra,dec]
+```
+```
+source = int/str, Gaia source_id
+```
+```
+radius = int/float, radius of data query. If not given, this is taken from simbad_radius or vizier_radius in the config, depending on the query type
+```
+
+**Returns:** None
+
+<br><br>
+
+## Examples<a id="examples"></a>
+
+### Example 1: Fetching and plotting an image
+
+```
+from AstroToolkit.Tools import query,plot,showplot
+
+image=query(type='image',survey='any',source=6050296829033196032,overlays='gaia')
+figure=plot(image)
+showplot(figure)
+```
+
+![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/imaging_example.png?raw=true)
+
+<br><br>
+
+### Example 2: Fetching and plotting a Gaia HRD
+
+```
+from AstroToolkit.Tools import query,plot,showplot
+
+data=query(type='hrd',sources=[6050296829033196032])
+figure=plot(data)
+showplot(figure)
+```
+
+![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/hrd_example.png?raw=true)
+
+<br><br>
+
+### Example 3: Fetching and plotting a ZTF lightcurve
+
+```
+from AstroToolkit.Tools import query,plot,showplot
+
+data=lightcurvequery(type='lightcurve',survey='ztf',source=6050296829033196032)
+showplot(plot(data,colours=['green','red','blue']))
+```
+
+**Note:** Each band will then be toggleable using the legend.
+
+![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/lightcurve_example.png?raw=true)
+
+<br><br>
+
+### Example 4: Fetching and plotting an SED
+
+```
+from AstroToolkit.Tools import query,plot,showplot
+
+data=query(type='sed',source=6050296829033196032)
+showplot(plot(data))
+```
+
+![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/sed_example.png?raw=true)
+
+<br><br>
+
+### Example 5: Fetching and plotting an SDSS spectrum
+
+```
+from AstroToolkit.Tools import query,plot,showplot
+
+data=query(type='spectra',survey='sdss',source=587316166180416640)
+plot=plot(data)
+showplot(plot)
+```
+
+![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/spectrum_example.png?raw=true)
+
+<br><br>
+
+### Example 6: Fetching ZTF ligthcurve data, and then plotting it as a power spectrum
+
+```
+from AstroToolkit.Tools import lightcurvequery,plotpowspec,showplot
+
+data=lightcurvequery(survey='ztf',source=6050296829033196032)
+plot=plotpowspec(data)
+showplot(plot)
+```
+
+![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/powspec_example.png?raw=true)
+
+<br><br>
+
+### Example 7: Fetching Gaia parallax and WISE data
+
+```
+from AstroToolkit.Tools import query
+
+source = 6050296829033196032
+
+parallax = query(type='data',survey='gaia',source=source)['data']['parallax']
+wise_data = query(type='data',survey='wise',source=source)['data']
+```
+
+### Example 8: Fetching 2MASS photometry for an object
+
+```
+from AstroToolkit.Tools import query
+
+data=query(type='phot',survey='twomass',source=6050296829033196032)['data']
+```
+
+### Example 9: Fetching photometry from all available surveys using a bulk photometry query
+
+```
+from AstroToolkit.Tools import query
+
+bulk_phot=query(type='bulkphot',source=6050296829033196032)['data']
+
+gaia_data=bulk_phot['gaia']
+galex_data=bulk_phot['galex']
+```
+
+<br><br>
+
+### Example 10: Fetching ZTF lightcurve data, and performing timeseries analysis
+
+```
+from AstroToolkit.Tools import query,tsanalysis
+
+data=query(type='lightcurve',survey='ztf',source=6050296829033196032)
+plot=tsanalysis(data)
+```
+
+![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/tsanalysis_example.png?raw=true)
+
+<br><br>
+
+### Example 11: Proper motion correction
+
+```
+from AstroToolkit.Tools import query,correctpm
+
+gaia_data=query(type='data',survey='gaia',source=6050296829033196032)['data']
+ra,dec,pmra,pmdec=gaia_data['ra'][0],gaia_data['dec'][0],gaia_data['pmra'][0],gaia_data['pmdec'][0]
+
+ra_corrected,dec_corrected=correctpm([2016,0],[2000,0],ra,dec,pmra,pmdec)
+```
```

### Comparing `AstroToolkit-1.3.5/pyproject.toml` & `AstroToolkit-1.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [project]
 name = "AstroToolkit"
-version = "1.3.5"
+version = "1.4.0"
 authors = [
   { name="Ethan Moorfield", email="ethan.moorfield@hotmail.co.uk"},
 ]
 description = "A package for the gathering and plotting of astronomical data."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Data/data.py` & `AstroToolkit-1.4.0/src/AstroToolkit/Data/data.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Data/imaging.py` & `AstroToolkit-1.4.0/src/AstroToolkit/Data/imaging.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,22 +141,22 @@
 		
 	return image_dict
 
 '''
 returns image dictionaries after correcting for proper motion (if source is used as input)
 '''
 def image_correction(survey,source=None,pos=None,size=30,band='g',overlay=None):
-	from ..Tools import dataquery
+	from ..Tools import query
 	from ..Misc.ProperMotionCorrection import PMCorrection
 	from ..Data.overlays import overlay_selection
 
 	if source!=None:
 		# get Gaia data, if None is returned this will fail, triggering except --> returns None
 
-		gaia_data=dataquery(survey='gaia',source=source)['data']
+		gaia_data=query(type='data',survey='gaia',source=source)['data']
 		if gaia_data!=None:
 			ra,dec,pmra,pmdec=gaia_data['ra'][0],gaia_data['dec'][0],gaia_data['pmra'][0],gaia_data['pmdec'][0]
 		else:
 			raise Exception('Gaia source not found.')
 
 		# get an initial image, which is just used to see when the image was taken
 		image_dict=get_image_dict(survey=survey,pos=pos,source=source,location=[ra,dec],size=size,band=band)
```

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Data/lightcurve_sigma_clip.py` & `AstroToolkit-1.4.0/src/AstroToolkit/Data/lightcurve_sigma_clip.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Data/lightcurves.py` & `AstroToolkit-1.4.0/src/AstroToolkit/Data/lightcurves.py`

 * *Files 0% similar despite different names*

```diff
@@ -544,15 +544,15 @@
 	return data_dict_arr
 
 
 '''
 corrects for proper motion to the survey time (if source input is used)
 '''
 def lightcurve_handling(survey,pos=None,source=None,radius=3,username=None,password=None):
-	from ..Tools import dataquery
+	from ..Tools import query
 	from ..Misc.ProperMotionCorrection import PMCorrection
 
 	# different surveys can have a different number of bands, so need to return an empty list with that survey's band count (i.e. here, ztf is [None,None,None] for g,r,i)
 	if survey=='ztf':
 		f_return=[{'type':'lightcurve','source':source,'pos':pos,'survey':survey,'band':'g','data':None},
 				  {'type':'lightcurve','source':source,'pos':pos,'survey':survey,'band':'r','data':None},
 				  {'type':'lightcurve','source':source,'pos':pos,'survey':survey,'band':'i','data':None}]
@@ -573,15 +573,15 @@
 	if pos!=None:
 		ra,dec=pos[0],pos[1]
 		pmra,pmdec=None,None
 				
 		data=get_data(survey=survey,ra=ra,dec=dec,radius=radius,pos=pos,source=source,username=username,password=password)
 
 	elif source!=None:
-		gaia_data=dataquery(survey='gaia',source=source)['data']
+		gaia_data=query(type='data',survey='gaia',source=source)['data']
 		if gaia_data!=None:
 			ra,dec,pmra,pmdec,ra_j2000,dec_j2000=gaia_data['ra'][0],gaia_data['dec'][0],gaia_data['pmra'][0],gaia_data['pmdec'][0],gaia_data['ra2000'][0],gaia_data['dec2000'][0]
 		else:
 			return f_return
 			
 		# correct for proper motion, if the survey is atlas, use in-built proper motion correction.
 		if survey=='atlas':
```

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Data/overlays.py` & `AstroToolkit-1.4.0/src/AstroToolkit/Data/overlays.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import pandas as pd
 import math
 
 from ..Misc.ProperMotionCorrection import PMCorrection
 from ..Misc.ProperMotionCorrection import get_adapted_radius
-from ..Tools import dataquery
-from ..Tools import lightcurvequery
+from ..Tools import query
 from ..Data.data import get_survey_times
 
 survey_times=get_survey_times()
 
 '''
 get overlay data for a given image and survey. overlay data is in format [{overlay_entry},{overlay_entry},...] with each overlay entry giving the information of a single overlay detection
 '''
@@ -26,30 +25,30 @@
 		image_time=image_dict['data']['image_time']
 
 		# left here as the size of the image isn't always the right radius to use in a query (some use circular, some use square), etc.
 		radius=size
 
 		# get gaia data for the source object, and use its proper motion to scale the radius used.
 		if source!=None:
-			gaia_data=dataquery(survey='gaia',source=source)['data']
+			gaia_data=query(type='data',survey='gaia',source=source)['data']
 			if gaia_data!=None:
 				pmra,pmdec=gaia_data['pmra'][0],gaia_data['pmdec'][0]
 				radius=get_adapted_radius(input=gaia_time,target=image_time,pmra=pmra,pmdec=pmdec,radius=radius)
 			else:
 				return None
 
 		# get overlay survey data
-		nearby_non_gaia=dataquery(survey=survey,pos=location,radius=radius)['data']
+		nearby_non_gaia=query(type='data',survey=survey,pos=location,radius=radius)['data']
 		if nearby_non_gaia==None:
 			return None
 		else:
 			non_gaia_count=len(nearby_non_gaia[list(nearby_non_gaia.keys())[0]])
 	
 		# get nearby gaia data (now using the radius calculated above)
-		nearby_gaia=dataquery(survey='gaia',pos=location,radius=radius)['data']
+		nearby_gaia=query(type='data',survey='gaia',pos=location,radius=radius)['data']
 		if nearby_gaia!=None:
 			gaia_count=len(nearby_gaia[list(nearby_gaia.keys())[0]])
 				
 		skip_mag=False
 		nearby_survey_ra=nearby_non_gaia[ra_name]
 		nearby_survey_dec=nearby_non_gaia[dec_name]
 		if mag_name!=None:
@@ -132,33 +131,33 @@
 			radius=math.sqrt(2*(size/2)**2)
 		elif survey=='atlas' or survey=='gaia_lc' or survey=='asassn' or survey=='crts':
 			radius=size
 
 		# get lightcurve data in format [band1,band2,etc]
 		if survey!='gaia_lc':
 			if source==None:
-				data_arr=lightcurvequery(survey=survey,pos=location,radius=radius)
+				data_arr=query(type='lightcurve',survey=survey,pos=location,radius=radius)
 			else:
-				data_arr=lightcurvequery(survey=survey,source=source,radius=radius)
+				data_arr=query(type='lightcurve',survey=survey,source=source,radius=radius)
 		else:
 			if source==None:
-				data_arr=lightcurvequery(survey='gaia',pos=location,radius=radius)
+				data_arr=query(type='lightcurve',survey='gaia',pos=location,radius=radius)
 			else:
-				data_arr=lightcurvequery(survey='gaia',source=source,radius=radius)
+				data_arr=query(type='lightcurve',survey='gaia',source=source,radius=radius)
 
 		data_exists=False		
 		for i,val in enumerate(data_arr):
-			if val!=None:
+			if val['data']!=None:
 				data_exists=True
 
 		if data_exists==False:
 			return None
 
 		# concats the above list of data for any None returns (e.g. [g,r,None] --> [g,r])
-		data_arr=[x for x in data_arr if x is not None]	
+		data_arr=[x for x in data_arr if x['data'] is not None]	
 
 		# combines all available data into single lists, with 'band' holding the band that this data is from
 		ra_arr=[]
 		dec_arr=[]
 		band=[]
 
 		for element in data_arr:
```

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Data/photometry.py` & `AstroToolkit-1.4.0/src/AstroToolkit/Data/photometry.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Data/reddening.py` & `AstroToolkit-1.4.0/src/AstroToolkit/Data/reddening.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from ..Tools import dataquery,getdistance
+from ..Tools import query,getdistance
 
 import pandas as pd
 import requests
 from requests.adapters import HTTPAdapter, Retry
 from io import StringIO
 import math
 
 # this code is adapted from https://stilism.obspm.fr/static/scripts/stilism_dist.py
 def getreddening(source=None):
 	# get gaia data of source
-	gaia_data=dataquery(survey='gaia',source=source)['data']
+	gaia_data=query(type='data',survey='gaia',source=source)['data']
 
 	gal_lon,gal_lat,parallax,parallax_error=gaia_data['l'][0],gaia_data['b'][0],gaia_data['parallax'][0],gaia_data['parallax_error'][0]
 	
 	distance=getdistance(parallax)
 	distance_plus_err=getdistance(parallax+parallax_error)
 	distance_sub_err=getdistance(parallax-parallax_error)
 
 	# perform reddening query
-	def query(gal_lon,gal_lat,distance):
+	def do_query(gal_lon,gal_lat,distance):
 		url=f'http://stilism.obspm.fr/reddening?frame=galactic&vlong={gal_lon}&ulong=deg&vlat={gal_lat}&ulat=deg&distance={distance}'
 	
 		s=requests.Session()
 		retries=Retry(total=5,backoff_factor=1)
 		s.mount('http://',HTTPAdapter(max_retries=retries))
 
 		r=requests.get(url,allow_redirects=True,timeout=30)
@@ -32,19 +32,19 @@
 			df=pd.read_csv(file)
 			
 			return df
 		else:
 			return None
 	
 	# get reddening at distance+-error, and use these upper and lower bounds to calculate errors on reddening
-	red_df=query(gal_lon=gal_lon,gal_lat=gal_lat,distance=distance)
-	red_max_df=query(gal_lon=gal_lon,gal_lat=gal_lat,distance=distance_plus_err)
-	red_min_df=query(gal_lon=gal_lon,gal_lat=gal_lat,distance=distance_sub_err)
+	red_df=do_query(gal_lon=gal_lon,gal_lat=gal_lat,distance=distance)
+	red_max_df=do_query(gal_lon=gal_lon,gal_lat=gal_lat,distance=distance_plus_err)
+	red_min_df=do_query(gal_lon=gal_lon,gal_lat=gal_lat,distance=distance_sub_err)
 
-	if red_df==None or red_max_df==None or red_min_df==None:
+	if not isinstance(red_df,pd.DataFrame)or not isinstance(red_max_df,pd.DataFrame) or not isinstance(red_min_df,pd.DataFrame):
 		return {'type':'reddening','source':source,'data':None}
 
 	reddening_upper=red_max_df['reddening[mag]'].tolist()[0]-red_df['reddening[mag]'].tolist()[0]
 	reddening_lower=red_min_df['reddening[mag]'].tolist()[0]-red_df['reddening[mag]'].tolist()[0]
 
 	# grab values at the central distance
 	dist=red_df['distance[pc]'].tolist()[0]
```

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Data/sed.py` & `AstroToolkit-1.4.0/src/AstroToolkit/Data/sed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from re import S
 import astropy.units as u
 import numpy as np
 import pandas as pd
 
-from ..Tools import bulkphotquery
+from ..Tools import query
 from .data import get_survey_times
 
 survey_times=get_survey_times()
 
 '''
 gets flux using wavelength and zeropoint of a filter, and magnitude through it
 '''
@@ -67,15 +67,15 @@
 
 	return sed_arr
 
 '''
 uses bulk phot to gather photometry for all available surveys, and then grabs sed points for each survey that returns data
 '''
 def get_data(source=None,pos=None,radius=3):
-	bulkphot=bulkphotquery(source=source,pos=pos,radius=radius)
+	bulkphot=query(type='bulkphot',source=source,pos=pos,radius=radius)
 
 	sed_data=[]
 	for key in bulkphot['data']:
 		if bulkphot['data'][key]!=None:
 			phot=bulkphot['data'][key]
 			# order of parameters (e.g. mag_names, error_names, zero_points, wavelengths) must match
 			if key=='gaia':
```

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Data/spectra.py` & `AstroToolkit-1.4.0/src/AstroToolkit/Data/spectra.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,24 +32,24 @@
 	return spectrum_dict
 
 '''
 handles input survey and accounts for proper motion before sending the request
 '''
 def survey_map(survey,pos=None,source=None,radius=3):
 	from ..Data.data import get_survey_times
-	from ..Tools import dataquery
+	from ..Tools import query
 	from ..Misc.ProperMotionCorrection import PMCorrection
 		
 	survey_times=get_survey_times()
 
 	if pos!=None:
 		ra,dec=pos[0],pos[1]
 	
 	elif source!=None:
-		gaia_data=dataquery(survey='gaia',source=source)['data']
+		gaia_data=query(type='data',survey='gaia',source=source)['data']
 		# correct for proper motion to survey time
 		if gaia_data!=None:
 			ra,dec,pmra,pmdec=gaia_data['ra'][0],gaia_data['dec'][0],gaia_data['pmra'][0],gaia_data['pmdec'][0]
 			pos_corrected=PMCorrection(survey_times['gaia'],survey_times[survey],ra,dec,pmra,pmdec)
 			ra,dec=pos_corrected[0],pos_corrected[1]
 		else:
 			raise Exception('Gaia source not found.')
```

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Datapages/buttons.py` & `AstroToolkit-1.4.0/src/AstroToolkit/Datapages/buttons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from bokeh.models import CustomJS, Button
 from bokeh.layouts import column
 
-from ..Tools import dataquery
+from ..Tools import query
 from ..Misc.ProperMotionCorrection import get_adapted_radius
 
 def getinfobuttons(grid_size,source=None,pos=None,simbad_radius=3,vizier_radius=3):
 	button_width=round(grid_size/2)
 	button_height=round(button_width/3)
 
 	# SIMBAD button
 	simbad_button = Button(label="SIMBAD",button_type='primary',height=button_height,width=button_width)	
 
 	if pos!=None:
 		ra,dec=pos[0],pos[1]
 	elif source!=None:
-		gaia_data=dataquery(survey='gaia',source=source)['data']
+		gaia_data=query(type='data',survey='gaia',source=source)['data']
 		ra,dec,pmra,pmdec=gaia_data['ra'][0],gaia_data['dec'][0],gaia_data['pmra'][0],gaia_data['pmdec'][0]
 		
 		# Scale search radius to include ~26 years of potential proper motion (doesn't actually correct coordinates, just gives a buffer)
 		simbad_radius=get_adapted_radius([2016,0],[1990,0],pmra,pmdec,simbad_radius)
 		vizier_radius=get_adapted_radius([2016,0],[1990,0],pmra,pmdec,vizier_radius)
 	
 	# format URL that the button uses
```

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Datapages/grid.py` & `AstroToolkit-1.4.0/src/AstroToolkit/Datapages/grid.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Datapages/metadata.py` & `AstroToolkit-1.4.0/src/AstroToolkit/Datapages/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from bokeh.models import ColumnDataSource,DataTable,TableColumn
 import pandas as pd
 
-from ..Tools import dataquery
+from ..Tools import query
 from ..Data.data import get_survey_list
 
 '''
 appends data points to the lists in list_dict
 '''
 def getdata(list_dict,sub_dict,survey,source,pos,default):
     supported_surveys=get_survey_list()    
@@ -16,19 +16,19 @@
     value_list=list_dict['value_list']
     error_list=list_dict['error_list']
     note_list=list_dict['note_list']
 
     # if key is a survey, grabs the data for that survey
     if survey in supported_surveys:
         if source!=None:
-            data=dataquery(survey=survey,source=source)['data']
+            data=query(type='data',survey=survey,source=source)['data']
             if data==None:
                 return list_dict
         elif pos!=None:
-            data=dataquery(survey=survey,pos=pos)['data']
+            data=query(type='data',survey=survey,pos=pos)['data']
             if data==None:
                 return list_dict
        
     # if a key (survey) has 'default' as its value, sets the default sub_dict used to create the data table
     if default==True:
         if survey=='gaia':
             sub_dict={'parameters':['source_id','ra','dec','pmra','pmdec','parallax','phot_g_mean_mag','phot_bp_mean_mag','phot_rp_mean_mag'],
```

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Examples/datapage_creation.py` & `AstroToolkit-1.4.0/src/AstroToolkit/Examples/datapage_creation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,42 @@
-from AstroToolkit.Tools import imagequery,plotimage,plothrd,sedquery,plotsed,spectrumquery,plotspectrum,lightcurvequery,plotlightcurve,plotpowspec,getbuttons,gridsetup,getmdtable,showplot,export
+from AstroToolkit.Tools import query,plot,getbuttons,gridsetup,getmdtable,showplot
 from bokeh.layouts import column,row,layout
 from bokeh.plotting import output_file
 
 # source = Hu Leo
 #source=2552928187080872832
 source=587316166180416640
 
 # set grid size (scales overally size of datapage)
 grid_size=275
 
 # get image data and plot it
-image_data=imagequery(survey='any',source=source,overlays='gaia,galex_nuv,galex_fuv')
-image=plotimage(image_data)
+image_data=query(type='image',survey='any',source=source,overlays='gaia,galex_nuv,galex_fuv')
+image=plot(image_data)
 
 # get hrd
-hrd=plothrd(source=source)
+hrd_data=query(type='hrd',sources=source)
+hrd=plot(hrd_data)
 
 # get sed data and plot it
-sed_data=sedquery(source=source)
-sed=plotsed(sed_data)
+sed_data=query(type='sed',source=source)
+sed=plot(sed_data)
 
 # get spectrum data and plot it
-spectrum_data=spectrumquery(survey='sdss',source=source)
-spectrum=plotspectrum(spectrum_data)
+spectrum_data=query(type='spectra',survey='sdss',source=source)
+spectrum=plot(spectrum_data)
 
 # get lightcurve data [g,r,i]
-lightcurve_data=lightcurvequery(survey='ztf',source=source)
+lightcurve_data=query(type='lightcurve',survey='ztf',source=source)
 
 # plot each lightcurve in lightcurve_data and set colour of each plot
-lightcurves=plotlightcurve(lightcurve_data,colours=['green','red','blue'])
+lightcurves=plot(lightcurve_data,colours=['green','red','blue'])
 
 # plot power spectrum data (lightcurve_data)
-power_spectrum=plotpowspec(lightcurve_data)
+power_spectrum=plot(lightcurve_data,type='powspec',)
 
 # get SIMBAD and Vizier buttons
 buttons=getbuttons(grid_size=grid_size,source=source)
 
 # make a custom metadatatable entry
 custom_entry={
     'parameters':['one'],
```

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Misc/ProperMotionCorrection.py` & `AstroToolkit-1.4.0/src/AstroToolkit/Misc/ProperMotionCorrection.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Misc/coord_conversion.py` & `AstroToolkit-1.4.0/src/AstroToolkit/Misc/coord_conversion.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Misc/file_handling.py` & `AstroToolkit-1.4.0/src/AstroToolkit/Misc/file_handling.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Misc/file_naming.py` & `AstroToolkit-1.4.0/src/AstroToolkit/Misc/file_naming.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,18 +68,18 @@
 		print('objRef Error')
 		return None
 
 	return objRef
 
 def convertsource(source):
 	from ..Misc.ProperMotionCorrection import PMCorrection as CorrectPM
-	from ..Tools import dataquery	
+	from ..Tools import query	
 
 	# Get Gaia data
-	gaia_data=dataquery(survey='gaia',source=source)['data']
+	gaia_data=query(type='data',survey='gaia',source=source)['data']
 	if gaia_data!=None:
 		ra,dec,pmra,pmdec=gaia_data['ra'][0],gaia_data['dec'][0],gaia_data['pmra'][0],gaia_data['pmdec'][0]
 		pos=[ra,dec]
 	else:
 		return 'SourceNotFound'
 
 	# Correct proper motion to epoch of 2000 used for coordinates. Gaia coordinates are already in ICRS frame of reference so don't need to do anything here.
@@ -93,20 +93,23 @@
 def name_file(data,data_type):
 	# names files based on their type
 	if data_type=='ATKimage':
 		source=data['source']
 		pos=data['pos']
 		survey=data['survey']
 	elif data_type=='ATKhrd':
-		source=data['source']
 		sources=data['sources']
-		if sources!=None:
-			file_name=f'MultipleSources_ATKhrd.html'
-			return file_name
-		survey=None
+		if isinstance(sources,list):
+			if len(sources)>1:
+				file_name=f'MultipleSources_ATKhrd.html'
+			else:
+				file_name=f'{sources[0]}_ATKhrd.html'
+		else:
+			file_name={f'{sources}_ATKhrd.html'}
+		return file_name
 	elif data_type=='ATKpowspec' or data_type=='ATKlightcurve':
 		if isinstance(data,list):
 			# just grab data from first non-None band, since sources and positions will all be the same
 			for band in data:
 				if band['data']!=None:
 					source=band['source']
 					pos=band['pos']
```

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Misc/input_validation.py` & `AstroToolkit-1.4.0/src/AstroToolkit/Misc/input_validation.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 				raise Exception(f'Unsupported photquery survey. Supported photquery surveys are [gaia,galex,rosat,panstarrs,skymapper,sdss,twomass,wise].')
 		elif tool=='lightcurvequery':
 			if survey not in ['ztf','atlas','gaia','asassn','crts','any']:
 				raise Exception(f'Unsupported lightcurvequery survey. Supported lightcurvequery surveys are [ztf,atlas,gaia,asassn,crts,any].')
 		elif tool=='spectrumquery':
 			if survey not in ['sdss']:
 				raise Exception(f'Unsupported spectrumquery survey. Supported spectrumquery surveys are [sdss].')
+		elif tool=='reddeningquery':
+			if survey not in ['stilism']:
+				raise Exception(f'Unsupported reddeningquery survey. Supported reddeningquery surveys are [stilism]')
 	
 	# handles pos input validation
 	if 'pos' in keys:
 		if parameters['pos']!=None:
 			pos=parameters['pos']
 			if not isinstance(pos,list):
 				data_type=type(survey)
```

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Misc/read_fits.py` & `AstroToolkit-1.4.0/src/AstroToolkit/Misc/read_fits.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Plotting/HRD.py` & `AstroToolkit-1.4.0/src/AstroToolkit/Plotting/HRD.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,22 +6,44 @@
 import cmasher as cmr
 from bokeh.plotting import figure
 import os
 from importlib_resources import files
 from bokeh.models import CustomJS
 from bokeh import events
 
-from ..Tools import dataquery
+from ..Tools import query
 
 fits_file = files('AstroToolkit.Plotting').joinpath('backdrop_hrd_allmags.fits')
 
+def get_data(sources):
+	if not isinstance(sources,list):
+		data=query(type='data',survey='gaia',source=sources)['data']
+		if data!=None:
+			gmag,bpmag,rpmag,parallax=data['phot_g_mean_mag'][0],data['phot_bp_mean_mag'][0],data['phot_rp_mean_mag'][0],data['parallax'][0]
+			x=bpmag-rpmag
+			y=gmag+5*np.log10(parallax/1000)+5
+		
+		hrd_data={'type':'hrd','sources':[sources],'data':{'absg':[y],'bp-rp':[x]}}
+	else:
+		x=[]
+		y=[]
+		for i in range(0,len(sources)):
+			data=query(type='data',survey='gaia',source=sources[i])['data']
+			gmag,bpmag,rpmag,parallax=data['phot_g_mean_mag'][0],data['phot_bp_mean_mag'][0],data['phot_rp_mean_mag'][0],data['parallax'][0]
+			x.append(bpmag-rpmag)
+			y.append(gmag+5*np.log10(parallax/1000)+5)
+
+		hrd_data={'type':'hrd','sources':sources,'data':{'absg':y,'bp-rp':x}}
+
+	return hrd_data
+
 '''
 Creates the HRD plot with a source/sources as an overlay
 '''
-def get_plot(source=None,sources=None):
+def get_plot(data):
 	# reads the background file ('backdrop_hrd_allmags.fits') into separate datasets based on their object classifications.
 	background=Table.read(fits_file).to_pandas()
 	background_100pc=background.loc[background['type']==b'100pc']
 	background_wd=background.loc[background['type']==b'WD']
 	background_cv=background.loc[background['type']==b'CV']
 	background_wd_dm=background.loc[background['type']==b'WD+dM']
 	background_sd=background.loc[background['type']==b'SD']
@@ -60,52 +82,30 @@
 		colour=["#%02x%02x%02x" % (int(r), int(g), int(b)) for r, g, b, _ in 255*colour_maps[i](weights)]
 		colour_arr.append(colour)
 
 	# Create plot
 	plot=figure(width=400,height=400,title='Gaia HRD',x_axis_label=r'\[\text{bp-rp}\]',y_axis_label=r'\[\text{abs g}\]')
 	plot.y_range.flipped = True
 
+	if len(x)>1:
+		label='Gaia sources'
+	else:
+		label='Gaia source'
+
+	for x,y in zip(data['data']['bp-rp'],data['data']['absg']):
+		if not math.isnan(x) and not math.isnan(y):
+			plot.scatter(x=x,y=y,marker='square_dot',line_color='black',fill_color=None,size=10,line_width=2,legend_label=label,level='overlay')
+
 	# sets labels for legend
 	labels=['100pc','WDs','CVs','WD+dM','SDs']
 	# places background points with their colours set, and addstheir respective category to the legend
 	for i in range(0,len(x_arr)):
 		plot.scatter(x_arr[i],y_arr[i],size=3,color=colour_arr[i],legend_label=labels[i])
 
 	# overlays source on top of background sample as long as all the necessary data is available
-	if source!=None:
-		data=dataquery(survey='gaia',source=source)['data']
-		if data==None:
-			return None
-		gmag,bpmag,rpmag,parallax=data['phot_g_mean_mag'][0],data['phot_bp_mean_mag'][0],data['phot_rp_mean_mag'][0],data['parallax'][0]
-		x=bpmag-rpmag
-		y=gmag+5*np.log10(parallax/1000)+5
-		
-		if not math.isnan(gmag) and not math.isnan(bpmag) and not math.isnan(rpmag) and not math.isnan(parallax):
-			if parallax>0:
-				plot.scatter(x=x,y=y,marker='square_dot',line_color='black',fill_color=None,size=20,line_width=2,legend_label='Source',level='overlay')
-			else:
-				return None
-		else:
-			return None
-	
-	# same as above but handles multiple sources
-	elif sources!=None:
-		for i in range(0,len(sources)):
-			data=dataquery(survey='gaia',source=sources[i])['data']
-			gmag,bpmag,rpmag,parallax=data['phot_g_mean_mag'][0],data['phot_bp_mean_mag'][0],data['phot_rp_mean_mag'][0],data['parallax'][0]
-			x=bpmag-rpmag
-			y=gmag+5*np.log10(parallax/1000)+5
-			
-			if not math.isnan(gmag) and not math.isnan(bpmag) and not math.isnan(rpmag) and not math.isnan(parallax):
-				if parallax>0:
-					plot.scatter(x=x,y=y,marker='square_dot',line_color='black',fill_color=None,size=10,line_width=2,legend_label='Sources',level='overlay')
-				else:
-					return None
-			else:
-				pass
 
 	if plot!=None:
 		plot.legend.click_policy="hide"		
 
 		# Double click to hide legend
 		toggle_legend_js = CustomJS(args=dict(leg=plot.legend[0]), code='''
 			 if (leg.visible) {
```

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Plotting/backdrop_hrd_allmags.fits` & `AstroToolkit-1.4.0/src/AstroToolkit/Plotting/backdrop_hrd_allmags.fits`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Plotting/imaging.py` & `AstroToolkit-1.4.0/src/AstroToolkit/Plotting/imaging.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Plotting/lightcurves.py` & `AstroToolkit-1.4.0/src/AstroToolkit/Plotting/lightcurves.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Plotting/powspec.py` & `AstroToolkit-1.4.0/src/AstroToolkit/Plotting/powspec.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Plotting/sed.py` & `AstroToolkit-1.4.0/src/AstroToolkit/Plotting/sed.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Plotting/spectra.py` & `AstroToolkit-1.4.0/src/AstroToolkit/Plotting/spectra.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Timeseries/README - Windows.txt` & `AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/README - Windows.txt`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Timeseries/README.txt` & `AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/README.txt`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Timeseries/aov.f90` & `AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/aov.f90`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Timeseries/aovconst.f90` & `AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/aovconst.f90`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Timeseries/aovsub.f90` & `AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/aovsub.f90`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Timeseries/build.sh` & `AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/build.sh`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Timeseries/buildwin.bat` & `AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/buildwin.bat`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Timeseries/pyaov.pdf` & `AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/pyaov.pdf`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Timeseries/pyaov.py` & `AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/pyaov.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Timeseries/ztfanalysis.py` & `AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/ztfanalysis.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit/Tools.py` & `AstroToolkit-1.4.0/src/AstroToolkit/Tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 '''
 Changelog:
-- added check for negative parallaxes in HRD plotting
+- added a webquery tool to perform SIMBAD/Vizier searches (matches functionality of datapage buttons)
+- updated README to reflect new functionality
+- Combined all query tools into a single tool 'query' which takes a 'type' argument.
+- Combined all plotting tools into a single tool 'plot' which automatically tries to find the data type, or takes an argument 'type' as an override.
+	- These two changes massively decrease the number of imports needed, and are now the main functions around which the whole toolkit works.
+- Updated hrd plotting to fit the query/plot tools
+- Updated datapage_creation example for new functionality
 '''
 
 '''
 To-Do:
 HIGH PRIORITY
-- specify versions in requirements
-- check config for if all keys are present, if not then make a new config file with current keys saved
+- Better scaling for detection overlay sizes
+- check config for if all keys are present, if not then make a new config file with existing key:value pairs saved
 - talk to boris about combining lightcurves
 - update README to reflect new changes (plots stored as dictionaries, showplot/saveplot/export now required to use on ATK plot objects, updated grid functionality)
-
-- fix issues with links in github/pypi not working (the ones on github are just me forgetting to format them properly), I think if possible just list features in pypi and have link to github 
-  for actual documentation. Not sure if external people (i.e. those outside WDPlanets) can definitely view this repository though?
   
 MEDIUM PRIORITY
-- could combine all plotting tools into a central plot function, which then uses the 'type' stored in data dicts to plot it automatically
 - add defaults for newly supported surveys to metadata table
 - comment new code
-- 'plot has no renderer' bokeh warning
 - clean up / optimize anything that needs it to make development easier
 - make some sort of error logging system that notes any errors encountered during runtime, maybe via a log file of some sort (?)
 
 LOW PRIORITY
 - (WEBSITE STILL DOWN?) update ASASA-SN SkyPatrol to v2 (don't like having to github clone it to install, still in beta)
 - sort out lightcurve times, i.e. could in theory combine mjd/hjd lightcurves currently (not properly) --> starts to get into combining lightcurves across time domain (Boris spoke about this)
 - add setting to config to change default hierarchy in 'any' survey searches (currently images/lightcurves)
@@ -139,523 +140,530 @@
 	else:
 		# get current value of parameter
 		current_value=config[parameter.upper()]
 
 		print(f'Current Value:{newline}{parameter} : {current_value}')
 		return current_value
 
-# Data Query --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+# Fetching ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
-def dataquery(survey,pos=None,source=None,radius=None):
+def query(type,survey=None,source=None,pos=None,radius=None,size=None,overlays='default',band='g',sigmaclip=None,username=None,password=None,sources=None):
 	config=readconfig()
-	
-	# if a radius isn't supplied, use default value from config
-	if radius==None:
-		radius=config['DATAQUERY_RADIUS']
-
-	# print notifications of currently running tools if enabled in the config
-	if config['ENABLE_NOTIFICATIONS']==1:
-		print(f'Running {survey} dataquery...{newline}source = {source}{newline}pos = {pos}{newline}radius = {radius}{newline}')
 
-	from .Data.data import survey_map
+	if survey==None and type not in ['sed','bulkphot','hrd']:
+		raise Exception('argument "survey" required for given query type.')
 
-	validateinput({'survey':survey,'pos':pos,'source':source,'radius':radius},'dataquery')
+	accepted_types=['data','phot','bulkphot','image','lightcurve','sed','spectra','reddening','hrd']
+	if type not in accepted_types:
+		raise Exception(f'Invalid type. Accepted types are {accepted_types}')
+
+	if type in ['data','phot','bulkphot','image','lightcurve','sed','spectra']:
+		if source!=None and pos!=None:
+			raise Exception('Simultaneous pos and source input detected in query.')
+		elif source==None and pos==None:
+			raise Exception('pos or source input required for query.')
+	elif type in ['reddening']:
+		if source==None:
+			raise Exception('Source input required for reddening query.')
+	elif type in ['hrd']:
+		if sources==None:
+			raise Exception('Sources input required for hrd query.')
+
+	if size!=None and type not in ['image']:
+		print('Note: argument "size" does not affect given query type.')
+	if overlays!='default' and type not in ['image']:
+		print('Note: argument "overlays" does not affect given query type.')
+	if band!='g' and type not in ['image']:
+		print('Note: argument "band" does not affect given query type.')
+	if sigmaclip!=None and type not in ['lightcurve']:
+		print('Note: argument "sigma_clip" does not affect given query type.')
+	if username!=None and type not in ['lightcurve']:
+		print('Note: argument "username" does not affect given query type.')
+	if password!=None and type not in ['lightcurve']:
+		print('Note: argument "password" does not affect given query type.')
+
+	if type=='data':
+		# if a radius isn't supplied, use default value from config
+		if radius==None:
+			radius=config['DATAQUERY_RADIUS']
+
+		# print notifications of currently running tools if enabled in the config
+		if config['ENABLE_NOTIFICATIONS']==1:
+			print(f'Running {survey} dataquery...{newline}source = {source}{newline}pos = {pos}{newline}radius = {radius}{newline}')
+
+		from .Data.data import survey_map
+
+		validateinput({'survey':survey,'pos':pos,'source':source,'radius':radius},'dataquery') 
+
+		data=survey_map(survey=survey,pos=pos,source=source,radius=radius)
+
+		return data
+	
+
+	elif type=='phot':
+		if radius==None:
+			radius=config['PHOTQUERY_RADIUS']
+
+		# print notifications of current running tools if enabled in the config
+		if config['ENABLE_NOTIFICATIONS']==1:
+			print(f'Running {survey} photquery...{newline}source = {source}{newline}pos = {pos}{newline}radius = {radius}{newline}')
 
-	if source!=None and pos!=None:
-		raise Exception('Simultaneous pos and source input detected in dataquery.')
-	elif source==None and pos==None:
-		raise Exception('pos or source input required in dataquery.')
+		from .Data.photometry import phot_query
+		
+		validateinput({'survey':survey,'pos':pos,'source':source,'radius':radius},'photquery')
 
-	data=survey_map(survey=survey,pos=pos,source=source,radius=radius)
+		photometry=phot_query(survey=survey,pos=pos,source=source,radius=radius)
 
-	return data
+		return photometry
+	
 
-# Phot Queries ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+	elif type=='bulkphot':
+		if radius==None:
+			radius=config['BULKPHOTQUERY_RADIUS']
 
-def photquery(survey,pos=None,source=None,radius=None):
-	config=readconfig()
-	
-	# get radius from config if one isn't given
-	if radius==None:
-		radius=config['PHOTQUERY_RADIUS']
+		# print notifications of currently running tools if enabled in the config
+		if config['ENABLE_NOTIFICATIONS']==1:
+			print(f'Running bulkphotquery...{newline}source = {source}{newline}pos = {pos}{newline}radius = {radius}{newline}')
 
-	# print notifications of current running tools if enabled in the config
-	if config['ENABLE_NOTIFICATIONS']==1:
-		print(f'Running {survey} photquery...{newline}source = {source}{newline}pos = {pos}{newline}radius = {radius}{newline}')
+		from .Data.photometry import bulk_query
+		
+		validateinput({'pos':pos,'source':source,'radius':radius},'bulkphot')
 
-	from .Data.photometry import phot_query
-	
-	validateinput({'survey':survey,'pos':pos,'source':source,'radius':radius},'photquery')
+		data=bulk_query(pos=pos,source=source,radius=radius)
+		
+		return data
 	
-	if source!=None and pos!=None:
-		raise Exception('Simultaneous pos and source input detected in photquery.')
-	elif source==None and pos==None:
-		raise Exception('pos or source input required in photquery.')
 
-	photometry=phot_query(survey=survey,pos=pos,source=source,radius=radius)
+	elif type=='image':
+		import numpy as np
 
-	return photometry
+		# get default size from config if one isn't supplied
+		if size==None:
+			size=config['IMAGEQUERY_SIZE']
 
-def bulkphotquery(pos=None,source=None,radius=None):
-	config=readconfig()
-	
-	# get radius from config if one isn't given
-	if radius==None:
-		radius=config['BULKPHOTQUERY_RADIUS']
+		# get default overlay list from config if one isn't given
+		if overlays=='default':
+			overlays=config['IMAGEQUERY_OVERLAYS']
+		
+		if not isinstance(size,int):
+			try:
+				size=int(size)
+			except:
+				size_type=type(size)
+				print(f'Invalid size data type. Expected int, got {size_type}.')
+
+		# print notifications of currently running tools if enabled in the config
+		if config['ENABLE_NOTIFICATIONS']==1:
+			print(f'Running {survey} imagequery...{newline}source = {source}{newline}pos = {pos}{newline}size = {size}{newline}overlays = {overlays}{newline}')
 
-	# print notifications of currently running tools if enabled in the config
-	if config['ENABLE_NOTIFICATIONS']==1:
-		print(f'Running bulkphotquery...{newline}source = {source}{newline}pos = {pos}{newline}radius = {radius}{newline}')
+		from .Data.imaging import image_correction
+		
+		validateinput({'survey':survey,'pos':pos,'source':source},'imagequery')
 
-	from .Data.photometry import bulk_query
-	
-	validateinput({'pos':pos,'source':source,'radius':radius},'bulkphot')
+		# set all overlays to enabled
+		if overlays=='all':
+			overlays='gaia,galex_nuv,galex_fuv,rosat,sdss,twomass,wise,ztf,erosita,atlas,gaia_lc,asassn,crts'
+
+		# split overlay string into a list, and check that they are all valid overlays.
+		if overlays!=None:
+			overlay_list=overlays.split(',')
+
+			for i in range(0,len(overlay_list)):
+				overlay_list[i]=overlay_list[i].lower()
+			for i in range(0,len(overlay_list)):
+				if overlay_list[i] not in ['gaia','galex_nuv','galex_fuv','rosat','ztf','wise','twomass','sdss','erosita','atlas','gaia_lc','asassn','crts']:
+					raise Exception('invalid overlay')
+		else:
+			overlay_list=[]
+		
+		# validate some inputs based on the survey. E.g. each survey has a maximum size, and skymapper/panstarrs need to have their 'band' parameters formatted differently
+		if survey=='panstarrs':
+			if size>1500:
+				raise Exception(f'Maximum supported size in {survey} is 1500 arcsec.')
+			if not re.match('^[grizy]+$', band):
+				raise Exception(f'Invalid {survey} bands. Supported bands are [g,r,i,z,y].')
+		
+		elif survey=='skymapper':
+			if size>600:
+				raise Exception(f'Maximum supported size in {survey} is 600 arcsec.')
+			if re.match('^[grizuv]+$', band):
+				pass
+			else:
+				raise Exception(f'Invalid {survey} bands. Supported bands are [g,r,i,z,u,v].')
+		
+			band=list(band)
+			temp_string=''
+			for i in range(0,len(band)):
+				temp_string+=(band[i]+',')
+			band=temp_string[:-1]
+			
+		elif survey=='dss':
+			if band!='g':
+				print('Note: DSS only supports g band imaging, input band has been ignored.')
+			if size>7200:
+				print(f'Maximum supported size in {survey} is 7200 arcsec.')
+
+		# do hierarchical query
+		if survey=='any':
+			image=image_correction(survey='panstarrs',pos=pos,source=source,size=size,band=band,overlay=overlay_list)
+			if image['data']==None:
+				image=image_correction(survey='skymapper',pos=pos,source=source,size=size,band=band,overlay=overlay_list)
+				if image['data']==None:
+					image=image_correction(survey='dss',pos=pos,source=source,size=size,band=band,overlay=overlay_list)
+					if image['data']==None:
+						print('Note: No image found in any supported imaging survey.')
+						pass
+		
+		# do single survey query
+		else:
+			image=image_correction(survey=survey,pos=pos,source=source,size=size,band=band,overlay=overlay_list)
+		
+		return image
 
-	if source!=None and pos!=None:
-		raise Exception('Simultaneous pos and source input detected in bulkphotquery.')
-	elif source==None and pos==None:
-		raise Exception('pos or source input required in bulkphotquery.')
 
-	data=bulk_query(pos=pos,source=source,radius=radius)
-	
-	return data
+	elif type=='lightcurve':
+		from .Data.lightcurve_sigma_clip import sigma_clip
 
-# Imaging -----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+		# get radius from config if not given
+		if radius==None:
+			radius=config['LIGHTCURVEQUERY_RADIUS']
+		
+		# get username from config if not given (only used in ATLAS queries)
+		if username==None:
+			username=config['ATLAS_USERNAME']
+		# get password from config if not given (only used in ATLAS queries)
+		if password==None:
+			password=config['ATLAS_PASSWORD']
+
+		# enables notifications of currently running tools if enabled in config
+		if config['ENABLE_NOTIFICATIONS']==1:
+			print(f'Running {survey} lightcurvequery...{newline}source = {source}{newline}pos = {pos}{newline}radius = {radius}{newline}')
 
-def imagequery(survey,pos=None,source=None,size=None,overlays='default',band='g'):
-	import numpy as np
+		from .Data.lightcurves import lightcurve_handling
+		
+		validateinput({'survey':survey,'pos':pos,'source':source,'radius':radius},'lightcurvequery')
 
-	config=readconfig()
+		# if any data exists in any band, returns True. Otherwise, returns False
+		def check_exists(data):
+			data_exists=False
+			for element in data:
+				if element['data']!=None:
+					data_exists=True
+			
+			return data_exists
+
+		# uses above function to perform heirarchical query if asked for
+		if survey=='any':
+			data=query(type='lightcurve',survey='ztf',pos=pos,source=source,radius=radius)
+			if check_exists(data)==False:
+				data=query(type='lightcurve',survey='crts',pos=pos,source=source,radius=radius)
+				if check_exists(data)==False:
+					data=query(type='lightcurve',survey='atlas',pos=pos,source=source,radius=radius,username=username,password=password)
+					if check_exists(data)==False:
+						data=query(type='lightcurve',survey='asassn',pos=pos,source=source,radius=radius)
+						if check_exists(data)==False:
+							data=query(type='lightcurve',survey='gaia',pos=pos,source=source,radius=radius)
 
-	# get default size from config if one isn't supplied
-	if size==None:
-		size=config['IMAGEQUERY_SIZE']
+		# otherwise	perform single survey query
+		else:
+			data=lightcurve_handling(survey=survey,pos=pos,source=source,radius=radius,username=username,password=password)
+		
+		# performs sigma clip on data to given sigma level if wanted
+		if sigmaclip!=None:
+			clipped_data=[]
+			for element in data:
+				if element['data']!=None:
+					clipped=sigma_clip(data=element,sigma=sigmaclip)
+					clipped_data.append(clipped)
+				else:
+					clipped_data.append(None)
+
+			data=clipped_data
+
+		return data
+	
+	
+	elif type=='sed':
+		# sets radius from default in config if one isn't supplied
+		if radius==None:
+			radius=config['SED_RADIUS']	
+
+		# enables notifications of currently running tools if enabled in the config
+		if config['ENABLE_NOTIFICATIONS']==1:
+			print(f'Running sedquery...{newline}source = {source}{newline}pos = {pos}{newline}radius = {radius}{newline}')	
 
-	# get default overlay list from config if one isn't given
-	if overlays=='default':
-		overlays=config['IMAGEQUERY_OVERLAYS']
-	
-	if not isinstance(size,int):
-		try:
-			size=int(size)
-		except:
-			size_type=type(size)
-			print(f'Invalid size data type. Expected int, got {size_type}.')
+		from .Data.sed import get_data
+		
+		data=get_data(pos=pos,source=source,radius=radius)
+		
+		validateinput({'source':source,'pos':pos},'sedquery')
 
-	# print notifications of currently running tools if enabled in the config
-	if config['ENABLE_NOTIFICATIONS']==1:
-		print(f'Running {survey} imagequery...{newline}source = {source}{newline}pos = {pos}{newline}size = {size}{newline}overlays = {overlays}{newline}')
+		return data
+	
 
-	from .Data.imaging import image_correction
+	elif type=='spectra':
+		# set radius to default in config if one isn't given
+		if radius==None:
+			radius=config['SPECTRUM_RADIUS']	
 
-	f_return=None
-	
-	validateinput({'survey':survey,'pos':pos,'source':source},'imagequery')
+		# enables notifications of current running tool if enabled in config
+		if config['ENABLE_NOTIFICATIONS']==1:
+			print(f'Running {survey} spectrumquery...{newline}source = {source}{newline}pos = {pos}{newline}radius = {radius}{newline}')	
 
-	if source!=None and pos!=None:
-		raise Exception('Simultaneous pos and source input detected in imagequery.')
-	elif source==None and pos==None:
-		raise Exception('pos or source input required in imagequery.')
+		from .Data.spectra import survey_map
+		
+		validateinput({'survey':survey,'pos':pos,'source':source,'radius':radius},'spectrumquery')
 
-	# set all overlays to enabled
-	if overlays=='all':
-		overlays='gaia,galex_nuv,galex_fuv,rosat,sdss,twomass,wise,ztf,erosita,atlas,gaia_lc,asassn,crts'
-
-	# split overlay string into a list, and check that they are all valid overlays.
-	if overlays!=None:
-		overlay_list=overlays.split(',')
-
-		for i in range(0,len(overlay_list)):
-			overlay_list[i]=overlay_list[i].lower()
-		for i in range(0,len(overlay_list)):
-			if overlay_list[i] not in ['gaia','galex_nuv','galex_fuv','rosat','ztf','wise','twomass','sdss','erosita','atlas','gaia_lc','asassn','crts']:
-				raise Exception('invalid overlay')
-	else:
-		overlay_list=[]
-	
-	# validate some inputs based on the survey. E.g. each survey has a maximum size, and skymapper/panstarrs need to have their 'band' parameters formatted differently
-	if survey=='panstarrs':
-		if size>1500:
-			raise Exception(f'Maximum supported size in {survey} is 1500 arcsec.')
-		if not re.match('^[grizy]+$', band):
-			raise Exception(f'Invalid {survey} bands. Supported bands are [g,r,i,z,y].')
-	
-	elif survey=='skymapper':
-		if size>600:
-			raise Exception(f'Maximum supported size in {survey} is 600 arcsec.')
-		if re.match('^[grizuv]+$', band):
-			pass
-		else:
-			raise Exception(f'Invalid {survey} bands. Supported bands are [g,r,i,z,u,v].')
-	
-		band=list(band)
-		temp_string=''
-		for i in range(0,len(band)):
-			temp_string+=(band[i]+',')
-		band=temp_string[:-1]
-		
-	elif survey=='dss':
-		if band!='g':
-			print('Note: DSS only supports g band imaging, input band has been ignored.')
-		if size>7200:
-			print(f'Maximum supported size in {survey} is 7200 arcsec.')
-
-	# do hierarchical query
-	if survey=='any':
-		image=image_correction(survey='panstarrs',pos=pos,source=source,size=size,band=band,overlay=overlay_list)
-		if image['data']==None:
-			image=image_correction(survey='skymapper',pos=pos,source=source,size=size,band=band,overlay=overlay_list)
-			if image['data']==None:
-				image=image_correction(survey='dss',pos=pos,source=source,size=size,band=band,overlay=overlay_list)
-				if image['data']==None:
-					print('Note: No image found in any supported imaging survey.')
-					pass
+		data=survey_map(survey=survey,pos=pos,source=source,radius=radius)
+		
+		return data
 	
-	# do single survey query
-	else:
-		image=image_correction(survey=survey,pos=pos,source=source,size=size,band=band,overlay=overlay_list)
+	elif type=='reddening':
+		from .Data.reddening import getreddening
 	
-	return image
-
-def plotimage(data):
-	config=readconfig()
+		if source==None:
+			raise Exception('getreddening requires source input.')
 
-	# print notifications of currently running tools if enabled in the config
-	if config['ENABLE_NOTIFICATIONS']==1:
-		print(f'Plotting image...{newline}')	
+		validateinput({'source':source,'survey':survey},'reddeningquery')
 
-	from .Plotting.imaging import plot_image
+		reddening=getreddening(source=source)
+			
+		return reddening
 	
-	# plot image
-	plot=plot_image(image_dict=data)
+	elif type=='hrd':
+		from .Plotting.HRD import get_data
 
-	# set file name
-	if plot!=None:
-		filename=name_file(data=data,data_type='ATKimage')
-		output_file(filename)
+		if source!=None and sources!=None:
+			raise Exception('Simultaneous source and sources input detected in hrd query.')
 
-		# scale plot size to values set by config
-		plot.width,plot.height=config['PLOT_SIZE'],config['PLOT_SIZE']
-	else:
-		filename=None
+		if isinstance(sources,list):
+			for source in sources:
+				validateinput({'source':source},'hrdquery')
+		else:
+			validateinput({'source':source})
 
-	plot_dict={'type':data['type'],'survey':data['survey'],'source':data['source'],'pos':data['pos'],'plot':plot,'ATKfilename':filename}
+		data=get_data(sources)
 
-	return plot_dict
+		return data
+		
 
-# HRD Plotting ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+# Plotting ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
-def plothrd(source=None,sources=None):
+def plot(data,type=None,colour='black',colours=None):
 	config=readconfig()
 
-	# prints notifications of currently running tools if enabled in the config
-	if config['ENABLE_NOTIFICATIONS']==1:
-		print(f'Plotting HRD...{newline}source = {source}{newline}sources = {sources}{newline}')
-
-	from bokeh.plotting import output_file
-
-	from .Plotting.HRD import get_plot
-	
-	validateinput({'source':source},'plothrd')
-
-	if source!=None and sources!=None:
-		raise Exception('Simultaneous source and sources input detected in plothrd.')
+	accepted_types=['image','lightcurve','sed','spectra','powspec','hrd']
 
-	# overlay a single gaia source
-	if source!=None:
-		plot=get_plot(source=source)
-	
-	# overlay multiple gaia sources
-	elif sources!=None:
-		# check data type of sources given (for single source input, this is already done through validateinput above)
-		for element in sources:
-			if not isinstance(element,int):
-				try:
-					element=int(element)
-				except:
-					data_type=type(element)
-					raise Exception(f'Incorrect source data type in sources. Expected int, got {data_type}.')
+	if colour!='black':
+		print('Note: argument "colour" only has an effect in lightcurve plotting.')
+	if colours!=None:
+		print('Note: argument "colours" only has an effect in lightcurve plotting.')
+
+	# if a type is not given, try to find the data type
+	if type==None:
+		# most data
+		if isinstance(data,dict):
+			try:
+				found_type=data['type']
+			except:
+				raise Exception(f'No type given to plot(), and could not find a "type" key in given data. Accepted types are {accepted_types}' )
+			
+		# e.g. for lightcurves
+		elif isinstance(data,list):
+			try:
+				# get type from first element. If multiple different types are found in the same list, raise an error.
+				found_type=data[0]['type']
+				for element in data:
+					if element['type']!=found_type:
+						raise Exception('Multiple data types found in given data. Only one type can be handled at a time.')
+			except:
+				raise Exception(f'No type given to plot(), and could not find a "type" key in given data. Accepted types are {accepted_types}' )
 		
-		plot=get_plot(sources=sources)
-	else:
-		raise Exception('source or sources input required in plothrd.')
-
-	if plot!=None:
-		# name file
-		filename=name_file(data={'source':source,'sources':sources},data_type='ATKhrd')
-		output_file(filename)
-
-		# set plot size from config defaults
-		plot.width,plot.height=config['PLOT_SIZE'],config['PLOT_SIZE']
-	else:
-		filename=None
-
-	if source!=None:
-		plot_dict={'source':source,'type':'hrd','plot':plot,'ATKfilename':filename}
-	elif sources!=None:
-		plot_dict={'sources':sources,'type':'hrd','plot':plot,'ATKfilename':filename}
-
-	return plot_dict
-
-# Light Curves ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-def lightcurvequery(survey,pos=None,source=None,radius=None,username=None,password=None,sigmaclip=None):
-	from .Data.lightcurve_sigma_clip import sigma_clip
+		type=found_type
 
-	config=readconfig()
+	# if a type is given, it doesn't matter so much if a type is not found in the data, but still check and raise a warning if given type doesn't match the found type.
+	elif type!=None:
+		found_type=None	
+		if isinstance(data,dict):
+			try:
+				found_type=data['type']
+			except:
+				pass
+		elif isinstance(data,list):
+			try:
+				found_type=data[0]['type']
+				for element in data:
+					if element['type']!=found_type:
+						raise Exception('Multiple data types found in given data. Only one type can be handled at a time.')
+			except:
+				pass
+
+		if found_type!=None:
+			if type!=found_type:
+				print('Note: type found within given data does not match type passed by user.')
 
-	# get radius from config if not given
-	if radius==None:
-		radius=config['LIGHTCURVEQUERY_RADIUS']
-	
-	# get username from config if not given (only used in ATLAS queries)
-	if username==None:
-		username=config['ATLAS_USERNAME']
-	# get password from config if not given (only used in ATLAS queries)
-	if password==None:
-		password=config['ATLAS_PASSWORD']
 
-	# enables notifications of currently running tools if enabled in config
 	if config['ENABLE_NOTIFICATIONS']==1:
-		print(f'Running {survey} lightcurvequery...{newline}source = {source}{newline}pos = {pos}{newline}radius = {radius}{newline}')
+		print(f'Plotting {type}...{newline}')
+	
+
+	if type=='image':
+		from .Plotting.imaging import plot_image
+	
+		# plot image
+		plot=plot_image(image_dict=data)
+
+		# set file name
+		if plot!=None:
+			filename=name_file(data=data,data_type='ATKimage')
+			output_file(filename)
 
-	from .Data.lightcurves import lightcurve_handling
-	
-	validateinput({'survey':survey,'pos':pos,'source':source,'radius':radius},'lightcurvequery')
+			# scale plot size to values set by config
+			plot.width,plot.height=config['PLOT_SIZE'],config['PLOT_SIZE']
+		else:
+			filename=None
 
-	if source!=None and pos!=None:
-		raise Exception('Simultaneous pos and source input detected in lightcurvequery')
-	elif source==None and pos==None:
-		raise Exception('pos or source input required in lightcurvequery.')
+		plot_dict={'type':data['type'],'survey':data['survey'],'source':data['source'],'pos':data['pos'],'plot':plot,'ATKfilename':filename}
 
-	# if any data exists in any band, returns True. Otherwise, returns False
-	def check_exists(data):
-		data_exists=False
-		for element in data:
-			if element['data']!=None:
-				data_exists=True
-		
-		return data_exists
-
-	# uses above function to perform heirarchical query if asked for
-	if survey=='any':
-		data=lightcurvequery(survey='ztf',pos=pos,source=source,radius=radius)
-		if check_exists(data)==False:
-			data=lightcurvequery(survey='crts',pos=pos,source=source,radius=radius)
-			if check_exists(data)==False:
-				data=lightcurvequery(survey='atlas',pos=pos,source=source,radius=radius,username=username,password=password)
-				if check_exists(data)==False:
-					data=lightcurvequery(survey='asassn',pos=pos,source=source,radius=radius)
-					if check_exists(data)==False:
-						data=lightcurvequery(survey='gaia',pos=pos,source=source,radius=radius)
+		return plot_dict
+	
 
-	# otherwise	perform single survey query
-	else:
-		data=lightcurve_handling(survey=survey,pos=pos,source=source,radius=radius,username=username,password=password)
+	elif type=='lightcurve':
+		from .Plotting.lightcurves import plot_lightcurve
 	
-	# performs sigma clip on data to given sigma level if wanted
-	if sigmaclip!=None:
-		clipped_data=[]
-		for element in data:
-			if element['data']!=None:
-				clipped=sigma_clip(data=element,sigma=sigmaclip)
-				clipped_data.append(clipped)
-			else:
-				clipped_data.append(None)
+		if colour not in ['green','red','blue','purple','orange','black']:
+			raise Exception('Unsupported colour in plotlightcurve.')
 
-		data=clipped_data
+		plot=plot_lightcurve(data=data,colour=colour,colours=colours)
 
-	return data
+		if plot!=None:
+			# names file
+			filename=name_file(data=data,data_type='ATKlightcurve')
+			output_file(filename)
+		
+			# sets plot size according to config defaults
+			plot.width,plot.height=config['PLOT_SIZE']*2,config['PLOT_SIZE']
+		else:
+			filename=None
+		
+		plot_dict={'type':'lightcurve'}
 
-def plotlightcurve(data,colour='black',colours=None):
-	config=readconfig()
+		if isinstance(data,list):
+			for i,val in enumerate(data):
+				if val!=None:
+					plot_dict['survey']=val['survey']
+					plot_dict['source']=val['source']
+					plot_dict['pos']=val['pos']
+		elif isinstance(data,dict):
+			plot_dict['survey']=data['survey']
+			plot_dict['source']=data['source']
+			plot_dict['pos']=data['pos']
+		else:
+			raise Exception('Expected ATK lightcurve dict or list of ATK lightcurve dicts')
 
-	# enables notifications of currently running tools if enabled in config
-	if config['ENABLE_NOTIFICATIONS']==1:
-		print(f'Plotting lightcurve...{newline}')	
+		plot_dict['plot']=plot
+		plot_dict['ATKfilename']=filename
 
-	from .Plotting.lightcurves import plot_lightcurve
+		return plot_dict
 	
-	if colour not in ['green','red','blue','purple','orange','black']:
-		raise Exception('Unsupported colour in plotlightcurve.')
-
-	plot=plot_lightcurve(data=data,colour=colour,colours=colours)
-
-	if plot!=None:
-		# names file
-		filename=name_file(data=data,data_type='ATKlightcurve')
-		output_file(filename)
 	
-		# sets plot size according to config defaults
-		plot.width,plot.height=config['PLOT_SIZE']*2,config['PLOT_SIZE']
-	else:
-		filename=None
+	elif type=='sed':
+		from .Plotting.sed import plot_sed
 	
-	plot_dict={'type':'lightcurve'}
-
-	if isinstance(data,list):
-		for i,val in enumerate(data):
-			if val!=None:
-				plot_dict['survey']=val['survey']
-				plot_dict['source']=val['source']
-				plot_dict['pos']=val['pos']
-	elif isinstance(data,dict):
-		plot_dict['survey']=data['survey']
-		plot_dict['source']=data['source']
-		plot_dict['pos']=data['pos']
-	else:
-		raise Exception('Expected ATK lightcurve dict or list of ATK lightcurve dicts')
-
-	plot_dict['plot']=plot
-	plot_dict['ATKfilename']=filename
+		plot=plot_sed(sed_data=data)
 
-	return plot_dict
-
-# SEDs --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-def sedquery(pos=None,source=None,radius=None):
-	config=readconfig()
+		if plot!=None:
+			# names file
+			filename=name_file(data=data,data_type='ATKsed')
+			output_file(filename)
+		
+			# scales plot according to defaults in the config
+			plot.width,plot.height=config['PLOT_SIZE']*2,config['PLOT_SIZE']
+		else:
+			filename=None
 
-	# sets radius from default in config if one isn't supplied
-	if radius==None:
-		radius=config['SED_RADIUS']	
+		plot_dict={'type':data['type'],'source':data['source'],'pos':data['pos'],'plot':plot,'ATKfilename':filename}
 
-	# enables notifications of currently running tools if enabled in the config
-	if config['ENABLE_NOTIFICATIONS']==1:
-		print(f'Running sedquery...{newline}source = {source}{newline}pos = {pos}{newline}radius = {radius}{newline}')	
+		return plot_dict
 
-	from .Data.sed import get_data
 	
-	data=get_data(pos=pos,source=source,radius=radius)
+	elif type=='spectra':
+		from .Plotting.spectra import get_plot
 	
-	validateinput({'source':source,'pos':pos},'sedquery')
-
-	if source!=None and pos!=None:
-		raise Exception('Simultaneous pos and source input detected in dataquery.')
-	elif source==None and pos==None:
-		raise Exception('pos or source input required in dataquery.')
+		plot=get_plot(spectrum_dict=data)
 
-	return data
+		if plot!=None:
+			# names file
+			filename=name_file(data=data,data_type='ATKspectrum')
+			output_file(filename)
 
-def plotsed(data):
-	config=readconfig()
+			# sets plot sizes to defaults from config
+			plot.width,plot.height=config['PLOT_SIZE']*2,config['PLOT_SIZE']
+		else:
+			filename=None
 
-	# enables notifications of currently running tools if enabled in the config
-	if config['ENABLE_NOTIFICATIONS']==1:
-		print(f'Plotting SED...{newline}')	
+		plot_dict={'type':'spectra','survey':data['survey'],'source':data['source'],'pos':data['pos'],'plot':plot,'ATKfilename':filename}
 
-	from .Plotting.sed import plot_sed
+		return plot_dict
 	
-	plot=plot_sed(sed_data=data)
 
-	if plot!=None:
-		# names file
-		filename=name_file(data=data,data_type='ATKsed')
-		output_file(filename)
+	elif type=='powspec':
+		import copy
+		
+		from .Plotting.powspec import get_plot
 	
-		# scales plot according to defaults in the config
-		plot.width,plot.height=config['PLOT_SIZE']*2,config['PLOT_SIZE']
-	else:
-		filename=None
-
-	plot_dict={'type':data['type'],'source':data['source'],'pos':data['pos'],'plot':plot,'ATKfilename':filename}
-
-	return plot_dict
-
-# Spectra -----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-def spectrumquery(survey=None,pos=None,source=None,radius=None):
-	config=readconfig()
+		# stops data from being flattened by the powspec plotting
+		data_copy=copy.deepcopy(data)
 
-	# set radius to default in config if one isn't given
-	if radius==None:
-		radius=config['SPECTRUM_RADIUS']	
+		plot=get_plot(dataset=data_copy)
 
-	# enables notifications of current running tool if enabled in config
-	if config['ENABLE_NOTIFICATIONS']==1:
-		print(f'Running {survey} spectrumquery...{newline}source = {source}{newline}pos = {pos}{newline}radius = {radius}{newline}')	
+		if plot!=None:
+			# name file
+			filename=name_file(data=data,data_type='ATKpowspec')
+			output_file(filename)
+		
+			# set size of file according to defaults in config
+			plot.width,plot.height=config['PLOT_SIZE']*2,config['PLOT_SIZE']
+		else:
+			filename=None
 
-	from .Data.spectra import survey_map
-	
-	validateinput({'survey':survey,'pos':pos,'source':source,'radius':radius},'spectrumquery')
+		plot_dict={'type':'powspec'}
+		for i,val in enumerate(data):
+			if val!=None:
+				plot_dict['survey']=val['survey']
+				plot_dict['source']=val['source']
+				plot_dict['pos']=val['pos']
 
-	if source!=None and pos!=None:
-		raise Exception('Simultaneous pos and source input detected in spectrumquery.')
-	elif source==None and pos==None:
-		raise Exception('pos or source input required in spectrumquery.')
+		plot_dict['plot']=plot
+		plot_dict['ATKfilename']=filename
 
-	data=survey_map(survey=survey,pos=pos,source=source,radius=radius)
+		return plot_dict
 	
-	return data
-
-def plotspectrum(data):
-	config=readconfig()
 
-	# enables notifications of the currently running tool if enabled in config
-	if config['ENABLE_NOTIFICATIONS']==1:
-		print(f'Plotting spectrum...{newline}')	
-
-	from .Plotting.spectra import get_plot
-	
-	plot=get_plot(spectrum_dict=data)
+	elif type=='hrd':
+		from .Plotting.HRD import get_plot
 
-	if plot!=None:
-		# names file
-		filename=name_file(data=data,data_type='ATKspectrum')
-		output_file(filename)
+		plot=get_plot(data)
 
-		# sets plot sizes to defaults from config
-		plot.width,plot.height=config['PLOT_SIZE']*2,config['PLOT_SIZE']
-	else:
-		filename=None
+		if plot!=None:
+			# name file
+			filename=name_file(data={'sources':data['sources']},data_type='ATKhrd')
+			output_file(filename)
 
-	plot_dict={'type':'spectra','survey':data['survey'],'source':data['source'],'pos':data['pos'],'plot':plot,'ATKfilename':filename}
+			# set plot size from config defaults
+			plot.width,plot.height=config['PLOT_SIZE'],config['PLOT_SIZE']
+		else:
+			filename=None
 
-	return plot_dict
+		plot_dict={'sources':data['sources'],'type':'hrd','plot':plot,'ATKfilename':filename}
+		
+		return plot_dict
 
 # Timeseries --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
-def plotpowspec(data):
-	import copy
-
-	config=readconfig()
-
-	# enables notifications of currently running tool if enabled in config
-	if config['ENABLE_NOTIFICATIONS']==1:
-		print(f'Plotting power spectrum...{newline}')	
-
-	from .Plotting.powspec import get_plot
-	
-	# stops data from being flattened by the powspec plotting
-	data_copy=copy.deepcopy(data)
-
-	plot=get_plot(dataset=data_copy)
-
-	if plot!=None:
-		# name file
-		filename=name_file(data=data,data_type='ATKpowspec')
-		output_file(filename)
-	
-		# set size of file according to defaults in config
-		plot.width,plot.height=config['PLOT_SIZE']*2,config['PLOT_SIZE']
-	else:
-		filename=None
-
-	plot_dict={'type':'powspec'}
-	for i,val in enumerate(data):
-		if val!=None:
-			plot_dict['survey']=val['survey']
-			plot_dict['source']=val['source']
-			plot_dict['pos']=val['pos']
-
-	plot_dict['plot']=plot
-	plot_dict['ATKfilename']=filename
-
-	return plot_dict
-
 def tsanalysis(data):
 	config=readconfig()
 
 	# enables notifications of currently running tool if enabled in config
 	if config['ENABLE_NOTIFICATIONS']==1:
 		print(f'Running time series analysis...{newline}')	
 
@@ -702,15 +710,15 @@
 	from .Datapages.buttons import getinfobuttons	
 
 	validateinput({'source':source,'pos':pos},'databuttons')
 
 	if source!=None and pos!=None:
 		raise Exception('Simultaneous pos and source input detected in getbuttons.')
 	elif source==None and pos==None:
-		raise Exception('pos or source input detected in getbuttons.')
+		raise Exception('pos or source input required in getbuttons.')
 
 	# validates data type of some parameters. Since these are only used here, didn't add to validateinput
 	if not (isinstance(simbad_radius,int) or isinstance(simbad_radius,float)):
 		data_type=type(simbad_radius)
 		raise Exception(f'Incorrect simbad_radius data type. Expected float/int, got {data_type}.')
 	if not (isinstance(vizier_radius,int) or isinstance(vizier_radius,float)):
 		data_type=type(vizier_radius)
@@ -742,28 +750,14 @@
 	
 	plot=gettable(metadata_dict=metadata,pos=pos,source=source)
 	
 	plot_dict={'type':'metadata','source':source,'pos':pos,'plot':plot}
 
 	return plot_dict
 
-# Reddening query ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-def getreddening(source=None):
-	from .Data.reddening import getreddening
-	
-	if source==None:
-		raise Exception('getreddening requires source input.')
-
-	validateinput({'source':source})
-
-	reddening=getreddening(source=source)
-	
-	return reddening
-
 # File Handling -----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def savedata(data):
 	config=readconfig()
 
 	# enables notifications for currently running tool if enabled in config
 	if config['ENABLE_NOTIFICATIONS']==1:
@@ -848,14 +842,41 @@
 		except:
 			raise Exception('Unexpected plot type, expected ATK dict or bokeh plot object.')
 
 	return None
 
 # Miscellaneous -----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
+def webquery(type,pos=None,source=None,radius=None):
+	from .Misc.database_queries import query
+
+	config=readconfig()
+
+	if type.lower() not in ['simbad','vizier']:
+		raise Exception(f"Invalid webquery type '{type}'. Valid types: ['simbad','vizier']")
+
+	# gets default radius to use in SIMBAD query if one isn't given
+	if radius==None and type=='simbad':
+		radius=config['SIMBAD_RADIUS']
+	# gets default radius to use in Vizier query if one isn't given
+	elif radius==None and type=='vizier':
+		radius=config['VIZIER_RADIUS']
+
+	if config['ENABLE_NOTIFICATIONS']==1:
+		print(f'Performing {type} query...{newline}source = {source}{newline}pos = {pos}{newline} radius = {radius}{newline}')
+
+	validateinput({'source':source,'pos':pos},'webquery')
+
+	if source!=None and pos!=None:
+		raise Exception('Simultaneous pos and source input detected in webquery.')
+	elif source==None and pos==None:
+		raise Exception('pos or source input required in webquery.')
+	
+	query(type=type,source=source,pos=pos,radius=radius)
+
 def correctpm(inputtime,targettime,ra,dec,pmra,pmdec):
 	from .Misc.ProperMotionCorrection import PMCorrection
 	
 	pos=PMCorrection(input=inputtime,target=targettime,ra=ra,dec=dec,pmra=pmra,pmdec=pmdec)
 
 	return pos
```

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit.egg-info/PKG-INFO` & `AstroToolkit-1.4.0/src/AstroToolkit.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AstroToolkit
-Version: 1.3.5
+Version: 1.4.0
 Summary: A package for the gathering and plotting of astronomical data.
 Author-email: Ethan Moorfield <ethan.moorfield@hotmail.co.uk>
 Project-URL: Homepage, https://github.com/WD-planets/AstroToolkit
 Project-URL: Issues, https://github.com/WD-planets/AstroToolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -25,65 +25,31 @@
 Requires-Dist: Requests==2.31.0
 Requires-Dist: scikit_learn==1.3.2
 Requires-Dist: scipy==1.10.1
 Requires-Dist: selenium==4.17.2
 
 # AstroToolkit
 
-AstroToolkit (ATK) is a set of useful tools for fetching, plotting, and analysing astronomical data.
+AstroToolkit (ATK) is a set of tools for fetching, plotting, and analysing astronomical data.
 
 ## Table of Contents
 
 1. [Installation](#installation)
 2. [Introduction](#introduction)
 3. [Configuration](#configuration)
 4. [Tools](#tools)
+5. [Examples](#examples)
 
 ### ATK Tools
 
-- 1 [Raw Data Tools](#1-raw-data-tools)
-	- 1.1 [dataquery](#11-dataquery)
-	- 1.2 [photquery](#12-photquery)
-	- 1.3 [bulkphotquery](#13-bulkphotquery)
-	- 1.4 [getreddening](#14-getreddening)
-- 2 [Imaging Tools](#2-imaging-tools)
-	- 2.1 [imagequery](#21-imagequery)
-	- 2.2 [plotimage](#22-plotimage)
-- 3 [HRD Tools](#3-hrd-tools)
-	- 3.1 [plothrd](#31-plothrd)
-- 4 [Lightcurve Tools](#4-lightcurve-tools)
-	- 4.1 [lightcurvequery](#41-lightcurvequery)
-	- 4.2 [plotlightcurve](#42-plotlightcurve)
-- 5 [SED Tools](#5-sed-tools)
-	- 5.1 [sedquery](#51-sedquery)
-	- 5.2 [plotsed](#52-plotsed)
-- 6 [Spectrum Tools](#6-spectrum-tools)
-	- 6.1 [spectrumquery](#61-spectrumquery)
-	- 6.2 [plotspectrum](#62-plotspectrum)
-- 7 [Timeseries Tools](#7-timeseries-tools)
-	- 7.1 [plotpowspec](#71-plotpowspec)
-	- 7.2 [tsanalysis](#72-tsanalysis)
-- 8 [Datapage Tools](#8-datapage-tools)
-	- 8.1 [gridsetup](#81-gridsetup)
-	- 8.2 [getbuttons](#82-getbuttons)
-	- 8.3 [getmdtable](#83-getmdtable)
-- 9 [File Handling Tools](#9-file-handling-tools)
-	- 9.1 [savedata](#91-savedata)
-	- 9.2 [readdata](#92-readdata)
-	- 9.3 [export](#93-export)
-- 10 [Miscellaneous Tools](#10-miscellaneous-tools)
-	- 10.1 [showplot](#101-showplot)
-	- 10.2 [saveplot](#102-saveplot)
-	- 10.3 [correctpm](#103-correctpm)
-	- 10.4 [getdistance](#104-getdistance)
-	- 10.5 [convfromdeg](#105-convfromdeg)
-	- 10.6 [convtodeg](#106-convtodeg)
-	- 10.7 [getcolumn](#107-getcolumn)
-	- 10.8 [getsources](#108-getsources)
-	- 10.9 [getpositions](#109-getpositions)
+- 1 [Query](#1-query)
+- 2 [Plot](#2-plot)
+- 3 [Datapage Tools](#3-datapage-tools)
+- 4 [File Handling Tools](#4-file-handling-tools)
+- 5 [Other Tools](#5-other-tools)
 
 <br>
 
 ## Installation<a id="installation"></a>
 
 The package can be installed as with any other package, e.g. using pip:
 ```
@@ -138,33 +104,33 @@
 editconfig(options)
 ```
 
 where options is a dictionary containing key : value pairs to set in the config. The list of accepted keys and their default values are shown below:
 - enable_notifications = False
 	- If True, notifications denoting basic information as each ATK tool is executed will be shown in the terminal. Can be useful for tracking the flow of data.
 - dataquery_radius = 3
-	- This sets the default radius (in arcseconds) to use in the [dataquery](#11-dataquery) tool.
+	- This sets the default radius (in arcseconds) to use in [data queries](#11-data-query).
 - photquery_radius = 3
-	- This sets the default radius (in arcseconds) to use in the [photquery](#12-photquery) tool.
+	- This sets the default radius (in arcseconds) to use in [photometry queries](#12-photometry-query).
 - bulkphotquery_radius = 3
-	- This sets the default radius (in arcseconds) to use in the [bulkphotquery](#13-bulkphotquery) tool.
+	- This sets the default radius (in arcseconds) to use in [bulk photometry queries](#13-bulk-photometry-query).
 - imagequery_size = 30
-	- This sets the default radius (in arcseconds) to use in the [imagequery](#21-imagequery) tool.
+	- This sets the default radius (in arcseconds) to use in [image queries](#15-imaging-query).
 - imagequery_overlays = gaia
-	- This sets the default radius (in arcseconds) to use in the [imagequery](#21-imagequery) tool.
+	- This sets the default radius (in arcseconds) to use in [image queries](#15-imaging-query).
 - lightcurvequery_radius = 3
-	- This sets the default radius (in arcseconds) to use in the [lightcurvequery](#31-lightcurvequery) tool.
+	- This sets the default radius (in arcseconds) to use in [lightcurve queries](#16-lightcurve-query).
 - atlas_username = None
-	- This sets the default username to use for ATLAS lightcurve queries in the [lightcurvequery](#31-lightcurvequery) tool.
+	- This sets the default username to use in ATLAS [lightcurve queries](#16-lightcurve-query).
 - atlas_password = None
-	- This sets the default password to use for ATLAS lightcurve queries in the [lightcurvequery](#31-lightcurvequery) tool.
+	- This sets the default password to use in ATLAS [lightcurve queries](#16-lightcurve-query).
 - sed_radius = 3
-	- This sets the default radius to use in the [sedquery](#41-sedquery) tool.
+	- This sets the default radius to use in [SED queries](#17-sed-query).
 - spectrum_radius = 3
-	- This sets the default radius to use in the [spectrumquery](#51-spectrumquery) tool.
+	- This sets the default radius to use in [spectrum queries](#18-spectrum-query).
 - grid_size = 250
 	- This sets the default grid size to use in the [gridsetup](#71-gridsetup) tool.
 - button_simbad_radius = 3
 	- This sets the default radius to use for the SIMBAD button in the [getbuttons](#72-getbuttons) tool.
 - button_vizier_radius = 3
 	- This sets the default radius to use for the Vizier button in the [getbuttons](#72-getbuttons) tool.
 - plot_size = 400
@@ -198,168 +164,153 @@
 parameter = string, name of config parameter from above list
 ```
 
 **Returns**: value of this parameter in the config.
 
 <br><br>
 
-## Tools
+## Tools<a id="tools"></a>
 
 In this section, the available tools will be outlined. Note that if a parameter is listed as having a default parameter CONFIG, this means that this parameter is taken from the config as listed above. These parameters can still be passed to the tool, in which case the config value will be ignored.
 
 **Note:** most data returned from fetching/plotting tools takes the form of a dictionary. This dictionary contains the returned data, as well as basic information such as the pos/source used to acquire the data. This format is then used by other ATK functions (such as file showing/saving/reading).
 
 **Note:** All plots created by ATK can have their legends toggled by double clicking the plot, and individual data can be hidden by clicking them in the legend.
 
 <br>
 
 **In all data returned by querying tools, the value of the 'data' key will be set to None if no data was returned. Likewise, in all plotting tools, the value of the 'plot' key will be set to None.**
 
 <br>
 
-### 1. Raw Data Tools<a id="1-raw-data-tools"></a>
-### 1.1. dataquery<a id="11-dataquery"></a>
+## 1. query<a id="1-query"></a>
 
-Returns all available data for a given survey (e.g. magnitudes, positions, etc.).
-
-<br>
-
-**Supported surveys:** gaia, galex, rosat, panstarrs, skymapper, sdss, twomass, wise, erosita
-
-<br>
+Returns available data of a given type from a given survey.
 
 **Usage:**
 
 ```
-dataquery(survey,pos=None,source=None,radius=CONFIG)
+query(type,survey=None,pos=None,source=None,radius=CONFIG)
 ```
 
 where:
 
 ```
+type = str, type of data to return
+```
+```
 survey = str, name of a supported survey
 ```
 ```
 pos = list, [ra,dec]
 ```
 ```
 source = int/str, Gaia source_id
 ```
 ```
-radius = int/float, radius of query
+radius = int/float, radius of query of given type. If not given, will be taken from config value for given query type.
 ```
 
-**Returns:** dict
+<br>
 
-```
-{
-'survey' : str, survey of data
-'type' : 'data'
-'source' : int/str, source used to get data (None if a pos was used)
-'pos' : [ra,dec], pos used to get data (None if a source was used)
-'data' : dict, the returned data
-}
-```
+**Note:** If no data is returned, the 'data' key of the returned dictionary will be set to None.
 
 <br>
 
-**Example:**
+**Supported query types:** data, phot, bulkphot, image, lightcurve, sed, spectra, reddening
+
+<br>
 
-To retrieve the parallax of a system through Gaia, and its WISE data:
+Below is an outline of the usage and output of each query type. Note that additonal arguments not listed above may be used, see individual query types below for details.
 
-```
-from AstroToolkit.Tools import dataquery
+<br>
 
-source = 6050296829033196032
+**Shortcuts**:
 
-parallax = dataquery(survey='gaia',source=source)['data']['parallax']
-wise_data = dataquery(survey='wise',source=source)['data']
-```
+[Data Queries](#11-data-query)
 
-<br><br>
+[Photometry Queries](#12-photometry-query)
 
-### 1.2. photquery<a id="12-photquery"></a>
+[Bulk Photomety Queries](#13-bulk-photometry-query)
 
-Returns data from a given survey, with columns filtered to only include photometry and other basic information.
+[Reddening Queries](#14-reddening-query)
 
-<br>
+[Imaging Queries](#15-imaging-query)
+
+[Lightcurve Queries](#16-lightcurve-query)
+
+[SED Queries](#17-sed-query)
+
+[Spectrum Queries](#18-spectrum-query)
 
-**Supported surveys:** gaia,panstarrs,skymapper,galex,rosat,sdss,wise,twomass
+[HRD Queries](#19-hrd-query)
 
 <br>
 
-**Usage:**
+### 1.1 Data Query<a id="11-data-query"></a>
 
-```
-photquery(survey,pos=None,source=None,radius=CONFIG)
-```
+Type argument: 'data'
 
-where:
+Description: Returns all available raw data for a given survey
 
-```
-survey = str, name of a supported survey
-```
-```
-pos = list, [ra,dec]
-```
-```
-source = int/str, Gaia source_id
-```
-```
-radius = int/float, radius of query
-```
+Supported Arguments: survey, pos, source, radius (all defined [above](#1-query))
+
+Supported Surveys: gaia, galex, rosat, panstarrs, skymapper, sdss, twomass, wise, erosita
+
+<br>
 
 **Returns:** dict
 
 ```
 {
 'survey' : str, survey of data
 'type' : 'data'
 'source' : int/str, source used to get data (None if a pos was used)
 'pos' : [ra,dec], pos used to get data (None if a source was used)
 'data' : dict, the returned data
 }
 ```
 
-<br>
-
-**Example:**
+<br><br>
 
-To retrieve the 2MASS photometry for an object:
-```
-from AstroToolkit.Tools import photquery
+### 1.2 Photometry Query<a id="12-photometry-query"></a>
 
-data=photquery(survey='twomass',source=6050296829033196032)['data']
-```
+Type argument: 'phot'
 
-<br>
+Description: Returns all photometry available from a given survey, as well as some basic parameters such as coordinates.
 
-### 1.3. bulkphotquery<a id="13-bulkphotquery"></a>
+Supported Arguments: survey, pos, source, radius (all defined [above](#1-query))
 
-Returns available photometry from all surveys supported by [photquery](#12-photquery).
+Supported Surveys: gaia, panstarrs, skymapper, galex, rosat, sdss, wise, twomass
 
 <br>
 
-**Usage:**
+**Returns:** dict
 
 ```
-bulkphotquery(pos=None,source=None,radius=CONFIG)
+{
+'survey' : str, survey of data
+'type' : 'data'
+'source' : int/str, source used to get data (None if a pos was used)
+'pos' : [ra,dec], pos used to get data (None if a source was used)
+'data' : dict, the returned data
+}
 ```
 
-where:
+<br><br>
 
-```
-pos = list, [ra,dec]
-```
-```
-source = int/str, Gaia source_id
-```
-```
-radius = int/float, radius of query
-```
+### 1.3 Bulk Photometry Query<a id="13-bulk-photometry-query"></a>
+
+Type argument: 'bulkphot'
+
+Description: Returns all photometry available from all surveys supported by [photometry queries](#12-photometry-query)
+
+Supported Arguments: pos, source, radius (all defined [above](#1-query))
+
+<br>
 
 **Returns:** dict
 
 ```
 {
 'type' : 'bulkphot'
 'source' : int/str, source used to get data (None if a pos was used)
@@ -371,50 +322,25 @@
           etc. for each survey in surveys supported by photquery
          }
 }
 ```
 
 **Note:** The value of each survey will be set to None if no data was returned. E.g. if no galex data was returned, the value of the ['galex'] key would be None.
 
-<br>
-
-**Example:**
-
-To retrieve the gaia and galex data for an object:
-
-```
-from AstroToolkit.Tools import bulkphotquery
-
-bulk_phot=bulkphotquery(source=6050296829033196032)['data']
-
-gaia_data=bulk_phot['gaia']
-galex_data=bulk_phot['galex']
-```
-
-<br>
-
-### 1.4. getreddening<a id="14-getreddening"></a>
-
-Returns the reddening of a Gaia source.
+<br><br>
 
-Currently supported reddening surveys:
-- STILISM (https://stilism.obspm.fr/)
+### 1.4. Reddening Query<a id="14-reddening-query"></a>
 
-<br>
+Type argument: 'reddening'
 
-**Usage:**
+Description: Returns the reddening for a given Gaia source from a given survey
 
-```
-getreddening(source)
-```
+Supported Arguments: source (defined [above](#1-query))
 
-where:
-```
-source = int/str, Gaia source_id
-```
+Supported Surveys: stilism (https://stilism.obspm.fr/)
 
 <br>
 
 **Returns:** dict
 
 ```
 {
@@ -429,79 +355,56 @@
          'red_lower' : reddening lower limit
          }
 }
 ```
 
 <br><br>
 
-### 2. Imaging Tools<a id="2-imaging-tools"></a>
-
-These functions retrieve and plotimages from supported surveys.
-
-**Note:** When using a 'pos' as input, some detections can be missing for high proper motion objects. When instead using a source as input, this is no longer a problem as the detection search radius is increased to account for this proper motion.
+### 1.5 Imaging Query<a id="15-imaging-query"></a>
 
-<br>
-
-### 2.1. imagequery<a id="21-imagequery"></a>
+Type argument: 'image'
 
-Retrieves an image from a given survey. Overlays  can be used to overlay detections from different surveys. There are two types of overlay: detections and tracers. Detections are proper motion-corrected circles that scale with the magnitude of the detection, and show that there is data available for a given object in a given survey. 
+Description: Returns an image from a given survey. Overlays  can be used to overlay detections from different surveys. There are two types of overlay: detections and tracers. Detections are proper motion-corrected circles that scale with the magnitude of the detection, and show that there is data available for a given object in a given survey. 
 
 Tracers (which are detections created from lightcurve surveys) can be used both to show that lightcurve data is available, but also to trace an object through time.
 
 **Note:** tracing an object through time works best with ZTF and CRTS overlays, as these give data with the necessary coordinate precision. Other tracer overlays are unlikely to work for this, and will hence only be useful to see where lightcurve data is available.
 
 **Note:** In the case of ATLAS overlays, the radius used is very small due to the time taken to perform ATLAS queries. Only data close to the focus of the image (i.e. at the location of the target object) will be shown. 
 
 **Example:**
 
 ![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/tracer_example.png?raw=true)
 
-<br>
-
-Supported surveys:
-- panstarrs, supported bands = g, r, i, z, y
-- skymapper, supported bands = g, r, i, z, u, v
-- dss, supported bands = g
-
-**Note:** Can also use 'any' to perform an image query according to the hierarchy: panstarrs > skymapper > dss
-
-<br>
-
-Supported overlays: gaia, galex_nuv, galex_fuv, rosat,sdss, twomass, wise, ztf, erosita ,atlas, gaia_lc, asassn, crts
-
-**Note:** Can also use 'all', which will enable overlays for all supported surveys.
-
-<br>
-
-**Usage:**
-
-```
-imagequery(survey,pos=None,source=None,size=CONFIG,band='g',overlays=CONFIG)
-```
+Supported Arguments: survey, pos, source, size, band, overlays
 
 where:
 ```
-survey = str, name of a supported survey
-```
-```
-pos = list, [ra,dec]
-```
-```
-source = int/str, Gaia source_id
-```
-```
 size = int/float, size of image in arcsec
 ```
 ```
 band = str, string containing the required bands (e.g. for all panstarrs bands, use band='grizy')
 ```
 ```
 overlays = str, required detection overlays (e.g. for gaia and wise detections, use overlays='gaia,wise') 
 ```
 
+and all other arguments have been defined [above](#1-query).
+
+Supported overlays: gaia, galex_nuv, galex_fuv, rosat,sdss, twomass, wise, ztf, erosita ,atlas, gaia_lc, asassn, crts
+
+**Note:** Can also use 'all', which will enable overlays for all supported surveys.
+
+Supported Surveys:
+- panstarrs, supported bands = g, r, i, z, y
+- skymapper, supported bands = g, r, i, z, u, v
+- dss, supported bands = g
+
+<br>
+
 **Returns:** dict
 
 ```
 {
 'type' : 'image'
 'survey' : str, image survey
 'source' : int/str, source used to get image (None if a pos was used)
@@ -527,159 +430,47 @@
 'radius' : float, radius of detection
 'corrected' : bool, whether or not the detection has been corrected for proper motion
 'mag' : str, name of the magnitude (column heaader) from a given survey
 'marker' : 'circle' or 'cross', detection symbol to overlay. Circles are scaled with radius, crosses are not (e.g. for surveys without a magnitude to scale by)
 }
 ```
 
-<br>
-
-### 2.2. plotimage<a id="22-plotimage"></a>
-
-Plots images in format returned by [imagequery](#21-imagequery).
-
-<br>
-
-**Usage:**
-
-```
-plotimage(data)
-```
-
-where:
-```
-data = dict in format returned by imagequery
-```
-
-**Returns:** dict
-
-```
-{
-'type' : 'image'
-'survey' : str, survey of image
-'source' : int/str, source used to get image (None if a pos was used)
-'pos' : [ra,dec], pos used to get image (None if a source was used)
-'plot' : bokeh figure object, the actual plot
-'ATKfilename' : the default filename given by ATK
-}
-```
-
-**Note:** if a plot is not returned (e.g. if no data was supplied to the plotting tool), the 'plot' key will be set to None.
-
-<br>
-
-**Example:**
-
-To retrieve and plot an image:
-```
-from AstroToolkit.Tools import imagequery,plotimage,showplot
-
-image=imagequery(survey='any',source=6050296829033196032,overlays='gaia')
-plot=plotimage(image)
-showplot(plot)
-```
-
-![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/imaging_example.png?raw=true)
-
 <br><br>
 
-### 3. HRD Tools<a id="3-hrd-tools"></a>
-### 3.1. plothrd<a id="31-plothrd"></a>
+### 1.6 Lightcurve Query<a id="16-lightcurve-query"></a>
 
-Returns a HRD with a source or list of sources overlayed over a Gaia 100pc background sample.
+Type argument: 'lightcurve'
 
-<br>
+Description: Returns lightcurve data from a given survey.
 
-**Usage:**
-
-```
-plothrd(source=None,sources=None)
-```
+Supported Arguments: survey, pos, source, radius, username, password, sigmaclip
 
 where:
-
-```
-source = int/str, Gaia source_id
-```
 ```
-sources = list of sources
+username = str, ATLAS username, hence only used in ATLAS queries
 ```
-
-**Returns:** dict
-
 ```
-{
-'type' : 'hrd'
-'source' : int/str, source overlayed in HRD
-'sources' : list, sources overlayed in HRD if multiple were given
-'plot' : bokeh figure object, the actual plot
-'ATKfilename' : the default filename given by ATK
-}
+password = str, ATLAS password, hence only used in ATLAS queries
 ```
-
-<br>
-
-**Example:**
-To retrieve a HRD with a single source overlayed:
 ```
-from AstroToolkit.Tools import plothrd,showplot
-
-plot=plothrd(source=6050296829033196032)
-showplot(plot)
+sigmaclip = int, performs sigma clipping on the data to this number of standard deviations
 ```
+and all other arguments have been defined [above](#1-query).
 
-![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/hrd_example.png?raw=true)
-
-<br><br>
-
-### 4. Lightcurve Tools<a id="4-lightcurve-tools"></a>
-### 4.1. lightcurvequery<a id="41-lightcurvequery"></a>
-
-Returns lightcurve data for a given survey.
-
-<br>
-
-Supported surveys:
+Supported Surveys (and filter bands):
 - ZTF (ztf) - g, r, i
 - ATLAS (atlas) - o, c, i
 - ASAS-SN (asassn) - g, v
 - Gaia (gaia) - g, bp, rp
 - CRTS (crts) - v
 
 **Note:** CRTS' data server is not designed for scripted queries. As a result, queries are limited in the toolkit to one query per 15 seconds. This cooldown is managed using the CRTS_TIMER.txt file in the Settings directory of the package files, and hence this should not be edited.
 
 <br>
 
-```
-lightcurvequery(survey,pos=None,source=None,radius=CONFIG,username=CONFIG,password=CONFIG,sigmaclip=None)
-```
-
-where:
-```
-survey = str, name of a supported survey
-```
-```
-pos = list, [ra,dec]
-```
-```
-source = int/str, Gaia source_id
-```
-```
-radius = int/float, radius of lightcurve query
-```
-```
-username = str, ATLAS username, hence only used in ATLAS queries
-```
-```
-password = str, ATLAS password, hence only used in ATLAS queries
-```
-```
-sigmaclip = int, performs sigma clipping on the data to this number of standard deviations
-```
-
 **Returns:** list of dicts
 
 list of lightcurve data dictionaries with an entry for each band in that survey (see below). Each entry has the format:
 
 ```
 {
 'type' : 'lightcurve'
@@ -696,340 +487,339 @@
          'hjd_ori'/'mjd_ori' : list of returned hjd/mjd values, unedited
          'mag' : list of returned magnitude values
          'mag_err' : list of returned magnitude error values
          }
 }
 ```
 
-<br>
-
-### 4.2. plotlightcurve<a id="42-plotlightcurve"></a>
+<br><br>
 
-Plots lightcurves in the format returned by [lightcurvequery](#41-lightcurvequery).
+### 1.7 SED Query<a id="17-sed-query"></a>
 
-<br>
+Type argument: 'sed'
 
-**Usage:**
+Description: Queries all supported [photometry surveys](#12-photometry-query) and returns SED data.
 
-```
-plotlightcurve(data,colour='black')
-```
+Supported Arguments: pos, source, radius (all defined [above](#1-query))
 
-where:
-```
-data = dict if passing a single lightcurve, list of dicts if passing multiple lightcurves
-```
-```
-colour = str, name of a supported colour. Only used when passing a single lightcurve
-```
-```
-colours = list of strings denoting supported colours, e.g. ['green','red','blue']. Only used when passing multiple lightcurves
-```
+<br>
 
 **Returns:** dict
 
 ```
 {
-'type' : 'lightcurve'
-'survey' : str, survey of lightcurve
+'type' : 'sed'
 'source' : int/str, source used to get data (None if a pos was used)
 'pos': [ra,dec], pos used to get data (None if a source was used)
-'plot' : bokeh figure object, the actual plot
-'ATKfilename' : the default filename given by ATK
+'data': list of entries with each entry taking the form of a dict:
+	{
+    'survey' : str, survey of data point
+    'wavelength' : filter wavelength of data point
+    'flux' : flux through filter
+    'rel_err' : relative error on flux
+    }
 }
 ```
 
-<br>
-
-**Example**:
-To retrieve and plot lightcurves from ZTF:
-```
-from AstroToolkit.Tools import lightcurvequery,plotlightcurve,showplot
-
-lightcurves=lightcurvequery(survey='ztf',source=6050296829033196032)
-showplot(plotlightcurve(lightcurves,colours=['green','red','blue']))
-```
+<br><br>
 
-![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/lightcurve_example.png?raw=true)
+### 1.8 Spectrum Query<a id="18-spectrum-query"></a>
 
-**Note:** Each band will then be toggleable using the legend.
+Type argument: 'spectra'
 
-<br><br>
+Description: Returns spectrum data for a given survey.
 
-### 5. SED Tools<a id="5-sed-tools"></a>
-### 5.1. sedquery<a id="51-sedquery"></a>
+Supported Arguments: survey, pos, source, radius (all defined [above](#1-query))
 
-Queries all supported photometry surveys and returns SED data.
+Supported Surveys: sdss
 
 <br>
 
-**Usage:**
+**Returns:**
 
 ```
-sedquery(pos=None,source=None,radius=CONFIG)
+{
+'type' : 'spectra'
+'survey' : str, survey of detection
+'source' : int/str, source used to get data (None if a pos was used)
+'pos': [ra,dec], pos used to get data (None if a source was used)
+'data': {
+        'wavelength' : list of wavelength values
+        'flux' : list of flux values
+        }
+}
 ```
 
+<br><br>
+
+### 1.9 HRD Query<a id="19-hrd-query"></a>
+
+Type argument: 'hrd'
+
+Description: Returns data for Gaia HRD creation given a Gaia source/list of Gaia sources.
+
+Supported Arguments: sources
+
 where:
 ```
-pos = list, [ra,dec]
-```
-```
-source = int/str, Gaia source_id
-```
-```
-radius = int/float, radius of data query
+sources = single Gaia source or list of Gaia sources
 ```
 
+<br>
+
 **Returns:** dict
 
 ```
-{
-'type' : 'sed'
-'source' : int/str, source used to get data (None if a pos was used)
-'pos': [ra,dec], pos used to get data (None if a source was used)
-'data': list of entries with each entry taking the form of a dict:
-	{
-    'survey' : str, survey of data point
-    'wavelength' : filter wavelength of data point
-    'flux' : flux through filter
-    'rel_err' : relative error on flux
-    }
-}
+'type' : 'hrd'
+'sources' : list, list of input Gaia sources
+'data': {
+        'absg' : list, absolute g magnitudes of given sources
+        'bp-rp' : list, bp-rp values of given sources
+        }
 ```
 
-<br>
+<br><br>
 
-### 5.2. plotsed<a id="52-plotsed"></a>
+## 2. plot<a id="2-plot"></a>
 
-Plots SEDs in the format returned by [sedquery](#51-sedquery).
-
-<br>
+Interprets and plots data.
 
 **Usage:**
 
 ```
-plotsed(data)
+plot(data,type=None)
 ```
 
 where:
-
 ```
-data = dict in format returned by sedquery
+data = list/dict data in structure returned by the query tool
 ```
 
-**Returns:** dict
+<br>
 
-```
-{
-'type' : 'sed'
-'source' : int/str, source used to get data (None if a pos was used)
-'pos': [ra,dec], pos used to get data (None if a source was used)
-'plot' : bokeh figure object, the actual plot
-'ATKfilename' : the default filename given by ATK
-}
-```
+**Note:** If no plot is returned, the 'plot' key of the returned dictionary will be set to None.
 
 <br>
 
-**Example:** To retrieve and plot an SED:
-```
-from AstroToolkit.Tools import sedquery,plotsed,showplot
+**Supported plot types:** image, lightcurve, sed, spectra, powspec, hrd
 
-data=sedquery(source=6050296829033196032)
-showplot(plotsed(data))
-```
+<br>
 
-![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/sed_example.png?raw=true)
+Below is an outline of the usage and output of each plot type. Note that additonal arguments not listed above may be used, see individual plot types below for details.
 
-<br><br>
+<br>
+
+**Shortcuts**:
+
+[Image Plotting](#21-image-plotting)
+
+[Lightcurve Plotting](#22-lightcurve-plotting)
 
-### 6. Spectrum Tools<a id="6-spectrum-tools"></a>
-### 6.1. spectrumquery<a id="61-spectrumquery"></a>
+[SED Plotting](#23-sed-plotting)
 
-Returns spectrum data from a given survey.
+[Spectrum Plotting](#24-spectrum-plotting)
+
+[HRD Plotting](#25-hrd-plotting)
+
+[Power Spectra Plotting](#26-power-spectra-plotting)
 
 <br>
 
-**Usage:**
+### 2.1 Image Plotting<a id="21-image-plotting"></a>
+
+Type argument: 'image'
+
+Description: Plots images in format returned by [image queries](#15-imaging-query).
+
+<br>
+
+**Returns:** dict
 
 ```
-spectrumquery(survey=None,pos=None,source=None,radius=CONFIG)
+{
+'type' : 'image'
+'survey' : str, survey of image
+'source' : int/str, source used to get image (None if a pos was used)
+'pos' : [ra,dec], pos used to get image (None if a source was used)
+'plot' : bokeh figure object, the actual plot
+'ATKfilename' : the default filename given by ATK
+}
 ```
 
+<br><br>
+
+### 2.2 Lightcurve Plotting<a id="22-lightcurve-plotting"></a>
+
+Type argument: 'lightcurve'
+
+Description: Plots lightcurves in the format returned by [lightcurve queries](#16-lightcurve-query). Here, you can either pass a single lightcurve, or multiple lightcurves (e.g. those returned from [lightcurve queries](#16-lightcurve-query)).
+
+Additional Supported Arguments: colour, colours
+
 where:
 ```
-survey = str, name of a supported survey
-```
-```
-pos = list, [ra,dec]
-```
-```
-source = int/str, Gaia source_id
+colour = str, name of a supported colour. Only used when passing a single lightcurve
 ```
 ```
-radius = int/float, radius of data query
+colours = list of strings denoting supported colours, e.g. ['green','red','blue']. Only used when passing multiple lightcurves
 ```
 
-**Returns:** dict
+**Note:** CRTS' data server is not designed for scripted queries. As a result, queries are limited in the toolkit to one query per 15 seconds. This cooldown is managed using the CRTS_TIMER.txt file in the Settings directory of the package files, and hence the contents of this file should not be edited.
+
+<br>
 
+**Returns:** dict
 ```
 {
-'type' : 'spectra'
-'survey' : str, survey of detection
+'type' : 'lightcurve'
+'survey' : str, survey of lightcurve
 'source' : int/str, source used to get data (None if a pos was used)
 'pos': [ra,dec], pos used to get data (None if a source was used)
-'data': {
-        'wavelength' : list of wavelength values
-        'flux' : list of flux values
-        }
+'plot' : bokeh figure object, the actual plot
+'ATKfilename' : the default filename given by ATK
 }
 ```
 
-<br>
+<br><br>
 
-### 6.2. plotspectrum<a id="62-plotspectrum"></a>
+### 2.3 SED Plotting<a id="23-sed-plotting"></a>
 
-Plots spectra in the format returned by [spectrumquery](#61-spectrumquery).
+Type argument: 'sed'
 
-<br>
+Description: Plots SED data in the format returned by [SED queries](#17-sed-query).
 
-**Usage:**
+<br>
 
+**Returns:** dict
 ```
-plotspectrum(data)
+{
+'type' : 'sed'
+'source' : int/str, source used to get data (None if a pos was used)
+'pos': [ra,dec], pos used to get data (None if a source was used)
+'data': list of entries with each entry taking the form of a dict:
+	{
+    'survey' : str, survey of data point
+    'wavelength' : filter wavelength of data point
+    'flux' : flux through filter
+    'rel_err' : relative error on flux
+    }
+}
 ```
 
-where:
+<br><br>
 
-```
-data = dict in format returned by spectrumquery
-```
+### 2.4 Spectrum Plotting<a id="24-spectrum-plotting"></a>
 
-**Returns:** dict
+Type argument: 'spectra'
+
+Description: Plots spectrum data in the format returned by [spectrum queries](#18-spectrum-query).
 
+<br>
+
+**Returns:** dict
 ```
 {
 'type' : 'spectrum'
 'survey' : str, survey of spectrum
 'source' : int/str, source used to get data (None if a pos was used)
 'pos': [ra,dec], pos used to get data (None if a source was used)
 'plot' : bokeh figure object, the actual plot
 'ATKfilename' : the default filename given by ATK
 }
 ```
 
-<br>
+<br><br>
 
-**Example:**
-To retrieve and plot an SDSS spectrum:
-```
-from AstroToolkit.Tools import spectrumquery,plotspectrum,showplot
+### 2.5 HRD Plotting<a id="25-hrd-plotting"></a>
 
-data=spectrumquery(survey='sdss',source=587316166180416640)
-plot=plotspectrum(data)
-showplot(plot)
-```
+Type argument: 'hrd'
 
-![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/spectrum_example.png?raw=true)
+Description: Plots Gaia HRD data in the format returned by [hrd queries](#19-hrd-query).
 
-<br><br>
+<br>
 
-### 7. Timeseries Tools<a id="7-timeseries-tools"></a>
-### 7.1 plotpowspec<a id="71-plotpowspec"></a>
+**Returns:** dict
+```
+{
+'type' : 'hrd'
+'source' : int/str, source overlayed in HRD
+'sources' : list, sources overlayed in HRD if multiple were given
+'plot' : bokeh figure object, the actual plot
+'ATKfilename' : the default filename given by ATK
+}
+```
 
-Plots a power spectrum from lightcurve data in the format returned by [lightcurvequery](#41-lightcurvequery)
+<br><br>
 
-<br>
+### 2.6 Power Spectra Plotting<a id="26-power-spectra-plotting"></a>
 
-**Usage:**
+Type argument: 'powspec'
 
-```
-plotpowspec(data)
-```
+Description: Plots power spectra from lightcurve data in the format returned by [lightcurve queries](#16-lightcurve-query).
 
-where:
-```
-data = dict or list in format returned by lightcurvequery
-```
+<br>
 
 **Returns:** dict
 
 ```
 {
 'type' : 'powspec'
 'survey' : str, survey of lightcurve data given to the powspec tool
 'source' : int/str, source used to get data (None if a pos was used)
 'pos': [ra,dec], pos used to get data (None if a source was used)
 'plot' : bokeh figure object, the actual plot
 'ATKfilename' : the default filename given by ATK
 }
 ```
 
-<br>
-
-**Example:**
-To retrieve lightcurve data from ZTF and plot a power spectrum:
-```
-from AstroToolkit.Tools import lightcurvequery,plotpowspec,showplot
-
-data=lightcurvequery(survey='ztf',source=6050296829033196032)
-plot=plotpowspec(data)
-showplot(plot)
-```
-
-![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/powspec_example.png?raw=true)
-
 <br><br>
 
-### 7.2 tsanalysis<a id="72-tsanalysis"></a>
+### 2.7 Timeseries Analysis<a id="27-timeseries-analysis"></a>
 
-Runs period analysis on lightcurve data in format returned by [lightcurvequery](#lightcurvequery)
+Description: Not explicitly a plotting function, but included here for completeness. Runs period analysis on lightcurve data in format returned by [lightcurve queries](#16-lightcurve-query).
 
 <br>
 
 **Usage:**
 
 ```
 tsanalysis(data)
 ```
 
 where:
 
 ```
-data = dict or list in format returned by lightcurvequery
-```
-
-<br>
-
-**Example:**
-To retrieve lightcurve data from ZTF and perform timeseries analysis:
-```
-from AstroToolkit.Tools import lightcurvequery,tsanalysis
-
-data=lightcurvequery(survey='ztf',source=6050296829033196032)
-plot=tsanalysis(data)
+data = dict or list in format returned by lightcurve queries
 ```
 
-![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/tsanalysis_example.png?raw=true)
-
 <br><br>
 
-## 8. Datapage Tools<a id="8-datapage-tools"></a>
+## 3. Datapage Tools<a id="3-datapage-tools"></a>
 
 These functions are used to create custom datapages from any plots/data supported by AstroToolkit.
 
 **NOTE:** An example of datapage creation can be found within the packages 'Examples' folder, named 'datapage_creation.py' (within the …/Lib/site-packages/AstroToolkit from earlier). This can be imported from a python terminal using from AstroToolkit.Examples import datapage_creation.
 
 Below is the datapage produced by this example. Once the script to create these has been written, they can be a very powerful way to quickly retrieve and show a wide range of information on a system, with the below example easily being generated in under 30s.
 
 ![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/datapage_example.png?raw=true)
 
 <br>
 
-### 8.1. gridsetup<a id="81-gridsetup"></a>
+Shortcuts:
+
+[Grid Creation](#31-gridsetup)
+
+[SIMBAD/Vizier Buttons](#32-getbuttons)
+
+[Metadata Table Creation](#33-getmdtable)
+
+<br><br>
+
+### 3.1 gridsetup<a id="31-gridsetup"></a>
 
 Formats plots for datapage creation by sizing them to a grid of given dimensions.
 
 <br>
 
 **Usage:**
 
@@ -1067,15 +857,15 @@
 
 where the keys "name ..." are the names given to the plots above, and the values 'plot ...' are the plots to which these names refer.
 
 **NOTE:** Again, see the datapage_creation example as noted [above](#8-datapage-tools) for an example.
 
 <br>
 
-### 8.2. getbuttons<a id="82-getbuttons"></a>
+### 3.2 getbuttons<a id="32-getbuttons"></a>
 
 Returns a Bokeh figure containing SIMBAD and Vizier buttons for use in datapages.
 
 <br>
 
 **Usage:**
 
@@ -1111,15 +901,15 @@
 }
 ```
 
 **NOTE:** Again, see the datapage_creation example as noted [above](#8-datapage-tools) for an example.
 
 <br>
 
-### 8.3. getmdtable<a id="83-getmdtable"></a>
+### 3.3 getmdtable<a id="33-getmdtable"></a>
 
 Creates a table of metadata table using data from supported surveys and/or custom data.
 
 <br>
 
 **Usage:**
 
@@ -1185,20 +975,31 @@
 }
 ```
 
 **NOTE:** Again, see the datapage_creation example as noted [above](#8-datapage-tools) for an example.
 
 <br><br>
 
-## 9. File Handling Tools<a id="9-file-handling-tools"></a>
+## 4. File Handling Tools<a id="4-file-handling-tools"></a>
+
 These tools can be used to transform many returned ATK data structures into local files, and vice versa. This process is designed to be completely lossless, allowing for the exact data structure that was used to create a file to be recreated at a later date.
 
 <br>
 
-### 9.1. savedata<a id="91-savedata"></a>
+Shortcuts:
+
+[Data Saving](#41-savedata)
+
+[Data Reading](#42-readdata)
+
+[Export Plots to PNG](#43-export)
+
+<br><br>
+
+### 4.1 savedata<a id="41-savedata"></a>
 
 This tool allows for the saving of many ATK data structures into local files.
 
 Supported ATK data types: data, phot, bulkphot, image, sed, spectra, lightcurve
 
 <br>
 
@@ -1220,15 +1021,15 @@
 
 <br>
 
 **Note:** Created files will contain a tag (e.g. ATKimage for an image). This is necessary, as it tells the readdata function (see below) how to interpret the file to recreate the original data structure.
 
 <br>
 
-### 9.2. readdata<a id="92-readdata"></a>
+### 4.2 readdata<a id="42-readdata"></a>
 
 This tool allows for the lossless recreation of ATK data stuctures from files created using [savedata](#91-savedata).
 
 <br>
 
 **Usage:**
 
@@ -1263,15 +1064,15 @@
 
 ![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/struct_recreation_example.png?raw=true)
 
 **Note:** The above example assumes that you have already set a default ATLAS username / password in the [config](#configuration).
 
 <br>
 
-### 9.3. export<a id="93-export"></a>
+### 4.3 export<a id="43-export"></a>
 
 This allows for ATK figures to be saved as a .png file.
 
 <br>
 
 **Usage:**
 
@@ -1285,59 +1086,79 @@
 ```
 ```
 keephtml = bool. To get the filename for the png, the plot must first be saved as a regular bokeh static html file. This tells ATk whether to delete this file or keep it.
 ```
 
 <br><br>
 
-### 10. Miscellaneous Tools<a id="10-miscellaneous-tools"></a>
+## 5. Other Tools<a id="5-other-tools"></a>
 
-These are tools that do not fit into the above categories, but can still be useful for quickly performing some basic functions.
+Below is a list of the other tools available in ATK.
 
-<br>
+Shortcuts:
+
+[Show Plots](531-showplot)
 
-### 10.1. showplot<a id="101-showplot"></a>
+[Save Plots](532-saveplot)
 
-This allows for the plot dictionaries returned by ATK to be opened in the browser. Doing so will also save the plot locally as a .html file. Can also be used with the same functionality as show() from bokeh for non-ATK bokeh figures.
+[Proper Motion Correction](533-correctpm)
+
+[Parallax to Distance](534-getdistance)
+
+[Convert Degrees to HMS/DMS](535-convfromdeg)
+
+[Convert from HMS/DMS to Degrees](536-convtodeg)
+
+[Read fits file columns](#57-getcolumn)
+
+[Read Sources from a fits file](#58-getsources)
+
+[Read Positions from a fits file](#59-getpositions)
+
+[Open object in SIMBAD/Vizier](#510-webquery)
+
+### 5.1 showplot<a id="51-showplot"></a>
+
+Description: This allows for the plot dictionaries returned by ATK to be opened in the browser. Doing so will also save the plot locally as a .html file. Can also be used with the same functionality as show() from bokeh for non-ATK bokeh figures.
 
 <br>
 
 **Usage:**
 ```
 showplot(plot)
 ```
 
 where:
 ```
-plot = ATK plot dictionary
+plot = ATK plot dictionary or bokeh figure
 ```
 
-<br>
+<br><br>
 
-### 10.2. saveplot<a id="102-saveplot"></a>
+### 5.2 saveplot<a id="52-saveplot"></a>
 
-This allows for the plot dictionaries returned by ATK to be saved to local .html files without opening them in the browser. Can also be used with the same functionality as save() from bokeh for non-ATK bokeh figures.
+Description: This allows for the plot dictionaries returned by ATK to be saved to local .html files without opening them in the browser. Can also be used with the same functionality as save() from bokeh for non-ATK bokeh figures.
 
 <br>
 
 **Usage:**
 ```
 saveplot(plot)
 ```
 
 where:
 ```
-plot = ATK plot dictionary
+plot = ATK plot dictionary or bokeh figure
 ```
 
-<br>
+<br><br>
 
-### 10.3. correctpm<a id="103-correctpm"></a>
+### 5.3 correctpm<a id="53-correctpm"></a>
 
-Corrects for proper motion of an object between an input time and a target time.
+Description: Corrects for proper motion of an object between an input time and a target time.
 
 <br>
 
 **Usage:**
 
 ```
 correctpm(inputtime,targettime,ra,dec,pmra,pmdec)
@@ -1366,30 +1187,17 @@
 
 <br>
 
 **Returns:** list
 
 [ra,dec] of object in degrees, corrected for proper motion.
 
-<br>
-
-**Example:**
-To correct an object for proper motion to the year 2000:
-```
-from AstroToolkit.Tools import dataquery,correctpm
-
-gaia_data=dataquery(survey='gaia',source=6050296829033196032)['data']
-ra,dec,pmra,pmdec=gaia_data['ra'][0],gaia_data['dec'][0],gaia_data['pmra'][0],gaia_data['pmdec'][0]
-
-ra_corrected,dec_corrected=correctpm([2016,0],[2000,0],ra,dec,pmra,pmdec)
-```
-
-<br>
+<br><br>
 
-### 10.4. getdistance<a id="104-getdistance"></a>
+### 5.4 getdistance<a id="54-getdistance"></a>
 
 Simply calculates the distance (1/parallax) of an object given its parallax in mas (the unit of parallax in Gaia).
 
 <br>
 
 **Usage:**
 
@@ -1406,15 +1214,15 @@
 
 **Returns:** float
 
 distance of object in pc
 
 <br>
 
-### 10.5. convfromdeg<a id="105-convfromdeg"></a>
+### 5.5 convfromdeg<a id="55-convfromdeg"></a>
 
 Converts deg coordinates to HMS/DMS format
 
 <br>
 
 **Usage:**
 
@@ -1431,15 +1239,15 @@
 
 **Returns:** list
 
 [ra,dec] of object in [HMS,DMS]
 
 <br>
 
-### 10.6. convtodeg<a id="106-convtodeg"></a>
+### 5.6 convtodeg<a id="56-convtodeg"></a>
 
 Converts HMS/DMS coordinates to deg.
 
 <br>
 
 **Usage:**
 
@@ -1456,15 +1264,15 @@
 
 **Returns:** list
 
 [ra,dec] of object in deg
 
 <br>
 
-### 10.7. getcolumn<a id="107-getcolumn"></a>
+### 5.7 getcolumn<a id="57-getcolumn"></a>
 
 Returns a list of values from a .fits file given a column name.
 
 **Usage:**
 
 ```
 getcolumn(file_name,col_name)
@@ -1480,15 +1288,15 @@
 
 **Returns:** list
 
 list of values for that column
 
 <br>
 
-### 10.8. getsources<a id="108-getsources"></a>
+### 5.8 getsources<a id="58-getsources"></a>
 
 Returns a list of source values from a .fits file given a column name, which can either be set in the tool or in the config.
 
 **Usage:**
 
 ```
 getsources(file_name,col_name=CONFIG)
@@ -1504,15 +1312,15 @@
 
 **Returns:** list
 
 list of Gaia sources
 
 <br>
 
-### 10.9. getpositions<a id="109-getpositions"></a>
+### 5.9 getpositions<a id="59-getpositions"></a>
 
 Returns a list of ra,dec values from a .fits file given ra and dec column names, which can either be set in the tool or in the config.
 
 **Usage:**
 
 ```
 getsources(file_name,col_name=CONFIG)
@@ -1525,7 +1333,177 @@
 ```
 col_name = str, comma separated string containing names of ra and dec columns. e.g. col_name = 'RA_ICRS,'DE_ICRS'. Must be in this order.
 ```
 
 **Returns:** list
 
 list of positions [[ra1,dec1],[ra2,dec2]], etc.
+
+### 5.10 webquery<a id="510-webquery"></a>
+
+Performs SIMBAD/Vizier queries given a source/pos in the web browser.
+
+**Usage:**
+
+```
+webquery(type,source=None,pos=None,radius=CONFIG)
+```
+
+where:
+```
+type = str, type of query from 'simbad' or 'vizier'
+```
+```
+pos = list, [ra,dec]
+```
+```
+source = int/str, Gaia source_id
+```
+```
+radius = int/float, radius of data query. If not given, this is taken from simbad_radius or vizier_radius in the config, depending on the query type
+```
+
+**Returns:** None
+
+<br><br>
+
+## Examples<a id="examples"></a>
+
+### Example 1: Fetching and plotting an image
+
+```
+from AstroToolkit.Tools import query,plot,showplot
+
+image=query(type='image',survey='any',source=6050296829033196032,overlays='gaia')
+figure=plot(image)
+showplot(figure)
+```
+
+![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/imaging_example.png?raw=true)
+
+<br><br>
+
+### Example 2: Fetching and plotting a Gaia HRD
+
+```
+from AstroToolkit.Tools import query,plot,showplot
+
+data=query(type='hrd',sources=[6050296829033196032])
+figure=plot(data)
+showplot(figure)
+```
+
+![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/hrd_example.png?raw=true)
+
+<br><br>
+
+### Example 3: Fetching and plotting a ZTF lightcurve
+
+```
+from AstroToolkit.Tools import query,plot,showplot
+
+data=lightcurvequery(type='lightcurve',survey='ztf',source=6050296829033196032)
+showplot(plot(data,colours=['green','red','blue']))
+```
+
+**Note:** Each band will then be toggleable using the legend.
+
+![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/lightcurve_example.png?raw=true)
+
+<br><br>
+
+### Example 4: Fetching and plotting an SED
+
+```
+from AstroToolkit.Tools import query,plot,showplot
+
+data=query(type='sed',source=6050296829033196032)
+showplot(plot(data))
+```
+
+![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/sed_example.png?raw=true)
+
+<br><br>
+
+### Example 5: Fetching and plotting an SDSS spectrum
+
+```
+from AstroToolkit.Tools import query,plot,showplot
+
+data=query(type='spectra',survey='sdss',source=587316166180416640)
+plot=plot(data)
+showplot(plot)
+```
+
+![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/spectrum_example.png?raw=true)
+
+<br><br>
+
+### Example 6: Fetching ZTF ligthcurve data, and then plotting it as a power spectrum
+
+```
+from AstroToolkit.Tools import lightcurvequery,plotpowspec,showplot
+
+data=lightcurvequery(survey='ztf',source=6050296829033196032)
+plot=plotpowspec(data)
+showplot(plot)
+```
+
+![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/powspec_example.png?raw=true)
+
+<br><br>
+
+### Example 7: Fetching Gaia parallax and WISE data
+
+```
+from AstroToolkit.Tools import query
+
+source = 6050296829033196032
+
+parallax = query(type='data',survey='gaia',source=source)['data']['parallax']
+wise_data = query(type='data',survey='wise',source=source)['data']
+```
+
+### Example 8: Fetching 2MASS photometry for an object
+
+```
+from AstroToolkit.Tools import query
+
+data=query(type='phot',survey='twomass',source=6050296829033196032)['data']
+```
+
+### Example 9: Fetching photometry from all available surveys using a bulk photometry query
+
+```
+from AstroToolkit.Tools import query
+
+bulk_phot=query(type='bulkphot',source=6050296829033196032)['data']
+
+gaia_data=bulk_phot['gaia']
+galex_data=bulk_phot['galex']
+```
+
+<br><br>
+
+### Example 10: Fetching ZTF lightcurve data, and performing timeseries analysis
+
+```
+from AstroToolkit.Tools import query,tsanalysis
+
+data=query(type='lightcurve',survey='ztf',source=6050296829033196032)
+plot=tsanalysis(data)
+```
+
+![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/tsanalysis_example.png?raw=true)
+
+<br><br>
+
+### Example 11: Proper motion correction
+
+```
+from AstroToolkit.Tools import query,correctpm
+
+gaia_data=query(type='data',survey='gaia',source=6050296829033196032)['data']
+ra,dec,pmra,pmdec=gaia_data['ra'][0],gaia_data['dec'][0],gaia_data['pmra'][0],gaia_data['pmdec'][0]
+
+ra_corrected,dec_corrected=correctpm([2016,0],[2000,0],ra,dec,pmra,pmdec)
+```
```

### Comparing `AstroToolkit-1.3.5/src/AstroToolkit.egg-info/SOURCES.txt` & `AstroToolkit-1.4.0/src/AstroToolkit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 src/AstroToolkit/Data/spectra.py
 src/AstroToolkit/Datapages/buttons.py
 src/AstroToolkit/Datapages/grid.py
 src/AstroToolkit/Datapages/metadata.py
 src/AstroToolkit/Examples/datapage_creation.py
 src/AstroToolkit/Misc/ProperMotionCorrection.py
 src/AstroToolkit/Misc/coord_conversion.py
+src/AstroToolkit/Misc/database_queries.py
 src/AstroToolkit/Misc/file_handling.py
 src/AstroToolkit/Misc/file_naming.py
 src/AstroToolkit/Misc/input_validation.py
 src/AstroToolkit/Misc/read_fits.py
 src/AstroToolkit/Plotting/HRD.py
 src/AstroToolkit/Plotting/backdrop_hrd_allmags.fits
 src/AstroToolkit/Plotting/imaging.py
```

