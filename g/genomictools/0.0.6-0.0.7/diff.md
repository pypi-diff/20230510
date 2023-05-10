# Comparing `tmp/genomictools-0.0.6.tar.gz` & `tmp/genomictools-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genomictools-0.0.6.tar", last modified: Sat Jan 14 09:54:48 2023, max compression
+gzip compressed data, was "genomictools-0.0.7.tar", last modified: Wed May 10 08:44:47 2023, max compression
```

## Comparing `genomictools-0.0.6.tar` & `genomictools-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2023-01-14 09:54:48.610522 genomictools-0.0.6/
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)      131 2022-12-28 03:23:32.000000 genomictools-0.0.6/MANIFEST.in
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)     4154 2023-01-14 09:54:48.600521 genomictools-0.0.6/PKG-INFO
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)     3627 2023-01-14 09:49:52.000000 genomictools-0.0.6/README.md
-drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2023-01-14 09:54:48.600521 genomictools-0.0.6/genomictools/
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)   907833 2023-01-03 17:21:47.000000 genomictools-0.0.6/genomictools/__init__.cpp
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)     9820 2022-12-28 03:23:32.000000 genomictools-0.0.6/genomictools/genomic.cpp
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)     1011 2022-12-28 03:23:32.000000 genomictools-0.0.6/genomictools/genomic.h
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)      867 2022-12-28 03:23:32.000000 genomictools-0.0.6/genomictools/genomic.pxd
-drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2023-01-14 09:54:48.600521 genomictools-0.0.6/genomictools.egg-info/
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)     4154 2023-01-14 09:54:48.000000 genomictools-0.0.6/genomictools.egg-info/PKG-INFO
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)      288 2023-01-14 09:54:48.000000 genomictools-0.0.6/genomictools.egg-info/SOURCES.txt
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)        1 2023-01-14 09:54:48.000000 genomictools-0.0.6/genomictools.egg-info/dependency_links.txt
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)       13 2023-01-14 09:54:48.000000 genomictools-0.0.6/genomictools.egg-info/top_level.txt
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)      109 2022-12-28 03:23:32.000000 genomictools-0.0.6/pyproject.toml
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)       38 2023-01-14 09:54:48.611522 genomictools-0.0.6/setup.cfg
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)     1462 2023-01-14 09:51:04.000000 genomictools-0.0.6/setup.py
+drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2023-05-10 08:44:47.850025 genomictools-0.0.7/
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)      131 2022-12-28 03:23:32.000000 genomictools-0.0.7/MANIFEST.in
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)     4154 2023-05-10 08:44:47.850025 genomictools-0.0.7/PKG-INFO
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)     3627 2023-01-14 09:49:52.000000 genomictools-0.0.7/README.md
+drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2023-05-10 08:44:47.849025 genomictools-0.0.7/genomictools/
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)   929019 2023-05-10 08:44:47.000000 genomictools-0.0.7/genomictools/__init__.cpp
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)     9820 2022-12-28 03:23:32.000000 genomictools-0.0.7/genomictools/genomic.cpp
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)     1011 2022-12-28 03:23:32.000000 genomictools-0.0.7/genomictools/genomic.h
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)      867 2022-12-28 03:23:32.000000 genomictools-0.0.7/genomictools/genomic.pxd
+drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2023-05-10 08:44:47.849025 genomictools-0.0.7/genomictools.egg-info/
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)     4154 2023-05-10 08:44:47.000000 genomictools-0.0.7/genomictools.egg-info/PKG-INFO
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)      288 2023-05-10 08:44:47.000000 genomictools-0.0.7/genomictools.egg-info/SOURCES.txt
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)        1 2023-05-10 08:44:47.000000 genomictools-0.0.7/genomictools.egg-info/dependency_links.txt
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)       13 2023-05-10 08:44:47.000000 genomictools-0.0.7/genomictools.egg-info/top_level.txt
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)      109 2022-12-28 03:23:32.000000 genomictools-0.0.7/pyproject.toml
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)       38 2023-05-10 08:44:47.850025 genomictools-0.0.7/setup.cfg
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)     1462 2023-05-10 08:44:27.000000 genomictools-0.0.7/setup.py
```

### Comparing `genomictools-0.0.6/PKG-INFO` & `genomictools-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomictools
-Version: 0.0.6
+Version: 0.0.7
 Summary: Tools for processing genomic ranges
 Author: Alden Leung
 Author-email: alden.leung@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `genomictools-0.0.6/README.md` & `genomictools-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `genomictools-0.0.6/genomictools/__init__.cpp` & `genomictools-0.0.7/genomictools/__init__.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1031,15 +1031,16 @@
 struct __pyx_obj_12genomictools___pyx_scope_struct_2_find_overlaps;
 struct __pyx_obj_12genomictools___pyx_scope_struct_3_find_non_overlaps;
 struct __pyx_obj_12genomictools___pyx_scope_struct_4_find_overlaps;
 struct __pyx_obj_12genomictools___pyx_scope_struct_5_intersection;
 struct __pyx_obj_12genomictools___pyx_scope_struct_6__internal_intersection;
 struct __pyx_obj_12genomictools___pyx_scope_struct_7_genexpr;
 struct __pyx_obj_12genomictools___pyx_scope_struct_8_union;
-struct __pyx_obj_12genomictools___pyx_scope_struct_9_substract;
+struct __pyx_obj_12genomictools___pyx_scope_struct_9_add;
+struct __pyx_obj_12genomictools___pyx_scope_struct_10_substract;
 
 /* "genomictools/__init__.pyx":20
  * 
  * @cython.auto_pickle(False)
  * cdef class GenomicAnnotation():             # <<<<<<<<<<<<<<
  * 	'''
  * 	Any object that contains a representation of the genomic position.
@@ -1271,19 +1272,36 @@
   PyObject *(*__pyx_t_2)(PyObject *);
 };
 
 
 /* "genomictools/__init__.pyx":498
  * 
  * @cython.binding(True)
+ * def add(*genomic_collections):             # <<<<<<<<<<<<<<
+ * 	'''
+ * 	Return all regions from all genomic collections.
+ */
+struct __pyx_obj_12genomictools___pyx_scope_struct_9_add {
+  PyObject_HEAD
+  PyObject *__pyx_v_genomic_collections;
+  PyObject *__pyx_v_r;
+  PyObject *__pyx_t_0;
+  Py_ssize_t __pyx_t_1;
+  PyObject *(*__pyx_t_2)(PyObject *);
+};
+
+
+/* "genomictools/__init__.pyx":524
+ * 
+ * @cython.binding(True)
  * def substract(query, *refs):             # <<<<<<<<<<<<<<
  * 	'''
  * 	Return all regions that are present in query but not in refs.
  */
