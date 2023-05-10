# Comparing `tmp/garpix_favourite-1.0.0.tar.gz` & `tmp/garpix_favourite-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpix_favourite-1.0.0.tar", last modified: Fri Aug 20 19:02:33 2021, max compression
+gzip compressed data, was "garpix_favourite-2.0.0.tar", last modified: Wed May 10 16:12:26 2023, max compression
```

## Comparing `garpix_favourite-1.0.0.tar` & `garpix_favourite-2.0.0.tar`

### file list

```diff
@@ -1,32 +1,35 @@
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-08-20 19:02:33.357149 garpix_favourite-1.0.0/
--rw-r--r--   0 crusat     (501) staff       (20)       36 2021-08-20 19:02:33.000000 garpix_favourite-1.0.0/MANIFEST.in
--rw-r--r--   0 crusat     (501) staff       (20)     1807 2021-08-20 19:02:33.357018 garpix_favourite-1.0.0/PKG-INFO
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-08-20 19:02:33.355463 garpix_favourite-1.0.0/garpix_favourite/
--rw-r--r--   0 crusat     (501) staff       (20)       36 2021-08-20 07:19:05.000000 garpix_favourite-1.0.0/garpix_favourite/MANIFEST.in
--rw-r--r--   0 crusat     (501) staff       (20)       67 2021-08-20 07:19:05.000000 garpix_favourite-1.0.0/garpix_favourite/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-08-20 19:02:33.356865 garpix_favourite-1.0.0/garpix_favourite/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      233 2021-08-20 19:02:18.000000 garpix_favourite-1.0.0/garpix_favourite/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      443 2021-08-20 19:02:18.000000 garpix_favourite-1.0.0/garpix_favourite/__pycache__/apps.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1673 2021-08-20 19:02:19.000000 garpix_favourite-1.0.0/garpix_favourite/__pycache__/models.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      353 2021-08-20 19:02:19.000000 garpix_favourite-1.0.0/garpix_favourite/__pycache__/routers.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     3478 2021-08-20 19:02:19.000000 garpix_favourite-1.0.0/garpix_favourite/__pycache__/serializers.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      307 2021-08-20 19:02:19.000000 garpix_favourite-1.0.0/garpix_favourite/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1660 2021-08-20 19:02:19.000000 garpix_favourite-1.0.0/garpix_favourite/__pycache__/views.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      143 2021-08-20 07:19:05.000000 garpix_favourite-1.0.0/garpix_favourite/apps.py
--rw-r--r--   0 crusat     (501) staff       (20)     1325 2021-08-20 16:16:50.000000 garpix_favourite-1.0.0/garpix_favourite/models.py
--rw-r--r--   0 crusat     (501) staff       (20)      180 2021-08-20 16:16:50.000000 garpix_favourite-1.0.0/garpix_favourite/routers.py
--rw-r--r--   0 crusat     (501) staff       (20)     3333 2021-08-20 16:16:50.000000 garpix_favourite-1.0.0/garpix_favourite/serializers.py
--rw-r--r--   0 crusat     (501) staff       (20)     1055 2021-08-20 18:58:38.000000 garpix_favourite-1.0.0/garpix_favourite/setup.py
--rw-r--r--   0 crusat     (501) staff       (20)     2299 2021-08-20 16:16:50.000000 garpix_favourite-1.0.0/garpix_favourite/tests.py
--rw-r--r--   0 crusat     (501) staff       (20)      205 2021-08-20 16:16:50.000000 garpix_favourite-1.0.0/garpix_favourite/urls.py
--rw-r--r--   0 crusat     (501) staff       (20)      848 2021-08-20 16:16:50.000000 garpix_favourite-1.0.0/garpix_favourite/utils.py
--rw-r--r--   0 crusat     (501) staff       (20)     1271 2021-08-20 16:16:50.000000 garpix_favourite-1.0.0/garpix_favourite/views.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-08-20 19:02:33.356120 garpix_favourite-1.0.0/garpix_favourite.egg-info/
--rw-r--r--   0 crusat     (501) staff       (20)     1807 2021-08-20 19:02:33.000000 garpix_favourite-1.0.0/garpix_favourite.egg-info/PKG-INFO
--rw-r--r--   0 crusat     (501) staff       (20)      917 2021-08-20 19:02:33.000000 garpix_favourite-1.0.0/garpix_favourite.egg-info/SOURCES.txt
--rw-r--r--   0 crusat     (501) staff       (20)        1 2021-08-20 19:02:33.000000 garpix_favourite-1.0.0/garpix_favourite.egg-info/dependency_links.txt
--rw-r--r--   0 crusat     (501) staff       (20)        1 2021-08-20 19:02:33.000000 garpix_favourite-1.0.0/garpix_favourite.egg-info/not-zip-safe
--rw-r--r--   0 crusat     (501) staff       (20)       17 2021-08-20 19:02:33.000000 garpix_favourite-1.0.0/garpix_favourite.egg-info/requires.txt
--rw-r--r--   0 crusat     (501) staff       (20)       17 2021-08-20 19:02:33.000000 garpix_favourite-1.0.0/garpix_favourite.egg-info/top_level.txt
--rw-r--r--   0 crusat     (501) staff       (20)       38 2021-08-20 19:02:33.357189 garpix_favourite-1.0.0/setup.cfg
--rw-r--r--   0 crusat     (501) staff       (20)     1055 2021-08-20 19:02:33.000000 garpix_favourite-1.0.0/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 16:12:26.662539 garpix_favourite-2.0.0/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       36 2023-05-10 16:12:26.000000 garpix_favourite-2.0.0/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1814 2023-05-10 16:12:26.662370 garpix_favourite-2.0.0/PKG-INFO
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 16:12:26.653899 garpix_favourite-2.0.0/garpix_favourite/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      181 2023-05-10 16:11:01.000000 garpix_favourite-2.0.0/garpix_favourite/CHANGELOG.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1020 2023-05-10 16:11:01.000000 garpix_favourite-2.0.0/garpix_favourite/CONTRIBUTING.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       36 2022-11-08 08:54:41.000000 garpix_favourite-2.0.0/garpix_favourite/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1241 2023-05-10 16:11:01.000000 garpix_favourite-2.0.0/garpix_favourite/README.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       67 2022-11-08 08:54:41.000000 garpix_favourite-2.0.0/garpix_favourite/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 16:12:26.662154 garpix_favourite-2.0.0/garpix_favourite/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      241 2022-11-14 21:15:49.000000 garpix_favourite-2.0.0/garpix_favourite/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      451 2022-11-14 21:15:49.000000 garpix_favourite-2.0.0/garpix_favourite/__pycache__/apps.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1672 2023-05-10 16:11:24.000000 garpix_favourite-2.0.0/garpix_favourite/__pycache__/models.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      361 2022-11-14 21:16:38.000000 garpix_favourite-2.0.0/garpix_favourite/__pycache__/routers.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3556 2023-05-10 16:11:26.000000 garpix_favourite-2.0.0/garpix_favourite/__pycache__/serializers.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      411 2023-05-10 16:11:26.000000 garpix_favourite-2.0.0/garpix_favourite/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1940 2023-05-10 16:11:26.000000 garpix_favourite-2.0.0/garpix_favourite/__pycache__/views.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      143 2022-11-08 08:54:41.000000 garpix_favourite-2.0.0/garpix_favourite/apps.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1327 2023-05-10 16:11:01.000000 garpix_favourite-2.0.0/garpix_favourite/models.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      180 2022-11-08 08:54:41.000000 garpix_favourite-2.0.0/garpix_favourite/routers.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3405 2023-05-10 16:11:01.000000 garpix_favourite-2.0.0/garpix_favourite/serializers.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1095 2023-05-10 16:12:24.000000 garpix_favourite-2.0.0/garpix_favourite/setup.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2299 2022-11-08 08:54:41.000000 garpix_favourite-2.0.0/garpix_favourite/tests.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      289 2023-05-10 16:11:01.000000 garpix_favourite-2.0.0/garpix_favourite/urls.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      848 2022-11-08 08:54:41.000000 garpix_favourite-2.0.0/garpix_favourite/utils.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1574 2023-05-10 16:11:01.000000 garpix_favourite-2.0.0/garpix_favourite/views.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 16:12:26.660895 garpix_favourite-2.0.0/garpix_favourite.egg-info/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1814 2023-05-10 16:12:26.000000 garpix_favourite-2.0.0/garpix_favourite.egg-info/PKG-INFO
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1007 2023-05-10 16:12:26.000000 garpix_favourite-2.0.0/garpix_favourite.egg-info/SOURCES.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-10 16:12:26.000000 garpix_favourite-2.0.0/garpix_favourite.egg-info/dependency_links.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-10 16:12:26.000000 garpix_favourite-2.0.0/garpix_favourite.egg-info/not-zip-safe
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       17 2023-05-10 16:12:26.000000 garpix_favourite-2.0.0/garpix_favourite.egg-info/requires.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       17 2023-05-10 16:12:26.000000 garpix_favourite-2.0.0/garpix_favourite.egg-info/top_level.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-05-10 16:12:26.662581 garpix_favourite-2.0.0/setup.cfg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1095 2023-05-10 16:12:26.000000 garpix_favourite-2.0.0/setup.py
```

### Comparing `garpix_favourite-1.0.0/garpix_favourite/__pycache__/models.cpython-38.pyc` & `garpix_favourite-2.0.0/garpix_favourite/__pycache__/models.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Aug 20 16:16:50 2021 UTC, .py size: 1325 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-00000000: 550d 0d0a 0000 0000 72d5 1f61 2d05 0000  U.......r..a-...
+00000000: 550d 0d0a 0000 0000 15c2 5b64 2f05 0000  U.........[d/...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
+00000020: 0004 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6405 6c08 6d09 5a0a 0100 6503 8300 5a0b  d.l.m.Z...e...Z.
-00000070: 4700 6406 6407 8400 6407 6501 6a0c 8303  G.d.d...d.e.j...
-00000080: 5a0d 6408 5300 2909 e900 0000 0029 01da  Z.d.S.)......)..
-00000090: 066d 6f64 656c 7329 01da 0e67 6574 5f75  .models)...get_u
-000000a0: 7365 725f 6d6f 6465 6c29 01da 1147 656e  ser_model)...Gen
-000000b0: 6572 6963 466f 7265 6967 6e4b 6579 2901  ericForeignKey).
-000000c0: da0b 436f 6e74 656e 7454 7970 6529 01da  ..ContentType)..
-000000d0: 0c67 6574 7465 7874 5f6c 617a 7963 0000  .gettext_lazyc..
-000000e0: 0000 0000 0000 0000 0000 0000 0000 0700  ................
-000000f0: 0000 4000 0000 7384 0000 0065 005a 0164  ..@...s....e.Z.d
-00000100: 005a 0264 015a 0365 046a 0565 0665 046a  .Z.d.Z.e.j.e.e.j
-00000110: 0765 0864 0283 0164 0364 0464 058d 055a  .e.d...d.d.d...Z
-00000120: 0965 046a 0a65 0864 0683 0164 078d 015a  .e.j.e.d...d...Z
-00000130: 0b65 046a 0565 0c65 046a 0765 0864 0883  .e.j.e.e.j.e.d..
-00000140: 0164 0464 098d 045a 0d65 0e64 0a64 0b83  .d.d...Z.e.d.d..
-00000150: 025a 0f65 046a 1064 0c65 0864 0d83 0164  .Z.e.j.d.e.d...d
-00000160: 0e8d 025a 1164 0f64 1084 005a 1247 0064  ...Z.d.d...Z.G.d
-00000170: 1164 1284 0064 1283 025a 1364 1353 0029  .d...d...Z.d.S.)
-00000180: 14da 0846 6176 6f72 6974 6575 5000 0000  ...FavoriteuP...
-00000190: 0a20 2020 2020 2020 20d0 9cd0 bed0 b4d0  .        .......
-000001a0: b5d0 bbd1 8c20 22d0 98d0 b7d0 b1d1 80d0  ..... ".........
-000001b0: b0d0 bdd0 bdd0 bed0 b522 20d0 b4d0 bbd1  ........." .....
-000001c0: 8f20 d0bf d0be d0bb d18c d0b7 d0be d0b2  . ..............
-000001d0: d0b0 d182 d0b5 d0bb d18f 2e0a 2020 2020  ............    
-000001e0: da04 5573 6572 5a09 6661 766f 7269 7465  ..UserZ.favorite
-000001f0: 7346 2904 da09 6f6e 5f64 656c 6574 65da  sF)...on_delete.
-00000200: 0c76 6572 626f 7365 5f6e 616d 65da 0c72  .verbose_name..r
-00000210: 656c 6174 6564 5f6e 616d 65da 0865 6469  elated_name..edi
-00000220: 7461 626c 657a 094f 626a 6563 7420 4944  tablez.Object ID
-00000230: 2901 720a 0000 007a 0c43 6f6e 7465 6e74  ).r....z.Content
-00000240: 2074 7970 6529 0372 0900 0000 720a 0000   type).r....r...
-00000250: 0072 0c00 0000 da0c 636f 6e74 656e 745f  .r......content_
-00000260: 7479 7065 da09 6f62 6a65 6374 5f69 6454  type..object_idT
-00000270: 7a0a 4372 6561 7465 6420 6174 2902 da0c  z.Created at)...
-00000280: 6175 746f 5f6e 6f77 5f61 6464 720a 0000  auto_now_addr...
-00000290: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
-000002a0: 0000 0400 0000 4300 0000 731a 0000 0064  ......C...s....d
-000002b0: 017c 006a 006a 017c 006a 027c 006a 036a  .|.j.j.|.j.|.j.j
-000002c0: 046a 0566 0316 0053 0029 024e 7a19 5573  .j.f...S.).Nz.Us
-000002d0: 6572 2025 6920 7c20 4661 766f 7269 7465  er %i | Favorite
-000002e0: 3a20 2573 2025 7329 06da 0475 7365 72da  : %s %s)...user.
-000002f0: 0269 6472 0e00 0000 da0e 636f 6e74 656e  .idr......conten
-00000300: 745f 6f62 6a65 6374 da09 5f5f 636c 6173  t_object..__clas
-00000310: 735f 5fda 085f 5f6e 616d 655f 5f29 01da  s__..__name__)..
-00000320: 0473 656c 66a9 0072 1600 0000 fa4a 2f55  .self..r.....J/U
-00000330: 7365 7273 2f63 7275 7361 742f 7072 6f6a  sers/crusat/proj
-00000340: 6563 7473 2f67 6172 7069 785f 6661 766f  ects/garpix_favo
-00000350: 7572 6974 652f 6261 636b 656e 642f 6761  urite/backend/ga
-00000360: 7270 6978 5f66 6176 6f75 7269 7465 2f6d  rpix_favourite/m
-00000370: 6f64 656c 732e 7079 da07 5f5f 7374 725f  odels.py..__str_
-00000380: 5f21 0000 0073 0a00 0000 0001 0201 0600  _!...s..........
-00000390: 0400 08ff 7a10 4661 766f 7269 7465 2e5f  ....z.Favorite._
-000003a0: 5f73 7472 5f5f 6300 0000 0000 0000 0000  _str__c.........
-000003b0: 0000 0000 0000 0002 0000 0040 0000 0073  ...........@...s
-000003c0: 2400 0000 6500 5a01 6400 5a02 6401 5a03  $...e.Z.d.Z.d.Z.
-000003d0: 6504 6402 8301 5a05 6504 6403 8301 5a06  e.d...Z.e.d...Z.
-000003e0: 6404 5a07 6405 5300 2906 7a0d 4661 766f  d.Z.d.S.).z.Favo
-000003f0: 7269 7465 2e4d 6574 6129 0172 1100 0000  rite.Meta).r....
-00000400: 7207 0000 005a 0946 6176 6f72 6974 6573  r....Z.Favorites
-00000410: 2901 2903 7210 0000 0072 0d00 0000 720e  ).).r....r....r.
-00000420: 0000 004e 2908 7214 0000 00da 0a5f 5f6d  ...N).r......__m
-00000430: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00000440: 616d 655f 5fda 086f 7264 6572 696e 67da  ame__..ordering.
-00000450: 015f 720a 0000 00da 1376 6572 626f 7365  ._r......verbose
-00000460: 5f6e 616d 655f 706c 7572 616c da0f 756e  _name_plural..un
-00000470: 6971 7565 5f74 6f67 6574 6865 7272 1600  ique_togetherr..
-00000480: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00000490: 00da 044d 6574 6126 0000 0073 0800 0000  ...Meta&...s....
-000004a0: 0801 0401 0801 0801 721f 0000 004e 2914  ........r....N).
-000004b0: 7214 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
-000004c0: 075f 5f64 6f63 5f5f 7202 0000 00da 0a46  .__doc__r......F
-000004d0: 6f72 6569 676e 4b65 7972 0800 0000 da07  oreignKeyr......
-000004e0: 4341 5343 4144 4572 1c00 0000 7210 0000  CASCADEr....r...
-000004f0: 00da 1450 6f73 6974 6976 6549 6e74 6567  ...PositiveInteg
-00000500: 6572 4669 656c 6472 0e00 0000 7205 0000  erFieldr....r...
-00000510: 0072 0d00 0000 7204 0000 0072 1200 0000  .r....r....r....
-00000520: da0d 4461 7465 5469 6d65 4669 656c 64da  ..DateTimeField.
-00000530: 0a63 7265 6174 6564 5f61 7472 1800 0000  .created_atr....
-00000540: 721f 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
-00000550: 1600 0000 7217 0000 0072 0700 0000 0a00  ....r....r......
-00000560: 0000 7336 0000 0008 0104 0404 0102 0004  ..s6............
-00000570: 0006 0102 0002 fe06 0404 0106 ff06 0304  ................
-00000580: 0102 0004 0006 0102 fe06 0402 0102 0002  ................
-00000590: ff04 0304 0102 0006 ff06 0408 0572 0700  .............r..
-000005a0: 0000 4e29 0eda 0964 6a61 6e67 6f2e 6462  ..N)...django.db
-000005b0: 7202 0000 00da 1364 6a61 6e67 6f2e 636f  r......django.co
-000005c0: 6e74 7269 622e 6175 7468 7203 0000 005a  ntrib.authr....Z
-000005d0: 2264 6a61 6e67 6f2e 636f 6e74 7269 622e  "django.contrib.
-000005e0: 636f 6e74 656e 7474 7970 6573 2e66 6965  contenttypes.fie
-000005f0: 6c64 7372 0400 0000 da22 646a 616e 676f  ldsr....."django
-00000600: 2e63 6f6e 7472 6962 2e63 6f6e 7465 6e74  .contrib.content
-00000610: 7479 7065 732e 6d6f 6465 6c73 7205 0000  types.modelsr...
-00000620: 00da 1864 6a61 6e67 6f2e 7574 696c 732e  ...django.utils.
-00000630: 7472 616e 736c 6174 696f 6e72 0600 0000  translationr....
-00000640: 721c 0000 0072 0800 0000 da05 4d6f 6465  r....r......Mode
-00000650: 6c72 0700 0000 7216 0000 0072 1600 0000  lr....r....r....
-00000660: 7216 0000 0072 1700 0000 da08 3c6d 6f64  r....r......<mod
-00000670: 756c 653e 0100 0000 730c 0000 000c 010c  ule>....s.......
-00000680: 010c 010c 010c 0206 03                   .........
+00000050: 0100 6400 6404 6c06 6d07 5a08 0100 6400  ..d.d.l.m.Z...d.
+00000060: 6405 6c09 6d0a 5a0a 0100 4700 6406 6407  d.l.m.Z...G.d.d.
+00000070: 8400 6407 6501 6a0b 8303 5a0c 6408 5300  ..d.e.j...Z.d.S.
+00000080: 2909 e900 0000 0029 01da 066d 6f64 656c  )......)...model
+00000090: 7329 01da 1147 656e 6572 6963 466f 7265  s)...GenericFore
+000000a0: 6967 6e4b 6579 2901 da0b 436f 6e74 656e  ignKey)...Conten
+000000b0: 7454 7970 6529 01da 0c67 6574 7465 7874  tType)...gettext
+000000c0: 5f6c 617a 7929 01da 0b55 7365 7253 6573  _lazy)...UserSes
+000000d0: 7369 6f6e 6300 0000 0000 0000 0000 0000  sionc...........
+000000e0: 0000 0000 0007 0000 0040 0000 0073 8400  .........@...s..
+000000f0: 0000 6500 5a01 6400 5a02 6401 5a03 6504  ..e.Z.d.Z.d.Z.e.
+00000100: 6a05 6506 6504 6a07 6508 6402 8301 6403  j.e.e.j.e.d...d.
+00000110: 6404 6405 8d05 5a09 6504 6a0a 6508 6406  d.d...Z.e.j.e.d.
+00000120: 8301 6407 8d01 5a0b 6504 6a05 650c 6504  ..d...Z.e.j.e.e.
+00000130: 6a07 6508 6408 8301 6404 6409 8d04 5a0d  j.e.d...d.d...Z.
+00000140: 650e 640a 640b 8302 5a0f 6504 6a10 640c  e.d.d...Z.e.j.d.
+00000150: 6508 640d 8301 640e 8d02 5a11 640f 6410  e.d...d...Z.d.d.
+00000160: 8400 5a12 4700 6411 6412 8400 6412 8302  ..Z.G.d.d...d...
+00000170: 5a13 6413 5300 2914 da08 4661 766f 7269  Z.d.S.)...Favori
+00000180: 7465 7550 0000 000a 2020 2020 2020 2020  teuP....        
+00000190: d09c d0be d0b4 d0b5 d0bb d18c 2022 d098  ............ "..
+000001a0: d0b7 d0b1 d180 d0b0 d0bd d0bd d0be d0b5  ................
+000001b0: 2220 d0b4 d0bb d18f 20d0 bfd0 bed0 bbd1  " ...... .......
+000001c0: 8cd0 b7d0 bed0 b2d0 b0d1 82d0 b5d0 bbd1  ................
+000001d0: 8f2e 0a20 2020 20da 0455 7365 725a 0966  ...    ..UserZ.f
+000001e0: 6176 6f72 6974 6573 4629 04da 096f 6e5f  avoritesF)...on_
+000001f0: 6465 6c65 7465 da0c 7665 7262 6f73 655f  delete..verbose_
+00000200: 6e61 6d65 da0c 7265 6c61 7465 645f 6e61  name..related_na
+00000210: 6d65 da08 6564 6974 6162 6c65 7a09 4f62  me..editablez.Ob
+00000220: 6a65 6374 2049 4429 0172 0a00 0000 7a0c  ject ID).r....z.
+00000230: 436f 6e74 656e 7420 7479 7065 2903 7209  Content type).r.
+00000240: 0000 0072 0a00 0000 720c 0000 00da 0c63  ...r....r......c
+00000250: 6f6e 7465 6e74 5f74 7970 65da 096f 626a  ontent_type..obj
+00000260: 6563 745f 6964 547a 0a43 7265 6174 6564  ect_idTz.Created
+00000270: 2061 7429 02da 0c61 7574 6f5f 6e6f 775f   at)...auto_now_
+00000280: 6164 6472 0a00 0000 6301 0000 0000 0000  addr....c.......
+00000290: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
+000002a0: 0073 1a00 0000 6401 7c00 6a00 6a01 7c00  .s....d.|.j.j.|.
+000002b0: 6a02 7c00 6a03 6a04 6a05 6603 1600 5300  j.|.j.j.j.f...S.
+000002c0: 2902 4e7a 1955 7365 7220 2569 207c 2046  ).Nz.User %i | F
+000002d0: 6176 6f72 6974 653a 2025 7320 2573 2906  avorite: %s %s).
+000002e0: da0c 7573 6572 5f73 6573 7369 6f6e da02  ..user_session..
+000002f0: 6964 720e 0000 00da 0e63 6f6e 7465 6e74  idr......content
+00000300: 5f6f 626a 6563 74da 095f 5f63 6c61 7373  _object..__class
+00000310: 5f5f da08 5f5f 6e61 6d65 5f5f 2901 da04  __..__name__)...
+00000320: 7365 6c66 a900 7216 0000 00fa 522f 5573  self..r.....R/Us
+00000330: 6572 732f 7669 6b74 6f72 6961 7265 7365  ers/viktoriarese
+00000340: 746f 7661 2f47 4152 5049 582f 6761 7270  tova/GARPIX/garp
+00000350: 6978 5f66 6176 6f75 7269 7465 2f62 6163  ix_favourite/bac
+00000360: 6b65 6e64 2f67 6172 7069 785f 6661 766f  kend/garpix_favo
+00000370: 7572 6974 652f 6d6f 6465 6c73 2e70 79da  urite/models.py.
+00000380: 075f 5f73 7472 5f5f 1f00 0000 730a 0000  .__str__....s...
+00000390: 0000 0102 0106 0004 0008 ff7a 1046 6176  ...........z.Fav
+000003a0: 6f72 6974 652e 5f5f 7374 725f 5f63 0000  orite.__str__c..
+000003b0: 0000 0000 0000 0000 0000 0000 0000 0200  ................
+000003c0: 0000 4000 0000 7324 0000 0065 005a 0164  ..@...s$...e.Z.d
+000003d0: 005a 0264 015a 0365 0464 0283 015a 0565  .Z.d.Z.e.d...Z.e
+000003e0: 0464 0383 015a 0664 045a 0764 0553 0029  .d...Z.d.Z.d.S.)
+000003f0: 067a 0d46 6176 6f72 6974 652e 4d65 7461  .z.Favorite.Meta
+00000400: 2901 7211 0000 0072 0700 0000 5a09 4661  ).r....r....Z.Fa
+00000410: 766f 7269 7465 7329 0129 0372 1000 0000  vorites).).r....
+00000420: 720d 0000 0072 0e00 0000 4e29 0872 1400  r....r....N).r..
+00000430: 0000 da0a 5f5f 6d6f 6475 6c65 5f5f da0c  ....__module__..
+00000440: 5f5f 7175 616c 6e61 6d65 5f5f da08 6f72  __qualname__..or
+00000450: 6465 7269 6e67 da01 5f72 0a00 0000 da13  dering.._r......
+00000460: 7665 7262 6f73 655f 6e61 6d65 5f70 6c75  verbose_name_plu
+00000470: 7261 6cda 0f75 6e69 7175 655f 746f 6765  ral..unique_toge
+00000480: 7468 6572 7216 0000 0072 1600 0000 7216  therr....r....r.
+00000490: 0000 0072 1700 0000 da04 4d65 7461 2400  ...r......Meta$.
+000004a0: 0000 7308 0000 0008 0104 0108 0108 0172  ..s............r
+000004b0: 1f00 0000 4e29 1472 1400 0000 7219 0000  ....N).r....r...
+000004c0: 0072 1a00 0000 da07 5f5f 646f 635f 5f72  .r......__doc__r
+000004d0: 0200 0000 da0a 466f 7265 6967 6e4b 6579  ......ForeignKey
+000004e0: 7206 0000 00da 0743 4153 4341 4445 721c  r......CASCADEr.
+000004f0: 0000 0072 1000 0000 da14 506f 7369 7469  ...r......Positi
+00000500: 7665 496e 7465 6765 7246 6965 6c64 720e  veIntegerFieldr.
+00000510: 0000 0072 0400 0000 720d 0000 0072 0300  ...r....r....r..
+00000520: 0000 7212 0000 00da 0d44 6174 6554 696d  ..r......DateTim
+00000530: 6546 6965 6c64 da0a 6372 6561 7465 645f  eField..created_
+00000540: 6174 7218 0000 0072 1f00 0000 7216 0000  atr....r....r...
+00000550: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
+00000560: 7207 0000 0008 0000 0073 3600 0000 0801  r........s6.....
+00000570: 0404 0401 0200 0400 0601 0200 02fe 0604  ................
+00000580: 0401 06ff 0603 0401 0200 0400 0601 02fe  ................
+00000590: 0604 0201 0200 02ff 0403 0401 0200 06ff  ................
+000005a0: 0604 0805 7207 0000 004e 290d da09 646a  ....r....N)...dj
+000005b0: 616e 676f 2e64 6272 0200 0000 5a22 646a  ango.dbr....Z"dj
+000005c0: 616e 676f 2e63 6f6e 7472 6962 2e63 6f6e  ango.contrib.con
+000005d0: 7465 6e74 7479 7065 732e 6669 656c 6473  tenttypes.fields
+000005e0: 7203 0000 00da 2264 6a61 6e67 6f2e 636f  r....."django.co
+000005f0: 6e74 7269 622e 636f 6e74 656e 7474 7970  ntrib.contenttyp
+00000600: 6573 2e6d 6f64 656c 7372 0400 0000 da18  es.modelsr......
+00000610: 646a 616e 676f 2e75 7469 6c73 2e74 7261  django.utils.tra
+00000620: 6e73 6c61 7469 6f6e 7205 0000 0072 1c00  nslationr....r..
+00000630: 0000 da12 6761 7270 6978 5f75 7365 722e  ....garpix_user.
+00000640: 6d6f 6465 6c73 7206 0000 00da 054d 6f64  modelsr......Mod
+00000650: 656c 7207 0000 0072 1600 0000 7216 0000  elr....r....r...
+00000660: 0072 1600 0000 7217 0000 00da 083c 6d6f  .r....r......<mo
+00000670: 6475 6c65 3e01 0000 0073 0a00 0000 0c01  dule>....s......
+00000680: 0c01 0c01 0c01 0c03                      ........
```

### Comparing `garpix_favourite-1.0.0/garpix_favourite/__pycache__/serializers.cpython-38.pyc` & `garpix_favourite-2.0.0/garpix_favourite/__pycache__/serializers.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Aug 20 16:16:50 2021 UTC, .py size: 3333 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,218 +1,223 @@
-00000000: 550d 0d0a 0000 0000 72d5 1f61 050d 0000  U.......r..a....
+00000000: 550d 0d0a 0000 0000 15c2 5b64 4d0d 0000  U.........[dM...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0008 0000 0040 0000 0073 ba00 0000 6400  .....@...s....d.
+00000020: 0008 0000 0040 0000 0073 c600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a0a 0100 6400 6406 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6400 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
-00000080: 0100 6408 6409 6c0f 6d10 5a10 0100 7a0a  ..d.d.l.m.Z...z.
-00000090: 6505 6a11 5a11 5700 6e20 0400 6512 6b0a  e.j.Z.W.n ..e.k.
-000000a0: 728a 0100 0100 0100 6512 650a 640a 8301  r.......e.e.d...
-000000b0: 8301 8201 5900 6e02 5800 6501 6513 8301  ....Y.n.X.e.e...
-000000c0: 5a14 6515 6507 640b 9c02 640c 640d 8404  Z.e.e.d...d.d...
-000000d0: 5a16 4700 640e 640f 8400 640f 650c 6a17  Z.G.d.d...d.e.j.
-000000e0: 8303 5a18 6410 5300 2911 e900 0000 0029  ..Z.d.S.)......)
-000000f0: 01da 0967 6574 4c6f 6767 6572 2901 da08  ...getLogger)...
-00000100: 4f70 7469 6f6e 616c 2901 da08 7365 7474  Optional)...sett
-00000110: 696e 6773 2901 da0b 436f 6e74 656e 7454  ings)...ContentT
-00000120: 7970 6529 01da 0c67 6574 7465 7874 5f6c  ype)...gettext_l
-00000130: 617a 7929 01da 0b73 6572 6961 6c69 7a65  azy)...serialize
-00000140: 7273 2901 da0f 5661 6c69 6461 7469 6f6e  rs)...Validation
-00000150: 4572 726f 72e9 0100 0000 2901 da08 4661  Error.....)...Fa
-00000160: 766f 7269 7465 7545 0000 0041 4343 4550  voriteuE...ACCEP
-00000170: 5445 445f 4641 564f 5249 5445 5f4d 4f44  TED_FAVORITE_MOD
-00000180: 454c 5320 d0bd d0b5 20d0 bdd0 b0d0 b9d0  ELS .... .......
-00000190: b4d0 b5d0 bdd0 be20 d0b2 20d0 bdd0 b0d1  ....... .. .....
-000001a0: 81d1 82d1 80d0 bed0 b9d0 bad0 b0d1 852e  ................
-000001b0: 2902 da0a 6d6f 6465 6c5f 6e61 6d65 da06  )...model_name..
-000001c0: 7265 7475 726e 6301 0000 0000 0000 0000  returnc.........
-000001d0: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
-000001e0: 1600 0000 7c00 a000 a100 7d00 7401 6a02  ....|.....}.t.j.
-000001f0: 6a03 7c00 6401 8d01 5300 2902 4e29 01da  j.|.d...S.).N)..
-00000200: 056d 6f64 656c 2904 da05 6c6f 7765 7272  .model)...lowerr
-00000210: 0500 0000 da07 6f62 6a65 6374 73da 0367  ......objects..g
-00000220: 6574 2901 720b 0000 00a9 0072 1100 0000  et).r......r....
-00000230: fa4f 2f55 7365 7273 2f63 7275 7361 742f  .O/Users/crusat/
-00000240: 7072 6f6a 6563 7473 2f67 6172 7069 785f  projects/garpix_
-00000250: 6661 766f 7572 6974 652f 6261 636b 656e  favourite/backen
-00000260: 642f 6761 7270 6978 5f66 6176 6f75 7269  d/garpix_favouri
-00000270: 7465 2f73 6572 6961 6c69 7a65 7273 2e70  te/serializers.p
-00000280: 79da 1f5f 6765 745f 636f 6e74 656e 745f  y.._get_content_
-00000290: 7479 7065 5f62 795f 6d6f 6465 6c5f 6e61  type_by_model_na
-000002a0: 6d65 1800 0000 7304 0000 0000 0108 0272  me....s........r
-000002b0: 1300 0000 6300 0000 0000 0000 0000 0000  ....c...........
-000002c0: 0000 0000 0005 0000 0000 0000 0073 7400  .............st.
-000002d0: 0000 6500 5a01 6400 5a02 6401 5a03 6504  ..e.Z.d.Z.d.Z.e.
-000002e0: 6a05 6402 6402 6403 6404 8d03 5a06 6504  j.d.d.d.d...Z.e.
-000002f0: 6a07 6402 6405 8d01 5a08 6406 6407 8400  j.d.d...Z.d.d...
-00000300: 5a09 650a 650b 1900 6408 9c01 6409 640a  Z.e.e...d...d.d.
-00000310: 8404 5a0c 640b 640c 8400 5a0d 640d 640e  ..Z.d.d...Z.d.d.
-00000320: 8400 5a0e 8700 6601 640f 6410 8408 5a0f  ..Z...f.d.d...Z.
-00000330: 4700 6411 6412 8400 6412 8302 5a10 8700  G.d.d...d...Z...
-00000340: 0400 5a11 5300 2913 da12 4661 766f 7269  ..Z.S.)...Favori
-00000350: 7465 5365 7269 616c 697a 6572 7543 0000  teSerializeruC..
-00000360: 000a 2020 2020 2020 2020 d0a1 d0b5 d180  ..        ......
-00000370: d0b8 d0b0 d0bb d0b8 d0b7 d0b0 d182 d0be  ................
-00000380: d180 20d0 b4d0 bbd1 8f20 d0b8 d0b7 d0b1  .. ...... ......
-00000390: d180 d0b0 d0bd d0bd d0be d0b3 d0be 2e0a  ................
-000003a0: 2020 2020 54e9 6400 0000 2903 da08 7265      T.d...)...re
-000003b0: 7175 6972 6564 da0a 7772 6974 655f 6f6e  quired..write_on
-000003c0: 6c79 da0a 6d61 785f 6c65 6e67 7468 2901  ly..max_length).
-000003d0: da09 7265 6164 5f6f 6e6c 7963 0100 0000  ..read_onlyc....
-000003e0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-000003f0: 4300 0000 730c 0000 007c 006a 00a0 0164  C...s....|.j...d
-00000400: 01a1 0153 0029 024e da07 7265 7175 6573  ...S.).N..reques
-00000410: 7429 02da 0763 6f6e 7465 7874 7210 0000  t)...contextr...
-00000420: 0029 01da 0473 656c 6672 1100 0000 7211  .)...selfr....r.
-00000430: 0000 0072 1200 0000 da0c 5f67 6574 5f72  ...r......_get_r
-00000440: 6571 7565 7374 2900 0000 7302 0000 0000  equest)...s.....
-00000450: 017a 1f46 6176 6f72 6974 6553 6572 6961  .z.FavoriteSeria
-00000460: 6c69 7a65 722e 5f67 6574 5f72 6571 7565  lizer._get_reque
-00000470: 7374 2901 720c 0000 0063 0200 0000 0000  st).r....c......
-00000480: 0000 0000 0000 0200 0000 0800 0000 4300  ..............C.
-00000490: 0000 734a 0000 007a 167c 00a0 00a1 00a0  ..sJ...z.|......
-000004a0: 017c 016a 02a0 03a1 00a1 0157 0053 0004  .|.j.......W.S..
-000004b0: 0074 046b 0a72 4401 0001 0001 0074 05a0  .t.k.rD......t..
-000004c0: 0674 0764 017c 016a 026a 086a 0916 0083  .t.d.|.j.j.j....
-000004d0: 01a1 0101 0059 0064 0253 0058 0064 0253  .....Y.d.S.X.d.S
-000004e0: 0029 0375 6400 0000 0a20 2020 2020 2020  .).ud....       
-000004f0: 2020 2020 20d0 92d0 bed0 b7d0 b2d1 80d0       ...........
-00000500: b0d1 89d0 b0d0 b5d1 8220 d0bf d0be d0bb  ......... ......
-00000510: d0bd d18b d0b9 20d0 bfd1 83d1 82d1 8c20  ...... ........ 
-00000520: d0b4 d0be 20d0 bed0 b1d1 8ad0 b5d0 bad1  .... ...........
-00000530: 82d0 b020 636f 6e74 656e 745f 6f62 6a65  ... content_obje
-00000540: 6374 2e0a 2020 2020 2020 2020 75b4 0000  ct..        u...
-00000550: 00d0 9cd0 bed0 b4d0 b5d0 bbd1 8c20 2225  ............. "%
-00000560: 7322 20d0 bdd0 b520 d0b8 d0bc d0b5 d0b5  s" .... ........
-00000570: d182 2067 6574 5f61 6273 6f6c 7574 655f  .. get_absolute_
-00000580: 7572 6c28 292e 0a66 6176 6f72 6974 655f  url()..favorite_
-00000590: 7572 6c20 d0b1 d183 d0b4 d0b5 d182 20d0  url .......... .
-000005a0: bed0 b1d0 bed0 b7d0 bdd0 b0d1 87d0 b5d0  ................
-000005b0: bd2c 20d0 bad0 b0d0 ba20 4e6f 6e65 2e0a  ., ...... None..
-000005c0: 4661 766f 7269 7465 4d69 7869 6e20 d0be  FavoriteMixin ..
-000005d0: d0b1 d18f d0b7 d0b0 d182 d0b5 d0bb d0b5  ................
-000005e0: d0bd 20d0 b4d0 bbd1 8f20 d0b8 d181 d0bf  .. ...... ......
-000005f0: d0be d0bb d18c d0b7 d0be d0b2 d0b0 d0bd  ................
-00000600: d0b8 d18f 2e4e 290a 721d 0000 00da 1262  .....N).r......b
-00000610: 7569 6c64 5f61 6273 6f6c 7574 655f 7572  uild_absolute_ur
-00000620: 69da 0e63 6f6e 7465 6e74 5f6f 626a 6563  i..content_objec
-00000630: 74da 1067 6574 5f61 6273 6f6c 7574 655f  t..get_absolute_
-00000640: 7572 6cda 0e41 7474 7269 6275 7465 4572  url..AttributeEr
-00000650: 726f 72da 066c 6f67 6765 72da 0565 7272  ror..logger..err
-00000660: 6f72 da01 5fda 095f 5f63 6c61 7373 5f5f  or.._..__class__
-00000670: da08 5f5f 6e61 6d65 5f5f 2902 721c 0000  ..__name__).r...
-00000680: 00da 0869 6e73 7461 6e63 6572 1100 0000  ...instancer....
-00000690: 7211 0000 0072 1200 0000 da10 6765 745f  r....r......get_
-000006a0: 6661 766f 7269 7465 5f75 726c 2c00 0000  favorite_url,...
-000006b0: 731a 0000 0000 0502 0108 0108 ff06 030e  s...............
-000006c0: 0104 0102 0102 0308 fd02 ff02 ff04 087a  ...............z
-000006d0: 2346 6176 6f72 6974 6553 6572 6961 6c69  #FavoriteSeriali
-000006e0: 7a65 722e 6765 745f 6661 766f 7269 7465  zer.get_favorite
-000006f0: 5f75 726c 6302 0000 0000 0000 0000 0000  _urlc...........
-00000700: 0008 0000 0006 0000 0043 0000 0073 8a00  .........C...s..
-00000710: 0000 7c00 a000 a100 6a01 7d02 7c01 6401  ..|.....j.}.|.d.
-00000720: 1900 7d03 7c01 6402 1900 7d04 7402 7c03  ..}.|.d...}.t.|.
-00000730: 8301 7d05 7c00 6a03 6a04 7d06 7c05 a005  ..}.|.j.j.}.|...
-00000740: a100 0400 7d07 7260 7c07 6a06 6a07 7c04  ....}.r`|.j.j.|.
-00000750: 6403 8d01 a008 a100 7360 7409 6404 740a  d.......s`t.d.t.
-00000760: 6405 7c03 7c04 6602 1600 8301 6901 8301  d.|.|.f.....i...
-00000770: 8201 7c06 6a06 6a07 7c02 7c05 7c04 6406  ..|.j.j.|.|.|.d.
-00000780: 8d03 a008 a100 7286 7409 6404 740a 6407  ......r.t.d.t.d.
-00000790: 8301 6901 8301 8201 7c01 5300 2908 4e72  ..i.....|.S.).Nr
-000007a0: 0b00 0000 da09 6f62 6a65 6374 5f69 6429  ......object_id)
-000007b0: 01da 0269 6472 2300 0000 7a1e 2573 2077  ...idr#...z.%s w
-000007c0: 6974 6820 6964 2025 6920 646f 6573 206e  ith id %i does n
-000007d0: 6f74 2065 7869 7374 732e 2903 da04 7573  ot exists.)...us
-000007e0: 6572 da0c 636f 6e74 656e 745f 7479 7065  er..content_type
-000007f0: 7229 0000 007a 2f54 6865 206f 626a 6563  r)...z/The objec
-00000800: 7420 6861 7320 616c 7265 6164 7920 6265  t has already be
-00000810: 656e 2061 6464 6564 2074 6f20 6661 766f  en added to favo
-00000820: 7269 7465 732e 290b 721d 0000 0072 2b00  rites.).r....r+.
-00000830: 0000 7213 0000 00da 044d 6574 6172 0d00  ..r......Metar..
-00000840: 0000 da0b 6d6f 6465 6c5f 636c 6173 7372  ....model_classr
-00000850: 0f00 0000 da06 6669 6c74 6572 da06 6578  ......filter..ex
-00000860: 6973 7473 7208 0000 0072 2400 0000 2908  istsr....r$...).
-00000870: 721c 0000 00da 0561 7474 7273 722b 0000  r......attrsr+..
-00000880: 0072 0b00 0000 7229 0000 0072 2c00 0000  .r....r)...r,...
-00000890: 720d 0000 0072 2e00 0000 7211 0000 0072  r....r....r....r
-000008a0: 1100 0000 7212 0000 00da 0876 616c 6964  ....r......valid
-000008b0: 6174 6540 0000 0073 2600 0000 0001 0a01  ate@...s&.......
-000008c0: 0801 0801 0801 0802 0c01 1201 0201 12ff  ................
-000008d0: 0404 0601 0201 0201 02fd 0a05 0201 0aff  ................
-000008e0: 0404 7a1b 4661 766f 7269 7465 5365 7269  ..z.FavoriteSeri
-000008f0: 616c 697a 6572 2e76 616c 6964 6174 6563  alizer.validatec
-00000900: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000910: 0600 0000 4300 0000 7322 0000 007c 0174  ....C...s"...|.t
-00000920: 006b 0772 1e74 0174 0264 0164 02a0 0374  .k.r.t.t.d.d...t
-00000930: 00a1 0116 0083 0183 0182 017c 0153 0029  ...........|.S.)
-00000940: 034e 7a14 4d6f 6465 6c20 6d75 7374 2062  .Nz.Model must b
-00000950: 6520 696e 3a20 2573 7a02 2c20 2904 da18  e in: %sz., )...
-00000960: 4143 4345 5054 4544 5f46 4156 4f52 4954  ACCEPTED_FAVORIT
-00000970: 455f 4d4f 4445 4c53 7208 0000 0072 2400  E_MODELSr....r$.
-00000980: 0000 da04 6a6f 696e 2902 721c 0000 00da  ....join).r.....
-00000990: 0576 616c 7565 7211 0000 0072 1100 0000  .valuer....r....
-000009a0: 7212 0000 00da 1376 616c 6964 6174 655f  r......validate_
-000009b0: 6d6f 6465 6c5f 6e61 6d65 5800 0000 730a  model_nameX...s.
-000009c0: 0000 0000 0108 0102 0110 ff04 037a 2646  .............z&F
-000009d0: 6176 6f72 6974 6553 6572 6961 6c69 7a65  avoriteSerialize
-000009e0: 722e 7661 6c69 6461 7465 5f6d 6f64 656c  r.validate_model
-000009f0: 5f6e 616d 6563 0200 0000 0000 0000 0000  _namec..........
-00000a00: 0000 0400 0000 0400 0000 0300 0000 732c  ..............s,
-00000a10: 0000 007c 01a0 0064 01a1 017d 0274 017c  ...|...d...}.t.|
-00000a20: 0283 017d 037c 01a0 0264 027c 0369 01a1  ...}.|...d.|.i..
-00000a30: 0101 0074 0383 00a0 047c 01a1 0153 0029  ...t.....|...S.)
-00000a40: 034e 720b 0000 0072 2c00 0000 2905 da03  .Nr....r,...)...
-00000a50: 706f 7072 1300 0000 da06 7570 6461 7465  popr......update
-00000a60: da05 7375 7065 72da 0663 7265 6174 6529  ..super..create)
-00000a70: 0472 1c00 0000 da0e 7661 6c69 6461 7465  .r......validate
-00000a80: 645f 6461 7461 720b 0000 0072 2c00 0000  d_datar....r,...
-00000a90: a901 7225 0000 0072 1100 0000 7212 0000  ..r%...r....r...
-00000aa0: 0072 3a00 0000 5f00 0000 730e 0000 0000  .r:..._...s.....
-00000ab0: 010a 0108 0204 0102 0002 ff06 047a 1946  .............z.F
-00000ac0: 6176 6f72 6974 6553 6572 6961 6c69 7a65  avoriteSerialize
-00000ad0: 722e 6372 6561 7465 6300 0000 0000 0000  r.createc.......
-00000ae0: 0000 0000 0000 0000 0001 0000 0040 0000  .............@..
-00000af0: 0073 1400 0000 6500 5a01 6400 5a02 6503  .s....e.Z.d.Z.e.
-00000b00: 5a04 6401 5a05 6402 5300 2903 7a17 4661  Z.d.Z.d.S.).z.Fa
-00000b10: 766f 7269 7465 5365 7269 616c 697a 6572  voriteSerializer
-00000b20: 2e4d 6574 6129 0172 2b00 0000 4e29 0672  .Meta).r+...N).r
-00000b30: 2600 0000 da0a 5f5f 6d6f 6475 6c65 5f5f  &.....__module__
-00000b40: da0c 5f5f 7175 616c 6e61 6d65 5f5f 720a  ..__qualname__r.
-00000b50: 0000 0072 0d00 0000 da07 6578 636c 7564  ...r......exclud
-00000b60: 6572 1100 0000 7211 0000 0072 1100 0000  er....r....r....
-00000b70: 7212 0000 0072 2d00 0000 6900 0000 7304  r....r-...i...s.
-00000b80: 0000 0008 0104 0172 2d00 0000 2912 7226  .......r-...).r&
-00000b90: 0000 0072 3d00 0000 723e 0000 00da 075f  ...r=...r>....._
-00000ba0: 5f64 6f63 5f5f 7207 0000 00da 0943 6861  _doc__r......Cha
-00000bb0: 7246 6965 6c64 720b 0000 00da 1553 6572  rFieldr......Ser
-00000bc0: 6961 6c69 7a65 724d 6574 686f 6446 6965  ializerMethodFie
-00000bd0: 6c64 5a0c 6661 766f 7269 7465 5f75 726c  ldZ.favorite_url
-00000be0: 721d 0000 0072 0300 0000 da03 7374 7272  r....r......strr
-00000bf0: 2800 0000 7232 0000 0072 3600 0000 723a  (...r2...r6...r:
-00000c00: 0000 0072 2d00 0000 da0d 5f5f 636c 6173  ...r-.....__clas
-00000c10: 7363 656c 6c5f 5f72 1100 0000 7211 0000  scell__r....r...
-00000c20: 0072 3c00 0000 7212 0000 0072 1400 0000  .r<...r....r....
-00000c30: 1e00 0000 731e 0000 0008 0104 0304 0102  ....s...........
-00000c40: 0002 0002 ff06 0304 0102 ff06 0408 0312  ................
-00000c50: 1408 1808 070c 0a72 1400 0000 4e29 19da  .......r....N)..
-00000c60: 076c 6f67 6769 6e67 7202 0000 00da 0674  .loggingr......t
-00000c70: 7970 696e 6772 0300 0000 da0b 646a 616e  ypingr......djan
-00000c80: 676f 2e63 6f6e 6672 0400 0000 da22 646a  go.confr....."dj
-00000c90: 616e 676f 2e63 6f6e 7472 6962 2e63 6f6e  ango.contrib.con
-00000ca0: 7465 6e74 7479 7065 732e 6d6f 6465 6c73  tenttypes.models
-00000cb0: 7205 0000 00da 1864 6a61 6e67 6f2e 7574  r......django.ut
-00000cc0: 696c 732e 7472 616e 736c 6174 696f 6e72  ils.translationr
-00000cd0: 0600 0000 7224 0000 00da 0e72 6573 745f  ....r$.....rest_
-00000ce0: 6672 616d 6577 6f72 6b72 0700 0000 da19  frameworkr......
-00000cf0: 7265 7374 5f66 7261 6d65 776f 726b 2e65  rest_framework.e
-00000d00: 7863 6570 7469 6f6e 7372 0800 0000 da06  xceptionsr......
-00000d10: 6d6f 6465 6c73 720a 0000 0072 3300 0000  modelsr....r3...
-00000d20: 7221 0000 0072 2600 0000 7222 0000 0072  r!...r&...r"...r
-00000d30: 4300 0000 7213 0000 00da 0f4d 6f64 656c  C...r......Model
-00000d40: 5365 7269 616c 697a 6572 7214 0000 0072  Serializerr....r
-00000d50: 1100 0000 7211 0000 0072 1100 0000 7212  ....r....r....r.
-00000d60: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000d70: 0073 2000 0000 0c02 0c02 0c01 0c01 0c02  .s .............
-00000d80: 0c01 0c02 0c02 0201 0a01 0e01 0201 06ff  ................
-00000d90: 0a04 0803 1006                           ......
+00000080: 0100 6400 6408 6c0f 6d10 5a10 0100 6409  ..d.d.l.m.Z...d.
+00000090: 640a 6c11 6d12 5a12 0100 7a0a 6505 6a13  d.l.m.Z...z.e.j.
+000000a0: 5a13 5700 6e20 0400 6514 6b0a 7296 0100  Z.W.n ..e.k.r...
+000000b0: 0100 0100 6514 650a 640b 8301 8301 8201  ....e.e.d.......
+000000c0: 5900 6e02 5800 6501 6515 8301 5a16 6517  Y.n.X.e.e...Z.e.
+000000d0: 6507 640c 9c02 640d 640e 8404 5a18 4700  e.d...d.d...Z.G.
+000000e0: 640f 6410 8400 6410 650e 6a19 8303 5a1a  d.d...d.e.j...Z.
+000000f0: 6411 5300 2912 e900 0000 0029 01da 0967  d.S.)......)...g
+00000100: 6574 4c6f 6767 6572 2901 da08 4f70 7469  etLogger)...Opti
+00000110: 6f6e 616c 2901 da08 7365 7474 696e 6773  onal)...settings
+00000120: 2901 da0b 436f 6e74 656e 7454 7970 6529  )...ContentType)
+00000130: 01da 0c67 6574 7465 7874 5f6c 617a 7929  ...gettext_lazy)
+00000140: 01da 0b55 7365 7253 6573 7369 6f6e 2901  ...UserSession).
+00000150: da0b 7365 7269 616c 697a 6572 7329 01da  ..serializers)..
+00000160: 0f56 616c 6964 6174 696f 6e45 7272 6f72  .ValidationError
+00000170: e901 0000 0029 01da 0846 6176 6f72 6974  .....)...Favorit
+00000180: 657a 2f41 4343 4550 5445 445f 4641 564f  ez/ACCEPTED_FAVO
+00000190: 5249 5445 5f4d 4f44 454c 5320 6e6f 7420  RITE_MODELS not 
+000001a0: 666f 756e 6420 696e 2073 6574 7469 6e67  found in setting
+000001b0: 732e 2902 da0a 6d6f 6465 6c5f 6e61 6d65  s.)...model_name
+000001c0: da06 7265 7475 726e 6301 0000 0000 0000  ..returnc.......
+000001d0: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
+000001e0: 0073 1600 0000 7c00 a000 a100 7d00 7401  .s....|.....}.t.
+000001f0: 6a02 6a03 7c00 6401 8d01 5300 2902 4e29  j.j.|.d...S.).N)
+00000200: 01da 056d 6f64 656c 2904 da05 6c6f 7765  ...model)...lowe
+00000210: 7272 0500 0000 da07 6f62 6a65 6374 73da  rr......objects.
+00000220: 0367 6574 2901 720c 0000 00a9 0072 1200  .get).r......r..
+00000230: 0000 fa57 2f55 7365 7273 2f76 696b 746f  ...W/Users/vikto
+00000240: 7269 6172 6573 6574 6f76 612f 4741 5250  riaresetova/GARP
+00000250: 4958 2f67 6172 7069 785f 6661 766f 7572  IX/garpix_favour
+00000260: 6974 652f 6261 636b 656e 642f 6761 7270  ite/backend/garp
+00000270: 6978 5f66 6176 6f75 7269 7465 2f73 6572  ix_favourite/ser
+00000280: 6961 6c69 7a65 7273 2e70 79da 1f5f 6765  ializers.py.._ge
+00000290: 745f 636f 6e74 656e 745f 7479 7065 5f62  t_content_type_b
+000002a0: 795f 6d6f 6465 6c5f 6e61 6d65 1900 0000  y_model_name....
+000002b0: 7304 0000 0000 0108 0272 1400 0000 6300  s........r....c.
+000002c0: 0000 0000 0000 0000 0000 0000 0000 0005  ................
+000002d0: 0000 0000 0000 0073 7400 0000 6500 5a01  .......st...e.Z.
+000002e0: 6400 5a02 6401 5a03 6504 6a05 6402 6402  d.Z.d.Z.e.j.d.d.
+000002f0: 6403 6404 8d03 5a06 6504 6a07 6402 6405  d.d...Z.e.j.d.d.
+00000300: 8d01 5a08 6406 6407 8400 5a09 650a 650b  ..Z.d.d...Z.e.e.
+00000310: 1900 6408 9c01 6409 640a 8404 5a0c 640b  ..d...d.d...Z.d.
+00000320: 640c 8400 5a0d 640d 640e 8400 5a0e 8700  d...Z.d.d...Z...
+00000330: 6601 640f 6410 8408 5a0f 4700 6411 6412  f.d.d...Z.G.d.d.
+00000340: 8400 6412 8302 5a10 8700 0400 5a11 5300  ..d...Z.....Z.S.
+00000350: 2913 da12 4661 766f 7269 7465 5365 7269  )...FavoriteSeri
+00000360: 616c 697a 6572 7543 0000 000a 2020 2020  alizeruC....    
+00000370: 2020 2020 d0a1 d0b5 d180 d0b8 d0b0 d0bb      ............
+00000380: d0b8 d0b7 d0b0 d182 d0be d180 20d0 b4d0  ............ ...
+00000390: bbd1 8f20 d0b8 d0b7 d0b1 d180 d0b0 d0bd  ... ............
+000003a0: d0bd d0be d0b3 d0be 2e0a 2020 2020 54e9  ..........    T.
+000003b0: 6400 0000 2903 da08 7265 7175 6972 6564  d...)...required
+000003c0: da0a 7772 6974 655f 6f6e 6c79 da0a 6d61  ..write_only..ma
+000003d0: 785f 6c65 6e67 7468 2901 da09 7265 6164  x_length)...read
+000003e0: 5f6f 6e6c 7963 0100 0000 0000 0000 0000  _onlyc..........
+000003f0: 0000 0100 0000 0300 0000 4300 0000 730c  ..........C...s.
+00000400: 0000 007c 006a 00a0 0164 01a1 0153 0029  ...|.j...d...S.)
+00000410: 024e da07 7265 7175 6573 7429 02da 0763  .N..request)...c
+00000420: 6f6e 7465 7874 7211 0000 0029 01da 0473  ontextr....)...s
+00000430: 656c 6672 1200 0000 7212 0000 0072 1300  elfr....r....r..
+00000440: 0000 da0c 5f67 6574 5f72 6571 7565 7374  ...._get_request
+00000450: 2a00 0000 7302 0000 0000 017a 1f46 6176  *...s......z.Fav
+00000460: 6f72 6974 6553 6572 6961 6c69 7a65 722e  oriteSerializer.
+00000470: 5f67 6574 5f72 6571 7565 7374 2901 720d  _get_request).r.
+00000480: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+00000490: 0200 0000 0800 0000 4300 0000 734a 0000  ........C...sJ..
+000004a0: 007a 167c 00a0 00a1 00a0 017c 016a 02a0  .z.|.......|.j..
+000004b0: 03a1 00a1 0157 0053 0004 0074 046b 0a72  .....W.S...t.k.r
+000004c0: 4401 0001 0001 0074 05a0 0674 0764 017c  D......t...t.d.|
+000004d0: 016a 026a 086a 0916 0083 01a1 0101 0059  .j.j.j.........Y
+000004e0: 0064 0253 0058 0064 0253 0029 0375 6400  .d.S.X.d.S.).ud.
+000004f0: 0000 0a20 2020 2020 2020 2020 2020 20d0  ...            .
+00000500: 92d0 bed0 b7d0 b2d1 80d0 b0d1 89d0 b0d0  ................
+00000510: b5d1 8220 d0bf d0be d0bb d0bd d18b d0b9  ... ............
+00000520: 20d0 bfd1 83d1 82d1 8c20 d0b4 d0be 20d0   ........ .... .
+00000530: bed0 b1d1 8ad0 b5d0 bad1 82d0 b020 636f  ............. co
+00000540: 6e74 656e 745f 6f62 6a65 6374 2e0a 2020  ntent_object..  
+00000550: 2020 2020 2020 75b4 0000 00d0 9cd0 bed0        u.........
+00000560: b4d0 b5d0 bbd1 8c20 2225 7322 20d0 bdd0  ....... "%s" ...
+00000570: b520 d0b8 d0bc d0b5 d0b5 d182 2067 6574  . .......... get
+00000580: 5f61 6273 6f6c 7574 655f 7572 6c28 292e  _absolute_url().
+00000590: 0a66 6176 6f72 6974 655f 7572 6c20 d0b1  .favorite_url ..
+000005a0: d183 d0b4 d0b5 d182 20d0 bed0 b1d0 bed0  ........ .......
+000005b0: b7d0 bdd0 b0d1 87d0 b5d0 bd2c 20d0 bad0  ..........., ...
+000005c0: b0d0 ba20 4e6f 6e65 2e0a 4661 766f 7269  ... None..Favori
+000005d0: 7465 4d69 7869 6e20 d0be d0b1 d18f d0b7  teMixin ........
+000005e0: d0b0 d182 d0b5 d0bb d0b5 d0bd 20d0 b4d0  ............ ...
+000005f0: bbd1 8f20 d0b8 d181 d0bf d0be d0bb d18c  ... ............
+00000600: d0b7 d0be d0b2 d0b0 d0bd d0b8 d18f 2e4e  ...............N
+00000610: 290a 721e 0000 00da 1262 7569 6c64 5f61  ).r......build_a
+00000620: 6273 6f6c 7574 655f 7572 69da 0e63 6f6e  bsolute_uri..con
+00000630: 7465 6e74 5f6f 626a 6563 74da 1067 6574  tent_object..get
+00000640: 5f61 6273 6f6c 7574 655f 7572 6cda 0e41  _absolute_url..A
+00000650: 7474 7269 6275 7465 4572 726f 72da 066c  ttributeError..l
+00000660: 6f67 6765 72da 0565 7272 6f72 da01 5fda  ogger..error.._.
+00000670: 095f 5f63 6c61 7373 5f5f da08 5f5f 6e61  .__class__..__na
+00000680: 6d65 5f5f 2902 721d 0000 00da 0869 6e73  me__).r......ins
+00000690: 7461 6e63 6572 1200 0000 7212 0000 0072  tancer....r....r
+000006a0: 1300 0000 da10 6765 745f 6661 766f 7269  ......get_favori
+000006b0: 7465 5f75 726c 2d00 0000 731a 0000 0000  te_url-...s.....
+000006c0: 0502 0108 0108 ff06 030e 0104 0102 0102  ................
+000006d0: 0308 fd02 ff02 ff04 087a 2346 6176 6f72  .........z#Favor
+000006e0: 6974 6553 6572 6961 6c69 7a65 722e 6765  iteSerializer.ge
+000006f0: 745f 6661 766f 7269 7465 5f75 726c 6302  t_favorite_urlc.
+00000700: 0000 0000 0000 0000 0000 0008 0000 0006  ................
+00000710: 0000 0043 0000 0073 8e00 0000 7400 a001  ...C...s....t...
+00000720: 7c00 a002 a100 a101 7d02 7c01 6401 1900  |.......}.|.d...
+00000730: 7d03 7c01 6402 1900 7d04 7403 7c03 8301  }.|.d...}.t.|...
+00000740: 7d05 7c00 6a04 6a05 7d06 7c05 a006 a100  }.|.j.j.}.|.....
+00000750: 0400 7d07 7264 7c07 6a07 6a08 7c04 6403  ..}.rd|.j.j.|.d.
+00000760: 8d01 a009 a100 7364 740a 6404 740b 6405  ......sdt.d.t.d.
+00000770: 7c03 7c04 6602 1600 8301 6901 8301 8201  |.|.f.....i.....
+00000780: 7c06 6a07 6a08 7c02 7c05 7c04 6406 8d03  |.j.j.|.|.|.d...
+00000790: a009 a100 728a 740a 6404 740b 6407 8301  ....r.t.d.t.d...
+000007a0: 6901 8301 8201 7c01 5300 2908 4e72 0c00  i.....|.S.).Nr..
+000007b0: 0000 da09 6f62 6a65 6374 5f69 6429 01da  ....object_id)..
+000007c0: 0269 6472 2400 0000 7a1e 2573 2077 6974  .idr$...z.%s wit
+000007d0: 6820 6964 2025 6920 646f 6573 206e 6f74  h id %i does not
+000007e0: 2065 7869 7374 732e 2903 da0c 7573 6572   exists.)...user
+000007f0: 5f73 6573 7369 6f6e da0c 636f 6e74 656e  _session..conten
+00000800: 745f 7479 7065 722a 0000 007a 2f54 6865  t_typer*...z/The
+00000810: 206f 626a 6563 7420 6861 7320 616c 7265   object has alre
+00000820: 6164 7920 6265 656e 2061 6464 6564 2074  ady been added t
+00000830: 6f20 6661 766f 7269 7465 732e 290c 7207  o favorites.).r.
+00000840: 0000 00da 1a67 6574 5f6f 725f 6372 6561  .....get_or_crea
+00000850: 7465 5f75 7365 725f 7365 7373 696f 6e72  te_user_sessionr
+00000860: 1e00 0000 7214 0000 00da 044d 6574 6172  ....r......Metar
+00000870: 0e00 0000 da0b 6d6f 6465 6c5f 636c 6173  ......model_clas
+00000880: 7372 1000 0000 da06 6669 6c74 6572 da06  sr......filter..
+00000890: 6578 6973 7473 7209 0000 0072 2500 0000  existsr....r%...
+000008a0: 2908 721d 0000 00da 0561 7474 7273 da04  ).r......attrs..
+000008b0: 7573 6572 720c 0000 0072 2a00 0000 722d  userr....r*...r-
+000008c0: 0000 0072 0e00 0000 7230 0000 0072 1200  ...r....r0...r..
+000008d0: 0000 7212 0000 0072 1300 0000 da08 7661  ..r....r......va
+000008e0: 6c69 6461 7465 4100 0000 7326 0000 0000  lidateA...s&....
+000008f0: 010e 0108 0108 0108 0108 020c 0112 0102  ................
+00000900: 0112 ff04 0406 0102 0102 0102 fd0a 0502  ................
+00000910: 010a ff04 047a 1b46 6176 6f72 6974 6553  .....z.FavoriteS
+00000920: 6572 6961 6c69 7a65 722e 7661 6c69 6461  erializer.valida
+00000930: 7465 6302 0000 0000 0000 0000 0000 0002  tec.............
+00000940: 0000 0006 0000 0043 0000 0073 2200 0000  .......C...s"...
+00000950: 7c01 7400 6b07 721e 7401 7402 6401 6402  |.t.k.r.t.t.d.d.
+00000960: a003 7400 a101 1600 8301 8301 8201 7c01  ..t...........|.
+00000970: 5300 2903 4e7a 144d 6f64 656c 206d 7573  S.).Nz.Model mus
+00000980: 7420 6265 2069 6e3a 2025 737a 022c 2029  t be in: %sz., )
+00000990: 04da 1841 4343 4550 5445 445f 4641 564f  ...ACCEPTED_FAVO
+000009a0: 5249 5445 5f4d 4f44 454c 5372 0900 0000  RITE_MODELSr....
+000009b0: 7225 0000 00da 046a 6f69 6e29 0272 1d00  r%.....join).r..
+000009c0: 0000 da05 7661 6c75 6572 1200 0000 7212  ....valuer....r.
+000009d0: 0000 0072 1300 0000 da13 7661 6c69 6461  ...r......valida
+000009e0: 7465 5f6d 6f64 656c 5f6e 616d 6559 0000  te_model_nameY..
+000009f0: 0073 0a00 0000 0001 0801 0201 10ff 0403  .s..............
+00000a00: 7a26 4661 766f 7269 7465 5365 7269 616c  z&FavoriteSerial
+00000a10: 697a 6572 2e76 616c 6964 6174 655f 6d6f  izer.validate_mo
+00000a20: 6465 6c5f 6e61 6d65 6302 0000 0000 0000  del_namec.......
+00000a30: 0000 0000 0004 0000 0004 0000 0003 0000  ................
+00000a40: 0073 2c00 0000 7c01 a000 6401 a101 7d02  .s,...|...d...}.
+00000a50: 7401 7c02 8301 7d03 7c01 a002 6402 7c03  t.|...}.|...d.|.
+00000a60: 6901 a101 0100 7403 8300 a004 7c01 a101  i.....t.....|...
+00000a70: 5300 2903 4e72 0c00 0000 722d 0000 0029  S.).Nr....r-...)
+00000a80: 05da 0370 6f70 7214 0000 00da 0675 7064  ...popr......upd
+00000a90: 6174 65da 0573 7570 6572 da06 6372 6561  ate..super..crea
+00000aa0: 7465 2904 721d 0000 00da 0e76 616c 6964  te).r......valid
+00000ab0: 6174 6564 5f64 6174 6172 0c00 0000 722d  ated_datar....r-
+00000ac0: 0000 00a9 0172 2600 0000 7212 0000 0072  .....r&...r....r
+00000ad0: 1300 0000 723d 0000 0060 0000 0073 0e00  ....r=...`...s..
+00000ae0: 0000 0001 0a01 0802 0401 0200 02ff 0604  ................
+00000af0: 7a19 4661 766f 7269 7465 5365 7269 616c  z.FavoriteSerial
+00000b00: 697a 6572 2e63 7265 6174 6563 0000 0000  izer.createc....
+00000b10: 0000 0000 0000 0000 0000 0000 0100 0000  ................
+00000b20: 4000 0000 7314 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
+00000b30: 0265 035a 0464 015a 0564 0253 0029 037a  .e.Z.d.Z.d.S.).z
+00000b40: 1746 6176 6f72 6974 6553 6572 6961 6c69  .FavoriteSeriali
+00000b50: 7a65 722e 4d65 7461 2901 722c 0000 004e  zer.Meta).r,...N
+00000b60: 2906 7227 0000 00da 0a5f 5f6d 6f64 756c  ).r'.....__modul
+00000b70: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+00000b80: 5f72 0b00 0000 720e 0000 00da 0765 7863  _r....r......exc
+00000b90: 6c75 6465 7212 0000 0072 1200 0000 7212  luder....r....r.
+00000ba0: 0000 0072 1300 0000 722f 0000 006a 0000  ...r....r/...j..
+00000bb0: 0073 0400 0000 0801 0401 722f 0000 0029  .s........r/...)
+00000bc0: 1272 2700 0000 7240 0000 0072 4100 0000  .r'...r@...rA...
+00000bd0: da07 5f5f 646f 635f 5f72 0800 0000 da09  ..__doc__r......
+00000be0: 4368 6172 4669 656c 6472 0c00 0000 da15  CharFieldr......
+00000bf0: 5365 7269 616c 697a 6572 4d65 7468 6f64  SerializerMethod
+00000c00: 4669 656c 645a 0c66 6176 6f72 6974 655f  FieldZ.favorite_
+00000c10: 7572 6c72 1e00 0000 7203 0000 00da 0373  urlr....r......s
+00000c20: 7472 7229 0000 0072 3500 0000 7239 0000  trr)...r5...r9..
+00000c30: 0072 3d00 0000 722f 0000 00da 0d5f 5f63  .r=...r/.....__c
+00000c40: 6c61 7373 6365 6c6c 5f5f 7212 0000 0072  lasscell__r....r
+00000c50: 1200 0000 723f 0000 0072 1300 0000 7215  ....r?...r....r.
+00000c60: 0000 001f 0000 0073 1e00 0000 0801 0403  .......s........
+00000c70: 0401 0200 0200 02ff 0603 0401 02ff 0604  ................
+00000c80: 0803 1214 0818 0807 0c0a 7215 0000 004e  ..........r....N
+00000c90: 291b da07 6c6f 6767 696e 6772 0200 0000  )...loggingr....
+00000ca0: da06 7479 7069 6e67 7203 0000 00da 0b64  ..typingr......d
+00000cb0: 6a61 6e67 6f2e 636f 6e66 7204 0000 00da  jango.confr.....
+00000cc0: 2264 6a61 6e67 6f2e 636f 6e74 7269 622e  "django.contrib.
+00000cd0: 636f 6e74 656e 7474 7970 6573 2e6d 6f64  contenttypes.mod
+00000ce0: 656c 7372 0500 0000 da18 646a 616e 676f  elsr......django
+00000cf0: 2e75 7469 6c73 2e74 7261 6e73 6c61 7469  .utils.translati
+00000d00: 6f6e 7206 0000 0072 2500 0000 da12 6761  onr....r%.....ga
+00000d10: 7270 6978 5f75 7365 722e 6d6f 6465 6c73  rpix_user.models
+00000d20: 7207 0000 00da 0e72 6573 745f 6672 616d  r......rest_fram
+00000d30: 6577 6f72 6b72 0800 0000 5a19 7265 7374  eworkr....Z.rest
+00000d40: 5f66 7261 6d65 776f 726b 2e65 7863 6570  _framework.excep
+00000d50: 7469 6f6e 7372 0900 0000 da06 6d6f 6465  tionsr......mode
+00000d60: 6c73 720b 0000 0072 3600 0000 7222 0000  lsr....r6...r"..
+00000d70: 0072 2700 0000 7223 0000 0072 4600 0000  .r'...r#...rF...
+00000d80: 7214 0000 00da 0f4d 6f64 656c 5365 7269  r......ModelSeri
+00000d90: 616c 697a 6572 7215 0000 0072 1200 0000  alizerr....r....
+00000da0: 7212 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
+00000db0: 083c 6d6f 6475 6c65 3e01 0000 0073 2200  .<module>....s".
+00000dc0: 0000 0c02 0c02 0c01 0c01 0c01 0c02 0c01  ................
+00000dd0: 0c02 0c02 0201 0a01 0e01 0201 06ff 0a04  ................
+00000de0: 0803 1006                                ....
```

