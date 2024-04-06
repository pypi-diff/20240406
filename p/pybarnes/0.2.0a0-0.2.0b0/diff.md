# Comparing `tmp/pybarnes-0.2.0a0.tar.gz` & `tmp/pybarnes-0.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybarnes-0.2.0a0.tar", last modified: Tue Aug  8 15:33:50 2023, max compression
+gzip compressed data, was "pybarnes-0.2.0b0.tar", last modified: Fri Aug 18 10:53:09 2023, max compression
```

## Comparing `pybarnes-0.2.0a0.tar` & `pybarnes-0.2.0b0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 ouyang    (1000) ouyang    (1000)        0 2023-08-08 15:33:50.353946 pybarnes-0.2.0a0/
--rw-r--r--   0 ouyang    (1000) ouyang    (1000)       73 2023-08-08 15:33:50.353946 pybarnes-0.2.0a0/PKG-INFO
-drwxr-xr-x   0 ouyang    (1000) ouyang    (1000)        0 2023-08-08 15:33:50.350612 pybarnes-0.2.0a0/pybarnes/
--rw-r--r--   0 ouyang    (1000) ouyang    (1000)       91 2023-08-08 15:31:54.000000 pybarnes-0.2.0a0/pybarnes/__init__.py
--rw-r--r--   0 ouyang    (1000) ouyang    (1000)    12031 2023-08-08 15:27:36.000000 pybarnes-0.2.0a0/pybarnes/barnes_filter.py
-drwxr-xr-x   0 ouyang    (1000) ouyang    (1000)        0 2023-08-08 15:33:50.353946 pybarnes-0.2.0a0/pybarnes.egg-info/
--rw-r--r--   0 ouyang    (1000) ouyang    (1000)       73 2023-08-08 15:33:50.000000 pybarnes-0.2.0a0/pybarnes.egg-info/PKG-INFO
--rw-r--r--   0 ouyang    (1000) ouyang    (1000)      214 2023-08-08 15:33:50.000000 pybarnes-0.2.0a0/pybarnes.egg-info/SOURCES.txt
--rw-r--r--   0 ouyang    (1000) ouyang    (1000)        1 2023-08-08 15:33:50.000000 pybarnes-0.2.0a0/pybarnes.egg-info/dependency_links.txt
--rw-r--r--   0 ouyang    (1000) ouyang    (1000)        6 2023-08-08 15:33:50.000000 pybarnes-0.2.0a0/pybarnes.egg-info/requires.txt
--rw-r--r--   0 ouyang    (1000) ouyang    (1000)        9 2023-08-08 15:33:50.000000 pybarnes-0.2.0a0/pybarnes.egg-info/top_level.txt
--rw-r--r--   0 ouyang    (1000) ouyang    (1000)       38 2023-08-08 15:33:50.353946 pybarnes-0.2.0a0/setup.cfg
--rwxr-xr-x   0 ouyang    (1000) ouyang    (1000)      192 2023-08-08 15:30:04.000000 pybarnes-0.2.0a0/setup.py
+drwxr-xr-x   0 ouyang    (1000) ouyang    (1000)        0 2023-08-18 10:53:09.622463 pybarnes-0.2.0b0/
+-rw-r--r--   0 ouyang    (1000) ouyang    (1000)       73 2023-08-18 10:53:09.622463 pybarnes-0.2.0b0/PKG-INFO
+drwxr-xr-x   0 ouyang    (1000) ouyang    (1000)        0 2023-08-18 10:53:09.619129 pybarnes-0.2.0b0/pybarnes/
+-rw-r--r--   0 ouyang    (1000) ouyang    (1000)       90 2023-08-18 10:40:57.000000 pybarnes-0.2.0b0/pybarnes/__init__.py
+-rw-r--r--   0 ouyang    (1000) ouyang    (1000)    12308 2023-08-18 10:52:55.000000 pybarnes-0.2.0b0/pybarnes/barnes_filter.py
+drwxr-xr-x   0 ouyang    (1000) ouyang    (1000)        0 2023-08-18 10:53:09.622463 pybarnes-0.2.0b0/pybarnes.egg-info/
+-rw-r--r--   0 ouyang    (1000) ouyang    (1000)       73 2023-08-18 10:53:09.000000 pybarnes-0.2.0b0/pybarnes.egg-info/PKG-INFO
+-rw-r--r--   0 ouyang    (1000) ouyang    (1000)      214 2023-08-18 10:53:09.000000 pybarnes-0.2.0b0/pybarnes.egg-info/SOURCES.txt
+-rw-r--r--   0 ouyang    (1000) ouyang    (1000)        1 2023-08-18 10:53:09.000000 pybarnes-0.2.0b0/pybarnes.egg-info/dependency_links.txt
+-rw-r--r--   0 ouyang    (1000) ouyang    (1000)        6 2023-08-18 10:53:09.000000 pybarnes-0.2.0b0/pybarnes.egg-info/requires.txt
+-rw-r--r--   0 ouyang    (1000) ouyang    (1000)        9 2023-08-18 10:53:09.000000 pybarnes-0.2.0b0/pybarnes.egg-info/top_level.txt
+-rw-r--r--   0 ouyang    (1000) ouyang    (1000)       38 2023-08-18 10:53:09.622463 pybarnes-0.2.0b0/setup.cfg
+-rwxr-xr-x   0 ouyang    (1000) ouyang    (1000)      191 2023-08-18 10:40:43.000000 pybarnes-0.2.0b0/setup.py
```

### Comparing `pybarnes-0.2.0a0/pybarnes/barnes_filter.py` & `pybarnes-0.2.0b0/pybarnes/barnes_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,25 +213,26 @@
         lowpass1 = self.__lowpass(g1, c1)
         lowpass2 = self.__lowpass(g2, c2)
         return self.__convert_data(lowpass1 - lowpass2)
 
 
 class BarnesFilter4Scatter:
 