-struct __pyx_obj_12genomictools___pyx_scope_struct_9_substract {
+struct __pyx_obj_12genomictools___pyx_scope_struct_10_substract {
   PyObject_HEAD
   PyObject *__pyx_v_q;
   PyObject *__pyx_v_query;
   PyObject *__pyx_v_r;
   struct __pyx_obj_12genomictools_GenomicCollection *__pyx_v_ref;
   PyObject *__pyx_v_refs;
   PyObject *__pyx_v_start_pos;
@@ -1902,14 +1920,17 @@
 /* GeneratorYieldFrom.proto */
 static CYTHON_INLINE PyObject* __Pyx_Generator_Yield_From(__pyx_CoroutineObject *gen, PyObject *source);
 
 /* IterNext.proto */
 #define __Pyx_PyIter_Next(obj) __Pyx_PyIter_Next2(obj, NULL)
 static CYTHON_INLINE PyObject *__Pyx_PyIter_Next2(PyObject *, PyObject *);
 
+/* KeywordStringCheck.proto */
+static int __Pyx_CheckKeywordStrings(PyObject *kwdict, const char* function_name, int kw_allowed);
+
 /* PyIntBinop.proto */
 #if !CYTHON_COMPILING_IN_PYPY
 static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check);
 #else
 #define __Pyx_PyInt_AddObjC(op1, op2, intval, inplace, zerodivision_check)\
     (inplace ? PyNumber_InPlaceAdd(op1, op2) : PyNumber_Add(op1, op2))
 #endif
@@ -2066,15 +2087,16 @@
 static PyTypeObject *__pyx_ptype_12genomictools___pyx_scope_struct_2_find_overlaps = 0;
 static PyTypeObject *__pyx_ptype_12genomictools___pyx_scope_struct_3_find_non_overlaps = 0;
 static PyTypeObject *__pyx_ptype_12genomictools___pyx_scope_struct_4_find_overlaps = 0;
 static PyTypeObject *__pyx_ptype_12genomictools___pyx_scope_struct_5_intersection = 0;
 static PyTypeObject *__pyx_ptype_12genomictools___pyx_scope_struct_6__internal_intersection = 0;
 static PyTypeObject *__pyx_ptype_12genomictools___pyx_scope_struct_7_genexpr = 0;
 static PyTypeObject *__pyx_ptype_12genomictools___pyx_scope_struct_8_union = 0;
-static PyTypeObject *__pyx_ptype_12genomictools___pyx_scope_struct_9_substract = 0;
+static PyTypeObject *__pyx_ptype_12genomictools___pyx_scope_struct_9_add = 0;
+static PyTypeObject *__pyx_ptype_12genomictools___pyx_scope_struct_10_substract = 0;
 static PyObject *__pyx_f_12genomictools___pyx_unpickle_GenomicPos__set_state(struct __pyx_obj_12genomictools_GenomicPos *, PyObject *); /*proto*/
 static PyObject *__pyx_f_12genomictools___pyx_unpickle_StrandedGenomicPos__set_state(struct __pyx_obj_12genomictools_StrandedGenomicPos *, PyObject *); /*proto*/
 static PyObject *__pyx_f_12genomictools___pyx_unpickle_AbstractGenomicCollection__set_state(struct __pyx_obj_12genomictools_AbstractGenomicCollection *, PyObject *); /*proto*/
 static std::string __pyx_convert_string_from_py_std__in_string(PyObject *); /*proto*/
 #define __Pyx_MODULE_NAME "genomictools"
 extern int __pyx_module_is_main_genomictools;
 int __pyx_module_is_main_genomictools = 0;
@@ -2086,14 +2108,15 @@
 static PyObject *__pyx_builtin_StopIteration;
 static const char __pyx_k_[] = ":";
 static const char __pyx_k_i[] = "i";
 static const char __pyx_k_q[] = "q";
 static const char __pyx_k_r[] = "r";
 static const char __pyx_k__2[] = "-";
 static const char __pyx_k_re[] = "re";
+static const char __pyx_k_add[] = "add";
 static const char __pyx_k_all[] = "__all__";
 static const char __pyx_k_key[] = "key";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_ref[] = "ref";
 static const char __pyx_k_args[] = "args";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_main[] = "__main__";
@@ -2164,14 +2187,15 @@
 static const char __pyx_k_find_overlaps[] = "find_overlaps";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_NotImplemented[] = "NotImplemented";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_GenomicAnnotation[] = "GenomicAnnotation";
 static const char __pyx_k_GenomicCollection[] = "GenomicCollection";
+static const char __pyx_k_add_locals_lambda[] = "add.<locals>.<lambda>";
 static const char __pyx_k_find_non_overlaps[] = "find_non_overlaps";
 static const char __pyx_k_StrandedGenomicPos[] = "StrandedGenomicPos";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_genomic_collection[] = "genomic_collection";
 static const char __pyx_k_GenomicPos_overlaps[] = "GenomicPos.overlaps";
 static const char __pyx_k_NotImplementedError[] = "NotImplementedError";
 static const char __pyx_k_genomic_collections[] = "genomic_collections";
@@ -2239,14 +2263,17 @@
 static PyObject *__pyx_n_u_StrandedGenomicAnnotation;
 static PyObject *__pyx_n_s_StrandedGenomicPos;
 static PyObject *__pyx_n_u_StrandedGenomicPos;
 static PyObject *__pyx_n_s_StrandedGenomicPos___reduce_cyth;
 static PyObject *__pyx_n_s_StrandedGenomicPos___setstate_cy;
 static PyObject *__pyx_n_s_StrandedGenomicPos_overlaps;
 static PyObject *__pyx_kp_u__2;
+static PyObject *__pyx_n_s_add;
+static PyObject *__pyx_n_u_add;
+static PyObject *__pyx_n_s_add_locals_lambda;
 static PyObject *__pyx_n_s_all;
 static PyObject *__pyx_n_s_append;
 static PyObject *__pyx_n_s_args;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_close;
 static PyObject *__pyx_n_s_collections;
 static PyObject *__pyx_n_s_compile;
@@ -2402,18 +2429,20 @@
 static PyObject *__pyx_pf_12genomictools_17GenomicCollection_13__reduce__(struct __pyx_obj_12genomictools_GenomicCollection *__pyx_v_self); /* proto */
 static PyObject *__pyx_lambda_funcdef_lambda3(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_k); /* proto */
 static PyObject *__pyx_pf_12genomictools_intersection(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_mergefunc, PyObject *__pyx_v_genomic_collections); /* proto */
 static PyObject *__pyx_pf_12genomictools_12intersection_22_internal_intersection_genexpr(PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_12genomictools_12intersection__internal_intersection(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_refs, PyObject *__pyx_v_queries); /* proto */
 static PyObject *__pyx_lambda_funcdef_lambda4(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_k); /* proto */
 static PyObject *__pyx_pf_12genomictools_3union(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_mergefunc, PyObject *__pyx_v_genomic_collections); /* proto */
-static PyObject *__pyx_pf_12genomictools_6substract(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_query, PyObject *__pyx_v_refs); /* proto */
-static PyObject *__pyx_pf_12genomictools_9__pyx_unpickle_GenomicPos(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_pf_12genomictools_11__pyx_unpickle_StrandedGenomicPos(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_pf_12genomictools_13__pyx_unpickle_AbstractGenomicCollection(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_lambda_funcdef_lambda5(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_k); /* proto */
+static PyObject *__pyx_pf_12genomictools_6add(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_genomic_collections); /* proto */
+static PyObject *__pyx_pf_12genomictools_9substract(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_query, PyObject *__pyx_v_refs); /* proto */
+static PyObject *__pyx_pf_12genomictools_12__pyx_unpickle_GenomicPos(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_12genomictools_14__pyx_unpickle_StrandedGenomicPos(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_12genomictools_16__pyx_unpickle_AbstractGenomicCollection(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_12genomictools_GenomicAnnotation(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_12genomictools_StrandedGenomicAnnotation(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_12genomictools_GenomicPos(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_12genomictools_StrandedGenomicPos(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_12genomictools_AbstractGenomicCollection(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_12genomictools_GenomicCollection(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_12genomictools___pyx_scope_struct__overlaps(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
@@ -2421,64 +2450,67 @@
 static PyObject *__pyx_tp_new_12genomictools___pyx_scope_struct_2_find_overlaps(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_12genomictools___pyx_scope_struct_3_find_non_overlaps(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_12genomictools___pyx_scope_struct_4_find_overlaps(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_12genomictools___pyx_scope_struct_5_intersection(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_12genomictools___pyx_scope_struct_6__internal_intersection(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_12genomictools___pyx_scope_struct_7_genexpr(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_12genomictools___pyx_scope_struct_8_union(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_tp_new_12genomictools___pyx_scope_struct_9_substract(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_12genomictools___pyx_scope_struct_9_add(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_12genomictools___pyx_scope_struct_10_substract(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_5944678;
 static PyObject *__pyx_int_63583258;
 static PyObject *__pyx_int_74888693;
 static PyObject *__pyx_int_102133340;
 static PyObject *__pyx_int_131304010;
 static PyObject *__pyx_int_222419149;
 static PyObject *__pyx_int_223736985;
 static PyObject *__pyx_int_228825662;
 static PyObject *__pyx_int_238750788;
 static PyObject *__pyx_tuple__5;
-static PyObject *__pyx_tuple__9;
 static PyObject *__pyx_tuple__10;
 static PyObject *__pyx_tuple__11;
 static PyObject *__pyx_tuple__12;
 static PyObject *__pyx_tuple__13;
 static PyObject *__pyx_tuple__14;
-static PyObject *__pyx_tuple__16;
-static PyObject *__pyx_tuple__18;
-static PyObject *__pyx_tuple__20;
-static PyObject *__pyx_tuple__22;
-static PyObject *__pyx_tuple__24;
-static PyObject *__pyx_tuple__26;
-static PyObject *__pyx_tuple__28;
-static PyObject *__pyx_tuple__30;
+static PyObject *__pyx_tuple__15;
+static PyObject *__pyx_tuple__17;
+static PyObject *__pyx_tuple__19;
+static PyObject *__pyx_tuple__21;
+static PyObject *__pyx_tuple__23;
+static PyObject *__pyx_tuple__25;
+static PyObject *__pyx_tuple__27;
+static PyObject *__pyx_tuple__29;
 static PyObject *__pyx_tuple__31;
-static PyObject *__pyx_tuple__33;
+static PyObject *__pyx_tuple__32;
 static PyObject *__pyx_tuple__34;
 static PyObject *__pyx_tuple__35;
 static PyObject *__pyx_tuple__36;
+static PyObject *__pyx_tuple__37;
 static PyObject *__pyx_tuple__38;
 static PyObject *__pyx_tuple__40;
+static PyObject *__pyx_tuple__42;
 static PyObject *__pyx_codeobj__3;
 static PyObject *__pyx_codeobj__4;
 static PyObject *__pyx_codeobj__6;
 static PyObject *__pyx_codeobj__7;
 static PyObject *__pyx_codeobj__8;
-static PyObject *__pyx_codeobj__15;
-static PyObject *__pyx_codeobj__17;
-static PyObject *__pyx_codeobj__19;
-static PyObject *__pyx_codeobj__21;
-static PyObject *__pyx_codeobj__23;
-static PyObject *__pyx_codeobj__25;
-static PyObject *__pyx_codeobj__27;
-static PyObject *__pyx_codeobj__29;
-static PyObject *__pyx_codeobj__32;
-static PyObject *__pyx_codeobj__37;
+static PyObject *__pyx_codeobj__9;
+static PyObject *__pyx_codeobj__16;
+static PyObject *__pyx_codeobj__18;
+static PyObject *__pyx_codeobj__20;
+static PyObject *__pyx_codeobj__22;
+static PyObject *__pyx_codeobj__24;
+static PyObject *__pyx_codeobj__26;
+static PyObject *__pyx_codeobj__28;
+static PyObject *__pyx_codeobj__30;
+static PyObject *__pyx_codeobj__33;
 static PyObject *__pyx_codeobj__39;
 static PyObject *__pyx_codeobj__41;
+static PyObject *__pyx_codeobj__43;
 /* Late includes */
 
 /* "genomictools/__init__.pyx":25
  * 	'''
  * 	@property
  * 	def genomic_pos(self):             # <<<<<<<<<<<<<<
  * 		'''
@@ -7461,15 +7493,15 @@
   __Pyx_RefNannySetupContext("overlaps (wrapper)", 0);
   __pyx_r = __pyx_pf_12genomictools_25AbstractGenomicCollection_4overlaps(((struct __pyx_obj_12genomictools_AbstractGenomicCollection *)__pyx_v_self), ((PyObject *)__pyx_v_q));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-static PyObject *__pyx_gb_12genomictools_25AbstractGenomicCollection_8overlaps_2generator6(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
+static PyObject *__pyx_gb_12genomictools_25AbstractGenomicCollection_8overlaps_2generator7(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
 /* "genomictools/__init__.pyx":332
  * 		Deterimine whether this collection overlaps with any regions indicated in `q`.
  * 		'''
  * 		return any(True for _ in self.find_overlaps(q))             # <<<<<<<<<<<<<<
  * 
  * 	def find_overlaps(self, q):
@@ -7491,15 +7523,15 @@
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_outer_scope = (struct __pyx_obj_12genomictools___pyx_scope_struct__overlaps *) __pyx_self;
   __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_outer_scope));
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_outer_scope);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_12genomictools_25AbstractGenomicCollection_8overlaps_2generator6, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_overlaps_locals_genexpr, __pyx_n_s_genomictools); if (unlikely(!gen)) __PYX_ERR(0, 332, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_12genomictools_25AbstractGenomicCollection_8overlaps_2generator7, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_overlaps_locals_genexpr, __pyx_n_s_genomictools); if (unlikely(!gen)) __PYX_ERR(0, 332, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -7507,15 +7539,15 @@
   __pyx_r = NULL;
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_gb_12genomictools_25AbstractGenomicCollection_8overlaps_2generator6(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
+static PyObject *__pyx_gb_12genomictools_25AbstractGenomicCollection_8overlaps_2generator7(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
 {
   struct __pyx_obj_12genomictools___pyx_scope_struct_1_genexpr *__pyx_cur_scope = ((struct __pyx_obj_12genomictools___pyx_scope_struct_1_genexpr *)__pyx_generator->closure);
   PyObject *__pyx_r = NULL;
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   Py_ssize_t __pyx_t_4;
@@ -7638,15 +7670,15 @@
  * 	def overlaps(self, q):             # <<<<<<<<<<<<<<
  * 		'''
  * 		Deterimine whether this collection overlaps with any regions indicated in `q`.
  */
 
 static PyObject *__pyx_pf_12genomictools_25AbstractGenomicCollection_4overlaps(struct __pyx_obj_12genomictools_AbstractGenomicCollection *__pyx_v_self, PyObject *__pyx_v_q) {
   struct __pyx_obj_12genomictools___pyx_scope_struct__overlaps *__pyx_cur_scope;
-  PyObject *__pyx_gb_12genomictools_25AbstractGenomicCollection_8overlaps_2generator6 = 0;
+  PyObject *__pyx_gb_12genomictools_25AbstractGenomicCollection_8overlaps_2generator7 = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -7694,15 +7726,15 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_AddTraceback("genomictools.AbstractGenomicCollection.overlaps", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_gb_12genomictools_25AbstractGenomicCollection_8overlaps_2generator6);
+  __Pyx_XDECREF(__pyx_gb_12genomictools_25AbstractGenomicCollection_8overlaps_2generator7);
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_12genomictools_25AbstractGenomicCollection_8generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
@@ -9932,15 +9964,15 @@
  * def intersection(*genomic_collections, mergefunc=None):             # <<<<<<<<<<<<<<
  * 	'''
  * 	Return the intersection of all genomic collections.
  */
 
 static PyObject *__pyx_pf_12genomictools_intersection(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_mergefunc, PyObject *__pyx_v_genomic_collections) {
   struct __pyx_obj_12genomictools___pyx_scope_struct_5_intersection *__pyx_cur_scope;
-  PyObject *__pyx_gb_12genomictools_12intersection_2generator7 = 0;
+  PyObject *__pyx_gb_12genomictools_12intersection_2generator8 = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("intersection", 0);
   __pyx_cur_scope = (struct __pyx_obj_12genomictools___pyx_scope_struct_5_intersection *)__pyx_tp_new_12genomictools___pyx_scope_struct_5_intersection(__pyx_ptype_12genomictools___pyx_scope_struct_5_intersection, __pyx_empty_tuple, NULL);
@@ -9964,21 +9996,21 @@
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_AddTraceback("genomictools.intersection", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
-  __Pyx_XDECREF(__pyx_gb_12genomictools_12intersection_2generator7);
+  __Pyx_XDECREF(__pyx_gb_12genomictools_12intersection_2generator8);
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-static PyObject *__pyx_gb_12genomictools_12intersection_2generator7(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
+static PyObject *__pyx_gb_12genomictools_12intersection_2generator8(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
 /* "genomictools/__init__.pyx":449
  * 
  * 	'''
  * 	def _internal_intersection(refs, queries):             # <<<<<<<<<<<<<<
  * 		for q in queries:
  * 			yield from union(GenomicPos(q.genomic_pos.name, max(q.genomic_pos.start, hit.genomic_pos.start), min(q.genomic_pos.stop, hit.genomic_pos.stop)) for hit in refs.find_overlaps(q))
@@ -10044,15 +10076,15 @@
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_12genomictools_12intersection__internal_intersection(__pyx_self, __pyx_v_refs, __pyx_v_queries);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-static PyObject *__pyx_gb_12genomictools_12intersection_22_internal_intersection_2generator8(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
+static PyObject *__pyx_gb_12genomictools_12intersection_22_internal_intersection_2generator9(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
 /* "genomictools/__init__.pyx":451
  * 	def _internal_intersection(refs, queries):
  * 		for q in queries:
  * 			yield from union(GenomicPos(q.genomic_pos.name, max(q.genomic_pos.start, hit.genomic_pos.start), min(q.genomic_pos.stop, hit.genomic_pos.stop)) for hit in refs.find_overlaps(q))             # <<<<<<<<<<<<<<
  * 	if len(genomic_collections) == 0:
  * 		return
@@ -10074,15 +10106,15 @@
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_outer_scope = (struct __pyx_obj_12genomictools___pyx_scope_struct_6__internal_intersection *) __pyx_self;
   __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_outer_scope));
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_outer_scope);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_12genomictools_12intersection_22_internal_intersection_2generator8, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_intersection_locals__internal_in, __pyx_n_s_genomictools); if (unlikely(!gen)) __PYX_ERR(0, 451, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_12genomictools_12intersection_22_internal_intersection_2generator9, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_intersection_locals__internal_in, __pyx_n_s_genomictools); if (unlikely(!gen)) __PYX_ERR(0, 451, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -10090,15 +10122,15 @@
   __pyx_r = NULL;
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_gb_12genomictools_12intersection_22_internal_intersection_2generator8(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
+static PyObject *__pyx_gb_12genomictools_12intersection_22_internal_intersection_2generator9(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
 {
   struct __pyx_obj_12genomictools___pyx_scope_struct_7_genexpr *__pyx_cur_scope = ((struct __pyx_obj_12genomictools___pyx_scope_struct_7_genexpr *)__pyx_generator->closure);
   PyObject *__pyx_r = NULL;
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   Py_ssize_t __pyx_t_4;
@@ -10305,15 +10337,15 @@
  * 	def _internal_intersection(refs, queries):             # <<<<<<<<<<<<<<
  * 		for q in queries:
  * 			yield from union(GenomicPos(q.genomic_pos.name, max(q.genomic_pos.start, hit.genomic_pos.start), min(q.genomic_pos.stop, hit.genomic_pos.stop)) for hit in refs.find_overlaps(q))
  */
 
 static PyObject *__pyx_pf_12genomictools_12intersection__internal_intersection(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_refs, PyObject *__pyx_v_queries) {
   struct __pyx_obj_12genomictools___pyx_scope_struct_6__internal_intersection *__pyx_cur_scope;
-  PyObject *__pyx_gb_12genomictools_12intersection_22_internal_intersection_2generator8 = 0;
+  PyObject *__pyx_gb_12genomictools_12intersection_22_internal_intersection_2generator9 = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_internal_intersection", 0);
   __pyx_cur_scope = (struct __pyx_obj_12genomictools___pyx_scope_struct_6__internal_intersection *)__pyx_tp_new_12genomictools___pyx_scope_struct_6__internal_intersection(__pyx_ptype_12genomictools___pyx_scope_struct_6__internal_intersection, __pyx_empty_tuple, NULL);
@@ -10327,32 +10359,32 @@
   __pyx_cur_scope->__pyx_v_refs = __pyx_v_refs;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_refs);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_refs);
   __pyx_cur_scope->__pyx_v_queries = __pyx_v_queries;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_queries);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_queries);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_12genomictools_12intersection_2generator7, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_internal_intersection, __pyx_n_s_intersection_locals__internal_in_2, __pyx_n_s_genomictools); if (unlikely(!gen)) __PYX_ERR(0, 449, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_12genomictools_12intersection_2generator8, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_internal_intersection, __pyx_n_s_intersection_locals__internal_in_2, __pyx_n_s_genomictools); if (unlikely(!gen)) __PYX_ERR(0, 449, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_AddTraceback("genomictools.intersection._internal_intersection", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
-  __Pyx_XDECREF(__pyx_gb_12genomictools_12intersection_22_internal_intersection_2generator8);
+  __Pyx_XDECREF(__pyx_gb_12genomictools_12intersection_22_internal_intersection_2generator9);
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_gb_12genomictools_12intersection_2generator7(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
+static PyObject *__pyx_gb_12genomictools_12intersection_2generator8(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
 {
   struct __pyx_obj_12genomictools___pyx_scope_struct_6__internal_intersection *__pyx_cur_scope = ((struct __pyx_obj_12genomictools___pyx_scope_struct_6__internal_intersection *)__pyx_generator->closure);
   PyObject *__pyx_r = NULL;
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t __pyx_t_2;
   PyObject *(*__pyx_t_3)(PyObject *);
   PyObject *__pyx_t_4 = NULL;
@@ -11399,24 +11431,301 @@
   return __pyx_r;
 }
 static PyObject *__pyx_gb_12genomictools_8generator5(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
 /* "genomictools/__init__.pyx":498
  * 
  * @cython.binding(True)
+ * def add(*genomic_collections):             # <<<<<<<<<<<<<<
+ * 	'''
+ * 	Return all regions from all genomic collections.
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_12genomictools_7add(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_12genomictools_6add[] = "add(*genomic_collections)\n\n\tReturn all regions from all genomic collections. \n\t\n\t\n\t:param genomic_collections: GenomicCollection or an iterator of sorted GenomicPos\n\t\n\t:Example:\n\t\n\t.. code-block:: python\n\t\n\t\tfrom genomictools import GenomicCollection, GenomicPos, add\n\t\t\n\t\tfor r in add(GenomicCollection([GenomicPos(\"chr1\", 1, 10), GenomicPos(\"chr1\", 15, 20), GenomicPos(\"chr1\", 22, 24)]),\n\t\t               GenomicCollection([GenomicPos(\"chr1\", 8, 12), GenomicPos(\"chr1\", 14, 21)])):\n\t\t\tprint(r.name, r.start, r.stop)\n\t\t# chr1 1 10\n\t\t# chr1 8 12\n\t\t# chr1 14 21\n\t\t# chr1 15 20\n\t\t# chr1 22 24\n\t";
+static PyMethodDef __pyx_mdef_12genomictools_7add = {"add", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_12genomictools_7add, METH_VARARGS|METH_KEYWORDS, __pyx_doc_12genomictools_6add};
+static PyObject *__pyx_pw_12genomictools_7add(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_genomic_collections = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("add (wrapper)", 0);
+  if (unlikely(__pyx_kwds) && unlikely(PyDict_Size(__pyx_kwds) > 0) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "add", 0))) return NULL;
+  __Pyx_INCREF(__pyx_args);
+  __pyx_v_genomic_collections = __pyx_args;
+  __pyx_r = __pyx_pf_12genomictools_6add(__pyx_self, __pyx_v_genomic_collections);
+
+  /* function exit code */
+  __Pyx_XDECREF(__pyx_v_genomic_collections);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "genomictools/__init__.pyx":520
+ * 		# chr1 22 24
+ * 	'''
+ * 	for r in heapq.merge(*genomic_collections, key=lambda k: k.genomic_pos):             # <<<<<<<<<<<<<<
+ * 		yield r
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_12genomictools_3add_lambda5(PyObject *__pyx_self, PyObject *__pyx_v_k); /*proto*/
+static PyMethodDef __pyx_mdef_12genomictools_3add_lambda5 = {"lambda5", (PyCFunction)__pyx_pw_12genomictools_3add_lambda5, METH_O, 0};
+static PyObject *__pyx_pw_12genomictools_3add_lambda5(PyObject *__pyx_self, PyObject *__pyx_v_k) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("lambda5 (wrapper)", 0);
+  __pyx_r = __pyx_lambda_funcdef_lambda5(__pyx_self, ((PyObject *)__pyx_v_k));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_lambda_funcdef_lambda5(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_k) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("lambda5", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_k, __pyx_n_s_genomic_pos); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 520, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("genomictools.add.lambda5", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "genomictools/__init__.pyx":498
+ * 
+ * @cython.binding(True)
+ * def add(*genomic_collections):             # <<<<<<<<<<<<<<
+ * 	'''
+ * 	Return all regions from all genomic collections.
+ */
+
+static PyObject *__pyx_pf_12genomictools_6add(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_genomic_collections) {
+  struct __pyx_obj_12genomictools___pyx_scope_struct_9_add *__pyx_cur_scope;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("add", 0);
+  __pyx_cur_scope = (struct __pyx_obj_12genomictools___pyx_scope_struct_9_add *)__pyx_tp_new_12genomictools___pyx_scope_struct_9_add(__pyx_ptype_12genomictools___pyx_scope_struct_9_add, __pyx_empty_tuple, NULL);
+  if (unlikely(!__pyx_cur_scope)) {
+    __pyx_cur_scope = ((struct __pyx_obj_12genomictools___pyx_scope_struct_9_add *)Py_None);
+    __Pyx_INCREF(Py_None);
+    __PYX_ERR(0, 498, __pyx_L1_error)
+  } else {
+    __Pyx_GOTREF(__pyx_cur_scope);
+  }
+  __pyx_cur_scope->__pyx_v_genomic_collections = __pyx_v_genomic_collections;
+  __Pyx_INCREF(__pyx_cur_scope->__pyx_v_genomic_collections);
+  __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_genomic_collections);
+  {
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_12genomictools_8generator5, __pyx_codeobj__8, (PyObject *) __pyx_cur_scope, __pyx_n_s_add, __pyx_n_s_add, __pyx_n_s_genomictools); if (unlikely(!gen)) __PYX_ERR(0, 498, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_cur_scope);
+    __Pyx_RefNannyFinishContext();
+    return (PyObject *) gen;
+  }
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("genomictools.add", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_gb_12genomictools_8generator5(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
+{
+  struct __pyx_obj_12genomictools___pyx_scope_struct_9_add *__pyx_cur_scope = ((struct __pyx_obj_12genomictools___pyx_scope_struct_9_add *)__pyx_generator->closure);
+  PyObject *__pyx_r = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  Py_ssize_t __pyx_t_4;
+  PyObject *(*__pyx_t_5)(PyObject *);
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("add", 0);
+  switch (__pyx_generator->resume_label) {
+    case 0: goto __pyx_L3_first_run;
+    case 1: goto __pyx_L6_resume_from_yield;
+    default: /* CPython raises the right error here */
+    __Pyx_RefNannyFinishContext();
+    return NULL;
+  }
+  __pyx_L3_first_run:;
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 498, __pyx_L1_error)
+
+  /* "genomictools/__init__.pyx":520
+ * 		# chr1 22 24
+ * 	'''
+ * 	for r in heapq.merge(*genomic_collections, key=lambda k: k.genomic_pos):             # <<<<<<<<<<<<<<
+ * 		yield r
+ * 
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_heapq); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 520, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_merge); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 520, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 520, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_12genomictools_3add_lambda5, 0, __pyx_n_s_add_locals_lambda, NULL, __pyx_n_s_genomictools, __pyx_d, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 520, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_key, __pyx_t_3) < 0) __PYX_ERR(0, 520, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_cur_scope->__pyx_v_genomic_collections, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 520, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (likely(PyList_CheckExact(__pyx_t_3)) || PyTuple_CheckExact(__pyx_t_3)) {
+    __pyx_t_1 = __pyx_t_3; __Pyx_INCREF(__pyx_t_1); __pyx_t_4 = 0;
+    __pyx_t_5 = NULL;
+  } else {
+    __pyx_t_4 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 520, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 520, __pyx_L1_error)
+  }
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  for (;;) {
+    if (likely(!__pyx_t_5)) {
+      if (likely(PyList_CheckExact(__pyx_t_1))) {
+        if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_1)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 520, __pyx_L1_error)
+        #else
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 520, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
+        #endif
+      } else {
+        if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 520, __pyx_L1_error)
+        #else
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 520, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
+        #endif
+      }
+    } else {
+      __pyx_t_3 = __pyx_t_5(__pyx_t_1);
+      if (unlikely(!__pyx_t_3)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(0, 520, __pyx_L1_error)
+        }
+        break;
+      }
+      __Pyx_GOTREF(__pyx_t_3);
+    }
+    __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_r);
+    __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_r, __pyx_t_3);
+    __Pyx_GIVEREF(__pyx_t_3);
+    __pyx_t_3 = 0;
+
+    /* "genomictools/__init__.pyx":521
+ * 	'''
+ * 	for r in heapq.merge(*genomic_collections, key=lambda k: k.genomic_pos):
+ * 		yield r             # <<<<<<<<<<<<<<
+ * 
+ * @cython.binding(True)
+ */
+    __Pyx_INCREF(__pyx_cur_scope->__pyx_v_r);
+    __pyx_r = __pyx_cur_scope->__pyx_v_r;
+    __Pyx_XGIVEREF(__pyx_t_1);
+    __pyx_cur_scope->__pyx_t_0 = __pyx_t_1;
+    __pyx_cur_scope->__pyx_t_1 = __pyx_t_4;
+    __pyx_cur_scope->__pyx_t_2 = __pyx_t_5;
+    __Pyx_XGIVEREF(__pyx_r);
+    __Pyx_RefNannyFinishContext();
+    __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
+    /* return from generator, yielding value */
+    __pyx_generator->resume_label = 1;
+    return __pyx_r;
+    __pyx_L6_resume_from_yield:;
+    __pyx_t_1 = __pyx_cur_scope->__pyx_t_0;
+    __pyx_cur_scope->__pyx_t_0 = 0;
+    __Pyx_XGOTREF(__pyx_t_1);
+    __pyx_t_4 = __pyx_cur_scope->__pyx_t_1;
+    __pyx_t_5 = __pyx_cur_scope->__pyx_t_2;
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 521, __pyx_L1_error)
+
+    /* "genomictools/__init__.pyx":520
+ * 		# chr1 22 24
+ * 	'''
+ * 	for r in heapq.merge(*genomic_collections, key=lambda k: k.genomic_pos):             # <<<<<<<<<<<<<<
+ * 		yield r
+ * 
+ */
+  }
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
+
+  /* "genomictools/__init__.pyx":498
+ * 
+ * @cython.binding(True)
+ * def add(*genomic_collections):             # <<<<<<<<<<<<<<
+ * 	'''
+ * 	Return all regions from all genomic collections.
+ */
+
+  /* function exit code */
+  PyErr_SetNone(PyExc_StopIteration);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_AddTraceback("add", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_r); __pyx_r = 0;
+  #if !CYTHON_USE_EXC_INFO_STACK
+  __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
+  #endif
+  __pyx_generator->resume_label = -1;
+  __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+static PyObject *__pyx_gb_12genomictools_11generator6(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
+
+/* "genomictools/__init__.pyx":524
+ * 
+ * @cython.binding(True)
  * def substract(query, *refs):             # <<<<<<<<<<<<<<
  * 	'''
  * 	Return all regions that are present in query but not in refs.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_12genomictools_7substract(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_12genomictools_6substract[] = "substract(query, *refs)\n\n\tReturn all regions that are present in query but not in refs. \n\t\n\t:param query: GenomicCollection or an iterator of sorted GenomicPos\n\t:param refs: GenomicCollection\n\t\n\t:Example:\n\t\n\t.. code-block:: python\n\t\n\t\tfrom genomictools import GenomicCollection, GenomicPos, substract\n\t\t\n\t\tfor r in substract(GenomicCollection([GenomicPos(\"chr1\", 1, 10), GenomicPos(\"chr1\", 15, 20), GenomicPos(\"chr1\", 22, 24)]),\n\t\t               GenomicCollection([GenomicPos(\"chr1\", 8, 12), GenomicPos(\"chr1\", 14, 21)])):\n\t\t\tprint(r.name, r.start, r.stop)\n\t\t# chr1 1 7\n\t\t# chr1 22 24\n\t\n\t";
-static PyMethodDef __pyx_mdef_12genomictools_7substract = {"substract", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_12genomictools_7substract, METH_VARARGS|METH_KEYWORDS, __pyx_doc_12genomictools_6substract};
-static PyObject *__pyx_pw_12genomictools_7substract(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_12genomictools_10substract(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_12genomictools_9substract[] = "substract(query, *refs)\n\n\tReturn all regions that are present in query but not in refs. \n\t\n\t:param query: GenomicCollection or an iterator of sorted GenomicPos\n\t:param refs: GenomicCollection\n\t\n\t:Example:\n\t\n\t.. code-block:: python\n\t\n\t\tfrom genomictools import GenomicCollection, GenomicPos, substract\n\t\t\n\t\tfor r in substract(GenomicCollection([GenomicPos(\"chr1\", 1, 10), GenomicPos(\"chr1\", 15, 20), GenomicPos(\"chr1\", 22, 24)]),\n\t\t               GenomicCollection([GenomicPos(\"chr1\", 8, 12), GenomicPos(\"chr1\", 14, 21)])):\n\t\t\tprint(r.name, r.start, r.stop)\n\t\t# chr1 1 7\n\t\t# chr1 22 24\n\t\n\t";
+static PyMethodDef __pyx_mdef_12genomictools_10substract = {"substract", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_12genomictools_10substract, METH_VARARGS|METH_KEYWORDS, __pyx_doc_12genomictools_9substract};
+static PyObject *__pyx_pw_12genomictools_10substract(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_query = 0;
   PyObject *__pyx_v_refs = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -11447,64 +11756,64 @@
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_query_2)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t used_pos_args = (pos_args < 1) ? pos_args : 1;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, used_pos_args, "substract") < 0)) __PYX_ERR(0, 498, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, used_pos_args, "substract") < 0)) __PYX_ERR(0, 524, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) < 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_query = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("substract", 0, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 498, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("substract", 0, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 524, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_CLEAR(__pyx_v_refs);
   __Pyx_AddTraceback("genomictools.substract", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_12genomictools_6substract(__pyx_self, __pyx_v_query, __pyx_v_refs);
+  __pyx_r = __pyx_pf_12genomictools_9substract(__pyx_self, __pyx_v_query, __pyx_v_refs);
 
   /* function exit code */
   __Pyx_XDECREF(__pyx_v_refs);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12genomictools_6substract(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_query, PyObject *__pyx_v_refs) {
-  struct __pyx_obj_12genomictools___pyx_scope_struct_9_substract *__pyx_cur_scope;
+static PyObject *__pyx_pf_12genomictools_9substract(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_query, PyObject *__pyx_v_refs) {
+  struct __pyx_obj_12genomictools___pyx_scope_struct_10_substract *__pyx_cur_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("substract", 0);
-  __pyx_cur_scope = (struct __pyx_obj_12genomictools___pyx_scope_struct_9_substract *)__pyx_tp_new_12genomictools___pyx_scope_struct_9_substract(__pyx_ptype_12genomictools___pyx_scope_struct_9_substract, __pyx_empty_tuple, NULL);
+  __pyx_cur_scope = (struct __pyx_obj_12genomictools___pyx_scope_struct_10_substract *)__pyx_tp_new_12genomictools___pyx_scope_struct_10_substract(__pyx_ptype_12genomictools___pyx_scope_struct_10_substract, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
-    __pyx_cur_scope = ((struct __pyx_obj_12genomictools___pyx_scope_struct_9_substract *)Py_None);
+    __pyx_cur_scope = ((struct __pyx_obj_12genomictools___pyx_scope_struct_10_substract *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 498, __pyx_L1_error)
+    __PYX_ERR(0, 524, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_query = __pyx_v_query;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_query);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_query);
   __pyx_cur_scope->__pyx_v_refs = __pyx_v_refs;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_refs);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_refs);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_12genomictools_8generator5, __pyx_codeobj__8, (PyObject *) __pyx_cur_scope, __pyx_n_s_substract, __pyx_n_s_substract, __pyx_n_s_genomictools); if (unlikely(!gen)) __PYX_ERR(0, 498, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_12genomictools_11generator6, __pyx_codeobj__9, (PyObject *) __pyx_cur_scope, __pyx_n_s_substract, __pyx_n_s_substract, __pyx_n_s_genomictools); if (unlikely(!gen)) __PYX_ERR(0, 524, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -11512,17 +11821,17 @@
   __pyx_r = NULL;
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_gb_12genomictools_8generator5(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
+static PyObject *__pyx_gb_12genomictools_11generator6(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
 {
-  struct __pyx_obj_12genomictools___pyx_scope_struct_9_substract *__pyx_cur_scope = ((struct __pyx_obj_12genomictools___pyx_scope_struct_9_substract *)__pyx_generator->closure);
+  struct __pyx_obj_12genomictools___pyx_scope_struct_10_substract *__pyx_cur_scope = ((struct __pyx_obj_12genomictools___pyx_scope_struct_10_substract *)__pyx_generator->closure);
   PyObject *__pyx_r = NULL;
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t __pyx_t_3;
   PyObject *(*__pyx_t_4)(PyObject *);
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
@@ -11540,225 +11849,225 @@
     case 1: goto __pyx_L9_resume_from_yield;
     case 2: goto __pyx_L11_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 498, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 524, __pyx_L1_error)
 
-  /* "genomictools/__init__.pyx":518
+  /* "genomictools/__init__.pyx":544
  * 
  * 	'''
  * 	ref = GenomicCollection(union(*refs))             # <<<<<<<<<<<<<<
  * 	for q in query:
  * 		start_pos = q.genomic_pos.start
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_union); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 518, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_union); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 544, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_cur_scope->__pyx_v_refs, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 518, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_cur_scope->__pyx_v_refs, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 544, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_12genomictools_GenomicCollection), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 518, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_12genomictools_GenomicCollection), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 544, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_cur_scope->__pyx_v_ref = ((struct __pyx_obj_12genomictools_GenomicCollection *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "genomictools/__init__.pyx":519
+  /* "genomictools/__init__.pyx":545
  * 	'''
  * 	ref = GenomicCollection(union(*refs))
  * 	for q in query:             # <<<<<<<<<<<<<<
  * 		start_pos = q.genomic_pos.start
  * 		for r in ref.find_overlaps(q):
  */
   if (likely(PyList_CheckExact(__pyx_cur_scope->__pyx_v_query)) || PyTuple_CheckExact(__pyx_cur_scope->__pyx_v_query)) {
     __pyx_t_1 = __pyx_cur_scope->__pyx_v_query; __Pyx_INCREF(__pyx_t_1); __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
-    __pyx_t_3 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_cur_scope->__pyx_v_query); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 519, __pyx_L1_error)
+    __pyx_t_3 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_cur_scope->__pyx_v_query); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 545, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 519, __pyx_L1_error)
+    __pyx_t_4 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 545, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_2); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 519, __pyx_L1_error)
+        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_2); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 545, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 519, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 545, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       } else {
         if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_2); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 519, __pyx_L1_error)
+        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_2); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 545, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 519, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 545, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       }
     } else {
       __pyx_t_2 = __pyx_t_4(__pyx_t_1);
       if (unlikely(!__pyx_t_2)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 519, __pyx_L1_error)
+          else __PYX_ERR(0, 545, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_2);
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_q);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_q, __pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "genomictools/__init__.pyx":520
+    /* "genomictools/__init__.pyx":546
  * 	ref = GenomicCollection(union(*refs))
  * 	for q in query:
  * 		start_pos = q.genomic_pos.start             # <<<<<<<<<<<<<<
  * 		for r in ref.find_overlaps(q):
  * 			if start_pos <= r.genomic_pos.start - 1:
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_q, __pyx_n_s_genomic_pos); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 520, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_q, __pyx_n_s_genomic_pos); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 546, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_start); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 520, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_start); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 546, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_start_pos);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_start_pos, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "genomictools/__init__.pyx":521
+    /* "genomictools/__init__.pyx":547
  * 	for q in query:
  * 		start_pos = q.genomic_pos.start
  * 		for r in ref.find_overlaps(q):             # <<<<<<<<<<<<<<
  * 			if start_pos <= r.genomic_pos.start - 1:
  * 				yield(GenomicPos(q.genomic_pos.name, start_pos, r.genomic_pos.start - 1))
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_ref), __pyx_n_s_find_overlaps); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 521, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_ref), __pyx_n_s_find_overlaps); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 547, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_5 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_6, __pyx_cur_scope->__pyx_v_q) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_cur_scope->__pyx_v_q);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 521, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 547, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (likely(PyList_CheckExact(__pyx_t_5)) || PyTuple_CheckExact(__pyx_t_5)) {
       __pyx_t_2 = __pyx_t_5; __Pyx_INCREF(__pyx_t_2); __pyx_t_7 = 0;
       __pyx_t_8 = NULL;
     } else {
-      __pyx_t_7 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 521, __pyx_L1_error)
+      __pyx_t_7 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 547, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_8 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 521, __pyx_L1_error)
+      __pyx_t_8 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 547, __pyx_L1_error)
     }
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     for (;;) {
       if (likely(!__pyx_t_8)) {
         if (likely(PyList_CheckExact(__pyx_t_2))) {
           if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_2)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_7); __Pyx_INCREF(__pyx_t_5); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 521, __pyx_L1_error)
+          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_7); __Pyx_INCREF(__pyx_t_5); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 547, __pyx_L1_error)
           #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 521, __pyx_L1_error)
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 547, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         } else {
           if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_7); __Pyx_INCREF(__pyx_t_5); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 521, __pyx_L1_error)
+          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_7); __Pyx_INCREF(__pyx_t_5); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 547, __pyx_L1_error)
           #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 521, __pyx_L1_error)
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 547, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         }
       } else {
         __pyx_t_5 = __pyx_t_8(__pyx_t_2);
         if (unlikely(!__pyx_t_5)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 521, __pyx_L1_error)
+            else __PYX_ERR(0, 547, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_5);
       }
       __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_r);
       __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_r, __pyx_t_5);
       __Pyx_GIVEREF(__pyx_t_5);
       __pyx_t_5 = 0;
 
-      /* "genomictools/__init__.pyx":522
+      /* "genomictools/__init__.pyx":548
  * 		start_pos = q.genomic_pos.start
  * 		for r in ref.find_overlaps(q):
  * 			if start_pos <= r.genomic_pos.start - 1:             # <<<<<<<<<<<<<<
  * 				yield(GenomicPos(q.genomic_pos.name, start_pos, r.genomic_pos.start - 1))
  * 			start_pos = r.genomic_pos.stop + 1
  */
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_r, __pyx_n_s_genomic_pos); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 522, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_r, __pyx_n_s_genomic_pos); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 548, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_start); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 522, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_start); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 548, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_PyInt_SubtractObjC(__pyx_t_6, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 522, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_SubtractObjC(__pyx_t_6, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 548, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = PyObject_RichCompare(__pyx_cur_scope->__pyx_v_start_pos, __pyx_t_5, Py_LE); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 522, __pyx_L1_error)
+      __pyx_t_6 = PyObject_RichCompare(__pyx_cur_scope->__pyx_v_start_pos, __pyx_t_5, Py_LE); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 548, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 522, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 548, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       if (__pyx_t_9) {
 
-        /* "genomictools/__init__.pyx":523
+        /* "genomictools/__init__.pyx":549
  * 		for r in ref.find_overlaps(q):
  * 			if start_pos <= r.genomic_pos.start - 1:
  * 				yield(GenomicPos(q.genomic_pos.name, start_pos, r.genomic_pos.start - 1))             # <<<<<<<<<<<<<<
  * 			start_pos = r.genomic_pos.stop + 1
  * 		if start_pos <= q.genomic_pos.stop:
  */
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_q, __pyx_n_s_genomic_pos); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 523, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_q, __pyx_n_s_genomic_pos); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 549, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_name); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 523, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_name); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 549, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_r, __pyx_n_s_genomic_pos); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 523, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_r, __pyx_n_s_genomic_pos); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 549, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_start); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 523, __pyx_L1_error)
+        __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_start); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 549, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_10);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-        __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_t_10, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 523, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_t_10, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 549, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-        __pyx_t_10 = PyTuple_New(3); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 523, __pyx_L1_error)
+        __pyx_t_10 = PyTuple_New(3); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 549, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_10);
         __Pyx_GIVEREF(__pyx_t_5);
         PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_5);
         __Pyx_INCREF(__pyx_cur_scope->__pyx_v_start_pos);
         __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_start_pos);
         PyTuple_SET_ITEM(__pyx_t_10, 1, __pyx_cur_scope->__pyx_v_start_pos);
         __Pyx_GIVEREF(__pyx_t_6);
         PyTuple_SET_ITEM(__pyx_t_10, 2, __pyx_t_6);
         __pyx_t_5 = 0;
         __pyx_t_6 = 0;
-        __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_12genomictools_GenomicPos), __pyx_t_10, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 523, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_12genomictools_GenomicPos), __pyx_t_10, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 549, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
         __pyx_r = __pyx_t_6;
         __pyx_t_6 = 0;
         __Pyx_XGIVEREF(__pyx_t_1);
         __pyx_cur_scope->__pyx_t_0 = __pyx_t_1;
         __Pyx_XGIVEREF(__pyx_t_2);
@@ -11780,102 +12089,102 @@
         __pyx_t_2 = __pyx_cur_scope->__pyx_t_1;
         __pyx_cur_scope->__pyx_t_1 = 0;
         __Pyx_XGOTREF(__pyx_t_2);
         __pyx_t_3 = __pyx_cur_scope->__pyx_t_2;
         __pyx_t_4 = __pyx_cur_scope->__pyx_t_3;
         __pyx_t_7 = __pyx_cur_scope->__pyx_t_4;
         __pyx_t_8 = __pyx_cur_scope->__pyx_t_5;
-        if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 523, __pyx_L1_error)
+        if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 549, __pyx_L1_error)
 
-        /* "genomictools/__init__.pyx":522
+        /* "genomictools/__init__.pyx":548
  * 		start_pos = q.genomic_pos.start
  * 		for r in ref.find_overlaps(q):
  * 			if start_pos <= r.genomic_pos.start - 1:             # <<<<<<<<<<<<<<
  * 				yield(GenomicPos(q.genomic_pos.name, start_pos, r.genomic_pos.start - 1))
  * 			start_pos = r.genomic_pos.stop + 1
  */
       }
 