### Comparing `garpix_favourite-1.0.0/garpix_favourite/models.py` & `garpix_favourite-2.0.0/garpix_favourite/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from django.db import models
-from django.contrib.auth import get_user_model
 from django.contrib.contenttypes.fields import GenericForeignKey
 from django.contrib.contenttypes.models import ContentType
 from django.utils.translation import gettext_lazy as _
-
-User = get_user_model()
+from garpix_user.models import UserSession
 
 
 class Favorite(models.Model):
     """
         Модель "Избранное" для пользователя.
     """
 
-    user = models.ForeignKey(
-        User, on_delete=models.CASCADE, verbose_name=_('User'),
+    user_session = models.ForeignKey(
+        UserSession, on_delete=models.CASCADE, verbose_name=_('User'),
         related_name='favorites', editable=False
     )
     object_id = models.PositiveIntegerField(
         verbose_name=_('Object ID')
     )
     content_type = models.ForeignKey(
         ContentType, on_delete=models.CASCADE, verbose_name=_('Content type'),
@@ -28,15 +26,15 @@
     )
     created_at = models.DateTimeField(
         auto_now_add=True, verbose_name=_('Created at')
     )
 
     def __str__(self):
         return 'User %i | Favorite: %s %s' % (
-            self.user.id, self.object_id, self.content_object.__class__.__name__
+            self.user_session.id, self.object_id, self.content_object.__class__.__name__
         )
 
     class Meta:
         ordering = ('id',)
         verbose_name = _('Favorite')
         verbose_name_plural = _('Favorites')
-        unique_together = (('user', 'content_type', 'object_id'),)
+        unique_together = (('user_session', 'content_type', 'object_id'),)
```

### Comparing `garpix_favourite-1.0.0/garpix_favourite/serializers.py` & `garpix_favourite-2.0.0/garpix_favourite/serializers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from logging import getLogger
 
 from typing import Optional
 
 from django.conf import settings
 from django.contrib.contenttypes.models import ContentType
 from django.utils.translation import gettext_lazy as _
+from garpix_user.models import UserSession
 
 from rest_framework import serializers
 from rest_framework.exceptions import ValidationError
 
 from .models import Favorite
 
 try:
     ACCEPTED_FAVORITE_MODELS = settings.ACCEPTED_FAVORITE_MODELS
 except AttributeError:
     raise AttributeError(
-        _('ACCEPTED_FAVORITE_MODELS не найдено в настройках.')
+        _('ACCEPTED_FAVORITE_MODELS not found in settings.')
     )
 
 logger = getLogger(__name__)
 
 
 def _get_content_type_by_model_name(model_name: str) -> ContentType:
     model_name = model_name.lower()
@@ -58,28 +59,28 @@
                     'FavoriteMixin обязателен для использования.'
                     % instance.content_object.__class__.__name__
                 )
             )
             return None
 
     def validate(self, attrs):