-    def __init__(self, lon, lat, data_arr, radius_degree=10, neighbor_dots=None):
+    def __init__(self, lon, lat, data_arr, radius_degree=10, neighbor_dots=None, print_progress=True):
         assert data_arr.ndim == lon.ndim == lat.ndim == 1
         idx = np.isnan(data_arr)
         if idx.sum() > 0:
-            data = data_arr[~idx]
+            data_arr = data_arr[~idx]
             lon = lon[~idx]
             lat = lat[~idx]
         self.ndots = len(data_arr)
         self.lon = lon
         self.data = data_arr
         self.lat = lat
+        self.print_progress = print_progress
 
         lat0, lon0 = np.mean(self.lat), np.mean(self.lon)
         self.factor = 6370 * np.cos(np.deg2rad(lat0)) * np.pi/180
         deg2center = np.sqrt((self.lon - lon0) ** 2 + (self.lat - lat0) ** 2)
         if neighbor_dots is None:
             self.dots = max((deg2center <= radius_degree).sum(), 1)
         else:
@@ -245,22 +246,27 @@
             ddeg2 = dlon ** 2 + dlat ** 2
             k2 = ddeg2 * self.factor ** 2
             self.idx = np.argsort(k2, axis=-1)[:, :self.dots]
             self.kilometer_distance2 = k2[np.arange(self.ndots)[:, None], self.idx]
         else:
             pts = np.stack((self.lon, self.lat), 0)
             kilometer_distance2, idx = [], []
-            for x, y in np.array_split(pts, self.thereshold, axis=1):
+            it = np.array_split(pts, self.thereshold, axis=1)
+            if self.print_progress:
+                from tqdm import tqdm
+                it = tqdm(it)
+            for x, y in it:
                 dlon = get_lon_distance(x, self.lon)
                 dlat = y[:, None] - self.lat
                 ddeg2 = dlon ** 2 + dlat ** 2
                 k2 = ddeg2 * self.factor ** 2
                 ind = np.argsort(k2, axis=-1)[:, :self.dots]
-                kilometer_distance2.append(k2[np.arange(len(x))[:, None], ind])
-                idx.append(ind)
+                kilometer_distance2.append(k2[np.arange(len(x))[:, None], ind].astype(np.float32))
+                idx.append(ind.astype(np.int32))
+                del dlon, dlat, ddeg2, k2, ind
             self.idx = np.concatenate(idx, 0)
             self.kilometer_distance2 = np.concatenate(kilometer_distance2, 0)
     
     def __make_datafield(self, data):
         return data[self.idx]
 
     def lowpass(self, g=0.3, c=150000):
```

