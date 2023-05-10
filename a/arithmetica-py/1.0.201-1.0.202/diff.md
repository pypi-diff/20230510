# Comparing `tmp/arithmetica-py-1.0.201.tar.gz` & `tmp/arithmetica-py-1.0.202.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arithmetica-py-1.0.201.tar", last modified: Tue May  9 16:45:27 2023, max compression
+gzip compressed data, was "arithmetica-py-1.0.202.tar", last modified: Wed May 10 17:01:41 2023, max compression
```

## Comparing `arithmetica-py-1.0.201.tar` & `arithmetica-py-1.0.202.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:45:27.717964 arithmetica-py-1.0.201/
--rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-05-09 16:45:00.000000 arithmetica-py-1.0.201/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-09 16:45:27.717964 arithmetica-py-1.0.201/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10391 2023-05-09 16:45:00.000000 arithmetica-py-1.0.201/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:45:27.717964 arithmetica-py-1.0.201/arithmetica_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-09 16:45:27.000000 arithmetica-py-1.0.201/arithmetica_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-09 16:45:27.000000 arithmetica-py-1.0.201/arithmetica_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 16:45:27.000000 arithmetica-py-1.0.201/arithmetica_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-09 16:45:27.000000 arithmetica-py-1.0.201/arithmetica_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 16:45:27.717964 arithmetica-py-1.0.201/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-09 16:45:00.000000 arithmetica-py-1.0.201/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:45:27.717964 arithmetica-py-1.0.201/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:45:27.717964 arithmetica-py-1.0.201/src/python-module/
--rw-r--r--   0 runner    (1001) docker     (123)   182704 2023-05-09 16:45:27.000000 arithmetica-py-1.0.201/src/python-module/libarithmetica.a
--rw-r--r--   0 runner    (1001) docker     (123)    75112 2023-05-09 16:45:27.000000 arithmetica-py-1.0.201/src/python-module/libbasic_math_operations.a
--rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-05-09 16:45:00.000000 arithmetica-py-1.0.201/src/python-module/module.c
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-09 16:45:27.000000 arithmetica-py-1.0.201/src/python-module/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:01:41.117672 arithmetica-py-1.0.202/
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-05-10 17:01:25.000000 arithmetica-py-1.0.202/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-10 17:01:41.117672 arithmetica-py-1.0.202/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10391 2023-05-10 17:01:25.000000 arithmetica-py-1.0.202/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:01:41.117672 arithmetica-py-1.0.202/arithmetica_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-10 17:01:40.000000 arithmetica-py-1.0.202/arithmetica_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-10 17:01:41.000000 arithmetica-py-1.0.202/arithmetica_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 17:01:40.000000 arithmetica-py-1.0.202/arithmetica_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-10 17:01:40.000000 arithmetica-py-1.0.202/arithmetica_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 17:01:41.117672 arithmetica-py-1.0.202/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-10 17:01:25.000000 arithmetica-py-1.0.202/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:01:41.117672 arithmetica-py-1.0.202/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:01:41.117672 arithmetica-py-1.0.202/src/python-module/
+-rw-r--r--   0 runner    (1001) docker     (123)   183374 2023-05-10 17:01:40.000000 arithmetica-py-1.0.202/src/python-module/libarithmetica.a
+-rw-r--r--   0 runner    (1001) docker     (123)    75112 2023-05-10 17:01:40.000000 arithmetica-py-1.0.202/src/python-module/libbasic_math_operations.a
+-rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-05-10 17:01:25.000000 arithmetica-py-1.0.202/src/python-module/module.c
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 17:01:40.000000 arithmetica-py-1.0.202/src/python-module/version.txt
```

### Comparing `arithmetica-py-1.0.201/LICENSE` & `arithmetica-py-1.0.202/LICENSE`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.201/README.md` & `arithmetica-py-1.0.202/README.md`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.201/setup.py` & `arithmetica-py-1.0.202/setup.py`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.201/src/python-module/libarithmetica.a` & `arithmetica-py-1.0.202/src/python-module/libarithmetica.a`

 * *Files 1% similar despite different names*

#### nm -s {}

```diff
@@ -65,14 +65,15 @@
 _ZeqRKN11arithmetica8FractionES2_ in Fraction.cpp.o
 _ZltRKN11arithmetica8FractionES2_ in Fraction.cpp.o
 create_fraction in fraction.c.o
 delete_fraction in fraction.c.o
 add_fraction in add_fraction.c.o
 multiply_fraction in multiply_fraction.c.o
 parse_fraction in parse_fraction.c.o
+arithmetica_power_fraction_round_decimal in power_fraction.c.o
 power_fraction in power_fraction.c.o
 simplify_parsed_fraction in simplify_parsed_fraction.c.o
 subtract_fraction in subtract_fraction.c.o
 equal_fraction in equal_fraction.c.o
 create_complex_number in complex_arithmetica.c.o
 delete_complex_number in complex_arithmetica.c.o
 add_complex in add_complex.c.o
@@ -609,25 +610,28 @@
                  U simplify_parsed_fraction
                  U strchr
                  U strcpy
                  U strlen
                  U strncpy
 
 power_fraction.c.o:
+                 U __stack_chk_fail
+0000000000000000 T arithmetica_power_fraction_round_decimal
                  U calloc
                  U delete_fraction
                  U divide
                  U free
                  U memcpy
                  U memmove
                  U parse_fraction
                  U power
-0000000000000000 T power_fraction
+00000000000000c0 T power_fraction
                  U realloc
                  U stpcpy
+                 U strchr
                  U strlen
                  U strncpy
 
 simplify_parsed_fraction.c.o:
 0000000000000000 r .LC0
 0000000000000002 r .LC1
                  U calloc
```

#### file list