-        user = self._get_request().user
+        user = UserSession.get_or_create_user_session(self._get_request())
         model_name = attrs['model_name']
         object_id = attrs['object_id']
         content_type = _get_content_type_by_model_name(model_name)
         model = self.Meta.model
 
         if model_class := content_type.model_class():
             if not model_class.objects.filter(id=object_id).exists():
                 raise ValidationError(
                     {'error': _('%s with id %i does not exists.' % (model_name, object_id))}
                 )
 
         if model.objects.filter(
-                user=user,
+                user_session=user,
                 content_type=content_type,
                 object_id=object_id
         ).exists():
             raise ValidationError(
                 {'error': _('The object has already been added to favorites.')}
             )
 
@@ -100,8 +101,8 @@
             'content_type': content_type
         })
 
         return super().create(validated_data)
 
     class Meta:
         model = Favorite
-        exclude = ('user',)
+        exclude = ('user_session',)
```

### Comparing `garpix_favourite-1.0.0/garpix_favourite/setup.py` & `garpix_favourite-2.0.0/garpix_favourite/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 from os import path
-from m2r import convert
-from django.conf import settings
 
+here = path.join(path.abspath(path.dirname(__file__)), 'garpix_favourite')
 
-with open(path.join(settings.BASE_DIR, '..', 'README.md'), encoding='utf-8') as f:
-    long_description = convert(f.read())
+with open(path.join(here, 'README.md'), encoding='utf-8') as f:
+    long_description = f.read()
 
 setup(
     name='garpix_favourite',
-    version='1.0.0',
+    version='2.0.0',
     description='',
     long_description=long_description,
+    long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_favourite',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
     packages=find_packages(exclude=['testproject', 'testproject.*']),
     classifiers=[
         'Development Status :: 4 - Beta',
@@ -26,11 +26,11 @@
         'Programming Language :: Python',
         'Framework :: Django',
         'Programming Language :: Python :: 3.8',
     ],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
-        'garpixcms >= 2.0.2',
+        'garpixcms >= 4.0.0'
     ],
 )