-      /* "genomictools/__init__.pyx":524
+      /* "genomictools/__init__.pyx":550
  * 			if start_pos <= r.genomic_pos.start - 1:
  * 				yield(GenomicPos(q.genomic_pos.name, start_pos, r.genomic_pos.start - 1))
  * 			start_pos = r.genomic_pos.stop + 1             # <<<<<<<<<<<<<<
  * 		if start_pos <= q.genomic_pos.stop:
  * 			yield(GenomicPos(q.genomic_pos.name, start_pos, q.genomic_pos.stop))
  */
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_r, __pyx_n_s_genomic_pos); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 524, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_r, __pyx_n_s_genomic_pos); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 550, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_stop); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 524, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_stop); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 550, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyInt_AddObjC(__pyx_t_10, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 524, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyInt_AddObjC(__pyx_t_10, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 550, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_GOTREF(__pyx_cur_scope->__pyx_v_start_pos);
       __Pyx_DECREF_SET(__pyx_cur_scope->__pyx_v_start_pos, __pyx_t_6);
       __Pyx_GIVEREF(__pyx_t_6);
       __pyx_t_6 = 0;
 
-      /* "genomictools/__init__.pyx":521
+      /* "genomictools/__init__.pyx":547
  * 	for q in query:
  * 		start_pos = q.genomic_pos.start
  * 		for r in ref.find_overlaps(q):             # <<<<<<<<<<<<<<
  * 			if start_pos <= r.genomic_pos.start - 1:
  * 				yield(GenomicPos(q.genomic_pos.name, start_pos, r.genomic_pos.start - 1))
  */
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "genomictools/__init__.pyx":525
+    /* "genomictools/__init__.pyx":551
  * 				yield(GenomicPos(q.genomic_pos.name, start_pos, r.genomic_pos.start - 1))
  * 			start_pos = r.genomic_pos.stop + 1
  * 		if start_pos <= q.genomic_pos.stop:             # <<<<<<<<<<<<<<
  * 			yield(GenomicPos(q.genomic_pos.name, start_pos, q.genomic_pos.stop))
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_q, __pyx_n_s_genomic_pos); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 525, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_q, __pyx_n_s_genomic_pos); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 551, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_stop); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 525, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_stop); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 551, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = PyObject_RichCompare(__pyx_cur_scope->__pyx_v_start_pos, __pyx_t_6, Py_LE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 525, __pyx_L1_error)
+    __pyx_t_2 = PyObject_RichCompare(__pyx_cur_scope->__pyx_v_start_pos, __pyx_t_6, Py_LE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 551, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 525, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 551, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (__pyx_t_9) {
 
-      /* "genomictools/__init__.pyx":526
+      /* "genomictools/__init__.pyx":552
  * 			start_pos = r.genomic_pos.stop + 1
  * 		if start_pos <= q.genomic_pos.stop:
  * 			yield(GenomicPos(q.genomic_pos.name, start_pos, q.genomic_pos.stop))             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_q, __pyx_n_s_genomic_pos); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 526, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_q, __pyx_n_s_genomic_pos); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 552, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_name); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 526, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_name); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 552, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_q, __pyx_n_s_genomic_pos); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 526, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_q, __pyx_n_s_genomic_pos); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 552, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_stop); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 526, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_stop); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 552, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 526, __pyx_L1_error)
+      __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 552, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_6);
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_start_pos);
       __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_start_pos);
       PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_cur_scope->__pyx_v_start_pos);
       __Pyx_GIVEREF(__pyx_t_10);
       PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_t_10);
       __pyx_t_6 = 0;
       __pyx_t_10 = 0;
-      __pyx_t_10 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_12genomictools_GenomicPos), __pyx_t_2, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 526, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_12genomictools_GenomicPos), __pyx_t_2, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 552, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __pyx_r = __pyx_t_10;
       __pyx_t_10 = 0;
       __Pyx_XGIVEREF(__pyx_t_1);
       __pyx_cur_scope->__pyx_t_0 = __pyx_t_1;
       __pyx_cur_scope->__pyx_t_2 = __pyx_t_3;
@@ -11888,37 +12197,37 @@
       return __pyx_r;
       __pyx_L11_resume_from_yield:;
       __pyx_t_1 = __pyx_cur_scope->__pyx_t_0;
       __pyx_cur_scope->__pyx_t_0 = 0;
       __Pyx_XGOTREF(__pyx_t_1);
       __pyx_t_3 = __pyx_cur_scope->__pyx_t_2;
       __pyx_t_4 = __pyx_cur_scope->__pyx_t_3;
-      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 526, __pyx_L1_error)
+      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 552, __pyx_L1_error)
 
-      /* "genomictools/__init__.pyx":525
+      /* "genomictools/__init__.pyx":551
  * 				yield(GenomicPos(q.genomic_pos.name, start_pos, r.genomic_pos.start - 1))
  * 			start_pos = r.genomic_pos.stop + 1
  * 		if start_pos <= q.genomic_pos.stop:             # <<<<<<<<<<<<<<
  * 			yield(GenomicPos(q.genomic_pos.name, start_pos, q.genomic_pos.stop))
  * 
  */
     }
 
-    /* "genomictools/__init__.pyx":519
+    /* "genomictools/__init__.pyx":545
  * 	'''
  * 	ref = GenomicCollection(union(*refs))
  * 	for q in query:             # <<<<<<<<<<<<<<
  * 		start_pos = q.genomic_pos.start
  * 		for r in ref.find_overlaps(q):
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
-  /* "genomictools/__init__.pyx":498
+  /* "genomictools/__init__.pyx":524
  * 
  * @cython.binding(True)
  * def substract(query, *refs):             # <<<<<<<<<<<<<<
  * 	'''
  * 	Return all regions that are present in query but not in refs.
  */
 
@@ -11946,18 +12255,18 @@
 /* "(tree fragment)":1
  * def __pyx_unpickle_GenomicPos(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_12genomictools_10__pyx_unpickle_GenomicPos(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_12genomictools_9__pyx_unpickle_GenomicPos[] = "__pyx_unpickle_GenomicPos(__pyx_type, long __pyx_checksum, __pyx_state)";
-static PyMethodDef __pyx_mdef_12genomictools_10__pyx_unpickle_GenomicPos = {"__pyx_unpickle_GenomicPos", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_12genomictools_10__pyx_unpickle_GenomicPos, METH_VARARGS|METH_KEYWORDS, __pyx_doc_12genomictools_9__pyx_unpickle_GenomicPos};
-static PyObject *__pyx_pw_12genomictools_10__pyx_unpickle_GenomicPos(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_12genomictools_13__pyx_unpickle_GenomicPos(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_12genomictools_12__pyx_unpickle_GenomicPos[] = "__pyx_unpickle_GenomicPos(__pyx_type, long __pyx_checksum, __pyx_state)";
+static PyMethodDef __pyx_mdef_12genomictools_13__pyx_unpickle_GenomicPos = {"__pyx_unpickle_GenomicPos", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_12genomictools_13__pyx_unpickle_GenomicPos, METH_VARARGS|METH_KEYWORDS, __pyx_doc_12genomictools_12__pyx_unpickle_GenomicPos};
+static PyObject *__pyx_pw_12genomictools_13__pyx_unpickle_GenomicPos(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v___pyx_type = 0;
   long __pyx_v___pyx_checksum;
   PyObject *__pyx_v___pyx_state = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -12015,22 +12324,22 @@
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_GenomicPos", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 1, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("genomictools.__pyx_unpickle_GenomicPos", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_12genomictools_9__pyx_unpickle_GenomicPos(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_12genomictools_12__pyx_unpickle_GenomicPos(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12genomictools_9__pyx_unpickle_GenomicPos(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_12genomictools_12__pyx_unpickle_GenomicPos(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
@@ -12047,15 +12356,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x6166e5c, 0x476b5f5, 0x3ca341a):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6166e5c, 0x476b5f5, 0x3ca341a) = (name, ostop, zstart))" % __pyx_checksum)
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__9, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__10, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x6166e5c, 0x476b5f5, 0x3ca341a):
@@ -12368,18 +12677,18 @@
 /* "(tree fragment)":1
  * def __pyx_unpickle_StrandedGenomicPos(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_12genomictools_12__pyx_unpickle_StrandedGenomicPos(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_12genomictools_11__pyx_unpickle_StrandedGenomicPos[] = "__pyx_unpickle_StrandedGenomicPos(__pyx_type, long __pyx_checksum, __pyx_state)";
-static PyMethodDef __pyx_mdef_12genomictools_12__pyx_unpickle_StrandedGenomicPos = {"__pyx_unpickle_StrandedGenomicPos", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_12genomictools_12__pyx_unpickle_StrandedGenomicPos, METH_VARARGS|METH_KEYWORDS, __pyx_doc_12genomictools_11__pyx_unpickle_StrandedGenomicPos};
-static PyObject *__pyx_pw_12genomictools_12__pyx_unpickle_StrandedGenomicPos(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_12genomictools_15__pyx_unpickle_StrandedGenomicPos(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_12genomictools_14__pyx_unpickle_StrandedGenomicPos[] = "__pyx_unpickle_StrandedGenomicPos(__pyx_type, long __pyx_checksum, __pyx_state)";
+static PyMethodDef __pyx_mdef_12genomictools_15__pyx_unpickle_StrandedGenomicPos = {"__pyx_unpickle_StrandedGenomicPos", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_12genomictools_15__pyx_unpickle_StrandedGenomicPos, METH_VARARGS|METH_KEYWORDS, __pyx_doc_12genomictools_14__pyx_unpickle_StrandedGenomicPos};
+static PyObject *__pyx_pw_12genomictools_15__pyx_unpickle_StrandedGenomicPos(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v___pyx_type = 0;
   long __pyx_v___pyx_checksum;
   PyObject *__pyx_v___pyx_state = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -12437,22 +12746,22 @@
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_StrandedGenomicPos", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 1, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("genomictools.__pyx_unpickle_StrandedGenomicPos", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_12genomictools_11__pyx_unpickle_StrandedGenomicPos(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_12genomictools_14__pyx_unpickle_StrandedGenomicPos(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12genomictools_11__pyx_unpickle_StrandedGenomicPos(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_12genomictools_14__pyx_unpickle_StrandedGenomicPos(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
@@ -12469,15 +12778,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x05ab566, 0x7d38a4a, 0xd55f499):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x05ab566, 0x7d38a4a, 0xd55f499) = (name, ostop, strand, zstart))" % __pyx_checksum)
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__10, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__11, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x05ab566, 0x7d38a4a, 0xd55f499):
@@ -12802,18 +13111,18 @@
 /* "(tree fragment)":1
  * def __pyx_unpickle_AbstractGenomicCollection(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_12genomictools_14__pyx_unpickle_AbstractGenomicCollection(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_12genomictools_13__pyx_unpickle_AbstractGenomicCollection[] = "__pyx_unpickle_AbstractGenomicCollection(__pyx_type, long __pyx_checksum, __pyx_state)";
-static PyMethodDef __pyx_mdef_12genomictools_14__pyx_unpickle_AbstractGenomicCollection = {"__pyx_unpickle_AbstractGenomicCollection", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_12genomictools_14__pyx_unpickle_AbstractGenomicCollection, METH_VARARGS|METH_KEYWORDS, __pyx_doc_12genomictools_13__pyx_unpickle_AbstractGenomicCollection};
-static PyObject *__pyx_pw_12genomictools_14__pyx_unpickle_AbstractGenomicCollection(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_12genomictools_17__pyx_unpickle_AbstractGenomicCollection(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_12genomictools_16__pyx_unpickle_AbstractGenomicCollection[] = "__pyx_unpickle_AbstractGenomicCollection(__pyx_type, long __pyx_checksum, __pyx_state)";
+static PyMethodDef __pyx_mdef_12genomictools_17__pyx_unpickle_AbstractGenomicCollection = {"__pyx_unpickle_AbstractGenomicCollection", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_12genomictools_17__pyx_unpickle_AbstractGenomicCollection, METH_VARARGS|METH_KEYWORDS, __pyx_doc_12genomictools_16__pyx_unpickle_AbstractGenomicCollection};
+static PyObject *__pyx_pw_12genomictools_17__pyx_unpickle_AbstractGenomicCollection(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v___pyx_type = 0;
   long __pyx_v___pyx_checksum;
   PyObject *__pyx_v___pyx_state = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -12871,22 +13180,22 @@
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_AbstractGenomicCollection", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 1, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("genomictools.__pyx_unpickle_AbstractGenomicCollection", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_12genomictools_13__pyx_unpickle_AbstractGenomicCollection(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_12genomictools_16__pyx_unpickle_AbstractGenomicCollection(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12genomictools_13__pyx_unpickle_AbstractGenomicCollection(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_12genomictools_16__pyx_unpickle_AbstractGenomicCollection(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
@@ -12903,15 +13212,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__11, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__12, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):
@@ -15185,52 +15494,169 @@
   0, /*tp_print*/
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
-static struct __pyx_obj_12genomictools___pyx_scope_struct_9_substract *__pyx_freelist_12genomictools___pyx_scope_struct_9_substract[8];
-static int __pyx_freecount_12genomictools___pyx_scope_struct_9_substract = 0;
+static struct __pyx_obj_12genomictools___pyx_scope_struct_9_add *__pyx_freelist_12genomictools___pyx_scope_struct_9_add[8];
+static int __pyx_freecount_12genomictools___pyx_scope_struct_9_add = 0;
 
-static PyObject *__pyx_tp_new_12genomictools___pyx_scope_struct_9_substract(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+static PyObject *__pyx_tp_new_12genomictools___pyx_scope_struct_9_add(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
-  if (CYTHON_COMPILING_IN_CPYTHON && likely((__pyx_freecount_12genomictools___pyx_scope_struct_9_substract > 0) & (t->tp_basicsize == sizeof(struct __pyx_obj_12genomictools___pyx_scope_struct_9_substract)))) {
-    o = (PyObject*)__pyx_freelist_12genomictools___pyx_scope_struct_9_substract[--__pyx_freecount_12genomictools___pyx_scope_struct_9_substract];
-    memset(o, 0, sizeof(struct __pyx_obj_12genomictools___pyx_scope_struct_9_substract));
+  if (CYTHON_COMPILING_IN_CPYTHON && likely((__pyx_freecount_12genomictools___pyx_scope_struct_9_add > 0) & (t->tp_basicsize == sizeof(struct __pyx_obj_12genomictools___pyx_scope_struct_9_add)))) {
+    o = (PyObject*)__pyx_freelist_12genomictools___pyx_scope_struct_9_add[--__pyx_freecount_12genomictools___pyx_scope_struct_9_add];
+    memset(o, 0, sizeof(struct __pyx_obj_12genomictools___pyx_scope_struct_9_add));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else {
     o = (*t->tp_alloc)(t, 0);
     if (unlikely(!o)) return 0;
   }
   return o;
 }
 
-static void __pyx_tp_dealloc_12genomictools___pyx_scope_struct_9_substract(PyObject *o) {
-  struct __pyx_obj_12genomictools___pyx_scope_struct_9_substract *p = (struct __pyx_obj_12genomictools___pyx_scope_struct_9_substract *)o;
+static void __pyx_tp_dealloc_12genomictools___pyx_scope_struct_9_add(PyObject *o) {
+  struct __pyx_obj_12genomictools___pyx_scope_struct_9_add *p = (struct __pyx_obj_12genomictools___pyx_scope_struct_9_add *)o;
+  PyObject_GC_UnTrack(o);
+  Py_CLEAR(p->__pyx_v_genomic_collections);
+  Py_CLEAR(p->__pyx_v_r);
+  Py_CLEAR(p->__pyx_t_0);
+  if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_12genomictools___pyx_scope_struct_9_add < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_12genomictools___pyx_scope_struct_9_add)))) {
+    __pyx_freelist_12genomictools___pyx_scope_struct_9_add[__pyx_freecount_12genomictools___pyx_scope_struct_9_add++] = ((struct __pyx_obj_12genomictools___pyx_scope_struct_9_add *)o);
+  } else {
+    (*Py_TYPE(o)->tp_free)(o);
+  }
+}
+
+static int __pyx_tp_traverse_12genomictools___pyx_scope_struct_9_add(PyObject *o, visitproc v, void *a) {
+  int e;
+  struct __pyx_obj_12genomictools___pyx_scope_struct_9_add *p = (struct __pyx_obj_12genomictools___pyx_scope_struct_9_add *)o;
+  if (p->__pyx_v_genomic_collections) {
+    e = (*v)(p->__pyx_v_genomic_collections, a); if (e) return e;
+  }
+  if (p->__pyx_v_r) {
+    e = (*v)(p->__pyx_v_r, a); if (e) return e;
+  }
+  if (p->__pyx_t_0) {
+    e = (*v)(p->__pyx_t_0, a); if (e) return e;
+  }
+  return 0;
+}
+
+static PyTypeObject __pyx_type_12genomictools___pyx_scope_struct_9_add = {
+  PyVarObject_HEAD_INIT(0, 0)
+  "genomictools.__pyx_scope_struct_9_add", /*tp_name*/
+  sizeof(struct __pyx_obj_12genomictools___pyx_scope_struct_9_add), /*tp_basicsize*/
+  0, /*tp_itemsize*/
+  __pyx_tp_dealloc_12genomictools___pyx_scope_struct_9_add, /*tp_dealloc*/
+  #if PY_VERSION_HEX < 0x030800b4
+  0, /*tp_print*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b4
+  0, /*tp_vectorcall_offset*/
+  #endif
+  0, /*tp_getattr*/
+  0, /*tp_setattr*/
+  #if PY_MAJOR_VERSION < 3
+  0, /*tp_compare*/
+  #endif
+  #if PY_MAJOR_VERSION >= 3
+  0, /*tp_as_async*/
+  #endif
+  0, /*tp_repr*/
+  0, /*tp_as_number*/
+  0, /*tp_as_sequence*/
+  0, /*tp_as_mapping*/
+  0, /*tp_hash*/
+  0, /*tp_call*/
+  0, /*tp_str*/
+  0, /*tp_getattro*/
+  0, /*tp_setattro*/
+  0, /*tp_as_buffer*/
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
+  0, /*tp_doc*/
+  __pyx_tp_traverse_12genomictools___pyx_scope_struct_9_add, /*tp_traverse*/
+  0, /*tp_clear*/
+  0, /*tp_richcompare*/
+  0, /*tp_weaklistoffset*/
+  0, /*tp_iter*/
+  0, /*tp_iternext*/
+  0, /*tp_methods*/
+  0, /*tp_members*/
+  0, /*tp_getset*/
+  0, /*tp_base*/
+  0, /*tp_dict*/
+  0, /*tp_descr_get*/
+  0, /*tp_descr_set*/
+  0, /*tp_dictoffset*/
+  0, /*tp_init*/
+  0, /*tp_alloc*/
+  __pyx_tp_new_12genomictools___pyx_scope_struct_9_add, /*tp_new*/
+  0, /*tp_free*/
+  0, /*tp_is_gc*/
+  0, /*tp_bases*/
+  0, /*tp_mro*/
+  0, /*tp_cache*/
+  0, /*tp_subclasses*/
+  0, /*tp_weaklist*/
+  0, /*tp_del*/
+  0, /*tp_version_tag*/
+  #if PY_VERSION_HEX >= 0x030400a1
+  0, /*tp_finalize*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+  0, /*tp_vectorcall*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+  0, /*tp_print*/
+  #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  0, /*tp_pypy_flags*/
+  #endif
+};
+
+static struct __pyx_obj_12genomictools___pyx_scope_struct_10_substract *__pyx_freelist_12genomictools___pyx_scope_struct_10_substract[8];
+static int __pyx_freecount_12genomictools___pyx_scope_struct_10_substract = 0;
+
+static PyObject *__pyx_tp_new_12genomictools___pyx_scope_struct_10_substract(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+  PyObject *o;
+  if (CYTHON_COMPILING_IN_CPYTHON && likely((__pyx_freecount_12genomictools___pyx_scope_struct_10_substract > 0) & (t->tp_basicsize == sizeof(struct __pyx_obj_12genomictools___pyx_scope_struct_10_substract)))) {
+    o = (PyObject*)__pyx_freelist_12genomictools___pyx_scope_struct_10_substract[--__pyx_freecount_12genomictools___pyx_scope_struct_10_substract];
+    memset(o, 0, sizeof(struct __pyx_obj_12genomictools___pyx_scope_struct_10_substract));
+    (void) PyObject_INIT(o, t);
+    PyObject_GC_Track(o);
+  } else {
+    o = (*t->tp_alloc)(t, 0);
+    if (unlikely(!o)) return 0;
+  }
+  return o;
+}
+
+static void __pyx_tp_dealloc_12genomictools___pyx_scope_struct_10_substract(PyObject *o) {
+  struct __pyx_obj_12genomictools___pyx_scope_struct_10_substract *p = (struct __pyx_obj_12genomictools___pyx_scope_struct_10_substract *)o;
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_q);
   Py_CLEAR(p->__pyx_v_query);
   Py_CLEAR(p->__pyx_v_r);
   Py_CLEAR(p->__pyx_v_ref);
   Py_CLEAR(p->__pyx_v_refs);
   Py_CLEAR(p->__pyx_v_start_pos);
   Py_CLEAR(p->__pyx_t_0);
   Py_CLEAR(p->__pyx_t_1);
-  if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_12genomictools___pyx_scope_struct_9_substract < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_12genomictools___pyx_scope_struct_9_substract)))) {
-    __pyx_freelist_12genomictools___pyx_scope_struct_9_substract[__pyx_freecount_12genomictools___pyx_scope_struct_9_substract++] = ((struct __pyx_obj_12genomictools___pyx_scope_struct_9_substract *)o);
+  if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_12genomictools___pyx_scope_struct_10_substract < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_12genomictools___pyx_scope_struct_10_substract)))) {
+    __pyx_freelist_12genomictools___pyx_scope_struct_10_substract[__pyx_freecount_12genomictools___pyx_scope_struct_10_substract++] = ((struct __pyx_obj_12genomictools___pyx_scope_struct_10_substract *)o);
   } else {
     (*Py_TYPE(o)->tp_free)(o);
   }
 }
 