```diff
@@ -1,8 +1,8 @@
-----------   0        0        0     3650 1970-01-01 00:00:00.000000 /
+----------   0        0        0     3696 1970-01-01 00:00:00.000000 /
 ----------   0        0        0        0 1970-01-01 00:00:00.000000 //
 ?rw-r--r--   0        0        0    22216 1970-01-01 00:00:00.000000 arithmetica.cpp.o
 ?rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 arccos.c.o
 ?rw-r--r--   0        0        0     4056 1970-01-01 00:00:00.000000 arcsin.c.o
 ?rw-r--r--   0        0        0     2328 1970-01-01 00:00:00.000000 arctan.c.o
 ?rw-r--r--   0        0        0     1768 1970-01-01 00:00:00.000000 check_accuracy.c.o
 ?rw-r--r--   0        0        0     2528 1970-01-01 00:00:00.000000 continued_fraction_to_fraction.c.o
@@ -23,15 +23,15 @@
 ?rw-r--r--   0        0        0     1808 1970-01-01 00:00:00.000000 tangent.c.o
 ?rw-r--r--   0        0        0     2856 1970-01-01 00:00:00.000000 terminating_decimal_to_fraction.c.o
 ?rw-r--r--   0        0        0    18288 1970-01-01 00:00:00.000000 Fraction.cpp.o
 ?rw-r--r--   0        0        0     1896 1970-01-01 00:00:00.000000 fraction.c.o
 ?rw-r--r--   0        0        0     2320 1970-01-01 00:00:00.000000 add_fraction.c.o
 ?rw-r--r--   0        0        0     1944 1970-01-01 00:00:00.000000 multiply_fraction.c.o
 ?rw-r--r--   0        0        0     3464 1970-01-01 00:00:00.000000 parse_fraction.c.o
-?rw-r--r--   0        0        0     3704 1970-01-01 00:00:00.000000 power_fraction.c.o
+?rw-r--r--   0        0        0     4328 1970-01-01 00:00:00.000000 power_fraction.c.o
 ?rw-r--r--   0        0        0     2736 1970-01-01 00:00:00.000000 simplify_parsed_fraction.c.o
 ?rw-r--r--   0        0        0     2336 1970-01-01 00:00:00.000000 subtract_fraction.c.o
 ?rw-r--r--   0        0        0     1568 1970-01-01 00:00:00.000000 equal_fraction.c.o
 ?rw-r--r--   0        0        0     1920 1970-01-01 00:00:00.000000 complex_arithmetica.c.o
 ?rw-r--r--   0        0        0     1768 1970-01-01 00:00:00.000000 add_complex.c.o
 ?rw-r--r--   0        0        0     3032 1970-01-01 00:00:00.000000 divide_complex.c.o
 ?rw-r--r--   0        0        0     2064 1970-01-01 00:00:00.000000 exponential_complex.c.o
```

#### power_fraction.c.o

##### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              REL (Relocatable file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x0
   Start of program headers:          0 (bytes into file)
-  Start of section headers:          2872 (bytes into file)
+  Start of section headers:          3496 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           0 (bytes)
   Number of program headers:         0
   Size of section headers:           64 (bytes)
   Number of section headers:         13
   Section header string table index: 12
```

##### readelf --wide --sections {}

```diff
@@ -1,22 +1,22 @@
-There are 13 section headers, starting at offset 0xb38:
+There are 13 section headers, starting at offset 0xda8:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
-  [ 1] .text             PROGBITS        0000000000000000 000040 00034a 00  AX  0   0 16
-  [ 2] .rela.text        RELA            0000000000000000 000648 000468 18   I 10   1  8
-  [ 3] .data             PROGBITS        0000000000000000 00038a 000000 00  WA  0   0  1
-  [ 4] .bss              NOBITS          0000000000000000 00038a 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 00038a 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 0003b6 000000 00      0   0  1
-  [ 7] .note.gnu.property NOTE            0000000000000000 0003b8 000020 00   A  0   0  8
-  [ 8] .eh_frame         PROGBITS        0000000000000000 0003d8 000068 00   A  0   0  8
-  [ 9] .rela.eh_frame    RELA            0000000000000000 000ab0 000018 18   I 10   8  8
-  [10] .symtab           SYMTAB          0000000000000000 000440 000180 18     11   3  8
-  [11] .strtab           STRTAB          0000000000000000 0005c0 000086 00      0   0  1
-  [12] .shstrtab         STRTAB          0000000000000000 000ac8 00006c 00      0   0  1
+  [ 1] .text             PROGBITS        0000000000000000 000040 000493 00  AX  0   0 16
+  [ 2] .rela.text        RELA            0000000000000000 000840 0004c8 18   I 10   1  8
+  [ 3] .data             PROGBITS        0000000000000000 0004d3 000000 00  WA  0   0  1
+  [ 4] .bss              NOBITS          0000000000000000 0004d3 000000 00  WA  0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 0004d3 00002c 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 0004ff 000000 00      0   0  1
+  [ 7] .note.gnu.property NOTE            0000000000000000 000500 000020 00   A  0   0  8
+  [ 8] .eh_frame         PROGBITS        0000000000000000 000520 000090 00   A  0   0  8
+  [ 9] .rela.eh_frame    RELA            0000000000000000 000d08 000030 18   I 10   8  8
+  [10] .symtab           SYMTAB          0000000000000000 0005b0 0001c8 18     11   3  8
+  [11] .strtab           STRTAB          0000000000000000 000778 0000c7 00      0   0  1
+  [12] .shstrtab         STRTAB          0000000000000000 000d38 00006c 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --symbols {}

