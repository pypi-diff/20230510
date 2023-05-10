# Comparing `tmp/screeny-0.1.0.tar.gz` & `tmp/screeny-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screeny-0.1.0.tar", last modified: Tue May  9 14:23:29 2023, max compression
+gzip compressed data, was "screeny-0.2.0.tar", last modified: Wed May 10 13:57:31 2023, max compression
```

## Comparing `screeny-0.1.0.tar` & `screeny-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-05-09 14:23:29.895242 screeny-0.1.0/
--rw-r--r--   0 paulpol    (501) staff       (20)     1065 2023-04-28 17:23:56.000000 screeny-0.1.0/LICENSE
--rw-r--r--   0 paulpol    (501) staff       (20)    23170 2023-04-28 17:23:31.000000 screeny-0.1.0/LICENSE-3RD-Party.txt
--rw-r--r--   0 paulpol    (501) staff       (20)      887 2023-05-09 14:23:29.895377 screeny-0.1.0/PKG-INFO
--rw-r--r--   0 paulpol    (501) staff       (20)      507 2023-05-09 14:18:43.000000 screeny-0.1.0/README.md
-drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-05-09 14:23:29.892131 screeny-0.1.0/Screeny.egg-info/
--rw-r--r--   0 paulpol    (501) staff       (20)      887 2023-05-09 14:23:29.000000 screeny-0.1.0/Screeny.egg-info/PKG-INFO
--rw-r--r--   0 paulpol    (501) staff       (20)      428 2023-05-09 14:23:29.000000 screeny-0.1.0/Screeny.egg-info/SOURCES.txt
--rw-r--r--   0 paulpol    (501) staff       (20)        1 2023-05-09 14:23:29.000000 screeny-0.1.0/Screeny.egg-info/dependency_links.txt
--rw-r--r--   0 paulpol    (501) staff       (20)       32 2023-05-09 14:23:29.000000 screeny-0.1.0/Screeny.egg-info/requires.txt
--rw-r--r--   0 paulpol    (501) staff       (20)        8 2023-05-09 14:23:29.000000 screeny-0.1.0/Screeny.egg-info/top_level.txt
--rw-r--r--   0 paulpol    (501) staff       (20)       80 2023-04-28 18:10:34.000000 screeny-0.1.0/pyproject.toml
-drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-05-09 14:23:29.894260 screeny-0.1.0/screeny/
--rw-r--r--   0 paulpol    (501) staff       (20)       28 2023-04-28 18:03:41.000000 screeny-0.1.0/screeny/__init__.py
--rw-r--r--   0 paulpol    (501) staff       (20)      448 2023-05-09 13:48:00.000000 screeny-0.1.0/screeny/mouse.py
--rw-r--r--   0 paulpol    (501) staff       (20)     1139 2023-05-09 14:12:55.000000 screeny-0.1.0/screeny/screeny.py
--rw-r--r--   0 paulpol    (501) staff       (20)      503 2023-05-09 14:23:29.895947 screeny-0.1.0/setup.cfg
+drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-05-10 13:57:31.605181 screeny-0.2.0/
+-rw-r--r--   0 paulpol    (501) staff       (20)     1065 2023-04-28 17:23:56.000000 screeny-0.2.0/LICENSE
+-rw-r--r--   0 paulpol    (501) staff       (20)    25653 2023-05-10 13:55:29.000000 screeny-0.2.0/LICENSE-3RD-Party.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)     1617 2023-05-10 13:57:31.605320 screeny-0.2.0/PKG-INFO
+-rw-r--r--   0 paulpol    (501) staff       (20)     1236 2023-05-10 13:47:16.000000 screeny-0.2.0/README.md
+-rw-r--r--   0 paulpol    (501) staff       (20)       80 2023-05-09 15:01:19.000000 screeny-0.2.0/pyproject.toml
+drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-05-10 13:57:31.602661 screeny-0.2.0/screeny/
+-rw-r--r--   0 paulpol    (501) staff       (20)       28 2023-04-28 18:03:41.000000 screeny-0.2.0/screeny/__init__.py
+-rw-r--r--   0 paulpol    (501) staff       (20)      446 2023-05-10 13:56:04.000000 screeny-0.2.0/screeny/mouse.py
+-rw-r--r--   0 paulpol    (501) staff       (20)     4326 2023-05-10 13:36:01.000000 screeny-0.2.0/screeny/screeny.py
+drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-05-10 13:57:31.604889 screeny-0.2.0/screeny.egg-info/
+-rw-r--r--   0 paulpol    (501) staff       (20)     1617 2023-05-10 13:57:31.000000 screeny-0.2.0/screeny.egg-info/PKG-INFO
+-rw-r--r--   0 paulpol    (501) staff       (20)      274 2023-05-10 13:57:31.000000 screeny-0.2.0/screeny.egg-info/SOURCES.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)        1 2023-05-10 13:57:31.000000 screeny-0.2.0/screeny.egg-info/dependency_links.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)       43 2023-05-10 13:57:31.000000 screeny-0.2.0/screeny.egg-info/requires.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)        8 2023-05-10 13:57:31.000000 screeny-0.2.0/screeny.egg-info/top_level.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)      515 2023-05-10 13:57:31.606038 screeny-0.2.0/setup.cfg
```

### Comparing `screeny-0.1.0/LICENSE` & `screeny-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `screeny-0.1.0/LICENSE-3RD-Party.txt` & `screeny-0.2.0/LICENSE-3RD-Party.txt`

 * *Files 3% similar despite different names*

