# Comparing `tmp/py_ballisticcalc.exts-2.0.0b3.tar.gz` & `tmp/py_ballisticcalc.exts-2.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ballisticcalc.exts-2.0.0b3.tar", last modified: Thu Apr  4 18:32:43 2024, max compression
+gzip compressed data, was "py_ballisticcalc.exts-2.0.0b4.tar", last modified: Sat Apr  6 18:23:19 2024, max compression
```

## Comparing `py_ballisticcalc.exts-2.0.0b3.tar` & `py_ballisticcalc.exts-2.0.0b4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:32:43.125635 py_ballisticcalc.exts-2.0.0b3/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-04 18:32:26.000000 py_ballisticcalc.exts-2.0.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    18977 2024-04-04 18:32:43.125635 py_ballisticcalc.exts-2.0.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8770 2024-04-04 18:32:26.000000 py_ballisticcalc.exts-2.0.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:32:43.125635 py_ballisticcalc.exts-2.0.0b3/py_ballisticcalc.exts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18977 2024-04-04 18:32:43.000000 py_ballisticcalc.exts-2.0.0b3/py_ballisticcalc.exts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-04 18:32:43.000000 py_ballisticcalc.exts-2.0.0b3/py_ballisticcalc.exts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 18:32:43.000000 py_ballisticcalc.exts-2.0.0b3/py_ballisticcalc.exts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 18:32:43.000000 py_ballisticcalc.exts-2.0.0b3/py_ballisticcalc.exts.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:32:43.125635 py_ballisticcalc.exts-2.0.0b3/py_ballisticcalc_exts/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-04 18:32:26.000000 py_ballisticcalc.exts-2.0.0b3/py_ballisticcalc_exts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   885017 2024-04-04 18:32:42.000000 py_ballisticcalc.exts-2.0.0b3/py_ballisticcalc_exts/trajectory_calc.c
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-04 18:32:26.000000 py_ballisticcalc.exts-2.0.0b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 18:32:43.125635 py_ballisticcalc.exts-2.0.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-04 18:32:26.000000 py_ballisticcalc.exts-2.0.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:23:19.067284 py_ballisticcalc.exts-2.0.0b4/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-06 18:23:07.000000 py_ballisticcalc.exts-2.0.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18977 2024-04-06 18:23:19.067284 py_ballisticcalc.exts-2.0.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8770 2024-04-06 18:23:07.000000 py_ballisticcalc.exts-2.0.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:23:19.067284 py_ballisticcalc.exts-2.0.0b4/py_ballisticcalc.exts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18977 2024-04-06 18:23:19.000000 py_ballisticcalc.exts-2.0.0b4/py_ballisticcalc.exts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-06 18:23:19.000000 py_ballisticcalc.exts-2.0.0b4/py_ballisticcalc.exts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:23:19.000000 py_ballisticcalc.exts-2.0.0b4/py_ballisticcalc.exts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-06 18:23:19.000000 py_ballisticcalc.exts-2.0.0b4/py_ballisticcalc.exts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:23:19.067284 py_ballisticcalc.exts-2.0.0b4/py_ballisticcalc_exts/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-06 18:23:07.000000 py_ballisticcalc.exts-2.0.0b4/py_ballisticcalc_exts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   816102 2024-04-06 18:23:18.000000 py_ballisticcalc.exts-2.0.0b4/py_ballisticcalc_exts/trajectory_calc.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-06 18:23:07.000000 py_ballisticcalc.exts-2.0.0b4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 18:23:19.067284 py_ballisticcalc.exts-2.0.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-06 18:23:07.000000 py_ballisticcalc.exts-2.0.0b4/setup.py
```

### Comparing `py_ballisticcalc.exts-2.0.0b3/LICENSE` & `py_ballisticcalc.exts-2.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc.exts-2.0.0b3/PKG-INFO` & `py_ballisticcalc.exts-2.0.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ballisticcalc.exts
-Version: 2.0.0b3
+Version: 2.0.0b4
 Summary: LGPL library for small arms ballistic calculations (Python 3)
 Author-email: o-murphy <thehelixpg@gmail.com>, dbookstaber <bookstaber@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `py_ballisticcalc.exts-2.0.0b3/README.md` & `py_ballisticcalc.exts-2.0.0b4/README.md`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc.exts-2.0.0b3/py_ballisticcalc.exts.egg-info/PKG-INFO` & `py_ballisticcalc.exts-2.0.0b4/py_ballisticcalc.exts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ballisticcalc.exts
-Version: 2.0.0b3
+Version: 2.0.0b4
 Summary: LGPL library for small arms ballistic calculations (Python 3)
 Author-email: o-murphy <thehelixpg@gmail.com>, dbookstaber <bookstaber@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `py_ballisticcalc.exts-2.0.0b3/py_ballisticcalc_exts/trajectory_calc.c` & `py_ballisticcalc.exts-2.0.0b4/py_ballisticcalc_exts/trajectory_calc.c`

 * *Files 4% similar despite different names*

```diff
@@ -1494,84 +1494,84 @@
 /* #### Code section: complex_type_declarations ### */
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector;
 struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc;
 struct __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CurvePoint;
-struct __pyx_opt_args_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_get_calc_step;
+struct __pyx_opt_args_21py_ballisticcalc_exts_15trajectory_calc_get_calc_step;
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":21
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":58
  *     double a, b, c
  * 
  * cdef enum CTrajFlag:             # <<<<<<<<<<<<<<
  *     NONE = 0
  *     ZERO_UP = 1
  */
 enum __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag {
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":29
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":66
  *     DANGER = 16
  *     ZERO = ZERO_UP | ZERO_DOWN
  *     ALL = RANGE | ZERO_UP | ZERO_DOWN | MACH | DANGER             # <<<<<<<<<<<<<<
  * 
- * cdef class Vector:
+ * 
  */
   __pyx_e_21py_ballisticcalc_exts_15trajectory_calc_NONE = 0,
   __pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_UP = 1,
   __pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_DOWN = 2,
   __pyx_e_21py_ballisticcalc_exts_15trajectory_calc_MACH = 4,
   __pyx_e_21py_ballisticcalc_exts_15trajectory_calc_RANGE = 8,
   __pyx_e_21py_ballisticcalc_exts_15trajectory_calc_DANGER = 16,
   __pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO = (__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_UP | __pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_DOWN),
   __pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ALL = ((((__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_RANGE | __pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_UP) | __pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_DOWN) | __pyx_e_21py_ballisticcalc_exts_15trajectory_calc_MACH) | __pyx_e_21py_ballisticcalc_exts_15trajectory_calc_DANGER)
 };
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":18
- * cdef double cGravityConstant = -32.17405
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":55
+ * 
  * 
  * cdef struct CurvePoint:             # <<<<<<<<<<<<<<
  *     double a, b, c
  * 
  */
 struct __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CurvePoint {
   double a;
   double b;
   double c;
 };
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":128
- *         self.gravity_vector = Vector(.0, cGravityConstant, .0)
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":439
  * 
- *     cdef double get_calc_step(self, double step = 0):             # <<<<<<<<<<<<<<
- *         if step == 0:
- *             return Settings.get_max_calc_step_size() / 2.0
+ * @cython.cdivision(True)
+ * cdef double get_calc_step(double step = 0):             # <<<<<<<<<<<<<<
+ *     cdef double preferred_step = _globalMaxCalcStepSize >> Distance.Foot
+ *     # cdef double defined_max = 0.5  # const will be better optimized with cython
  */
-struct __pyx_opt_args_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_get_calc_step {
+struct __pyx_opt_args_21py_ballisticcalc_exts_15trajectory_calc_get_calc_step {
   int __pyx_n;
   double step;
 };
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":31
- *     ALL = RANGE | ZERO_UP | ZERO_DOWN | MACH | DANGER
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":69
+ * 
  * 
  * cdef class Vector:             # <<<<<<<<<<<<<<
  *     cdef double x
  *     cdef double y
  */
 struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector {
   PyObject_HEAD
   struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_vtab;
   double x;
   double y;
   double z;
 };
 
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":99
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":137
  *         return self.negate()
  * 
  * cdef class TrajectoryCalc:             # <<<<<<<<<<<<<<
  *     cdef:
  *         object ammo
  */
 struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc {
@@ -1596,16 +1596,16 @@
   double calc_step;
   double muzzle_velocity;
   double stability_coefficient;
 };
 
 
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":31
- *     ALL = RANGE | ZERO_UP | ZERO_DOWN | MACH | DANGER
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":69
+ * 
  * 
  * cdef class Vector:             # <<<<<<<<<<<<<<
  *     cdef double x
  *     cdef double y
  */
 
 struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector {
@@ -1616,27 +1616,26 @@
   struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *(*subtract)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *, struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *);
   struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *(*negate)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *);
   struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *(*normalize)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *);
 };
 static struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_vtabptr_21py_ballisticcalc_exts_15trajectory_calc_Vector;
 
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":99
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":137
  *         return self.negate()
  * 
  * cdef class TrajectoryCalc:             # <<<<<<<<<<<<<<
  *     cdef:
  *         object ammo
  */
 
 struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc {
-  double (*get_calc_step)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *, struct __pyx_opt_args_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_get_calc_step *__pyx_optional_args);
   PyObject *(*_init_trajectory)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *, PyObject *);
   PyObject *(*_zero_angle)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *, PyObject *, PyObject *);
-  PyObject *(*_trajectory)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *, PyObject *, double, double, enum __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag);
+  PyObject *(*_trajectory)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *, PyObject *, double, double, int);
   double (*drag_by_mach)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *, double);
   double (*spin_drift)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *, double);
   double (*calc_stability_coefficient)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *, PyObject *);
 };
 static struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_vtabptr_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc;
 /* #### Code section: utility_code_proto ### */
 
@@ -1889,35 +1888,73 @@
 #define __Pyx_ArgsSlice_VARARGS(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_VARARGS(args, start), stop - start)
 #define __Pyx_ArgsSlice_FASTCALL(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_FASTCALL(args, start), stop - start)
 #else
 #define __Pyx_ArgsSlice_VARARGS(args, start, stop) PyTuple_GetSlice(args, start, stop)
 #define __Pyx_ArgsSlice_FASTCALL(args, start, stop) PyTuple_GetSlice(args, start, stop)
 #endif
 
-/* RaiseArgTupleInvalid.proto */
-static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
-    Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
-
 /* RaiseDoubleKeywords.proto */
 static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
 
 /* ParseKeywords.proto */
 static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject *const *kwvalues,
     PyObject **argnames[],
     PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,
     const char* function_name);
 
-/* ArgTypeTest.proto */
-#define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
-    ((likely(__Pyx_IS_TYPE(obj, type) | (none_allowed && (obj == Py_None)))) ? 1 :\
-        __Pyx__ArgTypeTest(obj, type, name, exact))
-static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
+/* RaiseArgTupleInvalid.proto */
+static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
+    Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
 
-/* ExtTypeTest.proto */
-static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
+/* PyDictVersioning.proto */
+#if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
+#define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
+#define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
+#define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
+    (version_var) = __PYX_GET_DICT_VERSION(dict);\
+    (cache_var) = (value);
+#define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP) {\
+    static PY_UINT64_T __pyx_dict_version = 0;\
+    static PyObject *__pyx_dict_cached_value = NULL;\
+    if (likely(__PYX_GET_DICT_VERSION(DICT) == __pyx_dict_version)) {\
+        (VAR) = __pyx_dict_cached_value;\
+    } else {\
+        (VAR) = __pyx_dict_cached_value = (LOOKUP);\
+        __pyx_dict_version = __PYX_GET_DICT_VERSION(DICT);\
+    }\
+}
+static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj);
+static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj);
+static CYTHON_INLINE int __Pyx_object_dict_version_matches(PyObject* obj, PY_UINT64_T tp_dict_version, PY_UINT64_T obj_dict_version);
+#else
+#define __PYX_GET_DICT_VERSION(dict)  (0)
+#define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
+#define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
+#endif
+
+/* GetModuleGlobalName.proto */
+#if CYTHON_USE_DICT_VERSIONS
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
+    static PY_UINT64_T __pyx_dict_version = 0;\
+    static PyObject *__pyx_dict_cached_value = NULL;\
+    (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
+        (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
+        __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
+    PY_UINT64_T __pyx_dict_version;\
+    PyObject *__pyx_dict_cached_value;\
+    (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
+} while(0)
+static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
+#else
+#define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
+static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
+#endif
 
 /* PyFunctionFastCall.proto */
 #if CYTHON_FAST_PYCALL
 #if !CYTHON_VECTORCALL
 #define __Pyx_PyFunction_FastCall(func, args, nargs)\
     __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
 static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
@@ -1955,78 +1992,40 @@
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
 #endif
 
 /* PyObjectFastCall.proto */
 #define __Pyx_PyObject_FastCall(func, args, nargs)  __Pyx_PyObject_FastCallDict(func, args, (size_t)(nargs), NULL)
 static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs);
 
+/* PyObjectFormatAndDecref.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FormatSimpleAndDecref(PyObject* s, PyObject* f);
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FormatAndDecref(PyObject* s, PyObject* f);
+
+/* JoinPyUnicode.proto */
+static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
+                                      Py_UCS4 max_char);
+
 /* PyObjectCallOneArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
 
+/* ArgTypeTest.proto */
+#define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
+    ((likely(__Pyx_IS_TYPE(obj, type) | (none_allowed && (obj == Py_None)))) ? 1 :\
+        __Pyx__ArgTypeTest(obj, type, name, exact))
+static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
+
+/* ExtTypeTest.proto */
+static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
+
 /* KeywordStringCheck.proto */
 static int __Pyx_CheckKeywordStrings(PyObject *kw, const char* function_name, int kw_allowed);
 
 /* RaiseUnexpectedTypeError.proto */
 static int __Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj);
 
-/* PyFloatBinop.proto */
-#if !CYTHON_COMPILING_IN_PYPY
-static PyObject* __Pyx_PyFloat_TrueDivideObjC(PyObject *op1, PyObject *op2, double floatval, int inplace, int zerodivision_check);
-#else
-#define __Pyx_PyFloat_TrueDivideObjC(op1, op2, floatval, inplace, zerodivision_check)\
-    (inplace ? PyNumber_InPlaceTrueDivide(op1, op2) : PyNumber_TrueDivide(op1, op2))
-#endif
-
-/* PyDictVersioning.proto */
-#if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
-#define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
-#define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
-#define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
-    (version_var) = __PYX_GET_DICT_VERSION(dict);\
-    (cache_var) = (value);
-#define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP) {\
-    static PY_UINT64_T __pyx_dict_version = 0;\
-    static PyObject *__pyx_dict_cached_value = NULL;\
-    if (likely(__PYX_GET_DICT_VERSION(DICT) == __pyx_dict_version)) {\
-        (VAR) = __pyx_dict_cached_value;\
-    } else {\
-        (VAR) = __pyx_dict_cached_value = (LOOKUP);\
-        __pyx_dict_version = __PYX_GET_DICT_VERSION(DICT);\
-    }\
-}
-static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj);
-static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj);
-static CYTHON_INLINE int __Pyx_object_dict_version_matches(PyObject* obj, PY_UINT64_T tp_dict_version, PY_UINT64_T obj_dict_version);
-#else
-#define __PYX_GET_DICT_VERSION(dict)  (0)
-#define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
-#define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
-#endif
-
-/* GetModuleGlobalName.proto */
-#if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  do {\
-    static PY_UINT64_T __pyx_dict_version = 0;\
-    static PyObject *__pyx_dict_cached_value = NULL;\
-    (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
-        (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
-        __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-} while(0)
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
-    PY_UINT64_T __pyx_dict_version;\
-    PyObject *__pyx_dict_cached_value;\
-    (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-} while(0)
-static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
-#else
-#define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
-static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
-#endif
-
 /* GetItemInt.proto */
 #define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
     (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
     __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
     (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
                __Pyx_GetItemInt_Generic(o, to_py_func(i))))
 #define __Pyx_GetItemInt_List(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
@@ -2075,18 +2074,14 @@
 /* BuildPyUnicode.proto */
 static PyObject* __Pyx_PyUnicode_BuildFromAscii(Py_ssize_t ulength, char* chars, int clength,
                                                 int prepend_sign, char padding_char);
 
 /* CIntToPyUnicode.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_From_int(int value, Py_ssize_t width, char padding_char, char format_char);
 
-/* JoinPyUnicode.proto */
-static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
-                                      Py_UCS4 max_char);
-
 /* PyIntBinop.proto */
 #if !CYTHON_COMPILING_IN_PYPY
 static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check);
 #else
 #define __Pyx_PyInt_AddObjC(op1, op2, intval, inplace, zerodivision_check)\
     (inplace ? PyNumber_InPlaceAdd(op1, op2) : PyNumber_Add(op1, op2))
 #endif
@@ -2127,43 +2122,17 @@
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
 #endif
 
-/* RaiseUnboundLocalError.proto */
-static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname);
-
-/* PyIntBinop.proto */
-#if !CYTHON_COMPILING_IN_PYPY
-static PyObject* __Pyx_PyInt_TrueDivideObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check);
-#else
-#define __Pyx_PyInt_TrueDivideObjC(op1, op2, intval, inplace, zerodivision_check)\
-    (inplace ? PyNumber_InPlaceTrueDivide(op1, op2) : PyNumber_TrueDivide(op1, op2))
-#endif
-
 /* GetAttr3.proto */
 static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *, PyObject *, PyObject *);
 
-/* PyIntBinop.proto */
-#if !CYTHON_COMPILING_IN_PYPY
-static PyObject* __Pyx_PyInt_SubtractObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check);
-#else
-#define __Pyx_PyInt_SubtractObjC(op1, op2, intval, inplace, zerodivision_check)\
-    (inplace ? PyNumber_InPlaceSubtract(op1, op2) : PyNumber_Subtract(op1, op2))
-#endif
-
-/* ObjectGetItem.proto */
-#if CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject *key);
-#else
-#define __Pyx_PyObject_GetItem(obj, key)  PyObject_GetItem(obj, key)
-#endif
-
 /* PySequenceContains.proto */
 static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
     int result = PySequence_Contains(seq, item);
     return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
 }
 
 /* Import.proto */
@@ -2233,154 +2202,14 @@
 #endif
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
-/* FetchSharedCythonModule.proto */
-static PyObject *__Pyx_FetchSharedCythonABIModule(void);
-
-/* FetchCommonType.proto */
-#if !CYTHON_USE_TYPE_SPECS
-static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
-#else
-static PyTypeObject* __Pyx_FetchCommonTypeFromSpec(PyObject *module, PyType_Spec *spec, PyObject *bases);
-#endif
-
-/* PyMethodNew.proto */
-#if CYTHON_COMPILING_IN_LIMITED_API
-static PyObject *__Pyx_PyMethod_New(PyObject *func, PyObject *self, PyObject *typ) {
-    PyObject *typesModule=NULL, *methodType=NULL, *result=NULL;
-    CYTHON_UNUSED_VAR(typ);
-    if (!self)
-        return __Pyx_NewRef(func);
-    typesModule = PyImport_ImportModule("types");
-    if (!typesModule) return NULL;
-    methodType = PyObject_GetAttrString(typesModule, "MethodType");
-    Py_DECREF(typesModule);
-    if (!methodType) return NULL;
-    result = PyObject_CallFunctionObjArgs(methodType, func, self, NULL);
-    Py_DECREF(methodType);
-    return result;
-}
-#elif PY_MAJOR_VERSION >= 3
-static PyObject *__Pyx_PyMethod_New(PyObject *func, PyObject *self, PyObject *typ) {
-    CYTHON_UNUSED_VAR(typ);
-    if (!self)
-        return __Pyx_NewRef(func);
-    return PyMethod_New(func, self);
-}
-#else
-    #define __Pyx_PyMethod_New PyMethod_New
-#endif
-
-/* PyVectorcallFastCallDict.proto */
-#if CYTHON_METH_FASTCALL
-static CYTHON_INLINE PyObject *__Pyx_PyVectorcall_FastCallDict(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw);
-#endif
-
-/* CythonFunctionShared.proto */
-#define __Pyx_CyFunction_USED
-#define __Pyx_CYFUNCTION_STATICMETHOD  0x01
-#define __Pyx_CYFUNCTION_CLASSMETHOD   0x02
-#define __Pyx_CYFUNCTION_CCLASS        0x04
-#define __Pyx_CYFUNCTION_COROUTINE     0x08
-#define __Pyx_CyFunction_GetClosure(f)\
-    (((__pyx_CyFunctionObject *) (f))->func_closure)
-#if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
-  #define __Pyx_CyFunction_GetClassObj(f)\
-      (((__pyx_CyFunctionObject *) (f))->func_classobj)
-#else
-  #define __Pyx_CyFunction_GetClassObj(f)\
-      ((PyObject*) ((PyCMethodObject *) (f))->mm_class)
-#endif
-#define __Pyx_CyFunction_SetClassObj(f, classobj)\
-    __Pyx__CyFunction_SetClassObj((__pyx_CyFunctionObject *) (f), (classobj))
-#define __Pyx_CyFunction_Defaults(type, f)\
-    ((type *)(((__pyx_CyFunctionObject *) (f))->defaults))
-#define __Pyx_CyFunction_SetDefaultsGetter(f, g)\
-    ((__pyx_CyFunctionObject *) (f))->defaults_getter = (g)
-typedef struct {
-#if CYTHON_COMPILING_IN_LIMITED_API
-    PyObject_HEAD
-    PyObject *func;
-#elif PY_VERSION_HEX < 0x030900B1
-    PyCFunctionObject func;
-#else
-    PyCMethodObject func;
-#endif
-#if CYTHON_BACKPORT_VECTORCALL
-    __pyx_vectorcallfunc func_vectorcall;
-#endif
-#if PY_VERSION_HEX < 0x030500A0 || CYTHON_COMPILING_IN_LIMITED_API
-    PyObject *func_weakreflist;
-#endif
-    PyObject *func_dict;
-    PyObject *func_name;
-    PyObject *func_qualname;
-    PyObject *func_doc;
-    PyObject *func_globals;
-    PyObject *func_code;
-    PyObject *func_closure;
-#if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
-    PyObject *func_classobj;
-#endif
-    void *defaults;
-    int defaults_pyobjects;
-    size_t defaults_size;
-    int flags;
-    PyObject *defaults_tuple;
-    PyObject *defaults_kwdict;
-    PyObject *(*defaults_getter)(PyObject *);
-    PyObject *func_annotations;
-    PyObject *func_is_coroutine;
-} __pyx_CyFunctionObject;
-#undef __Pyx_CyOrPyCFunction_Check
-#define __Pyx_CyFunction_Check(obj)  __Pyx_TypeCheck(obj, __pyx_CyFunctionType)
-#define __Pyx_CyOrPyCFunction_Check(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
-#define __Pyx_CyFunction_CheckExact(obj)  __Pyx_IS_TYPE(obj, __pyx_CyFunctionType)
-static CYTHON_INLINE int __Pyx__IsSameCyOrCFunction(PyObject *func, void *cfunc);
-#undef __Pyx_IsSameCFunction
-#define __Pyx_IsSameCFunction(func, cfunc)   __Pyx__IsSameCyOrCFunction(func, cfunc)
-static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject* op, PyMethodDef *ml,
-                                      int flags, PyObject* qualname,
-                                      PyObject *closure,
-                                      PyObject *module, PyObject *globals,
-                                      PyObject* code);
-static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj);
-static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *m,
-                                                         size_t size,
-                                                         int pyobjects);
-static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *m,
-                                                            PyObject *tuple);
-static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *m,
-                                                             PyObject *dict);
-static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *m,
-                                                              PyObject *dict);
-static int __pyx_CyFunction_init(PyObject *module);
-#if CYTHON_METH_FASTCALL
-static PyObject * __Pyx_CyFunction_Vectorcall_NOARGS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
-static PyObject * __Pyx_CyFunction_Vectorcall_O(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
-static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
-static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
-#if CYTHON_BACKPORT_VECTORCALL
-#define __Pyx_CyFunction_func_vectorcall(f) (((__pyx_CyFunctionObject*)f)->func_vectorcall)
-#else
-#define __Pyx_CyFunction_func_vectorcall(f) (((PyCFunctionObject*)f)->vectorcall)
-#endif
-#endif
-
-/* CythonFunction.proto */
-static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml,
-                                      int flags, PyObject* qualname,
-                                      PyObject *closure,
-                                      PyObject *module, PyObject *globals,
-                                      PyObject* code);
-
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
 #endif
 
@@ -2407,24 +2236,21 @@
 
 struct __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CurvePoint;
 static PyObject* __pyx_convert__to_py_struct____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CurvePoint(struct __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CurvePoint s);
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(enum __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag value);
-
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* FormatTypeName.proto */
 #if CYTHON_COMPILING_IN_LIMITED_API
 typedef PyObject *__Pyx_TypeName;
 #define __Pyx_FMT_TYPENAME "%U"
 static __Pyx_TypeName __Pyx_PyType_GetName(PyTypeObject* tp);
 #define __Pyx_DECREF_TypeName(obj) Py_XDECREF(obj)
@@ -2466,123 +2292,120 @@
 static double __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_6Vector_magnitude(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_self); /* proto*/
 static struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_6Vector_mul_by_const(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_self, double __pyx_v_a); /* proto*/
 static double __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_6Vector_mul_by_vector(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_self, struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_b); /* proto*/
 static struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_6Vector_add(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_self, struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_b); /* proto*/
 static struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_6Vector_subtract(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_self, struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_b); /* proto*/
 static struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_6Vector_negate(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_self); /* proto*/
 static struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_6Vector_normalize(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_self); /* proto*/
-static double __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_get_calc_step(CYTHON_UNUSED struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, struct __pyx_opt_args_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_get_calc_step *__pyx_optional_args); /* proto*/
 static PyObject *__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc__init_trajectory(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, PyObject *__pyx_v_shot_info); /* proto*/
 static PyObject *__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc__zero_angle(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, PyObject *__pyx_v_shot_info, PyObject *__pyx_v_distance); /* proto*/
-static PyObject *__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc__trajectory(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, PyObject *__pyx_v_shot_info, double __pyx_v_maximum_range, double __pyx_v_step, enum __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag __pyx_v_filter_flags); /* proto*/
+static PyObject *__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc__trajectory(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, PyObject *__pyx_v_shot_info, double __pyx_v_maximum_range, double __pyx_v_step, int __pyx_v_filter_flags); /* proto*/
 static double __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_drag_by_mach(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, double __pyx_v_mach); /* proto*/
 static double __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_spin_drift(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, double __pyx_v_time); /* proto*/
 static double __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_calc_stability_coefficient(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, PyObject *__pyx_v_atmo); /* proto*/
 
 /* Module declarations from "libc.math" */
 
 /* Module declarations from "cython" */
 
 /* Module declarations from "py_ballisticcalc_exts.trajectory_calc" */
 static double __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cZeroFindingAccuracy;
 static double __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cMinimumVelocity;
 static double __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cMaximumDrop;
 static int __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cMaxIterations;
 static double __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cGravityConstant;
+static int __pyx_v_21py_ballisticcalc_exts_15trajectory_calc__globalUsePowderSensitivity;
+static PyObject *__pyx_v_21py_ballisticcalc_exts_15trajectory_calc__globalMaxCalcStepSize = 0;
 static struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_wind_to_vector(PyObject *); /*proto*/
 static PyObject *__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_create_trajectory_row(double, struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *, struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *, double, double, double, double, double, double, double, PyObject *); /*proto*/
 static double __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_get_correction(double, double); /*proto*/
+static double __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_get_calc_step(struct __pyx_opt_args_21py_ballisticcalc_exts_15trajectory_calc_get_calc_step *__pyx_optional_args); /*proto*/
 static double __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_calculate_energy(double, double); /*proto*/
 static double __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_calculate_ogv(double, double); /*proto*/
 static PyObject *__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_calculate_curve(PyObject *); /*proto*/
 static double __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_calculate_by_curve(PyObject *, PyObject *, double); /*proto*/
 static PyObject *__pyx_f_21py_ballisticcalc_exts_15trajectory_calc___pyx_unpickle_TrajectoryCalc__set_state(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *, PyObject *); /*proto*/
 static struct __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CurvePoint __pyx_convert__from_py_struct____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CurvePoint(PyObject *); /*proto*/
 /* #### Code section: typeinfo ### */
 /* #### Code section: before_global_var ### */
 #define __Pyx_MODULE_NAME "py_ballisticcalc_exts.trajectory_calc"
 extern int __pyx_module_is_main_py_ballisticcalc_exts__trajectory_calc;
 int __pyx_module_is_main_py_ballisticcalc_exts__trajectory_calc = 0;
 
 /* Implementation of "py_ballisticcalc_exts.trajectory_calc" */
 /* #### Code section: global_var ### */
+static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_KeyError;
-static PyObject *__pyx_builtin_ValueError;
 /* #### Code section: string_decls ### */
 static const char __pyx_k_a[] = "a";
 static const char __pyx_k_b[] = "b";
 static const char __pyx_k_c[] = "c";
 static const char __pyx_k_x[] = "x";
 static const char __pyx_k_y[] = "y";
 static const char __pyx_k_z[] = "z";
 static const char __pyx_k_BC[] = "BC";
 static const char __pyx_k_CD[] = "CD";
-static const char __pyx_k__6[] = ".";
-static const char __pyx_k__7[] = "*";
+static const char __pyx_k__7[] = ".";
+static const char __pyx_k__8[] = "*";
 static const char __pyx_k_dm[] = "dm";
 static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_mv[] = "mv";
 static const char __pyx_k_FPS[] = "FPS";
-static const char __pyx_k__23[] = "?";
+static const char __pyx_k__20[] = "?";
 static const char __pyx_k_all[] = "__all__";
 static const char __pyx_k_mul[] = "__mul__";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_ogw[] = "ogw";
 static const char __pyx_k_Ammo[] = "Ammo";
-static const char __pyx_k_Atmo[] = "Atmo";
 static const char __pyx_k_Foot[] = "Foot";
 static const char __pyx_k_InHg[] = "InHg";
 static const char __pyx_k_Inch[] = "Inch";
 static const char __pyx_k_Mach[] = "Mach";
 static const char __pyx_k_Shot[] = "Shot";
 static const char __pyx_k_Wind[] = "Wind";
 static const char __pyx_k_ammo[] = "ammo";
 static const char __pyx_k_atmo[] = "atmo";
-static const char __pyx_k_bool[] = "bool";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_drag[] = "drag";
 static const char __pyx_k_flag[] = "flag";
 static const char __pyx_k_mach[] = "mach";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
-static const char __pyx_k_self[] = "self";
-static const char __pyx_k_step[] = "step";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_time[] = "time";
 static const char __pyx_k_Grain[] = "Grain";
 static const char __pyx_k_Pound[] = "Pound";
 static const char __pyx_k_angle[] = "angle";
 static const char __pyx_k_range[] = "range";
-static const char __pyx_k_state[] = "state";
 static const char __pyx_k_twist[] = "twist";
+static const char __pyx_k_value[] = "value";
 static const char __pyx_k_winds[] = "winds";
 static const char __pyx_k_Energy[] = "Energy";
 static const char __pyx_k_Radian[] = "Radian";
 static const char __pyx_k_Vector[] = "Vector";
 static const char __pyx_k_Weight[] = "Weight";
-static const char __pyx_k_dict_2[] = "_dict";
 static const char __pyx_k_enable[] = "enable";
 static const char __pyx_k_energy[] = "energy";
 static const char __pyx_k_height[] = "height";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_length[] = "length";
 static const char __pyx_k_pickle[] = "pickle";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_update[] = "update";
 static const char __pyx_k_weapon[] = "weapon";
 static const char __pyx_k_weight[] = "weight";
 static const char __pyx_k_Angular[] = "Angular";
 static const char __pyx_k_disable[] = "disable";
+static const char __pyx_k_value_2[] = "_value";
 static const char __pyx_k_windage[] = "windage";
 static const char __pyx_k_Distance[] = "Distance";
 static const char __pyx_k_KeyError[] = "KeyError";
 static const char __pyx_k_Pressure[] = "Pressure";
-static const char __pyx_k_Settings[] = "Settings";
 static const char __pyx_k_Velocity[] = "Velocity";
 static const char __pyx_k_altitude[] = "altitude";
 static const char __pyx_k_diameter[] = "diameter";
 static const char __pyx_k_distance[] = "distance";
 static const char __pyx_k_drop_adj[] = "drop_adj";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_pressure[] = "pressure";
@@ -2591,80 +2414,78 @@
 static const char __pyx_k_velocity[] = "velocity";
 static const char __pyx_k_FootPound[] = "FootPound";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_dist_step[] = "dist_step";
 static const char __pyx_k_isenabled[] = "isenabled";
 static const char __pyx_k_max_range[] = "max_range";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
+static const char __pyx_k_raw_value[] = "raw_value";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_shot_info[] = "shot_info";
 static const char __pyx_k_Fahrenheit[] = "Fahrenheit";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_cant_angle[] = "cant_angle";
 static const char __pyx_k_drag_table[] = "drag_table";
 static const char __pyx_k_extra_data[] = "extra_data";
 static const char __pyx_k_feet_after[] = " feet, after ";
 static const char __pyx_k_iterations[] = " iterations.";
 static const char __pyx_k_look_angle[] = "look_angle";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
-static const char __pyx_k_trajectory[] = "trajectory";
-static const char __pyx_k_zero_angle[] = "zero_angle";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_Temperature[] = "Temperature";
 static const char __pyx_k_target_drop[] = "target_drop";
 static const char __pyx_k_temperature[] = "temperature";
 static const char __pyx_k_windage_adj[] = "windage_adj";
-static const char __pyx_k_filter_flags[] = "filter_flags";
-static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_sight_height[] = "sight_height";
 static const char __pyx_k_stringsource[] = "<stringsource>";
-static const char __pyx_k_use_setstate[] = "use_setstate";
-static const char __pyx_k_class_getitem[] = "__class_getitem__";
 static const char __pyx_k_look_distance[] = "look_distance";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
+static const char __pyx_k_reset_globals[] = "reset_globals";
 static const char __pyx_k_PreferredUnits[] = "PreferredUnits";
 static const char __pyx_k_TrajectoryCalc[] = "TrajectoryCalc";
 static const char __pyx_k_TrajectoryData[] = "TrajectoryData";
 static const char __pyx_k_barrel_azimuth[] = "barrel_azimuth";
 static const char __pyx_k_density_factor[] = "density_factor";
 static const char __pyx_k_direction_from[] = "direction_from";
 static const char __pyx_k_until_distance[] = "until_distance";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_barrel_elevation[] = "barrel_elevation";
+static const char __pyx_k_is_not_a_boolean[] = " is not a boolean";
 static const char __pyx_k_MAX_DISTANCE_FEET[] = "MAX_DISTANCE_FEET";
-static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_Zero_vertical_error[] = "Zero vertical error ";
 static const char __pyx_k_get_velocity_for_temp[] = "get_velocity_for_temp";
 static const char __pyx_k_py_ballisticcalc_unit[] = "py_ballisticcalc.unit";
-static const char __pyx_k_USE_POWDER_SENSITIVITY[] = "USE_POWDER_SENSITIVITY";
-static const char __pyx_k_Vector___reduce_cython[] = "Vector.__reduce_cython__";
-static const char __pyx_k_get_max_calc_step_size[] = "get_max_calc_step_size";
-static const char __pyx_k_Vector___setstate_cython[] = "Vector.__setstate_cython__";
-static const char __pyx_k_TrajectoryCalc_trajectory[] = "TrajectoryCalc.trajectory";
-static const char __pyx_k_TrajectoryCalc_zero_angle[] = "TrajectoryCalc.zero_angle";
 static const char __pyx_k_py_ballisticcalc_munition[] = "py_ballisticcalc.munition";
-static const char __pyx_k_py_ballisticcalc_settings[] = "py_ballisticcalc.settings";
 static const char __pyx_k_py_ballisticcalc_conditions[] = "py_ballisticcalc.conditions";
 static const char __pyx_k_pyx_unpickle_TrajectoryCalc[] = "__pyx_unpickle_TrajectoryCalc";
-static const char __pyx_k_TrajectoryCalc___reduce_cython[] = "TrajectoryCalc.__reduce_cython__";
+static const char __pyx_k_get_global_max_calc_step_size[] = "get_global_max_calc_step_size";
+static const char __pyx_k_set_global_max_calc_step_size[] = "set_global_max_calc_step_size";
 static const char __pyx_k_get_density_factor_and_mach_for[] = "get_density_factor_and_mach_for_altitude";
+static const char __pyx_k_globalMaxCalcStepSize_have_to_b[] = "_globalMaxCalcStepSize have to be > 0";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0x1a1505e, 0xaee47ca, 0x4420ce0) = (_bc, _curve, _table_data, alt0, ammo, barrel_azimuth, barrel_elevation, calc_step, cant_cosine, cant_sine, diameter, gravity_vector, length, look_angle, muzzle_velocity, sight_height, stability_coefficient, twist, weight))";
 static const char __pyx_k_No_value_specified_for_struct_at[] = "No value specified for struct attribute 'a'";
-static const char __pyx_k_TrajectoryCalc___setstate_cython[] = "TrajectoryCalc.__setstate_cython__";
+static const char __pyx_k_get_global_use_powder_sensitivit[] = "get_global_use_powder_sensitivity";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
-static const char __pyx_k_py_ballisticcalc_exts_trajectory[] = "py_ballisticcalc_exts.trajectory_calc";
+static const char __pyx_k_py_ballisticcalc_exts_trajectory[] = "py_ballisticcalc_exts/trajectory_calc.pyx";
 static const char __pyx_k_py_ballisticcalc_trajectory_data[] = "py_ballisticcalc.trajectory_data";
+static const char __pyx_k_set_global_use_powder_sensitivit[] = "set_global_use_powder_sensitivity value=";
 static const char __pyx_k_No_value_specified_for_struct_at_2[] = "No value specified for struct attribute 'b'";
 static const char __pyx_k_No_value_specified_for_struct_at_3[] = "No value specified for struct attribute 'c'";
-static const char __pyx_k_py_ballisticcalc_exts_trajectory_2[] = "py_ballisticcalc_exts/trajectory_calc.pyx";
+static const char __pyx_k_py_ballisticcalc_exts_trajectory_2[] = "py_ballisticcalc_exts.trajectory_calc";
+static const char __pyx_k_set_global_use_powder_sensitivit_2[] = "set_global_use_powder_sensitivity";
 /* #### Code section: decls ### */
+static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_get_global_max_calc_step_size(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_2get_global_use_powder_sensitivity(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_4set_global_max_calc_step_size(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_value); /* proto */
+static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_6set_global_use_powder_sensitivity(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_value); /* proto */
+static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_8reset_globals(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static int __pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_6Vector___cinit__(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_self, double __pyx_v_x, double __pyx_v_y, double __pyx_v_z); /* proto */
 static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_6Vector_2__add__(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_self, struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_other); /* proto */
 static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_6Vector_4__radd__(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_self, struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_other); /* proto */
 static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_6Vector_6__iadd__(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_self, struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_other); /* proto */
 static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_6Vector_8__sub__(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_self, struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_other); /* proto */
 static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_6Vector_10__rsub__(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_self, struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_other); /* proto */
 static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_6Vector_12__isub__(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_self, struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_other); /* proto */
@@ -2675,15 +2496,15 @@
 static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_6Vector_22__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_6Vector_24__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc___init__(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, PyObject *__pyx_v_ammo); /* proto */
 static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_2zero_angle(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, PyObject *__pyx_v_shot_info, PyObject *__pyx_v_distance); /* proto */
 static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_4trajectory(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, PyObject *__pyx_v_shot_info, PyObject *__pyx_v_max_range, PyObject *__pyx_v_dist_step, PyObject *__pyx_v_extra_data); /* proto */
 static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_6__reduce_cython__(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_8__setstate_cython__(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc___pyx_unpickle_TrajectoryCalc(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_10__pyx_unpickle_TrajectoryCalc(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_21py_ballisticcalc_exts_15trajectory_calc_Vector(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
   PyObject *__pyx_d;
   PyObject *__pyx_b;
@@ -2717,15 +2538,14 @@
   PyObject *__pyx_type_21py_ballisticcalc_exts_15trajectory_calc_Vector;
   PyObject *__pyx_type_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc;
   #endif
   PyTypeObject *__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector;
   PyTypeObject *__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc;
   PyObject *__pyx_n_s_Ammo;
   PyObject *__pyx_n_s_Angular;
-  PyObject *__pyx_n_s_Atmo;
   PyObject *__pyx_n_s_BC;
   PyObject *__pyx_n_s_CD;
   PyObject *__pyx_n_s_Distance;
   PyObject *__pyx_n_s_Energy;
   PyObject *__pyx_n_s_FPS;
   PyObject *__pyx_n_s_Fahrenheit;
   PyObject *__pyx_n_s_Foot;
@@ -2741,78 +2561,69 @@
   PyObject *__pyx_kp_s_No_value_specified_for_struct_at_2;
   PyObject *__pyx_kp_s_No_value_specified_for_struct_at_3;
   PyObject *__pyx_n_s_PickleError;
   PyObject *__pyx_n_s_Pound;
   PyObject *__pyx_n_s_PreferredUnits;
   PyObject *__pyx_n_s_Pressure;
   PyObject *__pyx_n_s_Radian;
-  PyObject *__pyx_n_s_Settings;
   PyObject *__pyx_n_s_Shot;
   PyObject *__pyx_n_s_Temperature;
   PyObject *__pyx_n_s_TrajectoryCalc;
   PyObject *__pyx_n_u_TrajectoryCalc;
-  PyObject *__pyx_n_s_TrajectoryCalc___reduce_cython;
-  PyObject *__pyx_n_s_TrajectoryCalc___setstate_cython;
-  PyObject *__pyx_n_s_TrajectoryCalc_trajectory;
-  PyObject *__pyx_n_s_TrajectoryCalc_zero_angle;
   PyObject *__pyx_n_s_TrajectoryData;
   PyObject *__pyx_n_s_TypeError;
-  PyObject *__pyx_n_s_USE_POWDER_SENSITIVITY;
   PyObject *__pyx_n_s_ValueError;
   PyObject *__pyx_n_s_Vector;
-  PyObject *__pyx_n_s_Vector___reduce_cython;
-  PyObject *__pyx_n_s_Vector___setstate_cython;
   PyObject *__pyx_n_s_Velocity;
   PyObject *__pyx_n_s_Weight;
   PyObject *__pyx_n_s_Wind;
   PyObject *__pyx_kp_u_Zero_vertical_error;
-  PyObject *__pyx_n_s__23;
-  PyObject *__pyx_kp_u__6;
-  PyObject *__pyx_n_s__7;
+  PyObject *__pyx_n_s__20;
+  PyObject *__pyx_kp_u__7;
+  PyObject *__pyx_n_s__8;
   PyObject *__pyx_n_s_a;
   PyObject *__pyx_n_s_all;
   PyObject *__pyx_n_s_altitude;
   PyObject *__pyx_n_s_ammo;
   PyObject *__pyx_n_s_angle;
-  PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_atmo;
   PyObject *__pyx_n_s_b;
   PyObject *__pyx_n_s_barrel_azimuth;
   PyObject *__pyx_n_s_barrel_elevation;
-  PyObject *__pyx_n_s_bool;
   PyObject *__pyx_n_s_c;
   PyObject *__pyx_n_s_cant_angle;
-  PyObject *__pyx_n_s_class_getitem;
   PyObject *__pyx_n_s_cline_in_traceback;
   PyObject *__pyx_n_s_density_factor;
   PyObject *__pyx_n_s_diameter;
   PyObject *__pyx_n_s_dict;
-  PyObject *__pyx_n_s_dict_2;
   PyObject *__pyx_n_s_direction_from;
   PyObject *__pyx_kp_u_disable;
   PyObject *__pyx_n_s_dist_step;
   PyObject *__pyx_n_s_distance;
   PyObject *__pyx_n_s_dm;
   PyObject *__pyx_n_s_drag;
   PyObject *__pyx_n_s_drag_table;
   PyObject *__pyx_n_s_drop_adj;
   PyObject *__pyx_kp_u_enable;
   PyObject *__pyx_n_s_energy;
   PyObject *__pyx_n_s_extra_data;
   PyObject *__pyx_kp_u_feet_after;
-  PyObject *__pyx_n_s_filter_flags;
   PyObject *__pyx_n_s_flag;
   PyObject *__pyx_kp_u_gc;
   PyObject *__pyx_n_s_get_density_factor_and_mach_for;
-  PyObject *__pyx_n_s_get_max_calc_step_size;
+  PyObject *__pyx_n_s_get_global_max_calc_step_size;
+  PyObject *__pyx_n_u_get_global_max_calc_step_size;
+  PyObject *__pyx_n_s_get_global_use_powder_sensitivit;
+  PyObject *__pyx_n_u_get_global_use_powder_sensitivit;
   PyObject *__pyx_n_s_get_velocity_for_temp;
   PyObject *__pyx_n_s_getstate;
+  PyObject *__pyx_kp_u_globalMaxCalcStepSize_have_to_b;
   PyObject *__pyx_n_s_height;
   PyObject *__pyx_n_s_import;
-  PyObject *__pyx_n_s_is_coroutine;
+  PyObject *__pyx_kp_u_is_not_a_boolean;
   PyObject *__pyx_kp_u_isenabled;
   PyObject *__pyx_kp_u_iterations;
   PyObject *__pyx_n_s_length;
   PyObject *__pyx_n_s_look_angle;
   PyObject *__pyx_n_s_look_distance;
   PyObject *__pyx_n_s_mach;
   PyObject *__pyx_n_s_main;
@@ -2822,89 +2633,88 @@
   PyObject *__pyx_n_s_name;
   PyObject *__pyx_n_s_new;
   PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
   PyObject *__pyx_n_s_ogw;
   PyObject *__pyx_n_s_pickle;
   PyObject *__pyx_n_s_pressure;
   PyObject *__pyx_n_s_py_ballisticcalc_conditions;
-  PyObject *__pyx_n_s_py_ballisticcalc_exts_trajectory;
-  PyObject *__pyx_kp_s_py_ballisticcalc_exts_trajectory_2;
+  PyObject *__pyx_kp_s_py_ballisticcalc_exts_trajectory;
+  PyObject *__pyx_n_s_py_ballisticcalc_exts_trajectory_2;
   PyObject *__pyx_n_s_py_ballisticcalc_munition;
-  PyObject *__pyx_n_s_py_ballisticcalc_settings;
   PyObject *__pyx_n_s_py_ballisticcalc_trajectory_data;
   PyObject *__pyx_n_s_py_ballisticcalc_unit;
   PyObject *__pyx_n_s_pyx_PickleError;
   PyObject *__pyx_n_s_pyx_checksum;
   PyObject *__pyx_n_s_pyx_result;
   PyObject *__pyx_n_s_pyx_state;
   PyObject *__pyx_n_s_pyx_type;
   PyObject *__pyx_n_s_pyx_unpickle_TrajectoryCalc;
   PyObject *__pyx_n_s_pyx_vtable;
   PyObject *__pyx_n_s_range;
+  PyObject *__pyx_n_s_raw_value;
   PyObject *__pyx_n_s_reduce;
   PyObject *__pyx_n_s_reduce_cython;
   PyObject *__pyx_n_s_reduce_ex;
-  PyObject *__pyx_n_s_self;
+  PyObject *__pyx_n_s_reset_globals;
+  PyObject *__pyx_n_u_reset_globals;
+  PyObject *__pyx_n_s_set_global_max_calc_step_size;
+  PyObject *__pyx_n_u_set_global_max_calc_step_size;
+  PyObject *__pyx_kp_u_set_global_use_powder_sensitivit;
+  PyObject *__pyx_n_s_set_global_use_powder_sensitivit_2;
+  PyObject *__pyx_n_u_set_global_use_powder_sensitivit_2;
   PyObject *__pyx_n_s_setstate;
   PyObject *__pyx_n_s_setstate_cython;
   PyObject *__pyx_n_s_shot_info;
   PyObject *__pyx_n_s_sight_height;
-  PyObject *__pyx_n_s_state;
-  PyObject *__pyx_n_s_step;
   PyObject *__pyx_kp_s_stringsource;
   PyObject *__pyx_n_s_target_drop;
   PyObject *__pyx_n_s_temperature;
   PyObject *__pyx_n_s_test;
   PyObject *__pyx_n_s_time;
-  PyObject *__pyx_n_s_trajectory;
   PyObject *__pyx_n_s_twist;
   PyObject *__pyx_n_s_until_distance;
   PyObject *__pyx_n_s_update;
-  PyObject *__pyx_n_s_use_setstate;
+  PyObject *__pyx_n_s_value;
+  PyObject *__pyx_n_s_value_2;
   PyObject *__pyx_n_s_velocity;
   PyObject *__pyx_n_s_weapon;
   PyObject *__pyx_n_s_weight;
   PyObject *__pyx_n_s_windage;
   PyObject *__pyx_n_s_windage_adj;
   PyObject *__pyx_n_s_winds;
   PyObject *__pyx_n_s_x;
   PyObject *__pyx_n_s_y;
   PyObject *__pyx_n_s_z;
-  PyObject *__pyx_n_s_zero_angle;
   PyObject *__pyx_float__0;
   PyObject *__pyx_float_0_;
   PyObject *__pyx_float_0_0;
   PyObject *__pyx_float_0_2;
-  PyObject *__pyx_float_2_0;
+  PyObject *__pyx_float_0_5;
+  PyObject *__pyx_int_0;
   PyObject *__pyx_int_1;
-  PyObject *__pyx_int_12;
   PyObject *__pyx_int_27349086;
   PyObject *__pyx_int_71437536;
   PyObject *__pyx_int_183388106;
-  PyObject *__pyx_int_neg_1;
   PyObject *__pyx_tuple_;
   PyObject *__pyx_tuple__2;
   PyObject *__pyx_tuple__3;
   PyObject *__pyx_tuple__4;
   PyObject *__pyx_tuple__5;
-  PyObject *__pyx_tuple__8;
+  PyObject *__pyx_tuple__6;
   PyObject *__pyx_tuple__9;
-  PyObject *__pyx_tuple__11;
+  PyObject *__pyx_tuple__10;
   PyObject *__pyx_tuple__13;
   PyObject *__pyx_tuple__15;
-  PyObject *__pyx_tuple__17;
   PyObject *__pyx_tuple__18;
-  PyObject *__pyx_tuple__21;
-  PyObject *__pyx_codeobj__10;
+  PyObject *__pyx_codeobj__11;
   PyObject *__pyx_codeobj__12;
   PyObject *__pyx_codeobj__14;
   PyObject *__pyx_codeobj__16;
+  PyObject *__pyx_codeobj__17;
   PyObject *__pyx_codeobj__19;
-  PyObject *__pyx_codeobj__20;
-  PyObject *__pyx_codeobj__22;
 } __pyx_mstate;
 
 #if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
 namespace {
   extern struct PyModuleDef __pyx_moduledef;
 } /* anonymous namespace */
@@ -2945,15 +2755,14 @@
   #endif
   Py_CLEAR(clear_module_state->__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector);
   Py_CLEAR(clear_module_state->__pyx_type_21py_ballisticcalc_exts_15trajectory_calc_Vector);
   Py_CLEAR(clear_module_state->__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc);
   Py_CLEAR(clear_module_state->__pyx_type_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc);
   Py_CLEAR(clear_module_state->__pyx_n_s_Ammo);
   Py_CLEAR(clear_module_state->__pyx_n_s_Angular);
-  Py_CLEAR(clear_module_state->__pyx_n_s_Atmo);
   Py_CLEAR(clear_module_state->__pyx_n_s_BC);
   Py_CLEAR(clear_module_state->__pyx_n_s_CD);
   Py_CLEAR(clear_module_state->__pyx_n_s_Distance);
   Py_CLEAR(clear_module_state->__pyx_n_s_Energy);
   Py_CLEAR(clear_module_state->__pyx_n_s_FPS);
   Py_CLEAR(clear_module_state->__pyx_n_s_Fahrenheit);
   Py_CLEAR(clear_module_state->__pyx_n_s_Foot);
@@ -2969,78 +2778,69 @@
   Py_CLEAR(clear_module_state->__pyx_kp_s_No_value_specified_for_struct_at_2);
   Py_CLEAR(clear_module_state->__pyx_kp_s_No_value_specified_for_struct_at_3);
   Py_CLEAR(clear_module_state->__pyx_n_s_PickleError);
   Py_CLEAR(clear_module_state->__pyx_n_s_Pound);
   Py_CLEAR(clear_module_state->__pyx_n_s_PreferredUnits);
   Py_CLEAR(clear_module_state->__pyx_n_s_Pressure);
   Py_CLEAR(clear_module_state->__pyx_n_s_Radian);
-  Py_CLEAR(clear_module_state->__pyx_n_s_Settings);
   Py_CLEAR(clear_module_state->__pyx_n_s_Shot);
   Py_CLEAR(clear_module_state->__pyx_n_s_Temperature);
   Py_CLEAR(clear_module_state->__pyx_n_s_TrajectoryCalc);
   Py_CLEAR(clear_module_state->__pyx_n_u_TrajectoryCalc);
-  Py_CLEAR(clear_module_state->__pyx_n_s_TrajectoryCalc___reduce_cython);
-  Py_CLEAR(clear_module_state->__pyx_n_s_TrajectoryCalc___setstate_cython);
-  Py_CLEAR(clear_module_state->__pyx_n_s_TrajectoryCalc_trajectory);
-  Py_CLEAR(clear_module_state->__pyx_n_s_TrajectoryCalc_zero_angle);
   Py_CLEAR(clear_module_state->__pyx_n_s_TrajectoryData);
   Py_CLEAR(clear_module_state->__pyx_n_s_TypeError);
-  Py_CLEAR(clear_module_state->__pyx_n_s_USE_POWDER_SENSITIVITY);
   Py_CLEAR(clear_module_state->__pyx_n_s_ValueError);
   Py_CLEAR(clear_module_state->__pyx_n_s_Vector);
-  Py_CLEAR(clear_module_state->__pyx_n_s_Vector___reduce_cython);
-  Py_CLEAR(clear_module_state->__pyx_n_s_Vector___setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_Velocity);
   Py_CLEAR(clear_module_state->__pyx_n_s_Weight);
   Py_CLEAR(clear_module_state->__pyx_n_s_Wind);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Zero_vertical_error);
-  Py_CLEAR(clear_module_state->__pyx_n_s__23);
-  Py_CLEAR(clear_module_state->__pyx_kp_u__6);
-  Py_CLEAR(clear_module_state->__pyx_n_s__7);
+  Py_CLEAR(clear_module_state->__pyx_n_s__20);
+  Py_CLEAR(clear_module_state->__pyx_kp_u__7);
+  Py_CLEAR(clear_module_state->__pyx_n_s__8);
   Py_CLEAR(clear_module_state->__pyx_n_s_a);
   Py_CLEAR(clear_module_state->__pyx_n_s_all);
   Py_CLEAR(clear_module_state->__pyx_n_s_altitude);
   Py_CLEAR(clear_module_state->__pyx_n_s_ammo);
   Py_CLEAR(clear_module_state->__pyx_n_s_angle);
-  Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_atmo);
   Py_CLEAR(clear_module_state->__pyx_n_s_b);
   Py_CLEAR(clear_module_state->__pyx_n_s_barrel_azimuth);
   Py_CLEAR(clear_module_state->__pyx_n_s_barrel_elevation);
-  Py_CLEAR(clear_module_state->__pyx_n_s_bool);
   Py_CLEAR(clear_module_state->__pyx_n_s_c);
   Py_CLEAR(clear_module_state->__pyx_n_s_cant_angle);
-  Py_CLEAR(clear_module_state->__pyx_n_s_class_getitem);
   Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
   Py_CLEAR(clear_module_state->__pyx_n_s_density_factor);
   Py_CLEAR(clear_module_state->__pyx_n_s_diameter);
   Py_CLEAR(clear_module_state->__pyx_n_s_dict);
-  Py_CLEAR(clear_module_state->__pyx_n_s_dict_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_direction_from);
   Py_CLEAR(clear_module_state->__pyx_kp_u_disable);
   Py_CLEAR(clear_module_state->__pyx_n_s_dist_step);
   Py_CLEAR(clear_module_state->__pyx_n_s_distance);
   Py_CLEAR(clear_module_state->__pyx_n_s_dm);
   Py_CLEAR(clear_module_state->__pyx_n_s_drag);
   Py_CLEAR(clear_module_state->__pyx_n_s_drag_table);
   Py_CLEAR(clear_module_state->__pyx_n_s_drop_adj);
   Py_CLEAR(clear_module_state->__pyx_kp_u_enable);
   Py_CLEAR(clear_module_state->__pyx_n_s_energy);
   Py_CLEAR(clear_module_state->__pyx_n_s_extra_data);
   Py_CLEAR(clear_module_state->__pyx_kp_u_feet_after);
-  Py_CLEAR(clear_module_state->__pyx_n_s_filter_flags);
   Py_CLEAR(clear_module_state->__pyx_n_s_flag);
   Py_CLEAR(clear_module_state->__pyx_kp_u_gc);
   Py_CLEAR(clear_module_state->__pyx_n_s_get_density_factor_and_mach_for);
-  Py_CLEAR(clear_module_state->__pyx_n_s_get_max_calc_step_size);
+  Py_CLEAR(clear_module_state->__pyx_n_s_get_global_max_calc_step_size);
+  Py_CLEAR(clear_module_state->__pyx_n_u_get_global_max_calc_step_size);
+  Py_CLEAR(clear_module_state->__pyx_n_s_get_global_use_powder_sensitivit);
+  Py_CLEAR(clear_module_state->__pyx_n_u_get_global_use_powder_sensitivit);
   Py_CLEAR(clear_module_state->__pyx_n_s_get_velocity_for_temp);
   Py_CLEAR(clear_module_state->__pyx_n_s_getstate);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_globalMaxCalcStepSize_have_to_b);
   Py_CLEAR(clear_module_state->__pyx_n_s_height);
   Py_CLEAR(clear_module_state->__pyx_n_s_import);
-  Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_is_not_a_boolean);
   Py_CLEAR(clear_module_state->__pyx_kp_u_isenabled);
   Py_CLEAR(clear_module_state->__pyx_kp_u_iterations);
   Py_CLEAR(clear_module_state->__pyx_n_s_length);
   Py_CLEAR(clear_module_state->__pyx_n_s_look_angle);
   Py_CLEAR(clear_module_state->__pyx_n_s_look_distance);
   Py_CLEAR(clear_module_state->__pyx_n_s_mach);
   Py_CLEAR(clear_module_state->__pyx_n_s_main);
@@ -3050,89 +2850,88 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_new);
   Py_CLEAR(clear_module_state->__pyx_kp_s_no_default___reduce___due_to_non);
   Py_CLEAR(clear_module_state->__pyx_n_s_ogw);
   Py_CLEAR(clear_module_state->__pyx_n_s_pickle);
   Py_CLEAR(clear_module_state->__pyx_n_s_pressure);
   Py_CLEAR(clear_module_state->__pyx_n_s_py_ballisticcalc_conditions);
-  Py_CLEAR(clear_module_state->__pyx_n_s_py_ballisticcalc_exts_trajectory);
-  Py_CLEAR(clear_module_state->__pyx_kp_s_py_ballisticcalc_exts_trajectory_2);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_py_ballisticcalc_exts_trajectory);
+  Py_CLEAR(clear_module_state->__pyx_n_s_py_ballisticcalc_exts_trajectory_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_py_ballisticcalc_munition);
-  Py_CLEAR(clear_module_state->__pyx_n_s_py_ballisticcalc_settings);
   Py_CLEAR(clear_module_state->__pyx_n_s_py_ballisticcalc_trajectory_data);
   Py_CLEAR(clear_module_state->__pyx_n_s_py_ballisticcalc_unit);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_PickleError);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_checksum);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_result);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_state);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_type);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_unpickle_TrajectoryCalc);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_vtable);
   Py_CLEAR(clear_module_state->__pyx_n_s_range);
+  Py_CLEAR(clear_module_state->__pyx_n_s_raw_value);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce_ex);
-  Py_CLEAR(clear_module_state->__pyx_n_s_self);
+  Py_CLEAR(clear_module_state->__pyx_n_s_reset_globals);
+  Py_CLEAR(clear_module_state->__pyx_n_u_reset_globals);
+  Py_CLEAR(clear_module_state->__pyx_n_s_set_global_max_calc_step_size);
+  Py_CLEAR(clear_module_state->__pyx_n_u_set_global_max_calc_step_size);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_set_global_use_powder_sensitivit);
+  Py_CLEAR(clear_module_state->__pyx_n_s_set_global_use_powder_sensitivit_2);
+  Py_CLEAR(clear_module_state->__pyx_n_u_set_global_use_powder_sensitivit_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_shot_info);
   Py_CLEAR(clear_module_state->__pyx_n_s_sight_height);
-  Py_CLEAR(clear_module_state->__pyx_n_s_state);
-  Py_CLEAR(clear_module_state->__pyx_n_s_step);
   Py_CLEAR(clear_module_state->__pyx_kp_s_stringsource);
   Py_CLEAR(clear_module_state->__pyx_n_s_target_drop);
   Py_CLEAR(clear_module_state->__pyx_n_s_temperature);
   Py_CLEAR(clear_module_state->__pyx_n_s_test);
   Py_CLEAR(clear_module_state->__pyx_n_s_time);
-  Py_CLEAR(clear_module_state->__pyx_n_s_trajectory);
   Py_CLEAR(clear_module_state->__pyx_n_s_twist);
   Py_CLEAR(clear_module_state->__pyx_n_s_until_distance);
   Py_CLEAR(clear_module_state->__pyx_n_s_update);
-  Py_CLEAR(clear_module_state->__pyx_n_s_use_setstate);
+  Py_CLEAR(clear_module_state->__pyx_n_s_value);
+  Py_CLEAR(clear_module_state->__pyx_n_s_value_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_velocity);
   Py_CLEAR(clear_module_state->__pyx_n_s_weapon);
   Py_CLEAR(clear_module_state->__pyx_n_s_weight);
   Py_CLEAR(clear_module_state->__pyx_n_s_windage);
   Py_CLEAR(clear_module_state->__pyx_n_s_windage_adj);
   Py_CLEAR(clear_module_state->__pyx_n_s_winds);
   Py_CLEAR(clear_module_state->__pyx_n_s_x);
   Py_CLEAR(clear_module_state->__pyx_n_s_y);
   Py_CLEAR(clear_module_state->__pyx_n_s_z);
-  Py_CLEAR(clear_module_state->__pyx_n_s_zero_angle);
   Py_CLEAR(clear_module_state->__pyx_float__0);
   Py_CLEAR(clear_module_state->__pyx_float_0_);
   Py_CLEAR(clear_module_state->__pyx_float_0_0);
   Py_CLEAR(clear_module_state->__pyx_float_0_2);
-  Py_CLEAR(clear_module_state->__pyx_float_2_0);
+  Py_CLEAR(clear_module_state->__pyx_float_0_5);
+  Py_CLEAR(clear_module_state->__pyx_int_0);
   Py_CLEAR(clear_module_state->__pyx_int_1);
-  Py_CLEAR(clear_module_state->__pyx_int_12);
   Py_CLEAR(clear_module_state->__pyx_int_27349086);
   Py_CLEAR(clear_module_state->__pyx_int_71437536);
   Py_CLEAR(clear_module_state->__pyx_int_183388106);
-  Py_CLEAR(clear_module_state->__pyx_int_neg_1);
   Py_CLEAR(clear_module_state->__pyx_tuple_);
   Py_CLEAR(clear_module_state->__pyx_tuple__2);
   Py_CLEAR(clear_module_state->__pyx_tuple__3);
   Py_CLEAR(clear_module_state->__pyx_tuple__4);
   Py_CLEAR(clear_module_state->__pyx_tuple__5);
-  Py_CLEAR(clear_module_state->__pyx_tuple__8);
+  Py_CLEAR(clear_module_state->__pyx_tuple__6);
   Py_CLEAR(clear_module_state->__pyx_tuple__9);
-  Py_CLEAR(clear_module_state->__pyx_tuple__11);
+  Py_CLEAR(clear_module_state->__pyx_tuple__10);
   Py_CLEAR(clear_module_state->__pyx_tuple__13);
   Py_CLEAR(clear_module_state->__pyx_tuple__15);
-  Py_CLEAR(clear_module_state->__pyx_tuple__17);
   Py_CLEAR(clear_module_state->__pyx_tuple__18);
-  Py_CLEAR(clear_module_state->__pyx_tuple__21);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__10);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__11);
   Py_CLEAR(clear_module_state->__pyx_codeobj__12);
   Py_CLEAR(clear_module_state->__pyx_codeobj__14);
   Py_CLEAR(clear_module_state->__pyx_codeobj__16);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__17);
   Py_CLEAR(clear_module_state->__pyx_codeobj__19);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__20);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__22);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
 #if CYTHON_USE_MODULE_STATE
 static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
   __pyx_mstate *traverse_module_state = __pyx_mstate(m);
@@ -3151,15 +2950,14 @@
   #endif
   Py_VISIT(traverse_module_state->__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector);
   Py_VISIT(traverse_module_state->__pyx_type_21py_ballisticcalc_exts_15trajectory_calc_Vector);
   Py_VISIT(traverse_module_state->__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc);
   Py_VISIT(traverse_module_state->__pyx_type_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc);
   Py_VISIT(traverse_module_state->__pyx_n_s_Ammo);
   Py_VISIT(traverse_module_state->__pyx_n_s_Angular);
-  Py_VISIT(traverse_module_state->__pyx_n_s_Atmo);
   Py_VISIT(traverse_module_state->__pyx_n_s_BC);
   Py_VISIT(traverse_module_state->__pyx_n_s_CD);
   Py_VISIT(traverse_module_state->__pyx_n_s_Distance);
   Py_VISIT(traverse_module_state->__pyx_n_s_Energy);
   Py_VISIT(traverse_module_state->__pyx_n_s_FPS);
   Py_VISIT(traverse_module_state->__pyx_n_s_Fahrenheit);
   Py_VISIT(traverse_module_state->__pyx_n_s_Foot);
@@ -3175,78 +2973,69 @@
   Py_VISIT(traverse_module_state->__pyx_kp_s_No_value_specified_for_struct_at_2);
   Py_VISIT(traverse_module_state->__pyx_kp_s_No_value_specified_for_struct_at_3);
   Py_VISIT(traverse_module_state->__pyx_n_s_PickleError);
   Py_VISIT(traverse_module_state->__pyx_n_s_Pound);
   Py_VISIT(traverse_module_state->__pyx_n_s_PreferredUnits);
   Py_VISIT(traverse_module_state->__pyx_n_s_Pressure);
   Py_VISIT(traverse_module_state->__pyx_n_s_Radian);
-  Py_VISIT(traverse_module_state->__pyx_n_s_Settings);
   Py_VISIT(traverse_module_state->__pyx_n_s_Shot);
   Py_VISIT(traverse_module_state->__pyx_n_s_Temperature);
   Py_VISIT(traverse_module_state->__pyx_n_s_TrajectoryCalc);
   Py_VISIT(traverse_module_state->__pyx_n_u_TrajectoryCalc);
-  Py_VISIT(traverse_module_state->__pyx_n_s_TrajectoryCalc___reduce_cython);
-  Py_VISIT(traverse_module_state->__pyx_n_s_TrajectoryCalc___setstate_cython);
-  Py_VISIT(traverse_module_state->__pyx_n_s_TrajectoryCalc_trajectory);
-  Py_VISIT(traverse_module_state->__pyx_n_s_TrajectoryCalc_zero_angle);
   Py_VISIT(traverse_module_state->__pyx_n_s_TrajectoryData);
   Py_VISIT(traverse_module_state->__pyx_n_s_TypeError);
-  Py_VISIT(traverse_module_state->__pyx_n_s_USE_POWDER_SENSITIVITY);
   Py_VISIT(traverse_module_state->__pyx_n_s_ValueError);
   Py_VISIT(traverse_module_state->__pyx_n_s_Vector);
-  Py_VISIT(traverse_module_state->__pyx_n_s_Vector___reduce_cython);
-  Py_VISIT(traverse_module_state->__pyx_n_s_Vector___setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_Velocity);
   Py_VISIT(traverse_module_state->__pyx_n_s_Weight);
   Py_VISIT(traverse_module_state->__pyx_n_s_Wind);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Zero_vertical_error);
-  Py_VISIT(traverse_module_state->__pyx_n_s__23);
-  Py_VISIT(traverse_module_state->__pyx_kp_u__6);
-  Py_VISIT(traverse_module_state->__pyx_n_s__7);
+  Py_VISIT(traverse_module_state->__pyx_n_s__20);
+  Py_VISIT(traverse_module_state->__pyx_kp_u__7);
+  Py_VISIT(traverse_module_state->__pyx_n_s__8);
   Py_VISIT(traverse_module_state->__pyx_n_s_a);
   Py_VISIT(traverse_module_state->__pyx_n_s_all);
   Py_VISIT(traverse_module_state->__pyx_n_s_altitude);
   Py_VISIT(traverse_module_state->__pyx_n_s_ammo);
   Py_VISIT(traverse_module_state->__pyx_n_s_angle);
-  Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_atmo);
   Py_VISIT(traverse_module_state->__pyx_n_s_b);
   Py_VISIT(traverse_module_state->__pyx_n_s_barrel_azimuth);
   Py_VISIT(traverse_module_state->__pyx_n_s_barrel_elevation);
-  Py_VISIT(traverse_module_state->__pyx_n_s_bool);
   Py_VISIT(traverse_module_state->__pyx_n_s_c);
   Py_VISIT(traverse_module_state->__pyx_n_s_cant_angle);
-  Py_VISIT(traverse_module_state->__pyx_n_s_class_getitem);
   Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
   Py_VISIT(traverse_module_state->__pyx_n_s_density_factor);
   Py_VISIT(traverse_module_state->__pyx_n_s_diameter);
   Py_VISIT(traverse_module_state->__pyx_n_s_dict);
-  Py_VISIT(traverse_module_state->__pyx_n_s_dict_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_direction_from);
   Py_VISIT(traverse_module_state->__pyx_kp_u_disable);
   Py_VISIT(traverse_module_state->__pyx_n_s_dist_step);
   Py_VISIT(traverse_module_state->__pyx_n_s_distance);
   Py_VISIT(traverse_module_state->__pyx_n_s_dm);
   Py_VISIT(traverse_module_state->__pyx_n_s_drag);
   Py_VISIT(traverse_module_state->__pyx_n_s_drag_table);
   Py_VISIT(traverse_module_state->__pyx_n_s_drop_adj);
   Py_VISIT(traverse_module_state->__pyx_kp_u_enable);
   Py_VISIT(traverse_module_state->__pyx_n_s_energy);
   Py_VISIT(traverse_module_state->__pyx_n_s_extra_data);
   Py_VISIT(traverse_module_state->__pyx_kp_u_feet_after);
-  Py_VISIT(traverse_module_state->__pyx_n_s_filter_flags);
   Py_VISIT(traverse_module_state->__pyx_n_s_flag);
   Py_VISIT(traverse_module_state->__pyx_kp_u_gc);
   Py_VISIT(traverse_module_state->__pyx_n_s_get_density_factor_and_mach_for);
-  Py_VISIT(traverse_module_state->__pyx_n_s_get_max_calc_step_size);
+  Py_VISIT(traverse_module_state->__pyx_n_s_get_global_max_calc_step_size);
+  Py_VISIT(traverse_module_state->__pyx_n_u_get_global_max_calc_step_size);
+  Py_VISIT(traverse_module_state->__pyx_n_s_get_global_use_powder_sensitivit);
+  Py_VISIT(traverse_module_state->__pyx_n_u_get_global_use_powder_sensitivit);
   Py_VISIT(traverse_module_state->__pyx_n_s_get_velocity_for_temp);
   Py_VISIT(traverse_module_state->__pyx_n_s_getstate);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_globalMaxCalcStepSize_have_to_b);
   Py_VISIT(traverse_module_state->__pyx_n_s_height);
   Py_VISIT(traverse_module_state->__pyx_n_s_import);
-  Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_is_not_a_boolean);
   Py_VISIT(traverse_module_state->__pyx_kp_u_isenabled);
   Py_VISIT(traverse_module_state->__pyx_kp_u_iterations);
   Py_VISIT(traverse_module_state->__pyx_n_s_length);
   Py_VISIT(traverse_module_state->__pyx_n_s_look_angle);
   Py_VISIT(traverse_module_state->__pyx_n_s_look_distance);
   Py_VISIT(traverse_module_state->__pyx_n_s_mach);
   Py_VISIT(traverse_module_state->__pyx_n_s_main);
@@ -3256,89 +3045,88 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_new);
   Py_VISIT(traverse_module_state->__pyx_kp_s_no_default___reduce___due_to_non);
   Py_VISIT(traverse_module_state->__pyx_n_s_ogw);
   Py_VISIT(traverse_module_state->__pyx_n_s_pickle);
   Py_VISIT(traverse_module_state->__pyx_n_s_pressure);
   Py_VISIT(traverse_module_state->__pyx_n_s_py_ballisticcalc_conditions);
-  Py_VISIT(traverse_module_state->__pyx_n_s_py_ballisticcalc_exts_trajectory);
-  Py_VISIT(traverse_module_state->__pyx_kp_s_py_ballisticcalc_exts_trajectory_2);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_py_ballisticcalc_exts_trajectory);
+  Py_VISIT(traverse_module_state->__pyx_n_s_py_ballisticcalc_exts_trajectory_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_py_ballisticcalc_munition);
-  Py_VISIT(traverse_module_state->__pyx_n_s_py_ballisticcalc_settings);
   Py_VISIT(traverse_module_state->__pyx_n_s_py_ballisticcalc_trajectory_data);
   Py_VISIT(traverse_module_state->__pyx_n_s_py_ballisticcalc_unit);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_PickleError);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_checksum);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_result);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_state);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_type);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_unpickle_TrajectoryCalc);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_vtable);
   Py_VISIT(traverse_module_state->__pyx_n_s_range);
+  Py_VISIT(traverse_module_state->__pyx_n_s_raw_value);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce_ex);
-  Py_VISIT(traverse_module_state->__pyx_n_s_self);
+  Py_VISIT(traverse_module_state->__pyx_n_s_reset_globals);
+  Py_VISIT(traverse_module_state->__pyx_n_u_reset_globals);
+  Py_VISIT(traverse_module_state->__pyx_n_s_set_global_max_calc_step_size);
+  Py_VISIT(traverse_module_state->__pyx_n_u_set_global_max_calc_step_size);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_set_global_use_powder_sensitivit);
+  Py_VISIT(traverse_module_state->__pyx_n_s_set_global_use_powder_sensitivit_2);
+  Py_VISIT(traverse_module_state->__pyx_n_u_set_global_use_powder_sensitivit_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_shot_info);
   Py_VISIT(traverse_module_state->__pyx_n_s_sight_height);
-  Py_VISIT(traverse_module_state->__pyx_n_s_state);
-  Py_VISIT(traverse_module_state->__pyx_n_s_step);
   Py_VISIT(traverse_module_state->__pyx_kp_s_stringsource);
   Py_VISIT(traverse_module_state->__pyx_n_s_target_drop);
   Py_VISIT(traverse_module_state->__pyx_n_s_temperature);
   Py_VISIT(traverse_module_state->__pyx_n_s_test);
   Py_VISIT(traverse_module_state->__pyx_n_s_time);
-  Py_VISIT(traverse_module_state->__pyx_n_s_trajectory);
   Py_VISIT(traverse_module_state->__pyx_n_s_twist);
   Py_VISIT(traverse_module_state->__pyx_n_s_until_distance);
   Py_VISIT(traverse_module_state->__pyx_n_s_update);
-  Py_VISIT(traverse_module_state->__pyx_n_s_use_setstate);
+  Py_VISIT(traverse_module_state->__pyx_n_s_value);
+  Py_VISIT(traverse_module_state->__pyx_n_s_value_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_velocity);
   Py_VISIT(traverse_module_state->__pyx_n_s_weapon);
   Py_VISIT(traverse_module_state->__pyx_n_s_weight);
   Py_VISIT(traverse_module_state->__pyx_n_s_windage);
   Py_VISIT(traverse_module_state->__pyx_n_s_windage_adj);
   Py_VISIT(traverse_module_state->__pyx_n_s_winds);
   Py_VISIT(traverse_module_state->__pyx_n_s_x);
   Py_VISIT(traverse_module_state->__pyx_n_s_y);
   Py_VISIT(traverse_module_state->__pyx_n_s_z);
-  Py_VISIT(traverse_module_state->__pyx_n_s_zero_angle);
   Py_VISIT(traverse_module_state->__pyx_float__0);
   Py_VISIT(traverse_module_state->__pyx_float_0_);
   Py_VISIT(traverse_module_state->__pyx_float_0_0);
   Py_VISIT(traverse_module_state->__pyx_float_0_2);
-  Py_VISIT(traverse_module_state->__pyx_float_2_0);
+  Py_VISIT(traverse_module_state->__pyx_float_0_5);
+  Py_VISIT(traverse_module_state->__pyx_int_0);
   Py_VISIT(traverse_module_state->__pyx_int_1);
-  Py_VISIT(traverse_module_state->__pyx_int_12);
   Py_VISIT(traverse_module_state->__pyx_int_27349086);
   Py_VISIT(traverse_module_state->__pyx_int_71437536);
   Py_VISIT(traverse_module_state->__pyx_int_183388106);
-  Py_VISIT(traverse_module_state->__pyx_int_neg_1);
   Py_VISIT(traverse_module_state->__pyx_tuple_);
   Py_VISIT(traverse_module_state->__pyx_tuple__2);
   Py_VISIT(traverse_module_state->__pyx_tuple__3);
   Py_VISIT(traverse_module_state->__pyx_tuple__4);
   Py_VISIT(traverse_module_state->__pyx_tuple__5);
-  Py_VISIT(traverse_module_state->__pyx_tuple__8);
+  Py_VISIT(traverse_module_state->__pyx_tuple__6);
   Py_VISIT(traverse_module_state->__pyx_tuple__9);
-  Py_VISIT(traverse_module_state->__pyx_tuple__11);
+  Py_VISIT(traverse_module_state->__pyx_tuple__10);
   Py_VISIT(traverse_module_state->__pyx_tuple__13);
   Py_VISIT(traverse_module_state->__pyx_tuple__15);
-  Py_VISIT(traverse_module_state->__pyx_tuple__17);
   Py_VISIT(traverse_module_state->__pyx_tuple__18);
-  Py_VISIT(traverse_module_state->__pyx_tuple__21);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__10);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__11);
   Py_VISIT(traverse_module_state->__pyx_codeobj__12);
   Py_VISIT(traverse_module_state->__pyx_codeobj__14);
   Py_VISIT(traverse_module_state->__pyx_codeobj__16);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__17);
   Py_VISIT(traverse_module_state->__pyx_codeobj__19);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__20);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__22);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
 #define __pyx_d __pyx_mstate_global->__pyx_d
 #define __pyx_b __pyx_mstate_global->__pyx_b
 #define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
@@ -3371,15 +3159,14 @@
 #define __pyx_type_21py_ballisticcalc_exts_15trajectory_calc_Vector __pyx_mstate_global->__pyx_type_21py_ballisticcalc_exts_15trajectory_calc_Vector
 #define __pyx_type_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc __pyx_mstate_global->__pyx_type_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc
 #endif
 #define __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector __pyx_mstate_global->__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector
 #define __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc __pyx_mstate_global->__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc
 #define __pyx_n_s_Ammo __pyx_mstate_global->__pyx_n_s_Ammo
 #define __pyx_n_s_Angular __pyx_mstate_global->__pyx_n_s_Angular
-#define __pyx_n_s_Atmo __pyx_mstate_global->__pyx_n_s_Atmo
 #define __pyx_n_s_BC __pyx_mstate_global->__pyx_n_s_BC
 #define __pyx_n_s_CD __pyx_mstate_global->__pyx_n_s_CD
 #define __pyx_n_s_Distance __pyx_mstate_global->__pyx_n_s_Distance
 #define __pyx_n_s_Energy __pyx_mstate_global->__pyx_n_s_Energy
 #define __pyx_n_s_FPS __pyx_mstate_global->__pyx_n_s_FPS
 #define __pyx_n_s_Fahrenheit __pyx_mstate_global->__pyx_n_s_Fahrenheit
 #define __pyx_n_s_Foot __pyx_mstate_global->__pyx_n_s_Foot
@@ -3395,78 +3182,69 @@
 #define __pyx_kp_s_No_value_specified_for_struct_at_2 __pyx_mstate_global->__pyx_kp_s_No_value_specified_for_struct_at_2
 #define __pyx_kp_s_No_value_specified_for_struct_at_3 __pyx_mstate_global->__pyx_kp_s_No_value_specified_for_struct_at_3
 #define __pyx_n_s_PickleError __pyx_mstate_global->__pyx_n_s_PickleError
 #define __pyx_n_s_Pound __pyx_mstate_global->__pyx_n_s_Pound
 #define __pyx_n_s_PreferredUnits __pyx_mstate_global->__pyx_n_s_PreferredUnits
 #define __pyx_n_s_Pressure __pyx_mstate_global->__pyx_n_s_Pressure
 #define __pyx_n_s_Radian __pyx_mstate_global->__pyx_n_s_Radian
-#define __pyx_n_s_Settings __pyx_mstate_global->__pyx_n_s_Settings
 #define __pyx_n_s_Shot __pyx_mstate_global->__pyx_n_s_Shot
 #define __pyx_n_s_Temperature __pyx_mstate_global->__pyx_n_s_Temperature
 #define __pyx_n_s_TrajectoryCalc __pyx_mstate_global->__pyx_n_s_TrajectoryCalc
 #define __pyx_n_u_TrajectoryCalc __pyx_mstate_global->__pyx_n_u_TrajectoryCalc
-#define __pyx_n_s_TrajectoryCalc___reduce_cython __pyx_mstate_global->__pyx_n_s_TrajectoryCalc___reduce_cython
-#define __pyx_n_s_TrajectoryCalc___setstate_cython __pyx_mstate_global->__pyx_n_s_TrajectoryCalc___setstate_cython
-#define __pyx_n_s_TrajectoryCalc_trajectory __pyx_mstate_global->__pyx_n_s_TrajectoryCalc_trajectory
-#define __pyx_n_s_TrajectoryCalc_zero_angle __pyx_mstate_global->__pyx_n_s_TrajectoryCalc_zero_angle
 #define __pyx_n_s_TrajectoryData __pyx_mstate_global->__pyx_n_s_TrajectoryData
 #define __pyx_n_s_TypeError __pyx_mstate_global->__pyx_n_s_TypeError
-#define __pyx_n_s_USE_POWDER_SENSITIVITY __pyx_mstate_global->__pyx_n_s_USE_POWDER_SENSITIVITY
 #define __pyx_n_s_ValueError __pyx_mstate_global->__pyx_n_s_ValueError
 #define __pyx_n_s_Vector __pyx_mstate_global->__pyx_n_s_Vector
-#define __pyx_n_s_Vector___reduce_cython __pyx_mstate_global->__pyx_n_s_Vector___reduce_cython
-#define __pyx_n_s_Vector___setstate_cython __pyx_mstate_global->__pyx_n_s_Vector___setstate_cython
 #define __pyx_n_s_Velocity __pyx_mstate_global->__pyx_n_s_Velocity
 #define __pyx_n_s_Weight __pyx_mstate_global->__pyx_n_s_Weight
 #define __pyx_n_s_Wind __pyx_mstate_global->__pyx_n_s_Wind
 #define __pyx_kp_u_Zero_vertical_error __pyx_mstate_global->__pyx_kp_u_Zero_vertical_error
-#define __pyx_n_s__23 __pyx_mstate_global->__pyx_n_s__23
-#define __pyx_kp_u__6 __pyx_mstate_global->__pyx_kp_u__6
-#define __pyx_n_s__7 __pyx_mstate_global->__pyx_n_s__7
+#define __pyx_n_s__20 __pyx_mstate_global->__pyx_n_s__20
+#define __pyx_kp_u__7 __pyx_mstate_global->__pyx_kp_u__7
+#define __pyx_n_s__8 __pyx_mstate_global->__pyx_n_s__8
 #define __pyx_n_s_a __pyx_mstate_global->__pyx_n_s_a
 #define __pyx_n_s_all __pyx_mstate_global->__pyx_n_s_all
 #define __pyx_n_s_altitude __pyx_mstate_global->__pyx_n_s_altitude
 #define __pyx_n_s_ammo __pyx_mstate_global->__pyx_n_s_ammo
 #define __pyx_n_s_angle __pyx_mstate_global->__pyx_n_s_angle
-#define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_atmo __pyx_mstate_global->__pyx_n_s_atmo
 #define __pyx_n_s_b __pyx_mstate_global->__pyx_n_s_b
 #define __pyx_n_s_barrel_azimuth __pyx_mstate_global->__pyx_n_s_barrel_azimuth
 #define __pyx_n_s_barrel_elevation __pyx_mstate_global->__pyx_n_s_barrel_elevation
-#define __pyx_n_s_bool __pyx_mstate_global->__pyx_n_s_bool
 #define __pyx_n_s_c __pyx_mstate_global->__pyx_n_s_c
 #define __pyx_n_s_cant_angle __pyx_mstate_global->__pyx_n_s_cant_angle
-#define __pyx_n_s_class_getitem __pyx_mstate_global->__pyx_n_s_class_getitem
 #define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
 #define __pyx_n_s_density_factor __pyx_mstate_global->__pyx_n_s_density_factor
 #define __pyx_n_s_diameter __pyx_mstate_global->__pyx_n_s_diameter
 #define __pyx_n_s_dict __pyx_mstate_global->__pyx_n_s_dict
-#define __pyx_n_s_dict_2 __pyx_mstate_global->__pyx_n_s_dict_2
 #define __pyx_n_s_direction_from __pyx_mstate_global->__pyx_n_s_direction_from
 #define __pyx_kp_u_disable __pyx_mstate_global->__pyx_kp_u_disable
 #define __pyx_n_s_dist_step __pyx_mstate_global->__pyx_n_s_dist_step
 #define __pyx_n_s_distance __pyx_mstate_global->__pyx_n_s_distance
 #define __pyx_n_s_dm __pyx_mstate_global->__pyx_n_s_dm
 #define __pyx_n_s_drag __pyx_mstate_global->__pyx_n_s_drag
 #define __pyx_n_s_drag_table __pyx_mstate_global->__pyx_n_s_drag_table
 #define __pyx_n_s_drop_adj __pyx_mstate_global->__pyx_n_s_drop_adj
 #define __pyx_kp_u_enable __pyx_mstate_global->__pyx_kp_u_enable
 #define __pyx_n_s_energy __pyx_mstate_global->__pyx_n_s_energy
 #define __pyx_n_s_extra_data __pyx_mstate_global->__pyx_n_s_extra_data
 #define __pyx_kp_u_feet_after __pyx_mstate_global->__pyx_kp_u_feet_after
-#define __pyx_n_s_filter_flags __pyx_mstate_global->__pyx_n_s_filter_flags
 #define __pyx_n_s_flag __pyx_mstate_global->__pyx_n_s_flag
 #define __pyx_kp_u_gc __pyx_mstate_global->__pyx_kp_u_gc
 #define __pyx_n_s_get_density_factor_and_mach_for __pyx_mstate_global->__pyx_n_s_get_density_factor_and_mach_for
-#define __pyx_n_s_get_max_calc_step_size __pyx_mstate_global->__pyx_n_s_get_max_calc_step_size
+#define __pyx_n_s_get_global_max_calc_step_size __pyx_mstate_global->__pyx_n_s_get_global_max_calc_step_size
+#define __pyx_n_u_get_global_max_calc_step_size __pyx_mstate_global->__pyx_n_u_get_global_max_calc_step_size
+#define __pyx_n_s_get_global_use_powder_sensitivit __pyx_mstate_global->__pyx_n_s_get_global_use_powder_sensitivit
+#define __pyx_n_u_get_global_use_powder_sensitivit __pyx_mstate_global->__pyx_n_u_get_global_use_powder_sensitivit
 #define __pyx_n_s_get_velocity_for_temp __pyx_mstate_global->__pyx_n_s_get_velocity_for_temp
 #define __pyx_n_s_getstate __pyx_mstate_global->__pyx_n_s_getstate
+#define __pyx_kp_u_globalMaxCalcStepSize_have_to_b __pyx_mstate_global->__pyx_kp_u_globalMaxCalcStepSize_have_to_b
 #define __pyx_n_s_height __pyx_mstate_global->__pyx_n_s_height
 #define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
-#define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
+#define __pyx_kp_u_is_not_a_boolean __pyx_mstate_global->__pyx_kp_u_is_not_a_boolean
 #define __pyx_kp_u_isenabled __pyx_mstate_global->__pyx_kp_u_isenabled
 #define __pyx_kp_u_iterations __pyx_mstate_global->__pyx_kp_u_iterations
 #define __pyx_n_s_length __pyx_mstate_global->__pyx_n_s_length
 #define __pyx_n_s_look_angle __pyx_mstate_global->__pyx_n_s_look_angle
 #define __pyx_n_s_look_distance __pyx_mstate_global->__pyx_n_s_look_distance
 #define __pyx_n_s_mach __pyx_mstate_global->__pyx_n_s_mach
 #define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
@@ -3476,89 +3254,88 @@
 #define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
 #define __pyx_n_s_new __pyx_mstate_global->__pyx_n_s_new
 #define __pyx_kp_s_no_default___reduce___due_to_non __pyx_mstate_global->__pyx_kp_s_no_default___reduce___due_to_non
 #define __pyx_n_s_ogw __pyx_mstate_global->__pyx_n_s_ogw
 #define __pyx_n_s_pickle __pyx_mstate_global->__pyx_n_s_pickle
 #define __pyx_n_s_pressure __pyx_mstate_global->__pyx_n_s_pressure
 #define __pyx_n_s_py_ballisticcalc_conditions __pyx_mstate_global->__pyx_n_s_py_ballisticcalc_conditions
-#define __pyx_n_s_py_ballisticcalc_exts_trajectory __pyx_mstate_global->__pyx_n_s_py_ballisticcalc_exts_trajectory
-#define __pyx_kp_s_py_ballisticcalc_exts_trajectory_2 __pyx_mstate_global->__pyx_kp_s_py_ballisticcalc_exts_trajectory_2
+#define __pyx_kp_s_py_ballisticcalc_exts_trajectory __pyx_mstate_global->__pyx_kp_s_py_ballisticcalc_exts_trajectory
+#define __pyx_n_s_py_ballisticcalc_exts_trajectory_2 __pyx_mstate_global->__pyx_n_s_py_ballisticcalc_exts_trajectory_2
 #define __pyx_n_s_py_ballisticcalc_munition __pyx_mstate_global->__pyx_n_s_py_ballisticcalc_munition
-#define __pyx_n_s_py_ballisticcalc_settings __pyx_mstate_global->__pyx_n_s_py_ballisticcalc_settings
 #define __pyx_n_s_py_ballisticcalc_trajectory_data __pyx_mstate_global->__pyx_n_s_py_ballisticcalc_trajectory_data
 #define __pyx_n_s_py_ballisticcalc_unit __pyx_mstate_global->__pyx_n_s_py_ballisticcalc_unit
 #define __pyx_n_s_pyx_PickleError __pyx_mstate_global->__pyx_n_s_pyx_PickleError
 #define __pyx_n_s_pyx_checksum __pyx_mstate_global->__pyx_n_s_pyx_checksum
 #define __pyx_n_s_pyx_result __pyx_mstate_global->__pyx_n_s_pyx_result
 #define __pyx_n_s_pyx_state __pyx_mstate_global->__pyx_n_s_pyx_state
 #define __pyx_n_s_pyx_type __pyx_mstate_global->__pyx_n_s_pyx_type
 #define __pyx_n_s_pyx_unpickle_TrajectoryCalc __pyx_mstate_global->__pyx_n_s_pyx_unpickle_TrajectoryCalc
 #define __pyx_n_s_pyx_vtable __pyx_mstate_global->__pyx_n_s_pyx_vtable
 #define __pyx_n_s_range __pyx_mstate_global->__pyx_n_s_range
+#define __pyx_n_s_raw_value __pyx_mstate_global->__pyx_n_s_raw_value
 #define __pyx_n_s_reduce __pyx_mstate_global->__pyx_n_s_reduce
 #define __pyx_n_s_reduce_cython __pyx_mstate_global->__pyx_n_s_reduce_cython
 #define __pyx_n_s_reduce_ex __pyx_mstate_global->__pyx_n_s_reduce_ex
-#define __pyx_n_s_self __pyx_mstate_global->__pyx_n_s_self
+#define __pyx_n_s_reset_globals __pyx_mstate_global->__pyx_n_s_reset_globals
+#define __pyx_n_u_reset_globals __pyx_mstate_global->__pyx_n_u_reset_globals
+#define __pyx_n_s_set_global_max_calc_step_size __pyx_mstate_global->__pyx_n_s_set_global_max_calc_step_size
+#define __pyx_n_u_set_global_max_calc_step_size __pyx_mstate_global->__pyx_n_u_set_global_max_calc_step_size
+#define __pyx_kp_u_set_global_use_powder_sensitivit __pyx_mstate_global->__pyx_kp_u_set_global_use_powder_sensitivit
+#define __pyx_n_s_set_global_use_powder_sensitivit_2 __pyx_mstate_global->__pyx_n_s_set_global_use_powder_sensitivit_2
+#define __pyx_n_u_set_global_use_powder_sensitivit_2 __pyx_mstate_global->__pyx_n_u_set_global_use_powder_sensitivit_2
 #define __pyx_n_s_setstate __pyx_mstate_global->__pyx_n_s_setstate
 #define __pyx_n_s_setstate_cython __pyx_mstate_global->__pyx_n_s_setstate_cython
 #define __pyx_n_s_shot_info __pyx_mstate_global->__pyx_n_s_shot_info
 #define __pyx_n_s_sight_height __pyx_mstate_global->__pyx_n_s_sight_height
-#define __pyx_n_s_state __pyx_mstate_global->__pyx_n_s_state
-#define __pyx_n_s_step __pyx_mstate_global->__pyx_n_s_step
 #define __pyx_kp_s_stringsource __pyx_mstate_global->__pyx_kp_s_stringsource
 #define __pyx_n_s_target_drop __pyx_mstate_global->__pyx_n_s_target_drop
 #define __pyx_n_s_temperature __pyx_mstate_global->__pyx_n_s_temperature
 #define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
 #define __pyx_n_s_time __pyx_mstate_global->__pyx_n_s_time
-#define __pyx_n_s_trajectory __pyx_mstate_global->__pyx_n_s_trajectory
 #define __pyx_n_s_twist __pyx_mstate_global->__pyx_n_s_twist
 #define __pyx_n_s_until_distance __pyx_mstate_global->__pyx_n_s_until_distance
 #define __pyx_n_s_update __pyx_mstate_global->__pyx_n_s_update
-#define __pyx_n_s_use_setstate __pyx_mstate_global->__pyx_n_s_use_setstate
+#define __pyx_n_s_value __pyx_mstate_global->__pyx_n_s_value
+#define __pyx_n_s_value_2 __pyx_mstate_global->__pyx_n_s_value_2
 #define __pyx_n_s_velocity __pyx_mstate_global->__pyx_n_s_velocity
 #define __pyx_n_s_weapon __pyx_mstate_global->__pyx_n_s_weapon
 #define __pyx_n_s_weight __pyx_mstate_global->__pyx_n_s_weight
 #define __pyx_n_s_windage __pyx_mstate_global->__pyx_n_s_windage
 #define __pyx_n_s_windage_adj __pyx_mstate_global->__pyx_n_s_windage_adj
 #define __pyx_n_s_winds __pyx_mstate_global->__pyx_n_s_winds
 #define __pyx_n_s_x __pyx_mstate_global->__pyx_n_s_x
 #define __pyx_n_s_y __pyx_mstate_global->__pyx_n_s_y
 #define __pyx_n_s_z __pyx_mstate_global->__pyx_n_s_z
-#define __pyx_n_s_zero_angle __pyx_mstate_global->__pyx_n_s_zero_angle
 #define __pyx_float__0 __pyx_mstate_global->__pyx_float__0
 #define __pyx_float_0_ __pyx_mstate_global->__pyx_float_0_
 #define __pyx_float_0_0 __pyx_mstate_global->__pyx_float_0_0
 #define __pyx_float_0_2 __pyx_mstate_global->__pyx_float_0_2
-#define __pyx_float_2_0 __pyx_mstate_global->__pyx_float_2_0
+#define __pyx_float_0_5 __pyx_mstate_global->__pyx_float_0_5
+#define __pyx_int_0 __pyx_mstate_global->__pyx_int_0
 #define __pyx_int_1 __pyx_mstate_global->__pyx_int_1
-#define __pyx_int_12 __pyx_mstate_global->__pyx_int_12
 #define __pyx_int_27349086 __pyx_mstate_global->__pyx_int_27349086
 #define __pyx_int_71437536 __pyx_mstate_global->__pyx_int_71437536
 #define __pyx_int_183388106 __pyx_mstate_global->__pyx_int_183388106
-#define __pyx_int_neg_1 __pyx_mstate_global->__pyx_int_neg_1
 #define __pyx_tuple_ __pyx_mstate_global->__pyx_tuple_
 #define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
 #define __pyx_tuple__3 __pyx_mstate_global->__pyx_tuple__3
 #define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
 #define __pyx_tuple__5 __pyx_mstate_global->__pyx_tuple__5
-#define __pyx_tuple__8 __pyx_mstate_global->__pyx_tuple__8
+#define __pyx_tuple__6 __pyx_mstate_global->__pyx_tuple__6
 #define __pyx_tuple__9 __pyx_mstate_global->__pyx_tuple__9
-#define __pyx_tuple__11 __pyx_mstate_global->__pyx_tuple__11
+#define __pyx_tuple__10 __pyx_mstate_global->__pyx_tuple__10
 #define __pyx_tuple__13 __pyx_mstate_global->__pyx_tuple__13
 #define __pyx_tuple__15 __pyx_mstate_global->__pyx_tuple__15
-#define __pyx_tuple__17 __pyx_mstate_global->__pyx_tuple__17
 #define __pyx_tuple__18 __pyx_mstate_global->__pyx_tuple__18
-#define __pyx_tuple__21 __pyx_mstate_global->__pyx_tuple__21
-#define __pyx_codeobj__10 __pyx_mstate_global->__pyx_codeobj__10
+#define __pyx_codeobj__11 __pyx_mstate_global->__pyx_codeobj__11
 #define __pyx_codeobj__12 __pyx_mstate_global->__pyx_codeobj__12
 #define __pyx_codeobj__14 __pyx_mstate_global->__pyx_codeobj__14
 #define __pyx_codeobj__16 __pyx_mstate_global->__pyx_codeobj__16
+#define __pyx_codeobj__17 __pyx_mstate_global->__pyx_codeobj__17
 #define __pyx_codeobj__19 __pyx_mstate_global->__pyx_codeobj__19
-#define __pyx_codeobj__20 __pyx_mstate_global->__pyx_codeobj__20
-#define __pyx_codeobj__22 __pyx_mstate_global->__pyx_codeobj__22
 /* #### Code section: module_code ### */
 
 /* "FromPyStructUtility":12
  * 
  * @cname("__pyx_convert__from_py_struct____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CurvePoint")
  * cdef struct_type __pyx_convert__from_py_struct____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CurvePoint(obj) except *:             # <<<<<<<<<<<<<<
  *     cdef struct_type result
@@ -3944,15 +3721,715 @@
   __Pyx_pretend_to_initialize(&__pyx_r);
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_value);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":36
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":27
+ * cdef object _globalMaxCalcStepSize = Distance.Foot(0.5)
+ * 
+ * def get_global_max_calc_step_size() -> Distance:             # <<<<<<<<<<<<<<
+ *     return _globalMaxCalcStepSize
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_1get_global_max_calc_step_size(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+PyDoc_STRVAR(__pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_get_global_max_calc_step_size, "get_global_max_calc_step_size() -> Distance");
+static PyMethodDef __pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_1get_global_max_calc_step_size = {"get_global_max_calc_step_size", (PyCFunction)__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_1get_global_max_calc_step_size, METH_NOARGS, __pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_get_global_max_calc_step_size};
+static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_1get_global_max_calc_step_size(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("get_global_max_calc_step_size (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  __pyx_r = __pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_get_global_max_calc_step_size(__pyx_self);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_get_global_max_calc_step_size(CYTHON_UNUSED PyObject *__pyx_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("get_global_max_calc_step_size", 1);
+
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":28
+ * 
+ * def get_global_max_calc_step_size() -> Distance:
+ *     return _globalMaxCalcStepSize             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_21py_ballisticcalc_exts_15trajectory_calc__globalMaxCalcStepSize);
+  __pyx_r = __pyx_v_21py_ballisticcalc_exts_15trajectory_calc__globalMaxCalcStepSize;
+  goto __pyx_L0;
+
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":27
+ * cdef object _globalMaxCalcStepSize = Distance.Foot(0.5)
+ * 
+ * def get_global_max_calc_step_size() -> Distance:             # <<<<<<<<<<<<<<
+ *     return _globalMaxCalcStepSize
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":31
+ * 
+ * 
+ * def get_global_use_powder_sensitivity() -> bool:             # <<<<<<<<<<<<<<
+ *     return bool(_globalUsePowderSensitivity)
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_3get_global_use_powder_sensitivity(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+PyDoc_STRVAR(__pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_2get_global_use_powder_sensitivity, "get_global_use_powder_sensitivity() -> bool");
+static PyMethodDef __pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_3get_global_use_powder_sensitivity = {"get_global_use_powder_sensitivity", (PyCFunction)__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_3get_global_use_powder_sensitivity, METH_NOARGS, __pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_2get_global_use_powder_sensitivity};
+static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_3get_global_use_powder_sensitivity(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("get_global_use_powder_sensitivity (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  __pyx_r = __pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_2get_global_use_powder_sensitivity(__pyx_self);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_2get_global_use_powder_sensitivity(CYTHON_UNUSED PyObject *__pyx_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("get_global_use_powder_sensitivity", 1);
+
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":32
+ * 
+ * def get_global_use_powder_sensitivity() -> bool:
+ *     return bool(_globalUsePowderSensitivity)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_21py_ballisticcalc_exts_15trajectory_calc__globalUsePowderSensitivity); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 32, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyBool_FromLong((!(!__pyx_t_2))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":31
+ * 
+ * 
+ * def get_global_use_powder_sensitivity() -> bool:             # <<<<<<<<<<<<<<
+ *     return bool(_globalUsePowderSensitivity)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("py_ballisticcalc_exts.trajectory_calc.get_global_use_powder_sensitivity", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":35
+ * 
+ * 
+ * def set_global_max_calc_step_size(value: [object, float]) -> None:             # <<<<<<<<<<<<<<
+ *     global _globalMaxCalcStepSize
+ *     if (_value := PreferredUnits.distance(value)).raw_value <= 0:
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_5set_global_max_calc_step_size(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_4set_global_max_calc_step_size, "set_global_max_calc_step_size(value: [object, float]) -> None");
+static PyMethodDef __pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_5set_global_max_calc_step_size = {"set_global_max_calc_step_size", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_5set_global_max_calc_step_size, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_4set_global_max_calc_step_size};
+static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_5set_global_max_calc_step_size(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  PyObject *__pyx_v_value = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[1] = {0};
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("set_global_max_calc_step_size (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_value,0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_value)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 35, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "set_global_max_calc_step_size") < 0)) __PYX_ERR(0, 35, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 1)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+    }
+    __pyx_v_value = values[0];
+  }
+  goto __pyx_L6_skip;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("set_global_max_calc_step_size", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 35, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
+  __Pyx_AddTraceback("py_ballisticcalc_exts.trajectory_calc.set_global_max_calc_step_size", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_4set_global_max_calc_step_size(__pyx_self, __pyx_v_value);
+
+  /* function exit code */
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_4set_global_max_calc_step_size(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_value) {
+  CYTHON_UNUSED PyObject *__pyx_v__value = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  int __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("set_global_max_calc_step_size", 1);
+
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":37
+ * def set_global_max_calc_step_size(value: [object, float]) -> None:
+ *     global _globalMaxCalcStepSize
+ *     if (_value := PreferredUnits.distance(value)).raw_value <= 0:             # <<<<<<<<<<<<<<
+ *         raise ValueError("_globalMaxCalcStepSize have to be > 0")
+ *     _globalMaxCalcStepSize = PreferredUnits.distance(value)
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_PreferredUnits); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_distance); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = NULL;
+  __pyx_t_4 = 0;
+  #if CYTHON_UNPACK_METHODS
+  if (unlikely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_2)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_2);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
+      __pyx_t_4 = 1;
+    }
+  }
+  #endif
+  {
+    PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_v_value};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  }
+  __pyx_v__value = __pyx_t_1;
+  __Pyx_INCREF(__pyx_t_1);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_raw_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = PyObject_RichCompare(__pyx_t_3, __pyx_int_0, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 37, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (unlikely(__pyx_t_5)) {
+
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":38
+ *     global _globalMaxCalcStepSize
+ *     if (_value := PreferredUnits.distance(value)).raw_value <= 0:
+ *         raise ValueError("_globalMaxCalcStepSize have to be > 0")             # <<<<<<<<<<<<<<
+ *     _globalMaxCalcStepSize = PreferredUnits.distance(value)
+ * 
+ */
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_Raise(__pyx_t_1, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __PYX_ERR(0, 38, __pyx_L1_error)
+
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":37
+ * def set_global_max_calc_step_size(value: [object, float]) -> None:
+ *     global _globalMaxCalcStepSize
+ *     if (_value := PreferredUnits.distance(value)).raw_value <= 0:             # <<<<<<<<<<<<<<
+ *         raise ValueError("_globalMaxCalcStepSize have to be > 0")
+ *     _globalMaxCalcStepSize = PreferredUnits.distance(value)
+ */
+  }
+
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":39
+ *     if (_value := PreferredUnits.distance(value)).raw_value <= 0:
+ *         raise ValueError("_globalMaxCalcStepSize have to be > 0")
+ *     _globalMaxCalcStepSize = PreferredUnits.distance(value)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_PreferredUnits); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_distance); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = NULL;
+  __pyx_t_4 = 0;
+  #if CYTHON_UNPACK_METHODS
+  if (unlikely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_3);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_4 = 1;
+    }
+  }
+  #endif
+  {
+    PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_value};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 39, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
+  __Pyx_XGOTREF(__pyx_v_21py_ballisticcalc_exts_15trajectory_calc__globalMaxCalcStepSize);
+  __Pyx_DECREF_SET(__pyx_v_21py_ballisticcalc_exts_15trajectory_calc__globalMaxCalcStepSize, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":35
+ * 
+ * 
+ * def set_global_max_calc_step_size(value: [object, float]) -> None:             # <<<<<<<<<<<<<<
+ *     global _globalMaxCalcStepSize
+ *     if (_value := PreferredUnits.distance(value)).raw_value <= 0:
+ */
+
+  /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_AddTraceback("py_ballisticcalc_exts.trajectory_calc.set_global_max_calc_step_size", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v__value);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":42
+ * 
+ * 
+ * def set_global_use_powder_sensitivity(value: bool) -> None:             # <<<<<<<<<<<<<<
+ *     global _globalUsePowderSensitivity
+ *     if not isinstance(value, bool):
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_7set_global_use_powder_sensitivity(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_6set_global_use_powder_sensitivity, "set_global_use_powder_sensitivity(value: bool) -> None");
+static PyMethodDef __pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_7set_global_use_powder_sensitivity = {"set_global_use_powder_sensitivity", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_7set_global_use_powder_sensitivity, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_6set_global_use_powder_sensitivity};
+static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_7set_global_use_powder_sensitivity(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  PyObject *__pyx_v_value = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[1] = {0};
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("set_global_use_powder_sensitivity (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_value,0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_value)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 42, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "set_global_use_powder_sensitivity") < 0)) __PYX_ERR(0, 42, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 1)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+    }
+    __pyx_v_value = values[0];
+  }
+  goto __pyx_L6_skip;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("set_global_use_powder_sensitivity", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 42, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
+  __Pyx_AddTraceback("py_ballisticcalc_exts.trajectory_calc.set_global_use_powder_sensitivity", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_6set_global_use_powder_sensitivity(__pyx_self, __pyx_v_value);
+
+  /* function exit code */
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_6set_global_use_powder_sensitivity(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_value) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
+  Py_ssize_t __pyx_t_4;
+  Py_UCS4 __pyx_t_5;
+  PyObject *__pyx_t_6 = NULL;
+  int __pyx_t_7;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("set_global_use_powder_sensitivity", 1);
+
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":44
+ * def set_global_use_powder_sensitivity(value: bool) -> None:
+ *     global _globalUsePowderSensitivity
+ *     if not isinstance(value, bool):             # <<<<<<<<<<<<<<
+ *         raise TypeError(f"set_global_use_powder_sensitivity {value=} is not a boolean")
+ *     _globalUsePowderSensitivity = int(value)
+ */
+  __pyx_t_1 = ((PyObject*)&PyBool_Type);
+  __Pyx_INCREF(__pyx_t_1);
+  __pyx_t_2 = PyObject_IsInstance(__pyx_v_value, __pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 44, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (!__pyx_t_2);
+  if (unlikely(__pyx_t_3)) {
+
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":45
+ *     global _globalUsePowderSensitivity
+ *     if not isinstance(value, bool):
+ *         raise TypeError(f"set_global_use_powder_sensitivity {value=} is not a boolean")             # <<<<<<<<<<<<<<
+ *     _globalUsePowderSensitivity = int(value)
+ * 
+ */
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 45, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = 0;
+    __pyx_t_5 = 127;
+    __Pyx_INCREF(__pyx_kp_u_set_global_use_powder_sensitivit);
+    __pyx_t_4 += 40;
+    __Pyx_GIVEREF(__pyx_kp_u_set_global_use_powder_sensitivit);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_set_global_use_powder_sensitivit);
+    __pyx_t_6 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Repr(__pyx_v_value), __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 45, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_6) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_6) : __pyx_t_5;
+    __pyx_t_4 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_6);
+    __Pyx_GIVEREF(__pyx_t_6);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_6);
+    __pyx_t_6 = 0;
+    __Pyx_INCREF(__pyx_kp_u_is_not_a_boolean);
+    __pyx_t_4 += 17;
+    __Pyx_GIVEREF(__pyx_kp_u_is_not_a_boolean);
+    PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u_is_not_a_boolean);
+    __pyx_t_6 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 45, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 45, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_Raise(__pyx_t_1, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __PYX_ERR(0, 45, __pyx_L1_error)
+
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":44
+ * def set_global_use_powder_sensitivity(value: bool) -> None:
+ *     global _globalUsePowderSensitivity
+ *     if not isinstance(value, bool):             # <<<<<<<<<<<<<<
+ *         raise TypeError(f"set_global_use_powder_sensitivity {value=} is not a boolean")
+ *     _globalUsePowderSensitivity = int(value)
+ */
+  }
+
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":46
+ *     if not isinstance(value, bool):
+ *         raise TypeError(f"set_global_use_powder_sensitivity {value=} is not a boolean")
+ *     _globalUsePowderSensitivity = int(value)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_t_1 = __Pyx_PyNumber_Int(__pyx_v_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 46, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v_21py_ballisticcalc_exts_15trajectory_calc__globalUsePowderSensitivity = __pyx_t_7;
+
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":42
+ * 
+ * 
+ * def set_global_use_powder_sensitivity(value: bool) -> None:             # <<<<<<<<<<<<<<
+ *     global _globalUsePowderSensitivity
+ *     if not isinstance(value, bool):
+ */
+
+  /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_AddTraceback("py_ballisticcalc_exts.trajectory_calc.set_global_use_powder_sensitivity", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":49
+ * 
+ * 
+ * def reset_globals() -> None:             # <<<<<<<<<<<<<<
+ *     global _globalUsePowderSensitivity, _globalMaxCalcStepSize
+ *     _globalUsePowderSensitivity = False
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_9reset_globals(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+PyDoc_STRVAR(__pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_8reset_globals, "reset_globals() -> None");
+static PyMethodDef __pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_9reset_globals = {"reset_globals", (PyCFunction)__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_9reset_globals, METH_NOARGS, __pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_8reset_globals};
+static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_9reset_globals(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("reset_globals (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  __pyx_r = __pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_8reset_globals(__pyx_self);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_8reset_globals(CYTHON_UNUSED PyObject *__pyx_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("reset_globals", 1);
+
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":51
+ * def reset_globals() -> None:
+ *     global _globalUsePowderSensitivity, _globalMaxCalcStepSize
+ *     _globalUsePowderSensitivity = False             # <<<<<<<<<<<<<<
+ *     _globalMaxCalcStepSize = Distance.Foot(0.5)
+ * 
+ */
+  __pyx_v_21py_ballisticcalc_exts_15trajectory_calc__globalUsePowderSensitivity = 0;
+
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":52
+ *     global _globalUsePowderSensitivity, _globalMaxCalcStepSize
+ *     _globalUsePowderSensitivity = False
+ *     _globalMaxCalcStepSize = Distance.Foot(0.5)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Distance); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_Foot); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = NULL;
+  __pyx_t_4 = 0;
+  #if CYTHON_UNPACK_METHODS
+  if (unlikely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_2)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_2);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
+      __pyx_t_4 = 1;
+    }
+  }
+  #endif
+  {
+    PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_float_0_5};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  }
+  __Pyx_XGOTREF(__pyx_v_21py_ballisticcalc_exts_15trajectory_calc__globalMaxCalcStepSize);
+  __Pyx_DECREF_SET(__pyx_v_21py_ballisticcalc_exts_15trajectory_calc__globalMaxCalcStepSize, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":49
+ * 
+ * 
+ * def reset_globals() -> None:             # <<<<<<<<<<<<<<
+ *     global _globalUsePowderSensitivity, _globalMaxCalcStepSize
+ *     _globalUsePowderSensitivity = False
+ */
+
+  /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_AddTraceback("py_ballisticcalc_exts.trajectory_calc.reset_globals", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":74
  *     cdef double z
  * 
  *     def __cinit__(Vector self, double x, double y, double z):             # <<<<<<<<<<<<<<
  *         self.x = x
  *         self.y = y
  */
 
@@ -3994,55 +4471,55 @@
       kw_args = __Pyx_NumKwargs_VARARGS(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_x)) != 0)) {
           (void)__Pyx_Arg_NewRef_VARARGS(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 36, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 74, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_y)) != 0)) {
           (void)__Pyx_Arg_NewRef_VARARGS(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 36, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 74, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, 1); __PYX_ERR(0, 36, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, 1); __PYX_ERR(0, 74, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_z)) != 0)) {
           (void)__Pyx_Arg_NewRef_VARARGS(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 36, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 74, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, 2); __PYX_ERR(0, 36, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, 2); __PYX_ERR(0, 74, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__cinit__") < 0)) __PYX_ERR(0, 36, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__cinit__") < 0)) __PYX_ERR(0, 74, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 3)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
       values[1] = __Pyx_Arg_VARARGS(__pyx_args, 1);
       values[2] = __Pyx_Arg_VARARGS(__pyx_args, 2);
     }
-    __pyx_v_x = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_x == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 36, __pyx_L3_error)
-    __pyx_v_y = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_y == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 36, __pyx_L3_error)
-    __pyx_v_z = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_z == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 36, __pyx_L3_error)
+    __pyx_v_x = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_x == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 74, __pyx_L3_error)
+    __pyx_v_y = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_y == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 74, __pyx_L3_error)
+    __pyx_v_z = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_z == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 74, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 36, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 74, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
@@ -4064,89 +4541,89 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static int __pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_6Vector___cinit__(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_self, double __pyx_v_x, double __pyx_v_y, double __pyx_v_z) {
   int __pyx_r;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":37
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":75
  * 
  *     def __cinit__(Vector self, double x, double y, double z):
  *         self.x = x             # <<<<<<<<<<<<<<
  *         self.y = y
  *         self.z = z
  */
   __pyx_v_self->x = __pyx_v_x;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":38
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":76
  *     def __cinit__(Vector self, double x, double y, double z):
  *         self.x = x
  *         self.y = y             # <<<<<<<<<<<<<<
  *         self.z = z
  * 
  */
   __pyx_v_self->y = __pyx_v_y;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":39
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":77
  *         self.x = x
  *         self.y = y
  *         self.z = z             # <<<<<<<<<<<<<<
  * 
  *     cdef double magnitude(Vector self):
  */
   __pyx_v_self->z = __pyx_v_z;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":36
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":74
  *     cdef double z
  * 
  *     def __cinit__(Vector self, double x, double y, double z):             # <<<<<<<<<<<<<<
  *         self.x = x
  *         self.y = y
  */
 
   /* function exit code */
   __pyx_r = 0;
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":41
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":79
  *         self.z = z
  * 
  *     cdef double magnitude(Vector self):             # <<<<<<<<<<<<<<
  *         return sqrt(self.x * self.x + self.y * self.y + self.z * self.z)
  * 
  */
 
 static double __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_6Vector_magnitude(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_self) {
   double __pyx_r;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":42
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":80
  * 
  *     cdef double magnitude(Vector self):
  *         return sqrt(self.x * self.x + self.y * self.y + self.z * self.z)             # <<<<<<<<<<<<<<
  * 
  *     cdef Vector mul_by_const(Vector self, double a):
  */
   __pyx_r = sqrt((((__pyx_v_self->x * __pyx_v_self->x) + (__pyx_v_self->y * __pyx_v_self->y)) + (__pyx_v_self->z * __pyx_v_self->z)));
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":41
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":79
  *         self.z = z
  * 
  *     cdef double magnitude(Vector self):             # <<<<<<<<<<<<<<
  *         return sqrt(self.x * self.x + self.y * self.y + self.z * self.z)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":44
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":82
  *         return sqrt(self.x * self.x + self.y * self.y + self.z * self.z)
  * 
  *     cdef Vector mul_by_const(Vector self, double a):             # <<<<<<<<<<<<<<
  *         return Vector(self.x * a, self.y * a, self.z * a)
  * 
  */
 
@@ -4158,47 +4635,47 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("mul_by_const", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":45
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":83
  * 
  *     cdef Vector mul_by_const(Vector self, double a):
  *         return Vector(self.x * a, self.y * a, self.z * a)             # <<<<<<<<<<<<<<
  * 
  *     cdef double mul_by_vector(Vector self, Vector b):
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_self->x * __pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_self->x * __pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyFloat_FromDouble((__pyx_v_self->y * __pyx_v_a)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble((__pyx_v_self->y * __pyx_v_a)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyFloat_FromDouble((__pyx_v_self->z * __pyx_v_a)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_t_3 = PyFloat_FromDouble((__pyx_v_self->z * __pyx_v_a)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1)) __PYX_ERR(0, 45, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1)) __PYX_ERR(0, 83, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2)) __PYX_ERR(0, 45, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2)) __PYX_ERR(0, 83, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_3)) __PYX_ERR(0, 45, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_3)) __PYX_ERR(0, 83, __pyx_L1_error);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_r = ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_3);
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":44
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":82
  *         return sqrt(self.x * self.x + self.y * self.y + self.z * self.z)
  * 
  *     cdef Vector mul_by_const(Vector self, double a):             # <<<<<<<<<<<<<<
  *         return Vector(self.x * a, self.y * a, self.z * a)
  * 
  */
 
@@ -4212,49 +4689,49 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":47
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":85
  *         return Vector(self.x * a, self.y * a, self.z * a)
  * 
  *     cdef double mul_by_vector(Vector self, Vector b):             # <<<<<<<<<<<<<<
  *         return self.x * b.x + self.y * b.y + self.z * b.z
  * 
  */
 
 static double __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_6Vector_mul_by_vector(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_self, struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_b) {
   double __pyx_r;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":48
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":86
  * 
  *     cdef double mul_by_vector(Vector self, Vector b):
  *         return self.x * b.x + self.y * b.y + self.z * b.z             # <<<<<<<<<<<<<<
  * 
  *     cdef Vector add(Vector self, Vector b):
  */
   __pyx_r = (((__pyx_v_self->x * __pyx_v_b->x) + (__pyx_v_self->y * __pyx_v_b->y)) + (__pyx_v_self->z * __pyx_v_b->z));
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":47
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":85
  *         return Vector(self.x * a, self.y * a, self.z * a)
  * 
  *     cdef double mul_by_vector(Vector self, Vector b):             # <<<<<<<<<<<<<<
  *         return self.x * b.x + self.y * b.y + self.z * b.z
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":50
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":88
  *         return self.x * b.x + self.y * b.y + self.z * b.z
  * 
  *     cdef Vector add(Vector self, Vector b):             # <<<<<<<<<<<<<<
  *         return Vector(self.x + b.x, self.y + b.y, self.z + b.z)
  * 
  */
 
@@ -4266,47 +4743,47 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("add", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":51
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":89
  * 
  *     cdef Vector add(Vector self, Vector b):
  *         return Vector(self.x + b.x, self.y + b.y, self.z + b.z)             # <<<<<<<<<<<<<<
  * 
  *     cdef Vector subtract(Vector self, Vector b):
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_self->x + __pyx_v_b->x)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_self->x + __pyx_v_b->x)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyFloat_FromDouble((__pyx_v_self->y + __pyx_v_b->y)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble((__pyx_v_self->y + __pyx_v_b->y)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyFloat_FromDouble((__pyx_v_self->z + __pyx_v_b->z)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_3 = PyFloat_FromDouble((__pyx_v_self->z + __pyx_v_b->z)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1)) __PYX_ERR(0, 89, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2)) __PYX_ERR(0, 51, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2)) __PYX_ERR(0, 89, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_3)) __PYX_ERR(0, 51, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_3)) __PYX_ERR(0, 89, __pyx_L1_error);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_r = ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_3);
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":50
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":88
  *         return self.x * b.x + self.y * b.y + self.z * b.z
  * 
  *     cdef Vector add(Vector self, Vector b):             # <<<<<<<<<<<<<<
  *         return Vector(self.x + b.x, self.y + b.y, self.z + b.z)
  * 
  */
 
@@ -4320,15 +4797,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":53
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":91
  *         return Vector(self.x + b.x, self.y + b.y, self.z + b.z)
  * 
  *     cdef Vector subtract(Vector self, Vector b):             # <<<<<<<<<<<<<<
  *         return Vector(self.x - b.x, self.y - b.y, self.z - b.z)
  * 
  */
 
@@ -4340,47 +4817,47 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("subtract", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":54
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":92
  * 
  *     cdef Vector subtract(Vector self, Vector b):
  *         return Vector(self.x - b.x, self.y - b.y, self.z - b.z)             # <<<<<<<<<<<<<<
  * 
  *     cdef Vector negate(Vector self):
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_self->x - __pyx_v_b->x)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_self->x - __pyx_v_b->x)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyFloat_FromDouble((__pyx_v_self->y - __pyx_v_b->y)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble((__pyx_v_self->y - __pyx_v_b->y)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyFloat_FromDouble((__pyx_v_self->z - __pyx_v_b->z)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_t_3 = PyFloat_FromDouble((__pyx_v_self->z - __pyx_v_b->z)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1)) __PYX_ERR(0, 54, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2)) __PYX_ERR(0, 54, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2)) __PYX_ERR(0, 92, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_3)) __PYX_ERR(0, 54, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_3)) __PYX_ERR(0, 92, __pyx_L1_error);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_r = ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_3);
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":53
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":91
  *         return Vector(self.x + b.x, self.y + b.y, self.z + b.z)
  * 
  *     cdef Vector subtract(Vector self, Vector b):             # <<<<<<<<<<<<<<
  *         return Vector(self.x - b.x, self.y - b.y, self.z - b.z)
  * 
  */
 
@@ -4394,15 +4871,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":56
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":94
  *         return Vector(self.x - b.x, self.y - b.y, self.z - b.z)
  * 
  *     cdef Vector negate(Vector self):             # <<<<<<<<<<<<<<
  *         return Vector(-self.x, -self.y, -self.z)
  * 
  */
 
@@ -4414,47 +4891,47 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("negate", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":57
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":95
  * 
  *     cdef Vector negate(Vector self):
  *         return Vector(-self.x, -self.y, -self.z)             # <<<<<<<<<<<<<<
  * 
  *     cdef Vector normalize(Vector self):
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble((-__pyx_v_self->x)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble((-__pyx_v_self->x)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyFloat_FromDouble((-__pyx_v_self->y)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble((-__pyx_v_self->y)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyFloat_FromDouble((-__pyx_v_self->z)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __pyx_t_3 = PyFloat_FromDouble((-__pyx_v_self->z)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1)) __PYX_ERR(0, 95, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2)) __PYX_ERR(0, 95, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_3)) __PYX_ERR(0, 57, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_3)) __PYX_ERR(0, 95, __pyx_L1_error);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_r = ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_3);
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":56
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":94
  *         return Vector(self.x - b.x, self.y - b.y, self.z - b.z)
  * 
  *     cdef Vector negate(Vector self):             # <<<<<<<<<<<<<<
  *         return Vector(-self.x, -self.y, -self.z)
  * 
  */
 
@@ -4468,15 +4945,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":59
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":97
  *         return Vector(-self.x, -self.y, -self.z)
  * 
  *     cdef Vector normalize(Vector self):             # <<<<<<<<<<<<<<
  *         cdef double m = self.magnitude()
  *         if fabs(m) < 1e-10:
  */
 
@@ -4491,94 +4968,90 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("normalize", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":60
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":98
  * 
  *     cdef Vector normalize(Vector self):
  *         cdef double m = self.magnitude()             # <<<<<<<<<<<<<<
  *         if fabs(m) < 1e-10:
  *             return Vector(self.x, self.y, self.z)
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_self->__pyx_vtab)->magnitude(__pyx_v_self); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 60, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_self->__pyx_vtab)->magnitude(__pyx_v_self); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 98, __pyx_L1_error)
   __pyx_v_m = __pyx_t_1;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":61
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":99
  *     cdef Vector normalize(Vector self):
  *         cdef double m = self.magnitude()
  *         if fabs(m) < 1e-10:             # <<<<<<<<<<<<<<
  *             return Vector(self.x, self.y, self.z)
  *         return self.mul_by_const(1.0 / m)
  */
   __pyx_t_2 = (fabs(__pyx_v_m) < 1e-10);
   if (__pyx_t_2) {
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":62
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":100
  *         cdef double m = self.magnitude()
  *         if fabs(m) < 1e-10:
  *             return Vector(self.x, self.y, self.z)             # <<<<<<<<<<<<<<
  *         return self.mul_by_const(1.0 / m)
  * 
  */
     __Pyx_XDECREF((PyObject *)__pyx_r);
-    __pyx_t_3 = PyFloat_FromDouble(__pyx_v_self->x); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 62, __pyx_L1_error)
+    __pyx_t_3 = PyFloat_FromDouble(__pyx_v_self->x); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 100, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = PyFloat_FromDouble(__pyx_v_self->y); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 62, __pyx_L1_error)
+    __pyx_t_4 = PyFloat_FromDouble(__pyx_v_self->y); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 100, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PyFloat_FromDouble(__pyx_v_self->z); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 62, __pyx_L1_error)
+    __pyx_t_5 = PyFloat_FromDouble(__pyx_v_self->z); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 100, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 62, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 100, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_3);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3)) __PYX_ERR(0, 62, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3)) __PYX_ERR(0, 100, __pyx_L1_error);
     __Pyx_GIVEREF(__pyx_t_4);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_4)) __PYX_ERR(0, 62, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_4)) __PYX_ERR(0, 100, __pyx_L1_error);
     __Pyx_GIVEREF(__pyx_t_5);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_t_5)) __PYX_ERR(0, 62, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_t_5)) __PYX_ERR(0, 100, __pyx_L1_error);
     __pyx_t_3 = 0;
     __pyx_t_4 = 0;
     __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_t_6, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 62, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_t_6, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 100, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_r = ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_5);
     __pyx_t_5 = 0;
     goto __pyx_L0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":61
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":99
  *     cdef Vector normalize(Vector self):
  *         cdef double m = self.magnitude()
  *         if fabs(m) < 1e-10:             # <<<<<<<<<<<<<<
  *             return Vector(self.x, self.y, self.z)
  *         return self.mul_by_const(1.0 / m)
  */
   }
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":63
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":101
  *         if fabs(m) < 1e-10:
  *             return Vector(self.x, self.y, self.z)
  *         return self.mul_by_const(1.0 / m)             # <<<<<<<<<<<<<<
  * 
  *     def __add__(Vector self, Vector other):
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
-  if (unlikely(__pyx_v_m == 0)) {
-    PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(0, 63, __pyx_L1_error)
-  }
-  __pyx_t_5 = ((PyObject *)((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_self->__pyx_vtab)->mul_by_const(__pyx_v_self, (1.0 / __pyx_v_m))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_5 = ((PyObject *)((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_self->__pyx_vtab)->mul_by_const(__pyx_v_self, (1.0 / __pyx_v_m))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_r = ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_5);
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":59
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":97
  *         return Vector(-self.x, -self.y, -self.z)
  * 
  *     cdef Vector normalize(Vector self):             # <<<<<<<<<<<<<<
  *         cdef double m = self.magnitude()
  *         if fabs(m) < 1e-10:
  */
 
@@ -4592,15 +5065,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":65
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":103
  *         return self.mul_by_const(1.0 / m)
  * 
  *     def __add__(Vector self, Vector other):             # <<<<<<<<<<<<<<
  *         return self.add(other)
  * 
  */
 
@@ -4611,15 +5084,16 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__add__ (wrapper)", 0);
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_other), __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector, 1, "other", 0))) __PYX_ERR(0, 65, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_self), __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector, 1, "self", 0))) __PYX_ERR(0, 103, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_other), __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector, 1, "other", 0))) __PYX_ERR(0, 103, __pyx_L1_error)
   __pyx_r = __pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_6Vector_2__add__(((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_self), ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_other));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4632,29 +5106,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__add__", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":66
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":104
  * 
  *     def __add__(Vector self, Vector other):
  *         return self.add(other)             # <<<<<<<<<<<<<<
  * 
  *     def __radd__(Vector self, Vector other):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_self->__pyx_vtab)->add(__pyx_v_self, __pyx_v_other)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_self->__pyx_vtab)->add(__pyx_v_self, __pyx_v_other)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 104, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":65
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":103
  *         return self.mul_by_const(1.0 / m)
  * 
  *     def __add__(Vector self, Vector other):             # <<<<<<<<<<<<<<
  *         return self.add(other)
  * 
  */
 
@@ -4665,15 +5139,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":68
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":106
  *         return self.add(other)
  * 
  *     def __radd__(Vector self, Vector other):             # <<<<<<<<<<<<<<
  *         return self.add(other)
  * 
  */
 
@@ -4684,15 +5158,16 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__radd__ (wrapper)", 0);
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_other), __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector, 1, "other", 0))) __PYX_ERR(0, 68, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_self), __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector, 1, "self", 0))) __PYX_ERR(0, 106, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_other), __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector, 1, "other", 0))) __PYX_ERR(0, 106, __pyx_L1_error)
   __pyx_r = __pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_6Vector_4__radd__(((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_self), ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_other));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4705,29 +5180,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__radd__", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":69
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":107
  * 
  *     def __radd__(Vector self, Vector other):
  *         return self.add(other)             # <<<<<<<<<<<<<<
  * 
  *     def __iadd__(Vector self, Vector other):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_self->__pyx_vtab)->add(__pyx_v_self, __pyx_v_other)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_self->__pyx_vtab)->add(__pyx_v_self, __pyx_v_other)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":68
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":106
  *         return self.add(other)
  * 
  *     def __radd__(Vector self, Vector other):             # <<<<<<<<<<<<<<
  *         return self.add(other)
  * 
  */
 
@@ -4738,15 +5213,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":71
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":109
  *         return self.add(other)
  * 
  *     def __iadd__(Vector self, Vector other):             # <<<<<<<<<<<<<<
  *         return self.add(other)
  * 
  */
 
@@ -4757,15 +5232,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__iadd__ (wrapper)", 0);
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_other), __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector, 1, "other", 0))) __PYX_ERR(0, 71, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_other), __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector, 1, "other", 0))) __PYX_ERR(0, 109, __pyx_L1_error)
   __pyx_r = __pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_6Vector_6__iadd__(((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_self), ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_other));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4778,29 +5253,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__iadd__", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":72
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":110
  * 
  *     def __iadd__(Vector self, Vector other):
  *         return self.add(other)             # <<<<<<<<<<<<<<
  * 
  *     def __sub__(Vector self, Vector other):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_self->__pyx_vtab)->add(__pyx_v_self, __pyx_v_other)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_self->__pyx_vtab)->add(__pyx_v_self, __pyx_v_other)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":71
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":109
  *         return self.add(other)
  * 
  *     def __iadd__(Vector self, Vector other):             # <<<<<<<<<<<<<<
  *         return self.add(other)
  * 
  */
 
@@ -4811,15 +5286,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":74
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":112
  *         return self.add(other)
  * 
  *     def __sub__(Vector self, Vector other):             # <<<<<<<<<<<<<<
  *         return self.subtract(other)
  * 
  */
 
@@ -4830,15 +5305,16 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__sub__ (wrapper)", 0);
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_other), __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector, 1, "other", 0))) __PYX_ERR(0, 74, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_self), __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector, 1, "self", 0))) __PYX_ERR(0, 112, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_other), __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector, 1, "other", 0))) __PYX_ERR(0, 112, __pyx_L1_error)
   __pyx_r = __pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_6Vector_8__sub__(((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_self), ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_other));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4851,29 +5327,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__sub__", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":75
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":113
  * 
  *     def __sub__(Vector self, Vector other):
  *         return self.subtract(other)             # <<<<<<<<<<<<<<
  * 
  *     def __rsub__(Vector self, Vector other):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_self->__pyx_vtab)->subtract(__pyx_v_self, __pyx_v_other)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_self->__pyx_vtab)->subtract(__pyx_v_self, __pyx_v_other)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":74
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":112
  *         return self.add(other)
  * 
  *     def __sub__(Vector self, Vector other):             # <<<<<<<<<<<<<<
  *         return self.subtract(other)
  * 
  */
 
@@ -4884,15 +5360,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":77
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":115
  *         return self.subtract(other)
  * 
  *     def __rsub__(Vector self, Vector other):             # <<<<<<<<<<<<<<
  *         return self.subtract(other)
  * 
  */
 
@@ -4903,15 +5379,16 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__rsub__ (wrapper)", 0);
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_other), __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector, 1, "other", 0))) __PYX_ERR(0, 77, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_self), __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector, 1, "self", 0))) __PYX_ERR(0, 115, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_other), __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector, 1, "other", 0))) __PYX_ERR(0, 115, __pyx_L1_error)
   __pyx_r = __pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_6Vector_10__rsub__(((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_self), ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_other));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4924,29 +5401,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__rsub__", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":78
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":116
  * 
  *     def __rsub__(Vector self, Vector other):
  *         return self.subtract(other)             # <<<<<<<<<<<<<<
  * 
  *     def __isub__(Vector self, Vector other):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_self->__pyx_vtab)->subtract(__pyx_v_self, __pyx_v_other)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_self->__pyx_vtab)->subtract(__pyx_v_self, __pyx_v_other)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":77
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":115
  *         return self.subtract(other)
  * 
  *     def __rsub__(Vector self, Vector other):             # <<<<<<<<<<<<<<
  *         return self.subtract(other)
  * 
  */
 
@@ -4957,15 +5434,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":80
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":118
  *         return self.subtract(other)
  * 
  *     def __isub__(Vector self, Vector other):             # <<<<<<<<<<<<<<
  *         return self.subtract(other)
  * 
  */
 
@@ -4976,15 +5453,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__isub__ (wrapper)", 0);
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_other), __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector, 1, "other", 0))) __PYX_ERR(0, 80, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_other), __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector, 1, "other", 0))) __PYX_ERR(0, 118, __pyx_L1_error)
   __pyx_r = __pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_6Vector_12__isub__(((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_self), ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_other));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4997,29 +5474,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__isub__", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":81
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":119
  * 
  *     def __isub__(Vector self, Vector other):
  *         return self.subtract(other)             # <<<<<<<<<<<<<<
  * 
  *     def __mul__(Vector self, object other):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_self->__pyx_vtab)->subtract(__pyx_v_self, __pyx_v_other)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_self->__pyx_vtab)->subtract(__pyx_v_self, __pyx_v_other)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":80
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":118
  *         return self.subtract(other)
  * 
  *     def __isub__(Vector self, Vector other):             # <<<<<<<<<<<<<<
  *         return self.subtract(other)
  * 
  */
 
@@ -5030,33 +5507,41 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":83
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":121
  *         return self.subtract(other)
  * 
  *     def __mul__(Vector self, object other):             # <<<<<<<<<<<<<<
  *         if isinstance(other, (int, float)):
  *             return self.mul_by_const(other)
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_6Vector_15__mul__(PyObject *__pyx_v_self, PyObject *__pyx_v_other); /*proto*/
 static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_6Vector_15__mul__(PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__mul__ (wrapper)", 0);
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_self), __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector, 1, "self", 0))) __PYX_ERR(0, 121, __pyx_L1_error)
   __pyx_r = __pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_6Vector_14__mul__(((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_self), ((PyObject *)__pyx_v_other));
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_6Vector_14__mul__(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_self, PyObject *__pyx_v_other) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
@@ -5065,15 +5550,15 @@
   double __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__mul__", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":84
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":122
  * 
  *     def __mul__(Vector self, object other):
  *         if isinstance(other, (int, float)):             # <<<<<<<<<<<<<<
  *             return self.mul_by_const(other)
  *         if isinstance(other, Vector):
  */
   __pyx_t_2 = PyInt_Check(__pyx_v_other); 
@@ -5083,87 +5568,87 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_2 = PyFloat_Check(__pyx_v_other); 
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":85
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":123
  *     def __mul__(Vector self, object other):
  *         if isinstance(other, (int, float)):
  *             return self.mul_by_const(other)             # <<<<<<<<<<<<<<
  *         if isinstance(other, Vector):
  *             return self.mul_by_vector(other)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __pyx_PyFloat_AsDouble(__pyx_v_other); if (unlikely((__pyx_t_3 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 85, __pyx_L1_error)
-    __pyx_t_4 = ((PyObject *)((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_self->__pyx_vtab)->mul_by_const(__pyx_v_self, __pyx_t_3)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 85, __pyx_L1_error)
+    __pyx_t_3 = __pyx_PyFloat_AsDouble(__pyx_v_other); if (unlikely((__pyx_t_3 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 123, __pyx_L1_error)
+    __pyx_t_4 = ((PyObject *)((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_self->__pyx_vtab)->mul_by_const(__pyx_v_self, __pyx_t_3)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 123, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":84
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":122
  * 
  *     def __mul__(Vector self, object other):
  *         if isinstance(other, (int, float)):             # <<<<<<<<<<<<<<
  *             return self.mul_by_const(other)
  *         if isinstance(other, Vector):
  */
   }
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":86
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":124
  *         if isinstance(other, (int, float)):
  *             return self.mul_by_const(other)
  *         if isinstance(other, Vector):             # <<<<<<<<<<<<<<
  *             return self.mul_by_vector(other)
  *         raise TypeError(other)
  */
   __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_other, __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector); 
   if (__pyx_t_1) {
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":87
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":125
  *             return self.mul_by_const(other)
  *         if isinstance(other, Vector):
  *             return self.mul_by_vector(other)             # <<<<<<<<<<<<<<
  *         raise TypeError(other)
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    if (!(likely(((__pyx_v_other) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_other, __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector))))) __PYX_ERR(0, 87, __pyx_L1_error)
-    __pyx_t_3 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_self->__pyx_vtab)->mul_by_vector(__pyx_v_self, ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_other)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 87, __pyx_L1_error)
-    __pyx_t_4 = PyFloat_FromDouble(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 87, __pyx_L1_error)
+    if (!(likely(((__pyx_v_other) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_other, __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector))))) __PYX_ERR(0, 125, __pyx_L1_error)
+    __pyx_t_3 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_self->__pyx_vtab)->mul_by_vector(__pyx_v_self, ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_other)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 125, __pyx_L1_error)
+    __pyx_t_4 = PyFloat_FromDouble(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 125, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":86
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":124
  *         if isinstance(other, (int, float)):
  *             return self.mul_by_const(other)
  *         if isinstance(other, Vector):             # <<<<<<<<<<<<<<
  *             return self.mul_by_vector(other)
  *         raise TypeError(other)
  */
   }
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":88
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":126
  *         if isinstance(other, Vector):
  *             return self.mul_by_vector(other)
  *         raise TypeError(other)             # <<<<<<<<<<<<<<
  * 
  *     def __rmul__(Vector self, object other):
  */
-  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_v_other); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_v_other); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_Raise(__pyx_t_4, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __PYX_ERR(0, 88, __pyx_L1_error)
+  __PYX_ERR(0, 126, __pyx_L1_error)
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":83
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":121
  *         return self.subtract(other)
  * 
  *     def __mul__(Vector self, object other):             # <<<<<<<<<<<<<<
  *         if isinstance(other, (int, float)):
  *             return self.mul_by_const(other)
  */
 
@@ -5174,33 +5659,41 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":90
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":128
  *         raise TypeError(other)
  * 
  *     def __rmul__(Vector self, object other):             # <<<<<<<<<<<<<<
  *         return self.__mul__(other)
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_6Vector_17__rmul__(PyObject *__pyx_v_self, PyObject *__pyx_v_other); /*proto*/
 static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_6Vector_17__rmul__(PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__rmul__ (wrapper)", 0);
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_self), __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector, 1, "self", 0))) __PYX_ERR(0, 128, __pyx_L1_error)
   __pyx_r = __pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_6Vector_16__rmul__(((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_self), ((PyObject *)__pyx_v_other));
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_6Vector_16__rmul__(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_self, PyObject *__pyx_v_other) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
@@ -5209,23 +5702,23 @@
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__rmul__", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":91
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":129
  * 
  *     def __rmul__(Vector self, object other):
  *         return self.__mul__(other)             # <<<<<<<<<<<<<<
  * 
  *     def __imul__(Vector self, object other):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_mul); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 91, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_mul); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
@@ -5237,23 +5730,23 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_other};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 91, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":90
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":128
  *         raise TypeError(other)
  * 
  *     def __rmul__(Vector self, object other):             # <<<<<<<<<<<<<<
  *         return self.__mul__(other)
  * 
  */
 
@@ -5266,15 +5759,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":93
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":131
  *         return self.__mul__(other)
  * 
  *     def __imul__(Vector self, object other):             # <<<<<<<<<<<<<<
  *         return self.__mul__(other)
  * 
  */
 
@@ -5301,23 +5794,23 @@
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__imul__", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":94
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":132
  * 
  *     def __imul__(Vector self, object other):
  *         return self.__mul__(other)             # <<<<<<<<<<<<<<
  * 
  *     def __neg__(Vector self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_mul); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_mul); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 132, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
@@ -5329,23 +5822,23 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_other};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 132, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":93
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":131
  *         return self.__mul__(other)
  * 
  *     def __imul__(Vector self, object other):             # <<<<<<<<<<<<<<
  *         return self.__mul__(other)
  * 
  */
 
@@ -5358,15 +5851,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":96
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":134
  *         return self.__mul__(other)
  * 
  *     def __neg__(Vector self):             # <<<<<<<<<<<<<<
  *         return self.negate()
  * 
  */
 
@@ -5390,29 +5883,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__neg__", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":97
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":135
  * 
  *     def __neg__(Vector self):
  *         return self.negate()             # <<<<<<<<<<<<<<
  * 
  * cdef class TrajectoryCalc:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_self->__pyx_vtab)->negate(__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_self->__pyx_vtab)->negate(__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":96
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":134
  *         return self.__mul__(other)
  * 
  *     def __neg__(Vector self):             # <<<<<<<<<<<<<<
  *         return self.negate()
  * 
  */
 
@@ -5438,15 +5931,14 @@
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
 PyDoc_STRVAR(__pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_6Vector_22__reduce_cython__, "Vector.__reduce_cython__(self)");
-static PyMethodDef __pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_6Vector_23__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_6Vector_23__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_6Vector_22__reduce_cython__};
 static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_6Vector_23__reduce_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
@@ -5519,15 +6011,14 @@
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
 PyDoc_STRVAR(__pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_6Vector_24__setstate_cython__, "Vector.__setstate_cython__(self, __pyx_state)");
-static PyMethodDef __pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_6Vector_25__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_6Vector_25__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_6Vector_24__setstate_cython__};
 static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_6Vector_25__setstate_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
@@ -5639,15 +6130,15 @@
   __Pyx_AddTraceback("py_ballisticcalc_exts.trajectory_calc.Vector.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":121
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":159
  *         double stability_coefficient
  * 
  *     def __init__(self, ammo: Ammo):             # <<<<<<<<<<<<<<
  *         self.ammo = ammo
  *         self._bc = self.ammo.dm.BC
  */
 
@@ -5683,31 +6174,31 @@
       kw_args = __Pyx_NumKwargs_VARARGS(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_ammo)) != 0)) {
           (void)__Pyx_Arg_NewRef_VARARGS(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 121, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 159, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 121, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 159, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
     }
     __pyx_v_ammo = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 121, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 159, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
@@ -5737,110 +6228,110 @@
   PyObject *__pyx_t_2 = NULL;
   double __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":122
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":160
  * 
  *     def __init__(self, ammo: Ammo):
  *         self.ammo = ammo             # <<<<<<<<<<<<<<
  *         self._bc = self.ammo.dm.BC
  *         self._table_data = ammo.dm.drag_table
  */
   __Pyx_INCREF(__pyx_v_ammo);
   __Pyx_GIVEREF(__pyx_v_ammo);
   __Pyx_GOTREF(__pyx_v_self->ammo);
   __Pyx_DECREF(__pyx_v_self->ammo);
   __pyx_v_self->ammo = __pyx_v_ammo;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":123
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":161
  *     def __init__(self, ammo: Ammo):
  *         self.ammo = ammo
  *         self._bc = self.ammo.dm.BC             # <<<<<<<<<<<<<<
  *         self._table_data = ammo.dm.drag_table
  *         self._curve = calculate_curve(self._table_data)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->ammo, __pyx_n_s_dm); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 123, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->ammo, __pyx_n_s_dm); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 161, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_BC); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 123, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_BC); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 161, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_3 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 123, __pyx_L1_error)
+  __pyx_t_3 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_3 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 161, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_self->_bc = __pyx_t_3;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":124
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":162
  *         self.ammo = ammo
  *         self._bc = self.ammo.dm.BC
  *         self._table_data = ammo.dm.drag_table             # <<<<<<<<<<<<<<
  *         self._curve = calculate_curve(self._table_data)
  *         self.gravity_vector = Vector(.0, cGravityConstant, .0)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_ammo, __pyx_n_s_dm); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 124, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_ammo, __pyx_n_s_dm); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 162, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_drag_table); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 124, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_drag_table); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(PyList_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("list", __pyx_t_1))) __PYX_ERR(0, 124, __pyx_L1_error)
+  if (!(likely(PyList_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("list", __pyx_t_1))) __PYX_ERR(0, 162, __pyx_L1_error)
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->_table_data);
   __Pyx_DECREF(__pyx_v_self->_table_data);
   __pyx_v_self->_table_data = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":125
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":163
  *         self._bc = self.ammo.dm.BC
  *         self._table_data = ammo.dm.drag_table
  *         self._curve = calculate_curve(self._table_data)             # <<<<<<<<<<<<<<
  *         self.gravity_vector = Vector(.0, cGravityConstant, .0)
  * 
  */
   __pyx_t_1 = __pyx_v_self->_table_data;
   __Pyx_INCREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_calculate_curve(((PyObject*)__pyx_t_1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 125, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_calculate_curve(((PyObject*)__pyx_t_1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_self->_curve);
   __Pyx_DECREF(__pyx_v_self->_curve);
   __pyx_v_self->_curve = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":126
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":164
  *         self._table_data = ammo.dm.drag_table
  *         self._curve = calculate_curve(self._table_data)
  *         self.gravity_vector = Vector(.0, cGravityConstant, .0)             # <<<<<<<<<<<<<<
  * 
- *     cdef double get_calc_step(self, double step = 0):
+ *     def zero_angle(self, shot_info: Shot, distance: Distance):
  */
-  __pyx_t_2 = PyFloat_FromDouble(__pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cGravityConstant); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble(__pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cGravityConstant); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_float__0);
   __Pyx_GIVEREF(__pyx_float__0);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_float__0)) __PYX_ERR(0, 126, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_float__0)) __PYX_ERR(0, 164, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2)) __PYX_ERR(0, 126, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2)) __PYX_ERR(0, 164, __pyx_L1_error);
   __Pyx_INCREF(__pyx_float__0);
   __Pyx_GIVEREF(__pyx_float__0);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_float__0)) __PYX_ERR(0, 126, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_float__0)) __PYX_ERR(0, 164, __pyx_L1_error);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF((PyObject *)__pyx_v_self->gravity_vector);
   __Pyx_DECREF((PyObject *)__pyx_v_self->gravity_vector);
   __pyx_v_self->gravity_vector = ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":121
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":159
  *         double stability_coefficient
  * 
  *     def __init__(self, ammo: Ammo):             # <<<<<<<<<<<<<<
  *         self.ammo = ammo
  *         self._bc = self.ammo.dm.BC
  */
 
@@ -5853,202 +6344,31 @@
   __Pyx_AddTraceback("py_ballisticcalc_exts.trajectory_calc.TrajectoryCalc.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":128
- *         self.gravity_vector = Vector(.0, cGravityConstant, .0)
- * 
- *     cdef double get_calc_step(self, double step = 0):             # <<<<<<<<<<<<<<
- *         if step == 0:
- *             return Settings.get_max_calc_step_size() / 2.0
- */
-
-static double __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_get_calc_step(CYTHON_UNUSED struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, struct __pyx_opt_args_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_get_calc_step *__pyx_optional_args) {
-  double __pyx_v_step = ((double)0.0);
-  double __pyx_r;
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
-  int __pyx_t_5;
-  double __pyx_t_6;
-  PyObject *__pyx_t_7 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("get_calc_step", 1);
-  if (__pyx_optional_args) {
-    if (__pyx_optional_args->__pyx_n > 0) {
-      __pyx_v_step = __pyx_optional_args->step;
-    }
-  }
-
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":129
- * 
- *     cdef double get_calc_step(self, double step = 0):
- *         if step == 0:             # <<<<<<<<<<<<<<
- *             return Settings.get_max_calc_step_size() / 2.0
- *         return min(step, Settings.get_max_calc_step_size()) / 2.0
- */
-  __pyx_t_1 = (__pyx_v_step == 0.0);
-  if (__pyx_t_1) {
-
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":130
- *     cdef double get_calc_step(self, double step = 0):
- *         if step == 0:
- *             return Settings.get_max_calc_step_size() / 2.0             # <<<<<<<<<<<<<<
- *         return min(step, Settings.get_max_calc_step_size()) / 2.0
- * 
- */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Settings); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 130, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_get_max_calc_step_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 130, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = NULL;
-    __pyx_t_5 = 0;
-    #if CYTHON_UNPACK_METHODS
-    if (unlikely(PyMethod_Check(__pyx_t_4))) {
-      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
-      if (likely(__pyx_t_3)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-        __Pyx_INCREF(__pyx_t_3);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_4, function);
-        __pyx_t_5 = 1;
-      }
-    }
-    #endif
-    {
-      PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
-      __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
-      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 130, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    }
-    __pyx_t_4 = __Pyx_PyFloat_TrueDivideObjC(__pyx_t_2, __pyx_float_2_0, 2.0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 130, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_6 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_6 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 130, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_r = __pyx_t_6;
-    goto __pyx_L0;
-
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":129
- * 
- *     cdef double get_calc_step(self, double step = 0):
- *         if step == 0:             # <<<<<<<<<<<<<<
- *             return Settings.get_max_calc_step_size() / 2.0
- *         return min(step, Settings.get_max_calc_step_size()) / 2.0
- */
-  }
-
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":131
- *         if step == 0:
- *             return Settings.get_max_calc_step_size() / 2.0
- *         return min(step, Settings.get_max_calc_step_size()) / 2.0             # <<<<<<<<<<<<<<
- * 
- *     def zero_angle(self, shot_info: Shot, distance: Distance):
- */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Settings); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 131, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get_max_calc_step_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 131, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = NULL;
-  __pyx_t_5 = 0;
-  #if CYTHON_UNPACK_METHODS
-  if (unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_2)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_2);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-      __pyx_t_5 = 1;
-    }
-  }
-  #endif
-  {
-    PyObject *__pyx_callargs[2] = {__pyx_t_2, NULL};
-    __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 131, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  }
-  __pyx_t_6 = __pyx_v_step;
-  __pyx_t_2 = PyFloat_FromDouble(__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 131, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_7 = PyObject_RichCompare(__pyx_t_4, __pyx_t_2, Py_LT); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 131, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 131, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (__pyx_t_1) {
-    __Pyx_INCREF(__pyx_t_4);
-    __pyx_t_3 = __pyx_t_4;
-  } else {
-    __pyx_t_7 = PyFloat_FromDouble(__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 131, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_3 = __pyx_t_7;
-    __pyx_t_7 = 0;
-  }
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyFloat_TrueDivideObjC(__pyx_t_3, __pyx_float_2_0, 2.0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 131, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_6 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_6 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 131, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_r = __pyx_t_6;
-  goto __pyx_L0;
-
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":128
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":166
  *         self.gravity_vector = Vector(.0, cGravityConstant, .0)
  * 
- *     cdef double get_calc_step(self, double step = 0):             # <<<<<<<<<<<<<<
- *         if step == 0:
- *             return Settings.get_max_calc_step_size() / 2.0
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_AddTraceback("py_ballisticcalc_exts.trajectory_calc.TrajectoryCalc.get_calc_step", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":133
- *         return min(step, Settings.get_max_calc_step_size()) / 2.0
- * 
  *     def zero_angle(self, shot_info: Shot, distance: Distance):             # <<<<<<<<<<<<<<
  *         return self._zero_angle(shot_info, distance)
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_3zero_angle(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
 PyDoc_STRVAR(__pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_2zero_angle, "TrajectoryCalc.zero_angle(self, shot_info: Shot, distance: Distance)");
-static PyMethodDef __pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_3zero_angle = {"zero_angle", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_3zero_angle, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_2zero_angle};
 static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_3zero_angle(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
@@ -6088,43 +6408,43 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_shot_info)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 133, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 166, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_distance)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 133, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 166, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("zero_angle", 1, 2, 2, 1); __PYX_ERR(0, 133, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("zero_angle", 1, 2, 2, 1); __PYX_ERR(0, 166, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "zero_angle") < 0)) __PYX_ERR(0, 133, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "zero_angle") < 0)) __PYX_ERR(0, 166, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_shot_info = values[0];
     __pyx_v_distance = values[1];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("zero_angle", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 133, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("zero_angle", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 166, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -6152,30 +6472,30 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("zero_angle", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":134
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":167
  * 
  *     def zero_angle(self, shot_info: Shot, distance: Distance):
  *         return self._zero_angle(shot_info, distance)             # <<<<<<<<<<<<<<
  * 
  *     def trajectory(self, shot_info: Shot, max_range: Distance, dist_step: Distance,
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self->__pyx_vtab)->_zero_angle(__pyx_v_self, __pyx_v_shot_info, __pyx_v_distance); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 134, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self->__pyx_vtab)->_zero_angle(__pyx_v_self, __pyx_v_shot_info, __pyx_v_distance); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":133
- *         return min(step, Settings.get_max_calc_step_size()) / 2.0
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":166
+ *         self.gravity_vector = Vector(.0, cGravityConstant, .0)
  * 
  *     def zero_angle(self, shot_info: Shot, distance: Distance):             # <<<<<<<<<<<<<<
  *         return self._zero_angle(shot_info, distance)
  * 
  */
 
   /* function exit code */
@@ -6185,15 +6505,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":136
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":169
  *         return self._zero_angle(shot_info, distance)
  * 
  *     def trajectory(self, shot_info: Shot, max_range: Distance, dist_step: Distance,             # <<<<<<<<<<<<<<
  *                    extra_data: bool = False):
  *         cdef:
  */
 
@@ -6202,15 +6522,14 @@
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
 PyDoc_STRVAR(__pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_4trajectory, "TrajectoryCalc.trajectory(self, shot_info: Shot, max_range: Distance, dist_step: Distance, extra_data: bool = False)");
-static PyMethodDef __pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_5trajectory = {"trajectory", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_5trajectory, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_4trajectory};
 static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_5trajectory(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
@@ -6236,20 +6555,20 @@
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_shot_info,&__pyx_n_s_max_range,&__pyx_n_s_dist_step,&__pyx_n_s_extra_data,0};
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":137
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":170
  * 
  *     def trajectory(self, shot_info: Shot, max_range: Distance, dist_step: Distance,
  *                    extra_data: bool = False):             # <<<<<<<<<<<<<<
  *         cdef:
- *             object step = PreferredUnits.distance(dist_step)
+ *             # object atmo = shot_info.atmo
  */
     values[3] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)Py_False));
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
@@ -6265,47 +6584,47 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_shot_info)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 136, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 169, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_max_range)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 136, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 169, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("trajectory", 0, 3, 4, 1); __PYX_ERR(0, 136, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("trajectory", 0, 3, 4, 1); __PYX_ERR(0, 169, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_dist_step)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 136, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 169, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("trajectory", 0, 3, 4, 2); __PYX_ERR(0, 136, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("trajectory", 0, 3, 4, 2); __PYX_ERR(0, 169, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_extra_data);
           if (value) { values[3] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 136, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 169, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "trajectory") < 0)) __PYX_ERR(0, 136, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "trajectory") < 0)) __PYX_ERR(0, 169, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
@@ -6317,15 +6636,15 @@
     __pyx_v_shot_info = values[0];
     __pyx_v_max_range = values[1];
     __pyx_v_dist_step = values[2];
     __pyx_v_extra_data = values[3];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("trajectory", 0, 3, 4, __pyx_nargs); __PYX_ERR(0, 136, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("trajectory", 0, 3, 4, __pyx_nargs); __PYX_ERR(0, 169, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -6333,15 +6652,15 @@
   }
   __Pyx_AddTraceback("py_ballisticcalc_exts.trajectory_calc.TrajectoryCalc.trajectory", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_4trajectory(((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self), __pyx_v_shot_info, __pyx_v_max_range, __pyx_v_dist_step, __pyx_v_extra_data);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":136
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":169
  *         return self._zero_angle(shot_info, distance)
  * 
  *     def trajectory(self, shot_info: Shot, max_range: Distance, dist_step: Distance,             # <<<<<<<<<<<<<<
  *                    extra_data: bool = False):
  *         cdef:
  */
 
@@ -6353,17 +6672,14 @@
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_4trajectory(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, PyObject *__pyx_v_shot_info, PyObject *__pyx_v_max_range, PyObject *__pyx_v_dist_step, PyObject *__pyx_v_extra_data) {
-  CYTHON_UNUSED PyObject *__pyx_v_step = 0;
-  CYTHON_UNUSED PyObject *__pyx_v_atmo = 0;
-  CYTHON_UNUSED PyObject *__pyx_v_winds = 0;
   enum __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag __pyx_v_filter_flags;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
@@ -6372,24 +6688,33 @@
   double __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("trajectory", 0);
   __Pyx_INCREF(__pyx_v_dist_step);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":139
- *                    extra_data: bool = False):
- *         cdef:
- *             object step = PreferredUnits.distance(dist_step)             # <<<<<<<<<<<<<<
- *             object atmo = shot_info.atmo
- *             list winds = shot_info.winds
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":174
+ *             # object atmo = shot_info.atmo
+ *             # list winds = shot_info.winds
+ *             CTrajFlag filter_flags = CTrajFlag.RANGE             # <<<<<<<<<<<<<<
+ * 
+ *         dist_step = PreferredUnits.distance(dist_step)  #  was unused there ???
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_PreferredUnits); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 139, __pyx_L1_error)
+  __pyx_v_filter_flags = __pyx_e_21py_ballisticcalc_exts_15trajectory_calc_RANGE;
+
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":176
+ *             CTrajFlag filter_flags = CTrajFlag.RANGE
+ * 
+ *         dist_step = PreferredUnits.distance(dist_step)  #  was unused there ???             # <<<<<<<<<<<<<<
+ * 
+ *         if extra_data:
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_PreferredUnits); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 176, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_distance); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 139, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_distance); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 176, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
@@ -6402,75 +6727,41 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_v_dist_step};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 139, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 176, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __pyx_v_step = __pyx_t_1;
-  __pyx_t_1 = 0;
-
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":140
- *         cdef:
- *             object step = PreferredUnits.distance(dist_step)
- *             object atmo = shot_info.atmo             # <<<<<<<<<<<<<<
- *             list winds = shot_info.winds
- *             CTrajFlag filter_flags = CTrajFlag.RANGE
- */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_atmo); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 140, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_v_atmo = __pyx_t_1;
+  __Pyx_DECREF_SET(__pyx_v_dist_step, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":141
- *             object step = PreferredUnits.distance(dist_step)
- *             object atmo = shot_info.atmo
- *             list winds = shot_info.winds             # <<<<<<<<<<<<<<
- *             CTrajFlag filter_flags = CTrajFlag.RANGE
- * 
- */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_winds); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 141, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(PyList_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("list", __pyx_t_1))) __PYX_ERR(0, 141, __pyx_L1_error)
-  __pyx_v_winds = ((PyObject*)__pyx_t_1);
-  __pyx_t_1 = 0;
-
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":142
- *             object atmo = shot_info.atmo
- *             list winds = shot_info.winds
- *             CTrajFlag filter_flags = CTrajFlag.RANGE             # <<<<<<<<<<<<<<
- * 
- *         if extra_data:
- */
-  __pyx_v_filter_flags = __pyx_e_21py_ballisticcalc_exts_15trajectory_calc_RANGE;
-
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":144
- *             CTrajFlag filter_flags = CTrajFlag.RANGE
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":178
+ *         dist_step = PreferredUnits.distance(dist_step)  #  was unused there ???
  * 
  *         if extra_data:             # <<<<<<<<<<<<<<
  *             dist_step = Distance.Foot(0.2)
  *             filter_flags = CTrajFlag.ALL
  */
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_extra_data); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 144, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_extra_data); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 178, __pyx_L1_error)
   if (__pyx_t_5) {
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":145
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":179
  * 
  *         if extra_data:
  *             dist_step = Distance.Foot(0.2)             # <<<<<<<<<<<<<<
  *             filter_flags = CTrajFlag.ALL
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Distance); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 145, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Distance); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 179, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Foot); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 145, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Foot); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 179, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     __pyx_t_4 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
@@ -6483,85 +6774,85 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_float_0_2};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 145, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __Pyx_DECREF_SET(__pyx_v_dist_step, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":146
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":180
  *         if extra_data:
  *             dist_step = Distance.Foot(0.2)
  *             filter_flags = CTrajFlag.ALL             # <<<<<<<<<<<<<<
  * 
  *         self._init_trajectory(shot_info)
  */
     __pyx_v_filter_flags = __pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ALL;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":144
- *             CTrajFlag filter_flags = CTrajFlag.RANGE
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":178
+ *         dist_step = PreferredUnits.distance(dist_step)  #  was unused there ???
  * 
  *         if extra_data:             # <<<<<<<<<<<<<<
  *             dist_step = Distance.Foot(0.2)
  *             filter_flags = CTrajFlag.ALL
  */
   }
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":148
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":182
  *             filter_flags = CTrajFlag.ALL
  * 
  *         self._init_trajectory(shot_info)             # <<<<<<<<<<<<<<
  *         return self._trajectory(shot_info, max_range >> Distance.Foot, dist_step >> Distance.Foot, filter_flags)
  * 
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self->__pyx_vtab)->_init_trajectory(__pyx_v_self, __pyx_v_shot_info); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self->__pyx_vtab)->_init_trajectory(__pyx_v_self, __pyx_v_shot_info); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 182, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":149
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":183
  * 
  *         self._init_trajectory(shot_info)
  *         return self._trajectory(shot_info, max_range >> Distance.Foot, dist_step >> Distance.Foot, filter_flags)             # <<<<<<<<<<<<<<
  * 
  *     cdef _init_trajectory(self, shot_info: Shot):
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Distance); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Distance); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Foot); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Foot); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Rshift(__pyx_v_max_range, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Rshift(__pyx_v_max_range, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_6 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_6 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_t_6 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_6 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Distance); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Distance); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Foot); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Foot); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Rshift(__pyx_v_dist_step, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Rshift(__pyx_v_dist_step, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_7 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_7 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_t_7 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_7 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self->__pyx_vtab)->_trajectory(__pyx_v_self, __pyx_v_shot_info, __pyx_t_6, __pyx_t_7, __pyx_v_filter_flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self->__pyx_vtab)->_trajectory(__pyx_v_self, __pyx_v_shot_info, __pyx_t_6, __pyx_t_7, __pyx_v_filter_flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":136
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":169
  *         return self._zero_angle(shot_info, distance)
  * 
  *     def trajectory(self, shot_info: Shot, max_range: Distance, dist_step: Distance,             # <<<<<<<<<<<<<<
  *                    extra_data: bool = False):
  *         cdef:
  */
 
@@ -6569,24 +6860,21 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_AddTraceback("py_ballisticcalc_exts.trajectory_calc.TrajectoryCalc.trajectory", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_step);
-  __Pyx_XDECREF(__pyx_v_atmo);
-  __Pyx_XDECREF(__pyx_v_winds);
   __Pyx_XDECREF(__pyx_v_dist_step);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":151
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":185
  *         return self._trajectory(shot_info, max_range >> Distance.Foot, dist_step >> Distance.Foot, filter_flags)
  * 
  *     cdef _init_trajectory(self, shot_info: Shot):             # <<<<<<<<<<<<<<
  *         self.look_angle = shot_info.look_angle >> Angular.Radian
  *         self.twist = shot_info.weapon.twist >> Distance.Inch
  */
 
@@ -6601,414 +6889,408 @@
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_init_trajectory", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":152
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":186
  * 
  *     cdef _init_trajectory(self, shot_info: Shot):
  *         self.look_angle = shot_info.look_angle >> Angular.Radian             # <<<<<<<<<<<<<<
  *         self.twist = shot_info.weapon.twist >> Distance.Inch
  *         self.length = shot_info.ammo.dm.length >> Distance.Inch
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_look_angle); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_look_angle); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 186, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Angular); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Angular); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 186, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_Radian); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_Radian); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 186, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Rshift(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Rshift(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 186, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 186, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_self->look_angle = __pyx_t_4;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":153
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":187
  *     cdef _init_trajectory(self, shot_info: Shot):
  *         self.look_angle = shot_info.look_angle >> Angular.Radian
  *         self.twist = shot_info.weapon.twist >> Distance.Inch             # <<<<<<<<<<<<<<
  *         self.length = shot_info.ammo.dm.length >> Distance.Inch
  *         self.diameter = shot_info.ammo.dm.diameter >> Distance.Inch
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_weapon); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 153, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_weapon); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_twist); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 153, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_twist); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Distance); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 153, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Distance); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_Inch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 153, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_Inch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Rshift(__pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 153, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Rshift(__pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 153, __pyx_L1_error)
+  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_self->twist = __pyx_t_4;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":154
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":188
  *         self.look_angle = shot_info.look_angle >> Angular.Radian
  *         self.twist = shot_info.weapon.twist >> Distance.Inch
  *         self.length = shot_info.ammo.dm.length >> Distance.Inch             # <<<<<<<<<<<<<<
  *         self.diameter = shot_info.ammo.dm.diameter >> Distance.Inch
  *         self.weight = shot_info.ammo.dm.weight >> Weight.Grain
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_ammo); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_ammo); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_dm); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_dm); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_length); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_length); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Distance); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Distance); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Inch); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Inch); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Rshift(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Rshift(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 154, __pyx_L1_error)
+  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_self->length = __pyx_t_4;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":155
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":189
  *         self.twist = shot_info.weapon.twist >> Distance.Inch
  *         self.length = shot_info.ammo.dm.length >> Distance.Inch
  *         self.diameter = shot_info.ammo.dm.diameter >> Distance.Inch             # <<<<<<<<<<<<<<
  *         self.weight = shot_info.ammo.dm.weight >> Weight.Grain
  *         self.barrel_elevation = shot_info.barrel_elevation >> Angular.Radian
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_ammo); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_ammo); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_dm); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_dm); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_diameter); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_diameter); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Distance); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Distance); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Inch); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Inch); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyNumber_Rshift(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Rshift(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 155, __pyx_L1_error)
+  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_self->diameter = __pyx_t_4;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":156
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":190
  *         self.length = shot_info.ammo.dm.length >> Distance.Inch
  *         self.diameter = shot_info.ammo.dm.diameter >> Distance.Inch
  *         self.weight = shot_info.ammo.dm.weight >> Weight.Grain             # <<<<<<<<<<<<<<
  *         self.barrel_elevation = shot_info.barrel_elevation >> Angular.Radian
  *         self.barrel_azimuth = shot_info.barrel_azimuth >> Angular.Radian
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_ammo); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 156, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_ammo); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 190, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_dm); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 156, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_dm); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 190, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_weight); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 156, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_weight); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 190, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Weight); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 156, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Weight); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 190, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_Grain); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 156, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_Grain); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 190, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Rshift(__pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 156, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Rshift(__pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 190, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 156, __pyx_L1_error)
+  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 190, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_self->weight = __pyx_t_4;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":157
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":191
  *         self.diameter = shot_info.ammo.dm.diameter >> Distance.Inch
  *         self.weight = shot_info.ammo.dm.weight >> Weight.Grain
  *         self.barrel_elevation = shot_info.barrel_elevation >> Angular.Radian             # <<<<<<<<<<<<<<
  *         self.barrel_azimuth = shot_info.barrel_azimuth >> Angular.Radian
  *         self.sight_height = shot_info.weapon.sight_height >> Distance.Foot
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_barrel_elevation); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 157, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_barrel_elevation); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Angular); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 157, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Angular); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Radian); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 157, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Radian); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Rshift(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 157, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Rshift(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 157, __pyx_L1_error)
+  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_self->barrel_elevation = __pyx_t_4;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":158
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":192
  *         self.weight = shot_info.ammo.dm.weight >> Weight.Grain
  *         self.barrel_elevation = shot_info.barrel_elevation >> Angular.Radian
  *         self.barrel_azimuth = shot_info.barrel_azimuth >> Angular.Radian             # <<<<<<<<<<<<<<
  *         self.sight_height = shot_info.weapon.sight_height >> Distance.Foot
  *         self.cant_cosine = cos(shot_info.cant_angle >> Angular.Radian)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_barrel_azimuth); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 158, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_barrel_azimuth); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 192, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Angular); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 158, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Angular); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 192, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Radian); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 158, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Radian); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 192, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyNumber_Rshift(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 158, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Rshift(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 192, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 158, __pyx_L1_error)
+  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 192, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_self->barrel_azimuth = __pyx_t_4;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":159
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":193
  *         self.barrel_elevation = shot_info.barrel_elevation >> Angular.Radian
  *         self.barrel_azimuth = shot_info.barrel_azimuth >> Angular.Radian
  *         self.sight_height = shot_info.weapon.sight_height >> Distance.Foot             # <<<<<<<<<<<<<<
  *         self.cant_cosine = cos(shot_info.cant_angle >> Angular.Radian)
  *         self.cant_sine = sin(shot_info.cant_angle >> Angular.Radian)
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_weapon); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 159, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_weapon); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 193, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_sight_height); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 159, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_sight_height); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 193, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Distance); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 159, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Distance); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 193, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Foot); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 159, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Foot); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 193, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyNumber_Rshift(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 159, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Rshift(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 193, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 159, __pyx_L1_error)
+  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 193, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_self->sight_height = __pyx_t_4;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":160
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":194
  *         self.barrel_azimuth = shot_info.barrel_azimuth >> Angular.Radian
  *         self.sight_height = shot_info.weapon.sight_height >> Distance.Foot
  *         self.cant_cosine = cos(shot_info.cant_angle >> Angular.Radian)             # <<<<<<<<<<<<<<
  *         self.cant_sine = sin(shot_info.cant_angle >> Angular.Radian)
  *         self.alt0 = shot_info.atmo.altitude >> Distance.Foot
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_cant_angle); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 160, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_cant_angle); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Angular); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 160, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Angular); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Radian); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 160, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Radian); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Rshift(__pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 160, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Rshift(__pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 160, __pyx_L1_error)
+  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_self->cant_cosine = cos(__pyx_t_4);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":161
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":195
  *         self.sight_height = shot_info.weapon.sight_height >> Distance.Foot
  *         self.cant_cosine = cos(shot_info.cant_angle >> Angular.Radian)
  *         self.cant_sine = sin(shot_info.cant_angle >> Angular.Radian)             # <<<<<<<<<<<<<<
  *         self.alt0 = shot_info.atmo.altitude >> Distance.Foot
- *         self.calc_step = self.get_calc_step()
+ *         self.calc_step = get_calc_step()
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_cant_angle); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_cant_angle); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 195, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Angular); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Angular); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 195, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_Radian); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_Radian); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 195, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Rshift(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Rshift(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 195, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 161, __pyx_L1_error)
+  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 195, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_self->cant_sine = sin(__pyx_t_4);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":162
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":196
  *         self.cant_cosine = cos(shot_info.cant_angle >> Angular.Radian)
  *         self.cant_sine = sin(shot_info.cant_angle >> Angular.Radian)
  *         self.alt0 = shot_info.atmo.altitude >> Distance.Foot             # <<<<<<<<<<<<<<
- *         self.calc_step = self.get_calc_step()
- *         if Settings.USE_POWDER_SENSITIVITY:
+ *         self.calc_step = get_calc_step()
+ *         if _globalUsePowderSensitivity:
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_atmo); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 162, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_atmo); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_altitude); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 162, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_altitude); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Distance); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 162, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Distance); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_Foot); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_Foot); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Rshift(__pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 162, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Rshift(__pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 162, __pyx_L1_error)
+  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_self->alt0 = __pyx_t_4;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":163
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":197
  *         self.cant_sine = sin(shot_info.cant_angle >> Angular.Radian)
  *         self.alt0 = shot_info.atmo.altitude >> Distance.Foot
- *         self.calc_step = self.get_calc_step()             # <<<<<<<<<<<<<<
- *         if Settings.USE_POWDER_SENSITIVITY:
+ *         self.calc_step = get_calc_step()             # <<<<<<<<<<<<<<
+ *         if _globalUsePowderSensitivity:
  *             self.muzzle_velocity = shot_info.ammo.get_velocity_for_temp(shot_info.atmo.temperature) >> Velocity.FPS
  */
-  __pyx_t_4 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self->__pyx_vtab)->get_calc_step(__pyx_v_self, NULL); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 163, __pyx_L1_error)
+  __pyx_t_4 = __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_get_calc_step(NULL); if (unlikely(__pyx_t_4 == ((double)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L1_error)
   __pyx_v_self->calc_step = __pyx_t_4;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":164
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":198
  *         self.alt0 = shot_info.atmo.altitude >> Distance.Foot
- *         self.calc_step = self.get_calc_step()
- *         if Settings.USE_POWDER_SENSITIVITY:             # <<<<<<<<<<<<<<
+ *         self.calc_step = get_calc_step()
+ *         if _globalUsePowderSensitivity:             # <<<<<<<<<<<<<<
  *             self.muzzle_velocity = shot_info.ammo.get_velocity_for_temp(shot_info.atmo.temperature) >> Velocity.FPS
  *         else:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Settings); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 164, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_USE_POWDER_SENSITIVITY); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 164, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_5 = (__pyx_v_21py_ballisticcalc_exts_15trajectory_calc__globalUsePowderSensitivity != 0);
   if (__pyx_t_5) {
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":165
- *         self.calc_step = self.get_calc_step()
- *         if Settings.USE_POWDER_SENSITIVITY:
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":199
+ *         self.calc_step = get_calc_step()
+ *         if _globalUsePowderSensitivity:
  *             self.muzzle_velocity = shot_info.ammo.get_velocity_for_temp(shot_info.atmo.temperature) >> Velocity.FPS             # <<<<<<<<<<<<<<
  *         else:
  *             self.muzzle_velocity = shot_info.ammo.mv >> Velocity.FPS
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_ammo); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get_velocity_for_temp); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 165, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_ammo); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 199, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_get_velocity_for_temp); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 199, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_atmo); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_temperature); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 165, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_atmo); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 199, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_temperature); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 199, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = NULL;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = NULL;
     __pyx_t_7 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_3))) {
-      __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
-      if (likely(__pyx_t_2)) {
+      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
+      if (likely(__pyx_t_1)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-        __Pyx_INCREF(__pyx_t_2);
+        __Pyx_INCREF(__pyx_t_1);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
         __pyx_t_7 = 1;
       }
     }
     #endif
     {
-      PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_t_6};
-      __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
-      __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+      PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_t_6};
+      __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
+      __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Velocity); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 165, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Velocity); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 199, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_FPS); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 165, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_FPS); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 199, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyNumber_Rshift(__pyx_t_1, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 165, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Rshift(__pyx_t_2, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 199, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 165, __pyx_L1_error)
+    __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 199, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_self->muzzle_velocity = __pyx_t_4;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":164
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":198
  *         self.alt0 = shot_info.atmo.altitude >> Distance.Foot
- *         self.calc_step = self.get_calc_step()
- *         if Settings.USE_POWDER_SENSITIVITY:             # <<<<<<<<<<<<<<
+ *         self.calc_step = get_calc_step()
+ *         if _globalUsePowderSensitivity:             # <<<<<<<<<<<<<<
  *             self.muzzle_velocity = shot_info.ammo.get_velocity_for_temp(shot_info.atmo.temperature) >> Velocity.FPS
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":167
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":201
  *             self.muzzle_velocity = shot_info.ammo.get_velocity_for_temp(shot_info.atmo.temperature) >> Velocity.FPS
  *         else:
  *             self.muzzle_velocity = shot_info.ammo.mv >> Velocity.FPS             # <<<<<<<<<<<<<<
  *         self.stability_coefficient = self.calc_stability_coefficient(shot_info.atmo)
  * 
  */
   /*else*/ {
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_ammo); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 167, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_ammo); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_mv); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 167, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_mv); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Velocity); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 167, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Velocity); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_FPS); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_FPS); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyNumber_Rshift(__pyx_t_6, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 167, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Rshift(__pyx_t_6, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 167, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_self->muzzle_velocity = __pyx_t_4;
   }
   __pyx_L3:;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":168
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":202
  *         else:
  *             self.muzzle_velocity = shot_info.ammo.mv >> Velocity.FPS
  *         self.stability_coefficient = self.calc_stability_coefficient(shot_info.atmo)             # <<<<<<<<<<<<<<
  * 
  *     cdef _zero_angle(TrajectoryCalc self, object shot_info, object distance):
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_atmo); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_atmo); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self->__pyx_vtab)->calc_stability_coefficient(__pyx_v_self, __pyx_t_3); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 168, __pyx_L1_error)
+  __pyx_t_4 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self->__pyx_vtab)->calc_stability_coefficient(__pyx_v_self, __pyx_t_3); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 202, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_self->stability_coefficient = __pyx_t_4;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":151
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":185
  *         return self._trajectory(shot_info, max_range >> Distance.Foot, dist_step >> Distance.Foot, filter_flags)
  * 
  *     cdef _init_trajectory(self, shot_info: Shot):             # <<<<<<<<<<<<<<
  *         self.look_angle = shot_info.look_angle >> Angular.Radian
  *         self.twist = shot_info.weapon.twist >> Distance.Inch
  */
 
@@ -7024,202 +7306,198 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":170
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":204
  *         self.stability_coefficient = self.calc_stability_coefficient(shot_info.atmo)
  * 
  *     cdef _zero_angle(TrajectoryCalc self, object shot_info, object distance):             # <<<<<<<<<<<<<<
  *         cdef:
  *             double zero_distance = cos(shot_info.look_angle >> Angular.Radian) * (distance >> Distance.Foot)
  */
 
 static PyObject *__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc__zero_angle(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, PyObject *__pyx_v_shot_info, PyObject *__pyx_v_distance) {
   double __pyx_v_zero_distance;
   double __pyx_v_height_at_zero;
   double __pyx_v_maximum_range;
   int __pyx_v_iterations_count;
   double __pyx_v_zero_finding_error;
-  PyObject *__pyx_v_t = NULL;
-  PyObject *__pyx_v_height = NULL;
+  PyObject *__pyx_v_t = 0;
+  double __pyx_v_height;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   double __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
-  PyObject *__pyx_t_7 = NULL;
-  Py_ssize_t __pyx_t_8;
-  Py_UCS4 __pyx_t_9;
+  Py_ssize_t __pyx_t_7;
+  Py_UCS4 __pyx_t_8;
+  PyObject *__pyx_t_9 = NULL;
   int __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_zero_angle", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":172
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":206
  *     cdef _zero_angle(TrajectoryCalc self, object shot_info, object distance):
  *         cdef:
  *             double zero_distance = cos(shot_info.look_angle >> Angular.Radian) * (distance >> Distance.Foot)             # <<<<<<<<<<<<<<
  *             double height_at_zero = sin(shot_info.look_angle >> Angular.Radian) * (distance >> Distance.Foot)
  *             double maximum_range = zero_distance
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_look_angle); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_look_angle); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 206, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Angular); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Angular); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 206, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_Radian); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_Radian); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 206, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Rshift(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Rshift(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 206, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 206, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyFloat_FromDouble(cos(__pyx_t_4)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble(cos(__pyx_t_4)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 206, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Distance); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Distance); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 206, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Foot); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Foot); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 206, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyNumber_Rshift(__pyx_v_distance, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Rshift(__pyx_v_distance, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 206, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Multiply(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Multiply(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 206, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 206, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_zero_distance = __pyx_t_4;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":173
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":207
  *         cdef:
  *             double zero_distance = cos(shot_info.look_angle >> Angular.Radian) * (distance >> Distance.Foot)
  *             double height_at_zero = sin(shot_info.look_angle >> Angular.Radian) * (distance >> Distance.Foot)             # <<<<<<<<<<<<<<
  *             double maximum_range = zero_distance
  *             int iterations_count = 0
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_look_angle); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 173, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_look_angle); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 207, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Angular); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 173, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Angular); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 207, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Radian); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 173, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Radian); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 207, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyNumber_Rshift(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 173, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Rshift(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 207, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 173, __pyx_L1_error)
+  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 207, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyFloat_FromDouble(sin(__pyx_t_4)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 173, __pyx_L1_error)
+  __pyx_t_3 = PyFloat_FromDouble(sin(__pyx_t_4)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 207, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Distance); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 173, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Distance); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 207, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_Foot); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 173, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_Foot); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 207, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Rshift(__pyx_v_distance, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 173, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Rshift(__pyx_v_distance, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 207, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Multiply(__pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 173, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Multiply(__pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 207, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 173, __pyx_L1_error)
+  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 207, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_height_at_zero = __pyx_t_4;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":174
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":208
  *             double zero_distance = cos(shot_info.look_angle >> Angular.Radian) * (distance >> Distance.Foot)
  *             double height_at_zero = sin(shot_info.look_angle >> Angular.Radian) * (distance >> Distance.Foot)
  *             double maximum_range = zero_distance             # <<<<<<<<<<<<<<
  *             int iterations_count = 0
  *             double zero_finding_error = cZeroFindingAccuracy * 2
  */
   __pyx_v_maximum_range = __pyx_v_zero_distance;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":175
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":209
  *             double height_at_zero = sin(shot_info.look_angle >> Angular.Radian) * (distance >> Distance.Foot)
  *             double maximum_range = zero_distance
  *             int iterations_count = 0             # <<<<<<<<<<<<<<
  *             double zero_finding_error = cZeroFindingAccuracy * 2
  * 
  */
   __pyx_v_iterations_count = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":176
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":210
  *             double maximum_range = zero_distance
  *             int iterations_count = 0
  *             double zero_finding_error = cZeroFindingAccuracy * 2             # <<<<<<<<<<<<<<
  * 
- *         self._init_trajectory(shot_info)
+ *             object t
  */
   __pyx_v_zero_finding_error = (__pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cZeroFindingAccuracy * 2.0);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":178
- *             double zero_finding_error = cZeroFindingAccuracy * 2
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":215
+ *             double height
  * 
  *         self._init_trajectory(shot_info)             # <<<<<<<<<<<<<<
  *         self.barrel_azimuth = 0.0
  *         self.barrel_elevation = atan(height_at_zero / zero_distance)
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self->__pyx_vtab)->_init_trajectory(__pyx_v_self, __pyx_v_shot_info); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 178, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self->__pyx_vtab)->_init_trajectory(__pyx_v_self, __pyx_v_shot_info); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 215, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":179
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":216
  * 
  *         self._init_trajectory(shot_info)
  *         self.barrel_azimuth = 0.0             # <<<<<<<<<<<<<<
  *         self.barrel_elevation = atan(height_at_zero / zero_distance)
  *         self.twist = 0
  */
   __pyx_v_self->barrel_azimuth = 0.0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":180
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":217
  *         self._init_trajectory(shot_info)
  *         self.barrel_azimuth = 0.0
  *         self.barrel_elevation = atan(height_at_zero / zero_distance)             # <<<<<<<<<<<<<<
  *         self.twist = 0
  *         maximum_range -= 1.5*self.calc_step
  */
-  if (unlikely(__pyx_v_zero_distance == 0)) {
-    PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(0, 180, __pyx_L1_error)
-  }
   __pyx_v_self->barrel_elevation = atan((__pyx_v_height_at_zero / __pyx_v_zero_distance));
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":181
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":218
  *         self.barrel_azimuth = 0.0
  *         self.barrel_elevation = atan(height_at_zero / zero_distance)
  *         self.twist = 0             # <<<<<<<<<<<<<<
  *         maximum_range -= 1.5*self.calc_step
  * 
  */
   __pyx_v_self->twist = 0.0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":182
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":219
  *         self.barrel_elevation = atan(height_at_zero / zero_distance)
  *         self.twist = 0
  *         maximum_range -= 1.5*self.calc_step             # <<<<<<<<<<<<<<
  * 
  *         # x = horizontal distance down range, y = drop, z = windage
  */
   __pyx_v_maximum_range = (__pyx_v_maximum_range - (1.5 * __pyx_v_self->calc_step));
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":185
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":222
  * 
  *         # x = horizontal distance down range, y = drop, z = windage
  *         while zero_finding_error > cZeroFindingAccuracy and iterations_count < cMaxIterations:             # <<<<<<<<<<<<<<
  *             t = self._trajectory(shot_info, maximum_range, zero_distance, CTrajFlag.NONE)[0]
  *             height = t.height >> Distance.Foot
  */
   while (1) {
@@ -7230,302 +7508,277 @@
       goto __pyx_L5_bool_binop_done;
     }
     __pyx_t_6 = (__pyx_v_iterations_count < __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cMaxIterations);
     __pyx_t_5 = __pyx_t_6;
     __pyx_L5_bool_binop_done:;
     if (!__pyx_t_5) break;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":186
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":223
  *         # x = horizontal distance down range, y = drop, z = windage
  *         while zero_finding_error > cZeroFindingAccuracy and iterations_count < cMaxIterations:
  *             t = self._trajectory(shot_info, maximum_range, zero_distance, CTrajFlag.NONE)[0]             # <<<<<<<<<<<<<<
  *             height = t.height >> Distance.Foot
  *             zero_finding_error = fabs(height - height_at_zero)
  */
-    __pyx_t_1 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self->__pyx_vtab)->_trajectory(__pyx_v_self, __pyx_v_shot_info, __pyx_v_maximum_range, __pyx_v_zero_distance, __pyx_e_21py_ballisticcalc_exts_15trajectory_calc_NONE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 186, __pyx_L1_error)
+    __pyx_t_1 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self->__pyx_vtab)->_trajectory(__pyx_v_self, __pyx_v_shot_info, __pyx_v_maximum_range, __pyx_v_zero_distance, __pyx_e_21py_ballisticcalc_exts_15trajectory_calc_NONE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 186, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 223, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF_SET(__pyx_v_t, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":187
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":224
  *         while zero_finding_error > cZeroFindingAccuracy and iterations_count < cMaxIterations:
  *             t = self._trajectory(shot_info, maximum_range, zero_distance, CTrajFlag.NONE)[0]
  *             height = t.height >> Distance.Foot             # <<<<<<<<<<<<<<
  *             zero_finding_error = fabs(height - height_at_zero)
  *             if zero_finding_error > cZeroFindingAccuracy:
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_t, __pyx_n_s_height); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 187, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_t, __pyx_n_s_height); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 224, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Distance); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Distance); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 224, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Foot); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 187, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Foot); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 224, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyNumber_Rshift(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Rshift(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 224, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_height, __pyx_t_1);
-    __pyx_t_1 = 0;
+    __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 224, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_v_height = __pyx_t_4;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":188
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":225
  *             t = self._trajectory(shot_info, maximum_range, zero_distance, CTrajFlag.NONE)[0]
  *             height = t.height >> Distance.Foot
  *             zero_finding_error = fabs(height - height_at_zero)             # <<<<<<<<<<<<<<
  *             if zero_finding_error > cZeroFindingAccuracy:
  *                 self.barrel_elevation -= (height - height_at_zero) / zero_distance
  */
-    __pyx_t_1 = PyFloat_FromDouble(__pyx_v_height_at_zero); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = PyNumber_Subtract(__pyx_v_height, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 188, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 188, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_v_zero_finding_error = fabs(__pyx_t_4);
+    __pyx_v_zero_finding_error = fabs((__pyx_v_height - __pyx_v_height_at_zero));
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":189
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":226
  *             height = t.height >> Distance.Foot
  *             zero_finding_error = fabs(height - height_at_zero)
  *             if zero_finding_error > cZeroFindingAccuracy:             # <<<<<<<<<<<<<<
  *                 self.barrel_elevation -= (height - height_at_zero) / zero_distance
  *             else:  # last barrel_elevation hit zero!
  */
     __pyx_t_5 = (__pyx_v_zero_finding_error > __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cZeroFindingAccuracy);
     if (__pyx_t_5) {
 
-      /* "py_ballisticcalc_exts/trajectory_calc.pyx":190
+      /* "py_ballisticcalc_exts/trajectory_calc.pyx":227
  *             zero_finding_error = fabs(height - height_at_zero)
  *             if zero_finding_error > cZeroFindingAccuracy:
  *                 self.barrel_elevation -= (height - height_at_zero) / zero_distance             # <<<<<<<<<<<<<<
  *             else:  # last barrel_elevation hit zero!
  *                 break
  */
-      __pyx_t_3 = PyFloat_FromDouble(__pyx_v_self->barrel_elevation); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 190, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_1 = PyFloat_FromDouble(__pyx_v_height_at_zero); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 190, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_2 = PyNumber_Subtract(__pyx_v_height, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 190, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = PyFloat_FromDouble(__pyx_v_zero_distance); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 190, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_7 = __Pyx_PyNumber_Divide(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 190, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = PyNumber_InPlaceSubtract(__pyx_t_3, __pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 190, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 190, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_v_self->barrel_elevation = __pyx_t_4;
+      __pyx_v_self->barrel_elevation = (__pyx_v_self->barrel_elevation - ((__pyx_v_height - __pyx_v_height_at_zero) / __pyx_v_zero_distance));
 
-      /* "py_ballisticcalc_exts/trajectory_calc.pyx":189
+      /* "py_ballisticcalc_exts/trajectory_calc.pyx":226
  *             height = t.height >> Distance.Foot
  *             zero_finding_error = fabs(height - height_at_zero)
  *             if zero_finding_error > cZeroFindingAccuracy:             # <<<<<<<<<<<<<<
  *                 self.barrel_elevation -= (height - height_at_zero) / zero_distance
  *             else:  # last barrel_elevation hit zero!
  */
       goto __pyx_L7;
     }
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":192
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":229
  *                 self.barrel_elevation -= (height - height_at_zero) / zero_distance
  *             else:  # last barrel_elevation hit zero!
  *                 break             # <<<<<<<<<<<<<<
  *             iterations_count += 1
  *         if zero_finding_error > cZeroFindingAccuracy:
  */
     /*else*/ {
       goto __pyx_L4_break;
     }
     __pyx_L7:;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":193
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":230
  *             else:  # last barrel_elevation hit zero!
  *                 break
  *             iterations_count += 1             # <<<<<<<<<<<<<<
  *         if zero_finding_error > cZeroFindingAccuracy:
  *             raise Exception(f'Zero vertical error {zero_finding_error} feet, after {iterations_count} iterations.')
  */
     __pyx_v_iterations_count = (__pyx_v_iterations_count + 1);
   }
   __pyx_L4_break:;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":194
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":231
  *                 break
  *             iterations_count += 1
  *         if zero_finding_error > cZeroFindingAccuracy:             # <<<<<<<<<<<<<<
  *             raise Exception(f'Zero vertical error {zero_finding_error} feet, after {iterations_count} iterations.')
  *         return Angular.Radian(self.barrel_elevation)
  */
   __pyx_t_5 = (__pyx_v_zero_finding_error > __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cZeroFindingAccuracy);
   if (unlikely(__pyx_t_5)) {
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":195
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":232
  *             iterations_count += 1
  *         if zero_finding_error > cZeroFindingAccuracy:
  *             raise Exception(f'Zero vertical error {zero_finding_error} feet, after {iterations_count} iterations.')             # <<<<<<<<<<<<<<
  *         return Angular.Radian(self.barrel_elevation)
  * 
  */
-    __pyx_t_1 = PyTuple_New(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 195, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 232, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_8 = 0;
-    __pyx_t_9 = 127;
+    __pyx_t_7 = 0;
+    __pyx_t_8 = 127;
     __Pyx_INCREF(__pyx_kp_u_Zero_vertical_error);
-    __pyx_t_8 += 20;
+    __pyx_t_7 += 20;
     __Pyx_GIVEREF(__pyx_kp_u_Zero_vertical_error);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_Zero_vertical_error);
-    __pyx_t_7 = PyFloat_FromDouble(__pyx_v_zero_finding_error); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 195, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_3 = __Pyx_PyObject_FormatSimple(__pyx_t_7, __pyx_empty_unicode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 195, __pyx_L1_error)
+    __pyx_t_3 = PyFloat_FromDouble(__pyx_v_zero_finding_error); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 232, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_9 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_3) > __pyx_t_9) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_3) : __pyx_t_9;
-    __pyx_t_8 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
-    __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_3);
-    __pyx_t_3 = 0;
+    __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_t_3, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 232, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_8 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) > __pyx_t_8) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) : __pyx_t_8;
+    __pyx_t_7 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_2);
+    __Pyx_GIVEREF(__pyx_t_2);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2);
+    __pyx_t_2 = 0;
     __Pyx_INCREF(__pyx_kp_u_feet_after);
-    __pyx_t_8 += 13;
+    __pyx_t_7 += 13;
     __Pyx_GIVEREF(__pyx_kp_u_feet_after);
     PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u_feet_after);
-    __pyx_t_3 = __Pyx_PyUnicode_From_int(__pyx_v_iterations_count, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 195, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_8 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
-    __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_t_3);
-    __pyx_t_3 = 0;
+    __pyx_t_2 = __Pyx_PyUnicode_From_int(__pyx_v_iterations_count, 0, ' ', 'd'); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 232, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_7 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_2);
+    __Pyx_GIVEREF(__pyx_t_2);
+    PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_t_2);
+    __pyx_t_2 = 0;
     __Pyx_INCREF(__pyx_kp_u_iterations);
-    __pyx_t_8 += 12;
+    __pyx_t_7 += 12;
     __Pyx_GIVEREF(__pyx_kp_u_iterations);
     PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_kp_u_iterations);
-    __pyx_t_3 = __Pyx_PyUnicode_Join(__pyx_t_1, 5, __pyx_t_8, __pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 195, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_2 = __Pyx_PyUnicode_Join(__pyx_t_1, 5, __pyx_t_7, __pyx_t_8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 232, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 195, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 232, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 195, __pyx_L1_error)
+    __PYX_ERR(0, 232, __pyx_L1_error)
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":194
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":231
  *                 break
  *             iterations_count += 1
  *         if zero_finding_error > cZeroFindingAccuracy:             # <<<<<<<<<<<<<<
  *             raise Exception(f'Zero vertical error {zero_finding_error} feet, after {iterations_count} iterations.')
  *         return Angular.Radian(self.barrel_elevation)
  */
   }
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":196
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":233
  *         if zero_finding_error > cZeroFindingAccuracy:
  *             raise Exception(f'Zero vertical error {zero_finding_error} feet, after {iterations_count} iterations.')
  *         return Angular.Radian(self.barrel_elevation)             # <<<<<<<<<<<<<<
  * 
  *     cdef _trajectory(TrajectoryCalc self, object shot_info,
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Angular); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 196, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Radian); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 196, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_self->barrel_elevation); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Angular); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_Radian); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 233, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = NULL;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = PyFloat_FromDouble(__pyx_v_self->barrel_elevation); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_9 = NULL;
   __pyx_t_10 = 0;
   #if CYTHON_UNPACK_METHODS
-  if (unlikely(PyMethod_Check(__pyx_t_7))) {
-    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_7);
-    if (likely(__pyx_t_2)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
-      __Pyx_INCREF(__pyx_t_2);
+  if (unlikely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_9)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_9);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_7, function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_10 = 1;
     }
   }
   #endif
   {
-    PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_t_3};
-    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 196, __pyx_L1_error)
+    PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_t_2};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
+    __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 233, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":170
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":204
  *         self.stability_coefficient = self.calc_stability_coefficient(shot_info.atmo)
  * 
  *     cdef _zero_angle(TrajectoryCalc self, object shot_info, object distance):             # <<<<<<<<<<<<<<
  *         cdef:
  *             double zero_distance = cos(shot_info.look_angle >> Angular.Radian) * (distance >> Distance.Foot)
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_9);
   __Pyx_AddTraceback("py_ballisticcalc_exts.trajectory_calc.TrajectoryCalc._zero_angle", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_t);
-  __Pyx_XDECREF(__pyx_v_height);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":198
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":235
  *         return Angular.Radian(self.barrel_elevation)
  * 
  *     cdef _trajectory(TrajectoryCalc self, object shot_info,             # <<<<<<<<<<<<<<
- *                      double maximum_range, double step, CTrajFlag filter_flags):
+ *                      double maximum_range, double step, int filter_flags):
  *         cdef:
  */
 
-static PyObject *__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc__trajectory(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, PyObject *__pyx_v_shot_info, double __pyx_v_maximum_range, double __pyx_v_step, enum __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag __pyx_v_filter_flags) {
-  PyObject *__pyx_v__flag = 0;
-  PyObject *__pyx_v_seen_zero = 0;
+static PyObject *__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc__trajectory(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, PyObject *__pyx_v_shot_info, double __pyx_v_maximum_range, double __pyx_v_step, int __pyx_v_filter_flags) {
+  int __pyx_v__flag;
+  int __pyx_v_seen_zero;
   double __pyx_v_density_factor;
   double __pyx_v_mach;
   double __pyx_v_velocity;
   double __pyx_v_delta_time;
   PyObject *__pyx_v_ranges = 0;
   int __pyx_v_ranges_length;
   int __pyx_v_current_item;
   double __pyx_v_time;
   double __pyx_v_previous_mach;
   double __pyx_v_drag;
   int __pyx_v_len_winds;
   int __pyx_v_current_wind;
   double __pyx_v_next_range_distance;
   double __pyx_v_next_wind_range;
+  double __pyx_v__max_wind_distance_feed;
+  double __pyx_v_reference_height;
   struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_velocity_vector = 0;
   struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_velocity_adjusted = 0;
   struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_range_vector = 0;
   struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_delta_range_vector = 0;
   struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_wind_vector = 0;
-  double __pyx_v_reference_height;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   double __pyx_t_5;
@@ -7537,365 +7790,368 @@
   double __pyx_t_11;
   int __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_trajectory", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":203
- *             object _flag, seen_zero  # CTrajFlag
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":240
+ *             int _flag, seen_zero  # CTrajFlag
  *             double density_factor, mach, velocity, delta_time
  *             list ranges = []             # <<<<<<<<<<<<<<
  *             int ranges_length = int(maximum_range / step) + 1
  *             int current_item = 0
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 240, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_ranges = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":204
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":241
  *             double density_factor, mach, velocity, delta_time
  *             list ranges = []
  *             int ranges_length = int(maximum_range / step) + 1             # <<<<<<<<<<<<<<
  *             int current_item = 0
  *             double time = .0
  */
-  if (unlikely(__pyx_v_step == 0)) {
-    PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(0, 204, __pyx_L1_error)
-  }
-  __pyx_t_1 = __Pyx_PyInt_FromDouble((__pyx_v_maximum_range / __pyx_v_step)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 204, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_FromDouble((__pyx_v_maximum_range / __pyx_v_step)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_AddObjC(__pyx_t_1, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 204, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_AddObjC(__pyx_t_1, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 204, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 241, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_ranges_length = __pyx_t_3;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":205
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":242
  *             list ranges = []
  *             int ranges_length = int(maximum_range / step) + 1
  *             int current_item = 0             # <<<<<<<<<<<<<<
  *             double time = .0
  *             double previous_mach = .0
  */
   __pyx_v_current_item = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":206
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":243
  *             int ranges_length = int(maximum_range / step) + 1
  *             int current_item = 0
  *             double time = .0             # <<<<<<<<<<<<<<
  *             double previous_mach = .0
  *             double drag = .0
  */
   __pyx_v_time = .0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":207
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":244
  *             int current_item = 0
  *             double time = .0
  *             double previous_mach = .0             # <<<<<<<<<<<<<<
  *             double drag = .0
  * 
  */
   __pyx_v_previous_mach = .0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":208
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":245
  *             double time = .0
  *             double previous_mach = .0
  *             double drag = .0             # <<<<<<<<<<<<<<
  * 
  *             int len_winds = len(shot_info.winds)
  */
   __pyx_v_drag = .0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":210
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":247
  *             double drag = .0
  * 
  *             int len_winds = len(shot_info.winds)             # <<<<<<<<<<<<<<
  *             int current_wind = 0
  *             double next_range_distance = .0
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_winds); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 210, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_winds); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyObject_Length(__pyx_t_2); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 210, __pyx_L1_error)
+  __pyx_t_4 = PyObject_Length(__pyx_t_2); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_len_winds = __pyx_t_4;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":211
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":248
  * 
  *             int len_winds = len(shot_info.winds)
  *             int current_wind = 0             # <<<<<<<<<<<<<<
  *             double next_range_distance = .0
  *             double next_wind_range = Wind.MAX_DISTANCE_FEET
  */
   __pyx_v_current_wind = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":212
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":249
  *             int len_winds = len(shot_info.winds)
  *             int current_wind = 0
  *             double next_range_distance = .0             # <<<<<<<<<<<<<<
  *             double next_wind_range = Wind.MAX_DISTANCE_FEET
- * 
+ *             double _max_wind_distance_feed = Wind.MAX_DISTANCE_FEET
  */
   __pyx_v_next_range_distance = .0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":213
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":250
  *             int current_wind = 0
  *             double next_range_distance = .0
  *             double next_wind_range = Wind.MAX_DISTANCE_FEET             # <<<<<<<<<<<<<<
+ *             double _max_wind_distance_feed = Wind.MAX_DISTANCE_FEET
  * 
- *             Vector velocity_vector, velocity_adjusted
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Wind); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 213, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Wind); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_MAX_DISTANCE_FEET); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 213, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_MAX_DISTANCE_FEET); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 213, __pyx_L1_error)
+  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 250, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_next_wind_range = __pyx_t_5;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":218
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":251
+ *             double next_range_distance = .0
+ *             double next_wind_range = Wind.MAX_DISTANCE_FEET
+ *             double _max_wind_distance_feed = Wind.MAX_DISTANCE_FEET             # <<<<<<<<<<<<<<
+ * 
+ *             double reference_height
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Wind); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 251, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_MAX_DISTANCE_FEET); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 251, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 251, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_v__max_wind_distance_feed = __pyx_t_5;
+
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":258
  *             Vector range_vector, delta_range_vector, wind_vector
  * 
  *         if len_winds < 1:             # <<<<<<<<<<<<<<
  *             wind_vector = Vector(.0, .0, .0)
  *         else:
  */
   __pyx_t_6 = (__pyx_v_len_winds < 1);
   if (__pyx_t_6) {
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":219
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":259
  * 
  *         if len_winds < 1:
  *             wind_vector = Vector(.0, .0, .0)             # <<<<<<<<<<<<<<
  *         else:
  *             wind_vector = wind_to_vector(shot_info.winds[0])
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_v_wind_vector = ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_1);
-    __pyx_t_1 = 0;
+    __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 259, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_v_wind_vector = ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_2);
+    __pyx_t_2 = 0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":218
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":258
  *             Vector range_vector, delta_range_vector, wind_vector
  * 
  *         if len_winds < 1:             # <<<<<<<<<<<<<<
  *             wind_vector = Vector(.0, .0, .0)
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":221
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":261
  *             wind_vector = Vector(.0, .0, .0)
  *         else:
  *             wind_vector = wind_to_vector(shot_info.winds[0])             # <<<<<<<<<<<<<<
  *             next_wind_range = shot_info.winds[0].until_distance >> Distance.Foot
  * 
  */
   /*else*/ {
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_winds); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 221, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 221, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_winds); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 261, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = ((PyObject *)__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_wind_to_vector(__pyx_t_2)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 221, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_GetItemInt(__pyx_t_2, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 261, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_v_wind_vector = ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_1);
-    __pyx_t_1 = 0;
+    __pyx_t_2 = ((PyObject *)__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_wind_to_vector(__pyx_t_1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 261, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_v_wind_vector = ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_2);
+    __pyx_t_2 = 0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":222
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":262
  *         else:
  *             wind_vector = wind_to_vector(shot_info.winds[0])
  *             next_wind_range = shot_info.winds[0].until_distance >> Distance.Foot             # <<<<<<<<<<<<<<
  * 
  *         velocity = self.muzzle_velocity
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_winds); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 222, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 222, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_winds); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 262, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_until_distance); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 222, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_GetItemInt(__pyx_t_2, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 262, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Distance); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 222, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_until_distance); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 262, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_Foot); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 222, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Distance); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 262, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Foot); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 262, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = PyNumber_Rshift(__pyx_t_1, __pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 222, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 222, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Rshift(__pyx_t_2, __pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 262, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 262, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_next_wind_range = __pyx_t_5;
   }
   __pyx_L3:;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":224
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":264
  *             next_wind_range = shot_info.winds[0].until_distance >> Distance.Foot
  * 
  *         velocity = self.muzzle_velocity             # <<<<<<<<<<<<<<
  *         # x: downrange distance, y: drop, z: windage
  *         range_vector = Vector(.0, -self.cant_cosine*self.sight_height, -self.cant_sine*self.sight_height)
  */
   __pyx_t_5 = __pyx_v_self->muzzle_velocity;
   __pyx_v_velocity = __pyx_t_5;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":226
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":266
  *         velocity = self.muzzle_velocity
  *         # x: downrange distance, y: drop, z: windage
  *         range_vector = Vector(.0, -self.cant_cosine*self.sight_height, -self.cant_sine*self.sight_height)             # <<<<<<<<<<<<<<
  *         velocity_vector = Vector(cos(self.barrel_elevation) * cos(self.barrel_azimuth),
  *                                  sin(self.barrel_elevation),
  */
-  __pyx_t_2 = PyFloat_FromDouble(((-__pyx_v_self->cant_cosine) * __pyx_v_self->sight_height)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 226, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_7 = PyFloat_FromDouble(((-__pyx_v_self->cant_sine) * __pyx_v_self->sight_height)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 226, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 226, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(((-__pyx_v_self->cant_cosine) * __pyx_v_self->sight_height)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 266, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_7 = PyFloat_FromDouble(((-__pyx_v_self->cant_sine) * __pyx_v_self->sight_height)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 266, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 266, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_float__0);
   __Pyx_GIVEREF(__pyx_float__0);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_float__0)) __PYX_ERR(0, 226, __pyx_L1_error);
-  __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2)) __PYX_ERR(0, 226, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_float__0)) __PYX_ERR(0, 266, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_1);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_1)) __PYX_ERR(0, 266, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_7);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_7)) __PYX_ERR(0, 226, __pyx_L1_error);
-  __pyx_t_2 = 0;
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_t_7)) __PYX_ERR(0, 266, __pyx_L1_error);
+  __pyx_t_1 = 0;
   __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_t_1, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 226, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_t_2, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 266, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_range_vector = ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_7);
   __pyx_t_7 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":227
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":267
  *         # x: downrange distance, y: drop, z: windage
  *         range_vector = Vector(.0, -self.cant_cosine*self.sight_height, -self.cant_sine*self.sight_height)
  *         velocity_vector = Vector(cos(self.barrel_elevation) * cos(self.barrel_azimuth),             # <<<<<<<<<<<<<<
  *                                  sin(self.barrel_elevation),
  *                                  cos(self.barrel_elevation) * sin(self.barrel_azimuth)) * velocity
  */
-  __pyx_t_7 = PyFloat_FromDouble((cos(__pyx_v_self->barrel_elevation) * cos(__pyx_v_self->barrel_azimuth))); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 227, __pyx_L1_error)
+  __pyx_t_7 = PyFloat_FromDouble((cos(__pyx_v_self->barrel_elevation) * cos(__pyx_v_self->barrel_azimuth))); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 267, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":228
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":268
  *         range_vector = Vector(.0, -self.cant_cosine*self.sight_height, -self.cant_sine*self.sight_height)
  *         velocity_vector = Vector(cos(self.barrel_elevation) * cos(self.barrel_azimuth),
  *                                  sin(self.barrel_elevation),             # <<<<<<<<<<<<<<
  *                                  cos(self.barrel_elevation) * sin(self.barrel_azimuth)) * velocity
  * 
  */
-  __pyx_t_1 = PyFloat_FromDouble(sin(__pyx_v_self->barrel_elevation)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 228, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = PyFloat_FromDouble(sin(__pyx_v_self->barrel_elevation)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 268, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":229
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":269
  *         velocity_vector = Vector(cos(self.barrel_elevation) * cos(self.barrel_azimuth),
  *                                  sin(self.barrel_elevation),
  *                                  cos(self.barrel_elevation) * sin(self.barrel_azimuth)) * velocity             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = PyFloat_FromDouble((cos(__pyx_v_self->barrel_elevation) * sin(__pyx_v_self->barrel_azimuth))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 229, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = PyFloat_FromDouble((cos(__pyx_v_self->barrel_elevation) * sin(__pyx_v_self->barrel_azimuth))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 269, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":227
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":267
  *         # x: downrange distance, y: drop, z: windage
  *         range_vector = Vector(.0, -self.cant_cosine*self.sight_height, -self.cant_sine*self.sight_height)
  *         velocity_vector = Vector(cos(self.barrel_elevation) * cos(self.barrel_azimuth),             # <<<<<<<<<<<<<<
  *                                  sin(self.barrel_elevation),
  *                                  cos(self.barrel_elevation) * sin(self.barrel_azimuth)) * velocity
  */
-  __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 227, __pyx_L1_error)
+  __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 267, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_GIVEREF(__pyx_t_7);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_7)) __PYX_ERR(0, 227, __pyx_L1_error);
-  __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_1)) __PYX_ERR(0, 227, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_7)) __PYX_ERR(0, 267, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_t_2)) __PYX_ERR(0, 227, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_2)) __PYX_ERR(0, 267, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_1);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_t_1)) __PYX_ERR(0, 267, __pyx_L1_error);
   __pyx_t_7 = 0;
-  __pyx_t_1 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 227, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_t_8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 267, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":229
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":269
  *         velocity_vector = Vector(cos(self.barrel_elevation) * cos(self.barrel_azimuth),
  *                                  sin(self.barrel_elevation),
  *                                  cos(self.barrel_elevation) * sin(self.barrel_azimuth)) * velocity             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_8 = PyFloat_FromDouble(__pyx_v_velocity); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 229, __pyx_L1_error)
+  __pyx_t_8 = PyFloat_FromDouble(__pyx_v_velocity); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 269, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_1 = PyNumber_Multiply(__pyx_t_2, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = PyNumber_Multiply(__pyx_t_1, __pyx_t_8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 269, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector))))) __PYX_ERR(0, 229, __pyx_L1_error)
-  __pyx_v_velocity_vector = ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_1);
-  __pyx_t_1 = 0;
+  if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector))))) __PYX_ERR(0, 269, __pyx_L1_error)
+  __pyx_v_velocity_vector = ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_2);
+  __pyx_t_2 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":233
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":273
  * 
  *         # With non-zero look_angle, rounding can suggest multiple adjacent zero-crossings
  *         seen_zero = CTrajFlag.NONE  # Record when we see each zero crossing so we only register one             # <<<<<<<<<<<<<<
  *         if range_vector.y >= 0:
  *             seen_zero |= CTrajFlag.ZERO_UP  # We're starting above zero; we can only go down
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_NONE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 233, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_v_seen_zero = __pyx_t_1;
-  __pyx_t_1 = 0;
+  __pyx_v_seen_zero = __pyx_e_21py_ballisticcalc_exts_15trajectory_calc_NONE;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":234
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":274
  *         # With non-zero look_angle, rounding can suggest multiple adjacent zero-crossings
  *         seen_zero = CTrajFlag.NONE  # Record when we see each zero crossing so we only register one
  *         if range_vector.y >= 0:             # <<<<<<<<<<<<<<
  *             seen_zero |= CTrajFlag.ZERO_UP  # We're starting above zero; we can only go down
  *         elif range_vector.y < 0 and self.barrel_elevation < self.look_angle:
  */
   __pyx_t_6 = (__pyx_v_range_vector->y >= 0.0);
   if (__pyx_t_6) {
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":235
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":275
  *         seen_zero = CTrajFlag.NONE  # Record when we see each zero crossing so we only register one
  *         if range_vector.y >= 0:
  *             seen_zero |= CTrajFlag.ZERO_UP  # We're starting above zero; we can only go down             # <<<<<<<<<<<<<<
  *         elif range_vector.y < 0 and self.barrel_elevation < self.look_angle:
  *             seen_zero |= CTrajFlag.ZERO_DOWN  # We're below and pointing down from look angle; no zeroes!
  */
-    __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_UP); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 235, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_8 = PyNumber_InPlaceOr(__pyx_v_seen_zero, __pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 235, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF_SET(__pyx_v_seen_zero, __pyx_t_8);
-    __pyx_t_8 = 0;
+    __pyx_v_seen_zero = (__pyx_v_seen_zero | __pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_UP);
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":234
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":274
  *         # With non-zero look_angle, rounding can suggest multiple adjacent zero-crossings
  *         seen_zero = CTrajFlag.NONE  # Record when we see each zero crossing so we only register one
  *         if range_vector.y >= 0:             # <<<<<<<<<<<<<<
  *             seen_zero |= CTrajFlag.ZERO_UP  # We're starting above zero; we can only go down
  *         elif range_vector.y < 0 and self.barrel_elevation < self.look_angle:
  */
     goto __pyx_L4;
   }
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":236
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":276
  *         if range_vector.y >= 0:
  *             seen_zero |= CTrajFlag.ZERO_UP  # We're starting above zero; we can only go down
  *         elif range_vector.y < 0 and self.barrel_elevation < self.look_angle:             # <<<<<<<<<<<<<<
  *             seen_zero |= CTrajFlag.ZERO_DOWN  # We're below and pointing down from look angle; no zeroes!
  * 
  */
   __pyx_t_9 = (__pyx_v_range_vector->y < 0.0);
@@ -7905,975 +8161,890 @@
     goto __pyx_L5_bool_binop_done;
   }
   __pyx_t_9 = (__pyx_v_self->barrel_elevation < __pyx_v_self->look_angle);
   __pyx_t_6 = __pyx_t_9;
   __pyx_L5_bool_binop_done:;
   if (__pyx_t_6) {
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":237
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":277
  *             seen_zero |= CTrajFlag.ZERO_UP  # We're starting above zero; we can only go down
  *         elif range_vector.y < 0 and self.barrel_elevation < self.look_angle:
  *             seen_zero |= CTrajFlag.ZERO_DOWN  # We're below and pointing down from look angle; no zeroes!             # <<<<<<<<<<<<<<
  * 
  *         #region Trajectory Loop
  */
-    __pyx_t_8 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_DOWN); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 237, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_1 = PyNumber_InPlaceOr(__pyx_v_seen_zero, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 237, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __Pyx_DECREF_SET(__pyx_v_seen_zero, __pyx_t_1);
-    __pyx_t_1 = 0;
+    __pyx_v_seen_zero = (__pyx_v_seen_zero | __pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_DOWN);
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":236
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":276
  *         if range_vector.y >= 0:
  *             seen_zero |= CTrajFlag.ZERO_UP  # We're starting above zero; we can only go down
  *         elif range_vector.y < 0 and self.barrel_elevation < self.look_angle:             # <<<<<<<<<<<<<<
  *             seen_zero |= CTrajFlag.ZERO_DOWN  # We're below and pointing down from look angle; no zeroes!
  * 
  */
   }
   __pyx_L4:;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":240
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":280
  * 
  *         #region Trajectory Loop
  *         while range_vector.x <= maximum_range + self.calc_step:             # <<<<<<<<<<<<<<
  *             _flag = CTrajFlag.NONE
  * 
  */
   while (1) {
     __pyx_t_6 = (__pyx_v_range_vector->x <= (__pyx_v_maximum_range + __pyx_v_self->calc_step));
     if (!__pyx_t_6) break;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":241
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":281
  *         #region Trajectory Loop
  *         while range_vector.x <= maximum_range + self.calc_step:
  *             _flag = CTrajFlag.NONE             # <<<<<<<<<<<<<<
  * 
  *             if range_vector.x >= next_wind_range:
  */
-    __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_NONE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 241, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_XDECREF_SET(__pyx_v__flag, __pyx_t_1);
-    __pyx_t_1 = 0;
+    __pyx_v__flag = __pyx_e_21py_ballisticcalc_exts_15trajectory_calc_NONE;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":243
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":283
  *             _flag = CTrajFlag.NONE
  * 
  *             if range_vector.x >= next_wind_range:             # <<<<<<<<<<<<<<
  *                 current_wind += 1
  *                 if current_wind >= len_winds:  # No more winds listed after this range
  */
     __pyx_t_6 = (__pyx_v_range_vector->x >= __pyx_v_next_wind_range);
     if (__pyx_t_6) {
 
-      /* "py_ballisticcalc_exts/trajectory_calc.pyx":244
+      /* "py_ballisticcalc_exts/trajectory_calc.pyx":284
  * 
  *             if range_vector.x >= next_wind_range:
  *                 current_wind += 1             # <<<<<<<<<<<<<<
  *                 if current_wind >= len_winds:  # No more winds listed after this range
  *                     wind_vector = Vector(.0, .0, .0)
  */
       __pyx_v_current_wind = (__pyx_v_current_wind + 1);
 
-      /* "py_ballisticcalc_exts/trajectory_calc.pyx":245
+      /* "py_ballisticcalc_exts/trajectory_calc.pyx":285
  *             if range_vector.x >= next_wind_range:
  *                 current_wind += 1
  *                 if current_wind >= len_winds:  # No more winds listed after this range             # <<<<<<<<<<<<<<
  *                     wind_vector = Vector(.0, .0, .0)
- *                     next_wind_range = Wind.MAX_DISTANCE_FEET
+ *                     next_wind_range = _max_wind_distance_feed  # better for cython optimization
  */
       __pyx_t_6 = (__pyx_v_current_wind >= __pyx_v_len_winds);
       if (__pyx_t_6) {
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":246
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":286
  *                 current_wind += 1
  *                 if current_wind >= len_winds:  # No more winds listed after this range
  *                     wind_vector = Vector(.0, .0, .0)             # <<<<<<<<<<<<<<
- *                     next_wind_range = Wind.MAX_DISTANCE_FEET
+ *                     next_wind_range = _max_wind_distance_feed  # better for cython optimization
  *                 else:
  */
-        __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_1);
-        __Pyx_DECREF_SET(__pyx_v_wind_vector, ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_1));
-        __pyx_t_1 = 0;
+        __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 286, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_DECREF_SET(__pyx_v_wind_vector, ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_2));
+        __pyx_t_2 = 0;
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":247
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":287
  *                 if current_wind >= len_winds:  # No more winds listed after this range
  *                     wind_vector = Vector(.0, .0, .0)
- *                     next_wind_range = Wind.MAX_DISTANCE_FEET             # <<<<<<<<<<<<<<
+ *                     next_wind_range = _max_wind_distance_feed  # better for cython optimization             # <<<<<<<<<<<<<<
  *                 else:
  *                     wind_vector = wind_to_vector(shot_info.winds[current_wind])
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Wind); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 247, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_MAX_DISTANCE_FEET); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 247, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_8);
-        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_8); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 247, __pyx_L1_error)
-        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-        __pyx_v_next_wind_range = __pyx_t_5;
+        __pyx_v_next_wind_range = __pyx_v__max_wind_distance_feed;
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":245
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":285
  *             if range_vector.x >= next_wind_range:
  *                 current_wind += 1
  *                 if current_wind >= len_winds:  # No more winds listed after this range             # <<<<<<<<<<<<<<
  *                     wind_vector = Vector(.0, .0, .0)
- *                     next_wind_range = Wind.MAX_DISTANCE_FEET
+ *                     next_wind_range = _max_wind_distance_feed  # better for cython optimization
  */
         goto __pyx_L10;
       }
 
-      /* "py_ballisticcalc_exts/trajectory_calc.pyx":249
- *                     next_wind_range = Wind.MAX_DISTANCE_FEET
+      /* "py_ballisticcalc_exts/trajectory_calc.pyx":289
+ *                     next_wind_range = _max_wind_distance_feed  # better for cython optimization
  *                 else:
  *                     wind_vector = wind_to_vector(shot_info.winds[current_wind])             # <<<<<<<<<<<<<<
  *                     next_wind_range = shot_info.winds[current_wind].until_distance >> Distance.Foot
  * 
  */
       /*else*/ {
-        __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_winds); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 249, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_winds); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 289, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __pyx_t_8 = __Pyx_GetItemInt(__pyx_t_2, __pyx_v_current_wind, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 289, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
-        __pyx_t_1 = __Pyx_GetItemInt(__pyx_t_8, __pyx_v_current_wind, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 249, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_1);
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __pyx_t_2 = ((PyObject *)__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_wind_to_vector(__pyx_t_8)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 289, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-        __pyx_t_8 = ((PyObject *)__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_wind_to_vector(__pyx_t_1)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 249, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_8);
-        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __Pyx_DECREF_SET(__pyx_v_wind_vector, ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_8));
-        __pyx_t_8 = 0;
+        __Pyx_DECREF_SET(__pyx_v_wind_vector, ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_2));
+        __pyx_t_2 = 0;
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":250
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":290
  *                 else:
  *                     wind_vector = wind_to_vector(shot_info.winds[current_wind])
  *                     next_wind_range = shot_info.winds[current_wind].until_distance >> Distance.Foot             # <<<<<<<<<<<<<<
  * 
  *             density_factor, mach = shot_info.atmo.get_density_factor_and_mach_for_altitude(
  */
-        __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_winds); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 250, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_winds); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 290, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __pyx_t_8 = __Pyx_GetItemInt(__pyx_t_2, __pyx_v_current_wind, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 290, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
-        __pyx_t_1 = __Pyx_GetItemInt(__pyx_t_8, __pyx_v_current_wind, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 250, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_1);
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_until_distance); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 290, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-        __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_until_distance); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 250, __pyx_L1_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Distance); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 290, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
-        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Distance); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 250, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Foot); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 250, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
-        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_1 = PyNumber_Rshift(__pyx_t_8, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 250, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_Foot); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 290, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+        __pyx_t_8 = PyNumber_Rshift(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 290, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 250, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_8); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 290, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         __pyx_v_next_wind_range = __pyx_t_5;
       }
       __pyx_L10:;
 
-      /* "py_ballisticcalc_exts/trajectory_calc.pyx":243
+      /* "py_ballisticcalc_exts/trajectory_calc.pyx":283
  *             _flag = CTrajFlag.NONE
  * 
  *             if range_vector.x >= next_wind_range:             # <<<<<<<<<<<<<<
  *                 current_wind += 1
  *                 if current_wind >= len_winds:  # No more winds listed after this range
  */
     }
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":252
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":292
  *                     next_wind_range = shot_info.winds[current_wind].until_distance >> Distance.Foot
  * 
  *             density_factor, mach = shot_info.atmo.get_density_factor_and_mach_for_altitude(             # <<<<<<<<<<<<<<
  *                 self.alt0 + range_vector.y)
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_atmo); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 252, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_atmo); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 292, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_get_density_factor_and_mach_for); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 292, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get_density_factor_and_mach_for); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 252, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":253
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":293
  * 
  *             density_factor, mach = shot_info.atmo.get_density_factor_and_mach_for_altitude(
  *                 self.alt0 + range_vector.y)             # <<<<<<<<<<<<<<
  * 
  *             if filter_flags:
  */
-    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_self->alt0 + __pyx_v_range_vector->y)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 253, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyFloat_FromDouble((__pyx_v_self->alt0 + __pyx_v_range_vector->y)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 293, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_7 = NULL;
     __pyx_t_3 = 0;
     #if CYTHON_UNPACK_METHODS
-    if (likely(PyMethod_Check(__pyx_t_8))) {
-      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_8);
+    if (likely(PyMethod_Check(__pyx_t_2))) {
+      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_7)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_8, function);
+        __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_3 = 1;
       }
     }
     #endif
     {
-      PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_2};
-      __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_3, 1+__pyx_t_3);
+      PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_1};
+      __pyx_t_8 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_3, 1+__pyx_t_3);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 292, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 252, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
-    if ((likely(PyTuple_CheckExact(__pyx_t_1))) || (PyList_CheckExact(__pyx_t_1))) {
-      PyObject* sequence = __pyx_t_1;
+    if ((likely(PyTuple_CheckExact(__pyx_t_8))) || (PyList_CheckExact(__pyx_t_8))) {
+      PyObject* sequence = __pyx_t_8;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 2)) {
         if (size > 2) __Pyx_RaiseTooManyValuesError(2);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 252, __pyx_L1_error)
+        __PYX_ERR(0, 292, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       if (likely(PyTuple_CheckExact(sequence))) {
-        __pyx_t_8 = PyTuple_GET_ITEM(sequence, 0); 
-        __pyx_t_2 = PyTuple_GET_ITEM(sequence, 1); 
+        __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
+        __pyx_t_1 = PyTuple_GET_ITEM(sequence, 1); 
       } else {
-        __pyx_t_8 = PyList_GET_ITEM(sequence, 0); 
-        __pyx_t_2 = PyList_GET_ITEM(sequence, 1); 
+        __pyx_t_2 = PyList_GET_ITEM(sequence, 0); 
+        __pyx_t_1 = PyList_GET_ITEM(sequence, 1); 
       }
-      __Pyx_INCREF(__pyx_t_8);
       __Pyx_INCREF(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_1);
       #else
-      __pyx_t_8 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 252, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_2 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 252, __pyx_L1_error)
+      __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 292, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
+      __pyx_t_1 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 292, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
       #endif
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     } else {
       Py_ssize_t index = -1;
-      __pyx_t_7 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 252, __pyx_L1_error)
+      __pyx_t_7 = PyObject_GetIter(__pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 292, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __pyx_t_10 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_7);
-      index = 0; __pyx_t_8 = __pyx_t_10(__pyx_t_7); if (unlikely(!__pyx_t_8)) goto __pyx_L11_unpacking_failed;
-      __Pyx_GOTREF(__pyx_t_8);
-      index = 1; __pyx_t_2 = __pyx_t_10(__pyx_t_7); if (unlikely(!__pyx_t_2)) goto __pyx_L11_unpacking_failed;
+      index = 0; __pyx_t_2 = __pyx_t_10(__pyx_t_7); if (unlikely(!__pyx_t_2)) goto __pyx_L11_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_2);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_10(__pyx_t_7), 2) < 0) __PYX_ERR(0, 252, __pyx_L1_error)
+      index = 1; __pyx_t_1 = __pyx_t_10(__pyx_t_7); if (unlikely(!__pyx_t_1)) goto __pyx_L11_unpacking_failed;
+      __Pyx_GOTREF(__pyx_t_1);
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_10(__pyx_t_7), 2) < 0) __PYX_ERR(0, 292, __pyx_L1_error)
       __pyx_t_10 = NULL;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       goto __pyx_L12_unpacking_done;
       __pyx_L11_unpacking_failed:;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __pyx_t_10 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(0, 252, __pyx_L1_error)
+      __PYX_ERR(0, 292, __pyx_L1_error)
       __pyx_L12_unpacking_done:;
     }
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":252
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":292
  *                     next_wind_range = shot_info.winds[current_wind].until_distance >> Distance.Foot
  * 
  *             density_factor, mach = shot_info.atmo.get_density_factor_and_mach_for_altitude(             # <<<<<<<<<<<<<<
  *                 self.alt0 + range_vector.y)
  * 
  */
-    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_8); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 252, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_11 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_11 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 252, __pyx_L1_error)
+    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 292, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_11 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_11 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 292, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_density_factor = __pyx_t_5;
     __pyx_v_mach = __pyx_t_11;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":255
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":295
  *                 self.alt0 + range_vector.y)
  * 
  *             if filter_flags:             # <<<<<<<<<<<<<<
  *                 # Zero-crossing checks
  *                 if range_vector.x > 0:
  */
-    if (__pyx_v_filter_flags) {
+    __pyx_t_6 = (__pyx_v_filter_flags != 0);
+    if (__pyx_t_6) {
 
-      /* "py_ballisticcalc_exts/trajectory_calc.pyx":257
+      /* "py_ballisticcalc_exts/trajectory_calc.pyx":297
  *             if filter_flags:
  *                 # Zero-crossing checks
  *                 if range_vector.x > 0:             # <<<<<<<<<<<<<<
  *                     # Zero reference line is the sight line defined by look_angle
  *                     reference_height = range_vector.x * tan(self.look_angle)
  */
       __pyx_t_6 = (__pyx_v_range_vector->x > 0.0);
       if (__pyx_t_6) {
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":259
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":299
  *                 if range_vector.x > 0:
  *                     # Zero reference line is the sight line defined by look_angle
  *                     reference_height = range_vector.x * tan(self.look_angle)             # <<<<<<<<<<<<<<
  *                     # If we haven't seen ZERO_UP, we look for that first
  *                     if not seen_zero & CTrajFlag.ZERO_UP:
  */
         __pyx_v_reference_height = (__pyx_v_range_vector->x * tan(__pyx_v_self->look_angle));
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":261
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":301
  *                     reference_height = range_vector.x * tan(self.look_angle)
  *                     # If we haven't seen ZERO_UP, we look for that first
  *                     if not seen_zero & CTrajFlag.ZERO_UP:             # <<<<<<<<<<<<<<
  *                         if range_vector.y >= reference_height:
  *                             _flag |= CTrajFlag.ZERO_UP
  */
-        __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_UP); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 261, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_2 = PyNumber_And(__pyx_v_seen_zero, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 261, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
-        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 261, __pyx_L1_error)
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __pyx_t_9 = (!__pyx_t_6);
-        if (__pyx_t_9) {
+        __pyx_t_6 = (!((__pyx_v_seen_zero & __pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_UP) != 0));
+        if (__pyx_t_6) {
 
-          /* "py_ballisticcalc_exts/trajectory_calc.pyx":262
+          /* "py_ballisticcalc_exts/trajectory_calc.pyx":302
  *                     # If we haven't seen ZERO_UP, we look for that first
  *                     if not seen_zero & CTrajFlag.ZERO_UP:
  *                         if range_vector.y >= reference_height:             # <<<<<<<<<<<<<<
  *                             _flag |= CTrajFlag.ZERO_UP
  *                             seen_zero |= CTrajFlag.ZERO_UP
  */
-          __pyx_t_9 = (__pyx_v_range_vector->y >= __pyx_v_reference_height);
-          if (__pyx_t_9) {
+          __pyx_t_6 = (__pyx_v_range_vector->y >= __pyx_v_reference_height);
+          if (__pyx_t_6) {
 
-            /* "py_ballisticcalc_exts/trajectory_calc.pyx":263
+            /* "py_ballisticcalc_exts/trajectory_calc.pyx":303
  *                     if not seen_zero & CTrajFlag.ZERO_UP:
  *                         if range_vector.y >= reference_height:
  *                             _flag |= CTrajFlag.ZERO_UP             # <<<<<<<<<<<<<<
  *                             seen_zero |= CTrajFlag.ZERO_UP
  *                     # We've crossed above sight line; now look for crossing back through it
  */
-            __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_UP); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 263, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_2);
-            __pyx_t_1 = PyNumber_InPlaceOr(__pyx_v__flag, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 263, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_1);
-            __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-            __Pyx_DECREF_SET(__pyx_v__flag, __pyx_t_1);
-            __pyx_t_1 = 0;
+            __pyx_v__flag = (__pyx_v__flag | __pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_UP);
 
-            /* "py_ballisticcalc_exts/trajectory_calc.pyx":264
+            /* "py_ballisticcalc_exts/trajectory_calc.pyx":304
  *                         if range_vector.y >= reference_height:
  *                             _flag |= CTrajFlag.ZERO_UP
  *                             seen_zero |= CTrajFlag.ZERO_UP             # <<<<<<<<<<<<<<
  *                     # We've crossed above sight line; now look for crossing back through it
  *                     elif not seen_zero & CTrajFlag.ZERO_DOWN:
  */
-            __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_UP); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 264, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_1);
-            __pyx_t_2 = PyNumber_InPlaceOr(__pyx_v_seen_zero, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 264, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_2);
-            __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-            __Pyx_DECREF_SET(__pyx_v_seen_zero, __pyx_t_2);
-            __pyx_t_2 = 0;
+            __pyx_v_seen_zero = (__pyx_v_seen_zero | __pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_UP);
 
-            /* "py_ballisticcalc_exts/trajectory_calc.pyx":262
+            /* "py_ballisticcalc_exts/trajectory_calc.pyx":302
  *                     # If we haven't seen ZERO_UP, we look for that first
  *                     if not seen_zero & CTrajFlag.ZERO_UP:
  *                         if range_vector.y >= reference_height:             # <<<<<<<<<<<<<<
  *                             _flag |= CTrajFlag.ZERO_UP
  *                             seen_zero |= CTrajFlag.ZERO_UP
  */
           }
 
-          /* "py_ballisticcalc_exts/trajectory_calc.pyx":261
+          /* "py_ballisticcalc_exts/trajectory_calc.pyx":301
  *                     reference_height = range_vector.x * tan(self.look_angle)
  *                     # If we haven't seen ZERO_UP, we look for that first
  *                     if not seen_zero & CTrajFlag.ZERO_UP:             # <<<<<<<<<<<<<<
  *                         if range_vector.y >= reference_height:
  *                             _flag |= CTrajFlag.ZERO_UP
  */
           goto __pyx_L15;
         }
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":266
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":306
  *                             seen_zero |= CTrajFlag.ZERO_UP
  *                     # We've crossed above sight line; now look for crossing back through it
  *                     elif not seen_zero & CTrajFlag.ZERO_DOWN:             # <<<<<<<<<<<<<<
  *                         if range_vector.y < reference_height:
  *                             _flag |= CTrajFlag.ZERO_DOWN
  */
-        __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_DOWN); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 266, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_1 = PyNumber_And(__pyx_v_seen_zero, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 266, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_1);
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 266, __pyx_L1_error)
-        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_6 = (!__pyx_t_9);
+        __pyx_t_6 = (!((__pyx_v_seen_zero & __pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_DOWN) != 0));
         if (__pyx_t_6) {
 
-          /* "py_ballisticcalc_exts/trajectory_calc.pyx":267
+          /* "py_ballisticcalc_exts/trajectory_calc.pyx":307
  *                     # We've crossed above sight line; now look for crossing back through it
  *                     elif not seen_zero & CTrajFlag.ZERO_DOWN:
  *                         if range_vector.y < reference_height:             # <<<<<<<<<<<<<<
  *                             _flag |= CTrajFlag.ZERO_DOWN
  *                             seen_zero |= CTrajFlag.ZERO_DOWN
  */
           __pyx_t_6 = (__pyx_v_range_vector->y < __pyx_v_reference_height);
           if (__pyx_t_6) {
 
-            /* "py_ballisticcalc_exts/trajectory_calc.pyx":268
+            /* "py_ballisticcalc_exts/trajectory_calc.pyx":308
  *                     elif not seen_zero & CTrajFlag.ZERO_DOWN:
  *                         if range_vector.y < reference_height:
  *                             _flag |= CTrajFlag.ZERO_DOWN             # <<<<<<<<<<<<<<
  *                             seen_zero |= CTrajFlag.ZERO_DOWN
  * 
  */
-            __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_DOWN); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 268, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_1);
-            __pyx_t_2 = PyNumber_InPlaceOr(__pyx_v__flag, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 268, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_2);
-            __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-            __Pyx_DECREF_SET(__pyx_v__flag, __pyx_t_2);
-            __pyx_t_2 = 0;
+            __pyx_v__flag = (__pyx_v__flag | __pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_DOWN);
 
-            /* "py_ballisticcalc_exts/trajectory_calc.pyx":269
+            /* "py_ballisticcalc_exts/trajectory_calc.pyx":309
  *                         if range_vector.y < reference_height:
  *                             _flag |= CTrajFlag.ZERO_DOWN
  *                             seen_zero |= CTrajFlag.ZERO_DOWN             # <<<<<<<<<<<<<<
  * 
  *                 # Mach crossing check
  */
-            __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_DOWN); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 269, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_2);
-            __pyx_t_1 = PyNumber_InPlaceOr(__pyx_v_seen_zero, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 269, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_1);
-            __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-            __Pyx_DECREF_SET(__pyx_v_seen_zero, __pyx_t_1);
-            __pyx_t_1 = 0;
+            __pyx_v_seen_zero = (__pyx_v_seen_zero | __pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_DOWN);
 
-            /* "py_ballisticcalc_exts/trajectory_calc.pyx":267
+            /* "py_ballisticcalc_exts/trajectory_calc.pyx":307
  *                     # We've crossed above sight line; now look for crossing back through it
  *                     elif not seen_zero & CTrajFlag.ZERO_DOWN:
  *                         if range_vector.y < reference_height:             # <<<<<<<<<<<<<<
  *                             _flag |= CTrajFlag.ZERO_DOWN
  *                             seen_zero |= CTrajFlag.ZERO_DOWN
  */
           }
 
-          /* "py_ballisticcalc_exts/trajectory_calc.pyx":266
+          /* "py_ballisticcalc_exts/trajectory_calc.pyx":306
  *                             seen_zero |= CTrajFlag.ZERO_UP
  *                     # We've crossed above sight line; now look for crossing back through it
  *                     elif not seen_zero & CTrajFlag.ZERO_DOWN:             # <<<<<<<<<<<<<<
  *                         if range_vector.y < reference_height:
  *                             _flag |= CTrajFlag.ZERO_DOWN
  */
         }
         __pyx_L15:;
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":257
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":297
  *             if filter_flags:
  *                 # Zero-crossing checks
  *                 if range_vector.x > 0:             # <<<<<<<<<<<<<<
  *                     # Zero reference line is the sight line defined by look_angle
  *                     reference_height = range_vector.x * tan(self.look_angle)
  */
       }
 
-      /* "py_ballisticcalc_exts/trajectory_calc.pyx":272
- * 
+      /* "py_ballisticcalc_exts/trajectory_calc.pyx":313
  *                 # Mach crossing check
- *                 if (velocity / mach <= 1) and (previous_mach > 1):             # <<<<<<<<<<<<<<
+ *                 # if (velocity / mach <= 1) and (previous_mach > 1):
+ *                 if velocity / mach <= 1 < previous_mach:  # better cython optimization             # <<<<<<<<<<<<<<
  *                     _flag |= CTrajFlag.MACH
  * 
  */
-      if (unlikely(__pyx_v_mach == 0)) {
-        PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-        __PYX_ERR(0, 272, __pyx_L1_error)
-      }
-      __pyx_t_9 = ((__pyx_v_velocity / __pyx_v_mach) <= 1.0);
-      if (__pyx_t_9) {
-      } else {
-        __pyx_t_6 = __pyx_t_9;
-        goto __pyx_L19_bool_binop_done;
+      __pyx_t_6 = ((__pyx_v_velocity / __pyx_v_mach) <= 1.0);
+      if (__pyx_t_6) {
+        __pyx_t_6 = (1.0 < __pyx_v_previous_mach);
       }
-      __pyx_t_9 = (__pyx_v_previous_mach > 1.0);
-      __pyx_t_6 = __pyx_t_9;
-      __pyx_L19_bool_binop_done:;
       if (__pyx_t_6) {
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":273
- *                 # Mach crossing check
- *                 if (velocity / mach <= 1) and (previous_mach > 1):
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":314
+ *                 # if (velocity / mach <= 1) and (previous_mach > 1):
+ *                 if velocity / mach <= 1 < previous_mach:  # better cython optimization
  *                     _flag |= CTrajFlag.MACH             # <<<<<<<<<<<<<<
  * 
  *                 # Next range check
  */
-        __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_MACH); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 273, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_2 = PyNumber_InPlaceOr(__pyx_v__flag, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 273, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
-        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __Pyx_DECREF_SET(__pyx_v__flag, __pyx_t_2);
-        __pyx_t_2 = 0;
+        __pyx_v__flag = (__pyx_v__flag | __pyx_e_21py_ballisticcalc_exts_15trajectory_calc_MACH);
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":272
- * 
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":313
  *                 # Mach crossing check
- *                 if (velocity / mach <= 1) and (previous_mach > 1):             # <<<<<<<<<<<<<<
+ *                 # if (velocity / mach <= 1) and (previous_mach > 1):
+ *                 if velocity / mach <= 1 < previous_mach:  # better cython optimization             # <<<<<<<<<<<<<<
  *                     _flag |= CTrajFlag.MACH
  * 
  */
       }
 
-      /* "py_ballisticcalc_exts/trajectory_calc.pyx":276
+      /* "py_ballisticcalc_exts/trajectory_calc.pyx":317
  * 
  *                 # Next range check
  *                 if range_vector.x >= next_range_distance:             # <<<<<<<<<<<<<<
  *                     _flag |= CTrajFlag.RANGE
  *                     next_range_distance += step
  */
       __pyx_t_6 = (__pyx_v_range_vector->x >= __pyx_v_next_range_distance);
       if (__pyx_t_6) {
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":277
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":318
  *                 # Next range check
  *                 if range_vector.x >= next_range_distance:
  *                     _flag |= CTrajFlag.RANGE             # <<<<<<<<<<<<<<
  *                     next_range_distance += step
  *                     current_item += 1
  */
-        __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_RANGE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 277, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_1 = PyNumber_InPlaceOr(__pyx_v__flag, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 277, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_1);
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __Pyx_DECREF_SET(__pyx_v__flag, __pyx_t_1);
-        __pyx_t_1 = 0;
+        __pyx_v__flag = (__pyx_v__flag | __pyx_e_21py_ballisticcalc_exts_15trajectory_calc_RANGE);
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":278
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":319
  *                 if range_vector.x >= next_range_distance:
  *                     _flag |= CTrajFlag.RANGE
  *                     next_range_distance += step             # <<<<<<<<<<<<<<
  *                     current_item += 1
  * 
  */
         __pyx_v_next_range_distance = (__pyx_v_next_range_distance + __pyx_v_step);
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":279
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":320
  *                     _flag |= CTrajFlag.RANGE
  *                     next_range_distance += step
  *                     current_item += 1             # <<<<<<<<<<<<<<
  * 
  *                 # Record TrajectoryData row
  */
         __pyx_v_current_item = (__pyx_v_current_item + 1);
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":276
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":317
  * 
  *                 # Next range check
  *                 if range_vector.x >= next_range_distance:             # <<<<<<<<<<<<<<
  *                     _flag |= CTrajFlag.RANGE
  *                     next_range_distance += step
  */
       }
 
-      /* "py_ballisticcalc_exts/trajectory_calc.pyx":282
+      /* "py_ballisticcalc_exts/trajectory_calc.pyx":323
  * 
  *                 # Record TrajectoryData row
  *                 if _flag & filter_flags:             # <<<<<<<<<<<<<<
  *                     ranges.append(create_trajectory_row(
  *                         time, range_vector, velocity_vector,
  */
-      __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_v_filter_flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 282, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_2 = PyNumber_And(__pyx_v__flag, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 282, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 282, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __pyx_t_6 = ((__pyx_v__flag & __pyx_v_filter_flags) != 0);
       if (__pyx_t_6) {
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":285
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":326
  *                     ranges.append(create_trajectory_row(
  *                         time, range_vector, velocity_vector,
  *                         velocity, mach, self.spin_drift(time), self.look_angle,             # <<<<<<<<<<<<<<
  *                         density_factor, drag, self.weight, _flag
  *                     ))
  */
-        __pyx_t_11 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self->__pyx_vtab)->spin_drift(__pyx_v_self, __pyx_v_time); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 285, __pyx_L1_error)
+        __pyx_t_11 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self->__pyx_vtab)->spin_drift(__pyx_v_self, __pyx_v_time); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 326, __pyx_L1_error)
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":283
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":327
+ *                         time, range_vector, velocity_vector,
+ *                         velocity, mach, self.spin_drift(time), self.look_angle,
+ *                         density_factor, drag, self.weight, _flag             # <<<<<<<<<<<<<<
+ *                     ))
+ *                     if current_item == ranges_length:
+ */
+        __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v__flag); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 327, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_8);
+
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":324
  *                 # Record TrajectoryData row
  *                 if _flag & filter_flags:
  *                     ranges.append(create_trajectory_row(             # <<<<<<<<<<<<<<
  *                         time, range_vector, velocity_vector,
  *                         velocity, mach, self.spin_drift(time), self.look_angle,
  */
-        __pyx_t_2 = __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_create_trajectory_row(__pyx_v_time, __pyx_v_range_vector, __pyx_v_velocity_vector, __pyx_v_velocity, __pyx_v_mach, __pyx_t_11, __pyx_v_self->look_angle, __pyx_v_density_factor, __pyx_v_drag, __pyx_v_self->weight, __pyx_v__flag); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 283, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_12 = __Pyx_PyList_Append(__pyx_v_ranges, __pyx_t_2); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 283, __pyx_L1_error)
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __pyx_t_1 = __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_create_trajectory_row(__pyx_v_time, __pyx_v_range_vector, __pyx_v_velocity_vector, __pyx_v_velocity, __pyx_v_mach, __pyx_t_11, __pyx_v_self->look_angle, __pyx_v_density_factor, __pyx_v_drag, __pyx_v_self->weight, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 324, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+        __pyx_t_12 = __Pyx_PyList_Append(__pyx_v_ranges, __pyx_t_1); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 324, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":288
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":329
  *                         density_factor, drag, self.weight, _flag
  *                     ))
  *                     if current_item == ranges_length:             # <<<<<<<<<<<<<<
  *                         break
  * 
  */
         __pyx_t_6 = (__pyx_v_current_item == __pyx_v_ranges_length);
         if (__pyx_t_6) {
 
-          /* "py_ballisticcalc_exts/trajectory_calc.pyx":289
+          /* "py_ballisticcalc_exts/trajectory_calc.pyx":330
  *                     ))
  *                     if current_item == ranges_length:
  *                         break             # <<<<<<<<<<<<<<
  * 
  *             previous_mach = velocity / mach
  */
           goto __pyx_L8_break;
 
-          /* "py_ballisticcalc_exts/trajectory_calc.pyx":288
+          /* "py_ballisticcalc_exts/trajectory_calc.pyx":329
  *                         density_factor, drag, self.weight, _flag
  *                     ))
  *                     if current_item == ranges_length:             # <<<<<<<<<<<<<<
  *                         break
  * 
  */
         }
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":282
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":323
  * 
  *                 # Record TrajectoryData row
  *                 if _flag & filter_flags:             # <<<<<<<<<<<<<<
  *                     ranges.append(create_trajectory_row(
  *                         time, range_vector, velocity_vector,
  */
       }
 
-      /* "py_ballisticcalc_exts/trajectory_calc.pyx":255
+      /* "py_ballisticcalc_exts/trajectory_calc.pyx":295
  *                 self.alt0 + range_vector.y)
  * 
  *             if filter_flags:             # <<<<<<<<<<<<<<
  *                 # Zero-crossing checks
  *                 if range_vector.x > 0:
  */
     }
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":291
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":332
  *                         break
  * 
  *             previous_mach = velocity / mach             # <<<<<<<<<<<<<<
  * 
  *             #region Ballistic calculation step
  */
-    if (unlikely(__pyx_v_mach == 0)) {
-      PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(0, 291, __pyx_L1_error)
-    }
     __pyx_v_previous_mach = (__pyx_v_velocity / __pyx_v_mach);
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":294
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":335
  * 
  *             #region Ballistic calculation step
  *             delta_time = self.calc_step / velocity_vector.x             # <<<<<<<<<<<<<<
- *             velocity_adjusted = velocity_vector - wind_vector
- *             velocity = velocity_adjusted.magnitude()
+ * 
+ *             # using .subtract insstead of "/" better optimized by cython
  */
-    if (unlikely(__pyx_v_velocity_vector->x == 0)) {
-      PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(0, 294, __pyx_L1_error)
-    }
     __pyx_v_delta_time = (__pyx_v_self->calc_step / __pyx_v_velocity_vector->x);
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":295
- *             #region Ballistic calculation step
- *             delta_time = self.calc_step / velocity_vector.x
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":338
+ * 
+ *             # using .subtract insstead of "/" better optimized by cython
  *             velocity_adjusted = velocity_vector - wind_vector             # <<<<<<<<<<<<<<
  *             velocity = velocity_adjusted.magnitude()
  *             drag = density_factor * velocity * self.drag_by_mach(velocity / mach)
  */
-    __pyx_t_2 = PyNumber_Subtract(((PyObject *)__pyx_v_velocity_vector), ((PyObject *)__pyx_v_wind_vector)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 295, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector))))) __PYX_ERR(0, 295, __pyx_L1_error)
-    __Pyx_XDECREF_SET(__pyx_v_velocity_adjusted, ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_2));
-    __pyx_t_2 = 0;
+    __pyx_t_1 = PyNumber_Subtract(((PyObject *)__pyx_v_velocity_vector), ((PyObject *)__pyx_v_wind_vector)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 338, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector))))) __PYX_ERR(0, 338, __pyx_L1_error)
+    __Pyx_XDECREF_SET(__pyx_v_velocity_adjusted, ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_1));
+    __pyx_t_1 = 0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":296
- *             delta_time = self.calc_step / velocity_vector.x
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":339
+ *             # using .subtract insstead of "/" better optimized by cython
  *             velocity_adjusted = velocity_vector - wind_vector
  *             velocity = velocity_adjusted.magnitude()             # <<<<<<<<<<<<<<
  *             drag = density_factor * velocity * self.drag_by_mach(velocity / mach)
  *             velocity_vector -= (velocity_adjusted * drag - self.gravity_vector) * delta_time
  */
-    __pyx_t_11 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_velocity_adjusted->__pyx_vtab)->magnitude(__pyx_v_velocity_adjusted); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 296, __pyx_L1_error)
+    __pyx_t_11 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_velocity_adjusted->__pyx_vtab)->magnitude(__pyx_v_velocity_adjusted); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 339, __pyx_L1_error)
     __pyx_v_velocity = __pyx_t_11;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":297
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":340
  *             velocity_adjusted = velocity_vector - wind_vector
  *             velocity = velocity_adjusted.magnitude()
  *             drag = density_factor * velocity * self.drag_by_mach(velocity / mach)             # <<<<<<<<<<<<<<
  *             velocity_vector -= (velocity_adjusted * drag - self.gravity_vector) * delta_time
  *             delta_range_vector = Vector(self.calc_step,
  */
-    if (unlikely(__pyx_v_mach == 0)) {
-      PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(0, 297, __pyx_L1_error)
-    }
-    __pyx_t_11 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self->__pyx_vtab)->drag_by_mach(__pyx_v_self, (__pyx_v_velocity / __pyx_v_mach)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 297, __pyx_L1_error)
+    __pyx_t_11 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self->__pyx_vtab)->drag_by_mach(__pyx_v_self, (__pyx_v_velocity / __pyx_v_mach)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 340, __pyx_L1_error)
     __pyx_v_drag = ((__pyx_v_density_factor * __pyx_v_velocity) * __pyx_t_11);
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":298
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":341
  *             velocity = velocity_adjusted.magnitude()
  *             drag = density_factor * velocity * self.drag_by_mach(velocity / mach)
  *             velocity_vector -= (velocity_adjusted * drag - self.gravity_vector) * delta_time             # <<<<<<<<<<<<<<
  *             delta_range_vector = Vector(self.calc_step,
  *                                         velocity_vector.y * delta_time,
  */
-    __pyx_t_2 = PyFloat_FromDouble(__pyx_v_drag); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 298, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = PyNumber_Multiply(((PyObject *)__pyx_v_velocity_adjusted), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 298, __pyx_L1_error)
+    __pyx_t_1 = PyFloat_FromDouble(__pyx_v_drag); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 341, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = PyNumber_Subtract(__pyx_t_1, ((PyObject *)__pyx_v_self->gravity_vector)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 298, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_8 = PyNumber_Multiply(((PyObject *)__pyx_v_velocity_adjusted), __pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 341, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyFloat_FromDouble(__pyx_v_delta_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 298, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Subtract(__pyx_t_8, ((PyObject *)__pyx_v_self->gravity_vector)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 341, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_8 = PyNumber_Multiply(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 298, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __pyx_t_8 = PyFloat_FromDouble(__pyx_v_delta_time); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 341, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_2 = PyNumber_Multiply(__pyx_t_1, __pyx_t_8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 341, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyNumber_InPlaceSubtract(((PyObject *)__pyx_v_velocity_vector), __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 298, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector))))) __PYX_ERR(0, 298, __pyx_L1_error)
-    __Pyx_DECREF_SET(__pyx_v_velocity_vector, ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_1));
-    __pyx_t_1 = 0;
+    __pyx_t_8 = PyNumber_InPlaceSubtract(((PyObject *)__pyx_v_velocity_vector), __pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 341, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    if (!(likely(((__pyx_t_8) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_8, __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector))))) __PYX_ERR(0, 341, __pyx_L1_error)
+    __Pyx_DECREF_SET(__pyx_v_velocity_vector, ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_8));
+    __pyx_t_8 = 0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":299
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":342
  *             drag = density_factor * velocity * self.drag_by_mach(velocity / mach)
  *             velocity_vector -= (velocity_adjusted * drag - self.gravity_vector) * delta_time
  *             delta_range_vector = Vector(self.calc_step,             # <<<<<<<<<<<<<<
  *                                         velocity_vector.y * delta_time,
  *                                         velocity_vector.z * delta_time)
  */
-    __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->calc_step); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 299, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_8 = PyFloat_FromDouble(__pyx_v_self->calc_step); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 342, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":300
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":343
  *             velocity_vector -= (velocity_adjusted * drag - self.gravity_vector) * delta_time
  *             delta_range_vector = Vector(self.calc_step,
  *                                         velocity_vector.y * delta_time,             # <<<<<<<<<<<<<<
  *                                         velocity_vector.z * delta_time)
  *             range_vector += delta_range_vector
  */
-    __pyx_t_8 = PyFloat_FromDouble((__pyx_v_velocity_vector->y * __pyx_v_delta_time)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 300, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_velocity_vector->y * __pyx_v_delta_time)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 343, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":301
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":344
  *             delta_range_vector = Vector(self.calc_step,
  *                                         velocity_vector.y * delta_time,
  *                                         velocity_vector.z * delta_time)             # <<<<<<<<<<<<<<
  *             range_vector += delta_range_vector
  *             velocity = velocity_vector.magnitude()
  */
-    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_velocity_vector->z * __pyx_v_delta_time)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 301, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyFloat_FromDouble((__pyx_v_velocity_vector->z * __pyx_v_delta_time)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 344, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":299
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":342
  *             drag = density_factor * velocity * self.drag_by_mach(velocity / mach)
  *             velocity_vector -= (velocity_adjusted * drag - self.gravity_vector) * delta_time
  *             delta_range_vector = Vector(self.calc_step,             # <<<<<<<<<<<<<<
  *                                         velocity_vector.y * delta_time,
  *                                         velocity_vector.z * delta_time)
  */
-    __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 299, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 342, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_GIVEREF(__pyx_t_1);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_1)) __PYX_ERR(0, 299, __pyx_L1_error);
     __Pyx_GIVEREF(__pyx_t_8);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_8)) __PYX_ERR(0, 299, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_8)) __PYX_ERR(0, 342, __pyx_L1_error);
     __Pyx_GIVEREF(__pyx_t_2);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 2, __pyx_t_2)) __PYX_ERR(0, 299, __pyx_L1_error);
-    __pyx_t_1 = 0;
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_2)) __PYX_ERR(0, 342, __pyx_L1_error);
+    __Pyx_GIVEREF(__pyx_t_1);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 2, __pyx_t_1)) __PYX_ERR(0, 342, __pyx_L1_error);
     __pyx_t_8 = 0;
     __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_t_7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 299, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 342, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_delta_range_vector, ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_2));
-    __pyx_t_2 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_delta_range_vector, ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_1));
+    __pyx_t_1 = 0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":302
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":345
  *                                         velocity_vector.y * delta_time,
  *                                         velocity_vector.z * delta_time)
  *             range_vector += delta_range_vector             # <<<<<<<<<<<<<<
  *             velocity = velocity_vector.magnitude()
  *             time += delta_range_vector.magnitude() / velocity
  */
-    __pyx_t_2 = PyNumber_InPlaceAdd(((PyObject *)__pyx_v_range_vector), ((PyObject *)__pyx_v_delta_range_vector)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 302, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector))))) __PYX_ERR(0, 302, __pyx_L1_error)
-    __Pyx_DECREF_SET(__pyx_v_range_vector, ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_2));
-    __pyx_t_2 = 0;
+    __pyx_t_1 = PyNumber_InPlaceAdd(((PyObject *)__pyx_v_range_vector), ((PyObject *)__pyx_v_delta_range_vector)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 345, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector))))) __PYX_ERR(0, 345, __pyx_L1_error)
+    __Pyx_DECREF_SET(__pyx_v_range_vector, ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_1));
+    __pyx_t_1 = 0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":303
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":346
  *                                         velocity_vector.z * delta_time)
  *             range_vector += delta_range_vector
  *             velocity = velocity_vector.magnitude()             # <<<<<<<<<<<<<<
  *             time += delta_range_vector.magnitude() / velocity
  * 
  */
-    __pyx_t_11 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_velocity_vector->__pyx_vtab)->magnitude(__pyx_v_velocity_vector); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 303, __pyx_L1_error)
+    __pyx_t_11 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_velocity_vector->__pyx_vtab)->magnitude(__pyx_v_velocity_vector); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 346, __pyx_L1_error)
     __pyx_v_velocity = __pyx_t_11;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":304
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":347
  *             range_vector += delta_range_vector
  *             velocity = velocity_vector.magnitude()
  *             time += delta_range_vector.magnitude() / velocity             # <<<<<<<<<<<<<<
  * 
  *             if velocity < cMinimumVelocity or range_vector.y < cMaximumDrop:
  */
-    __pyx_t_11 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_delta_range_vector->__pyx_vtab)->magnitude(__pyx_v_delta_range_vector); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 304, __pyx_L1_error)
-    if (unlikely(__pyx_v_velocity == 0)) {
-      PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(0, 304, __pyx_L1_error)
-    }
+    __pyx_t_11 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_delta_range_vector->__pyx_vtab)->magnitude(__pyx_v_delta_range_vector); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 347, __pyx_L1_error)
     __pyx_v_time = (__pyx_v_time + (__pyx_t_11 / __pyx_v_velocity));
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":306
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":349
  *             time += delta_range_vector.magnitude() / velocity
  * 
  *             if velocity < cMinimumVelocity or range_vector.y < cMaximumDrop:             # <<<<<<<<<<<<<<
  *                 break
  *             #endregion
  */
     __pyx_t_9 = (__pyx_v_velocity < __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cMinimumVelocity);
     if (!__pyx_t_9) {
     } else {
       __pyx_t_6 = __pyx_t_9;
-      goto __pyx_L25_bool_binop_done;
+      goto __pyx_L23_bool_binop_done;
     }
     __pyx_t_9 = (__pyx_v_range_vector->y < __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cMaximumDrop);
     __pyx_t_6 = __pyx_t_9;
-    __pyx_L25_bool_binop_done:;
+    __pyx_L23_bool_binop_done:;
     if (__pyx_t_6) {
 
-      /* "py_ballisticcalc_exts/trajectory_calc.pyx":307
+      /* "py_ballisticcalc_exts/trajectory_calc.pyx":350
  * 
  *             if velocity < cMinimumVelocity or range_vector.y < cMaximumDrop:
  *                 break             # <<<<<<<<<<<<<<
  *             #endregion
  *         #endregion
  */
       goto __pyx_L8_break;
 
-      /* "py_ballisticcalc_exts/trajectory_calc.pyx":306
+      /* "py_ballisticcalc_exts/trajectory_calc.pyx":349
  *             time += delta_range_vector.magnitude() / velocity
  * 
  *             if velocity < cMinimumVelocity or range_vector.y < cMaximumDrop:             # <<<<<<<<<<<<<<
  *                 break
  *             #endregion
  */
     }
   }
   __pyx_L8_break:;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":311
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":354
  *         #endregion
  *         # If filter_flags == 0 then all we want is the ending value
  *         if not filter_flags:             # <<<<<<<<<<<<<<
  *             ranges.append(create_trajectory_row(
  *                         time, range_vector, velocity_vector,
  */
-  __pyx_t_6 = (!__pyx_v_filter_flags);
+  __pyx_t_6 = (!(__pyx_v_filter_flags != 0));
   if (__pyx_t_6) {
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":314
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":357
  *             ranges.append(create_trajectory_row(
  *                         time, range_vector, velocity_vector,
  *                         velocity, mach, self.spin_drift(time), self.look_angle,             # <<<<<<<<<<<<<<
  *                         density_factor, drag, self.weight, _flag))
  *         return ranges
  */
-    __pyx_t_11 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self->__pyx_vtab)->spin_drift(__pyx_v_self, __pyx_v_time); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 314, __pyx_L1_error)
+    __pyx_t_11 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self->__pyx_vtab)->spin_drift(__pyx_v_self, __pyx_v_time); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 357, __pyx_L1_error)
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":315
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":358
  *                         time, range_vector, velocity_vector,
  *                         velocity, mach, self.spin_drift(time), self.look_angle,
  *                         density_factor, drag, self.weight, _flag))             # <<<<<<<<<<<<<<
  *         return ranges
  * 
  */
-    if (unlikely(!__pyx_v__flag)) { __Pyx_RaiseUnboundLocalError("_flag"); __PYX_ERR(0, 315, __pyx_L1_error) }
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v__flag); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 358, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":312
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":355
  *         # If filter_flags == 0 then all we want is the ending value
  *         if not filter_flags:
  *             ranges.append(create_trajectory_row(             # <<<<<<<<<<<<<<
  *                         time, range_vector, velocity_vector,
  *                         velocity, mach, self.spin_drift(time), self.look_angle,
  */
-    __pyx_t_2 = __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_create_trajectory_row(__pyx_v_time, __pyx_v_range_vector, __pyx_v_velocity_vector, __pyx_v_velocity, __pyx_v_mach, __pyx_t_11, __pyx_v_self->look_angle, __pyx_v_density_factor, __pyx_v_drag, __pyx_v_self->weight, __pyx_v__flag); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 312, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_12 = __Pyx_PyList_Append(__pyx_v_ranges, __pyx_t_2); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 312, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_7 = __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_create_trajectory_row(__pyx_v_time, __pyx_v_range_vector, __pyx_v_velocity_vector, __pyx_v_velocity, __pyx_v_mach, __pyx_t_11, __pyx_v_self->look_angle, __pyx_v_density_factor, __pyx_v_drag, __pyx_v_self->weight, __pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 355, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_12 = __Pyx_PyList_Append(__pyx_v_ranges, __pyx_t_7); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 355, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":311
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":354
  *         #endregion
  *         # If filter_flags == 0 then all we want is the ending value
  *         if not filter_flags:             # <<<<<<<<<<<<<<
  *             ranges.append(create_trajectory_row(
  *                         time, range_vector, velocity_vector,
  */
   }
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":316
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":359
  *                         velocity, mach, self.spin_drift(time), self.look_angle,
  *                         density_factor, drag, self.weight, _flag))
  *         return ranges             # <<<<<<<<<<<<<<
  * 
  *     cdef double drag_by_mach(self, double mach):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_ranges);
   __pyx_r = __pyx_v_ranges;
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":198
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":235
  *         return Angular.Radian(self.barrel_elevation)
  * 
  *     cdef _trajectory(TrajectoryCalc self, object shot_info,             # <<<<<<<<<<<<<<
- *                      double maximum_range, double step, CTrajFlag filter_flags):
+ *                      double maximum_range, double step, int filter_flags):
  *         cdef:
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_AddTraceback("py_ballisticcalc_exts.trajectory_calc.TrajectoryCalc._trajectory", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v__flag);
-  __Pyx_XDECREF(__pyx_v_seen_zero);
   __Pyx_XDECREF(__pyx_v_ranges);
   __Pyx_XDECREF((PyObject *)__pyx_v_velocity_vector);
   __Pyx_XDECREF((PyObject *)__pyx_v_velocity_adjusted);
   __Pyx_XDECREF((PyObject *)__pyx_v_range_vector);
   __Pyx_XDECREF((PyObject *)__pyx_v_delta_range_vector);
   __Pyx_XDECREF((PyObject *)__pyx_v_wind_vector);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":318
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":361
  *         return ranges
  * 
  *     cdef double drag_by_mach(self, double mach):             # <<<<<<<<<<<<<<
  *         """ Drag force = V^2 * Cd * AirDensity * S / 2m where:
  *             cStandardDensity of Air = 0.076474 lb/ft^3
  */
 
@@ -8885,46 +9056,41 @@
   PyObject *__pyx_t_2 = NULL;
   double __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("drag_by_mach", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":326
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":369
  *         Thus: The magic constant found here = StandardDensity * pi / (4 * 2 * 144)
  *         """
  *         cdef double cd = calculate_by_curve(self._table_data, self._curve, mach)             # <<<<<<<<<<<<<<
  *         return cd * 2.08551e-04 / self._bc
  * 
  */
   __pyx_t_1 = __pyx_v_self->_table_data;
   __Pyx_INCREF(__pyx_t_1);
   __pyx_t_2 = __pyx_v_self->_curve;
   __Pyx_INCREF(__pyx_t_2);
-  __pyx_t_3 = __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_calculate_by_curve(((PyObject*)__pyx_t_1), ((PyObject*)__pyx_t_2), __pyx_v_mach); if (unlikely(__pyx_t_3 == ((double)-1) && PyErr_Occurred())) __PYX_ERR(0, 326, __pyx_L1_error)
+  __pyx_t_3 = __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_calculate_by_curve(((PyObject*)__pyx_t_1), ((PyObject*)__pyx_t_2), __pyx_v_mach); if (unlikely(__pyx_t_3 == ((double)-1) && PyErr_Occurred())) __PYX_ERR(0, 369, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_cd = __pyx_t_3;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":327
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":370
  *         """
  *         cdef double cd = calculate_by_curve(self._table_data, self._curve, mach)
  *         return cd * 2.08551e-04 / self._bc             # <<<<<<<<<<<<<<
  * 
  *     cdef double spin_drift(self, double time):
  */
-  __pyx_t_3 = (__pyx_v_cd * 2.08551e-04);
-  if (unlikely(__pyx_v_self->_bc == 0)) {
-    PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(0, 327, __pyx_L1_error)
-  }
-  __pyx_r = (__pyx_t_3 / __pyx_v_self->_bc);
+  __pyx_r = ((__pyx_v_cd * 2.08551e-04) / __pyx_v_self->_bc);
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":318
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":361
  *         return ranges
  * 
  *     cdef double drag_by_mach(self, double mach):             # <<<<<<<<<<<<<<
  *         """ Drag force = V^2 * Cd * AirDensity * S / 2m where:
  *             cStandardDensity of Air = 0.076474 lb/ft^3
  */
 
@@ -8935,123 +9101,96 @@
   __Pyx_AddTraceback("py_ballisticcalc_exts.trajectory_calc.TrajectoryCalc.drag_by_mach", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":329
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":372
  *         return cd * 2.08551e-04 / self._bc
  * 
  *     cdef double spin_drift(self, double time):             # <<<<<<<<<<<<<<
  *         """Litz spin-drift approximation
  *         :param time: Time of flight
  */
 
 static double __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_spin_drift(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, double __pyx_v_time) {
-  PyObject *__pyx_v_sign = NULL;
+  int __pyx_v_sign;
   double __pyx_r;
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  double __pyx_t_4;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("spin_drift", 1);
+  int __pyx_t_2;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":334
- *         :return: windage due to spin drift, in feet
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":378
  *         """
+ *         cdef int sign
  *         if self.twist != 0:             # <<<<<<<<<<<<<<
  *             sign = 1 if self.twist > 0 else -1
  *             return sign * (1.25 * (self.stability_coefficient + 1.2) * pow(time, 1.83) ) / 12
  */
   __pyx_t_1 = (__pyx_v_self->twist != 0.0);
   if (__pyx_t_1) {
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":335
- *         """
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":379
+ *         cdef int sign
  *         if self.twist != 0:
  *             sign = 1 if self.twist > 0 else -1             # <<<<<<<<<<<<<<
  *             return sign * (1.25 * (self.stability_coefficient + 1.2) * pow(time, 1.83) ) / 12
  *         return 0
  */
     __pyx_t_1 = (__pyx_v_self->twist > 0.0);
     if (__pyx_t_1) {
-      __Pyx_INCREF(__pyx_int_1);
-      __pyx_t_2 = __pyx_int_1;
+      __pyx_t_2 = 1;
     } else {
-      __Pyx_INCREF(__pyx_int_neg_1);
-      __pyx_t_2 = __pyx_int_neg_1;
+      __pyx_t_2 = -1;
     }
     __pyx_v_sign = __pyx_t_2;
-    __pyx_t_2 = 0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":336
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":380
  *         if self.twist != 0:
  *             sign = 1 if self.twist > 0 else -1
  *             return sign * (1.25 * (self.stability_coefficient + 1.2) * pow(time, 1.83) ) / 12             # <<<<<<<<<<<<<<
  *         return 0
  * 
  */
-    __pyx_t_2 = PyFloat_FromDouble(((1.25 * (__pyx_v_self->stability_coefficient + 1.2)) * pow(__pyx_v_time, 1.83))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 336, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_Multiply(__pyx_v_sign, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 336, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyInt_TrueDivideObjC(__pyx_t_3, __pyx_int_12, 12, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 336, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 336, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_r = __pyx_t_4;
+    __pyx_r = ((__pyx_v_sign * ((1.25 * (__pyx_v_self->stability_coefficient + 1.2)) * pow(__pyx_v_time, 1.83))) / 12.0);
     goto __pyx_L0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":334
- *         :return: windage due to spin drift, in feet
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":378
  *         """
+ *         cdef int sign
  *         if self.twist != 0:             # <<<<<<<<<<<<<<
  *             sign = 1 if self.twist > 0 else -1
  *             return sign * (1.25 * (self.stability_coefficient + 1.2) * pow(time, 1.83) ) / 12
  */
   }
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":337
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":381
  *             sign = 1 if self.twist > 0 else -1
  *             return sign * (1.25 * (self.stability_coefficient + 1.2) * pow(time, 1.83) ) / 12
  *         return 0             # <<<<<<<<<<<<<<
  * 
  *     cdef double calc_stability_coefficient(self, object atmo):
  */
   __pyx_r = 0.0;
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":329
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":372
  *         return cd * 2.08551e-04 / self._bc
  * 
  *     cdef double spin_drift(self, double time):             # <<<<<<<<<<<<<<
  *         """Litz spin-drift approximation
  *         :param time: Time of flight
  */
 
   /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("py_ballisticcalc_exts.trajectory_calc.TrajectoryCalc.spin_drift", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_sign);
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":339
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":383
  *         return 0
  * 
  *     cdef double calc_stability_coefficient(self, object atmo):             # <<<<<<<<<<<<<<
  *         """Miller stability coefficient"""
  *         cdef:
  */
 
@@ -9063,25 +9202,24 @@
   double __pyx_v_ft;
   double __pyx_v_pt;
   double __pyx_v_ftp;
   double __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
-  double __pyx_t_3;
-  double __pyx_t_4;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
+  double __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("calc_stability_coefficient", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":343
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":387
  *         cdef:
  *             double twist_rate, length, sd, fv, ft, pt, ftp
  *         if self.twist and self.length and self.diameter:             # <<<<<<<<<<<<<<
  *             twist_rate = fabs(self.twist) / self.diameter
  *             length = self.length / self.diameter
  */
   __pyx_t_2 = (__pyx_v_self->twist != 0);
@@ -9097,164 +9235,145 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_2 = (__pyx_v_self->diameter != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":344
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":388
  *             double twist_rate, length, sd, fv, ft, pt, ftp
  *         if self.twist and self.length and self.diameter:
  *             twist_rate = fabs(self.twist) / self.diameter             # <<<<<<<<<<<<<<
  *             length = self.length / self.diameter
  *             sd = 30 * self.weight / (pow(twist_rate, 2) * pow(self.diameter, 3) * length * (1 + pow(length, 2)))
  */
-    __pyx_t_3 = fabs(__pyx_v_self->twist);
-    if (unlikely(__pyx_v_self->diameter == 0)) {
-      PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(0, 344, __pyx_L1_error)
-    }
-    __pyx_v_twist_rate = (__pyx_t_3 / __pyx_v_self->diameter);
+    __pyx_v_twist_rate = (fabs(__pyx_v_self->twist) / __pyx_v_self->diameter);
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":345
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":389
  *         if self.twist and self.length and self.diameter:
  *             twist_rate = fabs(self.twist) / self.diameter
  *             length = self.length / self.diameter             # <<<<<<<<<<<<<<
  *             sd = 30 * self.weight / (pow(twist_rate, 2) * pow(self.diameter, 3) * length * (1 + pow(length, 2)))
  *             fv = pow(self.muzzle_velocity / 2800, 1.0 / 3.0)
  */
-    if (unlikely(__pyx_v_self->diameter == 0)) {
-      PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(0, 345, __pyx_L1_error)
-    }
     __pyx_v_length = (__pyx_v_self->length / __pyx_v_self->diameter);
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":346
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":390
  *             twist_rate = fabs(self.twist) / self.diameter
  *             length = self.length / self.diameter
  *             sd = 30 * self.weight / (pow(twist_rate, 2) * pow(self.diameter, 3) * length * (1 + pow(length, 2)))             # <<<<<<<<<<<<<<
  *             fv = pow(self.muzzle_velocity / 2800, 1.0 / 3.0)
  *             ft = atmo.temperature >> Temperature.Fahrenheit
  */
-    __pyx_t_3 = (30.0 * __pyx_v_self->weight);
-    __pyx_t_4 = (((pow(__pyx_v_twist_rate, 2.0) * pow(__pyx_v_self->diameter, 3.0)) * __pyx_v_length) * (1.0 + pow(__pyx_v_length, 2.0)));
-    if (unlikely(__pyx_t_4 == 0)) {
-      PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(0, 346, __pyx_L1_error)
-    }
-    __pyx_v_sd = (__pyx_t_3 / __pyx_t_4);
+    __pyx_v_sd = ((30.0 * __pyx_v_self->weight) / (((pow(__pyx_v_twist_rate, 2.0) * pow(__pyx_v_self->diameter, 3.0)) * __pyx_v_length) * (1.0 + pow(__pyx_v_length, 2.0))));
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":347
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":391
  *             length = self.length / self.diameter
  *             sd = 30 * self.weight / (pow(twist_rate, 2) * pow(self.diameter, 3) * length * (1 + pow(length, 2)))
  *             fv = pow(self.muzzle_velocity / 2800, 1.0 / 3.0)             # <<<<<<<<<<<<<<
  *             ft = atmo.temperature >> Temperature.Fahrenheit
  *             pt = atmo.pressure >> Pressure.InHg
  */
     __pyx_v_fv = pow((__pyx_v_self->muzzle_velocity / 2800.0), (1.0 / 3.0));
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":348
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":392
  *             sd = 30 * self.weight / (pow(twist_rate, 2) * pow(self.diameter, 3) * length * (1 + pow(length, 2)))
  *             fv = pow(self.muzzle_velocity / 2800, 1.0 / 3.0)
  *             ft = atmo.temperature >> Temperature.Fahrenheit             # <<<<<<<<<<<<<<
  *             pt = atmo.pressure >> Pressure.InHg
  *             ftp = ((ft + 460) / (59 + 460)) * (29.92 / pt)
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_atmo, __pyx_n_s_temperature); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 348, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_atmo, __pyx_n_s_temperature); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 392, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Temperature); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 392, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_Fahrenheit); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 392, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Temperature); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 348, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_Fahrenheit); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 348, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = PyNumber_Rshift(__pyx_t_5, __pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 348, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_4 = PyNumber_Rshift(__pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 392, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_6); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 348, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_v_ft = __pyx_t_4;
+    __pyx_t_6 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_6 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 392, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_v_ft = __pyx_t_6;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":349
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":393
  *             fv = pow(self.muzzle_velocity / 2800, 1.0 / 3.0)
  *             ft = atmo.temperature >> Temperature.Fahrenheit
  *             pt = atmo.pressure >> Pressure.InHg             # <<<<<<<<<<<<<<
  *             ftp = ((ft + 460) / (59 + 460)) * (29.92 / pt)
  *             return sd * fv * ftp
  */
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_atmo, __pyx_n_s_pressure); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 349, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_Pressure); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 349, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_InHg); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 349, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_atmo, __pyx_n_s_pressure); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Pressure); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 393, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = PyNumber_Rshift(__pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 349, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_InHg); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_7); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 349, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_v_pt = __pyx_t_4;
+    __pyx_t_5 = PyNumber_Rshift(__pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_6 = __pyx_PyFloat_AsDouble(__pyx_t_5); if (unlikely((__pyx_t_6 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 393, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_v_pt = __pyx_t_6;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":350
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":394
  *             ft = atmo.temperature >> Temperature.Fahrenheit
  *             pt = atmo.pressure >> Pressure.InHg
  *             ftp = ((ft + 460) / (59 + 460)) * (29.92 / pt)             # <<<<<<<<<<<<<<
  *             return sd * fv * ftp
  *         return 0
  */
-    if (unlikely(__pyx_v_pt == 0)) {
-      PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(0, 350, __pyx_L1_error)
-    }
     __pyx_v_ftp = (((__pyx_v_ft + 460.0) / 519.0) * (29.92 / __pyx_v_pt));
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":351
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":395
  *             pt = atmo.pressure >> Pressure.InHg
  *             ftp = ((ft + 460) / (59 + 460)) * (29.92 / pt)
  *             return sd * fv * ftp             # <<<<<<<<<<<<<<
  *         return 0
  * 
  */
     __pyx_r = ((__pyx_v_sd * __pyx_v_fv) * __pyx_v_ftp);
     goto __pyx_L0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":343
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":387
  *         cdef:
  *             double twist_rate, length, sd, fv, ft, pt, ftp
  *         if self.twist and self.length and self.diameter:             # <<<<<<<<<<<<<<
  *             twist_rate = fabs(self.twist) / self.diameter
  *             length = self.length / self.diameter
  */
   }
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":352
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":396
  *             ftp = ((ft + 460) / (59 + 460)) * (29.92 / pt)
  *             return sd * fv * ftp
  *         return 0             # <<<<<<<<<<<<<<
  * 
  * cdef Vector wind_to_vector(object wind):
  */
   __pyx_r = 0.0;
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":339
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":383
  *         return 0
  * 
  *     cdef double calc_stability_coefficient(self, object atmo):             # <<<<<<<<<<<<<<
  *         """Miller stability coefficient"""
  *         cdef:
  */
 
   /* function exit code */
   __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
   __Pyx_AddTraceback("py_ballisticcalc_exts.trajectory_calc.TrajectoryCalc.calc_stability_coefficient", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -9269,15 +9388,14 @@
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
 PyDoc_STRVAR(__pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_6__reduce_cython__, "TrajectoryCalc.__reduce_cython__(self)");
-static PyMethodDef __pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_7__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_7__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_6__reduce_cython__};
 static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_7__reduce_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
@@ -9661,15 +9779,14 @@
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
 PyDoc_STRVAR(__pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_8__setstate_cython__, "TrajectoryCalc.__setstate_cython__(self, __pyx_state)");
-static PyMethodDef __pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_9__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_9__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_8__setstate_cython__};
 static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_9__setstate_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
@@ -9788,15 +9905,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":354
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":398
  *         return 0
  * 
  * cdef Vector wind_to_vector(object wind):             # <<<<<<<<<<<<<<
  *     cdef:
  *         double range_component = (wind.velocity >> Velocity.FPS) * cos(wind.direction_from >> Angular.Radian)
  */
 
@@ -9811,127 +9928,127 @@
   PyObject *__pyx_t_4 = NULL;
   double __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("wind_to_vector", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":356
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":400
  * cdef Vector wind_to_vector(object wind):
  *     cdef:
  *         double range_component = (wind.velocity >> Velocity.FPS) * cos(wind.direction_from >> Angular.Radian)             # <<<<<<<<<<<<<<
  *         double cross_component = (wind.velocity >> Velocity.FPS) * sin(wind.direction_from >> Angular.Radian)
  *     return Vector(range_component, 0., cross_component)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_wind, __pyx_n_s_velocity); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 356, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_wind, __pyx_n_s_velocity); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Velocity); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 356, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Velocity); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_FPS); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 356, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_FPS); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Rshift(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 356, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Rshift(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_wind, __pyx_n_s_direction_from); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 356, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_wind, __pyx_n_s_direction_from); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Angular); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 356, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Angular); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Radian); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 356, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Radian); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Rshift(__pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 356, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Rshift(__pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 356, __pyx_L1_error)
+  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyFloat_FromDouble(cos(__pyx_t_5)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 356, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(cos(__pyx_t_5)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = PyNumber_Multiply(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 356, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Multiply(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 356, __pyx_L1_error)
+  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_range_component = __pyx_t_5;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":357
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":401
  *     cdef:
  *         double range_component = (wind.velocity >> Velocity.FPS) * cos(wind.direction_from >> Angular.Radian)
  *         double cross_component = (wind.velocity >> Velocity.FPS) * sin(wind.direction_from >> Angular.Radian)             # <<<<<<<<<<<<<<
  *     return Vector(range_component, 0., cross_component)
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_wind, __pyx_n_s_velocity); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 357, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_wind, __pyx_n_s_velocity); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 401, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Velocity); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 357, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Velocity); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 401, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_FPS); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 357, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_FPS); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 401, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Rshift(__pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 357, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Rshift(__pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 401, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_wind, __pyx_n_s_direction_from); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 357, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_wind, __pyx_n_s_direction_from); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 401, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Angular); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 357, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Angular); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 401, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_Radian); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 357, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_Radian); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 401, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyNumber_Rshift(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 357, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Rshift(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 401, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 357, __pyx_L1_error)
+  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 401, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyFloat_FromDouble(sin(__pyx_t_5)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 357, __pyx_L1_error)
+  __pyx_t_4 = PyFloat_FromDouble(sin(__pyx_t_5)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 401, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 357, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 401, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 357, __pyx_L1_error)
+  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 401, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_cross_component = __pyx_t_5;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":358
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":402
  *         double range_component = (wind.velocity >> Velocity.FPS) * cos(wind.direction_from >> Angular.Radian)
  *         double cross_component = (wind.velocity >> Velocity.FPS) * sin(wind.direction_from >> Angular.Radian)
  *     return Vector(range_component, 0., cross_component)             # <<<<<<<<<<<<<<
  * 
  * cdef create_trajectory_row(double time, Vector range_vector, Vector velocity_vector,
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
-  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_range_component); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 358, __pyx_L1_error)
+  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_range_component); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyFloat_FromDouble(__pyx_v_cross_component); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 358, __pyx_L1_error)
+  __pyx_t_4 = PyFloat_FromDouble(__pyx_v_cross_component); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 358, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_3)) __PYX_ERR(0, 358, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_3)) __PYX_ERR(0, 402, __pyx_L1_error);
   __Pyx_INCREF(__pyx_float_0_);
   __Pyx_GIVEREF(__pyx_float_0_);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_float_0_)) __PYX_ERR(0, 358, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_float_0_)) __PYX_ERR(0, 402, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_4)) __PYX_ERR(0, 358, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_4)) __PYX_ERR(0, 402, __pyx_L1_error);
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_t_1, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 358, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_t_1, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_4);
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":354
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":398
  *         return 0
  * 
  * cdef Vector wind_to_vector(object wind):             # <<<<<<<<<<<<<<
  *     cdef:
  *         double range_component = (wind.velocity >> Velocity.FPS) * cos(wind.direction_from >> Angular.Radian)
  */
 
@@ -9945,15 +10062,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":360
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":404
  *     return Vector(range_component, 0., cross_component)
  * 
  * cdef create_trajectory_row(double time, Vector range_vector, Vector velocity_vector,             # <<<<<<<<<<<<<<
  *                            double velocity, double mach, double spin_drift, double look_angle,
  *                            double density_factor, double drag, double weight, object flag):
  */
 
@@ -9974,94 +10091,90 @@
   int __pyx_t_8;
   int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("create_trajectory_row", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":364
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":408
  *                            double density_factor, double drag, double weight, object flag):
  *     cdef:
  *         double windage = range_vector.z + spin_drift             # <<<<<<<<<<<<<<
  *         double drop_adjustment = get_correction(range_vector.x, range_vector.y)
  *         double windage_adjustment = get_correction(range_vector.x, windage)
  */
   __pyx_v_windage = (__pyx_v_range_vector->z + __pyx_v_spin_drift);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":365
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":409
  *     cdef:
  *         double windage = range_vector.z + spin_drift
  *         double drop_adjustment = get_correction(range_vector.x, range_vector.y)             # <<<<<<<<<<<<<<
  *         double windage_adjustment = get_correction(range_vector.x, windage)
  *         double trajectory_angle = atan(velocity_vector.y / velocity_vector.x)
  */
-  __pyx_t_1 = __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_get_correction(__pyx_v_range_vector->x, __pyx_v_range_vector->y); if (unlikely(__pyx_t_1 == ((double)-1) && PyErr_Occurred())) __PYX_ERR(0, 365, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_get_correction(__pyx_v_range_vector->x, __pyx_v_range_vector->y); if (unlikely(__pyx_t_1 == ((double)-1) && PyErr_Occurred())) __PYX_ERR(0, 409, __pyx_L1_error)
   __pyx_v_drop_adjustment = __pyx_t_1;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":366
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":410
  *         double windage = range_vector.z + spin_drift
  *         double drop_adjustment = get_correction(range_vector.x, range_vector.y)
  *         double windage_adjustment = get_correction(range_vector.x, windage)             # <<<<<<<<<<<<<<
  *         double trajectory_angle = atan(velocity_vector.y / velocity_vector.x)
  * 
  */
-  __pyx_t_1 = __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_get_correction(__pyx_v_range_vector->x, __pyx_v_windage); if (unlikely(__pyx_t_1 == ((double)-1) && PyErr_Occurred())) __PYX_ERR(0, 366, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_get_correction(__pyx_v_range_vector->x, __pyx_v_windage); if (unlikely(__pyx_t_1 == ((double)-1) && PyErr_Occurred())) __PYX_ERR(0, 410, __pyx_L1_error)
   __pyx_v_windage_adjustment = __pyx_t_1;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":367
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":411
  *         double drop_adjustment = get_correction(range_vector.x, range_vector.y)
  *         double windage_adjustment = get_correction(range_vector.x, windage)
  *         double trajectory_angle = atan(velocity_vector.y / velocity_vector.x)             # <<<<<<<<<<<<<<
  * 
  *     return TrajectoryData(
  */
-  if (unlikely(__pyx_v_velocity_vector->x == 0)) {
-    PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(0, 367, __pyx_L1_error)
-  }
   __pyx_v_trajectory_angle = atan((__pyx_v_velocity_vector->y / __pyx_v_velocity_vector->x));
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":369
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":413
  *         double trajectory_angle = atan(velocity_vector.y / velocity_vector.x)
  * 
  *     return TrajectoryData(             # <<<<<<<<<<<<<<
  *         time=time,
  *         distance=Distance.Foot(range_vector.x),
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_TrajectoryData); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 369, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_TrajectoryData); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 413, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":370
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":414
  * 
  *     return TrajectoryData(
  *         time=time,             # <<<<<<<<<<<<<<
  *         distance=Distance.Foot(range_vector.x),
  *         velocity=Velocity.FPS(velocity),
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 370, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyFloat_FromDouble(__pyx_v_time); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 370, __pyx_L1_error)
+  __pyx_t_4 = PyFloat_FromDouble(__pyx_v_time); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_time, __pyx_t_4) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_time, __pyx_t_4) < 0) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":371
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":415
  *     return TrajectoryData(
  *         time=time,
  *         distance=Distance.Foot(range_vector.x),             # <<<<<<<<<<<<<<
  *         velocity=Velocity.FPS(velocity),
  *         mach=velocity / mach,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Distance); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 371, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Distance); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 415, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_Foot); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 371, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_Foot); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 415, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_range_vector->x); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 371, __pyx_L1_error)
+  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_range_vector->x); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 415, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_7 = NULL;
   __pyx_t_8 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_7)) {
@@ -10074,34 +10187,34 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_5};
     __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 371, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 415, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_distance, __pyx_t_4) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_distance, __pyx_t_4) < 0) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":372
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":416
  *         time=time,
  *         distance=Distance.Foot(range_vector.x),
  *         velocity=Velocity.FPS(velocity),             # <<<<<<<<<<<<<<
  *         mach=velocity / mach,
  *         height=Distance.Foot(range_vector.y),
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Velocity); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 372, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Velocity); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 416, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_FPS); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 372, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_FPS); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 416, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = PyFloat_FromDouble(__pyx_v_velocity); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 372, __pyx_L1_error)
+  __pyx_t_6 = PyFloat_FromDouble(__pyx_v_velocity); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 416, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = NULL;
   __pyx_t_8 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_7)) {
@@ -10114,50 +10227,46 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_6};
     __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 372, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 416, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_velocity, __pyx_t_4) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_velocity, __pyx_t_4) < 0) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":373
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":417
  *         distance=Distance.Foot(range_vector.x),
  *         velocity=Velocity.FPS(velocity),
  *         mach=velocity / mach,             # <<<<<<<<<<<<<<
  *         height=Distance.Foot(range_vector.y),
  *         target_drop=Distance.Foot((range_vector.y - range_vector.x * tan(look_angle)) * cos(look_angle)),
  */
-  if (unlikely(__pyx_v_mach == 0)) {
-    PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(0, 373, __pyx_L1_error)
-  }
-  __pyx_t_4 = PyFloat_FromDouble((__pyx_v_velocity / __pyx_v_mach)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 373, __pyx_L1_error)
+  __pyx_t_4 = PyFloat_FromDouble((__pyx_v_velocity / __pyx_v_mach)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 417, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_mach, __pyx_t_4) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_mach, __pyx_t_4) < 0) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":374
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":418
  *         velocity=Velocity.FPS(velocity),
  *         mach=velocity / mach,
  *         height=Distance.Foot(range_vector.y),             # <<<<<<<<<<<<<<
  *         target_drop=Distance.Foot((range_vector.y - range_vector.x * tan(look_angle)) * cos(look_angle)),
  *         drop_adj=Angular.Radian(drop_adjustment - (look_angle if range_vector.x else 0)),
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Distance); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 374, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Distance); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 418, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_Foot); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 374, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_Foot); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 418, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_range_vector->y); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 374, __pyx_L1_error)
+  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_range_vector->y); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 418, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_7 = NULL;
   __pyx_t_8 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_7)) {
@@ -10170,34 +10279,34 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_5};
     __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 374, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_height, __pyx_t_4) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_height, __pyx_t_4) < 0) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":375
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":419
  *         mach=velocity / mach,
  *         height=Distance.Foot(range_vector.y),
  *         target_drop=Distance.Foot((range_vector.y - range_vector.x * tan(look_angle)) * cos(look_angle)),             # <<<<<<<<<<<<<<
  *         drop_adj=Angular.Radian(drop_adjustment - (look_angle if range_vector.x else 0)),
  *         windage=Distance.Foot(windage),
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Distance); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 375, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Distance); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 419, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_Foot); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 375, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_Foot); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 419, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = PyFloat_FromDouble(((__pyx_v_range_vector->y - (__pyx_v_range_vector->x * tan(__pyx_v_look_angle))) * cos(__pyx_v_look_angle))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 375, __pyx_L1_error)
+  __pyx_t_6 = PyFloat_FromDouble(((__pyx_v_range_vector->y - (__pyx_v_range_vector->x * tan(__pyx_v_look_angle))) * cos(__pyx_v_look_angle))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 419, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = NULL;
   __pyx_t_8 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_7)) {
@@ -10210,40 +10319,40 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_6};
     __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 375, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 419, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_target_drop, __pyx_t_4) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_target_drop, __pyx_t_4) < 0) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":376
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":420
  *         height=Distance.Foot(range_vector.y),
  *         target_drop=Distance.Foot((range_vector.y - range_vector.x * tan(look_angle)) * cos(look_angle)),
  *         drop_adj=Angular.Radian(drop_adjustment - (look_angle if range_vector.x else 0)),             # <<<<<<<<<<<<<<
  *         windage=Distance.Foot(windage),
  *         windage_adj=Angular.Radian(windage_adjustment),
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Angular); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 376, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Angular); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 420, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_Radian); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 376, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_Radian); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 420, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_9 = (__pyx_v_range_vector->x != 0);
   if (__pyx_t_9) {
     __pyx_t_1 = __pyx_v_look_angle;
   } else {
     __pyx_t_1 = 0.0;
   }
-  __pyx_t_5 = PyFloat_FromDouble((__pyx_v_drop_adjustment - __pyx_t_1)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 376, __pyx_L1_error)
+  __pyx_t_5 = PyFloat_FromDouble((__pyx_v_drop_adjustment - __pyx_t_1)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 420, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_7 = NULL;
   __pyx_t_8 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_7)) {
@@ -10256,34 +10365,34 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_5};
     __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 376, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 420, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_drop_adj, __pyx_t_4) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_drop_adj, __pyx_t_4) < 0) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":377
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":421
  *         target_drop=Distance.Foot((range_vector.y - range_vector.x * tan(look_angle)) * cos(look_angle)),
  *         drop_adj=Angular.Radian(drop_adjustment - (look_angle if range_vector.x else 0)),
  *         windage=Distance.Foot(windage),             # <<<<<<<<<<<<<<
  *         windage_adj=Angular.Radian(windage_adjustment),
  *         look_distance= Distance.Foot(range_vector.x / cos(look_angle)),
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Distance); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 377, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Distance); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 421, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_Foot); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 377, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_Foot); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 421, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = PyFloat_FromDouble(__pyx_v_windage); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 377, __pyx_L1_error)
+  __pyx_t_6 = PyFloat_FromDouble(__pyx_v_windage); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 421, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = NULL;
   __pyx_t_8 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_7)) {
@@ -10296,34 +10405,34 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_6};
     __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 377, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 421, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_windage, __pyx_t_4) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_windage, __pyx_t_4) < 0) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":378
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":422
  *         drop_adj=Angular.Radian(drop_adjustment - (look_angle if range_vector.x else 0)),
  *         windage=Distance.Foot(windage),
  *         windage_adj=Angular.Radian(windage_adjustment),             # <<<<<<<<<<<<<<
  *         look_distance= Distance.Foot(range_vector.x / cos(look_angle)),
  *         angle=Angular.Radian(trajectory_angle),
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Angular); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 378, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Angular); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 422, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_Radian); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 378, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_Radian); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 422, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_windage_adjustment); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 378, __pyx_L1_error)
+  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_windage_adjustment); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 422, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_7 = NULL;
   __pyx_t_8 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_7)) {
@@ -10336,39 +10445,34 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_5};
     __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 378, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 422, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_windage_adj, __pyx_t_4) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_windage_adj, __pyx_t_4) < 0) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":379
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":423
  *         windage=Distance.Foot(windage),
  *         windage_adj=Angular.Radian(windage_adjustment),
  *         look_distance= Distance.Foot(range_vector.x / cos(look_angle)),             # <<<<<<<<<<<<<<
  *         angle=Angular.Radian(trajectory_angle),
  *         density_factor = density_factor-1,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Distance); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 379, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Distance); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 423, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_Foot); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 379, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_Foot); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 423, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_1 = cos(__pyx_v_look_angle);
-  if (unlikely(__pyx_t_1 == 0)) {
-    PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(0, 379, __pyx_L1_error)
-  }
-  __pyx_t_6 = PyFloat_FromDouble((__pyx_v_range_vector->x / __pyx_t_1)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 379, __pyx_L1_error)
+  __pyx_t_6 = PyFloat_FromDouble((__pyx_v_range_vector->x / cos(__pyx_v_look_angle))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 423, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = NULL;
   __pyx_t_8 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_7)) {
@@ -10381,34 +10485,34 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_6};
     __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 379, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 423, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_look_distance, __pyx_t_4) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_look_distance, __pyx_t_4) < 0) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":380
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":424
  *         windage_adj=Angular.Radian(windage_adjustment),
  *         look_distance= Distance.Foot(range_vector.x / cos(look_angle)),
  *         angle=Angular.Radian(trajectory_angle),             # <<<<<<<<<<<<<<
  *         density_factor = density_factor-1,
  *         drag = drag,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Angular); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 380, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Angular); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_Radian); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 380, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_Radian); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_trajectory_angle); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 380, __pyx_L1_error)
+  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_trajectory_angle); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_7 = NULL;
   __pyx_t_8 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_7)) {
@@ -10421,59 +10525,59 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_5};
     __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 380, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 424, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_angle, __pyx_t_4) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_angle, __pyx_t_4) < 0) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":381
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":425
  *         look_distance= Distance.Foot(range_vector.x / cos(look_angle)),
  *         angle=Angular.Radian(trajectory_angle),
  *         density_factor = density_factor-1,             # <<<<<<<<<<<<<<
  *         drag = drag,
  *         energy=Energy.FootPound(calculate_energy(weight, velocity)),
  */
-  __pyx_t_4 = PyFloat_FromDouble((__pyx_v_density_factor - 1.0)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 381, __pyx_L1_error)
+  __pyx_t_4 = PyFloat_FromDouble((__pyx_v_density_factor - 1.0)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 425, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_density_factor, __pyx_t_4) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_density_factor, __pyx_t_4) < 0) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":382
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":426
  *         angle=Angular.Radian(trajectory_angle),
  *         density_factor = density_factor-1,
  *         drag = drag,             # <<<<<<<<<<<<<<
  *         energy=Energy.FootPound(calculate_energy(weight, velocity)),
  *         ogw=Weight.Pound(calculate_ogv(weight, velocity)),
  */
-  __pyx_t_4 = PyFloat_FromDouble(__pyx_v_drag); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 382, __pyx_L1_error)
+  __pyx_t_4 = PyFloat_FromDouble(__pyx_v_drag); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 426, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_drag, __pyx_t_4) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_drag, __pyx_t_4) < 0) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":383
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":427
  *         density_factor = density_factor-1,
  *         drag = drag,
  *         energy=Energy.FootPound(calculate_energy(weight, velocity)),             # <<<<<<<<<<<<<<
  *         ogw=Weight.Pound(calculate_ogv(weight, velocity)),
  *         flag=flag
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Energy); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 383, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Energy); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_FootPound); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 383, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_FootPound); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_1 = __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_calculate_energy(__pyx_v_weight, __pyx_v_velocity); if (unlikely(__pyx_t_1 == ((double)-1) && PyErr_Occurred())) __PYX_ERR(0, 383, __pyx_L1_error)
-  __pyx_t_6 = PyFloat_FromDouble(__pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 383, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_calculate_energy(__pyx_v_weight, __pyx_v_velocity); if (unlikely(__pyx_t_1 == ((double)-1) && PyErr_Occurred())) __PYX_ERR(0, 427, __pyx_L1_error)
+  __pyx_t_6 = PyFloat_FromDouble(__pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = NULL;
   __pyx_t_8 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_7)) {
@@ -10486,35 +10590,35 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_6};
     __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 383, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 427, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_energy, __pyx_t_4) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_energy, __pyx_t_4) < 0) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":384
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":428
  *         drag = drag,
  *         energy=Energy.FootPound(calculate_energy(weight, velocity)),
  *         ogw=Weight.Pound(calculate_ogv(weight, velocity)),             # <<<<<<<<<<<<<<
  *         flag=flag
  *     )
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Weight); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 384, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Weight); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 428, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_Pound); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 384, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_Pound); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 428, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_1 = __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_calculate_ogv(__pyx_v_weight, __pyx_v_velocity); if (unlikely(__pyx_t_1 == ((double)-1) && PyErr_Occurred())) __PYX_ERR(0, 384, __pyx_L1_error)
-  __pyx_t_5 = PyFloat_FromDouble(__pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 384, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_calculate_ogv(__pyx_v_weight, __pyx_v_velocity); if (unlikely(__pyx_t_1 == ((double)-1) && PyErr_Occurred())) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_5 = PyFloat_FromDouble(__pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 428, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_7 = NULL;
   __pyx_t_8 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_7)) {
@@ -10527,46 +10631,46 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_5};
     __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 384, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 428, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_ogw, __pyx_t_4) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_ogw, __pyx_t_4) < 0) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":385
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":429
  *         energy=Energy.FootPound(calculate_energy(weight, velocity)),
  *         ogw=Weight.Pound(calculate_ogv(weight, velocity)),
  *         flag=flag             # <<<<<<<<<<<<<<
  *     )
  * 
  */
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_flag, __pyx_v_flag) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_flag, __pyx_v_flag) < 0) __PYX_ERR(0, 414, __pyx_L1_error)
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":369
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":413
  *         double trajectory_angle = atan(velocity_vector.y / velocity_vector.x)
  * 
  *     return TrajectoryData(             # <<<<<<<<<<<<<<
  *         time=time,
  *         distance=Distance.Foot(range_vector.x),
  */
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 369, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 413, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":360
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":404
  *     return Vector(range_component, 0., cross_component)
  * 
  * cdef create_trajectory_row(double time, Vector range_vector, Vector velocity_vector,             # <<<<<<<<<<<<<<
  *                            double velocity, double mach, double spin_drift, double look_angle,
  *                            double density_factor, double drag, double weight, object flag):
  */
 
@@ -10582,147 +10686,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":389
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":433
  * 
  * @cython.cdivision(True)
  * cdef double get_correction(double distance, double offset):             # <<<<<<<<<<<<<<
  *     if distance != 0:
  *         return atan(offset / distance)
  */
 
 static double __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_get_correction(double __pyx_v_distance, double __pyx_v_offset) {
   double __pyx_r;
   int __pyx_t_1;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":390
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":434
  * @cython.cdivision(True)
  * cdef double get_correction(double distance, double offset):
  *     if distance != 0:             # <<<<<<<<<<<<<<
  *         return atan(offset / distance)
  *     return 0  # better None
  */
   __pyx_t_1 = (__pyx_v_distance != 0.0);
   if (__pyx_t_1) {
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":391
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":435
  * cdef double get_correction(double distance, double offset):
  *     if distance != 0:
  *         return atan(offset / distance)             # <<<<<<<<<<<<<<
  *     return 0  # better None
  * 
  */
     __pyx_r = atan((__pyx_v_offset / __pyx_v_distance));
     goto __pyx_L0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":390
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":434
  * @cython.cdivision(True)
  * cdef double get_correction(double distance, double offset):
  *     if distance != 0:             # <<<<<<<<<<<<<<
  *         return atan(offset / distance)
  *     return 0  # better None
  */
   }
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":392
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":436
  *     if distance != 0:
  *         return atan(offset / distance)
  *     return 0  # better None             # <<<<<<<<<<<<<<
  * 
- * cdef double calculate_energy(double bullet_weight, double velocity):
+ * @cython.cdivision(True)
  */
   __pyx_r = 0.0;
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":389
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":433
  * 
  * @cython.cdivision(True)
  * cdef double get_correction(double distance, double offset):             # <<<<<<<<<<<<<<
  *     if distance != 0:
  *         return atan(offset / distance)
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":394
- *     return 0  # better None
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":439
+ * 
+ * @cython.cdivision(True)
+ * cdef double get_calc_step(double step = 0):             # <<<<<<<<<<<<<<
+ *     cdef double preferred_step = _globalMaxCalcStepSize >> Distance.Foot
+ *     # cdef double defined_max = 0.5  # const will be better optimized with cython
+ */
+
+static double __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_get_calc_step(struct __pyx_opt_args_21py_ballisticcalc_exts_15trajectory_calc_get_calc_step *__pyx_optional_args) {
+  double __pyx_v_step = ((double)0.0);
+  double __pyx_v_preferred_step;
+  double __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  double __pyx_t_3;
+  int __pyx_t_4;
+  double __pyx_t_5;
+  double __pyx_t_6;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("get_calc_step", 1);
+  if (__pyx_optional_args) {
+    if (__pyx_optional_args->__pyx_n > 0) {
+      __pyx_v_step = __pyx_optional_args->step;
+    }
+  }
+
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":440
+ * @cython.cdivision(True)
+ * cdef double get_calc_step(double step = 0):
+ *     cdef double preferred_step = _globalMaxCalcStepSize >> Distance.Foot             # <<<<<<<<<<<<<<
+ *     # cdef double defined_max = 0.5  # const will be better optimized with cython
+ *     if step == 0:
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Distance); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 440, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Foot); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 440, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = PyNumber_Rshift(__pyx_v_21py_ballisticcalc_exts_15trajectory_calc__globalMaxCalcStepSize, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 440, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_3 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_3 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 440, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v_preferred_step = __pyx_t_3;
+
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":442
+ *     cdef double preferred_step = _globalMaxCalcStepSize >> Distance.Foot
+ *     # cdef double defined_max = 0.5  # const will be better optimized with cython
+ *     if step == 0:             # <<<<<<<<<<<<<<
+ *         return preferred_step / 2.0
+ *     return min(step, preferred_step) / 2.0
+ */
+  __pyx_t_4 = (__pyx_v_step == 0.0);
+  if (__pyx_t_4) {
+
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":443
+ *     # cdef double defined_max = 0.5  # const will be better optimized with cython
+ *     if step == 0:
+ *         return preferred_step / 2.0             # <<<<<<<<<<<<<<
+ *     return min(step, preferred_step) / 2.0
+ * 
+ */
+    __pyx_r = (__pyx_v_preferred_step / 2.0);
+    goto __pyx_L0;
+
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":442
+ *     cdef double preferred_step = _globalMaxCalcStepSize >> Distance.Foot
+ *     # cdef double defined_max = 0.5  # const will be better optimized with cython
+ *     if step == 0:             # <<<<<<<<<<<<<<
+ *         return preferred_step / 2.0
+ *     return min(step, preferred_step) / 2.0
+ */
+  }
+
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":444
+ *     if step == 0:
+ *         return preferred_step / 2.0
+ *     return min(step, preferred_step) / 2.0             # <<<<<<<<<<<<<<
+ * 
+ * cdef double calculate_energy(double bullet_weight, double velocity):
+ */
+  __pyx_t_3 = __pyx_v_preferred_step;
+  __pyx_t_5 = __pyx_v_step;
+  __pyx_t_4 = (__pyx_t_3 < __pyx_t_5);
+  if (__pyx_t_4) {
+    __pyx_t_6 = __pyx_t_3;
+  } else {
+    __pyx_t_6 = __pyx_t_5;
+  }
+  __pyx_r = (__pyx_t_6 / 2.0);
+  goto __pyx_L0;
+
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":439
+ * 
+ * @cython.cdivision(True)
+ * cdef double get_calc_step(double step = 0):             # <<<<<<<<<<<<<<
+ *     cdef double preferred_step = _globalMaxCalcStepSize >> Distance.Foot
+ *     # cdef double defined_max = 0.5  # const will be better optimized with cython
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_AddTraceback("py_ballisticcalc_exts.trajectory_calc.get_calc_step", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":446
+ *     return min(step, preferred_step) / 2.0
  * 
  * cdef double calculate_energy(double bullet_weight, double velocity):             # <<<<<<<<<<<<<<
  *     return bullet_weight * pow(velocity, 2) / 450400
  * 
  */
 
 static double __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_calculate_energy(double __pyx_v_bullet_weight, double __pyx_v_velocity) {
   double __pyx_r;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":395
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":447
  * 
  * cdef double calculate_energy(double bullet_weight, double velocity):
  *     return bullet_weight * pow(velocity, 2) / 450400             # <<<<<<<<<<<<<<
  * 
  * cdef double calculate_ogv(double bullet_weight, double velocity):
  */
   __pyx_r = ((__pyx_v_bullet_weight * pow(__pyx_v_velocity, 2.0)) / 450400.0);
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":394
- *     return 0  # better None
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":446
+ *     return min(step, preferred_step) / 2.0
  * 
  * cdef double calculate_energy(double bullet_weight, double velocity):             # <<<<<<<<<<<<<<
  *     return bullet_weight * pow(velocity, 2) / 450400
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":397
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":449
  *     return bullet_weight * pow(velocity, 2) / 450400
  * 
  * cdef double calculate_ogv(double bullet_weight, double velocity):             # <<<<<<<<<<<<<<
  *     return pow(bullet_weight, 2) * pow(velocity, 3) * 1.5e-12
  * 
  */
 
 static double __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_calculate_ogv(double __pyx_v_bullet_weight, double __pyx_v_velocity) {
   double __pyx_r;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":398
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":450
  * 
  * cdef double calculate_ogv(double bullet_weight, double velocity):
  *     return pow(bullet_weight, 2) * pow(velocity, 3) * 1.5e-12             # <<<<<<<<<<<<<<
  * 
  * cdef list calculate_curve(list data_points):
  */
   __pyx_r = ((pow(__pyx_v_bullet_weight, 2.0) * pow(__pyx_v_velocity, 3.0)) * 1.5e-12);
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":397
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":449
  *     return bullet_weight * pow(velocity, 2) / 450400
  * 
  * cdef double calculate_ogv(double bullet_weight, double velocity):             # <<<<<<<<<<<<<<
  *     return pow(bullet_weight, 2) * pow(velocity, 3) * 1.5e-12
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":400
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":452
  *     return pow(bullet_weight, 2) * pow(velocity, 3) * 1.5e-12
  * 
  * cdef list calculate_curve(list data_points):             # <<<<<<<<<<<<<<
  *     cdef double rate, x1, x2, x3, y1, y2, y3, a, b, c
  *     cdef list curve = []
  */
 
@@ -10735,641 +10953,533 @@
   double __pyx_v_y2;
   double __pyx_v_y3;
   double __pyx_v_a;
   double __pyx_v_b;
   double __pyx_v_c;
   PyObject *__pyx_v_curve = 0;
   struct __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CurvePoint __pyx_v_curve_point;
+  int __pyx_v_i;
   int __pyx_v_num_points;
   int __pyx_v_len_data_points;
   int __pyx_v_len_data_range;
-  PyObject *__pyx_v_i = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   double __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   Py_ssize_t __pyx_t_7;
-  PyObject *(*__pyx_t_8)(PyObject *);
-  double __pyx_t_9;
-  struct __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CurvePoint __pyx_t_10;
-  int __pyx_t_11;
-  long __pyx_t_12;
+  int __pyx_t_8;
+  int __pyx_t_9;
+  int __pyx_t_10;
+  long __pyx_t_11;
+  struct __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CurvePoint __pyx_t_12;
+  int __pyx_t_13;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("calculate_curve", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":402
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":454
  * cdef list calculate_curve(list data_points):
  *     cdef double rate, x1, x2, x3, y1, y2, y3, a, b, c
  *     cdef list curve = []             # <<<<<<<<<<<<<<
  *     cdef CurvePoint curve_point
- *     cdef int num_points, len_data_points, len_data_range
+ *     cdef int i, num_points, len_data_points, len_data_range
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 402, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 454, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_curve = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":406
- *     cdef int num_points, len_data_points, len_data_range
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":458
+ *     cdef int i, num_points, len_data_points, len_data_range
  * 
  *     rate = (data_points[1].CD - data_points[0].CD) / (data_points[1].Mach - data_points[0].Mach)             # <<<<<<<<<<<<<<
  *     curve = [CurvePoint(0, rate, data_points[0].CD - data_points[0].Mach * rate)]
  *     len_data_points = int(len(data_points))
  */
   if (unlikely(__pyx_v_data_points == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 406, __pyx_L1_error)
+    __PYX_ERR(0, 458, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_data_points, 1, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_data_points, 1, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 458, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_CD); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_CD); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 458, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_v_data_points == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 406, __pyx_L1_error)
+    __PYX_ERR(0, 458, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_data_points, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_data_points, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 458, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_CD); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_CD); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 458, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Subtract(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Subtract(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 458, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(__pyx_v_data_points == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 406, __pyx_L1_error)
+    __PYX_ERR(0, 458, __pyx_L1_error)
   }
-  __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_data_points, 1, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_data_points, 1, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 458, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Mach); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Mach); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 458, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(__pyx_v_data_points == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 406, __pyx_L1_error)
+    __PYX_ERR(0, 458, __pyx_L1_error)
   }
-  __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_data_points, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_data_points, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 458, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Mach); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Mach); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 458, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyNumber_Subtract(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Subtract(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 458, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyNumber_Divide(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyNumber_Divide(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 458, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 458, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_rate = __pyx_t_5;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":407
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":459
  * 
  *     rate = (data_points[1].CD - data_points[0].CD) / (data_points[1].Mach - data_points[0].Mach)
  *     curve = [CurvePoint(0, rate, data_points[0].CD - data_points[0].Mach * rate)]             # <<<<<<<<<<<<<<
  *     len_data_points = int(len(data_points))
  *     len_data_range = len_data_points - 1
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 407, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 459, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_a, __pyx_float_0_0) < 0) __PYX_ERR(0, 407, __pyx_L1_error)
-  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_rate); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 407, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_a, __pyx_float_0_0) < 0) __PYX_ERR(0, 459, __pyx_L1_error)
+  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_rate); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 459, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_b, __pyx_t_3) < 0) __PYX_ERR(0, 407, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_b, __pyx_t_3) < 0) __PYX_ERR(0, 459, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(__pyx_v_data_points == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 407, __pyx_L1_error)
+    __PYX_ERR(0, 459, __pyx_L1_error)
   }
-  __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_data_points, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 407, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_data_points, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 459, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_CD); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 407, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_CD); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 459, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(__pyx_v_data_points == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 407, __pyx_L1_error)
+    __PYX_ERR(0, 459, __pyx_L1_error)
   }
-  __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_data_points, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 407, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_data_points, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 459, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Mach); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 407, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Mach); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 459, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_rate); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 407, __pyx_L1_error)
+  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_rate); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 459, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = PyNumber_Multiply(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 407, __pyx_L1_error)
+  __pyx_t_6 = PyNumber_Multiply(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 459, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyNumber_Subtract(__pyx_t_1, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 407, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Subtract(__pyx_t_1, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 459, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 407, __pyx_L1_error)
+  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 459, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyFloat_FromDouble(__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 407, __pyx_L1_error)
+  __pyx_t_3 = PyFloat_FromDouble(__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 459, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_c, __pyx_t_3) < 0) __PYX_ERR(0, 407, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_c, __pyx_t_3) < 0) __PYX_ERR(0, 459, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 407, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 459, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_t_4)) __PYX_ERR(0, 407, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_t_4)) __PYX_ERR(0, 459, __pyx_L1_error);
   __pyx_t_4 = 0;
   __Pyx_DECREF_SET(__pyx_v_curve, ((PyObject*)__pyx_t_3));
   __pyx_t_3 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":408
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":460
  *     rate = (data_points[1].CD - data_points[0].CD) / (data_points[1].Mach - data_points[0].Mach)
  *     curve = [CurvePoint(0, rate, data_points[0].CD - data_points[0].Mach * rate)]
  *     len_data_points = int(len(data_points))             # <<<<<<<<<<<<<<
  *     len_data_range = len_data_points - 1
  * 
  */
   if (unlikely(__pyx_v_data_points == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 408, __pyx_L1_error)
+    __PYX_ERR(0, 460, __pyx_L1_error)
   }
-  __pyx_t_7 = __Pyx_PyList_GET_SIZE(__pyx_v_data_points); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 408, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyList_GET_SIZE(__pyx_v_data_points); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 460, __pyx_L1_error)
   __pyx_v_len_data_points = ((int)__pyx_t_7);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":409
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":461
  *     curve = [CurvePoint(0, rate, data_points[0].CD - data_points[0].Mach * rate)]
  *     len_data_points = int(len(data_points))
  *     len_data_range = len_data_points - 1             # <<<<<<<<<<<<<<
  * 
  *     for i in range(1, len_data_range):
  */
   __pyx_v_len_data_range = (__pyx_v_len_data_points - 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":411
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":463
  *     len_data_range = len_data_points - 1
  * 
  *     for i in range(1, len_data_range):             # <<<<<<<<<<<<<<
  *         x1 = data_points[i - 1].Mach
  *         x2 = data_points[i].Mach
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_len_data_range); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 411, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 411, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_INCREF(__pyx_int_1);
-  __Pyx_GIVEREF(__pyx_int_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_1)) __PYX_ERR(0, 411, __pyx_L1_error);
-  __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_3)) __PYX_ERR(0, 411, __pyx_L1_error);
-  __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_range, __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 411, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (likely(PyList_CheckExact(__pyx_t_3)) || PyTuple_CheckExact(__pyx_t_3)) {
-    __pyx_t_4 = __pyx_t_3; __Pyx_INCREF(__pyx_t_4);
-    __pyx_t_7 = 0;
-    __pyx_t_8 = NULL;
-  } else {
-    __pyx_t_7 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 411, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_8 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 411, __pyx_L1_error)
-  }
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  for (;;) {
-    if (likely(!__pyx_t_8)) {
-      if (likely(PyList_CheckExact(__pyx_t_4))) {
-        {
-          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_4);
-          #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 411, __pyx_L1_error)
-          #endif
-          if (__pyx_t_7 >= __pyx_temp) break;
-        }
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_7); __Pyx_INCREF(__pyx_t_3); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 411, __pyx_L1_error)
-        #else
-        __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 411, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        #endif
-      } else {
-        {
-          Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_4);
-          #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 411, __pyx_L1_error)
-          #endif
-          if (__pyx_t_7 >= __pyx_temp) break;
-        }
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_7); __Pyx_INCREF(__pyx_t_3); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 411, __pyx_L1_error)
-        #else
-        __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 411, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        #endif
-      }
-    } else {
-      __pyx_t_3 = __pyx_t_8(__pyx_t_4);
-      if (unlikely(!__pyx_t_3)) {
-        PyObject* exc_type = PyErr_Occurred();
-        if (exc_type) {
-          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 411, __pyx_L1_error)
-        }
-        break;
-      }
-      __Pyx_GOTREF(__pyx_t_3);
-    }
-    __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_3);
-    __pyx_t_3 = 0;
+  __pyx_t_8 = __pyx_v_len_data_range;
+  __pyx_t_9 = __pyx_t_8;
+  for (__pyx_t_10 = 1; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
+    __pyx_v_i = __pyx_t_10;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":412
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":464
  * 
  *     for i in range(1, len_data_range):
  *         x1 = data_points[i - 1].Mach             # <<<<<<<<<<<<<<
  *         x2 = data_points[i].Mach
  *         x3 = data_points[i + 1].Mach
  */
     if (unlikely(__pyx_v_data_points == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 412, __pyx_L1_error)
+      __PYX_ERR(0, 464, __pyx_L1_error)
     }
-    __pyx_t_3 = __Pyx_PyInt_SubtractObjC(__pyx_v_i, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 412, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_v_data_points, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 412, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_Mach); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 412, __pyx_L1_error)
+    __pyx_t_11 = (__pyx_v_i - 1);
+    __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_data_points, __pyx_t_11, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 464, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 412, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Mach); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 464, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 464, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_x1 = __pyx_t_5;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":413
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":465
  *     for i in range(1, len_data_range):
  *         x1 = data_points[i - 1].Mach
  *         x2 = data_points[i].Mach             # <<<<<<<<<<<<<<
  *         x3 = data_points[i + 1].Mach
  *         y1 = data_points[i - 1].CD
  */
     if (unlikely(__pyx_v_data_points == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 413, __pyx_L1_error)
+      __PYX_ERR(0, 465, __pyx_L1_error)
     }
-    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_data_points, __pyx_v_i); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 413, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_GetItemInt_List(__pyx_v_data_points, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 465, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_Mach); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 465, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Mach); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 413, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 465, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_6); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 413, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_v_x2 = __pyx_t_5;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":414
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":466
  *         x1 = data_points[i - 1].Mach
  *         x2 = data_points[i].Mach
  *         x3 = data_points[i + 1].Mach             # <<<<<<<<<<<<<<
  *         y1 = data_points[i - 1].CD
  *         y2 = data_points[i].CD
  */
     if (unlikely(__pyx_v_data_points == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 414, __pyx_L1_error)
+      __PYX_ERR(0, 466, __pyx_L1_error)
     }
-    __pyx_t_6 = __Pyx_PyInt_AddObjC(__pyx_v_i, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 414, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_data_points, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 414, __pyx_L1_error)
+    __pyx_t_11 = (__pyx_v_i + 1);
+    __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_data_points, __pyx_t_11, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 466, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Mach); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 414, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Mach); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 466, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_6); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 414, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 466, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_x3 = __pyx_t_5;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":415
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":467
  *         x2 = data_points[i].Mach
  *         x3 = data_points[i + 1].Mach
  *         y1 = data_points[i - 1].CD             # <<<<<<<<<<<<<<
  *         y2 = data_points[i].CD
  *         y3 = data_points[i + 1].CD
  */
     if (unlikely(__pyx_v_data_points == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 415, __pyx_L1_error)
+      __PYX_ERR(0, 467, __pyx_L1_error)
     }
-    __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_v_i, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 415, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_data_points, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 415, __pyx_L1_error)
+    __pyx_t_11 = (__pyx_v_i - 1);
+    __pyx_t_4 = __Pyx_GetItemInt_List(__pyx_v_data_points, __pyx_t_11, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 467, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_CD); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 467, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_CD); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 415, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 467, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_6); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 415, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_v_y1 = __pyx_t_5;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":416
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":468
  *         x3 = data_points[i + 1].Mach
  *         y1 = data_points[i - 1].CD
  *         y2 = data_points[i].CD             # <<<<<<<<<<<<<<
  *         y3 = data_points[i + 1].CD
  *         a = ((y3 - y1) * (x2 - x1) - (y2 - y1) * (x3 - x1)) / (
  */
     if (unlikely(__pyx_v_data_points == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 416, __pyx_L1_error)
+      __PYX_ERR(0, 468, __pyx_L1_error)
     }
-    __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_v_data_points, __pyx_v_i); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 416, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_CD); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 416, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_data_points, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 468, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 416, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_CD); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 468, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 468, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_y2 = __pyx_t_5;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":417
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":469
  *         y1 = data_points[i - 1].CD
  *         y2 = data_points[i].CD
  *         y3 = data_points[i + 1].CD             # <<<<<<<<<<<<<<
  *         a = ((y3 - y1) * (x2 - x1) - (y2 - y1) * (x3 - x1)) / (
  *                 (x3 * x3 - x1 * x1) * (x2 - x1) - (x2 * x2 - x1 * x1) * (x3 - x1))
  */
     if (unlikely(__pyx_v_data_points == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 417, __pyx_L1_error)
+      __PYX_ERR(0, 469, __pyx_L1_error)
     }
-    __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_v_i, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 417, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_v_data_points, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 417, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_CD); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 417, __pyx_L1_error)
+    __pyx_t_11 = (__pyx_v_i + 1);
+    __pyx_t_4 = __Pyx_GetItemInt_List(__pyx_v_data_points, __pyx_t_11, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 469, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_CD); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 469, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 417, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 469, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_y3 = __pyx_t_5;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":418
- *         y2 = data_points[i].CD
- *         y3 = data_points[i + 1].CD
- *         a = ((y3 - y1) * (x2 - x1) - (y2 - y1) * (x3 - x1)) / (             # <<<<<<<<<<<<<<
- *                 (x3 * x3 - x1 * x1) * (x2 - x1) - (x2 * x2 - x1 * x1) * (x3 - x1))
- *         b = (y2 - y1 - a * (x2 * x2 - x1 * x1)) / (x2 - x1)
- */
-    __pyx_t_5 = (((__pyx_v_y3 - __pyx_v_y1) * (__pyx_v_x2 - __pyx_v_x1)) - ((__pyx_v_y2 - __pyx_v_y1) * (__pyx_v_x3 - __pyx_v_x1)));
-
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":419
- *         y3 = data_points[i + 1].CD
- *         a = ((y3 - y1) * (x2 - x1) - (y2 - y1) * (x3 - x1)) / (
- *                 (x3 * x3 - x1 * x1) * (x2 - x1) - (x2 * x2 - x1 * x1) * (x3 - x1))             # <<<<<<<<<<<<<<
- *         b = (y2 - y1 - a * (x2 * x2 - x1 * x1)) / (x2 - x1)
- *         c = y1 - (a * x1 * x1 + b * x1)
- */
-    __pyx_t_9 = ((((__pyx_v_x3 * __pyx_v_x3) - (__pyx_v_x1 * __pyx_v_x1)) * (__pyx_v_x2 - __pyx_v_x1)) - (((__pyx_v_x2 * __pyx_v_x2) - (__pyx_v_x1 * __pyx_v_x1)) * (__pyx_v_x3 - __pyx_v_x1)));
-
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":418
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":470
  *         y2 = data_points[i].CD
  *         y3 = data_points[i + 1].CD
  *         a = ((y3 - y1) * (x2 - x1) - (y2 - y1) * (x3 - x1)) / (             # <<<<<<<<<<<<<<
  *                 (x3 * x3 - x1 * x1) * (x2 - x1) - (x2 * x2 - x1 * x1) * (x3 - x1))
  *         b = (y2 - y1 - a * (x2 * x2 - x1 * x1)) / (x2 - x1)
  */
-    if (unlikely(__pyx_t_9 == 0)) {
-      PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(0, 418, __pyx_L1_error)
-    }
-    __pyx_v_a = (__pyx_t_5 / __pyx_t_9);
+    __pyx_v_a = ((((__pyx_v_y3 - __pyx_v_y1) * (__pyx_v_x2 - __pyx_v_x1)) - ((__pyx_v_y2 - __pyx_v_y1) * (__pyx_v_x3 - __pyx_v_x1))) / ((((__pyx_v_x3 * __pyx_v_x3) - (__pyx_v_x1 * __pyx_v_x1)) * (__pyx_v_x2 - __pyx_v_x1)) - (((__pyx_v_x2 * __pyx_v_x2) - (__pyx_v_x1 * __pyx_v_x1)) * (__pyx_v_x3 - __pyx_v_x1))));
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":420
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":472
  *         a = ((y3 - y1) * (x2 - x1) - (y2 - y1) * (x3 - x1)) / (
  *                 (x3 * x3 - x1 * x1) * (x2 - x1) - (x2 * x2 - x1 * x1) * (x3 - x1))
  *         b = (y2 - y1 - a * (x2 * x2 - x1 * x1)) / (x2 - x1)             # <<<<<<<<<<<<<<
  *         c = y1 - (a * x1 * x1 + b * x1)
  *         curve_point = CurvePoint(a, b, c)
  */
-    __pyx_t_9 = ((__pyx_v_y2 - __pyx_v_y1) - (__pyx_v_a * ((__pyx_v_x2 * __pyx_v_x2) - (__pyx_v_x1 * __pyx_v_x1))));
-    __pyx_t_5 = (__pyx_v_x2 - __pyx_v_x1);
-    if (unlikely(__pyx_t_5 == 0)) {
-      PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(0, 420, __pyx_L1_error)
-    }
-    __pyx_v_b = (__pyx_t_9 / __pyx_t_5);
+    __pyx_v_b = (((__pyx_v_y2 - __pyx_v_y1) - (__pyx_v_a * ((__pyx_v_x2 * __pyx_v_x2) - (__pyx_v_x1 * __pyx_v_x1)))) / (__pyx_v_x2 - __pyx_v_x1));
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":421
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":473
  *                 (x3 * x3 - x1 * x1) * (x2 - x1) - (x2 * x2 - x1 * x1) * (x3 - x1))
  *         b = (y2 - y1 - a * (x2 * x2 - x1 * x1)) / (x2 - x1)
  *         c = y1 - (a * x1 * x1 + b * x1)             # <<<<<<<<<<<<<<
  *         curve_point = CurvePoint(a, b, c)
  *         curve.append(curve_point)
  */
     __pyx_v_c = (__pyx_v_y1 - (((__pyx_v_a * __pyx_v_x1) * __pyx_v_x1) + (__pyx_v_b * __pyx_v_x1)));
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":422
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":474
  *         b = (y2 - y1 - a * (x2 * x2 - x1 * x1)) / (x2 - x1)
  *         c = y1 - (a * x1 * x1 + b * x1)
  *         curve_point = CurvePoint(a, b, c)             # <<<<<<<<<<<<<<
  *         curve.append(curve_point)
  * 
  */
-    __pyx_t_10.a = __pyx_v_a;
-    __pyx_t_10.b = __pyx_v_b;
-    __pyx_t_10.c = __pyx_v_c;
-    __pyx_v_curve_point = __pyx_t_10;
+    __pyx_t_12.a = __pyx_v_a;
+    __pyx_t_12.b = __pyx_v_b;
+    __pyx_t_12.c = __pyx_v_c;
+    __pyx_v_curve_point = __pyx_t_12;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":423
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":475
  *         c = y1 - (a * x1 * x1 + b * x1)
  *         curve_point = CurvePoint(a, b, c)
  *         curve.append(curve_point)             # <<<<<<<<<<<<<<
  * 
  *     num_points = len_data_points
  */
-    __pyx_t_3 = __pyx_convert__to_py_struct____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CurvePoint(__pyx_v_curve_point); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 423, __pyx_L1_error)
+    __pyx_t_3 = __pyx_convert__to_py_struct____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CurvePoint(__pyx_v_curve_point); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 475, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_11 = __Pyx_PyList_Append(__pyx_v_curve, __pyx_t_3); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(0, 423, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyList_Append(__pyx_v_curve, __pyx_t_3); if (unlikely(__pyx_t_13 == ((int)-1))) __PYX_ERR(0, 475, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":411
- *     len_data_range = len_data_points - 1
- * 
- *     for i in range(1, len_data_range):             # <<<<<<<<<<<<<<
- *         x1 = data_points[i - 1].Mach
- *         x2 = data_points[i].Mach
- */
   }
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":425
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":477
  *         curve.append(curve_point)
  * 
  *     num_points = len_data_points             # <<<<<<<<<<<<<<
  *     rate = (data_points[num_points - 1].CD - data_points[num_points - 2].CD) / \
  *            (data_points[num_points - 1].Mach - data_points[num_points - 2].Mach)
  */
   __pyx_v_num_points = __pyx_v_len_data_points;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":426
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":478
  * 
  *     num_points = len_data_points
  *     rate = (data_points[num_points - 1].CD - data_points[num_points - 2].CD) / \             # <<<<<<<<<<<<<<
  *            (data_points[num_points - 1].Mach - data_points[num_points - 2].Mach)
  *     curve_point = CurvePoint(0, rate, data_points[num_points - 1].CD - data_points[num_points - 2].Mach * rate)
  */
   if (unlikely(__pyx_v_data_points == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 426, __pyx_L1_error)
+    __PYX_ERR(0, 478, __pyx_L1_error)
   }
-  __pyx_t_12 = (__pyx_v_num_points - 1);
-  __pyx_t_4 = __Pyx_GetItemInt_List(__pyx_v_data_points, __pyx_t_12, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 426, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_CD); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 426, __pyx_L1_error)
+  __pyx_t_11 = (__pyx_v_num_points - 1);
+  __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_data_points, __pyx_t_11, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 478, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_CD); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 478, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(__pyx_v_data_points == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 426, __pyx_L1_error)
+    __PYX_ERR(0, 478, __pyx_L1_error)
   }
-  __pyx_t_12 = (__pyx_v_num_points - 2);
-  __pyx_t_4 = __Pyx_GetItemInt_List(__pyx_v_data_points, __pyx_t_12, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 426, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_CD); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 426, __pyx_L1_error)
+  __pyx_t_11 = (__pyx_v_num_points - 2);
+  __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_data_points, __pyx_t_11, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 478, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_CD); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 478, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyNumber_Subtract(__pyx_t_3, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 426, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = PyNumber_Subtract(__pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 478, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":427
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":479
  *     num_points = len_data_points
  *     rate = (data_points[num_points - 1].CD - data_points[num_points - 2].CD) / \
  *            (data_points[num_points - 1].Mach - data_points[num_points - 2].Mach)             # <<<<<<<<<<<<<<
  *     curve_point = CurvePoint(0, rate, data_points[num_points - 1].CD - data_points[num_points - 2].Mach * rate)
  *     curve.append(curve_point)
  */
   if (unlikely(__pyx_v_data_points == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 427, __pyx_L1_error)
+    __PYX_ERR(0, 479, __pyx_L1_error)
   }
-  __pyx_t_12 = (__pyx_v_num_points - 1);
-  __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_data_points, __pyx_t_12, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __pyx_t_11 = (__pyx_v_num_points - 1);
+  __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_data_points, __pyx_t_11, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 479, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_Mach); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 427, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_Mach); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 479, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (unlikely(__pyx_v_data_points == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 427, __pyx_L1_error)
+    __PYX_ERR(0, 479, __pyx_L1_error)
   }
-  __pyx_t_12 = (__pyx_v_num_points - 2);
-  __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_data_points, __pyx_t_12, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __pyx_t_11 = (__pyx_v_num_points - 2);
+  __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_data_points, __pyx_t_11, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 479, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_Mach); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_Mach); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 479, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = PyNumber_Subtract(__pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __pyx_t_6 = PyNumber_Subtract(__pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 479, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":426
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":478
  * 
  *     num_points = len_data_points
  *     rate = (data_points[num_points - 1].CD - data_points[num_points - 2].CD) / \             # <<<<<<<<<<<<<<
  *            (data_points[num_points - 1].Mach - data_points[num_points - 2].Mach)
  *     curve_point = CurvePoint(0, rate, data_points[num_points - 1].CD - data_points[num_points - 2].Mach * rate)
  */
-  __pyx_t_1 = __Pyx_PyNumber_Divide(__pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 426, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyNumber_Divide(__pyx_t_3, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 478, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 426, __pyx_L1_error)
+  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 478, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_rate = __pyx_t_5;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":428
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":480
  *     rate = (data_points[num_points - 1].CD - data_points[num_points - 2].CD) / \
  *            (data_points[num_points - 1].Mach - data_points[num_points - 2].Mach)
  *     curve_point = CurvePoint(0, rate, data_points[num_points - 1].CD - data_points[num_points - 2].Mach * rate)             # <<<<<<<<<<<<<<
  *     curve.append(curve_point)
  *     return curve
  */
-  __pyx_t_10.a = 0.0;
-  __pyx_t_10.b = __pyx_v_rate;
+  __pyx_t_12.a = 0.0;
+  __pyx_t_12.b = __pyx_v_rate;
   if (unlikely(__pyx_v_data_points == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 428, __pyx_L1_error)
+    __PYX_ERR(0, 480, __pyx_L1_error)
   }
-  __pyx_t_12 = (__pyx_v_num_points - 1);
-  __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_data_points, __pyx_t_12, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_11 = (__pyx_v_num_points - 1);
+  __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_data_points, __pyx_t_11, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 480, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_CD); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_CD); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 480, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_v_data_points == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 428, __pyx_L1_error)
+    __PYX_ERR(0, 480, __pyx_L1_error)
   }
-  __pyx_t_12 = (__pyx_v_num_points - 2);
-  __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_data_points, __pyx_t_12, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_11 = (__pyx_v_num_points - 2);
+  __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_data_points, __pyx_t_11, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 480, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Mach); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 428, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Mach); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 480, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_rate); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_rate); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 480, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyNumber_Multiply(__pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 428, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = PyNumber_Multiply(__pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 480, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Subtract(__pyx_t_6, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Subtract(__pyx_t_6, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 480, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 428, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 480, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_10.c = __pyx_t_5;
-  __pyx_v_curve_point = __pyx_t_10;
+  __pyx_t_12.c = __pyx_t_5;
+  __pyx_v_curve_point = __pyx_t_12;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":429
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":481
  *            (data_points[num_points - 1].Mach - data_points[num_points - 2].Mach)
  *     curve_point = CurvePoint(0, rate, data_points[num_points - 1].CD - data_points[num_points - 2].Mach * rate)
  *     curve.append(curve_point)             # <<<<<<<<<<<<<<
  *     return curve
  * 
  */
-  __pyx_t_1 = __pyx_convert__to_py_struct____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CurvePoint(__pyx_v_curve_point); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 429, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert__to_py_struct____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CurvePoint(__pyx_v_curve_point); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 481, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_11 = __Pyx_PyList_Append(__pyx_v_curve, __pyx_t_1); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(0, 429, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_PyList_Append(__pyx_v_curve, __pyx_t_1); if (unlikely(__pyx_t_13 == ((int)-1))) __PYX_ERR(0, 481, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":430
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":482
  *     curve_point = CurvePoint(0, rate, data_points[num_points - 1].CD - data_points[num_points - 2].Mach * rate)
  *     curve.append(curve_point)
  *     return curve             # <<<<<<<<<<<<<<
  * 
  * cdef double calculate_by_curve(list data, list curve, double mach):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_curve);
   __pyx_r = __pyx_v_curve;
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":400
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":452
  *     return pow(bullet_weight, 2) * pow(velocity, 3) * 1.5e-12
  * 
  * cdef list calculate_curve(list data_points):             # <<<<<<<<<<<<<<
  *     cdef double rate, x1, x2, x3, y1, y2, y3, a, b, c
  *     cdef list curve = []
  */
 
@@ -11380,262 +11490,261 @@
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("py_ballisticcalc_exts.trajectory_calc.calculate_curve", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_curve);
-  __Pyx_XDECREF(__pyx_v_i);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":432
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":484
  *     return curve
  * 
  * cdef double calculate_by_curve(list data, list curve, double mach):             # <<<<<<<<<<<<<<
- *     cdef int num_points, mlo, mhi, mid
+ *     cdef int num_points, mlo, mhi, mid, m
  *     cdef CurvePoint curve_m
  */
 
 static double __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_calculate_by_curve(PyObject *__pyx_v_data, PyObject *__pyx_v_curve, double __pyx_v_mach) {
   int __pyx_v_num_points;
   int __pyx_v_mlo;
   int __pyx_v_mhi;
   int __pyx_v_mid;
-  struct __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CurvePoint __pyx_v_curve_m;
   int __pyx_v_m;
+  struct __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CurvePoint __pyx_v_curve_m;
   double __pyx_r;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   struct __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CurvePoint __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("calculate_by_curve", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":436
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":488
  *     cdef CurvePoint curve_m
  * 
  *     num_points = int(len(curve))             # <<<<<<<<<<<<<<
  *     mlo = 0
  *     mhi = num_points - 2
  */
   if (unlikely(__pyx_v_curve == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 436, __pyx_L1_error)
+    __PYX_ERR(0, 488, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_PyList_GET_SIZE(__pyx_v_curve); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 436, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyList_GET_SIZE(__pyx_v_curve); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 488, __pyx_L1_error)
   __pyx_v_num_points = ((int)__pyx_t_1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":437
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":489
  * 
  *     num_points = int(len(curve))
  *     mlo = 0             # <<<<<<<<<<<<<<
  *     mhi = num_points - 2
  * 
  */
   __pyx_v_mlo = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":438
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":490
  *     num_points = int(len(curve))
  *     mlo = 0
  *     mhi = num_points - 2             # <<<<<<<<<<<<<<
  * 
  *     while mhi - mlo > 1:
  */
   __pyx_v_mhi = (__pyx_v_num_points - 2);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":440
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":492
  *     mhi = num_points - 2
  * 
  *     while mhi - mlo > 1:             # <<<<<<<<<<<<<<
  *         mid = int(floor(mhi + mlo) / 2.0)
  *         if data[mid].Mach < mach:
  */
   while (1) {
     __pyx_t_2 = ((__pyx_v_mhi - __pyx_v_mlo) > 1);
     if (!__pyx_t_2) break;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":441
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":493
  * 
  *     while mhi - mlo > 1:
  *         mid = int(floor(mhi + mlo) / 2.0)             # <<<<<<<<<<<<<<
  *         if data[mid].Mach < mach:
  *             mlo = mid
  */
     __pyx_v_mid = ((int)(floor((__pyx_v_mhi + __pyx_v_mlo)) / 2.0));
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":442
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":494
  *     while mhi - mlo > 1:
  *         mid = int(floor(mhi + mlo) / 2.0)
  *         if data[mid].Mach < mach:             # <<<<<<<<<<<<<<
  *             mlo = mid
  *         else:
  */
     if (unlikely(__pyx_v_data == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 442, __pyx_L1_error)
+      __PYX_ERR(0, 494, __pyx_L1_error)
     }
-    __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_data, __pyx_v_mid, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 442, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_data, __pyx_v_mid, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 494, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Mach); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 442, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Mach); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 494, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyFloat_FromDouble(__pyx_v_mach); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 442, __pyx_L1_error)
+    __pyx_t_3 = PyFloat_FromDouble(__pyx_v_mach); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 494, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = PyObject_RichCompare(__pyx_t_4, __pyx_t_3, Py_LT); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 442, __pyx_L1_error)
+    __pyx_t_5 = PyObject_RichCompare(__pyx_t_4, __pyx_t_3, Py_LT); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 494, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 442, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 494, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     if (__pyx_t_2) {
 
-      /* "py_ballisticcalc_exts/trajectory_calc.pyx":443
+      /* "py_ballisticcalc_exts/trajectory_calc.pyx":495
  *         mid = int(floor(mhi + mlo) / 2.0)
  *         if data[mid].Mach < mach:
  *             mlo = mid             # <<<<<<<<<<<<<<
  *         else:
  *             mhi = mid
  */
       __pyx_v_mlo = __pyx_v_mid;
 
-      /* "py_ballisticcalc_exts/trajectory_calc.pyx":442
+      /* "py_ballisticcalc_exts/trajectory_calc.pyx":494
  *     while mhi - mlo > 1:
  *         mid = int(floor(mhi + mlo) / 2.0)
  *         if data[mid].Mach < mach:             # <<<<<<<<<<<<<<
  *             mlo = mid
  *         else:
  */
       goto __pyx_L5;
     }
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":445
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":497
  *             mlo = mid
  *         else:
  *             mhi = mid             # <<<<<<<<<<<<<<
  * 
  *     if data[mhi].Mach - mach > mach - data[mlo].Mach:
  */
     /*else*/ {
       __pyx_v_mhi = __pyx_v_mid;
     }
     __pyx_L5:;
   }
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":447
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":499
  *             mhi = mid
  * 
  *     if data[mhi].Mach - mach > mach - data[mlo].Mach:             # <<<<<<<<<<<<<<
  *         m = mlo
  *     else:
  */
   if (unlikely(__pyx_v_data == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 447, __pyx_L1_error)
+    __PYX_ERR(0, 499, __pyx_L1_error)
   }
-  __pyx_t_5 = __Pyx_GetItemInt_List(__pyx_v_data, __pyx_v_mhi, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 447, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_GetItemInt_List(__pyx_v_data, __pyx_v_mhi, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 499, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_Mach); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 447, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_Mach); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 499, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_mach); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 447, __pyx_L1_error)
+  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_mach); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 499, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = PyNumber_Subtract(__pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 447, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Subtract(__pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 499, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_mach); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 447, __pyx_L1_error)
+  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_mach); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 499, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (unlikely(__pyx_v_data == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 447, __pyx_L1_error)
+    __PYX_ERR(0, 499, __pyx_L1_error)
   }
-  __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_data, __pyx_v_mlo, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 447, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_data, __pyx_v_mlo, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 499, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Mach); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 447, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Mach); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 499, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyNumber_Subtract(__pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 447, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Subtract(__pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 499, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = PyObject_RichCompare(__pyx_t_4, __pyx_t_3, Py_GT); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 447, __pyx_L1_error)
+  __pyx_t_6 = PyObject_RichCompare(__pyx_t_4, __pyx_t_3, Py_GT); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 499, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 447, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 499, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (__pyx_t_2) {
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":448
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":500
  * 
  *     if data[mhi].Mach - mach > mach - data[mlo].Mach:
  *         m = mlo             # <<<<<<<<<<<<<<
  *     else:
  *         m = mhi
  */
     __pyx_v_m = __pyx_v_mlo;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":447
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":499
  *             mhi = mid
  * 
  *     if data[mhi].Mach - mach > mach - data[mlo].Mach:             # <<<<<<<<<<<<<<
  *         m = mlo
  *     else:
  */
     goto __pyx_L6;
   }
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":450
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":502
  *         m = mlo
  *     else:
  *         m = mhi             # <<<<<<<<<<<<<<
  *     curve_m = curve[m]
  *     return curve_m.c + mach * (curve_m.b + curve_m.a * mach)
  */
   /*else*/ {
     __pyx_v_m = __pyx_v_mhi;
   }
   __pyx_L6:;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":451
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":503
  *     else:
  *         m = mhi
  *     curve_m = curve[m]             # <<<<<<<<<<<<<<
  *     return curve_m.c + mach * (curve_m.b + curve_m.a * mach)
  */
   if (unlikely(__pyx_v_curve == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 451, __pyx_L1_error)
+    __PYX_ERR(0, 503, __pyx_L1_error)
   }
-  __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_curve, __pyx_v_m, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 451, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_curve, __pyx_v_m, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 503, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = __pyx_convert__from_py_struct____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CurvePoint(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 451, __pyx_L1_error)
+  __pyx_t_7 = __pyx_convert__from_py_struct____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CurvePoint(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 503, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_v_curve_m = __pyx_t_7;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":452
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":504
  *         m = mhi
  *     curve_m = curve[m]
  *     return curve_m.c + mach * (curve_m.b + curve_m.a * mach)             # <<<<<<<<<<<<<<
  */
   __pyx_r = (__pyx_v_curve_m.c + (__pyx_v_mach * (__pyx_v_curve_m.b + (__pyx_v_curve_m.a * __pyx_v_mach))));
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":432
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":484
  *     return curve
  * 
  * cdef double calculate_by_curve(list data, list curve, double mach):             # <<<<<<<<<<<<<<
- *     cdef int num_points, mlo, mhi, mid
+ *     cdef int num_points, mlo, mhi, mid, m
  *     cdef CurvePoint curve_m
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
@@ -11651,24 +11760,24 @@
 /* "(tree fragment)":1
  * def __pyx_unpickle_TrajectoryCalc(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_1__pyx_unpickle_TrajectoryCalc(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_11__pyx_unpickle_TrajectoryCalc(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_21py_ballisticcalc_exts_15trajectory_calc___pyx_unpickle_TrajectoryCalc, "__pyx_unpickle_TrajectoryCalc(__pyx_type, long __pyx_checksum, __pyx_state)");
-static PyMethodDef __pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_1__pyx_unpickle_TrajectoryCalc = {"__pyx_unpickle_TrajectoryCalc", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_1__pyx_unpickle_TrajectoryCalc, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_21py_ballisticcalc_exts_15trajectory_calc___pyx_unpickle_TrajectoryCalc};
-static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_1__pyx_unpickle_TrajectoryCalc(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_10__pyx_unpickle_TrajectoryCalc, "__pyx_unpickle_TrajectoryCalc(__pyx_type, long __pyx_checksum, __pyx_state)");
+static PyMethodDef __pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_11__pyx_unpickle_TrajectoryCalc = {"__pyx_unpickle_TrajectoryCalc", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_11__pyx_unpickle_TrajectoryCalc, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_10__pyx_unpickle_TrajectoryCalc};
+static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_11__pyx_unpickle_TrajectoryCalc(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v___pyx_type = 0;
@@ -11764,28 +11873,28 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("py_ballisticcalc_exts.trajectory_calc.__pyx_unpickle_TrajectoryCalc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_21py_ballisticcalc_exts_15trajectory_calc___pyx_unpickle_TrajectoryCalc(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_10__pyx_unpickle_TrajectoryCalc(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc___pyx_unpickle_TrajectoryCalc(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_10__pyx_unpickle_TrajectoryCalc(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
@@ -11801,15 +11910,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x1a1505e, 0xaee47ca, 0x4420ce0):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x1a1505e, 0xaee47ca, 0x4420ce0) = (_bc, _curve, _table_data, alt0, ammo, barrel_azimuth, barrel_elevation, calc_step, cant_cosine, cant_sine, diameter, gravity_vector, length, look_angle, muzzle_velocity, sight_height, stability_coefficient, twist, weight))" % __pyx_checksum
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__5, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__6, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x1a1505e, 0xaee47ca, 0x4420ce0):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
@@ -12301,119 +12410,17 @@
   #else
   {
     freefunc tp_free = (freefunc)PyType_GetSlot(Py_TYPE(o), Py_tp_free);
     if (tp_free) tp_free(o);
   }
   #endif
 }
-
-static CYTHON_INLINE PyObject *__pyx_nb_add_21py_ballisticcalc_exts_15trajectory_calc_Vector_maybe_call_slot(PyTypeObject* type, PyObject *left, PyObject *right ) {
-    binaryfunc slot;
-#if CYTHON_USE_TYPE_SLOTS || PY_MAJOR_VERSION < 3 || CYTHON_COMPILING_IN_PYPY
-    slot = type->tp_as_number ? type->tp_as_number->nb_add : NULL;
-#else
-    slot = (binaryfunc) PyType_GetSlot(type, Py_nb_add);
-#endif
-    return slot ? slot(left, right ) : __Pyx_NewRef(Py_NotImplemented);
-}
-static PyObject *__pyx_nb_add_21py_ballisticcalc_exts_15trajectory_calc_Vector(PyObject *left, PyObject *right ) {
-    int maybe_self_is_left, maybe_self_is_right = 0;
-    maybe_self_is_left = Py_TYPE(left) == Py_TYPE(right)
-#if CYTHON_USE_TYPE_SLOTS
-            || (Py_TYPE(left)->tp_as_number && Py_TYPE(left)->tp_as_number->nb_add == &__pyx_nb_add_21py_ballisticcalc_exts_15trajectory_calc_Vector)
-#endif
-            || __Pyx_TypeCheck(left, __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector);
-    if (maybe_self_is_left) {
-        PyObject *res;
-        res = __pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_6Vector_3__add__(left, right);
-        if (res != Py_NotImplemented) return res;
-        Py_DECREF(res);
-    }
-    maybe_self_is_right = Py_TYPE(left) == Py_TYPE(right)
-#if CYTHON_USE_TYPE_SLOTS
-            || (Py_TYPE(right)->tp_as_number && Py_TYPE(right)->tp_as_number->nb_add == &__pyx_nb_add_21py_ballisticcalc_exts_15trajectory_calc_Vector)
-#endif
-            || PyType_IsSubtype(Py_TYPE(right), __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector);
-    if (maybe_self_is_right) {
-        return __pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_6Vector_5__radd__(right, left);
-    }
-    return __Pyx_NewRef(Py_NotImplemented);
-}
-
-
-
-static CYTHON_INLINE PyObject *__pyx_nb_subtract_21py_ballisticcalc_exts_15trajectory_calc_Vector_maybe_call_slot(PyTypeObject* type, PyObject *left, PyObject *right ) {
-    binaryfunc slot;
-#if CYTHON_USE_TYPE_SLOTS || PY_MAJOR_VERSION < 3 || CYTHON_COMPILING_IN_PYPY
-    slot = type->tp_as_number ? type->tp_as_number->nb_subtract : NULL;
-#else
-    slot = (binaryfunc) PyType_GetSlot(type, Py_nb_subtract);
-#endif
-    return slot ? slot(left, right ) : __Pyx_NewRef(Py_NotImplemented);
-}
-static PyObject *__pyx_nb_subtract_21py_ballisticcalc_exts_15trajectory_calc_Vector(PyObject *left, PyObject *right ) {
-    int maybe_self_is_left, maybe_self_is_right = 0;
-    maybe_self_is_left = Py_TYPE(left) == Py_TYPE(right)
-#if CYTHON_USE_TYPE_SLOTS
-            || (Py_TYPE(left)->tp_as_number && Py_TYPE(left)->tp_as_number->nb_subtract == &__pyx_nb_subtract_21py_ballisticcalc_exts_15trajectory_calc_Vector)
-#endif
-            || __Pyx_TypeCheck(left, __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector);
-    if (maybe_self_is_left) {
-        PyObject *res;
-        res = __pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_6Vector_9__sub__(left, right);
-        if (res != Py_NotImplemented) return res;
-        Py_DECREF(res);
-    }
-    maybe_self_is_right = Py_TYPE(left) == Py_TYPE(right)
-#if CYTHON_USE_TYPE_SLOTS
-            || (Py_TYPE(right)->tp_as_number && Py_TYPE(right)->tp_as_number->nb_subtract == &__pyx_nb_subtract_21py_ballisticcalc_exts_15trajectory_calc_Vector)
-#endif
-            || PyType_IsSubtype(Py_TYPE(right), __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector);
-    if (maybe_self_is_right) {
-        return __pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_6Vector_11__rsub__(right, left);
-    }
-    return __Pyx_NewRef(Py_NotImplemented);
-}
-
-
-
-static CYTHON_INLINE PyObject *__pyx_nb_multiply_21py_ballisticcalc_exts_15trajectory_calc_Vector_maybe_call_slot(PyTypeObject* type, PyObject *left, PyObject *right ) {
-    binaryfunc slot;
-#if CYTHON_USE_TYPE_SLOTS || PY_MAJOR_VERSION < 3 || CYTHON_COMPILING_IN_PYPY
-    slot = type->tp_as_number ? type->tp_as_number->nb_multiply : NULL;
-#else
-    slot = (binaryfunc) PyType_GetSlot(type, Py_nb_multiply);
-#endif
-    return slot ? slot(left, right ) : __Pyx_NewRef(Py_NotImplemented);
-}
-static PyObject *__pyx_nb_multiply_21py_ballisticcalc_exts_15trajectory_calc_Vector(PyObject *left, PyObject *right ) {
-    int maybe_self_is_left, maybe_self_is_right = 0;
-    maybe_self_is_left = Py_TYPE(left) == Py_TYPE(right)
-#if CYTHON_USE_TYPE_SLOTS
-            || (Py_TYPE(left)->tp_as_number && Py_TYPE(left)->tp_as_number->nb_multiply == &__pyx_nb_multiply_21py_ballisticcalc_exts_15trajectory_calc_Vector)
-#endif
-            || __Pyx_TypeCheck(left, __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector);
-    if (maybe_self_is_left) {
-        PyObject *res;
-        res = __pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_6Vector_15__mul__(left, right);
-        if (res != Py_NotImplemented) return res;
-        Py_DECREF(res);
-    }
-    maybe_self_is_right = Py_TYPE(left) == Py_TYPE(right)
-#if CYTHON_USE_TYPE_SLOTS
-            || (Py_TYPE(right)->tp_as_number && Py_TYPE(right)->tp_as_number->nb_multiply == &__pyx_nb_multiply_21py_ballisticcalc_exts_15trajectory_calc_Vector)
-#endif
-            || PyType_IsSubtype(Py_TYPE(right), __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector);
-    if (maybe_self_is_right) {
-        return __pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_6Vector_17__rmul__(right, left);
-    }
-    return __Pyx_NewRef(Py_NotImplemented);
-}
-
-
+#define __pyx_nb_add_21py_ballisticcalc_exts_15trajectory_calc_Vector __pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_6Vector_3__add__
+#define __pyx_nb_subtract_21py_ballisticcalc_exts_15trajectory_calc_Vector __pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_6Vector_9__sub__
+#define __pyx_nb_multiply_21py_ballisticcalc_exts_15trajectory_calc_Vector __pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_6Vector_15__mul__
 
 static PyMethodDef __pyx_methods_21py_ballisticcalc_exts_15trajectory_calc_Vector[] = {
   {"__radd__", (PyCFunction)__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_6Vector_5__radd__, METH_O|METH_COEXIST, 0},
   {"__rsub__", (PyCFunction)__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_6Vector_11__rsub__, METH_O|METH_COEXIST, 0},
   {"__rmul__", (PyCFunction)__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_6Vector_17__rmul__, METH_O|METH_COEXIST, 0},
   {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_6Vector_23__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_6Vector_22__reduce_cython__},
   {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_6Vector_25__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_6Vector_24__setstate_cython__},
@@ -12792,45 +12799,55 @@
     "Vector",
     "__pyx_ctuple_Py_ssize_t",
     "__pyx_ctuple_Py_ssize_t_struct",
     "__pyx_ctuple_double",
     "__pyx_ctuple_double__and_double__and_double",
     "__pyx_ctuple_double__and_double__and_double_struct",
     "__pyx_ctuple_double_struct",
+    "__pyx_ctuple_int",
+    "__pyx_ctuple_int_struct",
     "__pyx_ctuple_long__and_int",
     "__pyx_ctuple_long__and_int_struct",
     "__pyx_ctuple_long__and_long__and_long",
     "__pyx_ctuple_long__and_long__and_long_struct",
-    "__pyx_opt_args_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_get_calc_step",
+    "__pyx_opt_args_21py_ballisticcalc_exts_15trajectory_calc_get_calc_step",
     "struct_type",
     0
   };
   const char** type_name = internal_type_names;
   while (*type_name) {
     if (__Pyx_StrEq(name, *type_name)) {
       PyErr_Format(PyExc_TypeError, "Cannot overwrite C type %s", name);
       goto bad;
     }
     type_name++;
   }
   if (0);
+  else if (__Pyx_StrEq(name, "_globalMaxCalcStepSize")) {
+    Py_INCREF(o);
+    Py_DECREF(__pyx_v_21py_ballisticcalc_exts_15trajectory_calc__globalMaxCalcStepSize);
+    __pyx_v_21py_ballisticcalc_exts_15trajectory_calc__globalMaxCalcStepSize = o;
+  }
+  else if (__Pyx_StrEq(name, "_globalUsePowderSensitivity")) {
+    __pyx_v_21py_ballisticcalc_exts_15trajectory_calc__globalUsePowderSensitivity = __Pyx_PyInt_As_int(o); if (unlikely((__pyx_v_21py_ballisticcalc_exts_15trajectory_calc__globalUsePowderSensitivity == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 24, __pyx_L2_error)
+  }
   else if (__Pyx_StrEq(name, "cGravityConstant")) {
-    __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cGravityConstant = __pyx_PyFloat_AsDouble(o); if (unlikely((__pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cGravityConstant == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 16, __pyx_L2_error)
+    __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cGravityConstant = __pyx_PyFloat_AsDouble(o); if (unlikely((__pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cGravityConstant == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 22, __pyx_L2_error)
   }
   else if (__Pyx_StrEq(name, "cMaxIterations")) {
-    __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cMaxIterations = __Pyx_PyInt_As_int(o); if (unlikely((__pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cMaxIterations == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 15, __pyx_L2_error)
+    __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cMaxIterations = __Pyx_PyInt_As_int(o); if (unlikely((__pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cMaxIterations == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 21, __pyx_L2_error)
   }
   else if (__Pyx_StrEq(name, "cMaximumDrop")) {
-    __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cMaximumDrop = __pyx_PyFloat_AsDouble(o); if (unlikely((__pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cMaximumDrop == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 14, __pyx_L2_error)
+    __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cMaximumDrop = __pyx_PyFloat_AsDouble(o); if (unlikely((__pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cMaximumDrop == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 20, __pyx_L2_error)
   }
   else if (__Pyx_StrEq(name, "cMinimumVelocity")) {
-    __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cMinimumVelocity = __pyx_PyFloat_AsDouble(o); if (unlikely((__pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cMinimumVelocity == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 13, __pyx_L2_error)
+    __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cMinimumVelocity = __pyx_PyFloat_AsDouble(o); if (unlikely((__pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cMinimumVelocity == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 19, __pyx_L2_error)
   }
   else if (__Pyx_StrEq(name, "cZeroFindingAccuracy")) {
-    __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cZeroFindingAccuracy = __pyx_PyFloat_AsDouble(o); if (unlikely((__pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cZeroFindingAccuracy == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 12, __pyx_L2_error)
+    __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cZeroFindingAccuracy = __pyx_PyFloat_AsDouble(o); if (unlikely((__pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cZeroFindingAccuracy == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 18, __pyx_L2_error)
   }
   else {
     if (PyObject_SetAttr(__pyx_m, py_name, o) < 0) goto bad;
   }
   return 0;
   __pyx_L2_error:;
   __Pyx_AddTraceback("py_ballisticcalc_exts.trajectory_calc", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -12955,15 +12972,14 @@
 #endif
 /* #### Code section: pystring_table ### */
 
 static int __Pyx_CreateStringTabAndInitStrings(void) {
   __Pyx_StringTabEntry __pyx_string_tab[] = {
     {&__pyx_n_s_Ammo, __pyx_k_Ammo, sizeof(__pyx_k_Ammo), 0, 0, 1, 1},
     {&__pyx_n_s_Angular, __pyx_k_Angular, sizeof(__pyx_k_Angular), 0, 0, 1, 1},
-    {&__pyx_n_s_Atmo, __pyx_k_Atmo, sizeof(__pyx_k_Atmo), 0, 0, 1, 1},
     {&__pyx_n_s_BC, __pyx_k_BC, sizeof(__pyx_k_BC), 0, 0, 1, 1},
     {&__pyx_n_s_CD, __pyx_k_CD, sizeof(__pyx_k_CD), 0, 0, 1, 1},
     {&__pyx_n_s_Distance, __pyx_k_Distance, sizeof(__pyx_k_Distance), 0, 0, 1, 1},
     {&__pyx_n_s_Energy, __pyx_k_Energy, sizeof(__pyx_k_Energy), 0, 0, 1, 1},
     {&__pyx_n_s_FPS, __pyx_k_FPS, sizeof(__pyx_k_FPS), 0, 0, 1, 1},
     {&__pyx_n_s_Fahrenheit, __pyx_k_Fahrenheit, sizeof(__pyx_k_Fahrenheit), 0, 0, 1, 1},
     {&__pyx_n_s_Foot, __pyx_k_Foot, sizeof(__pyx_k_Foot), 0, 0, 1, 1},
@@ -12979,78 +12995,69 @@
     {&__pyx_kp_s_No_value_specified_for_struct_at_2, __pyx_k_No_value_specified_for_struct_at_2, sizeof(__pyx_k_No_value_specified_for_struct_at_2), 0, 0, 1, 0},
     {&__pyx_kp_s_No_value_specified_for_struct_at_3, __pyx_k_No_value_specified_for_struct_at_3, sizeof(__pyx_k_No_value_specified_for_struct_at_3), 0, 0, 1, 0},
     {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
     {&__pyx_n_s_Pound, __pyx_k_Pound, sizeof(__pyx_k_Pound), 0, 0, 1, 1},
     {&__pyx_n_s_PreferredUnits, __pyx_k_PreferredUnits, sizeof(__pyx_k_PreferredUnits), 0, 0, 1, 1},
     {&__pyx_n_s_Pressure, __pyx_k_Pressure, sizeof(__pyx_k_Pressure), 0, 0, 1, 1},
     {&__pyx_n_s_Radian, __pyx_k_Radian, sizeof(__pyx_k_Radian), 0, 0, 1, 1},
-    {&__pyx_n_s_Settings, __pyx_k_Settings, sizeof(__pyx_k_Settings), 0, 0, 1, 1},
     {&__pyx_n_s_Shot, __pyx_k_Shot, sizeof(__pyx_k_Shot), 0, 0, 1, 1},
     {&__pyx_n_s_Temperature, __pyx_k_Temperature, sizeof(__pyx_k_Temperature), 0, 0, 1, 1},
     {&__pyx_n_s_TrajectoryCalc, __pyx_k_TrajectoryCalc, sizeof(__pyx_k_TrajectoryCalc), 0, 0, 1, 1},
     {&__pyx_n_u_TrajectoryCalc, __pyx_k_TrajectoryCalc, sizeof(__pyx_k_TrajectoryCalc), 0, 1, 0, 1},
-    {&__pyx_n_s_TrajectoryCalc___reduce_cython, __pyx_k_TrajectoryCalc___reduce_cython, sizeof(__pyx_k_TrajectoryCalc___reduce_cython), 0, 0, 1, 1},
-    {&__pyx_n_s_TrajectoryCalc___setstate_cython, __pyx_k_TrajectoryCalc___setstate_cython, sizeof(__pyx_k_TrajectoryCalc___setstate_cython), 0, 0, 1, 1},
-    {&__pyx_n_s_TrajectoryCalc_trajectory, __pyx_k_TrajectoryCalc_trajectory, sizeof(__pyx_k_TrajectoryCalc_trajectory), 0, 0, 1, 1},
-    {&__pyx_n_s_TrajectoryCalc_zero_angle, __pyx_k_TrajectoryCalc_zero_angle, sizeof(__pyx_k_TrajectoryCalc_zero_angle), 0, 0, 1, 1},
     {&__pyx_n_s_TrajectoryData, __pyx_k_TrajectoryData, sizeof(__pyx_k_TrajectoryData), 0, 0, 1, 1},
     {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
-    {&__pyx_n_s_USE_POWDER_SENSITIVITY, __pyx_k_USE_POWDER_SENSITIVITY, sizeof(__pyx_k_USE_POWDER_SENSITIVITY), 0, 0, 1, 1},
     {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
     {&__pyx_n_s_Vector, __pyx_k_Vector, sizeof(__pyx_k_Vector), 0, 0, 1, 1},
-    {&__pyx_n_s_Vector___reduce_cython, __pyx_k_Vector___reduce_cython, sizeof(__pyx_k_Vector___reduce_cython), 0, 0, 1, 1},
-    {&__pyx_n_s_Vector___setstate_cython, __pyx_k_Vector___setstate_cython, sizeof(__pyx_k_Vector___setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_Velocity, __pyx_k_Velocity, sizeof(__pyx_k_Velocity), 0, 0, 1, 1},
     {&__pyx_n_s_Weight, __pyx_k_Weight, sizeof(__pyx_k_Weight), 0, 0, 1, 1},
     {&__pyx_n_s_Wind, __pyx_k_Wind, sizeof(__pyx_k_Wind), 0, 0, 1, 1},
     {&__pyx_kp_u_Zero_vertical_error, __pyx_k_Zero_vertical_error, sizeof(__pyx_k_Zero_vertical_error), 0, 1, 0, 0},
-    {&__pyx_n_s__23, __pyx_k__23, sizeof(__pyx_k__23), 0, 0, 1, 1},
-    {&__pyx_kp_u__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 1, 0, 0},
-    {&__pyx_n_s__7, __pyx_k__7, sizeof(__pyx_k__7), 0, 0, 1, 1},
+    {&__pyx_n_s__20, __pyx_k__20, sizeof(__pyx_k__20), 0, 0, 1, 1},
+    {&__pyx_kp_u__7, __pyx_k__7, sizeof(__pyx_k__7), 0, 1, 0, 0},
+    {&__pyx_n_s__8, __pyx_k__8, sizeof(__pyx_k__8), 0, 0, 1, 1},
     {&__pyx_n_s_a, __pyx_k_a, sizeof(__pyx_k_a), 0, 0, 1, 1},
     {&__pyx_n_s_all, __pyx_k_all, sizeof(__pyx_k_all), 0, 0, 1, 1},
     {&__pyx_n_s_altitude, __pyx_k_altitude, sizeof(__pyx_k_altitude), 0, 0, 1, 1},
     {&__pyx_n_s_ammo, __pyx_k_ammo, sizeof(__pyx_k_ammo), 0, 0, 1, 1},
     {&__pyx_n_s_angle, __pyx_k_angle, sizeof(__pyx_k_angle), 0, 0, 1, 1},
-    {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
     {&__pyx_n_s_atmo, __pyx_k_atmo, sizeof(__pyx_k_atmo), 0, 0, 1, 1},
     {&__pyx_n_s_b, __pyx_k_b, sizeof(__pyx_k_b), 0, 0, 1, 1},
     {&__pyx_n_s_barrel_azimuth, __pyx_k_barrel_azimuth, sizeof(__pyx_k_barrel_azimuth), 0, 0, 1, 1},
     {&__pyx_n_s_barrel_elevation, __pyx_k_barrel_elevation, sizeof(__pyx_k_barrel_elevation), 0, 0, 1, 1},
-    {&__pyx_n_s_bool, __pyx_k_bool, sizeof(__pyx_k_bool), 0, 0, 1, 1},
     {&__pyx_n_s_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 0, 1, 1},
     {&__pyx_n_s_cant_angle, __pyx_k_cant_angle, sizeof(__pyx_k_cant_angle), 0, 0, 1, 1},
-    {&__pyx_n_s_class_getitem, __pyx_k_class_getitem, sizeof(__pyx_k_class_getitem), 0, 0, 1, 1},
     {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
     {&__pyx_n_s_density_factor, __pyx_k_density_factor, sizeof(__pyx_k_density_factor), 0, 0, 1, 1},
     {&__pyx_n_s_diameter, __pyx_k_diameter, sizeof(__pyx_k_diameter), 0, 0, 1, 1},
     {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
-    {&__pyx_n_s_dict_2, __pyx_k_dict_2, sizeof(__pyx_k_dict_2), 0, 0, 1, 1},
     {&__pyx_n_s_direction_from, __pyx_k_direction_from, sizeof(__pyx_k_direction_from), 0, 0, 1, 1},
     {&__pyx_kp_u_disable, __pyx_k_disable, sizeof(__pyx_k_disable), 0, 1, 0, 0},
     {&__pyx_n_s_dist_step, __pyx_k_dist_step, sizeof(__pyx_k_dist_step), 0, 0, 1, 1},
     {&__pyx_n_s_distance, __pyx_k_distance, sizeof(__pyx_k_distance), 0, 0, 1, 1},
     {&__pyx_n_s_dm, __pyx_k_dm, sizeof(__pyx_k_dm), 0, 0, 1, 1},
     {&__pyx_n_s_drag, __pyx_k_drag, sizeof(__pyx_k_drag), 0, 0, 1, 1},
     {&__pyx_n_s_drag_table, __pyx_k_drag_table, sizeof(__pyx_k_drag_table), 0, 0, 1, 1},
     {&__pyx_n_s_drop_adj, __pyx_k_drop_adj, sizeof(__pyx_k_drop_adj), 0, 0, 1, 1},
     {&__pyx_kp_u_enable, __pyx_k_enable, sizeof(__pyx_k_enable), 0, 1, 0, 0},
     {&__pyx_n_s_energy, __pyx_k_energy, sizeof(__pyx_k_energy), 0, 0, 1, 1},
     {&__pyx_n_s_extra_data, __pyx_k_extra_data, sizeof(__pyx_k_extra_data), 0, 0, 1, 1},
     {&__pyx_kp_u_feet_after, __pyx_k_feet_after, sizeof(__pyx_k_feet_after), 0, 1, 0, 0},
-    {&__pyx_n_s_filter_flags, __pyx_k_filter_flags, sizeof(__pyx_k_filter_flags), 0, 0, 1, 1},
     {&__pyx_n_s_flag, __pyx_k_flag, sizeof(__pyx_k_flag), 0, 0, 1, 1},
     {&__pyx_kp_u_gc, __pyx_k_gc, sizeof(__pyx_k_gc), 0, 1, 0, 0},
     {&__pyx_n_s_get_density_factor_and_mach_for, __pyx_k_get_density_factor_and_mach_for, sizeof(__pyx_k_get_density_factor_and_mach_for), 0, 0, 1, 1},
-    {&__pyx_n_s_get_max_calc_step_size, __pyx_k_get_max_calc_step_size, sizeof(__pyx_k_get_max_calc_step_size), 0, 0, 1, 1},
+    {&__pyx_n_s_get_global_max_calc_step_size, __pyx_k_get_global_max_calc_step_size, sizeof(__pyx_k_get_global_max_calc_step_size), 0, 0, 1, 1},
+    {&__pyx_n_u_get_global_max_calc_step_size, __pyx_k_get_global_max_calc_step_size, sizeof(__pyx_k_get_global_max_calc_step_size), 0, 1, 0, 1},
+    {&__pyx_n_s_get_global_use_powder_sensitivit, __pyx_k_get_global_use_powder_sensitivit, sizeof(__pyx_k_get_global_use_powder_sensitivit), 0, 0, 1, 1},
+    {&__pyx_n_u_get_global_use_powder_sensitivit, __pyx_k_get_global_use_powder_sensitivit, sizeof(__pyx_k_get_global_use_powder_sensitivit), 0, 1, 0, 1},
     {&__pyx_n_s_get_velocity_for_temp, __pyx_k_get_velocity_for_temp, sizeof(__pyx_k_get_velocity_for_temp), 0, 0, 1, 1},
     {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
+    {&__pyx_kp_u_globalMaxCalcStepSize_have_to_b, __pyx_k_globalMaxCalcStepSize_have_to_b, sizeof(__pyx_k_globalMaxCalcStepSize_have_to_b), 0, 1, 0, 0},
     {&__pyx_n_s_height, __pyx_k_height, sizeof(__pyx_k_height), 0, 0, 1, 1},
     {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
-    {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
+    {&__pyx_kp_u_is_not_a_boolean, __pyx_k_is_not_a_boolean, sizeof(__pyx_k_is_not_a_boolean), 0, 1, 0, 0},
     {&__pyx_kp_u_isenabled, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
     {&__pyx_kp_u_iterations, __pyx_k_iterations, sizeof(__pyx_k_iterations), 0, 1, 0, 0},
     {&__pyx_n_s_length, __pyx_k_length, sizeof(__pyx_k_length), 0, 0, 1, 1},
     {&__pyx_n_s_look_angle, __pyx_k_look_angle, sizeof(__pyx_k_look_angle), 0, 0, 1, 1},
     {&__pyx_n_s_look_distance, __pyx_k_look_distance, sizeof(__pyx_k_look_distance), 0, 0, 1, 1},
     {&__pyx_n_s_mach, __pyx_k_mach, sizeof(__pyx_k_mach), 0, 0, 1, 1},
     {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
@@ -13060,68 +13067,71 @@
     {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
     {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
     {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
     {&__pyx_n_s_ogw, __pyx_k_ogw, sizeof(__pyx_k_ogw), 0, 0, 1, 1},
     {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
     {&__pyx_n_s_pressure, __pyx_k_pressure, sizeof(__pyx_k_pressure), 0, 0, 1, 1},
     {&__pyx_n_s_py_ballisticcalc_conditions, __pyx_k_py_ballisticcalc_conditions, sizeof(__pyx_k_py_ballisticcalc_conditions), 0, 0, 1, 1},
-    {&__pyx_n_s_py_ballisticcalc_exts_trajectory, __pyx_k_py_ballisticcalc_exts_trajectory, sizeof(__pyx_k_py_ballisticcalc_exts_trajectory), 0, 0, 1, 1},
-    {&__pyx_kp_s_py_ballisticcalc_exts_trajectory_2, __pyx_k_py_ballisticcalc_exts_trajectory_2, sizeof(__pyx_k_py_ballisticcalc_exts_trajectory_2), 0, 0, 1, 0},
+    {&__pyx_kp_s_py_ballisticcalc_exts_trajectory, __pyx_k_py_ballisticcalc_exts_trajectory, sizeof(__pyx_k_py_ballisticcalc_exts_trajectory), 0, 0, 1, 0},
+    {&__pyx_n_s_py_ballisticcalc_exts_trajectory_2, __pyx_k_py_ballisticcalc_exts_trajectory_2, sizeof(__pyx_k_py_ballisticcalc_exts_trajectory_2), 0, 0, 1, 1},
     {&__pyx_n_s_py_ballisticcalc_munition, __pyx_k_py_ballisticcalc_munition, sizeof(__pyx_k_py_ballisticcalc_munition), 0, 0, 1, 1},
-    {&__pyx_n_s_py_ballisticcalc_settings, __pyx_k_py_ballisticcalc_settings, sizeof(__pyx_k_py_ballisticcalc_settings), 0, 0, 1, 1},
     {&__pyx_n_s_py_ballisticcalc_trajectory_data, __pyx_k_py_ballisticcalc_trajectory_data, sizeof(__pyx_k_py_ballisticcalc_trajectory_data), 0, 0, 1, 1},
     {&__pyx_n_s_py_ballisticcalc_unit, __pyx_k_py_ballisticcalc_unit, sizeof(__pyx_k_py_ballisticcalc_unit), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_unpickle_TrajectoryCalc, __pyx_k_pyx_unpickle_TrajectoryCalc, sizeof(__pyx_k_pyx_unpickle_TrajectoryCalc), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
     {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
+    {&__pyx_n_s_raw_value, __pyx_k_raw_value, sizeof(__pyx_k_raw_value), 0, 0, 1, 1},
     {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
     {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
-    {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
+    {&__pyx_n_s_reset_globals, __pyx_k_reset_globals, sizeof(__pyx_k_reset_globals), 0, 0, 1, 1},
+    {&__pyx_n_u_reset_globals, __pyx_k_reset_globals, sizeof(__pyx_k_reset_globals), 0, 1, 0, 1},
+    {&__pyx_n_s_set_global_max_calc_step_size, __pyx_k_set_global_max_calc_step_size, sizeof(__pyx_k_set_global_max_calc_step_size), 0, 0, 1, 1},
+    {&__pyx_n_u_set_global_max_calc_step_size, __pyx_k_set_global_max_calc_step_size, sizeof(__pyx_k_set_global_max_calc_step_size), 0, 1, 0, 1},
+    {&__pyx_kp_u_set_global_use_powder_sensitivit, __pyx_k_set_global_use_powder_sensitivit, sizeof(__pyx_k_set_global_use_powder_sensitivit), 0, 1, 0, 0},
+    {&__pyx_n_s_set_global_use_powder_sensitivit_2, __pyx_k_set_global_use_powder_sensitivit_2, sizeof(__pyx_k_set_global_use_powder_sensitivit_2), 0, 0, 1, 1},
+    {&__pyx_n_u_set_global_use_powder_sensitivit_2, __pyx_k_set_global_use_powder_sensitivit_2, sizeof(__pyx_k_set_global_use_powder_sensitivit_2), 0, 1, 0, 1},
     {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
     {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_shot_info, __pyx_k_shot_info, sizeof(__pyx_k_shot_info), 0, 0, 1, 1},
     {&__pyx_n_s_sight_height, __pyx_k_sight_height, sizeof(__pyx_k_sight_height), 0, 0, 1, 1},
-    {&__pyx_n_s_state, __pyx_k_state, sizeof(__pyx_k_state), 0, 0, 1, 1},
-    {&__pyx_n_s_step, __pyx_k_step, sizeof(__pyx_k_step), 0, 0, 1, 1},
     {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
     {&__pyx_n_s_target_drop, __pyx_k_target_drop, sizeof(__pyx_k_target_drop), 0, 0, 1, 1},
     {&__pyx_n_s_temperature, __pyx_k_temperature, sizeof(__pyx_k_temperature), 0, 0, 1, 1},
     {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
     {&__pyx_n_s_time, __pyx_k_time, sizeof(__pyx_k_time), 0, 0, 1, 1},
-    {&__pyx_n_s_trajectory, __pyx_k_trajectory, sizeof(__pyx_k_trajectory), 0, 0, 1, 1},
     {&__pyx_n_s_twist, __pyx_k_twist, sizeof(__pyx_k_twist), 0, 0, 1, 1},
     {&__pyx_n_s_until_distance, __pyx_k_until_distance, sizeof(__pyx_k_until_distance), 0, 0, 1, 1},
     {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
-    {&__pyx_n_s_use_setstate, __pyx_k_use_setstate, sizeof(__pyx_k_use_setstate), 0, 0, 1, 1},
+    {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
+    {&__pyx_n_s_value_2, __pyx_k_value_2, sizeof(__pyx_k_value_2), 0, 0, 1, 1},
     {&__pyx_n_s_velocity, __pyx_k_velocity, sizeof(__pyx_k_velocity), 0, 0, 1, 1},
     {&__pyx_n_s_weapon, __pyx_k_weapon, sizeof(__pyx_k_weapon), 0, 0, 1, 1},
     {&__pyx_n_s_weight, __pyx_k_weight, sizeof(__pyx_k_weight), 0, 0, 1, 1},
     {&__pyx_n_s_windage, __pyx_k_windage, sizeof(__pyx_k_windage), 0, 0, 1, 1},
     {&__pyx_n_s_windage_adj, __pyx_k_windage_adj, sizeof(__pyx_k_windage_adj), 0, 0, 1, 1},
     {&__pyx_n_s_winds, __pyx_k_winds, sizeof(__pyx_k_winds), 0, 0, 1, 1},
     {&__pyx_n_s_x, __pyx_k_x, sizeof(__pyx_k_x), 0, 0, 1, 1},
     {&__pyx_n_s_y, __pyx_k_y, sizeof(__pyx_k_y), 0, 0, 1, 1},
     {&__pyx_n_s_z, __pyx_k_z, sizeof(__pyx_k_z), 0, 0, 1, 1},
-    {&__pyx_n_s_zero_angle, __pyx_k_zero_angle, sizeof(__pyx_k_zero_angle), 0, 0, 1, 1},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 88, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 411, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 463, __pyx_L1_error)
   __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(1, 19, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 20, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
@@ -13157,143 +13167,149 @@
  *     result.c = value
  *     return result
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_No_value_specified_for_struct_at_3); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":219
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":38
+ *     global _globalMaxCalcStepSize
+ *     if (_value := PreferredUnits.distance(value)).raw_value <= 0:
+ *         raise ValueError("_globalMaxCalcStepSize have to be > 0")             # <<<<<<<<<<<<<<
+ *     _globalMaxCalcStepSize = PreferredUnits.distance(value)
+ * 
+ */
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_globalMaxCalcStepSize_have_to_b); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__4);
+  __Pyx_GIVEREF(__pyx_tuple__4);
+
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":259
  * 
  *         if len_winds < 1:
  *             wind_vector = Vector(.0, .0, .0)             # <<<<<<<<<<<<<<
  *         else:
  *             wind_vector = wind_to_vector(shot_info.winds[0])
  */
-  __pyx_tuple__4 = PyTuple_Pack(3, __pyx_float__0, __pyx_float__0, __pyx_float__0); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 219, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
+  __pyx_tuple__5 = PyTuple_Pack(3, __pyx_float__0, __pyx_float__0, __pyx_float__0); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 259, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x1a1505e, 0xaee47ca, 0x4420ce0):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x1a1505e, 0xaee47ca, 0x4420ce0) = (_bc, _curve, _table_data, alt0, ammo, barrel_azimuth, barrel_elevation, calc_step, cant_cosine, cant_sine, diameter, gravity_vector, length, look_angle, muzzle_velocity, sight_height, stability_coefficient, twist, weight))" % __pyx_checksum
  */
-  __pyx_tuple__5 = PyTuple_Pack(3, __pyx_int_27349086, __pyx_int_183388106, __pyx_int_71437536); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__5);
-  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_tuple__6 = PyTuple_Pack(3, __pyx_int_27349086, __pyx_int_183388106, __pyx_int_71437536); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
 
   /* "py_ballisticcalc_exts/trajectory_calc.pyx":10
- * from py_ballisticcalc.unit import *
  * 
- * __all__ = ('TrajectoryCalc',)             # <<<<<<<<<<<<<<
+ * __all__ = (
+ *     'TrajectoryCalc',             # <<<<<<<<<<<<<<
+ *     'get_global_max_calc_step_size',
+ *     'get_global_use_powder_sensitivity',
+ */
+  __pyx_tuple__9 = PyTuple_Pack(6, __pyx_n_u_TrajectoryCalc, __pyx_n_u_get_global_max_calc_step_size, __pyx_n_u_get_global_use_powder_sensitivit, __pyx_n_u_set_global_max_calc_step_size, __pyx_n_u_set_global_use_powder_sensitivit_2, __pyx_n_u_reset_globals); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
+
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":25
  * 
- * cdef double cZeroFindingAccuracy = 0.000005
+ * cdef int _globalUsePowderSensitivity = False
+ * cdef object _globalMaxCalcStepSize = Distance.Foot(0.5)             # <<<<<<<<<<<<<<
+ * 
+ * def get_global_max_calc_step_size() -> Distance:
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_n_u_TrajectoryCalc); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 10, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_float_0_5); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__10);
+  __Pyx_GIVEREF(__pyx_tuple__10);
 
-  /* "(tree fragment)":1
- * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
- *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
- * def __setstate_cython__(self, __pyx_state):
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":27
+ * cdef object _globalMaxCalcStepSize = Distance.Foot(0.5)
+ * 
+ * def get_global_max_calc_step_size() -> Distance:             # <<<<<<<<<<<<<<
+ *     return _globalMaxCalcStepSize
+ * 
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
-  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_py_ballisticcalc_exts_trajectory, __pyx_n_s_get_global_max_calc_step_size, 27, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 27, __pyx_L1_error)
 
-  /* "(tree fragment)":3
- * def __reduce_cython__(self):
- *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
- * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
- *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":31
+ * 
+ * 
+ * def get_global_use_powder_sensitivity() -> bool:             # <<<<<<<<<<<<<<
+ *     return bool(_globalUsePowderSensitivity)
+ * 
  */
-  __pyx_tuple__11 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 3, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__11);
-  __Pyx_GIVEREF(__pyx_tuple__11);
-  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_py_ballisticcalc_exts_trajectory, __pyx_n_s_get_global_use_powder_sensitivit, 31, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 31, __pyx_L1_error)
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":133
- *         return min(step, Settings.get_max_calc_step_size()) / 2.0
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":35
  * 
- *     def zero_angle(self, shot_info: Shot, distance: Distance):             # <<<<<<<<<<<<<<
- *         return self._zero_angle(shot_info, distance)
  * 
+ * def set_global_max_calc_step_size(value: [object, float]) -> None:             # <<<<<<<<<<<<<<
+ *     global _globalMaxCalcStepSize
+ *     if (_value := PreferredUnits.distance(value)).raw_value <= 0:
  */
-  __pyx_tuple__13 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_shot_info, __pyx_n_s_distance); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(2, __pyx_n_s_value, __pyx_n_s_value_2); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
-  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_py_ballisticcalc_exts_trajectory_2, __pyx_n_s_zero_angle, 133, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_py_ballisticcalc_exts_trajectory, __pyx_n_s_set_global_max_calc_step_size, 35, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 35, __pyx_L1_error)
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":136
- *         return self._zero_angle(shot_info, distance)
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":42
  * 
- *     def trajectory(self, shot_info: Shot, max_range: Distance, dist_step: Distance,             # <<<<<<<<<<<<<<
- *                    extra_data: bool = False):
- *         cdef:
+ * 
+ * def set_global_use_powder_sensitivity(value: bool) -> None:             # <<<<<<<<<<<<<<
+ *     global _globalUsePowderSensitivity
+ *     if not isinstance(value, bool):
  */
-  __pyx_tuple__15 = PyTuple_Pack(9, __pyx_n_s_self, __pyx_n_s_shot_info, __pyx_n_s_max_range, __pyx_n_s_dist_step, __pyx_n_s_extra_data, __pyx_n_s_step, __pyx_n_s_atmo, __pyx_n_s_winds, __pyx_n_s_filter_flags); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_n_s_value); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
-  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_py_ballisticcalc_exts_trajectory_2, __pyx_n_s_trajectory, 136, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 136, __pyx_L1_error)
-  __pyx_tuple__17 = PyTuple_Pack(1, Py_False); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 136, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__17);
-  __Pyx_GIVEREF(__pyx_tuple__17);
-
-  /* "(tree fragment)":1
- * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
- *     cdef tuple state
- *     cdef object _dict
- */
-  __pyx_tuple__18 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_py_ballisticcalc_exts_trajectory, __pyx_n_s_set_global_use_powder_sensitivit_2, 42, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 42, __pyx_L1_error)
 
-  /* "(tree fragment)":16
- *     else:
- *         return __pyx_unpickle_TrajectoryCalc, (type(self), 0x1a1505e, state)
- * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
- *     __pyx_unpickle_TrajectoryCalc__set_state(self, __pyx_state)
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":49
+ * 
+ * 
+ * def reset_globals() -> None:             # <<<<<<<<<<<<<<
+ *     global _globalUsePowderSensitivity, _globalMaxCalcStepSize
+ *     _globalUsePowderSensitivity = False
  */
-  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_py_ballisticcalc_exts_trajectory, __pyx_n_s_reset_globals, 49, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 49, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_TrajectoryCalc(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__21 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__21);
-  __Pyx_GIVEREF(__pyx_tuple__21);
-  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_TrajectoryCalc, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__18 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__18);
+  __Pyx_GIVEREF(__pyx_tuple__18);
+  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_TrajectoryCalc, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitConstants(void) {
   if (__Pyx_CreateStringTabAndInitStrings() < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_float__0 = PyFloat_FromDouble(.0); if (unlikely(!__pyx_float__0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_0_ = PyFloat_FromDouble(0.); if (unlikely(!__pyx_float_0_)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_0_0 = PyFloat_FromDouble(0.0); if (unlikely(!__pyx_float_0_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_0_2 = PyFloat_FromDouble(0.2); if (unlikely(!__pyx_float_0_2)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_float_2_0 = PyFloat_FromDouble(2.0); if (unlikely(!__pyx_float_2_0)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_float_0_5 = PyFloat_FromDouble(0.5); if (unlikely(!__pyx_float_0_5)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_int_12 = PyInt_FromLong(12); if (unlikely(!__pyx_int_12)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_27349086 = PyInt_FromLong(27349086L); if (unlikely(!__pyx_int_27349086)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_71437536 = PyInt_FromLong(71437536L); if (unlikely(!__pyx_int_71437536)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_183388106 = PyInt_FromLong(183388106L); if (unlikely(!__pyx_int_183388106)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: init_globals ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
@@ -13309,14 +13325,15 @@
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_import_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_function_import_code(void); /*proto*/
 
 static int __Pyx_modinit_global_init_code(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_modinit_global_init_code", 0);
   /*--- Global init code ---*/
+  __pyx_v_21py_ballisticcalc_exts_15trajectory_calc__globalMaxCalcStepSize = Py_None; Py_INCREF(Py_None);
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 static int __Pyx_modinit_variable_export_code(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_modinit_variable_export_code", 0);
@@ -13345,74 +13362,73 @@
   __pyx_vtable_21py_ballisticcalc_exts_15trajectory_calc_Vector.mul_by_const = (struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *(*)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *, double))__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_6Vector_mul_by_const;
   __pyx_vtable_21py_ballisticcalc_exts_15trajectory_calc_Vector.mul_by_vector = (double (*)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *, struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *))__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_6Vector_mul_by_vector;
   __pyx_vtable_21py_ballisticcalc_exts_15trajectory_calc_Vector.add = (struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *(*)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *, struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *))__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_6Vector_add;
   __pyx_vtable_21py_ballisticcalc_exts_15trajectory_calc_Vector.subtract = (struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *(*)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *, struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *))__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_6Vector_subtract;
   __pyx_vtable_21py_ballisticcalc_exts_15trajectory_calc_Vector.negate = (struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *(*)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *))__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_6Vector_negate;
   __pyx_vtable_21py_ballisticcalc_exts_15trajectory_calc_Vector.normalize = (struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *(*)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *))__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_6Vector_normalize;
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_21py_ballisticcalc_exts_15trajectory_calc_Vector_spec, NULL); if (unlikely(!__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector)) __PYX_ERR(0, 31, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_21py_ballisticcalc_exts_15trajectory_calc_Vector_spec, __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_21py_ballisticcalc_exts_15trajectory_calc_Vector_spec, NULL); if (unlikely(!__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector)) __PYX_ERR(0, 69, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_21py_ballisticcalc_exts_15trajectory_calc_Vector_spec, __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
   #else
   __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector = &__pyx_type_21py_ballisticcalc_exts_15trajectory_calc_Vector;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector->tp_dictoffset && __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
-  if (__Pyx_SetVtable(__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector, __pyx_vtabptr_21py_ballisticcalc_exts_15trajectory_calc_Vector) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector, __pyx_vtabptr_21py_ballisticcalc_exts_15trajectory_calc_Vector) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_MergeVtables(__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
+  if (__Pyx_MergeVtables(__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Vector, (PyObject *) __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Vector, (PyObject *) __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
   #endif
   __pyx_vtabptr_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc = &__pyx_vtable_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc;
-  __pyx_vtable_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc.get_calc_step = (double (*)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *, struct __pyx_opt_args_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_get_calc_step *__pyx_optional_args))__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_get_calc_step;
   __pyx_vtable_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc._init_trajectory = (PyObject *(*)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *, PyObject *))__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc__init_trajectory;
   __pyx_vtable_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc._zero_angle = (PyObject *(*)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *, PyObject *, PyObject *))__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc__zero_angle;
-  __pyx_vtable_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc._trajectory = (PyObject *(*)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *, PyObject *, double, double, enum __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag))__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc__trajectory;
+  __pyx_vtable_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc._trajectory = (PyObject *(*)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *, PyObject *, double, double, int))__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc__trajectory;
   __pyx_vtable_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc.drag_by_mach = (double (*)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *, double))__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_drag_by_mach;
   __pyx_vtable_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc.spin_drift = (double (*)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *, double))__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_spin_drift;
   __pyx_vtable_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc.calc_stability_coefficient = (double (*)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *, PyObject *))__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_calc_stability_coefficient;
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc_spec, NULL); if (unlikely(!__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc)) __PYX_ERR(0, 99, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc_spec, __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc_spec, NULL); if (unlikely(!__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc)) __PYX_ERR(0, 137, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc_spec, __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
   #else
   __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc = &__pyx_type_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc->tp_dictoffset && __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
-  if (__Pyx_SetVtable(__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc, __pyx_vtabptr_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc, __pyx_vtabptr_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_MergeVtables(__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (__Pyx_MergeVtables(__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_TrajectoryCalc, (PyObject *) __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_TrajectoryCalc, (PyObject *) __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
   #endif
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
@@ -13719,52 +13735,45 @@
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
   /* "py_ballisticcalc_exts/trajectory_calc.pyx":4
  * cimport cython
  * 
- * from py_ballisticcalc.conditions import Atmo, Shot, Wind             # <<<<<<<<<<<<<<
+ * from py_ballisticcalc.conditions import Shot, Wind             # <<<<<<<<<<<<<<
  * from py_ballisticcalc.munition import Ammo
- * from py_ballisticcalc.settings import Settings
+ * from py_ballisticcalc.trajectory_data import TrajectoryData
  */
-  __pyx_t_2 = PyList_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_INCREF(__pyx_n_s_Atmo);
-  __Pyx_GIVEREF(__pyx_n_s_Atmo);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_Atmo)) __PYX_ERR(0, 4, __pyx_L1_error);
   __Pyx_INCREF(__pyx_n_s_Shot);
   __Pyx_GIVEREF(__pyx_n_s_Shot);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_s_Shot)) __PYX_ERR(0, 4, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_Shot)) __PYX_ERR(0, 4, __pyx_L1_error);
   __Pyx_INCREF(__pyx_n_s_Wind);
   __Pyx_GIVEREF(__pyx_n_s_Wind);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 2, __pyx_n_s_Wind)) __PYX_ERR(0, 4, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_s_Wind)) __PYX_ERR(0, 4, __pyx_L1_error);
   __pyx_t_3 = __Pyx_Import(__pyx_n_s_py_ballisticcalc_conditions, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_Atmo); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Atmo, __pyx_t_2) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_Shot); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_Shot, __pyx_t_2) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_Wind); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_Wind, __pyx_t_2) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "py_ballisticcalc_exts/trajectory_calc.pyx":5
  * 
- * from py_ballisticcalc.conditions import Atmo, Shot, Wind
+ * from py_ballisticcalc.conditions import Shot, Wind
  * from py_ballisticcalc.munition import Ammo             # <<<<<<<<<<<<<<
- * from py_ballisticcalc.settings import Settings
  * from py_ballisticcalc.trajectory_data import TrajectoryData
+ * from py_ballisticcalc.unit import *
  */
   __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_n_s_Ammo);
   __Pyx_GIVEREF(__pyx_n_s_Ammo);
   if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_Ammo)) __PYX_ERR(0, 5, __pyx_L1_error);
   __pyx_t_2 = __Pyx_Import(__pyx_n_s_py_ballisticcalc_munition, __pyx_t_3, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 5, __pyx_L1_error)
@@ -13773,231 +13782,214 @@
   __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Ammo); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_Ammo, __pyx_t_3) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "py_ballisticcalc_exts/trajectory_calc.pyx":6
- * from py_ballisticcalc.conditions import Atmo, Shot, Wind
+ * from py_ballisticcalc.conditions import Shot, Wind
  * from py_ballisticcalc.munition import Ammo
- * from py_ballisticcalc.settings import Settings             # <<<<<<<<<<<<<<
- * from py_ballisticcalc.trajectory_data import TrajectoryData
+ * from py_ballisticcalc.trajectory_data import TrajectoryData             # <<<<<<<<<<<<<<
  * from py_ballisticcalc.unit import *
+ * 
  */
   __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_INCREF(__pyx_n_s_Settings);
-  __Pyx_GIVEREF(__pyx_n_s_Settings);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_Settings)) __PYX_ERR(0, 6, __pyx_L1_error);
-  __pyx_t_3 = __Pyx_Import(__pyx_n_s_py_ballisticcalc_settings, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 6, __pyx_L1_error)
+  __Pyx_INCREF(__pyx_n_s_TrajectoryData);
+  __Pyx_GIVEREF(__pyx_n_s_TrajectoryData);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_TrajectoryData)) __PYX_ERR(0, 6, __pyx_L1_error);
+  __pyx_t_3 = __Pyx_Import(__pyx_n_s_py_ballisticcalc_trajectory_data, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_Settings); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 6, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_TrajectoryData); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Settings, __pyx_t_2) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_TrajectoryData, __pyx_t_2) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "py_ballisticcalc_exts/trajectory_calc.pyx":7
  * from py_ballisticcalc.munition import Ammo
- * from py_ballisticcalc.settings import Settings
- * from py_ballisticcalc.trajectory_data import TrajectoryData             # <<<<<<<<<<<<<<
- * from py_ballisticcalc.unit import *
+ * from py_ballisticcalc.trajectory_data import TrajectoryData
+ * from py_ballisticcalc.unit import *             # <<<<<<<<<<<<<<
  * 
+ * __all__ = (
  */
   __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_INCREF(__pyx_n_s_TrajectoryData);
-  __Pyx_GIVEREF(__pyx_n_s_TrajectoryData);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_TrajectoryData)) __PYX_ERR(0, 7, __pyx_L1_error);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_py_ballisticcalc_trajectory_data, __pyx_t_3, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __Pyx_INCREF(__pyx_n_s__8);
+  __Pyx_GIVEREF(__pyx_n_s__8);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_n_s__8)) __PYX_ERR(0, 7, __pyx_L1_error);
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_py_ballisticcalc_unit, __pyx_t_3, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_TrajectoryData); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_TrajectoryData, __pyx_t_3) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":8
- * from py_ballisticcalc.settings import Settings
- * from py_ballisticcalc.trajectory_data import TrajectoryData
- * from py_ballisticcalc.unit import *             # <<<<<<<<<<<<<<
- * 
- * __all__ = ('TrajectoryCalc',)
- */
-  __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 8, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_INCREF(__pyx_n_s__7);
-  __Pyx_GIVEREF(__pyx_n_s__7);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s__7)) __PYX_ERR(0, 8, __pyx_L1_error);
-  __pyx_t_3 = __Pyx_Import(__pyx_n_s_py_ballisticcalc_unit, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 8, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
+  if (__pyx_import_star(__pyx_t_2) < 0) __PYX_ERR(0, 7, __pyx_L1_error);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__pyx_import_star(__pyx_t_3) < 0) __PYX_ERR(0, 8, __pyx_L1_error);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "py_ballisticcalc_exts/trajectory_calc.pyx":10
- * from py_ballisticcalc.unit import *
  * 
- * __all__ = ('TrajectoryCalc',)             # <<<<<<<<<<<<<<
- * 
- * cdef double cZeroFindingAccuracy = 0.000005
+ * __all__ = (
+ *     'TrajectoryCalc',             # <<<<<<<<<<<<<<
+ *     'get_global_max_calc_step_size',
+ *     'get_global_use_powder_sensitivity',
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_all, __pyx_tuple__8) < 0) __PYX_ERR(0, 10, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_all, __pyx_tuple__9) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":12
- * __all__ = ('TrajectoryCalc',)
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":18
+ * )
  * 
  * cdef double cZeroFindingAccuracy = 0.000005             # <<<<<<<<<<<<<<
  * cdef double cMinimumVelocity = 50.0
  * cdef double cMaximumDrop = -15000
  */
   __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cZeroFindingAccuracy = 0.000005;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":13
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":19
  * 
  * cdef double cZeroFindingAccuracy = 0.000005
  * cdef double cMinimumVelocity = 50.0             # <<<<<<<<<<<<<<
  * cdef double cMaximumDrop = -15000
  * cdef int cMaxIterations = 20
  */
   __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cMinimumVelocity = 50.0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":14
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":20
  * cdef double cZeroFindingAccuracy = 0.000005
  * cdef double cMinimumVelocity = 50.0
  * cdef double cMaximumDrop = -15000             # <<<<<<<<<<<<<<
  * cdef int cMaxIterations = 20
  * cdef double cGravityConstant = -32.17405
  */
   __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cMaximumDrop = -15000.0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":15
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":21
  * cdef double cMinimumVelocity = 50.0
  * cdef double cMaximumDrop = -15000
  * cdef int cMaxIterations = 20             # <<<<<<<<<<<<<<
  * cdef double cGravityConstant = -32.17405
  * 
  */
   __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cMaxIterations = 20;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":16
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":22
  * cdef double cMaximumDrop = -15000
  * cdef int cMaxIterations = 20
  * cdef double cGravityConstant = -32.17405             # <<<<<<<<<<<<<<
  * 
- * cdef struct CurvePoint:
+ * cdef int _globalUsePowderSensitivity = False
  */
   __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cGravityConstant = -32.17405;
 
-  /* "(tree fragment)":1
- * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
- *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
- * def __setstate_cython__(self, __pyx_state):
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":24
+ * cdef double cGravityConstant = -32.17405
+ * 
+ * cdef int _globalUsePowderSensitivity = False             # <<<<<<<<<<<<<<
+ * cdef object _globalMaxCalcStepSize = Distance.Foot(0.5)
+ * 
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_6Vector_23__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Vector___reduce_cython, NULL, __pyx_n_s_py_ballisticcalc_exts_trajectory, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_v_21py_ballisticcalc_exts_15trajectory_calc__globalUsePowderSensitivity = 0;
 
-  /* "(tree fragment)":3
- * def __reduce_cython__(self):
- *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
- * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
- *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":25
+ * 
+ * cdef int _globalUsePowderSensitivity = False
+ * cdef object _globalMaxCalcStepSize = Distance.Foot(0.5)             # <<<<<<<<<<<<<<
+ * 
+ * def get_global_max_calc_step_size() -> Distance:
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_6Vector_25__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Vector___setstate_cython, NULL, __pyx_n_s_py_ballisticcalc_exts_trajectory, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Distance); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_Foot); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(1, 3, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_XGOTREF(__pyx_v_21py_ballisticcalc_exts_15trajectory_calc__globalMaxCalcStepSize);
+  __Pyx_DECREF_SET(__pyx_v_21py_ballisticcalc_exts_15trajectory_calc__globalMaxCalcStepSize, __pyx_t_2);
+  __Pyx_GIVEREF(__pyx_t_2);
+  __pyx_t_2 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":133
- *         return min(step, Settings.get_max_calc_step_size()) / 2.0
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":27
+ * cdef object _globalMaxCalcStepSize = Distance.Foot(0.5)
  * 
- *     def zero_angle(self, shot_info: Shot, distance: Distance):             # <<<<<<<<<<<<<<
- *         return self._zero_angle(shot_info, distance)
+ * def get_global_max_calc_step_size() -> Distance:             # <<<<<<<<<<<<<<
+ *     return _globalMaxCalcStepSize
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 133, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_shot_info, __pyx_n_s_Shot) < 0) __PYX_ERR(0, 133, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_distance, __pyx_n_s_Distance) < 0) __PYX_ERR(0, 133, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_3zero_angle, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_TrajectoryCalc_zero_angle, NULL, __pyx_n_s_py_ballisticcalc_exts_trajectory, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_1get_global_max_calc_step_size, NULL, __pyx_n_s_py_ballisticcalc_exts_trajectory_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc, __pyx_n_s_zero_angle, __pyx_t_2) < 0) __PYX_ERR(0, 133, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_global_max_calc_step_size, __pyx_t_2) < 0) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  PyType_Modified(__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":136
- *         return self._zero_angle(shot_info, distance)
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":31
+ * 
+ * 
+ * def get_global_use_powder_sensitivity() -> bool:             # <<<<<<<<<<<<<<
+ *     return bool(_globalUsePowderSensitivity)
  * 
- *     def trajectory(self, shot_info: Shot, max_range: Distance, dist_step: Distance,             # <<<<<<<<<<<<<<
- *                    extra_data: bool = False):
- *         cdef:
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_3get_global_use_powder_sensitivity, NULL, __pyx_n_s_py_ballisticcalc_exts_trajectory_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_shot_info, __pyx_n_s_Shot) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_max_range, __pyx_n_s_Distance) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dist_step, __pyx_n_s_Distance) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_extra_data, __pyx_n_s_bool) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_5trajectory, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_TrajectoryCalc_trajectory, NULL, __pyx_n_s_py_ballisticcalc_exts_trajectory, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 136, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__17);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_global_use_powder_sensitivit, __pyx_t_2) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc, __pyx_n_s_trajectory, __pyx_t_3) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  PyType_Modified(__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc);
 
-  /* "(tree fragment)":1
- * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
- *     cdef tuple state
- *     cdef object _dict
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":35
+ * 
+ * 
+ * def set_global_max_calc_step_size(value: [object, float]) -> None:             # <<<<<<<<<<<<<<
+ *     global _globalMaxCalcStepSize
+ *     if (_value := PreferredUnits.distance(value)).raw_value <= 0:
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_7__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_TrajectoryCalc___reduce_cython, NULL, __pyx_n_s_py_ballisticcalc_exts_trajectory, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  PyType_Modified(__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc);
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_5set_global_max_calc_step_size, NULL, __pyx_n_s_py_ballisticcalc_exts_trajectory_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_set_global_max_calc_step_size, __pyx_t_2) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "(tree fragment)":16
- *     else:
- *         return __pyx_unpickle_TrajectoryCalc, (type(self), 0x1a1505e, state)
- * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
- *     __pyx_unpickle_TrajectoryCalc__set_state(self, __pyx_state)
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":42
+ * 
+ * 
+ * def set_global_use_powder_sensitivity(value: bool) -> None:             # <<<<<<<<<<<<<<
+ *     global _globalUsePowderSensitivity
+ *     if not isinstance(value, bool):
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_9__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_TrajectoryCalc___setstate_cython, NULL, __pyx_n_s_py_ballisticcalc_exts_trajectory, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 16, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(1, 16, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  PyType_Modified(__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc);
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_7set_global_use_powder_sensitivity, NULL, __pyx_n_s_py_ballisticcalc_exts_trajectory_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_set_global_use_powder_sensitivit_2, __pyx_t_2) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":49
+ * 
+ * 
+ * def reset_globals() -> None:             # <<<<<<<<<<<<<<
+ *     global _globalUsePowderSensitivity, _globalMaxCalcStepSize
+ *     _globalUsePowderSensitivity = False
+ */
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_9reset_globals, NULL, __pyx_n_s_py_ballisticcalc_exts_trajectory_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_reset_globals, __pyx_t_2) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_TrajectoryCalc(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_1__pyx_unpickle_TrajectoryCalc, 0, __pyx_n_s_pyx_unpickle_TrajectoryCalc, NULL, __pyx_n_s_py_ballisticcalc_exts_trajectory, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_TrajectoryCalc, __pyx_t_3) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_11__pyx_unpickle_TrajectoryCalc, NULL, __pyx_n_s_py_ballisticcalc_exts_trajectory_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_TrajectoryCalc, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "py_ballisticcalc_exts/trajectory_calc.pyx":1
- * from libc.math cimport sqrt, fabs, pow, sin, cos, tan, atan, log10, floor             # <<<<<<<<<<<<<<
+ * from libc.math cimport sqrt, fabs, pow, sin, cos, tan, atan, floor             # <<<<<<<<<<<<<<
  * cimport cython
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
@@ -14831,40 +14823,14 @@
 bad:
     Py_DECREF(dict);
     return NULL;
 }
 #endif
 #endif
 
-/* RaiseArgTupleInvalid */
-static void __Pyx_RaiseArgtupleInvalid(
-    const char* func_name,
-    int exact,
-    Py_ssize_t num_min,
-    Py_ssize_t num_max,
-    Py_ssize_t num_found)
-{
-    Py_ssize_t num_expected;
-    const char *more_or_less;
-    if (num_found < num_min) {
-        num_expected = num_min;
-        more_or_less = "at least";
-    } else {
-        num_expected = num_max;
-        more_or_less = "at most";
-    }
-    if (exact) {
-        more_or_less = "exactly";
-    }
-    PyErr_Format(PyExc_TypeError,
-                 "%.200s() takes %.8s %" CYTHON_FORMAT_SSIZE_T "d positional argument%.1s (%" CYTHON_FORMAT_SSIZE_T "d given)",
-                 func_name, more_or_less, num_expected,
-                 (num_expected == 1) ? "" : "s", num_found);
-}
-
 /* RaiseDoubleKeywords */
 static void __Pyx_RaiseDoubleKeywordsError(
     const char* func_name,
     PyObject* kw_name)
 {
     PyErr_Format(PyExc_TypeError,
         #if PY_MAJOR_VERSION >= 3
@@ -15027,59 +14993,107 @@
     #endif
 bad:
     Py_XDECREF(key);
     Py_XDECREF(value);
     return -1;
 }
 
-/* ArgTypeTest */
-static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
+/* RaiseArgTupleInvalid */
+static void __Pyx_RaiseArgtupleInvalid(
+    const char* func_name,
+    int exact,
+    Py_ssize_t num_min,
+    Py_ssize_t num_max,
+    Py_ssize_t num_found)
 {
-    __Pyx_TypeName type_name;
-    __Pyx_TypeName obj_type_name;
-    if (unlikely(!type)) {
-        PyErr_SetString(PyExc_SystemError, "Missing type object");
-        return 0;
-    }
-    else if (exact) {
-        #if PY_MAJOR_VERSION == 2
-        if ((type == &PyBaseString_Type) && likely(__Pyx_PyBaseString_CheckExact(obj))) return 1;
-        #endif
+    Py_ssize_t num_expected;
+    const char *more_or_less;
+    if (num_found < num_min) {
+        num_expected = num_min;
+        more_or_less = "at least";
+    } else {
+        num_expected = num_max;
+        more_or_less = "at most";
     }
-    else {
-        if (likely(__Pyx_TypeCheck(obj, type))) return 1;
+    if (exact) {
+        more_or_less = "exactly";
     }
-    type_name = __Pyx_PyType_GetName(type);
-    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
     PyErr_Format(PyExc_TypeError,
-        "Argument '%.200s' has incorrect type (expected " __Pyx_FMT_TYPENAME
-        ", got " __Pyx_FMT_TYPENAME ")", name, type_name, obj_type_name);
-    __Pyx_DECREF_TypeName(type_name);
-    __Pyx_DECREF_TypeName(obj_type_name);
-    return 0;
+                 "%.200s() takes %.8s %" CYTHON_FORMAT_SSIZE_T "d positional argument%.1s (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                 func_name, more_or_less, num_expected,
+                 (num_expected == 1) ? "" : "s", num_found);
 }
 
-/* ExtTypeTest */
-static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
-    __Pyx_TypeName obj_type_name;
-    __Pyx_TypeName type_name;
-    if (unlikely(!type)) {
-        PyErr_SetString(PyExc_SystemError, "Missing type object");
+/* PyDictVersioning */
+#if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
+    PyObject *dict = Py_TYPE(obj)->tp_dict;
+    return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
+}
+static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj) {
+    PyObject **dictptr = NULL;
+    Py_ssize_t offset = Py_TYPE(obj)->tp_dictoffset;
+    if (offset) {
+#if CYTHON_COMPILING_IN_CPYTHON
+        dictptr = (likely(offset > 0)) ? (PyObject **) ((char *)obj + offset) : _PyObject_GetDictPtr(obj);
+#else
+        dictptr = _PyObject_GetDictPtr(obj);
+#endif
+    }
+    return (dictptr && *dictptr) ? __PYX_GET_DICT_VERSION(*dictptr) : 0;
+}
+static CYTHON_INLINE int __Pyx_object_dict_version_matches(PyObject* obj, PY_UINT64_T tp_dict_version, PY_UINT64_T obj_dict_version) {
+    PyObject *dict = Py_TYPE(obj)->tp_dict;
+    if (unlikely(!dict) || unlikely(tp_dict_version != __PYX_GET_DICT_VERSION(dict)))
         return 0;
+    return obj_dict_version == __Pyx_get_object_dict_version(obj);
+}
+#endif
+
+/* GetModuleGlobalName */
+#if CYTHON_USE_DICT_VERSIONS
+static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value)
+#else
+static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name)
+#endif
+{
+    PyObject *result;
+#if !CYTHON_AVOID_BORROWED_REFS
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && PY_VERSION_HEX < 0x030d0000
+    result = _PyDict_GetItem_KnownHash(__pyx_d, name, ((PyASCIIObject *) name)->hash);
+    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
+    if (likely(result)) {
+        return __Pyx_NewRef(result);
+    } else if (unlikely(PyErr_Occurred())) {
+        return NULL;
     }
-    if (likely(__Pyx_TypeCheck(obj, type)))
-        return 1;
-    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
-    type_name = __Pyx_PyType_GetName(type);
-    PyErr_Format(PyExc_TypeError,
-                 "Cannot convert " __Pyx_FMT_TYPENAME " to " __Pyx_FMT_TYPENAME,
-                 obj_type_name, type_name);
-    __Pyx_DECREF_TypeName(obj_type_name);
-    __Pyx_DECREF_TypeName(type_name);
-    return 0;
+#elif CYTHON_COMPILING_IN_LIMITED_API
+    if (unlikely(!__pyx_m)) {
+        return NULL;
+    }
+    result = PyObject_GetAttr(__pyx_m, name);
+    if (likely(result)) {
+        return result;
+    }
+#else
+    result = PyDict_GetItem(__pyx_d, name);
+    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
+    if (likely(result)) {
+        return __Pyx_NewRef(result);
+    }
+#endif
+#else
+    result = PyObject_GetItem(__pyx_d, name);
+    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
+    if (likely(result)) {
+        return __Pyx_NewRef(result);
+    }
+    PyErr_Clear();
+#endif
+    return __Pyx_GetBuiltinName(name);
 }
 
 /* PyFunctionFastCall */
 #if CYTHON_FAST_PYCALL && !CYTHON_VECTORCALL
 static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
                                                PyObject *globals) {
     PyFrameObject *f;
@@ -15300,20 +15314,157 @@
     #if PY_VERSION_HEX >= 0x03090000 && !CYTHON_COMPILING_IN_LIMITED_API
     return PyObject_VectorcallDict(func, args, (size_t)nargs, kwargs);
     #else
     return __Pyx_PyObject_FastCall_fallback(func, args, (size_t)nargs, kwargs);
     #endif
 }
 
+/* PyObjectFormatAndDecref */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FormatSimpleAndDecref(PyObject* s, PyObject* f) {
+    if (unlikely(!s)) return NULL;
+    if (likely(PyUnicode_CheckExact(s))) return s;
+    #if PY_MAJOR_VERSION < 3
+    if (likely(PyString_CheckExact(s))) {
+        PyObject *result = PyUnicode_FromEncodedObject(s, NULL, "strict");
+        Py_DECREF(s);
+        return result;
+    }
+    #endif
+    return __Pyx_PyObject_FormatAndDecref(s, f);
+}
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FormatAndDecref(PyObject* s, PyObject* f) {
+    PyObject *result;
+    if (unlikely(!s)) return NULL;
+    result = PyObject_Format(s, f);
+    Py_DECREF(s);
+    return result;
+}
+
+/* JoinPyUnicode */
+static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
+                                      Py_UCS4 max_char) {
+#if CYTHON_USE_UNICODE_INTERNALS && CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    PyObject *result_uval;
+    int result_ukind, kind_shift;
+    Py_ssize_t i, char_pos;
+    void *result_udata;
+    CYTHON_MAYBE_UNUSED_VAR(max_char);
+#if CYTHON_PEP393_ENABLED
+    result_uval = PyUnicode_New(result_ulength, max_char);
+    if (unlikely(!result_uval)) return NULL;
+    result_ukind = (max_char <= 255) ? PyUnicode_1BYTE_KIND : (max_char <= 65535) ? PyUnicode_2BYTE_KIND : PyUnicode_4BYTE_KIND;
+    kind_shift = (result_ukind == PyUnicode_4BYTE_KIND) ? 2 : result_ukind - 1;
+    result_udata = PyUnicode_DATA(result_uval);
+#else
+    result_uval = PyUnicode_FromUnicode(NULL, result_ulength);
+    if (unlikely(!result_uval)) return NULL;
+    result_ukind = sizeof(Py_UNICODE);
+    kind_shift = (result_ukind == 4) ? 2 : result_ukind - 1;
+    result_udata = PyUnicode_AS_UNICODE(result_uval);
+#endif
+    assert(kind_shift == 2 || kind_shift == 1 || kind_shift == 0);
+    char_pos = 0;
+    for (i=0; i < value_count; i++) {
+        int ukind;
+        Py_ssize_t ulength;
+        void *udata;
+        PyObject *uval = PyTuple_GET_ITEM(value_tuple, i);
+        if (unlikely(__Pyx_PyUnicode_READY(uval)))
+            goto bad;
+        ulength = __Pyx_PyUnicode_GET_LENGTH(uval);
+        if (unlikely(!ulength))
+            continue;
+        if (unlikely((PY_SSIZE_T_MAX >> kind_shift) - ulength < char_pos))
+            goto overflow;
+        ukind = __Pyx_PyUnicode_KIND(uval);
+        udata = __Pyx_PyUnicode_DATA(uval);
+        if (!CYTHON_PEP393_ENABLED || ukind == result_ukind) {
+            memcpy((char *)result_udata + (char_pos << kind_shift), udata, (size_t) (ulength << kind_shift));
+        } else {
+            #if PY_VERSION_HEX >= 0x030d0000
+            if (unlikely(PyUnicode_CopyCharacters(result_uval, char_pos, uval, 0, ulength) < 0)) goto bad;
+            #elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030300F0 || defined(_PyUnicode_FastCopyCharacters)
+            _PyUnicode_FastCopyCharacters(result_uval, char_pos, uval, 0, ulength);
+            #else
+            Py_ssize_t j;
+            for (j=0; j < ulength; j++) {
+                Py_UCS4 uchar = __Pyx_PyUnicode_READ(ukind, udata, j);
+                __Pyx_PyUnicode_WRITE(result_ukind, result_udata, char_pos+j, uchar);
+            }
+            #endif
+        }
+        char_pos += ulength;
+    }
+    return result_uval;
+overflow:
+    PyErr_SetString(PyExc_OverflowError, "join() result is too long for a Python string");
+bad:
+    Py_DECREF(result_uval);
+    return NULL;
+#else
+    CYTHON_UNUSED_VAR(max_char);
+    CYTHON_UNUSED_VAR(result_ulength);
+    CYTHON_UNUSED_VAR(value_count);
+    return PyUnicode_Join(__pyx_empty_unicode, value_tuple);
+#endif
+}
+
 /* PyObjectCallOneArg */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
     PyObject *args[2] = {NULL, arg};
     return __Pyx_PyObject_FastCall(func, args+1, 1 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
 }
 
+/* ArgTypeTest */
+static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
+{
+    __Pyx_TypeName type_name;
+    __Pyx_TypeName obj_type_name;
+    if (unlikely(!type)) {
+        PyErr_SetString(PyExc_SystemError, "Missing type object");
+        return 0;
+    }
+    else if (exact) {
+        #if PY_MAJOR_VERSION == 2
+        if ((type == &PyBaseString_Type) && likely(__Pyx_PyBaseString_CheckExact(obj))) return 1;
+        #endif
+    }
+    else {
+        if (likely(__Pyx_TypeCheck(obj, type))) return 1;
+    }
+    type_name = __Pyx_PyType_GetName(type);
+    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
+    PyErr_Format(PyExc_TypeError,
+        "Argument '%.200s' has incorrect type (expected " __Pyx_FMT_TYPENAME
+        ", got " __Pyx_FMT_TYPENAME ")", name, type_name, obj_type_name);
+    __Pyx_DECREF_TypeName(type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
+    return 0;
+}
+
+/* ExtTypeTest */
+static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
+    __Pyx_TypeName obj_type_name;
+    __Pyx_TypeName type_name;
+    if (unlikely(!type)) {
+        PyErr_SetString(PyExc_SystemError, "Missing type object");
+        return 0;
+    }
+    if (likely(__Pyx_TypeCheck(obj, type)))
+        return 1;
+    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
+    type_name = __Pyx_PyType_GetName(type);
+    PyErr_Format(PyExc_TypeError,
+                 "Cannot convert " __Pyx_FMT_TYPENAME " to " __Pyx_FMT_TYPENAME,
+                 obj_type_name, type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
+    __Pyx_DECREF_TypeName(type_name);
+    return 0;
+}
+
 /* KeywordStringCheck */
 static int __Pyx_CheckKeywordStrings(
     PyObject *kw,
     const char* function_name,
     int kw_allowed)
 {
     PyObject* key = 0;
@@ -15391,166 +15542,14 @@
     __Pyx_TypeName obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
     PyErr_Format(PyExc_TypeError, "Expected %s, got " __Pyx_FMT_TYPENAME,
                  expected, obj_type_name);
     __Pyx_DECREF_TypeName(obj_type_name);
     return 0;
 }
 
-/* PyFloatBinop */
-#if !CYTHON_COMPILING_IN_PYPY
-static PyObject* __Pyx_PyFloat_TrueDivideObjC(PyObject *op1, PyObject *op2, double floatval, int inplace, int zerodivision_check) {
-    const double b = floatval;
-    double a, result;
-    CYTHON_UNUSED_VAR(inplace);
-    CYTHON_UNUSED_VAR(zerodivision_check);
-    if (likely(PyFloat_CheckExact(op1))) {
-#if CYTHON_COMPILING_IN_LIMITED_API
-        a = __pyx_PyFloat_AsDouble(op1);
-#else
-        a = PyFloat_AS_DOUBLE(op1);
-#endif
-        
-    } else
-    #if PY_MAJOR_VERSION < 3
-    if (likely(PyInt_CheckExact(op1))) {
-        a = (double) PyInt_AS_LONG(op1);
-        
-    } else
-    #endif
-    if (likely(PyLong_CheckExact(op1))) {
-        #if CYTHON_USE_PYLONG_INTERNALS
-        if (__Pyx_PyLong_IsZero(op1)) {
-            a = 0.0;
-            
-        } else if (__Pyx_PyLong_IsCompact(op1)) {
-            a = (double) __Pyx_PyLong_CompactValue(op1);
-        } else {
-            const digit* digits = __Pyx_PyLong_Digits(op1);
-            const Py_ssize_t size = __Pyx_PyLong_SignedDigitCount(op1);
-            switch (size) {
-                case -2:
-                case 2:
-                    if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT && ((8 * sizeof(unsigned long) < 53) || (1 * PyLong_SHIFT < 53))) {
-                        a = (double) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        if ((8 * sizeof(unsigned long) < 53) || (2 * PyLong_SHIFT < 53) || (a < (double) ((PY_LONG_LONG)1 << 53))) {
-                            if (size == -2)
-                                a = -a;
-                            break;
-                        }
-                    }
-                    CYTHON_FALLTHROUGH;
-                case -3:
-                case 3:
-                    if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT && ((8 * sizeof(unsigned long) < 53) || (2 * PyLong_SHIFT < 53))) {
-                        a = (double) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        if ((8 * sizeof(unsigned long) < 53) || (3 * PyLong_SHIFT < 53) || (a < (double) ((PY_LONG_LONG)1 << 53))) {
-                            if (size == -3)
-                                a = -a;
-                            break;
-                        }
-                    }
-                    CYTHON_FALLTHROUGH;
-                case -4:
-                case 4:
-                    if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT && ((8 * sizeof(unsigned long) < 53) || (3 * PyLong_SHIFT < 53))) {
-                        a = (double) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        if ((8 * sizeof(unsigned long) < 53) || (4 * PyLong_SHIFT < 53) || (a < (double) ((PY_LONG_LONG)1 << 53))) {
-                            if (size == -4)
-                                a = -a;
-                            break;
-                        }
-                    }
-                    CYTHON_FALLTHROUGH;
-                default:
-        #endif
-                    a = PyLong_AsDouble(op1);
-                    if (unlikely(a == -1.0 && PyErr_Occurred())) return NULL;
-        #if CYTHON_USE_PYLONG_INTERNALS
-            }
-        }
-        #endif
-    } else {
-        return (inplace ? PyNumber_InPlaceTrueDivide : PyNumber_TrueDivide)(op1, op2);
-    }
-        PyFPE_START_PROTECT("divide", return NULL)
-        result = a / b;
-        PyFPE_END_PROTECT(result)
-        return PyFloat_FromDouble(result);
-}
-#endif
-
-/* PyDictVersioning */
-#if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
-    PyObject *dict = Py_TYPE(obj)->tp_dict;
-    return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
-}
-static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj) {
-    PyObject **dictptr = NULL;
-    Py_ssize_t offset = Py_TYPE(obj)->tp_dictoffset;
-    if (offset) {
-#if CYTHON_COMPILING_IN_CPYTHON
-        dictptr = (likely(offset > 0)) ? (PyObject **) ((char *)obj + offset) : _PyObject_GetDictPtr(obj);
-#else
-        dictptr = _PyObject_GetDictPtr(obj);
-#endif
-    }
-    return (dictptr && *dictptr) ? __PYX_GET_DICT_VERSION(*dictptr) : 0;
-}
-static CYTHON_INLINE int __Pyx_object_dict_version_matches(PyObject* obj, PY_UINT64_T tp_dict_version, PY_UINT64_T obj_dict_version) {
-    PyObject *dict = Py_TYPE(obj)->tp_dict;
-    if (unlikely(!dict) || unlikely(tp_dict_version != __PYX_GET_DICT_VERSION(dict)))
-        return 0;
-    return obj_dict_version == __Pyx_get_object_dict_version(obj);
-}
-#endif
-
-/* GetModuleGlobalName */
-#if CYTHON_USE_DICT_VERSIONS
-static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value)
-#else
-static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name)
-#endif
-{
-    PyObject *result;
-#if !CYTHON_AVOID_BORROWED_REFS
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && PY_VERSION_HEX < 0x030d0000
-    result = _PyDict_GetItem_KnownHash(__pyx_d, name, ((PyASCIIObject *) name)->hash);
-    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
-    if (likely(result)) {
-        return __Pyx_NewRef(result);
-    } else if (unlikely(PyErr_Occurred())) {
-        return NULL;
-    }
-#elif CYTHON_COMPILING_IN_LIMITED_API
-    if (unlikely(!__pyx_m)) {
-        return NULL;
-    }
-    result = PyObject_GetAttr(__pyx_m, name);
-    if (likely(result)) {
-        return result;
-    }
-#else
-    result = PyDict_GetItem(__pyx_d, name);
-    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
-    if (likely(result)) {
-        return __Pyx_NewRef(result);
-    }
-#endif
-#else
-    result = PyObject_GetItem(__pyx_d, name);
-    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
-    if (likely(result)) {
-        return __Pyx_NewRef(result);
-    }
-    PyErr_Clear();
-#endif
-    return __Pyx_GetBuiltinName(name);
-}
-
 /* GetItemInt */
 static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
     PyObject *r;
     if (unlikely(!j)) return NULL;
     r = PyObject_GetItem(o, j);
     Py_DECREF(j);
     return r;
@@ -15813,83 +15812,14 @@
     }
     if (ulength == 1) {
         return PyUnicode_FromOrdinal(*dpos);
     }
     return __Pyx_PyUnicode_BuildFromAscii(ulength, dpos, (int) length, prepend_sign, padding_char);
 }
 
-/* JoinPyUnicode */
-static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
-                                      Py_UCS4 max_char) {
-#if CYTHON_USE_UNICODE_INTERNALS && CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    PyObject *result_uval;
-    int result_ukind, kind_shift;
-    Py_ssize_t i, char_pos;
-    void *result_udata;
-    CYTHON_MAYBE_UNUSED_VAR(max_char);
-#if CYTHON_PEP393_ENABLED
-    result_uval = PyUnicode_New(result_ulength, max_char);
-    if (unlikely(!result_uval)) return NULL;
-    result_ukind = (max_char <= 255) ? PyUnicode_1BYTE_KIND : (max_char <= 65535) ? PyUnicode_2BYTE_KIND : PyUnicode_4BYTE_KIND;
-    kind_shift = (result_ukind == PyUnicode_4BYTE_KIND) ? 2 : result_ukind - 1;
-    result_udata = PyUnicode_DATA(result_uval);
-#else
-    result_uval = PyUnicode_FromUnicode(NULL, result_ulength);
-    if (unlikely(!result_uval)) return NULL;
-    result_ukind = sizeof(Py_UNICODE);
-    kind_shift = (result_ukind == 4) ? 2 : result_ukind - 1;
-    result_udata = PyUnicode_AS_UNICODE(result_uval);
-#endif
-    assert(kind_shift == 2 || kind_shift == 1 || kind_shift == 0);
-    char_pos = 0;
-    for (i=0; i < value_count; i++) {
-        int ukind;
-        Py_ssize_t ulength;
-        void *udata;
-        PyObject *uval = PyTuple_GET_ITEM(value_tuple, i);
-        if (unlikely(__Pyx_PyUnicode_READY(uval)))
-            goto bad;
-        ulength = __Pyx_PyUnicode_GET_LENGTH(uval);
-        if (unlikely(!ulength))
-            continue;
-        if (unlikely((PY_SSIZE_T_MAX >> kind_shift) - ulength < char_pos))
-            goto overflow;
-        ukind = __Pyx_PyUnicode_KIND(uval);
-        udata = __Pyx_PyUnicode_DATA(uval);
-        if (!CYTHON_PEP393_ENABLED || ukind == result_ukind) {
-            memcpy((char *)result_udata + (char_pos << kind_shift), udata, (size_t) (ulength << kind_shift));
-        } else {
-            #if PY_VERSION_HEX >= 0x030d0000
-            if (unlikely(PyUnicode_CopyCharacters(result_uval, char_pos, uval, 0, ulength) < 0)) goto bad;
-            #elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030300F0 || defined(_PyUnicode_FastCopyCharacters)
-            _PyUnicode_FastCopyCharacters(result_uval, char_pos, uval, 0, ulength);
-            #else
-            Py_ssize_t j;
-            for (j=0; j < ulength; j++) {
-                Py_UCS4 uchar = __Pyx_PyUnicode_READ(ukind, udata, j);
-                __Pyx_PyUnicode_WRITE(result_ukind, result_udata, char_pos+j, uchar);
-            }
-            #endif
-        }
-        char_pos += ulength;
-    }
-    return result_uval;
-overflow:
-    PyErr_SetString(PyExc_OverflowError, "join() result is too long for a Python string");
-bad:
-    Py_DECREF(result_uval);
-    return NULL;
-#else
-    CYTHON_UNUSED_VAR(max_char);
-    CYTHON_UNUSED_VAR(result_ulength);
-    CYTHON_UNUSED_VAR(value_count);
-    return PyUnicode_Join(__pyx_empty_unicode, value_tuple);
-#endif
-}
-
 /* PyIntBinop */
 #if !CYTHON_COMPILING_IN_PYPY
 static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check) {
     CYTHON_MAYBE_UNUSED_VAR(intval);
     CYTHON_MAYBE_UNUSED_VAR(inplace);
     CYTHON_UNUSED_VAR(zerodivision_check);
     #if PY_MAJOR_VERSION < 3
@@ -16063,114 +15993,14 @@
         Py_DECREF(retval);
         __Pyx_RaiseTooManyValuesError(expected);
         return -1;
     }
     return __Pyx_IterFinish();
 }
 
-/* RaiseUnboundLocalError */
-static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname) {
-    PyErr_Format(PyExc_UnboundLocalError, "local variable '%s' referenced before assignment", varname);
-}
-
-/* PyIntBinop */
-#if !CYTHON_COMPILING_IN_PYPY
-static PyObject* __Pyx_PyInt_TrueDivideObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check) {
-    CYTHON_MAYBE_UNUSED_VAR(intval);
-    CYTHON_MAYBE_UNUSED_VAR(inplace);
-    CYTHON_UNUSED_VAR(zerodivision_check);
-    #if PY_MAJOR_VERSION < 3
-    if (likely(PyInt_CheckExact(op1))) {
-        const long b = intval;
-        long a = PyInt_AS_LONG(op1);
-        
-            if (8 * sizeof(long) <= 53 || likely(labs(a) <= ((PY_LONG_LONG)1 << 53))) {
-                return PyFloat_FromDouble((double)a / (double)b);
-            }
-            return PyInt_Type.tp_as_number->nb_true_divide(op1, op2);
-    }
-    #endif
-    #if CYTHON_USE_PYLONG_INTERNALS
-    if (likely(PyLong_CheckExact(op1))) {
-        const long b = intval;
-        long a, x;
-        if (unlikely(__Pyx_PyLong_IsZero(op1))) {
-        }
-        if (likely(__Pyx_PyLong_IsCompact(op1))) {
-            a = __Pyx_PyLong_CompactValue(op1);
-        } else {
-            const digit* digits = __Pyx_PyLong_Digits(op1);
-            const Py_ssize_t size = __Pyx_PyLong_SignedDigitCount(op1);
-            switch (size) {
-                case -2:
-                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT && 1 * PyLong_SHIFT < 53) {
-                        a = -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    }
-                    CYTHON_FALLTHROUGH;
-                case 2:
-                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT && 1 * PyLong_SHIFT < 53) {
-                        a = (long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    }
-                    CYTHON_FALLTHROUGH;
-                case -3:
-                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT && 2 * PyLong_SHIFT < 53) {
-                        a = -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    }
-                    CYTHON_FALLTHROUGH;
-                case 3:
-                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT && 2 * PyLong_SHIFT < 53) {
-                        a = (long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    }
-                    CYTHON_FALLTHROUGH;
-                case -4:
-                    if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT && 3 * PyLong_SHIFT < 53) {
-                        a = -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    }
-                    CYTHON_FALLTHROUGH;
-                case 4:
-                    if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT && 3 * PyLong_SHIFT < 53) {
-                        a = (long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    }
-                    CYTHON_FALLTHROUGH;
-                default: return PyLong_Type.tp_as_number->nb_true_divide(op1, op2);
-            }
-        }
-                if ((8 * sizeof(long) <= 53 || likely(labs(a) <= ((PY_LONG_LONG)1 << 53)))
-                        || __Pyx_PyLong_DigitCount(op1) <= 52 / PyLong_SHIFT) {
-                    return PyFloat_FromDouble((double)a / (double)b);
-                }
-                return PyLong_Type.tp_as_number->nb_true_divide(op1, op2);
-            return PyLong_FromLong(x);
-        
-    }
-    #endif
-    if (PyFloat_CheckExact(op1)) {
-        const long b = intval;
-#if CYTHON_COMPILING_IN_LIMITED_API
-        double a = __pyx_PyFloat_AsDouble(op1);
-#else
-        double a = PyFloat_AS_DOUBLE(op1);
-#endif
-            double result;
-            
-            PyFPE_START_PROTECT("divide", return NULL)
-            result = ((double)a) / (double)b;
-            PyFPE_END_PROTECT(result)
-            return PyFloat_FromDouble(result);
-    }
-    return (inplace ? PyNumber_InPlaceTrueDivide : PyNumber_TrueDivide)(op1, op2);
-}
-#endif
-
 /* GetAttr3 */
 #if __PYX_LIMITED_VERSION_HEX < 0x030d00A1
 static PyObject *__Pyx_GetAttr3Default(PyObject *d) {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     if (unlikely(!__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
         return NULL;
@@ -16195,197 +16025,14 @@
     }
   #endif
     r = PyObject_GetAttr(o, n);
     return (likely(r)) ? r : __Pyx_GetAttr3Default(d);
 #endif
 }
 
-/* PyIntBinop */
-#if !CYTHON_COMPILING_IN_PYPY
-static PyObject* __Pyx_PyInt_SubtractObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check) {
-    CYTHON_MAYBE_UNUSED_VAR(intval);
-    CYTHON_MAYBE_UNUSED_VAR(inplace);
-    CYTHON_UNUSED_VAR(zerodivision_check);
-    #if PY_MAJOR_VERSION < 3
-    if (likely(PyInt_CheckExact(op1))) {
-        const long b = intval;
-        long x;
-        long a = PyInt_AS_LONG(op1);
-        
-            x = (long)((unsigned long)a - (unsigned long)b);
-            if (likely((x^a) >= 0 || (x^~b) >= 0))
-                return PyInt_FromLong(x);
-            return PyLong_Type.tp_as_number->nb_subtract(op1, op2);
-    }
-    #endif
-    #if CYTHON_USE_PYLONG_INTERNALS
-    if (likely(PyLong_CheckExact(op1))) {
-        const long b = intval;
-        long a, x;
-#ifdef HAVE_LONG_LONG
-        const PY_LONG_LONG llb = intval;
-        PY_LONG_LONG lla, llx;
-#endif
-        if (unlikely(__Pyx_PyLong_IsZero(op1))) {
-            return PyLong_FromLong(-intval);
-        }
-        if (likely(__Pyx_PyLong_IsCompact(op1))) {
-            a = __Pyx_PyLong_CompactValue(op1);
-        } else {
-            const digit* digits = __Pyx_PyLong_Digits(op1);
-            const Py_ssize_t size = __Pyx_PyLong_SignedDigitCount(op1);
-            switch (size) {
-                case -2:
-                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                        a = -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    #ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
-                        lla = -(PY_LONG_LONG) (((((unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-                    #endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                case 2:
-                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                        a = (long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    #ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
-                        lla = (PY_LONG_LONG) (((((unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-                    #endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                case -3:
-                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                        a = -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    #ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
-                        lla = -(PY_LONG_LONG) (((((((unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-                    #endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                case 3:
-                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                        a = (long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    #ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
-                        lla = (PY_LONG_LONG) (((((((unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-                    #endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                case -4:
-                    if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
-                        a = -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    #ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
-                        lla = -(PY_LONG_LONG) (((((((((unsigned PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-                    #endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                case 4:
-                    if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
-                        a = (long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    #ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
-                        lla = (PY_LONG_LONG) (((((((((unsigned PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-                    #endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                default: return PyLong_Type.tp_as_number->nb_subtract(op1, op2);
-            }
-        }
-                x = a - b;
-            return PyLong_FromLong(x);
-#ifdef HAVE_LONG_LONG
-        long_long:
-                llx = lla - llb;
-            return PyLong_FromLongLong(llx);
-#endif
-        
-        
-    }
-    #endif
-    if (PyFloat_CheckExact(op1)) {
-        const long b = intval;
-#if CYTHON_COMPILING_IN_LIMITED_API
-        double a = __pyx_PyFloat_AsDouble(op1);
-#else
-        double a = PyFloat_AS_DOUBLE(op1);
-#endif
-            double result;
-            
-            PyFPE_START_PROTECT("subtract", return NULL)
-            result = ((double)a) - (double)b;
-            PyFPE_END_PROTECT(result)
-            return PyFloat_FromDouble(result);
-    }
-    return (inplace ? PyNumber_InPlaceSubtract : PyNumber_Subtract)(op1, op2);
-}
-#endif
-
-/* ObjectGetItem */
-#if CYTHON_USE_TYPE_SLOTS
-static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject *index) {
-    PyObject *runerr = NULL;
-    Py_ssize_t key_value;
-    key_value = __Pyx_PyIndex_AsSsize_t(index);
-    if (likely(key_value != -1 || !(runerr = PyErr_Occurred()))) {
-        return __Pyx_GetItemInt_Fast(obj, key_value, 0, 1, 1);
-    }
-    if (PyErr_GivenExceptionMatches(runerr, PyExc_OverflowError)) {
-        __Pyx_TypeName index_type_name = __Pyx_PyType_GetName(Py_TYPE(index));
-        PyErr_Clear();
-        PyErr_Format(PyExc_IndexError,
-            "cannot fit '" __Pyx_FMT_TYPENAME "' into an index-sized integer", index_type_name);
-        __Pyx_DECREF_TypeName(index_type_name);
-    }
-    return NULL;
-}
-static PyObject *__Pyx_PyObject_GetItem_Slow(PyObject *obj, PyObject *key) {
-    __Pyx_TypeName obj_type_name;
-    if (likely(PyType_Check(obj))) {
-        PyObject *meth = __Pyx_PyObject_GetAttrStrNoError(obj, __pyx_n_s_class_getitem);
-        if (!meth) {
-            PyErr_Clear();
-        } else {
-            PyObject *result = __Pyx_PyObject_CallOneArg(meth, key);
-            Py_DECREF(meth);
-            return result;
-        }
-    }
-    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
-    PyErr_Format(PyExc_TypeError,
-        "'" __Pyx_FMT_TYPENAME "' object is not subscriptable", obj_type_name);
-    __Pyx_DECREF_TypeName(obj_type_name);
-    return NULL;
-}
-static PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject *key) {
-    PyTypeObject *tp = Py_TYPE(obj);
-    PyMappingMethods *mm = tp->tp_as_mapping;
-    PySequenceMethods *sm = tp->tp_as_sequence;
-    if (likely(mm && mm->mp_subscript)) {
-        return mm->mp_subscript(obj, key);
-    }
-    if (likely(sm && sm->sq_item)) {
-        return __Pyx_PyObject_GetIndex(obj, key);
-    }
-    return __Pyx_PyObject_GetItem_Slow(obj, key);
-}
-#endif
-
 /* Import */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
     PyObject *module = 0;
     PyObject *empty_dict = 0;
     PyObject *empty_list = 0;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_import;
@@ -16449,15 +16096,15 @@
         PyObject* module_dot = 0;
         PyObject* full_name = 0;
         PyErr_Clear();
         module_name_str = PyModule_GetName(module);
         if (unlikely(!module_name_str)) { goto modbad; }
         module_name = PyUnicode_FromString(module_name_str);
         if (unlikely(!module_name)) { goto modbad; }
-        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u__6);
+        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u__7);
         if (unlikely(!module_dot)) { goto modbad; }
         full_name = PyUnicode_Concat(module_dot, name);
         if (unlikely(!full_name)) { goto modbad; }
         #if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
         {
             PyObject *modules = PyImport_GetModuleDict();
             if (unlikely(!modules))
@@ -17129,1191 +16776,14 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
-/* FetchSharedCythonModule */
-static PyObject *__Pyx_FetchSharedCythonABIModule(void) {
-    return __Pyx_PyImport_AddModuleRef((char*) __PYX_ABI_MODULE_NAME);
-}
-
-/* FetchCommonType */
-static int __Pyx_VerifyCachedType(PyObject *cached_type,
-                               const char *name,
-                               Py_ssize_t basicsize,
-                               Py_ssize_t expected_basicsize) {
-    if (!PyType_Check(cached_type)) {
-        PyErr_Format(PyExc_TypeError,
-            "Shared Cython type %.200s is not a type object", name);
-        return -1;
-    }
-    if (basicsize != expected_basicsize) {
-        PyErr_Format(PyExc_TypeError,
-            "Shared Cython type %.200s has the wrong size, try recompiling",
-            name);
-        return -1;
-    }
-    return 0;
-}
-#if !CYTHON_USE_TYPE_SPECS
-static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type) {
-    PyObject* abi_module;
-    const char* object_name;
-    PyTypeObject *cached_type = NULL;
-    abi_module = __Pyx_FetchSharedCythonABIModule();
-    if (!abi_module) return NULL;
-    object_name = strrchr(type->tp_name, '.');
-    object_name = object_name ? object_name+1 : type->tp_name;
-    cached_type = (PyTypeObject*) PyObject_GetAttrString(abi_module, object_name);
-    if (cached_type) {
-        if (__Pyx_VerifyCachedType(
-              (PyObject *)cached_type,
-              object_name,
-              cached_type->tp_basicsize,
-              type->tp_basicsize) < 0) {
-            goto bad;
-        }
-        goto done;
-    }
-    if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
-    PyErr_Clear();
-    if (PyType_Ready(type) < 0) goto bad;
-    if (PyObject_SetAttrString(abi_module, object_name, (PyObject *)type) < 0)
-        goto bad;
-    Py_INCREF(type);
-    cached_type = type;
-done:
-    Py_DECREF(abi_module);
-    return cached_type;
-bad:
-    Py_XDECREF(cached_type);
-    cached_type = NULL;
-    goto done;
-}
-#else
-static PyTypeObject *__Pyx_FetchCommonTypeFromSpec(PyObject *module, PyType_Spec *spec, PyObject *bases) {
-    PyObject *abi_module, *cached_type = NULL;
-    const char* object_name = strrchr(spec->name, '.');
-    object_name = object_name ? object_name+1 : spec->name;
-    abi_module = __Pyx_FetchSharedCythonABIModule();
-    if (!abi_module) return NULL;
-    cached_type = PyObject_GetAttrString(abi_module, object_name);
-    if (cached_type) {
-        Py_ssize_t basicsize;
-#if CYTHON_COMPILING_IN_LIMITED_API
-        PyObject *py_basicsize;
-        py_basicsize = PyObject_GetAttrString(cached_type, "__basicsize__");
-        if (unlikely(!py_basicsize)) goto bad;
-        basicsize = PyLong_AsSsize_t(py_basicsize);
-        Py_DECREF(py_basicsize);
-        py_basicsize = 0;
-        if (unlikely(basicsize == (Py_ssize_t)-1) && PyErr_Occurred()) goto bad;
-#else
-        basicsize = likely(PyType_Check(cached_type)) ? ((PyTypeObject*) cached_type)->tp_basicsize : -1;
-#endif
-        if (__Pyx_VerifyCachedType(
-              cached_type,
-              object_name,
-              basicsize,
-              spec->basicsize) < 0) {
-            goto bad;
-        }
-        goto done;
-    }
-    if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
-    PyErr_Clear();
-    CYTHON_UNUSED_VAR(module);
-    cached_type = __Pyx_PyType_FromModuleAndSpec(abi_module, spec, bases);
-    if (unlikely(!cached_type)) goto bad;
-    if (unlikely(__Pyx_fix_up_extension_type_from_spec(spec, (PyTypeObject *) cached_type) < 0)) goto bad;
-    if (PyObject_SetAttrString(abi_module, object_name, cached_type) < 0) goto bad;
-done:
-    Py_DECREF(abi_module);
-    assert(cached_type == NULL || PyType_Check(cached_type));
-    return (PyTypeObject *) cached_type;
-bad:
-    Py_XDECREF(cached_type);
-    cached_type = NULL;
-    goto done;
-}
-#endif
-
-/* PyVectorcallFastCallDict */
-#if CYTHON_METH_FASTCALL
-static PyObject *__Pyx_PyVectorcall_FastCallDict_kw(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw)
-{
-    PyObject *res = NULL;
-    PyObject *kwnames;
-    PyObject **newargs;
-    PyObject **kwvalues;
-    Py_ssize_t i, pos;
-    size_t j;
-    PyObject *key, *value;
-    unsigned long keys_are_strings;
-    Py_ssize_t nkw = PyDict_GET_SIZE(kw);
-    newargs = (PyObject **)PyMem_Malloc((nargs + (size_t)nkw) * sizeof(args[0]));
-    if (unlikely(newargs == NULL)) {
-        PyErr_NoMemory();
-        return NULL;
-    }
-    for (j = 0; j < nargs; j++) newargs[j] = args[j];
-    kwnames = PyTuple_New(nkw);
-    if (unlikely(kwnames == NULL)) {
-        PyMem_Free(newargs);
-        return NULL;
-    }
-    kwvalues = newargs + nargs;
-    pos = i = 0;
-    keys_are_strings = Py_TPFLAGS_UNICODE_SUBCLASS;
-    while (PyDict_Next(kw, &pos, &key, &value)) {
-        keys_are_strings &= Py_TYPE(key)->tp_flags;
-        Py_INCREF(key);
-        Py_INCREF(value);
-        PyTuple_SET_ITEM(kwnames, i, key);
-        kwvalues[i] = value;
-        i++;
-    }
-    if (unlikely(!keys_are_strings)) {
-        PyErr_SetString(PyExc_TypeError, "keywords must be strings");
-        goto cleanup;
-    }
-    res = vc(func, newargs, nargs, kwnames);
-cleanup:
-    Py_DECREF(kwnames);
-    for (i = 0; i < nkw; i++)
-        Py_DECREF(kwvalues[i]);
-    PyMem_Free(newargs);
-    return res;
-}
-static CYTHON_INLINE PyObject *__Pyx_PyVectorcall_FastCallDict(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw)
-{
-    if (likely(kw == NULL) || PyDict_GET_SIZE(kw) == 0) {
-        return vc(func, args, nargs, NULL);
-    }
-    return __Pyx_PyVectorcall_FastCallDict_kw(func, vc, args, nargs, kw);
-}
-#endif
-
-/* CythonFunctionShared */
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE int __Pyx__IsSameCyOrCFunction(PyObject *func, void *cfunc) {
-    if (__Pyx_CyFunction_Check(func)) {
-        return PyCFunction_GetFunction(((__pyx_CyFunctionObject*)func)->func) == (PyCFunction) cfunc;
-    } else if (PyCFunction_Check(func)) {
-        return PyCFunction_GetFunction(func) == (PyCFunction) cfunc;
-    }
-    return 0;
-}
-#else
-static CYTHON_INLINE int __Pyx__IsSameCyOrCFunction(PyObject *func, void *cfunc) {
-    return __Pyx_CyOrPyCFunction_Check(func) && __Pyx_CyOrPyCFunction_GET_FUNCTION(func) == (PyCFunction) cfunc;
-}
-#endif
-static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj) {
-#if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
-    __Pyx_Py_XDECREF_SET(
-        __Pyx_CyFunction_GetClassObj(f),
-            ((classobj) ? __Pyx_NewRef(classobj) : NULL));
-#else
-    __Pyx_Py_XDECREF_SET(
-        ((PyCMethodObject *) (f))->mm_class,
-        (PyTypeObject*)((classobj) ? __Pyx_NewRef(classobj) : NULL));
-#endif
-}
-static PyObject *
-__Pyx_CyFunction_get_doc(__pyx_CyFunctionObject *op, void *closure)
-{
-    CYTHON_UNUSED_VAR(closure);
-    if (unlikely(op->func_doc == NULL)) {
-#if CYTHON_COMPILING_IN_LIMITED_API
-        op->func_doc = PyObject_GetAttrString(op->func, "__doc__");
-        if (unlikely(!op->func_doc)) return NULL;
-#else
-        if (((PyCFunctionObject*)op)->m_ml->ml_doc) {
-#if PY_MAJOR_VERSION >= 3
-            op->func_doc = PyUnicode_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
-#else
-            op->func_doc = PyString_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
-#endif
-            if (unlikely(op->func_doc == NULL))
-                return NULL;
-        } else {
-            Py_INCREF(Py_None);
-            return Py_None;
-        }
-#endif
-    }
-    Py_INCREF(op->func_doc);
-    return op->func_doc;
-}
-static int
-__Pyx_CyFunction_set_doc(__pyx_CyFunctionObject *op, PyObject *value, void *context)
-{
-    CYTHON_UNUSED_VAR(context);
-    if (value == NULL) {
-        value = Py_None;
-    }
-    Py_INCREF(value);
-    __Pyx_Py_XDECREF_SET(op->func_doc, value);
-    return 0;
-}
-static PyObject *
-__Pyx_CyFunction_get_name(__pyx_CyFunctionObject *op, void *context)
-{
-    CYTHON_UNUSED_VAR(context);
-    if (unlikely(op->func_name == NULL)) {
-#if CYTHON_COMPILING_IN_LIMITED_API
-        op->func_name = PyObject_GetAttrString(op->func, "__name__");
-#elif PY_MAJOR_VERSION >= 3
-        op->func_name = PyUnicode_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
-#else
-        op->func_name = PyString_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
-#endif
-        if (unlikely(op->func_name == NULL))
-            return NULL;
-    }
-    Py_INCREF(op->func_name);
-    return op->func_name;
-}
-static int
-__Pyx_CyFunction_set_name(__pyx_CyFunctionObject *op, PyObject *value, void *context)
-{
-    CYTHON_UNUSED_VAR(context);
-#if PY_MAJOR_VERSION >= 3
-    if (unlikely(value == NULL || !PyUnicode_Check(value)))
-#else
-    if (unlikely(value == NULL || !PyString_Check(value)))
-#endif
-    {
-        PyErr_SetString(PyExc_TypeError,
-                        "__name__ must be set to a string object");
-        return -1;
-    }
-    Py_INCREF(value);
-    __Pyx_Py_XDECREF_SET(op->func_name, value);
-    return 0;
-}
-static PyObject *
-__Pyx_CyFunction_get_qualname(__pyx_CyFunctionObject *op, void *context)
-{
-    CYTHON_UNUSED_VAR(context);
-    Py_INCREF(op->func_qualname);
-    return op->func_qualname;
-}
-static int
-__Pyx_CyFunction_set_qualname(__pyx_CyFunctionObject *op, PyObject *value, void *context)
-{
-    CYTHON_UNUSED_VAR(context);
-#if PY_MAJOR_VERSION >= 3
-    if (unlikely(value == NULL || !PyUnicode_Check(value)))
-#else
-    if (unlikely(value == NULL || !PyString_Check(value)))
-#endif
-    {
-        PyErr_SetString(PyExc_TypeError,
-                        "__qualname__ must be set to a string object");
-        return -1;
-    }
-    Py_INCREF(value);
-    __Pyx_Py_XDECREF_SET(op->func_qualname, value);
-    return 0;
-}
-static PyObject *
-__Pyx_CyFunction_get_dict(__pyx_CyFunctionObject *op, void *context)
-{
-    CYTHON_UNUSED_VAR(context);
-    if (unlikely(op->func_dict == NULL)) {
-        op->func_dict = PyDict_New();
-        if (unlikely(op->func_dict == NULL))
-            return NULL;
-    }
-    Py_INCREF(op->func_dict);
-    return op->func_dict;
-}
-static int
-__Pyx_CyFunction_set_dict(__pyx_CyFunctionObject *op, PyObject *value, void *context)
-{
-    CYTHON_UNUSED_VAR(context);
-    if (unlikely(value == NULL)) {
-        PyErr_SetString(PyExc_TypeError,
-               "function's dictionary may not be deleted");
-        return -1;
-    }
-    if (unlikely(!PyDict_Check(value))) {
-        PyErr_SetString(PyExc_TypeError,
-               "setting function's dictionary to a non-dict");
-        return -1;
-    }
-    Py_INCREF(value);
-    __Pyx_Py_XDECREF_SET(op->func_dict, value);
-    return 0;
-}
-static PyObject *
-__Pyx_CyFunction_get_globals(__pyx_CyFunctionObject *op, void *context)
-{
-    CYTHON_UNUSED_VAR(context);
-    Py_INCREF(op->func_globals);
-    return op->func_globals;
-}
-static PyObject *
-__Pyx_CyFunction_get_closure(__pyx_CyFunctionObject *op, void *context)
-{
-    CYTHON_UNUSED_VAR(op);
-    CYTHON_UNUSED_VAR(context);
-    Py_INCREF(Py_None);
-    return Py_None;
-}
-static PyObject *
-__Pyx_CyFunction_get_code(__pyx_CyFunctionObject *op, void *context)
-{
-    PyObject* result = (op->func_code) ? op->func_code : Py_None;
-    CYTHON_UNUSED_VAR(context);
-    Py_INCREF(result);
-    return result;
-}
-static int
-__Pyx_CyFunction_init_defaults(__pyx_CyFunctionObject *op) {
-    int result = 0;
-    PyObject *res = op->defaults_getter((PyObject *) op);
-    if (unlikely(!res))
-        return -1;
-    #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    op->defaults_tuple = PyTuple_GET_ITEM(res, 0);
-    Py_INCREF(op->defaults_tuple);
-    op->defaults_kwdict = PyTuple_GET_ITEM(res, 1);
-    Py_INCREF(op->defaults_kwdict);
-    #else
-    op->defaults_tuple = __Pyx_PySequence_ITEM(res, 0);
-    if (unlikely(!op->defaults_tuple)) result = -1;
-    else {
-        op->defaults_kwdict = __Pyx_PySequence_ITEM(res, 1);
-        if (unlikely(!op->defaults_kwdict)) result = -1;
-    }
-    #endif
-    Py_DECREF(res);
-    return result;
-}
-static int
-__Pyx_CyFunction_set_defaults(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
-    CYTHON_UNUSED_VAR(context);
-    if (!value) {
-        value = Py_None;
-    } else if (unlikely(value != Py_None && !PyTuple_Check(value))) {
-        PyErr_SetString(PyExc_TypeError,
-                        "__defaults__ must be set to a tuple object");
-        return -1;
-    }
-    PyErr_WarnEx(PyExc_RuntimeWarning, "changes to cyfunction.__defaults__ will not "
-                 "currently affect the values used in function calls", 1);
-    Py_INCREF(value);
-    __Pyx_Py_XDECREF_SET(op->defaults_tuple, value);
-    return 0;
-}
-static PyObject *
-__Pyx_CyFunction_get_defaults(__pyx_CyFunctionObject *op, void *context) {
-    PyObject* result = op->defaults_tuple;
-    CYTHON_UNUSED_VAR(context);
-    if (unlikely(!result)) {
-        if (op->defaults_getter) {
-            if (unlikely(__Pyx_CyFunction_init_defaults(op) < 0)) return NULL;
-            result = op->defaults_tuple;
-        } else {
-            result = Py_None;
-        }
-    }
-    Py_INCREF(result);
-    return result;
-}
-static int
-__Pyx_CyFunction_set_kwdefaults(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
-    CYTHON_UNUSED_VAR(context);
-    if (!value) {
-        value = Py_None;
-    } else if (unlikely(value != Py_None && !PyDict_Check(value))) {
-        PyErr_SetString(PyExc_TypeError,
-                        "__kwdefaults__ must be set to a dict object");
-        return -1;
-    }
-    PyErr_WarnEx(PyExc_RuntimeWarning, "changes to cyfunction.__kwdefaults__ will not "
-                 "currently affect the values used in function calls", 1);
-    Py_INCREF(value);
-    __Pyx_Py_XDECREF_SET(op->defaults_kwdict, value);
-    return 0;
-}
-static PyObject *
-__Pyx_CyFunction_get_kwdefaults(__pyx_CyFunctionObject *op, void *context) {
-    PyObject* result = op->defaults_kwdict;
-    CYTHON_UNUSED_VAR(context);
-    if (unlikely(!result)) {
-        if (op->defaults_getter) {
-            if (unlikely(__Pyx_CyFunction_init_defaults(op) < 0)) return NULL;
-            result = op->defaults_kwdict;
-        } else {
-            result = Py_None;
-        }
-    }
-    Py_INCREF(result);
-    return result;
-}
-static int
-__Pyx_CyFunction_set_annotations(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
-    CYTHON_UNUSED_VAR(context);
-    if (!value || value == Py_None) {
-        value = NULL;
-    } else if (unlikely(!PyDict_Check(value))) {
-        PyErr_SetString(PyExc_TypeError,
-                        "__annotations__ must be set to a dict object");
-        return -1;
-    }
-    Py_XINCREF(value);
-    __Pyx_Py_XDECREF_SET(op->func_annotations, value);
-    return 0;
-}
-static PyObject *
-__Pyx_CyFunction_get_annotations(__pyx_CyFunctionObject *op, void *context) {
-    PyObject* result = op->func_annotations;
-    CYTHON_UNUSED_VAR(context);
-    if (unlikely(!result)) {
-        result = PyDict_New();
-        if (unlikely(!result)) return NULL;
-        op->func_annotations = result;
-    }
-    Py_INCREF(result);
-    return result;
-}
-static PyObject *
-__Pyx_CyFunction_get_is_coroutine(__pyx_CyFunctionObject *op, void *context) {
-    int is_coroutine;
-    CYTHON_UNUSED_VAR(context);
-    if (op->func_is_coroutine) {
-        return __Pyx_NewRef(op->func_is_coroutine);
-    }
-    is_coroutine = op->flags & __Pyx_CYFUNCTION_COROUTINE;
-#if PY_VERSION_HEX >= 0x03050000
-    if (is_coroutine) {
-        PyObject *module, *fromlist, *marker = __pyx_n_s_is_coroutine;
-        fromlist = PyList_New(1);
-        if (unlikely(!fromlist)) return NULL;
-        Py_INCREF(marker);
-#if CYTHON_ASSUME_SAFE_MACROS
-        PyList_SET_ITEM(fromlist, 0, marker);
-#else
-        if (unlikely(PyList_SetItem(fromlist, 0, marker) < 0)) {
-            Py_DECREF(marker);
-            Py_DECREF(fromlist);
-            return NULL;
-        }
-#endif
-        module = PyImport_ImportModuleLevelObject(__pyx_n_s_asyncio_coroutines, NULL, NULL, fromlist, 0);
-        Py_DECREF(fromlist);
-        if (unlikely(!module)) goto ignore;
-        op->func_is_coroutine = __Pyx_PyObject_GetAttrStr(module, marker);
-        Py_DECREF(module);
-        if (likely(op->func_is_coroutine)) {
-            return __Pyx_NewRef(op->func_is_coroutine);
-        }
-ignore:
-        PyErr_Clear();
-    }
-#endif
-    op->func_is_coroutine = __Pyx_PyBool_FromLong(is_coroutine);
-    return __Pyx_NewRef(op->func_is_coroutine);
-}
-#if CYTHON_COMPILING_IN_LIMITED_API
-static PyObject *
-__Pyx_CyFunction_get_module(__pyx_CyFunctionObject *op, void *context) {
-    CYTHON_UNUSED_VAR(context);
-    return PyObject_GetAttrString(op->func, "__module__");
-}
-static int
-__Pyx_CyFunction_set_module(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
-    CYTHON_UNUSED_VAR(context);
-    return PyObject_SetAttrString(op->func, "__module__", value);
-}
-#endif
-static PyGetSetDef __pyx_CyFunction_getsets[] = {
-    {(char *) "func_doc", (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
-    {(char *) "__doc__",  (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
-    {(char *) "func_name", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
-    {(char *) "__name__", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
-    {(char *) "__qualname__", (getter)__Pyx_CyFunction_get_qualname, (setter)__Pyx_CyFunction_set_qualname, 0, 0},
-    {(char *) "func_dict", (getter)__Pyx_CyFunction_get_dict, (setter)__Pyx_CyFunction_set_dict, 0, 0},
-    {(char *) "__dict__", (getter)__Pyx_CyFunction_get_dict, (setter)__Pyx_CyFunction_set_dict, 0, 0},
-    {(char *) "func_globals", (getter)__Pyx_CyFunction_get_globals, 0, 0, 0},
-    {(char *) "__globals__", (getter)__Pyx_CyFunction_get_globals, 0, 0, 0},
-    {(char *) "func_closure", (getter)__Pyx_CyFunction_get_closure, 0, 0, 0},
-    {(char *) "__closure__", (getter)__Pyx_CyFunction_get_closure, 0, 0, 0},
-    {(char *) "func_code", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
-    {(char *) "__code__", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
-    {(char *) "func_defaults", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
-    {(char *) "__defaults__", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
-    {(char *) "__kwdefaults__", (getter)__Pyx_CyFunction_get_kwdefaults, (setter)__Pyx_CyFunction_set_kwdefaults, 0, 0},
-    {(char *) "__annotations__", (getter)__Pyx_CyFunction_get_annotations, (setter)__Pyx_CyFunction_set_annotations, 0, 0},
-    {(char *) "_is_coroutine", (getter)__Pyx_CyFunction_get_is_coroutine, 0, 0, 0},
-#if CYTHON_COMPILING_IN_LIMITED_API
-    {"__module__", (getter)__Pyx_CyFunction_get_module, (setter)__Pyx_CyFunction_set_module, 0, 0},
-#endif
-    {0, 0, 0, 0, 0}
-};
-static PyMemberDef __pyx_CyFunction_members[] = {
-#if !CYTHON_COMPILING_IN_LIMITED_API
-    {(char *) "__module__", T_OBJECT, offsetof(PyCFunctionObject, m_module), 0, 0},
-#endif
-#if CYTHON_USE_TYPE_SPECS
-    {(char *) "__dictoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_dict), READONLY, 0},
-#if CYTHON_METH_FASTCALL
-#if CYTHON_BACKPORT_VECTORCALL
-    {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_vectorcall), READONLY, 0},
-#else
-#if !CYTHON_COMPILING_IN_LIMITED_API
-    {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(PyCFunctionObject, vectorcall), READONLY, 0},
-#endif
-#endif
-#endif
-#if PY_VERSION_HEX < 0x030500A0 || CYTHON_COMPILING_IN_LIMITED_API
-    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_weakreflist), READONLY, 0},
-#else
-    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(PyCFunctionObject, m_weakreflist), READONLY, 0},
-#endif
-#endif
-    {0, 0, 0,  0, 0}
-};
-static PyObject *
-__Pyx_CyFunction_reduce(__pyx_CyFunctionObject *m, PyObject *args)
-{
-    CYTHON_UNUSED_VAR(args);
-#if PY_MAJOR_VERSION >= 3
-    Py_INCREF(m->func_qualname);
-    return m->func_qualname;
-#else
-    return PyString_FromString(((PyCFunctionObject*)m)->m_ml->ml_name);
-#endif
-}
-static PyMethodDef __pyx_CyFunction_methods[] = {
-    {"__reduce__", (PyCFunction)__Pyx_CyFunction_reduce, METH_VARARGS, 0},
-    {0, 0, 0, 0}
-};
-#if PY_VERSION_HEX < 0x030500A0 || CYTHON_COMPILING_IN_LIMITED_API
-#define __Pyx_CyFunction_weakreflist(cyfunc) ((cyfunc)->func_weakreflist)
-#else
-#define __Pyx_CyFunction_weakreflist(cyfunc) (((PyCFunctionObject*)cyfunc)->m_weakreflist)
-#endif
-static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject *op, PyMethodDef *ml, int flags, PyObject* qualname,
-                                       PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
-#if !CYTHON_COMPILING_IN_LIMITED_API
-    PyCFunctionObject *cf = (PyCFunctionObject*) op;
-#endif
-    if (unlikely(op == NULL))
-        return NULL;
-#if CYTHON_COMPILING_IN_LIMITED_API
-    op->func = PyCFunction_NewEx(ml, (PyObject*)op, module);
-    if (unlikely(!op->func)) return NULL;
-#endif
-    op->flags = flags;
-    __Pyx_CyFunction_weakreflist(op) = NULL;
-#if !CYTHON_COMPILING_IN_LIMITED_API
-    cf->m_ml = ml;
-    cf->m_self = (PyObject *) op;
-#endif
-    Py_XINCREF(closure);
-    op->func_closure = closure;
-#if !CYTHON_COMPILING_IN_LIMITED_API
-    Py_XINCREF(module);
-    cf->m_module = module;
-#endif
-    op->func_dict = NULL;
-    op->func_name = NULL;
-    Py_INCREF(qualname);
-    op->func_qualname = qualname;
-    op->func_doc = NULL;
-#if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
-    op->func_classobj = NULL;
-#else
-    ((PyCMethodObject*)op)->mm_class = NULL;
-#endif
-    op->func_globals = globals;
-    Py_INCREF(op->func_globals);
-    Py_XINCREF(code);
-    op->func_code = code;
-    op->defaults_pyobjects = 0;
-    op->defaults_size = 0;
-    op->defaults = NULL;
-    op->defaults_tuple = NULL;
-    op->defaults_kwdict = NULL;
-    op->defaults_getter = NULL;
-    op->func_annotations = NULL;
-    op->func_is_coroutine = NULL;
-#if CYTHON_METH_FASTCALL
-    switch (ml->ml_flags & (METH_VARARGS | METH_FASTCALL | METH_NOARGS | METH_O | METH_KEYWORDS | METH_METHOD)) {
-    case METH_NOARGS:
-        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_NOARGS;
-        break;
-    case METH_O:
-        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_O;
-        break;
-    case METH_METHOD | METH_FASTCALL | METH_KEYWORDS:
-        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD;
-        break;
-    case METH_FASTCALL | METH_KEYWORDS:
-        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS;
-        break;
-    case METH_VARARGS | METH_KEYWORDS:
-        __Pyx_CyFunction_func_vectorcall(op) = NULL;
-        break;
-    default:
-        PyErr_SetString(PyExc_SystemError, "Bad call flags for CyFunction");
-        Py_DECREF(op);
-        return NULL;
-    }
-#endif
-    return (PyObject *) op;
-}
-static int
-__Pyx_CyFunction_clear(__pyx_CyFunctionObject *m)
-{
-    Py_CLEAR(m->func_closure);
-#if CYTHON_COMPILING_IN_LIMITED_API
-    Py_CLEAR(m->func);
-#else
-    Py_CLEAR(((PyCFunctionObject*)m)->m_module);
-#endif
-    Py_CLEAR(m->func_dict);
-    Py_CLEAR(m->func_name);
-    Py_CLEAR(m->func_qualname);
-    Py_CLEAR(m->func_doc);
-    Py_CLEAR(m->func_globals);
-    Py_CLEAR(m->func_code);
-#if !CYTHON_COMPILING_IN_LIMITED_API
-#if PY_VERSION_HEX < 0x030900B1
-    Py_CLEAR(__Pyx_CyFunction_GetClassObj(m));
-#else
-    {
-        PyObject *cls = (PyObject*) ((PyCMethodObject *) (m))->mm_class;
-        ((PyCMethodObject *) (m))->mm_class = NULL;
-        Py_XDECREF(cls);
-    }
-#endif
-#endif
-    Py_CLEAR(m->defaults_tuple);
-    Py_CLEAR(m->defaults_kwdict);
-    Py_CLEAR(m->func_annotations);
-    Py_CLEAR(m->func_is_coroutine);
-    if (m->defaults) {
-        PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
-        int i;
-        for (i = 0; i < m->defaults_pyobjects; i++)
-            Py_XDECREF(pydefaults[i]);
-        PyObject_Free(m->defaults);
-        m->defaults = NULL;
-    }
-    return 0;
-}
-static void __Pyx__CyFunction_dealloc(__pyx_CyFunctionObject *m)
-{
-    if (__Pyx_CyFunction_weakreflist(m) != NULL)
-        PyObject_ClearWeakRefs((PyObject *) m);
-    __Pyx_CyFunction_clear(m);
-    __Pyx_PyHeapTypeObject_GC_Del(m);
-}
-static void __Pyx_CyFunction_dealloc(__pyx_CyFunctionObject *m)
-{
-    PyObject_GC_UnTrack(m);
-    __Pyx__CyFunction_dealloc(m);
-}
-static int __Pyx_CyFunction_traverse(__pyx_CyFunctionObject *m, visitproc visit, void *arg)
-{
-    Py_VISIT(m->func_closure);
-#if CYTHON_COMPILING_IN_LIMITED_API
-    Py_VISIT(m->func);
-#else
-    Py_VISIT(((PyCFunctionObject*)m)->m_module);
-#endif
-    Py_VISIT(m->func_dict);
-    Py_VISIT(m->func_name);
-    Py_VISIT(m->func_qualname);
-    Py_VISIT(m->func_doc);
-    Py_VISIT(m->func_globals);
-    Py_VISIT(m->func_code);
-#if !CYTHON_COMPILING_IN_LIMITED_API
-    Py_VISIT(__Pyx_CyFunction_GetClassObj(m));
-#endif
-    Py_VISIT(m->defaults_tuple);
-    Py_VISIT(m->defaults_kwdict);
-    Py_VISIT(m->func_is_coroutine);
-    if (m->defaults) {
-        PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
-        int i;
-        for (i = 0; i < m->defaults_pyobjects; i++)
-            Py_VISIT(pydefaults[i]);
-    }
-    return 0;
-}
-static PyObject*
-__Pyx_CyFunction_repr(__pyx_CyFunctionObject *op)
-{
-#if PY_MAJOR_VERSION >= 3
-    return PyUnicode_FromFormat("<cyfunction %U at %p>",
-                                op->func_qualname, (void *)op);
-#else
-    return PyString_FromFormat("<cyfunction %s at %p>",
-                               PyString_AsString(op->func_qualname), (void *)op);
-#endif
-}
-static PyObject * __Pyx_CyFunction_CallMethod(PyObject *func, PyObject *self, PyObject *arg, PyObject *kw) {
-#if CYTHON_COMPILING_IN_LIMITED_API
-    PyObject *f = ((__pyx_CyFunctionObject*)func)->func;
-    PyObject *py_name = NULL;
-    PyCFunction meth;
-    int flags;
-    meth = PyCFunction_GetFunction(f);
-    if (unlikely(!meth)) return NULL;
-    flags = PyCFunction_GetFlags(f);
-    if (unlikely(flags < 0)) return NULL;
-#else
-    PyCFunctionObject* f = (PyCFunctionObject*)func;
-    PyCFunction meth = f->m_ml->ml_meth;
-    int flags = f->m_ml->ml_flags;
-#endif
-    Py_ssize_t size;
-    switch (flags & (METH_VARARGS | METH_KEYWORDS | METH_NOARGS | METH_O)) {
-    case METH_VARARGS:
-        if (likely(kw == NULL || PyDict_Size(kw) == 0))
-            return (*meth)(self, arg);
-        break;
-    case METH_VARARGS | METH_KEYWORDS:
-        return (*(PyCFunctionWithKeywords)(void*)meth)(self, arg, kw);
-    case METH_NOARGS:
-        if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
-#if CYTHON_ASSUME_SAFE_MACROS
-            size = PyTuple_GET_SIZE(arg);
-#else
-            size = PyTuple_Size(arg);
-            if (unlikely(size < 0)) return NULL;
-#endif
-            if (likely(size == 0))
-                return (*meth)(self, NULL);
-#if CYTHON_COMPILING_IN_LIMITED_API
-            py_name = __Pyx_CyFunction_get_name((__pyx_CyFunctionObject*)func, NULL);
-            if (!py_name) return NULL;
-            PyErr_Format(PyExc_TypeError,
-                "%.200S() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
-                py_name, size);
-            Py_DECREF(py_name);
-#else
-            PyErr_Format(PyExc_TypeError,
-                "%.200s() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
-                f->m_ml->ml_name, size);
-#endif
-            return NULL;
-        }
-        break;
-    case METH_O:
-        if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
-#if CYTHON_ASSUME_SAFE_MACROS
-            size = PyTuple_GET_SIZE(arg);
-#else
-            size = PyTuple_Size(arg);
-            if (unlikely(size < 0)) return NULL;
-#endif
-            if (likely(size == 1)) {
-                PyObject *result, *arg0;
-                #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-                arg0 = PyTuple_GET_ITEM(arg, 0);
-                #else
-                arg0 = __Pyx_PySequence_ITEM(arg, 0); if (unlikely(!arg0)) return NULL;
-                #endif
-                result = (*meth)(self, arg0);
-                #if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
-                Py_DECREF(arg0);
-                #endif
-                return result;
-            }
-#if CYTHON_COMPILING_IN_LIMITED_API
-            py_name = __Pyx_CyFunction_get_name((__pyx_CyFunctionObject*)func, NULL);
-            if (!py_name) return NULL;
-            PyErr_Format(PyExc_TypeError,
-                "%.200S() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
-                py_name, size);
-            Py_DECREF(py_name);
-#else
-            PyErr_Format(PyExc_TypeError,
-                "%.200s() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
-                f->m_ml->ml_name, size);
-#endif
-            return NULL;
-        }
-        break;
-    default:
-        PyErr_SetString(PyExc_SystemError, "Bad call flags for CyFunction");
-        return NULL;
-    }
-#if CYTHON_COMPILING_IN_LIMITED_API
-    py_name = __Pyx_CyFunction_get_name((__pyx_CyFunctionObject*)func, NULL);
-    if (!py_name) return NULL;
-    PyErr_Format(PyExc_TypeError, "%.200S() takes no keyword arguments",
-                 py_name);
-    Py_DECREF(py_name);
-#else
-    PyErr_Format(PyExc_TypeError, "%.200s() takes no keyword arguments",
-                 f->m_ml->ml_name);
-#endif
-    return NULL;
-}
-static CYTHON_INLINE PyObject *__Pyx_CyFunction_Call(PyObject *func, PyObject *arg, PyObject *kw) {
-    PyObject *self, *result;
-#if CYTHON_COMPILING_IN_LIMITED_API
-    self = PyCFunction_GetSelf(((__pyx_CyFunctionObject*)func)->func);
-    if (unlikely(!self) && PyErr_Occurred()) return NULL;
-#else
-    self = ((PyCFunctionObject*)func)->m_self;
-#endif
-    result = __Pyx_CyFunction_CallMethod(func, self, arg, kw);
-    return result;
-}
-static PyObject *__Pyx_CyFunction_CallAsMethod(PyObject *func, PyObject *args, PyObject *kw) {
-    PyObject *result;
-    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *) func;
-#if CYTHON_METH_FASTCALL
-     __pyx_vectorcallfunc vc = __Pyx_CyFunction_func_vectorcall(cyfunc);
-    if (vc) {
-#if CYTHON_ASSUME_SAFE_MACROS
-        return __Pyx_PyVectorcall_FastCallDict(func, vc, &PyTuple_GET_ITEM(args, 0), (size_t)PyTuple_GET_SIZE(args), kw);
-#else
-        (void) &__Pyx_PyVectorcall_FastCallDict;
-        return PyVectorcall_Call(func, args, kw);
-#endif
-    }
-#endif
-    if ((cyfunc->flags & __Pyx_CYFUNCTION_CCLASS) && !(cyfunc->flags & __Pyx_CYFUNCTION_STATICMETHOD)) {
-        Py_ssize_t argc;
-        PyObject *new_args;
-        PyObject *self;
-#if CYTHON_ASSUME_SAFE_MACROS
-        argc = PyTuple_GET_SIZE(args);
-#else
-        argc = PyTuple_Size(args);
-        if (unlikely(!argc) < 0) return NULL;
-#endif
-        new_args = PyTuple_GetSlice(args, 1, argc);
-        if (unlikely(!new_args))
-            return NULL;
-        self = PyTuple_GetItem(args, 0);
-        if (unlikely(!self)) {
-            Py_DECREF(new_args);
-#if PY_MAJOR_VERSION > 2
-            PyErr_Format(PyExc_TypeError,
-                         "unbound method %.200S() needs an argument",
-                         cyfunc->func_qualname);
-#else
-            PyErr_SetString(PyExc_TypeError,
-                            "unbound method needs an argument");
-#endif
-            return NULL;
-        }
-        result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
-        Py_DECREF(new_args);
-    } else {
-        result = __Pyx_CyFunction_Call(func, args, kw);
-    }
-    return result;
-}
-#if CYTHON_METH_FASTCALL
-static CYTHON_INLINE int __Pyx_CyFunction_Vectorcall_CheckArgs(__pyx_CyFunctionObject *cyfunc, Py_ssize_t nargs, PyObject *kwnames)
-{
-    int ret = 0;
-    if ((cyfunc->flags & __Pyx_CYFUNCTION_CCLASS) && !(cyfunc->flags & __Pyx_CYFUNCTION_STATICMETHOD)) {
-        if (unlikely(nargs < 1)) {
-            PyErr_Format(PyExc_TypeError, "%.200s() needs an argument",
-                         ((PyCFunctionObject*)cyfunc)->m_ml->ml_name);
-            return -1;
-        }
-        ret = 1;
-    }
-    if (unlikely(kwnames) && unlikely(PyTuple_GET_SIZE(kwnames))) {
-        PyErr_Format(PyExc_TypeError,
-                     "%.200s() takes no keyword arguments", ((PyCFunctionObject*)cyfunc)->m_ml->ml_name);
-        return -1;
-    }
-    return ret;
-}
-static PyObject * __Pyx_CyFunction_Vectorcall_NOARGS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
-{
-    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
-    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
-#if CYTHON_BACKPORT_VECTORCALL
-    Py_ssize_t nargs = (Py_ssize_t)nargsf;
-#else
-    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
-#endif
-    PyObject *self;
-    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, kwnames)) {
-    case 1:
-        self = args[0];
-        args += 1;
-        nargs -= 1;
-        break;
-    case 0:
-        self = ((PyCFunctionObject*)cyfunc)->m_self;
-        break;
-    default:
-        return NULL;
-    }
-    if (unlikely(nargs != 0)) {
-        PyErr_Format(PyExc_TypeError,
-            "%.200s() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
-            def->ml_name, nargs);
-        return NULL;
-    }
-    return def->ml_meth(self, NULL);
-}
-static PyObject * __Pyx_CyFunction_Vectorcall_O(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
-{
-    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
-    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
-#if CYTHON_BACKPORT_VECTORCALL
-    Py_ssize_t nargs = (Py_ssize_t)nargsf;
-#else
-    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
-#endif
-    PyObject *self;
-    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, kwnames)) {
-    case 1:
-        self = args[0];
-        args += 1;
-        nargs -= 1;
-        break;
-    case 0:
-        self = ((PyCFunctionObject*)cyfunc)->m_self;
-        break;
-    default:
-        return NULL;
-    }
-    if (unlikely(nargs != 1)) {
-        PyErr_Format(PyExc_TypeError,
-            "%.200s() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
-            def->ml_name, nargs);
-        return NULL;
-    }
-    return def->ml_meth(self, args[0]);
-}
-static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
-{
-    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
-    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
-#if CYTHON_BACKPORT_VECTORCALL
-    Py_ssize_t nargs = (Py_ssize_t)nargsf;
-#else
-    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
-#endif
-    PyObject *self;
-    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, NULL)) {
-    case 1:
-        self = args[0];
-        args += 1;
-        nargs -= 1;
-        break;
-    case 0:
-        self = ((PyCFunctionObject*)cyfunc)->m_self;
-        break;
-    default:
-        return NULL;
-    }
-    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
-}
-static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
-{
-    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
-    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
-    PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
-#if CYTHON_BACKPORT_VECTORCALL
-    Py_ssize_t nargs = (Py_ssize_t)nargsf;
-#else
-    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
-#endif
-    PyObject *self;
-    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, NULL)) {
-    case 1:
-        self = args[0];
-        args += 1;
-        nargs -= 1;
-        break;
-    case 0:
-        self = ((PyCFunctionObject*)cyfunc)->m_self;
-        break;
-    default:
-        return NULL;
-    }
-    return ((__Pyx_PyCMethod)(void(*)(void))def->ml_meth)(self, cls, args, (size_t)nargs, kwnames);
-}
-#endif
-#if CYTHON_USE_TYPE_SPECS
-static PyType_Slot __pyx_CyFunctionType_slots[] = {
-    {Py_tp_dealloc, (void *)__Pyx_CyFunction_dealloc},
-    {Py_tp_repr, (void *)__Pyx_CyFunction_repr},
-    {Py_tp_call, (void *)__Pyx_CyFunction_CallAsMethod},
-    {Py_tp_traverse, (void *)__Pyx_CyFunction_traverse},
-    {Py_tp_clear, (void *)__Pyx_CyFunction_clear},
-    {Py_tp_methods, (void *)__pyx_CyFunction_methods},
-    {Py_tp_members, (void *)__pyx_CyFunction_members},
-    {Py_tp_getset, (void *)__pyx_CyFunction_getsets},
-    {Py_tp_descr_get, (void *)__Pyx_PyMethod_New},
-    {0, 0},
-};
-static PyType_Spec __pyx_CyFunctionType_spec = {
-    __PYX_TYPE_MODULE_PREFIX "cython_function_or_method",
-    sizeof(__pyx_CyFunctionObject),
-    0,
-#ifdef Py_TPFLAGS_METHOD_DESCRIPTOR
-    Py_TPFLAGS_METHOD_DESCRIPTOR |
-#endif
-#if (defined(_Py_TPFLAGS_HAVE_VECTORCALL) && CYTHON_METH_FASTCALL)
-    _Py_TPFLAGS_HAVE_VECTORCALL |
-#endif
-    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
-    __pyx_CyFunctionType_slots
-};
-#else
-static PyTypeObject __pyx_CyFunctionType_type = {
-    PyVarObject_HEAD_INIT(0, 0)
-    __PYX_TYPE_MODULE_PREFIX "cython_function_or_method",
-    sizeof(__pyx_CyFunctionObject),
-    0,
-    (destructor) __Pyx_CyFunction_dealloc,
-#if !CYTHON_METH_FASTCALL
-    0,
-#elif CYTHON_BACKPORT_VECTORCALL
-    (printfunc)offsetof(__pyx_CyFunctionObject, func_vectorcall),
-#else
-    offsetof(PyCFunctionObject, vectorcall),
-#endif
-    0,
-    0,
-#if PY_MAJOR_VERSION < 3
-    0,
-#else
-    0,
-#endif
-    (reprfunc) __Pyx_CyFunction_repr,
-    0,
-    0,
-    0,
-    0,
-    __Pyx_CyFunction_CallAsMethod,
-    0,
-    0,
-    0,
-    0,
-#ifdef Py_TPFLAGS_METHOD_DESCRIPTOR
-    Py_TPFLAGS_METHOD_DESCRIPTOR |
-#endif
-#if defined(_Py_TPFLAGS_HAVE_VECTORCALL) && CYTHON_METH_FASTCALL
-    _Py_TPFLAGS_HAVE_VECTORCALL |
-#endif
-    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
-    0,
-    (traverseproc) __Pyx_CyFunction_traverse,
-    (inquiry) __Pyx_CyFunction_clear,
-    0,
-#if PY_VERSION_HEX < 0x030500A0
-    offsetof(__pyx_CyFunctionObject, func_weakreflist),
-#else
-    offsetof(PyCFunctionObject, m_weakreflist),
-#endif
-    0,
-    0,
-    __pyx_CyFunction_methods,
-    __pyx_CyFunction_members,
-    __pyx_CyFunction_getsets,
-    0,
-    0,
-    __Pyx_PyMethod_New,
-    0,
-    offsetof(__pyx_CyFunctionObject, func_dict),
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-#if PY_VERSION_HEX >= 0x030400a1
-    0,
-#endif
-#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
-    0,
-#endif
-#if __PYX_NEED_TP_PRINT_SLOT
-    0,
-#endif
-#if PY_VERSION_HEX >= 0x030C0000
-    0,
-#endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
-    0,
-#endif
-};
-#endif
-static int __pyx_CyFunction_init(PyObject *module) {
-#if CYTHON_USE_TYPE_SPECS
-    __pyx_CyFunctionType = __Pyx_FetchCommonTypeFromSpec(module, &__pyx_CyFunctionType_spec, NULL);
-#else
-    CYTHON_UNUSED_VAR(module);
-    __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
-#endif
-    if (unlikely(__pyx_CyFunctionType == NULL)) {
-        return -1;
-    }
-    return 0;
-}
-static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *func, size_t size, int pyobjects) {
-    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
-    m->defaults = PyObject_Malloc(size);
-    if (unlikely(!m->defaults))
-        return PyErr_NoMemory();
-    memset(m->defaults, 0, size);
-    m->defaults_pyobjects = pyobjects;
-    m->defaults_size = size;
-    return m->defaults;
-}
-static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *func, PyObject *tuple) {
-    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
-    m->defaults_tuple = tuple;
-    Py_INCREF(tuple);
-}
-static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *func, PyObject *dict) {
-    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
-    m->defaults_kwdict = dict;
-    Py_INCREF(dict);
-}
-static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *func, PyObject *dict) {
-    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
-    m->func_annotations = dict;
-    Py_INCREF(dict);
-}
-
-/* CythonFunction */
-static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml, int flags, PyObject* qualname,
-                                      PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
-    PyObject *op = __Pyx_CyFunction_Init(
-        PyObject_GC_New(__pyx_CyFunctionObject, __pyx_CyFunctionType),
-        ml, flags, qualname, closure, module, globals, code
-    );
-    if (likely(op)) {
-        PyObject_GC_Track(op);
-    }
-    return op;
-}
-
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
@@ -18938,55 +17408,55 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to long");
     return (long) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
-    const long neg_one = (long) -1, const_zero = (long) 0;
+    const int neg_one = (int) -1, const_zero = (int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
-        if (sizeof(long) < sizeof(long)) {
+        if (sizeof(int) < sizeof(long)) {
             return PyInt_FromLong((long) value);
-        } else if (sizeof(long) <= sizeof(unsigned long)) {
+        } else if (sizeof(int) <= sizeof(unsigned long)) {
             return PyLong_FromUnsignedLong((unsigned long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
             return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
 #endif
         }
     } else {
-        if (sizeof(long) <= sizeof(long)) {
+        if (sizeof(int) <= sizeof(long)) {
             return PyInt_FromLong((long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
 #if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
-        return _PyLong_FromByteArray(bytes, sizeof(long),
+        return _PyLong_FromByteArray(bytes, sizeof(int),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
         from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
-        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(long));
+        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(int));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
         if (!is_unsigned) {
             kwds = PyDict_New();
@@ -19275,119 +17745,55 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(enum __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const enum __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag neg_one = (enum __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag) -1, const_zero = (enum __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(enum __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(enum __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(enum __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(enum __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(enum __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
-        return _PyLong_FromByteArray(bytes, sizeof(enum __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag),
-                                     little, !is_unsigned);
-#else
-        PyObject *from_bytes, *result = NULL;
-        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
-        if (!from_bytes) return NULL;
-        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(enum __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag));
-        if (!py_bytes) goto limited_bad;
-        order_str = PyUnicode_FromString(little ? "little" : "big");
-        if (!order_str) goto limited_bad;
-        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
-        if (!arg_tuple) goto limited_bad;
-        if (!is_unsigned) {
-            kwds = PyDict_New();
-            if (!kwds) goto limited_bad;
-            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
-        }
-        result = PyObject_Call(from_bytes, arg_tuple, kwds);
-        limited_bad:
-        Py_XDECREF(kwds);
-        Py_XDECREF(arg_tuple);
-        Py_XDECREF(order_str);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(from_bytes);
-        return result;
-#endif
-    }
-}
-
-/* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
-    const int neg_one = (int) -1, const_zero = (int) 0;
+    const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
-        if (sizeof(int) < sizeof(long)) {
+        if (sizeof(long) < sizeof(long)) {
             return PyInt_FromLong((long) value);
-        } else if (sizeof(int) <= sizeof(unsigned long)) {
+        } else if (sizeof(long) <= sizeof(unsigned long)) {
             return PyLong_FromUnsignedLong((unsigned long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
             return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
 #endif
         }
     } else {
-        if (sizeof(int) <= sizeof(long)) {
+        if (sizeof(long) <= sizeof(long)) {
             return PyInt_FromLong((long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
 #if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
-        return _PyLong_FromByteArray(bytes, sizeof(int),
+        return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
         from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
-        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(int));
+        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(long));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
         if (!is_unsigned) {
             kwds = PyDict_New();
@@ -19412,15 +17818,15 @@
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name);
     if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
         PyErr_Clear();
         Py_XDECREF(name);
-        name = __Pyx_NewRef(__pyx_n_s__23);
+        name = __Pyx_NewRef(__pyx_n_s__20);
     }
     return name;
 }
 #endif
 
 /* FastTypeChecks */
 #if CYTHON_COMPILING_IN_CPYTHON
```

### Comparing `py_ballisticcalc.exts-2.0.0b3/pyproject.toml` & `py_ballisticcalc.exts-2.0.0b4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [build-system]
 requires = ["setuptools", "wheel", 'cython']
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "py_ballisticcalc.exts"
-version = "2.0.0b3"
+version = "2.0.0b4"
 
 authors = [
     { name="o-murphy", email="thehelixpg@gmail.com" },
     { name="dbookstaber", email="bookstaber@gmail.com"}
 ]
 description = "LGPL library for small arms ballistic calculations (Python 3)"
 readme = "README.md"
```