```diff
@@ -1,19 +1,22 @@
 
-Symbol table '.symtab' contains 16 entries:
+Symbol table '.symtab' contains 19 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS power_fraction.c
      2: 0000000000000000     0 SECTION LOCAL  DEFAULT    1 .text
-     3: 0000000000000000   842 FUNC    GLOBAL DEFAULT    1 power_fraction
-     4: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strlen
-     5: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND calloc
-     6: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memcpy
-     7: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND divide
-     8: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND power
-     9: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strncpy
-    10: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND parse_fraction
-    11: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND free
-    12: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND delete_fraction
-    13: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memmove
-    14: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND realloc
-    15: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND stpcpy
+     3: 0000000000000000   190 FUNC    GLOBAL DEFAULT    1 arithmetica_power_fraction_round_decimal
+     4: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strchr
+     5: 00000000000000c0   979 FUNC    GLOBAL DEFAULT    1 power_fraction
+     6: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strlen
+     7: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND calloc
+     8: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memcpy
+     9: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND divide
+    10: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND power
+    11: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strncpy
+    12: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND parse_fraction
+    13: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND free
+    14: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND delete_fraction
+    15: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memmove
+    16: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND realloc
+    17: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND stpcpy
+    18: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND __stack_chk_fail
```

##### readelf --wide --relocs {}

```diff
@@ -1,54 +1,59 @@
 
-Relocation section '.rela.text' at offset 0x648 contains 47 entries:
+Relocation section '.rela.text' at offset 0x840 contains 51 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-0000000000000027  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-000000000000003d  0000000500000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000052  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-000000000000006d  0000000500000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000078  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000093  0000000500000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-000000000000009f  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-00000000000000ba  0000000500000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-00000000000000cf  0000000600000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-00000000000000e1  0000000600000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-00000000000000f1  0000000600000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000000104  0000000600000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000000116  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-000000000000012a  0000000500000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000141  0000000700000004 R_X86_64_PLT32         0000000000000000 divide - 4
-0000000000000150  0000000800000004 R_X86_64_PLT32         0000000000000000 power - 4
-000000000000016a  0000000800000004 R_X86_64_PLT32         0000000000000000 power - 4
-0000000000000175  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000181  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000194  0000000500000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-00000000000001a6  0000000900000004 R_X86_64_PLT32         0000000000000000 strncpy - 4
-00000000000001ae  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-00000000000001ba  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-00000000000001c6  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-00000000000001db  0000000900000004 R_X86_64_PLT32         0000000000000000 strncpy - 4
-00000000000001e3  0000000a00000004 R_X86_64_PLT32         0000000000000000 parse_fraction - 4
-00000000000001f6  0000000b00000004 R_X86_64_PLT32         0000000000000000 free - 4
-00000000000001fe  0000000b00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000206  0000000b00000004 R_X86_64_PLT32         0000000000000000 free - 4
-000000000000020e  0000000b00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000219  0000000c00000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-0000000000000226  0000000c00000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-0000000000000259  0000000d00000004 R_X86_64_PLT32         0000000000000000 memmove - 4
-0000000000000273  0000000500000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000284  0000000600000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000000291  0000000e00000004 R_X86_64_PLT32         0000000000000000 realloc - 4
-00000000000002a4  0000000600000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-00000000000002af  0000000e00000004 R_X86_64_PLT32         0000000000000000 realloc - 4
-00000000000002c0  0000000600000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-00000000000002c8  0000000b00000004 R_X86_64_PLT32         0000000000000000 free - 4
-00000000000002de  0000000500000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-00000000000002ee  0000000f00000004 R_X86_64_PLT32         0000000000000000 stpcpy - 4
-0000000000000305  0000000e00000004 R_X86_64_PLT32         0000000000000000 realloc - 4
-000000000000031d  0000000600000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000000328  0000000e00000004 R_X86_64_PLT32         0000000000000000 realloc - 4
-0000000000000339  0000000600000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000000341  0000000b00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000011  0000000400000004 R_X86_64_PLT32         0000000000000000 strchr - 4
+00000000000000f8  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+000000000000010e  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000122  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+000000000000013c  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+000000000000014c  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000167  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000177  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000192  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+00000000000001a5  0000000800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+00000000000001b6  0000000800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+00000000000001c8  0000000800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+00000000000001da  0000000800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+00000000000001f0  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000204  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000219  0000000900000004 R_X86_64_PLT32         0000000000000000 divide - 4
+0000000000000228  0000000a00000004 R_X86_64_PLT32         0000000000000000 power - 4
+0000000000000244  0000000a00000004 R_X86_64_PLT32         0000000000000000 power - 4
+0000000000000256  0000000300000004 R_X86_64_PLT32         0000000000000000 arithmetica_power_fraction_round_decimal - 4
+0000000000000263  0000000300000004 R_X86_64_PLT32         0000000000000000 arithmetica_power_fraction_round_decimal - 4
+0000000000000274  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000289  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000298  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+00000000000002aa  0000000b00000004 R_X86_64_PLT32         0000000000000000 strncpy - 4
+00000000000002bb  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+00000000000002d1  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+00000000000002de  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+00000000000002f0  0000000b00000004 R_X86_64_PLT32         0000000000000000 strncpy - 4
+00000000000002f8  0000000c00000004 R_X86_64_PLT32         0000000000000000 parse_fraction - 4
+000000000000030b  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000315  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+000000000000031f  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000327  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000332  0000000e00000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+000000000000033d  0000000e00000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+0000000000000381  0000000f00000004 R_X86_64_PLT32         0000000000000000 memmove - 4
+000000000000039f  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+00000000000003b2  0000000800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+00000000000003be  0000001000000004 R_X86_64_PLT32         0000000000000000 realloc - 4
+00000000000003d0  0000000800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+00000000000003db  0000001000000004 R_X86_64_PLT32         0000000000000000 realloc - 4
+00000000000003f5  0000000800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+00000000000003fe  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000416  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000428  0000001100000004 R_X86_64_PLT32         0000000000000000 stpcpy - 4
+000000000000043c  0000001000000004 R_X86_64_PLT32         0000000000000000 realloc - 4
+000000000000044f  0000000800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+000000000000046a  0000001000000004 R_X86_64_PLT32         0000000000000000 realloc - 4
+000000000000047c  0000000800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+0000000000000485  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+000000000000048f  0000001200000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
 
-Relocation section '.rela.eh_frame' at offset 0xab0 contains 1 entry:
+Relocation section '.rela.eh_frame' at offset 0xd08 contains 2 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000020  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 0
+0000000000000044  0000000200000002 R_X86_64_PC32          0000000000000000 .text + c0
```