-static int __pyx_tp_traverse_12genomictools___pyx_scope_struct_9_substract(PyObject *o, visitproc v, void *a) {
+static int __pyx_tp_traverse_12genomictools___pyx_scope_struct_10_substract(PyObject *o, visitproc v, void *a) {
   int e;
-  struct __pyx_obj_12genomictools___pyx_scope_struct_9_substract *p = (struct __pyx_obj_12genomictools___pyx_scope_struct_9_substract *)o;
+  struct __pyx_obj_12genomictools___pyx_scope_struct_10_substract *p = (struct __pyx_obj_12genomictools___pyx_scope_struct_10_substract *)o;
   if (p->__pyx_v_q) {
     e = (*v)(p->__pyx_v_q, a); if (e) return e;
   }
   if (p->__pyx_v_query) {
     e = (*v)(p->__pyx_v_query, a); if (e) return e;
   }
   if (p->__pyx_v_r) {
@@ -15250,20 +15676,20 @@
   }
   if (p->__pyx_t_1) {
     e = (*v)(p->__pyx_t_1, a); if (e) return e;
   }
   return 0;
 }
 
-static PyTypeObject __pyx_type_12genomictools___pyx_scope_struct_9_substract = {
+static PyTypeObject __pyx_type_12genomictools___pyx_scope_struct_10_substract = {
   PyVarObject_HEAD_INIT(0, 0)
-  "genomictools.__pyx_scope_struct_9_substract", /*tp_name*/
-  sizeof(struct __pyx_obj_12genomictools___pyx_scope_struct_9_substract), /*tp_basicsize*/
+  "genomictools.__pyx_scope_struct_10_substract", /*tp_name*/
+  sizeof(struct __pyx_obj_12genomictools___pyx_scope_struct_10_substract), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_12genomictools___pyx_scope_struct_9_substract, /*tp_dealloc*/
+  __pyx_tp_dealloc_12genomictools___pyx_scope_struct_10_substract, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -15282,15 +15708,15 @@
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
   0, /*tp_doc*/
-  __pyx_tp_traverse_12genomictools___pyx_scope_struct_9_substract, /*tp_traverse*/
+  __pyx_tp_traverse_12genomictools___pyx_scope_struct_10_substract, /*tp_traverse*/
   0, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   0, /*tp_methods*/
   0, /*tp_members*/
@@ -15298,15 +15724,15 @@
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   0, /*tp_dictoffset*/
   0, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_12genomictools___pyx_scope_struct_9_substract, /*tp_new*/
+  __pyx_tp_new_12genomictools___pyx_scope_struct_10_substract, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
@@ -15404,14 +15830,17 @@
   {&__pyx_n_u_StrandedGenomicAnnotation, __pyx_k_StrandedGenomicAnnotation, sizeof(__pyx_k_StrandedGenomicAnnotation), 0, 1, 0, 1},
   {&__pyx_n_s_StrandedGenomicPos, __pyx_k_StrandedGenomicPos, sizeof(__pyx_k_StrandedGenomicPos), 0, 0, 1, 1},
   {&__pyx_n_u_StrandedGenomicPos, __pyx_k_StrandedGenomicPos, sizeof(__pyx_k_StrandedGenomicPos), 0, 1, 0, 1},
   {&__pyx_n_s_StrandedGenomicPos___reduce_cyth, __pyx_k_StrandedGenomicPos___reduce_cyth, sizeof(__pyx_k_StrandedGenomicPos___reduce_cyth), 0, 0, 1, 1},
   {&__pyx_n_s_StrandedGenomicPos___setstate_cy, __pyx_k_StrandedGenomicPos___setstate_cy, sizeof(__pyx_k_StrandedGenomicPos___setstate_cy), 0, 0, 1, 1},
   {&__pyx_n_s_StrandedGenomicPos_overlaps, __pyx_k_StrandedGenomicPos_overlaps, sizeof(__pyx_k_StrandedGenomicPos_overlaps), 0, 0, 1, 1},
   {&__pyx_kp_u__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
+  {&__pyx_n_s_add, __pyx_k_add, sizeof(__pyx_k_add), 0, 0, 1, 1},
+  {&__pyx_n_u_add, __pyx_k_add, sizeof(__pyx_k_add), 0, 1, 0, 1},
+  {&__pyx_n_s_add_locals_lambda, __pyx_k_add_locals_lambda, sizeof(__pyx_k_add_locals_lambda), 0, 0, 1, 1},
   {&__pyx_n_s_all, __pyx_k_all, sizeof(__pyx_k_all), 0, 0, 1, 1},
   {&__pyx_n_s_append, __pyx_k_append, sizeof(__pyx_k_append), 0, 0, 1, 1},
   {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_close, __pyx_k_close, sizeof(__pyx_k_close), 0, 0, 1, 1},
   {&__pyx_n_s_collections, __pyx_k_collections, sizeof(__pyx_k_collections), 0, 0, 1, 1},
   {&__pyx_n_s_compile, __pyx_k_compile, sizeof(__pyx_k_compile), 0, 0, 1, 1},
@@ -15537,213 +15966,225 @@
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x6166e5c, 0x476b5f5, 0x3ca341a):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6166e5c, 0x476b5f5, 0x3ca341a) = (name, ostop, zstart))" % __pyx_checksum)
  */
-  __pyx_tuple__9 = PyTuple_Pack(3, __pyx_int_102133340, __pyx_int_74888693, __pyx_int_63583258); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
-  __pyx_tuple__10 = PyTuple_Pack(3, __pyx_int_5944678, __pyx_int_131304010, __pyx_int_223736985); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(3, __pyx_int_102133340, __pyx_int_74888693, __pyx_int_63583258); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_tuple__11 = PyTuple_Pack(3, __pyx_int_222419149, __pyx_int_238750788, __pyx_int_228825662); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(3, __pyx_int_5944678, __pyx_int_131304010, __pyx_int_223736985); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_tuple__12 = PyTuple_Pack(3, __pyx_int_222419149, __pyx_int_238750788, __pyx_int_228825662); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__12);
+  __Pyx_GIVEREF(__pyx_tuple__12);
 
   /* "genomictools/__init__.pyx":16
  * 
  * 
  * _genomic_pos_pattern = re.compile("([^:]+):(-?[0-9]+)(?:-(-?[0-9]+))?") # Used in parsing GenomicPos string             # <<<<<<<<<<<<<<
  * _stranded_genomic_pos_pattern = re.compile("([^:]+):(-?[0-9]+)(?:-(-?[0-9]+))?:([+\\-.])")
  * 
  */