```

### Comparing `garpix_favourite-1.0.0/garpix_favourite/tests.py` & `garpix_favourite-2.0.0/garpix_favourite/tests.py`

 * *Files identical despite different names*

### Comparing `garpix_favourite-1.0.0/garpix_favourite/utils.py` & `garpix_favourite-2.0.0/garpix_favourite/utils.py`

 * *Files identical despite different names*

### Comparing `garpix_favourite-1.0.0/garpix_favourite/views.py` & `garpix_favourite-2.0.0/garpix_favourite/views.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,42 @@
+from drf_spectacular.utils import extend_schema
+from garpix_user.models import UserSession
+from garpix_user.utils.drf_spectacular import user_session_token_header_parameter
 from rest_framework import viewsets, mixins, status
 from rest_framework.decorators import action
 from rest_framework.permissions import IsAuthenticated
 from rest_framework.response import Response
 
 from .models import Favorite
 from .serializers import FavoriteSerializer
 
 
+@extend_schema(
+    parameters=[
+        user_session_token_header_parameter()
+    ]
+)
 class FavoriteViewSet(mixins.CreateModelMixin,
                       mixins.DestroyModelMixin,
                       viewsets.GenericViewSet):
     serializer_class = FavoriteSerializer
-    permission_classes = (IsAuthenticated,)
 
     def get_queryset(self):