##### readelf --wide --debug-dump=frames {}

```diff
@@ -9,49 +9,68 @@
   Return address column: 16
   Augmentation data:     1b
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_offset: r16 (rip) at cfa-8
   DW_CFA_nop
   DW_CFA_nop
 
-00000018 000000000000004c 0000001c FDE cie=00000000 pc=0000000000000000..000000000000034a
-  DW_CFA_advance_loc: 6 to 0000000000000006
+00000018 0000000000000020 0000001c FDE cie=00000000 pc=0000000000000000..00000000000000be
+  DW_CFA_advance_loc: 5 to 0000000000000005
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_offset: r3 (rbx) at cfa-16
+  DW_CFA_advance_loc1: 82 to 0000000000000057
+  DW_CFA_remember_state
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 9 to 0000000000000060
+  DW_CFA_restore_state
+  DW_CFA_advance_loc1: 69 to 00000000000000a5
+  DW_CFA_remember_state
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 11 to 00000000000000b0
+  DW_CFA_restore_state
+
+0000003c 0000000000000050 00000040 FDE cie=00000000 pc=00000000000000c0..0000000000000493
+  DW_CFA_advance_loc: 6 to 00000000000000c6
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 0000000000000008
+  DW_CFA_advance_loc: 5 to 00000000000000cb
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 5 to 000000000000000d
+  DW_CFA_advance_loc: 5 to 00000000000000d0
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 000000000000000f
+  DW_CFA_advance_loc: 2 to 00000000000000d2
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 0000000000000010
+  DW_CFA_advance_loc: 1 to 00000000000000d3
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 4 to 0000000000000014
+  DW_CFA_advance_loc: 4 to 00000000000000d7
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 4 to 0000000000000018
-  DW_CFA_def_cfa_offset: 160
-  DW_CFA_advance_loc2: 543 to 0000000000000237
+  DW_CFA_advance_loc: 7 to 00000000000000de
+  DW_CFA_def_cfa_offset: 192
+  DW_CFA_advance_loc2: 647 to 0000000000000365
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 0000000000000238
+  DW_CFA_advance_loc: 1 to 0000000000000366
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000000239
+  DW_CFA_advance_loc: 1 to 0000000000000367
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 000000000000023b
+  DW_CFA_advance_loc: 2 to 0000000000000369
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 000000000000023d
+  DW_CFA_advance_loc: 2 to 000000000000036b
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000023f
+  DW_CFA_advance_loc: 2 to 000000000000036d
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000000241
+  DW_CFA_advance_loc: 2 to 000000000000036f
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 7 to 0000000000000248
+  DW_CFA_advance_loc: 1 to 0000000000000370
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
```

##### strings --all --bytes=8 {}

```diff
@@ -1,12 +1,14 @@
-h[]A\A]A^A_
+[]A\A]A^A_
 GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
 power_fraction.c
+arithmetica_power_fraction_round_decimal
 power_fraction
 parse_fraction
 delete_fraction
+__stack_chk_fail
 .shstrtab
 .rela.text
 .comment
 .note.GNU-stack
 .note.gnu.property
 .rela.eh_frame
```

##### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -1,266 +1,357 @@
 
 
 
 Disassembly of section .text:
 
-0000000000000000 <power_fraction>:
+0000000000000000 <arithmetica_power_fraction_round_decimal>:
+arithmetica_power_fraction_round_decimal():
+	endbr64
+	push   %rbx
+	mov    (%rdi),%rdi
+	mov    %rsi,%rbx
+	mov    $0x2e,%esi
+	call   15 <arithmetica_power_fraction_round_decimal+0x15>
+ R_X86_64_PLT32	strchr-0x4
+	test   %rax,%rax
+	je     56 <arithmetica_power_fraction_round_decimal+0x56>
+	lea    0x1(%rax,%rbx,1),%rdx
+	cmpb   $0x34,(%rdx)
+	jg     60 <arithmetica_power_fraction_round_decimal+0x60>
+	movb   $0x0,(%rdx)
+	movzbl -0x1(%rdx),%ecx
+	cmp    %rdx,%rax
+	jb     48 <arithmetica_power_fraction_round_decimal+0x48>
+	jmp    51 <arithmetica_power_fraction_round_decimal+0x51>
+	nopw   0x0(%rax,%rax,1)
+	lea    -0x1(%rdx),%rcx
+	movb   $0x0,-0x1(%rdx)
+	cmp    %rcx,%rax
+	je     b0 <arithmetica_power_fraction_round_decimal+0xb0>
+	mov    %rcx,%rdx
+	movzbl -0x1(%rdx),%ecx
+	cmp    $0x30,%cl
+	je     38 <arithmetica_power_fraction_round_decimal+0x38>
+	cmp    $0x2e,%cl
+	je     a0 <arithmetica_power_fraction_round_decimal+0xa0>
+	pop    %rbx
+	ret
+	nopl   0x0(%rax,%rax,1)
+	lea    (%rax,%rbx,1),%rcx
+	movzbl (%rcx),%esi
+	cmp    $0x39,%sil
+	jne    81 <arithmetica_power_fraction_round_decimal+0x81>
+	nopl   (%rax)
+	movb   $0x30,(%rcx)
+	movzbl -0x1(%rcx),%esi
+	sub    $0x1,%rcx
+	cmp    $0x39,%sil
+	je     70 <arithmetica_power_fraction_round_decimal+0x70>
+	cmp    $0x2e,%sil
+	jne    8f <arithmetica_power_fraction_round_decimal+0x8f>
+	movzbl -0x1(%rcx),%esi
+	sub    $0x1,%rcx
+	add    $0x1,%esi
+	mov    %sil,(%rcx)
+	jmp    24 <arithmetica_power_fraction_round_decimal+0x24>
+	nopw   0x0(%rax,%rax,1)
+	movb   $0x0,-0x1(%rdx)
+	pop    %rbx
+	ret
+	cs nopw 0x0(%rax,%rax,1)
+	movzbl -0x2(%rdx),%ecx
+	mov    %rax,%rdx
+	cmp    $0x2e,%cl
+	jne    56 <arithmetica_power_fraction_round_decimal+0x56>
+	jmp    a0 <arithmetica_power_fraction_round_decimal+0xa0>
+	xchg   %ax,%ax
+
+00000000000000c0 <power_fraction>:
 power_fraction():
 	endbr64
 	push   %r15