-  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_u_0_9_0_9); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 16, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__12);
-  __Pyx_GIVEREF(__pyx_tuple__12);
+  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_u_0_9_0_9); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
 
   /* "genomictools/__init__.pyx":17
  * 
  * _genomic_pos_pattern = re.compile("([^:]+):(-?[0-9]+)(?:-(-?[0-9]+))?") # Used in parsing GenomicPos string
  * _stranded_genomic_pos_pattern = re.compile("([^:]+):(-?[0-9]+)(?:-(-?[0-9]+))?:([+\\-.])")             # <<<<<<<<<<<<<<
  * 
  * @cython.auto_pickle(False)
  */
-  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_u_0_9_0_9_2); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__13);
-  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_u_0_9_0_9_2); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__14);
+  __Pyx_GIVEREF(__pyx_tuple__14);
 
   /* "genomictools/__init__.pyx":82
  * 		self.ostop = stop
  * 
  * 	cpdef bint overlaps(self, GenomicAnnotation other):             # <<<<<<<<<<<<<<
  * 		'''
  * 		check if this GenomicPos overlaps with the other GenomicPos
  */
-  __pyx_tuple__14 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_other); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 82, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_genomictools___init___pyx, __pyx_n_s_overlaps, 82, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_other); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_genomictools___init___pyx, __pyx_n_s_overlaps, 82, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 82, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_tuple__16 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
-  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__17);
+  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(1, 1, __pyx_L1_error)
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_GenomicPos, (type(self), 0x6166e5c, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_GenomicPos__set_state(self, __pyx_state)
  */
-  __pyx_tuple__18 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(1, 16, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __pyx_tuple__19 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(1, 16, __pyx_L1_error)
 
   /* "genomictools/__init__.pyx":210
  * 		self.strand = strand
  * 
  * 	cpdef bint overlaps(self, GenomicAnnotation other):             # <<<<<<<<<<<<<<
  * 		'''
  * 		check if this GenomicPos overlaps with the other GenomicPos
  */
-  __pyx_tuple__20 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_other); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 210, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__20);
-  __Pyx_GIVEREF(__pyx_tuple__20);
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_genomictools___init___pyx, __pyx_n_s_overlaps, 210, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 210, __pyx_L1_error)
+  __pyx_tuple__21 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_other); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 210, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_genomictools___init___pyx, __pyx_n_s_overlaps, 210, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 210, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_tuple__22 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__23 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(1, 1, __pyx_L1_error)
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_StrandedGenomicPos, (type(self), 0x05ab566, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_StrandedGenomicPos__set_state(self, __pyx_state)
  */
-  __pyx_tuple__24 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(1, 16, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __pyx_tuple__25 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(1, 16, __pyx_L1_error)
 
   /* "genomictools/__init__.pyx":404
  * 		return len(self.regions)
  * 
  * 	def _query(self, q):             # <<<<<<<<<<<<<<
  * 		if self.frs.find(q.genomic_pos.name.encode('utf-8')) == self.frs.end():
  * 			return []
  */
-  __pyx_tuple__26 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_q, __pyx_n_s_holders, __pyx_n_s_i); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 404, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__26);
-  __Pyx_GIVEREF(__pyx_tuple__26);
-  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_genomictools___init___pyx, __pyx_n_s_query, 404, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 404, __pyx_L1_error)
+  __pyx_tuple__27 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_q, __pyx_n_s_holders, __pyx_n_s_i); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 404, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_genomictools___init___pyx, __pyx_n_s_query, 404, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(0, 404, __pyx_L1_error)
 
   /* "genomictools/__init__.pyx":410
  * 		return [<object>i.pyObject for i in holders]
  * 
  * 	def overlaps(self, q):             # <<<<<<<<<<<<<<
  * 		if self.frs.find(q.genomic_pos.name.encode('utf-8')) == self.frs.end():
  * 			return False
  */