+        user = UserSession.get_or_create_user_session(self.request)
         return Favorite.objects.filter(
-            user=self.request.user
+            user_session=user
         )
 
     def perform_create(self, serializer):
+        user = UserSession.get_or_create_user_session(self.request)
         serializer.save(
-            user=self.request.user
+            user_session=user
         )
 
-    @action(methods=['GET'], detail=False, permission_classes=(IsAuthenticated,), url_path='current')
+    @action(methods=['GET'], detail=False, url_path='current')
     def get_user_favorites(self, request):
         queryset = self.filter_queryset(self.get_queryset())
 
         page = self.paginate_queryset(queryset)
         if page is not None:
             serializer = self.get_serializer(page, many=True)
             return self.get_paginated_response(serializer.data)
```

### Comparing `garpix_favourite-1.0.0/garpix_favourite.egg-info/SOURCES.txt` & `garpix_favourite-2.0.0/garpix_favourite.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 MANIFEST.in
 setup.py
+garpix_favourite/CHANGELOG.md
+garpix_favourite/CONTRIBUTING.md
 garpix_favourite/MANIFEST.in
+garpix_favourite/README.md
 garpix_favourite/__init__.py
 garpix_favourite/apps.py
 garpix_favourite/models.py
 garpix_favourite/routers.py
 garpix_favourite/serializers.py
 garpix_favourite/setup.py
 garpix_favourite/tests.py
```

### Comparing `garpix_favourite-1.0.0/setup.py` & `garpix_favourite-2.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 from os import path
-from m2r import convert
-from django.conf import settings
 
+here = path.join(path.abspath(path.dirname(__file__)), 'garpix_favourite')
 
-with open(path.join(settings.BASE_DIR, '..', 'README.md'), encoding='utf-8') as f:
-    long_description = convert(f.read())
+with open(path.join(here, 'README.md'), encoding='utf-8') as f:
+    long_description = f.read()
 
 setup(
     name='garpix_favourite',
-    version='1.0.0',
+    version='2.0.0',
     description='',
     long_description=long_description,
+    long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_favourite',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
     packages=find_packages(exclude=['testproject', 'testproject.*']),
     classifiers=[
         'Development Status :: 4 - Beta',
@@ -26,11 +26,11 @@
         'Programming Language :: Python',
         'Framework :: Django',
         'Programming Language :: Python :: 3.8',
     ],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
-        'garpixcms >= 2.0.2',
+        'garpixcms >= 4.0.0'
     ],
 )
```