+	mov    %rcx,%r15
 	push   %r14
 	mov    %r8,%r14
 	push   %r13
 	push   %r12
 	push   %rbp
 	mov    %rdx,%rbp
 	push   %rbx
-	sub    $0x68,%rsp
-	mov    %rcx,(%rsp)
-	mov    %rsi,0x10(%rsp)
+	sub    $0x88,%rsp
+	mov    %rsi,(%rsp)
+	mov    %fs:0x28,%rax
+	mov    %rax,0x78(%rsp)
+	xor    %eax,%eax
 	mov    %rdi,0x40(%rsp)
-	call   2b <power_fraction+0x2b>
+	call   fc <power_fraction+0x3c>
  R_X86_64_PLT32	strlen-0x4
 	mov    $0x1,%esi
 	lea    0x1(%rax),%rbx
 	mov    %rax,0x50(%rsp)
 	mov    %rbx,%rdi
-	call   41 <power_fraction+0x41>
+	call   112 <power_fraction+0x52>
  R_X86_64_PLT32	calloc-0x4
-	mov    0x10(%rsp),%r10
+	mov    (%rsp),%r10
 	mov    %rax,%r12
 	mov    %r10,%rdi
 	mov    %r10,0x38(%rsp)
-	call   56 <power_fraction+0x56>
+	call   126 <power_fraction+0x66>
  R_X86_64_PLT32	strlen-0x4
 	mov    $0x1,%esi
 	mov    %rax,0x58(%rsp)
 	add    $0x1,%rax
 	mov    %rax,%rdi
-	mov    %rax,0x18(%rsp)
-	call   71 <power_fraction+0x71>
+	mov    %rax,(%rsp)
+	call   140 <power_fraction+0x80>
  R_X86_64_PLT32	calloc-0x4
 	mov    %rbp,%rdi
+	mov    %rbp,0x18(%rsp)
 	mov    %rax,%r13
-	call   7c <power_fraction+0x7c>
+	call   150 <power_fraction+0x90>
  R_X86_64_PLT32	strlen-0x4
 	mov    $0x1,%esi
 	lea    0x1(%rax),%r9
 	mov    %rax,0x48(%rsp)
 	mov    %r9,%rdi
 	mov    %r9,0x30(%rsp)
-	call   97 <power_fraction+0x97>
+	call   16b <power_fraction+0xab>
  R_X86_64_PLT32	calloc-0x4
-	mov    (%rsp),%rdi
-	mov    %rax,%r15
-	call   a3 <power_fraction+0xa3>
+	mov    %r15,%rdi
+	mov    %r15,0x20(%rsp)
+	mov    %rax,%rbp
+	call   17b <power_fraction+0xbb>
  R_X86_64_PLT32	strlen-0x4
 	mov    $0x1,%esi
 	lea    0x1(%rax),%r8
-	mov    %rax,0x20(%rsp)
+	mov    %rax,0x10(%rsp)
 	mov    %r8,%rdi
 	mov    %r8,0x28(%rsp)
-	call   be <power_fraction+0xbe>
+	call   196 <power_fraction+0xd6>
  R_X86_64_PLT32	calloc-0x4
 	mov    0x40(%rsp),%rsi
 	mov    %rbx,%rdx
 	mov    %r12,%rdi
-	mov    %rax,0x10(%rsp)
-	call   d3 <power_fraction+0xd3>
+	mov    %rax,%r15
+	call   1a9 <power_fraction+0xe9>
  R_X86_64_PLT32	memcpy-0x4
-	mov    0x18(%rsp),%rdx
+	mov    (%rsp),%rdx
 	mov    0x38(%rsp),%rsi
 	mov    %r13,%rdi
-	call   e5 <power_fraction+0xe5>
+	call   1ba <power_fraction+0xfa>
  R_X86_64_PLT32	memcpy-0x4
 	mov    0x30(%rsp),%rdx
-	mov    %rbp,%rsi
-	mov    %r15,%rdi
-	call   f5 <power_fraction+0xf5>
+	mov    0x18(%rsp),%rsi
+	mov    %rbp,%rdi
+	call   1cc <power_fraction+0x10c>
  R_X86_64_PLT32	memcpy-0x4
 	mov    0x28(%rsp),%rdx
-	mov    (%rsp),%rsi
-	mov    0x10(%rsp),%rdi
-	call   108 <power_fraction+0x108>
- R_X86_64_PLT32	memcpy-0x4
-	cmpb   $0x2d,(%r15)
-	je     248 <power_fraction+0x248>
+	mov    0x20(%rsp),%rsi
 	mov    %r15,%rdi