-  __pyx_tuple__28 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_q); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 410, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__28);
-  __Pyx_GIVEREF(__pyx_tuple__28);
-  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_genomictools___init___pyx, __pyx_n_s_overlaps, 410, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 410, __pyx_L1_error)
+  __pyx_tuple__29 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_q); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 410, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__29);
+  __Pyx_GIVEREF(__pyx_tuple__29);
+  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_genomictools___init___pyx, __pyx_n_s_overlaps, 410, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 410, __pyx_L1_error)
 
   /* "genomictools/__init__.pyx":416
  * 
  * 
  * 	def find_overlaps(self, q):             # <<<<<<<<<<<<<<
  * 		yield from self._query(q)
  * 
  */
-  __pyx_tuple__30 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_q); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 416, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__30);
-  __Pyx_GIVEREF(__pyx_tuple__30);
-  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_genomictools___init___pyx, __pyx_n_s_find_overlaps, 416, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 416, __pyx_L1_error)
+  __pyx_tuple__31 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_q); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 416, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__31);
+  __Pyx_GIVEREF(__pyx_tuple__31);
+  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_genomictools___init___pyx, __pyx_n_s_find_overlaps, 416, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 416, __pyx_L1_error)
 
   /* "genomictools/__init__.pyx":419
  * 		yield from self._query(q)
  * 
  * 	def __reduce__(self):             # <<<<<<<<<<<<<<
  * 		return (GenomicCollection, (self.regions,))
  * 
  */
