# Comparing `tmp/doki-Mowstyl-1.3.2.tar.gz` & `tmp/doki-Mowstyl-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doki-Mowstyl-1.3.2.tar", last modified: Tue Feb 15 21:13:18 2022, max compression
+gzip compressed data, was "doki-Mowstyl-1.4.0.tar", last modified: Wed May 10 18:24:39 2023, max compression
```

## Comparing `doki-Mowstyl-1.3.2.tar` & `doki-Mowstyl-1.4.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2022-02-15 21:13:18.537455 doki-Mowstyl-1.3.2/
--rw-rw-rw-   0        0        0     1111 2021-09-20 14:20:25.000000 doki-Mowstyl-1.3.2/LICENSE
--rw-rw-rw-   0        0        0     1169 2022-02-15 21:13:18.536455 doki-Mowstyl-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0      824 2021-09-15 23:16:12.000000 doki-Mowstyl-1.3.2/README.md
-drwxrwxrwx   0        0        0        0 2022-02-15 21:13:18.527457 doki-Mowstyl-1.3.2/doki_Mowstyl.egg-info/
--rw-rw-rw-   0        0        0     1169 2022-02-15 21:13:18.000000 doki-Mowstyl-1.3.2/doki_Mowstyl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      522 2022-02-15 21:13:18.000000 doki-Mowstyl-1.3.2/doki_Mowstyl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-15 21:13:18.000000 doki-Mowstyl-1.3.2/doki_Mowstyl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2022-02-15 21:13:18.000000 doki-Mowstyl-1.3.2/doki_Mowstyl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      110 2021-07-23 13:21:51.000000 doki-Mowstyl-1.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-02-15 21:13:18.537455 doki-Mowstyl-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0     2819 2022-02-15 21:10:06.000000 doki-Mowstyl-1.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-02-15 21:13:18.519546 doki-Mowstyl-1.3.2/src/
-drwxrwxrwx   0        0        0        0 2022-02-15 21:13:18.535455 doki-Mowstyl-1.3.2/src/doki/
--rw-rw-rw-   0        0        0     1812 2021-10-19 13:02:35.000000 doki-Mowstyl-1.3.2/src/doki/arraylist.c
--rw-rw-rw-   0        0        0     1035 2021-10-19 12:10:13.000000 doki-Mowstyl-1.3.2/src/doki/arraylist.h
--rw-rw-rw-   0        0        0    46485 2022-02-15 21:10:06.000000 doki-Mowstyl-1.3.2/src/doki/doki.c
--rw-rw-rw-   0        0        0    12726 2022-02-15 21:10:06.000000 doki-Mowstyl-1.3.2/src/doki/funmatrix.c
--rw-rw-rw-   0        0        0     4006 2022-02-15 21:10:06.000000 doki-Mowstyl-1.3.2/src/doki/funmatrix.h
--rw-rw-rw-   0        0        0     4149 2021-10-19 12:10:13.000000 doki-Mowstyl-1.3.2/src/doki/platform.c
--rw-rw-rw-   0        0        0     7451 2022-02-15 14:46:56.000000 doki-Mowstyl-1.3.2/src/doki/platform.h
--rw-rw-rw-   0        0        0      313 2021-07-24 11:59:20.000000 doki-Mowstyl-1.3.2/src/doki/qgate.h
--rw-rw-rw-   0        0        0    11412 2022-02-15 19:02:13.000000 doki-Mowstyl-1.3.2/src/doki/qops.c
--rw-rw-rw-   0        0        0     2059 2021-10-19 12:10:13.000000 doki-Mowstyl-1.3.2/src/doki/qops.h
--rw-rw-rw-   0        0        0     3064 2022-02-15 14:46:56.000000 doki-Mowstyl-1.3.2/src/doki/qstate.c
--rw-rw-rw-   0        0        0     2320 2022-02-15 14:46:56.000000 doki-Mowstyl-1.3.2/src/doki/qstate.h
+drwxrwxrwx   0        0        0        0 2023-05-10 18:24:39.994444 doki-Mowstyl-1.4.0/
+-rw-rw-rw-   0        0        0     1111 2021-09-20 14:20:25.000000 doki-Mowstyl-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0     1148 2023-05-10 18:24:39.993445 doki-Mowstyl-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      824 2021-09-15 23:16:12.000000 doki-Mowstyl-1.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 18:24:39.983444 doki-Mowstyl-1.4.0/doki_Mowstyl.egg-info/
+-rw-rw-rw-   0        0        0     1148 2023-05-10 18:24:39.000000 doki-Mowstyl-1.4.0/doki_Mowstyl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      557 2023-05-10 18:24:39.000000 doki-Mowstyl-1.4.0/doki_Mowstyl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 18:24:39.000000 doki-Mowstyl-1.4.0/doki_Mowstyl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-10 18:24:39.000000 doki-Mowstyl-1.4.0/doki_Mowstyl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-10 18:24:39.000000 doki-Mowstyl-1.4.0/doki_Mowstyl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      124 2023-05-10 16:36:21.000000 doki-Mowstyl-1.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-10 18:24:39.994444 doki-Mowstyl-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     2966 2023-05-10 16:36:50.000000 doki-Mowstyl-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 18:24:39.976446 doki-Mowstyl-1.4.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 18:24:39.992447 doki-Mowstyl-1.4.0/src/doki/
+-rw-rw-rw-   0        0        0     1812 2021-10-19 13:02:35.000000 doki-Mowstyl-1.4.0/src/doki/arraylist.c
+-rw-rw-rw-   0        0        0     1035 2021-10-19 12:10:13.000000 doki-Mowstyl-1.4.0/src/doki/arraylist.h
+-rw-rw-rw-   0        0        0    50644 2023-05-10 18:15:50.000000 doki-Mowstyl-1.4.0/src/doki/doki.c
+-rw-rw-rw-   0        0        0    12726 2022-02-15 21:10:06.000000 doki-Mowstyl-1.4.0/src/doki/funmatrix.c
+-rw-rw-rw-   0        0        0     4006 2022-02-15 21:10:06.000000 doki-Mowstyl-1.4.0/src/doki/funmatrix.h
+-rw-rw-rw-   0        0        0     4149 2021-10-19 12:10:13.000000 doki-Mowstyl-1.4.0/src/doki/platform.c
+-rw-rw-rw-   0        0        0     7445 2023-05-10 14:44:41.000000 doki-Mowstyl-1.4.0/src/doki/platform.h
+-rw-rw-rw-   0        0        0      313 2021-07-24 11:59:20.000000 doki-Mowstyl-1.4.0/src/doki/qgate.h
+-rw-rw-rw-   0        0        0    11412 2022-02-15 19:02:13.000000 doki-Mowstyl-1.4.0/src/doki/qops.c
+-rw-rw-rw-   0        0        0     2059 2021-10-19 12:10:13.000000 doki-Mowstyl-1.4.0/src/doki/qops.h
+-rw-rw-rw-   0        0        0     3064 2022-02-15 14:46:56.000000 doki-Mowstyl-1.4.0/src/doki/qstate.c
+-rw-rw-rw-   0        0        0     2320 2022-02-15 14:46:56.000000 doki-Mowstyl-1.4.0/src/doki/qstate.h
```

### Comparing `doki-Mowstyl-1.3.2/LICENSE` & `doki-Mowstyl-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `doki-Mowstyl-1.3.2/PKG-INFO` & `doki-Mowstyl-1.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: doki-Mowstyl
-Version: 1.3.2
+Version: 1.4.0
 Summary: Python interface for Doki (QSimov core)
 Home-page: https://github.com/Mowstyl/Doki
 Author: Hernán Indíbil de la Cruz Calvo
 Author-email: HernanIndibil.LaCruz@alu.uclm.es
 License: MIT
 Keywords: qsimov simulator quantum
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -21,8 +20,7 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 License-File: LICENSE
 
 Python module containing Doki, the core of QSimov quantum computer simulation platform. Written in C with OpenMP parallelism.
-
```