-	call   11a <power_fraction+0x11a>
+	call   1de <power_fraction+0x11e>
+ R_X86_64_PLT32	memcpy-0x4
+	cmpb   $0x2d,0x0(%rbp)
+	je     370 <power_fraction+0x2b0>
+	mov    %rbp,%rdi
+	lea    0x3(%r14),%rbx
+	call   1f4 <power_fraction+0x134>
  R_X86_64_PLT32	strlen-0x4
 	mov    $0x1,%esi
-	lea    0x3(%r14,%rax,1),%rdi
-	add    0x20(%rsp),%rdi
-	call   12e <power_fraction+0x12e>
+	lea    0x6(%r14,%rax,1),%rdi
+	add    0x10(%rsp),%rdi
+	call   208 <power_fraction+0x148>
  R_X86_64_PLT32	calloc-0x4
-	mov    0x10(%rsp),%rsi
-	mov    %r14,%rcx
-	mov    %r15,%rdi
+	mov    %rbx,%rcx
+	mov    %r15,%rsi
+	mov    %rbp,%rdi
 	mov    %rax,%rdx
 	mov    %rax,(%rsp)
-	call   145 <power_fraction+0x145>
+	call   21d <power_fraction+0x15d>
  R_X86_64_PLT32	divide-0x4
 	mov    (%rsp),%rsi
-	mov    %r14,%rdx
+	mov    %rbx,%rdx
 	mov    %r12,%rdi
-	call   154 <power_fraction+0x154>
+	call   22c <power_fraction+0x16c>
  R_X86_64_PLT32	power-0x4
-	mov    (%rsp),%r10
-	mov    %r14,%rdx
+	mov    (%rsp),%r8
+	mov    %rbx,%rdx
 	mov    %r13,%rdi
-	mov    %rax,%rbp
-	mov    %r10,%rsi
-	mov    %r10,0x18(%rsp)
-	call   16e <power_fraction+0x16e>
+	mov    %rax,0x68(%rsp)
+	mov    %r8,%rsi
+	mov    %r8,0x20(%rsp)
+	call   248 <power_fraction+0x188>
  R_X86_64_PLT32	power-0x4
-	mov    %rbp,%rdi
-	mov    %rax,%r14
-	call   179 <power_fraction+0x179>
+	mov    %r14,%rsi
+	lea    0x68(%rsp),%rdi
+	mov    %rax,0x70(%rsp)
+	call   25a <power_fraction+0x19a>
+ R_X86_64_PLT32	arithmetica_power_fraction_round_decimal-0x4
+	mov    %r14,%rsi
+	lea    0x70(%rsp),%rdi
+	call   267 <power_fraction+0x1a7>
+ R_X86_64_PLT32	arithmetica_power_fraction_round_decimal-0x4
+	mov    0x68(%rsp),%r9
+	mov    %r9,%rdi
+	mov    %r9,(%rsp)
+	call   278 <power_fraction+0x1b8>
  R_X86_64_PLT32	strlen-0x4
-	mov    %r14,%rdi
-	mov    %rax,(%rsp)
-	call   185 <power_fraction+0x185>
+	mov    0x70(%rsp),%r10
+	mov    %rax,%rbx
+	mov    %r10,%rdi
+	mov    %r10,0x18(%rsp)
+	call   28d <power_fraction+0x1cd>
  R_X86_64_PLT32	strlen-0x4
-	mov    (%rsp),%rdx
 	mov    $0x1,%esi
-	lea    0x2(%rdx,%rax,1),%rdi
-	call   198 <power_fraction+0x198>
+	lea    0x2(%rbx,%rax,1),%rdi
+	call   29c <power_fraction+0x1dc>
  R_X86_64_PLT32	calloc-0x4
-	mov    (%rsp),%rdx
-	mov    %rbp,%rsi
+	mov    (%rsp),%rsi
+	mov    %rbx,%rdx
 	mov    %rax,%rdi
-	mov    %rax,%rbx
-	call   1aa <power_fraction+0x1aa>
+	mov    %rax,%r14
+	call   2ae <power_fraction+0x1ee>
  R_X86_64_PLT32	strncpy-0x4
-	mov    %rbp,%rdi
-	call   1b2 <power_fraction+0x1b2>
+	mov    (%rsp),%r9
+	mov    %r9,%rdi
+	mov    %r9,0x10(%rsp)
+	call   2bf <power_fraction+0x1ff>
  R_X86_64_PLT32	strlen-0x4
-	mov    %r14,%rdi
-	movb   $0x2f,(%rbx,%rax,1)
-	call   1be <power_fraction+0x1be>
+	mov    0x18(%rsp),%r10
+	movb   $0x2f,(%r14,%rax,1)
+	mov    %r10,%rdi
+	mov    %r10,(%rsp)
+	call   2d5 <power_fraction+0x215>
  R_X86_64_PLT32	strlen-0x4
-	mov    %rbp,%rdi
-	mov    %rax,(%rsp)
-	call   1ca <power_fraction+0x1ca>
+	mov    0x10(%rsp),%rdi
+	mov    %rax,%rbx
+	call   2e2 <power_fraction+0x222>
  R_X86_64_PLT32	strlen-0x4
-	mov    (%rsp),%rdx
-	mov    %r14,%rsi
-	lea    0x1(%rbx,%rax,1),%rdi
-	add    $0x1,%rdx
-	call   1df <power_fraction+0x1df>
+	mov    (%rsp),%rsi
+	lea    0x1(%rbx),%rdx
+	lea    0x1(%r14,%rax,1),%rdi
+	call   2f4 <power_fraction+0x234>
  R_X86_64_PLT32	strncpy-0x4