-  __pyx_tuple__31 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 419, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__31);
-  __Pyx_GIVEREF(__pyx_tuple__31);
-  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_genomictools___init___pyx, __pyx_n_s_reduce, 419, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 419, __pyx_L1_error)
+  __pyx_tuple__32 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(0, 419, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__32);
+  __Pyx_GIVEREF(__pyx_tuple__32);
+  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_genomictools___init___pyx, __pyx_n_s_reduce, 419, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(0, 419, __pyx_L1_error)
 
   /* "genomictools/__init__.pyx":424
  * 
  * @cython.binding(True)
  * def intersection(*genomic_collections, mergefunc=None):             # <<<<<<<<<<<<<<
  * 	'''
  * 	Return the intersection of all genomic collections.
  */
-  __pyx_tuple__33 = PyTuple_Pack(7, __pyx_n_s_mergefunc, __pyx_n_s_genomic_collections, __pyx_n_s_internal_intersection, __pyx_n_s_internal_intersection, __pyx_n_s_giter, __pyx_n_s_intersection_generator, __pyx_n_s_genomic_collection); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 424, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__33);
-  __Pyx_GIVEREF(__pyx_tuple__33);
-  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(0, 1, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_genomictools___init___pyx, __pyx_n_s_intersection, 424, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 424, __pyx_L1_error)
+  __pyx_tuple__34 = PyTuple_Pack(7, __pyx_n_s_mergefunc, __pyx_n_s_genomic_collections, __pyx_n_s_internal_intersection, __pyx_n_s_internal_intersection, __pyx_n_s_giter, __pyx_n_s_intersection_generator, __pyx_n_s_genomic_collection); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(0, 424, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__34);
+  __Pyx_GIVEREF(__pyx_tuple__34);
+  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(0, 1, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_genomictools___init___pyx, __pyx_n_s_intersection, 424, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 424, __pyx_L1_error)
 
   /* "genomictools/__init__.pyx":463
  * 
  * @cython.binding(True)
  * def union(*genomic_collections, mergefunc=None):             # <<<<<<<<<<<<<<
  * 	'''
  * 	Return the union of all genomic collections.
  */
-  __pyx_tuple__34 = PyTuple_Pack(5, __pyx_n_s_mergefunc, __pyx_n_s_genomic_collections, __pyx_n_s_giter, __pyx_n_s_stored, __pyx_n_s_r); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(0, 463, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__34);
-  __Pyx_GIVEREF(__pyx_tuple__34);
-  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(0, 1, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_genomictools___init___pyx, __pyx_n_s_union, 463, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 463, __pyx_L1_error)
+  __pyx_tuple__35 = PyTuple_Pack(5, __pyx_n_s_mergefunc, __pyx_n_s_genomic_collections, __pyx_n_s_giter, __pyx_n_s_stored, __pyx_n_s_r); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(0, 463, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__35);
+  __Pyx_GIVEREF(__pyx_tuple__35);
+  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(0, 1, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_genomictools___init___pyx, __pyx_n_s_union, 463, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 463, __pyx_L1_error)
 
   /* "genomictools/__init__.pyx":498
  * 
  * @cython.binding(True)
+ * def add(*genomic_collections):             # <<<<<<<<<<<<<<
+ * 	'''
+ * 	Return all regions from all genomic collections.
+ */
+  __pyx_tuple__36 = PyTuple_Pack(2, __pyx_n_s_genomic_collections, __pyx_n_s_r); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(0, 498, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__36);
+  __Pyx_GIVEREF(__pyx_tuple__36);
+  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_genomictools___init___pyx, __pyx_n_s_add, 498, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 498, __pyx_L1_error)
+
+  /* "genomictools/__init__.pyx":524
+ * 
+ * @cython.binding(True)
  * def substract(query, *refs):             # <<<<<<<<<<<<<<
  * 	'''
  * 	Return all regions that are present in query but not in refs.
  */
-  __pyx_tuple__35 = PyTuple_Pack(6, __pyx_n_s_query_2, __pyx_n_s_refs, __pyx_n_s_ref, __pyx_n_s_q, __pyx_n_s_start_pos, __pyx_n_s_r); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(0, 498, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__35);
-  __Pyx_GIVEREF(__pyx_tuple__35);
-  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(1, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_genomictools___init___pyx, __pyx_n_s_substract, 498, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 498, __pyx_L1_error)
+  __pyx_tuple__37 = PyTuple_Pack(6, __pyx_n_s_query_2, __pyx_n_s_refs, __pyx_n_s_ref, __pyx_n_s_q, __pyx_n_s_start_pos, __pyx_n_s_r); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(0, 524, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__37);
+  __Pyx_GIVEREF(__pyx_tuple__37);
+  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(1, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__37, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_genomictools___init___pyx, __pyx_n_s_substract, 524, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 524, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_GenomicPos(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__36 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__36);
-  __Pyx_GIVEREF(__pyx_tuple__36);
-  __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_GenomicPos, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_tuple__38 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__38);
   __Pyx_GIVEREF(__pyx_tuple__38);
-  __pyx_codeobj__39 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__38, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_StrandedGenomicPo, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__39)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__39 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__38, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_GenomicPos, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__39)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_tuple__40 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__40);
   __Pyx_GIVEREF(__pyx_tuple__40);
-  __pyx_codeobj__41 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__40, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_AbstractGenomicCo, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__41)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__41 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__40, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_StrandedGenomicPo, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__41)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__42 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__42)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__42);
+  __Pyx_GIVEREF(__pyx_tuple__42);
+  __pyx_codeobj__43 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__42, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_AbstractGenomicCo, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__43)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -15958,22 +16399,30 @@
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_12genomictools___pyx_scope_struct_8_union.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_12genomictools___pyx_scope_struct_8_union.tp_dictoffset && __pyx_type_12genomictools___pyx_scope_struct_8_union.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_12genomictools___pyx_scope_struct_8_union.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_12genomictools___pyx_scope_struct_8_union = &__pyx_type_12genomictools___pyx_scope_struct_8_union;
-  if (PyType_Ready(&__pyx_type_12genomictools___pyx_scope_struct_9_substract) < 0) __PYX_ERR(0, 498, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_12genomictools___pyx_scope_struct_9_add) < 0) __PYX_ERR(0, 498, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_12genomictools___pyx_scope_struct_9_substract.tp_print = 0;
+  __pyx_type_12genomictools___pyx_scope_struct_9_add.tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_12genomictools___pyx_scope_struct_9_substract.tp_dictoffset && __pyx_type_12genomictools___pyx_scope_struct_9_substract.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_12genomictools___pyx_scope_struct_9_substract.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_12genomictools___pyx_scope_struct_9_add.tp_dictoffset && __pyx_type_12genomictools___pyx_scope_struct_9_add.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_12genomictools___pyx_scope_struct_9_add.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
-  __pyx_ptype_12genomictools___pyx_scope_struct_9_substract = &__pyx_type_12genomictools___pyx_scope_struct_9_substract;
+  __pyx_ptype_12genomictools___pyx_scope_struct_9_add = &__pyx_type_12genomictools___pyx_scope_struct_9_add;
+  if (PyType_Ready(&__pyx_type_12genomictools___pyx_scope_struct_10_substract) < 0) __PYX_ERR(0, 524, __pyx_L1_error)
+  #if PY_VERSION_HEX < 0x030800B1
+  __pyx_type_12genomictools___pyx_scope_struct_10_substract.tp_print = 0;
+  #endif
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_12genomictools___pyx_scope_struct_10_substract.tp_dictoffset && __pyx_type_12genomictools___pyx_scope_struct_10_substract.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_12genomictools___pyx_scope_struct_10_substract.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
+  }
+  __pyx_ptype_12genomictools___pyx_scope_struct_10_substract = &__pyx_type_12genomictools___pyx_scope_struct_10_substract;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -16265,19 +16714,19 @@
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_defaultdict, __pyx_t_1) < 0) __PYX_ERR(0, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "genomictools/__init__.pyx":13
  * from genomictools.genomic cimport GenomicPosHolder, FastRangeLookUp, vector
  * 
- * __all__ = ["GenomicAnnotation", "StrandedGenomicAnnotation", "GenomicPos", "StrandedGenomicPos", "AbstractGenomicCollection", "GenomicCollection", "union", "intersection", "substract"]             # <<<<<<<<<<<<<<
+ * __all__ = ["GenomicAnnotation", "StrandedGenomicAnnotation", "GenomicPos", "StrandedGenomicPos", "AbstractGenomicCollection", "GenomicCollection", "union", "intersection", "add", "substract"]             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = PyList_New(9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_u_GenomicAnnotation);
   __Pyx_GIVEREF(__pyx_n_u_GenomicAnnotation);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_u_GenomicAnnotation);
   __Pyx_INCREF(__pyx_n_u_StrandedGenomicAnnotation);
   __Pyx_GIVEREF(__pyx_n_u_StrandedGenomicAnnotation);
   PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_u_StrandedGenomicAnnotation);