### Comparing `doki-Mowstyl-1.3.2/README.md` & `doki-Mowstyl-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `doki-Mowstyl-1.3.2/doki_Mowstyl.egg-info/PKG-INFO` & `doki-Mowstyl-1.4.0/doki_Mowstyl.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: doki-Mowstyl
-Version: 1.3.2
+Version: 1.4.0
 Summary: Python interface for Doki (QSimov core)
 Home-page: https://github.com/Mowstyl/Doki
 Author: Hernán Indíbil de la Cruz Calvo
 Author-email: HernanIndibil.LaCruz@alu.uclm.es
 License: MIT
 Keywords: qsimov simulator quantum
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -21,8 +20,7 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 License-File: LICENSE
 
 Python module containing Doki, the core of QSimov quantum computer simulation platform. Written in C with OpenMP parallelism.
-
```

### Comparing `doki-Mowstyl-1.3.2/doki_Mowstyl.egg-info/SOURCES.txt` & `doki-Mowstyl-1.4.0/doki_Mowstyl.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 doki_Mowstyl.egg-info/PKG-INFO
 doki_Mowstyl.egg-info/SOURCES.txt
 doki_Mowstyl.egg-info/dependency_links.txt
+doki_Mowstyl.egg-info/requires.txt
 doki_Mowstyl.egg-info/top_level.txt
 src/doki/arraylist.c
 src/doki/doki.c
 src/doki/funmatrix.c
 src/doki/platform.c
 src/doki/qops.c
 src/doki/qstate.c