```diff
@@ -350,8 +350,60 @@
 b) Give prominent notice with the combined library that part of it is a work based on the Library, and explaining where to find the accompanying uncombined form of the same work.
 6. Revised Versions of the GNU Lesser General Public License.
 
 The Free Software Foundation may publish revised and/or new versions of the GNU Lesser General Public License from time to time. Such new versions will be similar in spirit to the present version, but may differ in detail to address new problems or concerns.
 
 Each version is given a distinguishing version number. If the Library as you received it specifies that a certain numbered version of the GNU Lesser General Public License “or any later version” applies to it, you have the option of following the terms and conditions either of that published version or of any later version published by the Free Software Foundation. If the Library as you received it does not specify a version number of the GNU Lesser General Public License, you may choose any version of the GNU Lesser General Public License ever published by the Free Software Foundation.
 
-If the Library as you received it specifies that a proxy can decide whether future versions of the GNU Lesser General Public License shall apply, that proxy's public statement of acceptance of any version is permanent authorization for you to choose that version for the Library.
+If the Library as you received it specifies that a proxy can decide whether future versions of the GNU Lesser General Public License shall apply, that proxy's public statement of acceptance of any version is permanent authorization for you to choose that version for the Library.
+
+------------------------------------------------------------------------------
+matplotlib is redistributed within screeny package.
+This license applies to matplotlib.
+
+1. This LICENSE AGREEMENT is between the Matplotlib Development Team
+("MDT"), and the Individual or Organization ("Licensee") accessing and
+otherwise using matplotlib software in source or binary form and its
+associated documentation.
+
+2. Subject to the terms and conditions of this License Agreement, MDT
+hereby grants Licensee a nonexclusive, royalty-free, world-wide license
+to reproduce, analyze, test, perform and/or display publicly, prepare
+derivative works, distribute, and otherwise use matplotlib
+alone or in any derivative version, provided, however, that MDT's
+License Agreement and MDT's notice of copyright, i.e., "Copyright (c)
+2012- Matplotlib Development Team; All Rights Reserved" are retained in
+matplotlib  alone or in any derivative version prepared by
+Licensee.
+
+3. In the event Licensee prepares a derivative work that is based on or
+incorporates matplotlib or any part thereof, and wants to
+make the derivative work available to others as provided herein, then
+Licensee hereby agrees to include in any such work a brief summary of
+the changes made to matplotlib .
+
+4. MDT is making matplotlib available to Licensee on an "AS
+IS" basis.  MDT MAKES NO REPRESENTATIONS OR WARRANTIES, EXPRESS OR
+IMPLIED.  BY WAY OF EXAMPLE, BUT NOT LIMITATION, MDT MAKES NO AND
+DISCLAIMS ANY REPRESENTATION OR WARRANTY OF MERCHANTABILITY OR FITNESS
+FOR ANY PARTICULAR PURPOSE OR THAT THE USE OF MATPLOTLIB
+WILL NOT INFRINGE ANY THIRD PARTY RIGHTS.
+
+5. MDT SHALL NOT BE LIABLE TO LICENSEE OR ANY OTHER USERS OF MATPLOTLIB
+ FOR ANY INCIDENTAL, SPECIAL, OR CONSEQUENTIAL DAMAGES OR
+LOSS AS A RESULT OF MODIFYING, DISTRIBUTING, OR OTHERWISE USING
+MATPLOTLIB , OR ANY DERIVATIVE THEREOF, EVEN IF ADVISED OF
+THE POSSIBILITY THEREOF.
+
+6. This License Agreement will automatically terminate upon a material
+breach of its terms and conditions.
+
+7. Nothing in this License Agreement shall be deemed to create any
+relationship of agency, partnership, or joint venture between MDT and
+Licensee.  This License Agreement does not grant permission to use MDT
+trademarks or trade name in a trademark sense to endorse or promote
+products or services of Licensee, or any third party.
+
+8. By copying, installing or otherwise using matplotlib ,
+Licensee agrees to be bound by the terms and conditions of this License
+Agreement.
+
```