@@ -16295,17 +16744,20 @@
   PyList_SET_ITEM(__pyx_t_2, 5, __pyx_n_u_GenomicCollection);
   __Pyx_INCREF(__pyx_n_u_union);
   __Pyx_GIVEREF(__pyx_n_u_union);
   PyList_SET_ITEM(__pyx_t_2, 6, __pyx_n_u_union);
   __Pyx_INCREF(__pyx_n_u_intersection);
   __Pyx_GIVEREF(__pyx_n_u_intersection);
   PyList_SET_ITEM(__pyx_t_2, 7, __pyx_n_u_intersection);
+  __Pyx_INCREF(__pyx_n_u_add);
+  __Pyx_GIVEREF(__pyx_n_u_add);
+  PyList_SET_ITEM(__pyx_t_2, 8, __pyx_n_u_add);
   __Pyx_INCREF(__pyx_n_u_substract);
   __Pyx_GIVEREF(__pyx_n_u_substract);
-  PyList_SET_ITEM(__pyx_t_2, 8, __pyx_n_u_substract);
+  PyList_SET_ITEM(__pyx_t_2, 9, __pyx_n_u_substract);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_all, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "genomictools/__init__.pyx":16
  * 
  * 
  * _genomic_pos_pattern = re.compile("([^:]+):(-?[0-9]+)(?:-(-?[0-9]+))?") # Used in parsing GenomicPos string             # <<<<<<<<<<<<<<
@@ -16313,15 +16765,15 @@
  * 
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_re); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_compile); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_genomic_pos_pattern, __pyx_t_2) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "genomictools/__init__.pyx":17
  * 
@@ -16331,113 +16783,113 @@
  * @cython.auto_pickle(False)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_re); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_compile); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_stranded_genomic_pos_pattern, __pyx_t_2) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "genomictools/__init__.pyx":82
  * 		self.ostop = stop
  * 
  * 	cpdef bint overlaps(self, GenomicAnnotation other):             # <<<<<<<<<<<<<<
  * 		'''
  * 		check if this GenomicPos overlaps with the other GenomicPos
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_12genomictools_10GenomicPos_3overlaps, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_GenomicPos_overlaps, NULL, __pyx_n_s_genomictools, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_12genomictools_10GenomicPos_3overlaps, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_GenomicPos_overlaps, NULL, __pyx_n_s_genomictools, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem((PyObject *)__pyx_ptype_12genomictools_GenomicPos->tp_dict, __pyx_n_s_overlaps, __pyx_t_2) < 0) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_12genomictools_GenomicPos);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_12genomictools_10GenomicPos_17__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_GenomicPos___reduce_cython, NULL, __pyx_n_s_genomictools, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_12genomictools_10GenomicPos_17__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_GenomicPos___reduce_cython, NULL, __pyx_n_s_genomictools, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem((PyObject *)__pyx_ptype_12genomictools_GenomicPos->tp_dict, __pyx_n_s_reduce_cython, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_12genomictools_GenomicPos);
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_GenomicPos, (type(self), 0x6166e5c, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_GenomicPos__set_state(self, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_12genomictools_10GenomicPos_19__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_GenomicPos___setstate_cython, NULL, __pyx_n_s_genomictools, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_12genomictools_10GenomicPos_19__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_GenomicPos___setstate_cython, NULL, __pyx_n_s_genomictools, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem((PyObject *)__pyx_ptype_12genomictools_GenomicPos->tp_dict, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_12genomictools_GenomicPos);
 
   /* "genomictools/__init__.pyx":210
  * 		self.strand = strand
  * 
  * 	cpdef bint overlaps(self, GenomicAnnotation other):             # <<<<<<<<<<<<<<
  * 		'''
  * 		check if this GenomicPos overlaps with the other GenomicPos
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_12genomictools_18StrandedGenomicPos_3overlaps, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_StrandedGenomicPos_overlaps, NULL, __pyx_n_s_genomictools, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 210, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_12genomictools_18StrandedGenomicPos_3overlaps, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_StrandedGenomicPos_overlaps, NULL, __pyx_n_s_genomictools, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem((PyObject *)__pyx_ptype_12genomictools_StrandedGenomicPos->tp_dict, __pyx_n_s_overlaps, __pyx_t_2) < 0) __PYX_ERR(0, 210, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_12genomictools_StrandedGenomicPos);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_12genomictools_18StrandedGenomicPos_17__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_StrandedGenomicPos___reduce_cyth, NULL, __pyx_n_s_genomictools, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_12genomictools_18StrandedGenomicPos_17__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_StrandedGenomicPos___reduce_cyth, NULL, __pyx_n_s_genomictools, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem((PyObject *)__pyx_ptype_12genomictools_StrandedGenomicPos->tp_dict, __pyx_n_s_reduce_cython, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_12genomictools_StrandedGenomicPos);
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_StrandedGenomicPos, (type(self), 0x05ab566, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_StrandedGenomicPos__set_state(self, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_12genomictools_18StrandedGenomicPos_19__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_StrandedGenomicPos___setstate_cy, NULL, __pyx_n_s_genomictools, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_12genomictools_18StrandedGenomicPos_19__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_StrandedGenomicPos___setstate_cy, NULL, __pyx_n_s_genomictools, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem((PyObject *)__pyx_ptype_12genomictools_StrandedGenomicPos->tp_dict, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_12genomictools_StrandedGenomicPos);
 
   /* "genomictools/__init__.pyx":404
  * 		return len(self.regions)
  * 
  * 	def _query(self, q):             # <<<<<<<<<<<<<<
  * 		if self.frs.find(q.genomic_pos.name.encode('utf-8')) == self.frs.end():
  * 			return []
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_12genomictools_17GenomicCollection_7_query, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_GenomicCollection__query, NULL, __pyx_n_s_genomictools, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 404, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_12genomictools_17GenomicCollection_7_query, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_GenomicCollection__query, NULL, __pyx_n_s_genomictools, __pyx_d, ((PyObject *)__pyx_codeobj__28)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 404, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem((PyObject *)__pyx_ptype_12genomictools_GenomicCollection->tp_dict, __pyx_n_s_query, __pyx_t_2) < 0) __PYX_ERR(0, 404, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_12genomictools_GenomicCollection);
 
   /* "genomictools/__init__.pyx":410
  * 		return [<object>i.pyObject for i in holders]
  * 
  * 	def overlaps(self, q):             # <<<<<<<<<<<<<<
  * 		if self.frs.find(q.genomic_pos.name.encode('utf-8')) == self.frs.end():
  * 			return False
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_12genomictools_17GenomicCollection_9overlaps, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_GenomicCollection_overlaps, NULL, __pyx_n_s_genomictools, __pyx_d, ((PyObject *)__pyx_codeobj__29)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 410, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_12genomictools_17GenomicCollection_9overlaps, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_GenomicCollection_overlaps, NULL, __pyx_n_s_genomictools, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 410, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem((PyObject *)__pyx_ptype_12genomictools_GenomicCollection->tp_dict, __pyx_n_s_overlaps, __pyx_t_2) < 0) __PYX_ERR(0, 410, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_12genomictools_GenomicCollection);
 
   /* "genomictools/__init__.pyx":416
  * 
@@ -16455,15 +16907,15 @@
   /* "genomictools/__init__.pyx":419
  * 		yield from self._query(q)
  * 
  * 	def __reduce__(self):             # <<<<<<<<<<<<<<
  * 		return (GenomicCollection, (self.regions,))
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_12genomictools_17GenomicCollection_14__reduce__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_GenomicCollection___reduce, NULL, __pyx_n_s_genomictools, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 419, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_12genomictools_17GenomicCollection_14__reduce__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_GenomicCollection___reduce, NULL, __pyx_n_s_genomictools, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 419, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem((PyObject *)__pyx_ptype_12genomictools_GenomicCollection->tp_dict, __pyx_n_s_reduce, __pyx_t_2) < 0) __PYX_ERR(0, 419, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_12genomictools_GenomicCollection);
 
   /* "genomictools/__init__.pyx":424
  * 
@@ -16498,51 +16950,63 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_union, __pyx_t_2) < 0) __PYX_ERR(0, 463, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "genomictools/__init__.pyx":498
  * 
  * @cython.binding(True)
+ * def add(*genomic_collections):             # <<<<<<<<<<<<<<
+ * 	'''
+ * 	Return all regions from all genomic collections.
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_12genomictools_7add, 0, __pyx_n_s_add, NULL, __pyx_n_s_genomictools, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 498, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_add, __pyx_t_2) < 0) __PYX_ERR(0, 498, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "genomictools/__init__.pyx":524
+ * 
+ * @cython.binding(True)
  * def substract(query, *refs):             # <<<<<<<<<<<<<<
  * 	'''
  * 	Return all regions that are present in query but not in refs.
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_12genomictools_7substract, 0, __pyx_n_s_substract, NULL, __pyx_n_s_genomictools, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 498, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_12genomictools_10substract, 0, __pyx_n_s_substract, NULL, __pyx_n_s_genomictools, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 524, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_substract, __pyx_t_2) < 0) __PYX_ERR(0, 498, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_substract, __pyx_t_2) < 0) __PYX_ERR(0, 524, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_GenomicPos(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_12genomictools_10__pyx_unpickle_GenomicPos, 0, __pyx_n_s_pyx_unpickle_GenomicPos, NULL, __pyx_n_s_genomictools, __pyx_d, ((PyObject *)__pyx_codeobj__37)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_12genomictools_13__pyx_unpickle_GenomicPos, 0, __pyx_n_s_pyx_unpickle_GenomicPos, NULL, __pyx_n_s_genomictools, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_GenomicPos, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "(tree fragment)":11
  *         __pyx_unpickle_GenomicPos__set_state(<GenomicPos> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_GenomicPos__set_state(GenomicPos __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_result.name = __pyx_state[0]; __pyx_result.ostop = __pyx_state[1]; __pyx_result.zstart = __pyx_state[2]
  *     if len(__pyx_state) > 3 and hasattr(__pyx_result, '__dict__'):
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_12genomictools_12__pyx_unpickle_StrandedGenomicPos, 0, __pyx_n_s_pyx_unpickle_StrandedGenomicPo, NULL, __pyx_n_s_genomictools, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_12genomictools_15__pyx_unpickle_StrandedGenomicPos, 0, __pyx_n_s_pyx_unpickle_StrandedGenomicPo, NULL, __pyx_n_s_genomictools, __pyx_d, ((PyObject *)__pyx_codeobj__41)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_StrandedGenomicPo, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_AbstractGenomicCollection(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_12genomictools_14__pyx_unpickle_AbstractGenomicCollection, NULL, __pyx_n_s_genomictools); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_12genomictools_17__pyx_unpickle_AbstractGenomicCollection, NULL, __pyx_n_s_genomictools); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_AbstractGenomicCo, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "genomictools/__init__.pyx":1
  * from cpython.ref cimport PyObject             # <<<<<<<<<<<<<<
  * from libcpp.string cimport string
@@ -20176,14 +20640,54 @@
         if (likely(next))
             return next;
     }
 #endif
     return __Pyx_PyIter_Next2Default(defval);
 }
 
+/* KeywordStringCheck */
+static int __Pyx_CheckKeywordStrings(
+    PyObject *kwdict,
+    const char* function_name,
+    int kw_allowed)
+{
+    PyObject* key = 0;
+    Py_ssize_t pos = 0;
+#if CYTHON_COMPILING_IN_PYPY
+    if (!kw_allowed && PyDict_Next(kwdict, &pos, &key, 0))
+        goto invalid_keyword;
+    return 1;
+#else
+    while (PyDict_Next(kwdict, &pos, &key, 0)) {
+        #if PY_MAJOR_VERSION < 3
+        if (unlikely(!PyString_Check(key)))
+        #endif
+            if (unlikely(!PyUnicode_Check(key)))
+                goto invalid_keyword_type;
+    }
+    if ((!kw_allowed) && unlikely(key))
+        goto invalid_keyword;
+    return 1;
+invalid_keyword_type:
+    PyErr_Format(PyExc_TypeError,
+        "%.200s() keywords must be strings", function_name);
+    return 0;
+#endif
+invalid_keyword:
+    PyErr_Format(PyExc_TypeError,
+    #if PY_MAJOR_VERSION < 3
+        "%.200s() got an unexpected keyword argument '%.200s'",
+        function_name, PyString_AsString(key));
+    #else
+        "%s() got an unexpected keyword argument '%U'",
+        function_name, key);
+    #endif
+    return 0;
+}
+
 /* PyIntBinop */
 #if !CYTHON_COMPILING_IN_PYPY
 static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, CYTHON_UNUSED long intval, int inplace, int zerodivision_check) {
     (void)inplace;
     (void)zerodivision_check;
     #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_CheckExact(op1))) {
```

### Comparing `genomictools-0.0.6/genomictools/genomic.cpp` & `genomictools-0.0.7/genomictools/genomic.cpp`

 * *Files identical despite different names*

### Comparing `genomictools-0.0.6/genomictools/genomic.h` & `genomictools-0.0.7/genomictools/genomic.h`

 * *Files identical despite different names*

### Comparing `genomictools-0.0.6/genomictools/genomic.pxd` & `genomictools-0.0.7/genomictools/genomic.pxd`

 * *Files identical despite different names*

### Comparing `genomictools-0.0.6/genomictools.egg-info/PKG-INFO` & `genomictools-0.0.7/genomictools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomictools
-Version: 0.0.6
+Version: 0.0.7
 Summary: Tools for processing genomic ranges
 Author: Alden Leung
 Author-email: alden.leung@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `genomictools-0.0.6/setup.py` & `genomictools-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 with open("README.md", "r") as readme_file:
 	readme = readme_file.read()
 
 requirements=[]
 setup(
     name='genomictools', 
-    version="0.0.6",
+    version="0.0.7",
     author="Alden Leung",
     author_email="alden.leung@gmail.com",
     description="Tools for processing genomic ranges",
     long_description=readme,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=requirements,
```