```

### Comparing `doki-Mowstyl-1.3.2/setup.py` & `doki-Mowstyl-1.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Installation module."""
 
 import platform
+import numpy as np
 
 from setuptools import setup, Extension
 from setuptools.command.build_ext import build_ext
 
 headers = ["src/doki/platform.h",
            "src/doki/funmatrix.h",
            "src/doki/qstate.h",
@@ -40,15 +41,15 @@
         build_ext.build_extensions(self)
 
 
 def main():
     """Code to be executed on install."""
     setup(
         name="doki-Mowstyl",
-        version="1.3.2",
+        version="1.4.0",
         author="Hernán Indíbil de la Cruz Calvo",
         author_email="HernanIndibil.LaCruz@alu.uclm.es",
         cmdclass={'build_ext': DokiBuild},
         license="MIT",
         url="https://github.com/Mowstyl/Doki",
         description="Python interface for Doki (QSimov core)",
         long_description="Python module containing Doki, the core of QSimov" +
@@ -66,17 +67,21 @@
             'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: Implementation :: CPython',
             'Topic :: Software Development :: Libraries :: Python Modules',
             "Topic :: Scientific/Engineering",
         ],
         keywords="qsimov simulator quantum",
+        install_requires=[
+            "numpy>=1.21"
+        ],
         ext_modules=[Extension('doki', sources=sources,
                                extra_compile_args=_comp_args,
-                               extra_link_args=_comp_args)],
+                               extra_link_args=_comp_args,
+                               include_dirs=[np.get_include()])],
         data_files=[('headers', headers)],
         python_requires=">=3.6",
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `doki-Mowstyl-1.3.2/src/doki/arraylist.c` & `doki-Mowstyl-1.4.0/src/doki/arraylist.c`

 * *Files identical despite different names*

### Comparing `doki-Mowstyl-1.3.2/src/doki/arraylist.h` & `doki-Mowstyl-1.4.0/src/doki/arraylist.h`

 * *Files identical despite different names*

### Comparing `doki-Mowstyl-1.3.2/src/doki/doki.c` & `doki-Mowstyl-1.4.0/src/doki/doki.c`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #define PY_SSIZE_T_CLEAN
 #include <Python.h>
 #include <omp.h>
+#include <numpy/arrayobject.h>
 #include "platform.h"
 #include "qstate.h"
 #include "qgate.h"
 #include "qops.h"
 
 
 static PyObject *DokiError;
@@ -32,14 +33,23 @@
 
 static PyObject *
 doki_gate_get (PyObject *self, PyObject *args);
 
 static PyObject *
 doki_registry_get (PyObject *self, PyObject *args);
 
+void
+custom_state_init_py(PyObject *values, struct state_vector *state);
+
+void
+custom_state_init_np(PyObject *values, struct state_vector *state);
+
+static PyObject *
+doki_registry_new_data (PyObject *self, PyObject *args);
+
 static PyObject *
 doki_registry_apply (PyObject *self, PyObject *args);
 
 static PyObject *
 doki_registry_join (PyObject *self, PyObject *args);
 
 static PyObject *
@@ -90,14 +100,15 @@
 static PyObject *
 doki_funmatrix_trace (PyObject *self, PyObject *args);
 
 static PyMethodDef DokiMethods[] = {
     {"gate_new", doki_gate_new, METH_VARARGS, "Create new gate"},
     {"gate_get", doki_gate_get, METH_VARARGS, "Get matrix associated to gate"},
     {"registry_new", doki_registry_new, METH_VARARGS, "Create new registry"},
+    {"registry_new_data", doki_registry_new_data, METH_VARARGS, "Create new registry initialized with the specified values"},
     {"registry_clone", doki_registry_clone, METH_VARARGS, "Clone a registry"},
     {"registry_del", doki_registry_del, METH_VARARGS, "Destroy a registry"},
     {"registry_get", doki_registry_get, METH_VARARGS, "Get value from registry"},
     {"registry_apply", doki_registry_apply, METH_VARARGS, "Apply a gate"},
     {"registry_join", doki_registry_join, METH_VARARGS, "Merges two registries"},
     {"registry_measure", doki_registry_measure, METH_VARARGS, "Measures and collapses specified qubits"},
     {"registry_prob", doki_registry_prob, METH_VARARGS, "Get the chances of obtaining 1 when measuring a certain qubit"},
@@ -128,14 +139,16 @@
 };
 
 PyMODINIT_FUNC
 PyInit_doki(void)
 {
     PyObject *m;
 
+    assert(!PyErr_Occurred());
+    import_array(); // Initialise Numpy
     m = PyModule_Create(&dokimodule);
     if (m == NULL)
         return NULL;
 
     DokiError = PyErr_NewException("qsimov.doki.error", NULL, NULL);
     Py_XINCREF(DokiError);
     if (PyModule_AddObject(m, "error", DokiError) < 0) {
@@ -172,15 +185,15 @@
 
     /* Optionally import the module; alternatively,
        import can be deferred until the embedded script
        imports it. */
     PyObject *pmodule = PyImport_ImportModule("doki");
     if (!pmodule) {
         PyErr_Print();
-        fprintf(stderr, "Error: could not import module 'spam'\n");
+        fprintf(stderr, "Error: could not import module 'doki'\n");
     }
     PyMem_RawFree(program);
     return 0;
 }
 
 void
 doki_registry_destroy (PyObject *capsule)
@@ -500,14 +513,135 @@
         val = complex_mult(val, aux);
     }
     result = PyComplex_FromDoubles(RE(val), IM(val));
 
     return result;
 }
 
+void
+custom_state_init_py(PyObject *values, struct state_vector *state)
+{
+    NATURAL_TYPE i;
+    COMPLEX_TYPE val;
+    PyObject *aux;
+
+    for (i = 0; i < state->size; i++) {
+        aux = PyList_GetItem(values, i);
+        val = complex_init(PyComplex_RealAsDouble(aux), PyComplex_ImagAsDouble(aux));
+        state_set(state, i, val);
+    }
+}
+
+void
+custom_state_init_np(PyObject *values, struct state_vector *state)
+{
+    NATURAL_TYPE i;
+    COMPLEX_TYPE val;
+    PyObject *aux;
+
+    for (i = 0; i < state->size; i++) {
+        aux = PyArray_GETITEM(values, PyArray_GETPTR1(values, i));
+        val = complex_init(PyComplex_RealAsDouble(aux), PyComplex_ImagAsDouble(aux));
+        state_set(state, i, val);
+    }
+}
+
+static PyObject *
+doki_registry_new_data (PyObject *self, PyObject *args)
+{
+    PyObject *raw_vals;
+    unsigned int num_qubits;
+    unsigned char result;
+    struct state_vector *state;
+    short debug_enabled;
+
+    if (!PyArg_ParseTuple(args, "IOh", &num_qubits, &raw_vals, &debug_enabled)) {
+        PyErr_SetString(DokiError, "Syntax: registry_new_data(num_qubits, values, verbose)");
+        return NULL;
+    }
+    if (num_qubits == 0) {
+        PyErr_SetString(DokiError, "num_qubits can't be zero");
+        return NULL;
+    }
+    if (debug_enabled) {
+        printf("[DEBUG] State allocation\n");
+    }
+    state = MALLOC_TYPE(1, struct state_vector);
+    if (state == NULL) {
+        PyErr_SetString(DokiError, "Failed to allocate state structure");
+        return NULL;
+    }
+    if (debug_enabled) {
+        printf("[DEBUG] State initialization\n");
+    }
+    result = state_init(state, num_qubits, 0);
+    if (result == 1) {
+        PyErr_SetString(DokiError, "Failed to allocate state vector");
+        return NULL;
+    }
+    else if (result == 2) {
+        PyErr_SetString(DokiError, "Failed to allocate state chunk");
+        return NULL;
+    }
+    else if (result == 3) {
+        PyErr_SetString(DokiError, "Number of qubits exceeds maximum");
+        return NULL;
+    }
+    else if (result != 0) {
+        PyErr_SetString(DokiError, "Unknown error when creating state");
+        return NULL;
+    }
+    if (debug_enabled) {
+        printf("[DEBUG] Dumping data...\n");
+    }
+    if (PyArray_Check(raw_vals)) {
+        if (debug_enabled) {
+            printf("[DEBUG] Checking array type\n");
+        }
+        if (!PyArray_ISNUMBER(raw_vals)) {
+            PyErr_SetString(DokiError, "values have to be numbers");
+            return NULL;
+        }
+        if (debug_enabled) {
+            printf("[DEBUG] Checking array size\n");
+        }
+        if (PyArray_SIZE(raw_vals) != state->size) {
+            PyErr_SetString(DokiError, "Wrong array size for the specified number of qubits");
+            return NULL;
+        }
+        if (debug_enabled) {
+            printf("[DEBUG] Working with numpy array\n");
+        }
+        custom_state_init_np(raw_vals, state);
+    }
+    else if (PyList_Check(raw_vals)) {
+        if (debug_enabled) {
+            printf("[DEBUG] Checking list size\n");
+        }
+        if (PyList_GET_SIZE(raw_vals) != state->size) {
+            PyErr_SetString(DokiError, "Wrong list size for the specified number of qubits\n");
+            return NULL;
+        }
+        if (debug_enabled) {
+            printf("[DEBUG] Working with python list\n");
+        }
+        custom_state_init_py(raw_vals, state);
+    }
+    else {
+        PyErr_SetString(DokiError, "values has to be either a python list or a numpy array");
+        return NULL;
+    }
+    if (debug_enabled) {
+        printf("[DEBUG] Starting creation\n");
+    }
+
+    return PyCapsule_New((void*) state, "qsimov.doki.state_vector",
+                         &doki_registry_destroy);
+}
+
 static PyObject *
 doki_registry_apply (PyObject *self, PyObject *args)
 {
     PyObject *raw_val, *state_capsule, *gate_capsule,
              *target_list, *control_set, *acontrol_set, *aux;
     void *raw_state, *raw_gate;
     struct state_vector *state, *new_state;
```

### Comparing `doki-Mowstyl-1.3.2/src/doki/funmatrix.c` & `doki-Mowstyl-1.4.0/src/doki/funmatrix.c`

 * *Files identical despite different names*

### Comparing `doki-Mowstyl-1.3.2/src/doki/funmatrix.h` & `doki-Mowstyl-1.4.0/src/doki/funmatrix.h`

 * *Files identical despite different names*

### Comparing `doki-Mowstyl-1.3.2/src/doki/platform.c` & `doki-Mowstyl-1.4.0/src/doki/platform.c`

 * *Files identical despite different names*

### Comparing `doki-Mowstyl-1.3.2/src/doki/platform.h` & `doki-Mowstyl-1.4.0/src/doki/platform.h`

 * *Files 1% similar despite different names*

```diff
@@ -148,19 +148,19 @@
 	#endif
 #endif
 
 #define MALLOC_TYPE(n,type) ((type *) malloc((n) * sizeof(type)))
 #define CALLOC_TYPE(n,type) ((type *) calloc((n), sizeof(type)))
 #define REALLOC_TYPE(p,n,type) ((type *) realloc((p), (n) * sizeof(type)))
 
-#define NATURAL_TYPE long long int
-#define NATURAL_STRING_FORMAT "%lld"
+#define NATURAL_TYPE intmax_t
+#define NATURAL_STRING_FORMAT "%j"
 static const NATURAL_TYPE NATURAL_ZERO = 0;
 static const NATURAL_TYPE NATURAL_ONE = 1;
-static const NATURAL_TYPE NATURAL_MAX = LLONG_MAX;
+static const NATURAL_TYPE NATURAL_MAX = INTMAX_MAX;
 static const unsigned int NATURAL_BITS = sizeof(NATURAL_TYPE) * 8 - 1;
 
 #define DECIMAL_PLACES 5 // max: 17 (MinGWx64-gcc)
 #define DECIMAL_PLACES_S "5" // same as before, but as a string
 #define NOTATION "g" // f for normal behaviour, e for scientific notation, g for shortest (f or e)
 #define PRECISION 2
 #if PRECISION==1
```

### Comparing `doki-Mowstyl-1.3.2/src/doki/qops.c` & `doki-Mowstyl-1.4.0/src/doki/qops.c`

 * *Files identical despite different names*

### Comparing `doki-Mowstyl-1.3.2/src/doki/qops.h` & `doki-Mowstyl-1.4.0/src/doki/qops.h`

 * *Files identical despite different names*

### Comparing `doki-Mowstyl-1.3.2/src/doki/qstate.c` & `doki-Mowstyl-1.4.0/src/doki/qstate.c`

 * *Files identical despite different names*

### Comparing `doki-Mowstyl-1.3.2/src/doki/qstate.h` & `doki-Mowstyl-1.4.0/src/doki/qstate.h`

 * *Files identical despite different names*