-	mov    %rbx,%rdi
-	call   1e7 <power_fraction+0x1e7>
+	mov    %r14,%rdi
+	call   2fc <power_fraction+0x23c>
  R_X86_64_PLT32	parse_fraction-0x4
-	mov    0x18(%rsp),%rdi
+	mov    0x20(%rsp),%rdi
 	mov    %rax,(%rsp)
 	mov    %rdx,0x8(%rsp)
-	call   1fa <power_fraction+0x1fa>
+	call   30f <power_fraction+0x24f>
  R_X86_64_PLT32	free-0x4
-	mov    %rbp,%rdi
-	call   202 <power_fraction+0x202>
+	mov    0x68(%rsp),%rdi
+	call   319 <power_fraction+0x259>
  R_X86_64_PLT32	free-0x4
-	mov    %r14,%rdi
-	call   20a <power_fraction+0x20a>
+	mov    0x70(%rsp),%rdi
+	call   323 <power_fraction+0x263>
  R_X86_64_PLT32	free-0x4
-	mov    %rbx,%rdi
-	call   212 <power_fraction+0x212>
+	mov    %r14,%rdi
+	call   32b <power_fraction+0x26b>
  R_X86_64_PLT32	free-0x4
 	mov    %r12,%rdi
 	mov    %r13,%rsi
-	call   21d <power_fraction+0x21d>
+	call   336 <power_fraction+0x276>
  R_X86_64_PLT32	delete_fraction-0x4
-	mov    0x10(%rsp),%rsi
-	mov    %r15,%rdi
-	call   22a <power_fraction+0x22a>
+	mov    %rbp,%rdi
+	mov    %r15,%rsi
+	call   341 <power_fraction+0x281>
  R_X86_64_PLT32	delete_fraction-0x4
 	mov    (%rsp),%rax
 	mov    0x8(%rsp),%rdx
-	add    $0x68,%rsp
+	mov    0x78(%rsp),%rcx
+	sub    %fs:0x28,%rcx
+	jne    48e <power_fraction+0x3ce>
+	add    $0x88,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
-	nopw   0x0(%rax,%rax,1)
-	mov    0x48(%rsp),%rbp
-	lea    0x1(%r15),%rsi
-	mov    %r15,%rdi
-	lea    -0x1(%rbp),%rdx
-	call   25d <power_fraction+0x25d>
+	mov    0x48(%rsp),%rax
+	lea    0x1(%rbp),%rsi
+	mov    %rbp,%rdi
+	lea    -0x1(%rax),%rdx
+	call   385 <power_fraction+0x2c5>
  R_X86_64_PLT32	memmove-0x4
+	mov    0x48(%rsp),%rax
 	cmpb   $0x2d,(%r12)
-	movb   $0x0,-0x1(%r15,%rbp,1)
 	mov    $0x1,%esi
-	je     2d8 <power_fraction+0x2d8>
+	movb   $0x0,-0x1(%rbp,%rax,1)
+	je     410 <power_fraction+0x350>
 	mov    %rbx,%rdi
-	call   277 <power_fraction+0x277>
+	call   3a3 <power_fraction+0x2e3>
  R_X86_64_PLT32	calloc-0x4
 	mov    %rbx,%rdx
 	mov    %r12,%rsi
 	mov    %rax,%rdi
-	mov    %rax,%rbp
-	call   288 <power_fraction+0x288>
+	mov    %rax,0x18(%rsp)
+	call   3b6 <power_fraction+0x2f6>
  R_X86_64_PLT32	memcpy-0x4
-	mov    0x18(%rsp),%rsi
+	mov    (%rsp),%rsi
 	mov    %r12,%rdi
-	call   295 <power_fraction+0x295>
+	call   3c2 <power_fraction+0x302>
  R_X86_64_PLT32	realloc-0x4
-	mov    0x18(%rsp),%rdx
+	mov    (%rsp),%rdx
 	mov    %r13,%rsi
 	mov    %rax,%rdi
 	mov    %rax,%r12
-	call   2a8 <power_fraction+0x2a8>
+	call   3d4 <power_fraction+0x314>
  R_X86_64_PLT32	memcpy-0x4
 	mov    %rbx,%rsi
 	mov    %r13,%rdi
-	call   2b3 <power_fraction+0x2b3>
+	call   3df <power_fraction+0x31f>
  R_X86_64_PLT32	realloc-0x4
+	mov    0x18(%rsp),%r9
 	mov    %rbx,%rdx
-	mov    %rbp,%rsi
 	mov    %rax,%rdi
 	mov    %rax,%r13
-	call   2c4 <power_fraction+0x2c4>
+	mov    %r9,%rsi
+	mov    %r9,(%rsp)
+	call   3f9 <power_fraction+0x339>
  R_X86_64_PLT32	memcpy-0x4
-	mov    %rbp,%rdi
-	call   2cc <power_fraction+0x2cc>
+	mov    (%rsp),%rdi
+	call   402 <power_fraction+0x342>
  R_X86_64_PLT32	free-0x4
-	jmp    112 <power_fraction+0x112>
-	nopl   0x0(%rax)
+	jmp    1e8 <power_fraction+0x128>
+	nopw   0x0(%rax,%rax,1)
 	mov    0x50(%rsp),%rdi
-	call   2e2 <power_fraction+0x2e2>
+	call   41a <power_fraction+0x35a>
  R_X86_64_PLT32	calloc-0x4
 	lea    0x1(%r12),%rsi
 	mov    %rax,%rdi
-	mov    %rax,%rbx
-	call   2f2 <power_fraction+0x2f2>
+	mov    %rax,0x18(%rsp)
+	call   42c <power_fraction+0x36c>
  R_X86_64_PLT32	stpcpy-0x4
 	mov    0x58(%rsp),%rsi
 	mov    %r12,%rdi
