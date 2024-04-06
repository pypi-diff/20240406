# Comparing `tmp/soundtools-0.1.3.tar.gz` & `tmp/soundtools-0.1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soundtools-0.1.3.tar", last modified: Tue Mar 26 03:05:54 2024, max compression
+gzip compressed data, was "soundtools-0.1.3.1.tar", last modified: Sat Apr  6 19:19:41 2024, max compression
```

## Comparing `soundtools-0.1.3.tar` & `soundtools-0.1.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-03-26 03:05:54.707976 soundtools-0.1.3/
--rw-rw-rw-   0        0        0      343 2024-03-26 03:05:54.706925 soundtools-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      240 2024-03-26 02:19:51.000000 soundtools-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2024-03-26 03:05:54.707976 soundtools-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      409 2024-03-26 02:18:54.000000 soundtools-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-26 03:05:54.681214 soundtools-0.1.3/soundtools/
--rw-rw-rw-   0        0        0        0 2024-03-21 02:07:04.000000 soundtools-0.1.3/soundtools/__init__.py
--rw-rw-rw-   0        0        0    31322 2024-03-26 03:04:41.000000 soundtools-0.1.3/soundtools/soundtools.py
-drwxrwxrwx   0        0        0        0 2024-03-26 03:05:54.706925 soundtools-0.1.3/soundtools.egg-info/
--rw-rw-rw-   0        0        0      343 2024-03-26 03:05:54.000000 soundtools-0.1.3/soundtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-03-26 03:05:54.000000 soundtools-0.1.3/soundtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 03:05:54.000000 soundtools-0.1.3/soundtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-03-26 03:05:54.000000 soundtools-0.1.3/soundtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 19:19:41.693376 soundtools-0.1.3.1/
+-rw-rw-rw-   0        0        0      345 2024-04-06 19:19:41.693376 soundtools-0.1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-03-26 02:19:51.000000 soundtools-0.1.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-06 19:19:41.693376 soundtools-0.1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      411 2024-04-06 19:17:40.000000 soundtools-0.1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 19:19:41.680921 soundtools-0.1.3.1/soundtools/
+-rw-rw-rw-   0        0        0       24 2024-04-06 19:17:57.000000 soundtools-0.1.3.1/soundtools/__init__.py
+-rw-rw-rw-   0        0        0    31723 2024-03-29 13:04:18.000000 soundtools-0.1.3.1/soundtools/soundtools.py
+drwxrwxrwx   0        0        0        0 2024-04-06 19:19:41.692371 soundtools-0.1.3.1/soundtools.egg-info/
+-rw-rw-rw-   0        0        0      345 2024-04-06 19:19:41.000000 soundtools-0.1.3.1/soundtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-04-06 19:19:41.000000 soundtools-0.1.3.1/soundtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 19:19:41.000000 soundtools-0.1.3.1/soundtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-06 19:19:41.000000 soundtools-0.1.3.1/soundtools.egg-info/top_level.txt
```

### Comparing `soundtools-0.1.3/soundtools/soundtools.py` & `soundtools-0.1.3.1/soundtools/soundtools.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from os.path import splitext
 from pydub.audio_segment import AudioSegment
 from soundfile import read as sfRead
 
 
 # types #
 SoundBuffer = np.ndarray[np.any, np.dtype[np.float32|np.int16|np.uint8]]
-Wave = Callable[[float, float, float], np.ndarray[np.any, np.dtype]]
+Wave = Callable[[float, float, float], SoundBuffer]
 
 
 # its just a dictionary
 class Notes(dict[str, float]):
     """a dictionary used to store note names and frequencies"""
     def __init__(self):
         super().__init__()
@@ -53,24 +53,27 @@
         self.eight_over_pi_sqr = 8/np.pi**2
         
         self.dtype = dtype
         
     # caches the waves so if you had to generate a note multiple times its not gonna take long to execute
     # you can't use the lru_cache from the functools module because waves are stored as numpy arrays and numpy arrays are not hashable
     # so this decorator will save a tuple of that numpy array in self.existed_notes and convert it back to a numpy array each time you want to use that wave
-    def cache_wave(wave_type:str) -> SoundBuffer:
-        """returns the cached value if available, otherwise caches the returned wave"""
-        def decorator(func):
+    def cache_wave(wave_type: str) -> SoundBuffer:
+        """caches the waves so if you had to generate a note multiple times it's gonna use the cached wave. 
+        you can't use the lru_cache from the functools module because waves are stored as numpy arrays and numpy arrays are not hashable, 
+        so this decorator will store the numpy array as a tuple in "self.existed_notes" and convert it back to a numpy array each time you want to use that wave
+        \nreturns the cached value if available, otherwise caches the returned wave"""
+        def decorator(func: Wave) -> SoundBuffer:
             def wrapper(self, freq:float, dur:float, vol: float):
                 name = f"{wave_type}|{freq}|{dur}|{vol}"
                 if name in self.existed_notes.keys():
                     self.total_cached += 1
                     return np.array(self.existed_notes[name], dtype=self.dtype)
                 
-                result = func(self, freq, dur, vol)
+                result: SoundBuffer = func(self, freq, dur, vol)
                 self.existed_notes[name] = self.array_to_tuple(result)
                 
                 return result
             return wrapper
         return decorator
 
     @cache_wave("sine")
@@ -558,16 +561,14 @@
             data = np.frombuffer(sound._data, dtype=dtype)
             return (data, sound.frame_rate)
             
         
         #-- other files such as mp3, ogg, wav, aiff, flac --#
         else:
             return sfRead(file_path)
-            
-            
     
     
     def pitch_shift(self, wave: SoundBuffer, semitones: float, sample_rate: int|None=None, semitones_per_octave: int=12) -> SoundBuffer:
         """shifts the pitch by the given number of semitones"""
         if not sample_rate:
             sample_rate = self.default_sample_rate
```