-	mov    %rax,%rbp
+	mov    %rax,%rbx
 	add    $0x2,%rsi
-	sub    %rbx,%rbp
-	call   309 <power_fraction+0x309>
+	call   440 <power_fraction+0x380>
  R_X86_64_PLT32	realloc-0x4
-	mov    0x18(%rsp),%rdx
+	mov    (%rsp),%rdx
 	mov    %r13,%rsi
-	add    $0x1,%rbp
 	lea    0x1(%rax),%rdi
 	mov    %rax,%r12
-	call   321 <power_fraction+0x321>
+	call   453 <power_fraction+0x393>
  R_X86_64_PLT32	memcpy-0x4
-	mov    %rbp,%rsi
+	mov    0x18(%rsp),%r8
 	mov    %r13,%rdi
-	call   32c <power_fraction+0x32c>
- R_X86_64_PLT32	realloc-0x4
-	mov    %rbp,%rdx
+	sub    %r8,%rbx
+	mov    %r8,(%rsp)
+	add    $0x1,%rbx
 	mov    %rbx,%rsi
+	call   46e <power_fraction+0x3ae>
+ R_X86_64_PLT32	realloc-0x4
+	mov    (%rsp),%rsi
+	mov    %rbx,%rdx
 	mov    %rax,%rdi
 	mov    %rax,%r13
-	call   33d <power_fraction+0x33d>
+	call   480 <power_fraction+0x3c0>
  R_X86_64_PLT32	memcpy-0x4
-	mov    %rbx,%rdi
-	call   345 <power_fraction+0x345>
+	mov    (%rsp),%rdi
+	call   489 <power_fraction+0x3c9>
  R_X86_64_PLT32	free-0x4
-	jmp    112 <power_fraction+0x112>
+	jmp    1e8 <power_fraction+0x128>
+	call   493 <power_fraction+0x3d3>
+ R_X86_64_PLT32	__stack_chk_fail-0x4
```

##### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -1,11 +1,13 @@
 
 Hex dump of section '.eh_frame':
  NOTE: This section has relocations against it, but these have NOT been applied to this dump.
   0x00000000 14000000 00000000 017a5200 01781001 .........zR..x..
-  0x00000010 1b0c0708 90010000 4c000000 1c000000 ........L.......
-  0x00000020 00000000 4a030000 00460e10 8f02420e ....J....F....B.
-  0x00000030 188e0345 0e208d04 420e288c 05410e30 ...E. ..B.(..A.0
-  0x00000040 8606440e 38830744 0ea00103 1f020a0e ..D.8..D........
-  0x00000050 38410e30 410e2842 0e20420e 18420e10 8A.0A.(B. B..B..
-  0x00000060 420e0847 0b000000                   B..G....
+  0x00000010 1b0c0708 90010000 20000000 1c000000 ........ .......
+  0x00000020 00000000 be000000 00450e10 83020252 .........E.....R
+  0x00000030 0a0e0849 0b02450a 0e084b0b 50000000 ...I..E...K.P...
+  0x00000040 40000000 00000000 d3030000 00460e10 @............F..
+  0x00000050 8f02450e 188e0345 0e208d04 420e288c ..E....E. ..B.(.
+  0x00000060 05410e30 8606440e 38830747 0ec00103 .A.0..D.8..G....
+  0x00000070 87020a0e 38410e30 410e2842 0e20420e ....8A.0A.(B. B.
+  0x00000080 18420e10 420e0841 0b000000 00000000 .B..B..A........
```

##### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -1,12 +1,16 @@
 
 Hex dump of section '.strtab':
   0x00000000 00706f77 65725f66 72616374 696f6e2e .power_fraction.
-  0x00000010 6300706f 7765725f 66726163 74696f6e c.power_fraction
-  0x00000020 00737472 6c656e00 63616c6c 6f63006d .strlen.calloc.m
-  0x00000030 656d6370 79006469 76696465 00706f77 emcpy.divide.pow
-  0x00000040 65720073 74726e63 70790070 61727365 er.strncpy.parse
-  0x00000050 5f667261 6374696f 6e006672 65650064 _fraction.free.d
-  0x00000060 656c6574 655f6672 61637469 6f6e006d elete_fraction.m
-  0x00000070 656d6d6f 76650072 65616c6c 6f630073 emmove.realloc.s
-  0x00000080 74706370 7900                       tpcpy.
+  0x00000010 63006172 6974686d 65746963 615f706f c.arithmetica_po
+  0x00000020 7765725f 66726163 74696f6e 5f726f75 wer_fraction_rou
+  0x00000030 6e645f64 6563696d 616c0073 74726368 nd_decimal.strch
+  0x00000040 7200706f 7765725f 66726163 74696f6e r.power_fraction
+  0x00000050 00737472 6c656e00 63616c6c 6f63006d .strlen.calloc.m
+  0x00000060 656d6370 79006469 76696465 00706f77 emcpy.divide.pow
+  0x00000070 65720073 74726e63 70790070 61727365 er.strncpy.parse
+  0x00000080 5f667261 6374696f 6e006672 65650064 _fraction.free.d
+  0x00000090 656c6574 655f6672 61637469 6f6e006d elete_fraction.m
+  0x000000a0 656d6d6f 76650072 65616c6c 6f630073 emmove.realloc.s
+  0x000000b0 74706370 79005f5f 73746163 6b5f6368 tpcpy.__stack_ch
+  0x000000c0 6b5f6661 696c00                     k_fail.
```

### Comparing `arithmetica-py-1.0.201/src/python-module/libbasic_math_operations.a` & `arithmetica-py-1.0.202/src/python-module/libbasic_math_operations.a`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.201/src/python-module/module.c` & `arithmetica-py-1.0.202/src/python-module/module.c`

 * *Files identical despite different names*

