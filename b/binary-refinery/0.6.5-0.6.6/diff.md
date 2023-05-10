# Comparing `tmp/binary-refinery-0.6.5.tar.gz` & `tmp/binary-refinery-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/refinery/refinery/dist/.tmp-r6f6516x/binary-refinery-0.6.5.tar", last modified: Fri May  5 16:11:34 2023, max compression
+gzip compressed data, was "/home/runner/work/refinery/refinery/dist/.tmp-jllhhbmv/binary-refinery-0.6.6.tar", last modified: Wed May 10 11:25:31 2023, max compression
```

## Comparing `binary-refinery-0.6.5.tar` & `binary-refinery-0.6.6.tar`

### file list

```diff
@@ -1,381 +1,381 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/binary_refinery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/binary_refinery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11808 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/binary_refinery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/binary_refinery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/binary_refinery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/binary_refinery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/binary_refinery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/
--rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/__init__.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/data/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49846 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/data/rich.json
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/explore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59048 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/argformats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/argparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/chunks.py
--rw-r--r--   0 runner    (1001) docker     (123)    16375 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/decompression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/deobfuscation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/dex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/lib/dotnet/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/dotnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/dotnet/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    30549 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/dotnet/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/dotnet/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/dotnet/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    19041 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/executable.py
--rw-r--r--   0 runner    (1001) docker     (123)    23050 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)    23540 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/java.py
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/magic.py
--rw-r--r--   0 runner    (1001) docker     (123)    34515 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/mime.py
--rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/mscrypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/murmur.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/lib/patterns/
--rw-r--r--   0 runner    (1001) docker     (123)    16925 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18566 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/patterns/tlds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/powershell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/ripemd128.py
--rw-r--r--   0 runner    (1001) docker     (123)    10358 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/serpent.py
--rw-r--r--   0 runner    (1001) docker     (123)    23138 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/suffixtree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/lib/thirdparty/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/thirdparty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   163388 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/thirdparty/acefile.py
--rw-r--r--   0 runner    (1001) docker     (123)    16823 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/thirdparty/batch_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)   127576 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/thirdparty/pcode2code.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/thirdparty/xxhash.py
--rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/vfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/lib/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/units/
--rw-r--r--   0 runner    (1001) docker     (123)    70098 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/units/blockwise/
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/blockwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/blockwise/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/blockwise/alu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/blockwise/bitrev.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/blockwise/byteswap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/blockwise/map.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/blockwise/neg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/blockwise/pack.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/blockwise/rev.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/blockwise/rotl.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/blockwise/rotr.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/blockwise/shl.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/blockwise/shr.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/blockwise/sub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/blockwise/terminate.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/blockwise/xor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/units/compression/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/compression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/compression/ap.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/compression/blz.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/compression/bz2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/compression/decompress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/compression/jcalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/compression/lz.py
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/compression/lz4.py
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/compression/lzf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/compression/lzg.py
--rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/compression/lzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/compression/lzjb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/compression/lznt1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/compression/lzo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/compression/mscf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/compression/qlz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/compression/szdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/compression/zl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/units/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/units/crypto/cipher/
--rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/cipher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/cipher/aes.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/cipher/blowfish.py
--rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/cipher/camellia.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/cipher/cast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/cipher/chacha.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/cipher/des.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/cipher/des3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/cipher/gost.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/cipher/hc128.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/cipher/isaac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/cipher/rabbit.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/cipher/rc2.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/cipher/rc4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/cipher/rc4mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/cipher/rc5.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/cipher/rc6.py
--rw-r--r--   0 runner    (1001) docker     (123)    48363 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/cipher/rijndael.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/cipher/rncrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/cipher/rot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/cipher/rsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/cipher/rsakey.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/cipher/salsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/cipher/seal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/cipher/secstr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/cipher/serpent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/cipher/tea.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/cipher/vigenere.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/cipher/xtea.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/cipher/xxtea.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/units/crypto/hash/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/hash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/hash/checksums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/hash/cryptographic.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/hash/imphash.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/hash/murmur.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/hash/password_hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/hash/xxhash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/units/crypto/keyderive/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/keyderive/CryptDeriveKey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/keyderive/DESDerive.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/keyderive/PasswordDeriveBytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/keyderive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/keyderive/hkdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/keyderive/hmac.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/keyderive/kblob.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/keyderive/pbkdf1.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/keyderive/pbkdf2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19518 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/crypto/keyderive/unixcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/units/encoding/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/encoding/atbash.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/encoding/b32.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/encoding/b58.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/encoding/b64.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/encoding/b85.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/encoding/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/encoding/cp1252.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/encoding/esc.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/encoding/hex.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/encoding/htmlesc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/encoding/netbios.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/encoding/ps1str.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/encoding/recode.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/encoding/u16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/encoding/url.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/encoding/uuenc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/encoding/wshenc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/units/formats/
--rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/a3x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/units/formats/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/archive/xt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/archive/xt7z.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/archive/xtace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/archive/xtasar.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/archive/xtcab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/archive/xtcpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/archive/xtiso.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/archive/xtiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/archive/xtnode.py
--rw-r--r--   0 runner    (1001) docker     (123)    46989 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/archive/xtnsis.py
--rw-r--r--   0 runner    (1001) docker     (123)    20491 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/archive/xtpyi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/archive/xttar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/archive/xtzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/bat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/deserialize_php.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/dexstr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/email.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/evtx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/units/formats/exe/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/exe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/exe/vaddr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/exe/vmemref.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/exe/vsect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/exe/vsnip.py
--rw-r--r--   0 runner    (1001) docker     (123)    11318 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/exe/vstack.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/hexload.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/html.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/httpresponse.py
--rw-r--r--   0 runner    (1001) docker     (123)    30158 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/ifps.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/ifpsstr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/units/formats/java/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/java/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/java/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/java/jvdasm.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/java/jvstr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/msgpack.py
--rw-r--r--   0 runner    (1001) docker     (123)    13409 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/msi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/units/formats/office/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/office/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/office/doctxt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/office/officecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/office/vbapc.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/office/vbastr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/office/xlmdeobf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/office/xlxtr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/office/xtdoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/office/xtone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/office/xtrtf.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/office/xtvba.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/pcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/pcap_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/units/formats/pe/
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/pe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/units/formats/pe/dotnet/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/pe/dotnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/pe/dotnet/dnblob.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/pe/dotnet/dncfx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/pe/dotnet/dnds.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/pe/dotnet/dnfields.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/pe/dotnet/dnhdr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/pe/dotnet/dnmr.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/pe/dotnet/dnrc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/pe/dotnet/dnstr.py
--rw-r--r--   0 runner    (1001) docker     (123)    30943 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/pe/pemeta.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/pe/peoverlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/pe/perc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/pe/pesig.py
--rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/pe/pestrip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/pkcs7.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/pkcs7sig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/stego.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/tnetmtm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/winreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/formats/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/units/malware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/malware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/malware/n40.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/units/meta/
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/meta/chop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/meta/cm.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/meta/cull.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/meta/dedup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/meta/eat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/meta/ef.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/meta/emit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/meta/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/meta/groupby.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/meta/iff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/meta/iffp.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/meta/iffs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/meta/iffx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/meta/max.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/meta/min.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/meta/mvc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/meta/mvg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/meta/pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/meta/pick.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/meta/pop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/meta/push.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/meta/put.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/meta/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/meta/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/meta/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/meta/sep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/meta/sorted.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/meta/swap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/meta/transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/meta/xfcc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/units/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/misc/autoxor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/misc/couple.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/misc/datefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/misc/drp.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/misc/nop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/misc/urlfix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/misc/xkey.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/units/obfuscation/
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/obfuscation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/units/obfuscation/js/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/obfuscation/js/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/obfuscation/js/arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/obfuscation/js/getattr.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/obfuscation/js/tuples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/units/obfuscation/ps1/
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/obfuscation/ps1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/obfuscation/ps1/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/obfuscation/ps1/brackets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/obfuscation/ps1/cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/obfuscation/ps1/concat.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/obfuscation/ps1/escape.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/obfuscation/ps1/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/obfuscation/ps1/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/obfuscation/ps1/securestring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/obfuscation/ps1/stringreplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/obfuscation/ps1/typecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/obfuscation/ps1/uncurly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/units/obfuscation/vba/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/obfuscation/vba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/obfuscation/vba/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/obfuscation/vba/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/obfuscation/vba/brackets.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/obfuscation/vba/char.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/obfuscation/vba/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/obfuscation/vba/concat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/obfuscation/vba/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/obfuscation/vba/dummies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/obfuscation/vba/stringreplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/obfuscation/vba/stringreverse.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/obfuscation/vba/vba.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/units/pattern/
--rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/pattern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/pattern/carve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/pattern/carve_7z.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/pattern/carve_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/pattern/carve_lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/pattern/carve_pe.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/pattern/carve_rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/pattern/carve_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/pattern/carve_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/pattern/defang.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/pattern/dnsdomain.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/pattern/mimewords.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/pattern/resplit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/pattern/resub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/pattern/rex.py
--rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/pattern/struct_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/pattern/subfiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/pattern/urlguards.py
--rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/pattern/xtp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/pattern/xtw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/units/sinks/
--rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/sinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/sinks/asm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/sinks/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/sinks/iemap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10573 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/sinks/peek.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/sinks/ppjscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/sinks/ppjson.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/sinks/ppxml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/refinery/units/strings/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/strings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/strings/cca.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/strings/ccp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/strings/cfmt.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/strings/clower.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/strings/cswap.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/strings/cupper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/strings/rep.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/strings/repl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/strings/snip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/strings/stretch.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/strings/termfit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/refinery/units/strings/trim.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-05 16:11:34.000000 binary-refinery-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-05 16:11:18.000000 binary-refinery-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/binary_refinery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/binary_refinery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11808 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/binary_refinery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/binary_refinery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/binary_refinery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/binary_refinery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/binary_refinery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/
+-rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/__init__.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49846 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/data/rich.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/explore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59048 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/argformats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/argparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/chunks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16375 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/decompression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/deobfuscation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/dex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/lib/dotnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/dotnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/dotnet/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30549 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/dotnet/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/dotnet/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/dotnet/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19041 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/executable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23050 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23540 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/java.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34515 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/mime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/mscrypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/murmur.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/lib/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)    16925 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18566 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/patterns/tlds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/powershell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/ripemd128.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10358 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/serpent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23138 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/suffixtree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/lib/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/thirdparty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   163388 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/thirdparty/acefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16823 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/thirdparty/batch_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127576 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/thirdparty/pcode2code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/thirdparty/xxhash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/vfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/
+-rw-r--r--   0 runner    (1001) docker     (123)    70717 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/blockwise/
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/alu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/bitrev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/byteswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/neg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/rev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/rotl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/rotr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/shl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/shr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/terminate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/xor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/compression/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/ap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/blz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/bz2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/decompress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/jcalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/lz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/lz4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/lzf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/lzg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/lzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/lzjb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/lznt1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/lzo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/mscf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/qlz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/szdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/zl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/
+-rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/blowfish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/camellia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/chacha.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/des.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/des3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/gost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/hc128.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/isaac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/rabbit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/rc2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/rc4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/rc4mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/rc5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/rc6.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48363 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/rijndael.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/rncrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/rot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/rsakey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/salsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/seal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/secstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/serpent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/tea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/vigenere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/xtea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/xxtea.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/crypto/hash/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/hash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/hash/checksums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/hash/cryptographic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/hash/imphash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/hash/murmur.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/hash/password_hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/hash/xxhash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/crypto/keyderive/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/keyderive/CryptDeriveKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/keyderive/DESDerive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/keyderive/PasswordDeriveBytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/keyderive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/keyderive/hkdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/keyderive/hmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/keyderive/kblob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/keyderive/pbkdf1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/keyderive/pbkdf2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19518 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/keyderive/unixcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/encoding/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/atbash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/b32.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/b58.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/b64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/b85.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/cp1252.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/esc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/htmlesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/netbios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/ps1str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/recode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/u16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/uuenc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/wshenc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/a3x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/formats/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/archive/xt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/archive/xt7z.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/archive/xtace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/archive/xtasar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/archive/xtcab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/archive/xtcpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/archive/xtiso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/archive/xtiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/archive/xtnode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46989 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/archive/xtnsis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20487 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/archive/xtpyi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/archive/xttar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/archive/xtzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/bat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/deserialize_php.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/dexstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/evtx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/formats/exe/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/exe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/exe/vaddr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/exe/vmemref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/exe/vsect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/exe/vsnip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11318 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/exe/vstack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/hexload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/httpresponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30158 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/ifps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/ifpsstr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/formats/java/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/java/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/java/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/java/jvdasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/java/jvstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13409 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/msi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/formats/office/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/office/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/office/doctxt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/office/officecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/office/vbapc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/office/vbastr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/office/xlmdeobf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/office/xlxtr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/office/xtdoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/office/xtone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/office/xtrtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/office/xtvba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pcap_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/formats/pe/
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/dnblob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/dncfx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/dnds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/dnfields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/dnhdr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/dnmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/dnrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/dnstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31022 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pe/pemeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pe/peoverlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pe/perc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pe/pesig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pe/pestrip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pkcs7.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pkcs7sig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/stego.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/tnetmtm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/winreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/malware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/malware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/malware/n40.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/chop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/cm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/cull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/dedup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/eat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/ef.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/groupby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/iff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/iffp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/iffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/iffx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/min.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/mvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/mvg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/pick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/pop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/sep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/sorted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/swap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/xfcc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/misc/autoxor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/misc/couple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/misc/datefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/misc/drp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/misc/nop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/misc/urlfix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/misc/xkey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/obfuscation/
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/obfuscation/js/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/js/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/js/arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/js/getattr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/js/tuples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/obfuscation/ps1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/ps1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/ps1/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/ps1/brackets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/ps1/cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/ps1/concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/ps1/escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/ps1/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/ps1/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/ps1/securestring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/ps1/stringreplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/ps1/typecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/ps1/uncurly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/obfuscation/vba/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/vba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/vba/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/vba/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/vba/brackets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/vba/char.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/vba/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/vba/concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/vba/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/vba/dummies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/vba/stringreplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/vba/stringreverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/vba/vba.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/pattern/
+-rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/carve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/carve_7z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/carve_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/carve_lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/carve_pe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/carve_rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/carve_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/carve_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/defang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/dnsdomain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/mimewords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/resplit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/resub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/rex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/struct_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/subfiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/urlguards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/xtp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/xtw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/sinks/
+-rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/sinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/sinks/asm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/sinks/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/sinks/iemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10573 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/sinks/peek.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/sinks/ppjscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/sinks/ppjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/sinks/ppxml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/strings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/strings/cca.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/strings/ccp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/strings/cfmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/strings/clower.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/strings/cswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/strings/cupper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/strings/rep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/strings/repl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/strings/snip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/strings/stretch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/strings/termfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/strings/trim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/setup.py
```

### Comparing `binary-refinery-0.6.5/LICENSE` & `binary-refinery-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/PKG-INFO` & `binary-refinery-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binary-refinery
-Version: 0.6.5
+Version: 0.6.6
 Summary: A toolkit to transform and refine (mostly) binary data.
 Home-page: https://github.com/binref/refinery/
 Author: Jesko Huettenhain
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `binary-refinery-0.6.5/README.md` & `binary-refinery-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/binary_refinery.egg-info/PKG-INFO` & `binary-refinery-0.6.6/binary_refinery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binary-refinery
-Version: 0.6.5
+Version: 0.6.6
 Summary: A toolkit to transform and refine (mostly) binary data.
 Home-page: https://github.com/binref/refinery/
 Author: Jesko Huettenhain
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `binary-refinery-0.6.5/binary_refinery.egg-info/SOURCES.txt` & `binary-refinery-0.6.6/binary_refinery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/binary_refinery.egg-info/entry_points.txt` & `binary-refinery-0.6.6/binary_refinery.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/binary_refinery.egg-info/requires.txt` & `binary-refinery-0.6.6/binary_refinery.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -5,56 +5,56 @@
 pefile
 pycryptodomex
 pyelftools
 setuptools
 toml
 wheel
 python-magic
-pycdlib
-asn1crypto
-python-registry
-pyxlsb2
+phpserialize
 msoffcrypto-tool
-pyonenote
-extract-msg
-py7zr
-PyPDF2>=3.0.0
+asn1crypto
+Pillow
+pyperclip
 openpyxl
+javaobj-py3>=0.4.0.1
+cabarchive
+py7zr
+extract-msg
 olefile
-LnkParse3
 capstone
+XLMMacroDeobfuscator
 decompyle3
-phpserialize
+LnkParse3
+xlrd2
+pyonenote
+pycdlib
+xdis
 uncompyle6
 chardet
-XLMMacroDeobfuscator
-cabarchive
-javaobj-py3>=0.4.0.1
-pyperclip
-Pillow
-xdis
-xlrd2
+python-registry
+PyPDF2>=3.0.0
+pyxlsb2
 
 [add]
 numpy
 
 [all]
+mitmproxy
 unicorn
+python-evtx
+pyzipper
+angr
+pypcapkit[scapy]<0.16.0
+colorama
 intervaltree
+jsbeautifier
 capstone
-chardet
 numpy
-jsbeautifier
+chardet
 oletools
-mitmproxy
-angr
-python-evtx
-pypcapkit[scapy]<0.16.0
-pyzipper
-colorama
 
 [alu]
 numpy
 
 [asm]
 angr
```

### Comparing `binary-refinery-0.6.5/refinery/__init__.pkl` & `binary-refinery-0.6.6/refinery/__init__.pkl`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/__init__.py` & `binary-refinery-0.6.6/refinery/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 1. `refinery.lib.frame`: framing syntax for working on lists of binary chunks
 2. `refinery.lib.argformats`: the multibin syntax for refinery arguments
 3. `refinery.lib.meta`: defining and using metadata variables within frames
 4. `refinery.units`: writing custom units, add command-line arguments, and how to use refinery
    units within Python code.
 """
-__version__ = '0.6.5'
+__version__ = '0.6.6'
 __distribution__ = 'binary-refinery'
 
 from typing import Dict, List, Optional, Type
 from importlib import resources
 from datetime import datetime
 
 import pickle
```

### Comparing `binary-refinery-0.6.5/refinery/data/rich.json` & `binary-refinery-0.6.6/refinery/data/rich.json`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/explore.py` & `binary-refinery-0.6.6/refinery/explore.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/argformats.py` & `binary-refinery-0.6.6/refinery/lib/argformats.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/argparser.py` & `binary-refinery-0.6.6/refinery/lib/argparser.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/chunks.py` & `binary-refinery-0.6.6/refinery/lib/chunks.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/crypto.py` & `binary-refinery-0.6.6/refinery/lib/crypto.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/decompression.py` & `binary-refinery-0.6.6/refinery/lib/decompression.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/decorators.py` & `binary-refinery-0.6.6/refinery/lib/decorators.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/deobfuscation.py` & `binary-refinery-0.6.6/refinery/lib/deobfuscation.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/dex.py` & `binary-refinery-0.6.6/refinery/lib/dex.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/dotnet/deserialize.py` & `binary-refinery-0.6.6/refinery/lib/dotnet/deserialize.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/dotnet/header.py` & `binary-refinery-0.6.6/refinery/lib/dotnet/header.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/dotnet/resources.py` & `binary-refinery-0.6.6/refinery/lib/dotnet/resources.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/dotnet/types.py` & `binary-refinery-0.6.6/refinery/lib/dotnet/types.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/environment.py` & `binary-refinery-0.6.6/refinery/lib/environment.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/executable.py` & `binary-refinery-0.6.6/refinery/lib/executable.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/frame.py` & `binary-refinery-0.6.6/refinery/lib/frame.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/inline.py` & `binary-refinery-0.6.6/refinery/lib/inline.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/java.py` & `binary-refinery-0.6.6/refinery/lib/java.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/json.py` & `binary-refinery-0.6.6/refinery/lib/json.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/loader.py` & `binary-refinery-0.6.6/refinery/lib/loader.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/magic.py` & `binary-refinery-0.6.6/refinery/lib/magic.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/meta.py` & `binary-refinery-0.6.6/refinery/lib/meta.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/mime.py` & `binary-refinery-0.6.6/refinery/lib/mime.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/mscrypto.py` & `binary-refinery-0.6.6/refinery/lib/mscrypto.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/murmur.py` & `binary-refinery-0.6.6/refinery/lib/murmur.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/patterns/__init__.py` & `binary-refinery-0.6.6/refinery/lib/patterns/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/patterns/tlds.py` & `binary-refinery-0.6.6/refinery/lib/patterns/tlds.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/powershell.py` & `binary-refinery-0.6.6/refinery/lib/powershell.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/ripemd128.py` & `binary-refinery-0.6.6/refinery/lib/ripemd128.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/serpent.py` & `binary-refinery-0.6.6/refinery/lib/serpent.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/structures.py` & `binary-refinery-0.6.6/refinery/lib/structures.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/suffixtree.py` & `binary-refinery-0.6.6/refinery/lib/suffixtree.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/thirdparty/acefile.py` & `binary-refinery-0.6.6/refinery/lib/thirdparty/acefile.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/thirdparty/batch_interpreter.py` & `binary-refinery-0.6.6/refinery/lib/thirdparty/batch_interpreter.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/thirdparty/pcode2code.py` & `binary-refinery-0.6.6/refinery/lib/thirdparty/pcode2code.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/thirdparty/xxhash.py` & `binary-refinery-0.6.6/refinery/lib/thirdparty/xxhash.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/tools.py` & `binary-refinery-0.6.6/refinery/lib/tools.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/types.py` & `binary-refinery-0.6.6/refinery/lib/types.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/vfs.py` & `binary-refinery-0.6.6/refinery/lib/vfs.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/lib/xml.py` & `binary-refinery-0.6.6/refinery/lib/xml.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/__init__.py` & `binary-refinery-0.6.6/refinery/units/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -381,14 +381,27 @@
         try:
             return cls(value)
         except Exception as E:
             choices = ', '.join([option.name for option in cls])
             raise ValueError(F'Could not transform {value} into {cls.__name__}; the choices are: {choices}') from E
 
     @classmethod
+    def Counts(
+        cls,
+        *args   : str,
+        help    : Union[omit, str] = omit,
+        dest    : Union[omit, str] = omit,
+        group   : Optional[str] = None,
+    ):
+        """
+        A convenience method to add argparse arguments that introduce a counter.
+        """
+        return cls(*args, group=group, help=help, dest=dest, action='count')
+
+    @classmethod
     def Switch(
         cls,
         *args   : str, off=False,
         help    : Union[omit, str] = omit,
         dest    : Union[omit, str] = omit,
         group   : Optional[str] = None,
     ):
@@ -407,15 +420,17 @@
         nargs   : Union[omit, int, str] = omit,
         metavar : Optional[str] = None,
         group   : Optional[str] = None,
     ):
         """
         Used to add argparse arguments that contain binary data.
         """
-        return cls(*args, group=group, help=help, dest=dest, nargs=nargs, type=multibin, metavar=metavar or 'B')
+        if metavar is None and any('-' in a for a in args):
+            metavar = 'B'
+        return cls(*args, group=group, help=help, dest=dest, nargs=nargs, type=multibin, metavar=metavar)
 
     @classmethod
     def NumSeq(
         cls,
         *args   : str,
         help    : Union[omit, str] = omit,
         dest    : Union[omit, str] = omit,
@@ -629,18 +644,20 @@
     def merge_all(self, them: Arg) -> None:
         for key, value in them.kwargs.items():
             if value is Arg.delete:
                 self.kwargs.pop(key, None)
                 self.guessed.discard(key)
                 continue
             if key in them.guessed:
-                if key in self.kwargs and key not in self.guessed:
-                    continue
-                else:
-                    self.guessed.add(key)
+                if key not in self.guessed:
+                    if key == 'type' and self.kwargs.get('action', None) != 'store':
+                        continue
+                    if key in self.kwargs:
+                        continue
+                self.guessed.add(key)
             self.kwargs[key] = value
         self.merge_args(them)
         self.group = them.group or self.group
 
     def __copy__(self) -> Argument:
         cls = self.__class__
         clone = cls.__new__(cls)
@@ -1522,15 +1539,15 @@
                 return (self | stdout).getvalue()
         elif callable(stream):
             with MemoryFile(bytearray()) as stdout:
                 self | stdout
                 out: bytearray = stdout.getbuffer()
                 if isinstance(stream, type) and isinstance(out, stream):
                     return out
-                if stream is str:
+                if isinstance(stream, type) and issubclass(stream, str):
                     out = out.decode(self.codec)
                 return stream(out)
 
         stream: ByteIO
 
         if not stream.writable():
             raise ValueError('target stream is not writable')
```

### Comparing `binary-refinery-0.6.5/refinery/units/blockwise/__init__.py` & `binary-refinery-0.6.6/refinery/units/blockwise/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/blockwise/alu.py` & `binary-refinery-0.6.6/refinery/units/blockwise/alu.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/blockwise/bitrev.py` & `binary-refinery-0.6.6/refinery/units/blockwise/bitrev.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/blockwise/byteswap.py` & `binary-refinery-0.6.6/refinery/units/blockwise/byteswap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/blockwise/map.py` & `binary-refinery-0.6.6/refinery/units/blockwise/map.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/blockwise/pack.py` & `binary-refinery-0.6.6/refinery/units/blockwise/pack.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/blockwise/rev.py` & `binary-refinery-0.6.6/refinery/units/blockwise/rev.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/blockwise/terminate.py` & `binary-refinery-0.6.6/refinery/units/blockwise/terminate.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/blockwise/xor.py` & `binary-refinery-0.6.6/refinery/units/blockwise/xor.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/compression/ap.py` & `binary-refinery-0.6.6/refinery/units/compression/ap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/compression/blz.py` & `binary-refinery-0.6.6/refinery/units/compression/blz.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/compression/bz2.py` & `binary-refinery-0.6.6/refinery/units/compression/bz2.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/compression/decompress.py` & `binary-refinery-0.6.6/refinery/units/compression/decompress.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/compression/jcalg.py` & `binary-refinery-0.6.6/refinery/units/compression/jcalg.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/compression/lz.py` & `binary-refinery-0.6.6/refinery/units/compression/lz.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/compression/lz4.py` & `binary-refinery-0.6.6/refinery/units/compression/lz4.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/compression/lzf.py` & `binary-refinery-0.6.6/refinery/units/compression/lzf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/compression/lzg.py` & `binary-refinery-0.6.6/refinery/units/compression/lzg.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/compression/lzip.py` & `binary-refinery-0.6.6/refinery/units/compression/lzip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/compression/lzjb.py` & `binary-refinery-0.6.6/refinery/units/compression/lzjb.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/compression/lznt1.py` & `binary-refinery-0.6.6/refinery/units/compression/lznt1.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/compression/lzo.py` & `binary-refinery-0.6.6/refinery/units/compression/lzo.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/compression/mscf.py` & `binary-refinery-0.6.6/refinery/units/compression/mscf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/compression/qlz.py` & `binary-refinery-0.6.6/refinery/units/compression/qlz.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/compression/szdd.py` & `binary-refinery-0.6.6/refinery/units/compression/szdd.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/compression/zl.py` & `binary-refinery-0.6.6/refinery/units/compression/zl.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/cipher/__init__.py` & `binary-refinery-0.6.6/refinery/units/crypto/cipher/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/cipher/camellia.py` & `binary-refinery-0.6.6/refinery/units/crypto/cipher/camellia.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/cipher/chacha.py` & `binary-refinery-0.6.6/refinery/units/crypto/cipher/chacha.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/cipher/gost.py` & `binary-refinery-0.6.6/refinery/units/crypto/cipher/gost.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/cipher/hc128.py` & `binary-refinery-0.6.6/refinery/units/crypto/cipher/hc128.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/cipher/isaac.py` & `binary-refinery-0.6.6/refinery/units/crypto/cipher/isaac.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/cipher/rabbit.py` & `binary-refinery-0.6.6/refinery/units/crypto/cipher/rabbit.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/cipher/rc2.py` & `binary-refinery-0.6.6/refinery/units/crypto/cipher/rc2.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/cipher/rc4mod.py` & `binary-refinery-0.6.6/refinery/units/crypto/cipher/rc4mod.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/cipher/rc5.py` & `binary-refinery-0.6.6/refinery/units/crypto/cipher/rc5.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/cipher/rc6.py` & `binary-refinery-0.6.6/refinery/units/crypto/cipher/rc6.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/cipher/rijndael.py` & `binary-refinery-0.6.6/refinery/units/crypto/cipher/rijndael.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/cipher/rncrypt.py` & `binary-refinery-0.6.6/refinery/units/crypto/cipher/rncrypt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/cipher/rot.py` & `binary-refinery-0.6.6/refinery/units/crypto/cipher/rot.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/cipher/rsa.py` & `binary-refinery-0.6.6/refinery/units/crypto/cipher/rsa.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/cipher/rsakey.py` & `binary-refinery-0.6.6/refinery/units/crypto/cipher/rsakey.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/cipher/salsa.py` & `binary-refinery-0.6.6/refinery/units/crypto/cipher/salsa.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/cipher/seal.py` & `binary-refinery-0.6.6/refinery/units/crypto/cipher/seal.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/cipher/secstr.py` & `binary-refinery-0.6.6/refinery/units/crypto/cipher/secstr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/cipher/serpent.py` & `binary-refinery-0.6.6/refinery/units/crypto/cipher/serpent.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/cipher/tea.py` & `binary-refinery-0.6.6/refinery/units/crypto/cipher/tea.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/cipher/vigenere.py` & `binary-refinery-0.6.6/refinery/units/crypto/cipher/vigenere.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/cipher/xtea.py` & `binary-refinery-0.6.6/refinery/units/crypto/cipher/xtea.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/cipher/xxtea.py` & `binary-refinery-0.6.6/refinery/units/crypto/cipher/xxtea.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/hash/__init__.py` & `binary-refinery-0.6.6/refinery/units/crypto/hash/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/hash/checksums.py` & `binary-refinery-0.6.6/refinery/units/crypto/hash/checksums.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/hash/cryptographic.py` & `binary-refinery-0.6.6/refinery/units/crypto/hash/cryptographic.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/hash/imphash.py` & `binary-refinery-0.6.6/refinery/units/crypto/hash/imphash.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/hash/murmur.py` & `binary-refinery-0.6.6/refinery/units/crypto/hash/murmur.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/hash/xxhash.py` & `binary-refinery-0.6.6/refinery/units/crypto/hash/xxhash.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/keyderive/CryptDeriveKey.py` & `binary-refinery-0.6.6/refinery/units/crypto/keyderive/CryptDeriveKey.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/keyderive/DESDerive.py` & `binary-refinery-0.6.6/refinery/units/crypto/keyderive/DESDerive.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/keyderive/PasswordDeriveBytes.py` & `binary-refinery-0.6.6/refinery/units/crypto/keyderive/PasswordDeriveBytes.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/keyderive/__init__.py` & `binary-refinery-0.6.6/refinery/units/crypto/keyderive/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/keyderive/kblob.py` & `binary-refinery-0.6.6/refinery/units/crypto/keyderive/kblob.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/keyderive/pbkdf1.py` & `binary-refinery-0.6.6/refinery/units/crypto/keyderive/pbkdf1.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/keyderive/pbkdf2.py` & `binary-refinery-0.6.6/refinery/units/crypto/keyderive/pbkdf2.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/crypto/keyderive/unixcrypt.py` & `binary-refinery-0.6.6/refinery/units/crypto/keyderive/unixcrypt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/encoding/atbash.py` & `binary-refinery-0.6.6/refinery/units/encoding/atbash.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/encoding/b32.py` & `binary-refinery-0.6.6/refinery/units/encoding/b32.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/encoding/b64.py` & `binary-refinery-0.6.6/refinery/units/encoding/b64.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,21 +8,19 @@
 class b64(Unit):
     """
     Base64 encoding and decoding.
     """
     def __init__(self, urlsafe: Arg.Switch('-u', help='use URL-safe alphabet') = False):
         super().__init__(urlsafe=urlsafe)
 
-    @property
-    def altchars(self):
-        if self.args.urlsafe:
-            return B'-_'
-
     def reverse(self, data):
-        return base64.b64encode(data, altchars=self.altchars)
+        altchars = None
+        if self.args.urlsafe:
+            altchars = B'-_'
+        return base64.b64encode(data, altchars=altchars)
 
     def process(self, data: bytearray):
         if not data:
             return data
         if len(data) == 1:
             raise ValueError('single byte can not be base64-decoded.')
         data.extend(B'===')
```

### Comparing `binary-refinery-0.6.5/refinery/units/encoding/base.py` & `binary-refinery-0.6.6/refinery/units/encoding/base.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/encoding/esc.py` & `binary-refinery-0.6.6/refinery/units/encoding/esc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/encoding/hex.py` & `binary-refinery-0.6.6/refinery/units/encoding/hex.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/encoding/netbios.py` & `binary-refinery-0.6.6/refinery/units/encoding/netbios.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/encoding/ps1str.py` & `binary-refinery-0.6.6/refinery/units/encoding/ps1str.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/encoding/recode.py` & `binary-refinery-0.6.6/refinery/units/encoding/recode.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/encoding/url.py` & `binary-refinery-0.6.6/refinery/units/encoding/url.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/encoding/uuenc.py` & `binary-refinery-0.6.6/refinery/units/encoding/uuenc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/encoding/wshenc.py` & `binary-refinery-0.6.6/refinery/units/encoding/wshenc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/__init__.py` & `binary-refinery-0.6.6/refinery/units/formats/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,40 +43,38 @@
 
 class EndOfStringNotFound(ValueError):
     def __init__(self):
         super().__init__('end of string could not be determined')
 
 
 class PathPattern:
-    def __init__(self, pp: Union[str, re.Pattern], regex=False, fuzzy=False):
+    def __init__(self, pp: Union[str, re.Pattern], regex=False, fuzzy=0):
         if isinstance(pp, re.Pattern):
             self.stops = []
             self.pattern = pp
             return
         elif not regex:
             self.stops = [stop for stop in re.split(R'(.*?[/*?])', pp) if stop]
             pp, _, _ = fnmatch.translate(pp).partition(r'\Z')
-        pattern = re.compile(pp)
-        self._check = self._fuzzy = pattern.search
-        if not fuzzy:
-            self._check = pattern.fullmatch
+        p1 = re.compile(pp)
+        p2 = re.compile(F'.*?{pp}')
+        self.matchers = [p1.fullmatch, p2.fullmatch, p1.search]
+        self.fuzzy = fuzzy
 
     def reach(self, path):
         if not any(self.stops):
             return True
         for stop in self.stops:
             if fnmatch.fnmatch(path, stop):
                 return True
         return False
 
-    def check(self, path, fuzzy=False):
-        if fuzzy:
-            return self._fuzzy(path)
-        else:
-            return self._check(path)
+    def check(self, path, fuzzy=0):
+        fuzzy = min(max(fuzzy, self.fuzzy), 2)
+        return self.matchers[fuzzy](path)
 
     def __repr__(self):
         return F'<PathPattern:{"//".join(self.stops) or "RE"}>'
 
 
 class PathExtractorUnit(Unit, abstract=True):
 
@@ -84,24 +82,25 @@
 
     def __init__(
         self,
         *paths: Arg.Binary(metavar='path', nargs='*', help=(
             'Wildcard pattern for the path of the item to be extracted. Each item is returned '
             'as a separate output of this unit. Paths may contain wildcards; The default '
             'argument is a single wildcard, which means that every item will be extracted. If '
-            'a given path yields no results, the unit attempts to perform a fuzzy search with '
-            'it instead. This can be disabled using the --exact switch.')),
+            'a given path yields no results, the unit performs increasingly fuzzy searches '
+            'with it. This can be disabled using the --exact switch.')),
         list: Arg.Switch('-l',
             help='Return all matching paths as UTF8-encoded output chunks.') = False,
         join_path: Arg.Switch('-j', group='PATH',
             help='Join path names from container with previous path names.') = False,
         drop_path: Arg.Switch('-d', group='PATH',
             help='Do not modify the path variable for output chunks.') = False,
-        fuzzy: Arg.Switch('-z', group='MATCH',
-            help='Path patterns always match on substrings rather than whole paths.') = False,
+        fuzzy: Arg.Counts('-z', group='MATCH', help=(
+            'Specify once to add a leading wildcard to each patterns, twice to also add a '
+            'trailing wildcard.')) = 0,
         exact: Arg.Switch('-e', group='MATCH',
             help='Path patterns never match on substrings.') = False,
         regex: Arg.Switch('-r',
             help='Use regular expressions instead of wildcard patterns.') = False,
         path: Arg('-P', metavar='NAME', help=(
             'Name of the meta variable to receive the extracted path. The default value is '
             '"{default}".')) = b'path',
@@ -200,15 +199,15 @@
                 if any(F'{base}.v{c:0{width}d}{extension}' in occurrences for c in range(occurrences[path])):
                     result.path = F'{base}.{uuid.uuid4()}{extension}'
                 else:
                     result.path = F'{base}.v{counter:0{width}d}{extension}'
                 self.log_warn(F'read chunk with duplicate path; deduplicating to {result.path}')
 
         for p in patterns:
-            for fuzzy in (False, True):
+            for fuzzy in range(3):
                 done = self.args.exact
                 for result in results:
                     path = result.path
                     if not p.check(path, fuzzy):
                         continue
                     done = True
                     if self.args.list:
```

### Comparing `binary-refinery-0.6.5/refinery/units/formats/a3x.py` & `binary-refinery-0.6.6/refinery/units/formats/a3x.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/archive/__init__.py` & `binary-refinery-0.6.6/refinery/units/formats/archive/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datetime import datetime
 
 from refinery.units.formats import Arg, PathExtractorUnit, UnpackResult
 
 
 class ArchiveUnit(PathExtractorUnit, abstract=True):
     def __init__(
-        self, *paths, list=False, join_path=False, drop_path=False, fuzzy=False, exact=False, regex=False, path=b'path',
+        self, *paths, list=False, join_path=False, drop_path=False, fuzzy=0, exact=False, regex=False, path=b'path',
         date: Arg('-D', metavar='NAME',
             help='Name of the meta variable to receive the extracted file date. The default value is "{default}".') = b'date',
         pwd: Arg('-p', help='Optionally specify an extraction password.') = B'',
         **kwargs
     ):
         super().__init__(
             *paths,
```

### Comparing `binary-refinery-0.6.5/refinery/units/formats/archive/xt.py` & `binary-refinery-0.6.6/refinery/units/formats/archive/xt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/archive/xt7z.py` & `binary-refinery-0.6.6/refinery/units/formats/archive/xt7z.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/archive/xtace.py` & `binary-refinery-0.6.6/refinery/units/formats/archive/xtace.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/archive/xtasar.py` & `binary-refinery-0.6.6/refinery/units/formats/archive/xtasar.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/archive/xtcab.py` & `binary-refinery-0.6.6/refinery/units/formats/archive/xtcab.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/archive/xtcpio.py` & `binary-refinery-0.6.6/refinery/units/formats/archive/xtcpio.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/archive/xtiso.py` & `binary-refinery-0.6.6/refinery/units/formats/archive/xtiso.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class xtiso(ArchiveUnit):
     """
     Extract files from a ISO archive.
     """
     def __init__(
         self,
-        *paths, list=False, join_path=False, drop_path=False, fuzzy=False, exact=False, regex=False,
+        *paths, list=False, join_path=False, drop_path=False, fuzzy=0, exact=False, regex=False,
         path=b'path', date=b'date',
         fs: Arg.Choice('-s', metavar='TYPE', choices=_ISO_FILE_SYSTEMS, help=(
             'Specify a file system ({choices}) extension to use. The default setting {default} will automatically '
             'detect the first of the other available options and use it.')) = 'auto'
     ):
         if fs not in _ISO_FILE_SYSTEMS:
             raise ValueError(F'invalid file system {fs}: must be udf, joliet, rr, iso, or auto.')
```

### Comparing `binary-refinery-0.6.5/refinery/units/formats/archive/xtiss.py` & `binary-refinery-0.6.6/refinery/units/formats/archive/xtiss.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/archive/xtnode.py` & `binary-refinery-0.6.6/refinery/units/formats/archive/xtnode.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     _PKG_PAYLOAD_P = B'PAYLOAD_POSITION'
     _PKG_PAYLOAD_S = B'PAYLOAD_SIZE'
     _PKG_PRELUDE_P = B'PRELUDE_POSITION'
     _PKG_PRELUDE_S = B'PRELUDE_SIZE'
 
     def __init__(
         self, *paths, entry: Arg.Switch('-u', help='Only extract the entry point.') = False,
-        list=False, join_path=False, drop_path=False, fuzzy=False, exact=False, regex=False,
+        list=False, join_path=False, drop_path=False, fuzzy=0, exact=False, regex=False,
         path=b'path', date=b'date',
     ):
         super().__init__(*paths, entry=entry,
             list=list, join_path=join_path, drop_path=drop_path, fuzzy=fuzzy, exact=exact, regex=regex,
             path=path, date=date)
 
     def unpack(self, data: ByteStr) -> Iterable[UnpackResult]:
```

### Comparing `binary-refinery-0.6.5/refinery/units/formats/archive/xtnsis.py` & `binary-refinery-0.6.6/refinery/units/formats/archive/xtnsis.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/archive/xtpyi.py` & `binary-refinery-0.6.6/refinery/units/formats/archive/xtpyi.py`

 * *Files 0% similar despite different names*

```diff
@@ -444,15 +444,15 @@
 
 
 class xtpyi(ArchiveUnit):
     """
     Extracts and decompiles files from a Python Installer (aka PyInstaller) archive.
     """
     def __init__(
-        self, *paths, list=False, join_path=False, drop_path=False, fuzzy=False, exact=False, regex=False,
+        self, *paths, list=False, join_path=False, drop_path=False, fuzzy=0, exact=False, regex=False,
         path=b'path', date=b'date',
         user_code: Arg.Switch('-u', group='FILTER', help=(
             'Extract only source code files from the root of the archive. These usually implement '
             'the actual domain logic.')) = False,
         unmarshal: Arg('-y', action='count', group='FILTER', help=(
             '(DANGEROUS) Unmarshal embedded PYZ archives. Warning: Maliciously crafted packages can '
             'potentially exploit this to execute code. It is advised to only use this option inside '
```

### Comparing `binary-refinery-0.6.5/refinery/units/formats/archive/xttar.py` & `binary-refinery-0.6.6/refinery/units/formats/archive/xttar.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/archive/xtzip.py` & `binary-refinery-0.6.6/refinery/units/formats/archive/xtzip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/bat.py` & `binary-refinery-0.6.6/refinery/units/formats/bat.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/csv.py` & `binary-refinery-0.6.6/refinery/units/formats/csv.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/deserialize_php.py` & `binary-refinery-0.6.6/refinery/units/formats/deserialize_php.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/email.py` & `binary-refinery-0.6.6/refinery/units/formats/email.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/evtx.py` & `binary-refinery-0.6.6/refinery/units/formats/evtx.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/exe/vaddr.py` & `binary-refinery-0.6.6/refinery/units/formats/exe/vaddr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/exe/vmemref.py` & `binary-refinery-0.6.6/refinery/units/formats/exe/vmemref.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/exe/vsect.py` & `binary-refinery-0.6.6/refinery/units/formats/exe/vsect.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/exe/vsnip.py` & `binary-refinery-0.6.6/refinery/units/formats/exe/vsnip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/exe/vstack.py` & `binary-refinery-0.6.6/refinery/units/formats/exe/vstack.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/hexload.py` & `binary-refinery-0.6.6/refinery/units/formats/hexload.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/html.py` & `binary-refinery-0.6.6/refinery/units/formats/html.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/httpresponse.py` & `binary-refinery-0.6.6/refinery/units/formats/httpresponse.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/ifps.py` & `binary-refinery-0.6.6/refinery/units/formats/ifps.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/ifpsstr.py` & `binary-refinery-0.6.6/refinery/units/formats/ifpsstr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/java/deserialize.py` & `binary-refinery-0.6.6/refinery/units/formats/java/deserialize.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/java/jvdasm.py` & `binary-refinery-0.6.6/refinery/units/formats/java/jvdasm.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/json.py` & `binary-refinery-0.6.6/refinery/units/formats/json.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,16 +51,16 @@
     extract remaining fields as metadata: String values are extracted only if they do not exceed 80
     characters in length and do not contain any line breaks. Floating-point, integer, boolean values, and
     lists of the latter are also extracted.
     """
     def __init__(
         self,
         key: Unit.Arg.Binary(help='Optional key of a value to become the main body of the chunk.') = None,
-        raw: Unit.Arg('-r', group='META', help='Do not extract any other fields as metadata.') = False,
-        all: Unit.Arg('-a', group='META', help='Extract all other fields as metadata.') = False
+        raw: Unit.Arg.Switch('-r', group='META', help='Do not extract any other fields as metadata.') = False,
+        all: Unit.Arg.Switch('-a', group='META', help='Extract all other fields as metadata.') = False
     ):
         super().__init__(key=key, raw=raw, all=all)
 
     def process(self, data):
 
         def acceptable(key, value, inside_list=False):
             if not is_valid_variable_name(key):
```

### Comparing `binary-refinery-0.6.5/refinery/units/formats/lnk.py` & `binary-refinery-0.6.6/refinery/units/formats/lnk.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/msgpack.py` & `binary-refinery-0.6.6/refinery/units/formats/msgpack.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/msi.py` & `binary-refinery-0.6.6/refinery/units/formats/msi.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/office/doctxt.py` & `binary-refinery-0.6.6/refinery/units/formats/office/doctxt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/office/officecrypt.py` & `binary-refinery-0.6.6/refinery/units/formats/office/officecrypt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/office/vbapc.py` & `binary-refinery-0.6.6/refinery/units/formats/office/vbapc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/office/vbastr.py` & `binary-refinery-0.6.6/refinery/units/formats/office/vbastr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/office/xlmdeobf.py` & `binary-refinery-0.6.6/refinery/units/formats/office/xlmdeobf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/office/xlxtr.py` & `binary-refinery-0.6.6/refinery/units/formats/office/xlxtr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/office/xtdoc.py` & `binary-refinery-0.6.6/refinery/units/formats/office/xtdoc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/office/xtone.py` & `binary-refinery-0.6.6/refinery/units/formats/office/xtone.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/office/xtrtf.py` & `binary-refinery-0.6.6/refinery/units/formats/office/xtrtf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/office/xtvba.py` & `binary-refinery-0.6.6/refinery/units/formats/office/xtvba.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/pcap.py` & `binary-refinery-0.6.6/refinery/units/formats/pcap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/pcap_http.py` & `binary-refinery-0.6.6/refinery/units/formats/pcap_http.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/pdf.py` & `binary-refinery-0.6.6/refinery/units/formats/pdf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/pe/__init__.py` & `binary-refinery-0.6.6/refinery/units/formats/pe/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/pe/dotnet/__init__.py` & `binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/pe/dotnet/dncfx.py` & `binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/dncfx.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/pe/dotnet/dnds.py` & `binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/dnds.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/pe/dotnet/dnfields.py` & `binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/dnfields.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/pe/dotnet/dnhdr.py` & `binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/dnhdr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/pe/dotnet/dnmr.py` & `binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/dnmr.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class dnmr(PathExtractorUnit):
     """
     Extracts subfiles from .NET managed resources.
     """
     def __init__(
-        self, *paths, list=False, join_path=False, drop_path=False, exact=False, fuzzy=False, regex=False, path=b'name',
+        self, *paths, list=False, join_path=False, drop_path=False, exact=False, fuzzy=0, regex=False, path=b'name',
         raw: Arg.Switch('-w', help='Do not deserialize the managed resource entry data.') = False
     ):
         super().__init__(
             *paths,
             list=list,
             join_path=join_path,
             drop_path=drop_path,
```

### Comparing `binary-refinery-0.6.5/refinery/units/formats/pe/dotnet/dnrc.py` & `binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/dnrc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/pe/dotnet/dnstr.py` & `binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/dnstr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/pe/pemeta.py` & `binary-refinery-0.6.6/refinery/units/formats/pe/pemeta.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,14 +246,16 @@
                         main_certificate = certificate
                         break
             if main_certificate is None and len(certificates_with_extended_use) == 1:
                 main_certificate = certificates_with_extended_use[0]
         if main_certificate:
             crt = main_certificate['tbs_certificate']
             serial = crt['serial_number']
+            if isinstance(serial, int):
+                serial = F'{serial:x}'
             assert bytes.fromhex(serial) in data
             subject = crt['subject']
             location = [subject.get(t, '') for t in ('locality_name', 'state_or_province_name', 'country_name')]
             info.update(Subject=subject['common_name'])
             if any(location):
                 info.update(SubjectLocation=', '.join(filter(None, location)))
             for signer_info in signature['content'].get('signer_infos', ()):
```

### Comparing `binary-refinery-0.6.5/refinery/units/formats/pe/peoverlay.py` & `binary-refinery-0.6.6/refinery/units/formats/pe/peoverlay.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/pe/perc.py` & `binary-refinery-0.6.6/refinery/units/formats/pe/perc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/pe/pesig.py` & `binary-refinery-0.6.6/refinery/units/formats/pe/pesig.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/pe/pestrip.py` & `binary-refinery-0.6.6/refinery/units/formats/pe/pestrip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/pkcs7.py` & `binary-refinery-0.6.6/refinery/units/formats/pkcs7.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/pkcs7sig.py` & `binary-refinery-0.6.6/refinery/units/formats/pkcs7sig.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/stego.py` & `binary-refinery-0.6.6/refinery/units/formats/stego.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/tnetmtm.py` & `binary-refinery-0.6.6/refinery/units/formats/tnetmtm.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/winreg.py` & `binary-refinery-0.6.6/refinery/units/formats/winreg.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/formats/xml.py` & `binary-refinery-0.6.6/refinery/units/formats/xml.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/malware/n40.py` & `binary-refinery-0.6.6/refinery/units/malware/n40.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/meta/__init__.py` & `binary-refinery-0.6.6/refinery/units/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/meta/chop.py` & `binary-refinery-0.6.6/refinery/units/meta/chop.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/meta/cm.py` & `binary-refinery-0.6.6/refinery/units/meta/cm.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/meta/cull.py` & `binary-refinery-0.6.6/refinery/units/meta/cull.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/meta/dedup.py` & `binary-refinery-0.6.6/refinery/units/meta/dedup.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/meta/eat.py` & `binary-refinery-0.6.6/refinery/units/meta/eat.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/meta/ef.py` & `binary-refinery-0.6.6/refinery/units/meta/ef.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/meta/emit.py` & `binary-refinery-0.6.6/refinery/units/meta/emit.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/meta/group.py` & `binary-refinery-0.6.6/refinery/units/meta/group.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/meta/groupby.py` & `binary-refinery-0.6.6/refinery/units/meta/groupby.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/meta/iff.py` & `binary-refinery-0.6.6/refinery/units/meta/iff.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/meta/iffp.py` & `binary-refinery-0.6.6/refinery/units/meta/iffp.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/meta/iffs.py` & `binary-refinery-0.6.6/refinery/units/meta/iffs.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/meta/iffx.py` & `binary-refinery-0.6.6/refinery/units/meta/iffx.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/meta/max.py` & `binary-refinery-0.6.6/refinery/units/meta/max.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/meta/min.py` & `binary-refinery-0.6.6/refinery/units/meta/min.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/meta/mvc.py` & `binary-refinery-0.6.6/refinery/units/meta/mvc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/meta/mvg.py` & `binary-refinery-0.6.6/refinery/units/meta/mvg.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/meta/pad.py` & `binary-refinery-0.6.6/refinery/units/meta/pad.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/meta/pick.py` & `binary-refinery-0.6.6/refinery/units/meta/pick.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/meta/pop.py` & `binary-refinery-0.6.6/refinery/units/meta/pop.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/meta/push.py` & `binary-refinery-0.6.6/refinery/units/meta/push.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/meta/put.py` & `binary-refinery-0.6.6/refinery/units/meta/put.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/meta/queue.py` & `binary-refinery-0.6.6/refinery/units/meta/queue.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/meta/reduce.py` & `binary-refinery-0.6.6/refinery/units/meta/reduce.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/meta/scope.py` & `binary-refinery-0.6.6/refinery/units/meta/scope.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/meta/sep.py` & `binary-refinery-0.6.6/refinery/units/meta/sep.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/meta/sorted.py` & `binary-refinery-0.6.6/refinery/units/meta/sorted.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/meta/swap.py` & `binary-refinery-0.6.6/refinery/units/meta/swap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/meta/transpose.py` & `binary-refinery-0.6.6/refinery/units/meta/transpose.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/meta/xfcc.py` & `binary-refinery-0.6.6/refinery/units/meta/xfcc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/misc/autoxor.py` & `binary-refinery-0.6.6/refinery/units/misc/autoxor.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/misc/couple.py` & `binary-refinery-0.6.6/refinery/units/misc/couple.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/misc/datefix.py` & `binary-refinery-0.6.6/refinery/units/misc/datefix.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/misc/drp.py` & `binary-refinery-0.6.6/refinery/units/misc/drp.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/misc/nop.py` & `binary-refinery-0.6.6/refinery/units/misc/nop.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/misc/urlfix.py` & `binary-refinery-0.6.6/refinery/units/misc/urlfix.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/misc/xkey.py` & `binary-refinery-0.6.6/refinery/units/misc/xkey.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/obfuscation/__init__.py` & `binary-refinery-0.6.6/refinery/units/obfuscation/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/obfuscation/js/arrays.py` & `binary-refinery-0.6.6/refinery/units/obfuscation/js/arrays.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/obfuscation/js/getattr.py` & `binary-refinery-0.6.6/refinery/units/obfuscation/js/getattr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/obfuscation/js/tuples.py` & `binary-refinery-0.6.6/refinery/units/obfuscation/js/tuples.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/obfuscation/ps1/__init__.py` & `binary-refinery-0.6.6/refinery/units/obfuscation/ps1/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/obfuscation/ps1/all.py` & `binary-refinery-0.6.6/refinery/units/obfuscation/ps1/all.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/obfuscation/ps1/brackets.py` & `binary-refinery-0.6.6/refinery/units/obfuscation/ps1/brackets.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/obfuscation/ps1/cases.py` & `binary-refinery-0.6.6/refinery/units/obfuscation/ps1/cases.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/obfuscation/ps1/concat.py` & `binary-refinery-0.6.6/refinery/units/obfuscation/ps1/concat.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/obfuscation/ps1/format.py` & `binary-refinery-0.6.6/refinery/units/obfuscation/ps1/format.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/obfuscation/ps1/invoke.py` & `binary-refinery-0.6.6/refinery/units/obfuscation/ps1/invoke.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/obfuscation/ps1/securestring.py` & `binary-refinery-0.6.6/refinery/units/obfuscation/ps1/securestring.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/obfuscation/ps1/stringreplace.py` & `binary-refinery-0.6.6/refinery/units/obfuscation/ps1/stringreplace.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/obfuscation/ps1/typecast.py` & `binary-refinery-0.6.6/refinery/units/obfuscation/ps1/typecast.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/obfuscation/ps1/uncurly.py` & `binary-refinery-0.6.6/refinery/units/obfuscation/ps1/uncurly.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/obfuscation/vba/all.py` & `binary-refinery-0.6.6/refinery/units/obfuscation/vba/all.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/obfuscation/vba/arithmetic.py` & `binary-refinery-0.6.6/refinery/units/obfuscation/vba/arithmetic.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/obfuscation/vba/brackets.py` & `binary-refinery-0.6.6/refinery/units/obfuscation/vba/brackets.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/obfuscation/vba/char.py` & `binary-refinery-0.6.6/refinery/units/obfuscation/vba/char.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/obfuscation/vba/concat.py` & `binary-refinery-0.6.6/refinery/units/obfuscation/vba/concat.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/obfuscation/vba/constants.py` & `binary-refinery-0.6.6/refinery/units/obfuscation/vba/constants.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/obfuscation/vba/dummies.py` & `binary-refinery-0.6.6/refinery/units/obfuscation/vba/dummies.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/obfuscation/vba/stringreplace.py` & `binary-refinery-0.6.6/refinery/units/obfuscation/vba/stringreplace.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/obfuscation/vba/stringreverse.py` & `binary-refinery-0.6.6/refinery/units/obfuscation/vba/stringreverse.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/pattern/__init__.py` & `binary-refinery-0.6.6/refinery/units/pattern/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/pattern/carve.py` & `binary-refinery-0.6.6/refinery/units/pattern/carve.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/pattern/carve_7z.py` & `binary-refinery-0.6.6/refinery/units/pattern/carve_7z.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/pattern/carve_json.py` & `binary-refinery-0.6.6/refinery/units/pattern/carve_json.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/pattern/carve_lnk.py` & `binary-refinery-0.6.6/refinery/units/pattern/carve_lnk.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/pattern/carve_pe.py` & `binary-refinery-0.6.6/refinery/units/pattern/carve_pe.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/pattern/carve_rtf.py` & `binary-refinery-0.6.6/refinery/units/pattern/carve_rtf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/pattern/carve_xml.py` & `binary-refinery-0.6.6/refinery/units/pattern/carve_xml.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,17 @@
         self.delta = {'/': -1, '?': 0}.get(self.mod, 1)
 
     def __repr__(self) -> str:
         return F'<{self.mod}{self.name}>'
 
 
 class XMLCarver:
-    _MAX_TAG_SIZE = 400
+    _MAX_TAG_SIZE = 0x8000
 
-    def __init__(self, data):
+    def __init__(self, data: bytearray):
         self.data = data
         self.cursor = 0
 
     def __iter__(self):
         return self
 
     def _try_decode(self, data: bytes) -> Optional[str]:
@@ -42,15 +42,15 @@
                 if printable(decoded): return decoded
         if len(data) % 2 == 1:
             data = data + B'\0'
         with suppress(UnicodeDecodeError):
             decoded = data.decode('UTF-16LE')
             if printable(decoded): return decoded
 
-    def _seek_tag(self, start):
+    def _seek_tag(self, start: int):
         quote = None
         escaped = False
         for end in range(start + 1, min(start + self._MAX_TAG_SIZE, len(self.data))):
             if not quote:
                 if self.data[end] == B'>'[0]:
                     return end + 1
                 elif self.data[end] == B'<'[0]:
@@ -75,15 +75,15 @@
             tag = XMLTag(decoded)
         except ValueError:
             return None
         else:
             self.cursor = end
             return tag
 
-    def _find_xml_end(self, tag):
+    def _find_xml_end(self, tag: XMLTag):
         stack = 1
         while stack:
             self.cursor = self.data.find(B'<', self.cursor)
             if self.cursor < 0:
                 return False
             t = self._read_tag()
             if t is None:
```

### Comparing `binary-refinery-0.6.5/refinery/units/pattern/carve_zip.py` & `binary-refinery-0.6.6/refinery/units/pattern/carve_zip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/pattern/defang.py` & `binary-refinery-0.6.6/refinery/units/pattern/defang.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/pattern/dnsdomain.py` & `binary-refinery-0.6.6/refinery/units/pattern/dnsdomain.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/pattern/mimewords.py` & `binary-refinery-0.6.6/refinery/units/pattern/mimewords.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/pattern/resplit.py` & `binary-refinery-0.6.6/refinery/units/pattern/resplit.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/pattern/resub.py` & `binary-refinery-0.6.6/refinery/units/pattern/resub.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/pattern/rex.py` & `binary-refinery-0.6.6/refinery/units/pattern/rex.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/pattern/struct_parser.py` & `binary-refinery-0.6.6/refinery/units/pattern/struct_parser.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/pattern/subfiles.py` & `binary-refinery-0.6.6/refinery/units/pattern/subfiles.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/pattern/urlguards.py` & `binary-refinery-0.6.6/refinery/units/pattern/urlguards.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/pattern/xtp.py` & `binary-refinery-0.6.6/refinery/units/pattern/xtp.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/pattern/xtw.py` & `binary-refinery-0.6.6/refinery/units/pattern/xtw.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/sinks/__init__.py` & `binary-refinery-0.6.6/refinery/units/sinks/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/sinks/asm.py` & `binary-refinery-0.6.6/refinery/units/sinks/asm.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/sinks/dump.py` & `binary-refinery-0.6.6/refinery/units/sinks/dump.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/sinks/iemap.py` & `binary-refinery-0.6.6/refinery/units/sinks/iemap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/sinks/peek.py` & `binary-refinery-0.6.6/refinery/units/sinks/peek.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/sinks/ppjscript.py` & `binary-refinery-0.6.6/refinery/units/sinks/ppjscript.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/sinks/ppjson.py` & `binary-refinery-0.6.6/refinery/units/sinks/ppjson.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/sinks/ppxml.py` & `binary-refinery-0.6.6/refinery/units/sinks/ppxml.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/strings/cfmt.py` & `binary-refinery-0.6.6/refinery/units/strings/cfmt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/strings/cswap.py` & `binary-refinery-0.6.6/refinery/units/strings/cswap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/strings/rep.py` & `binary-refinery-0.6.6/refinery/units/strings/rep.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/strings/repl.py` & `binary-refinery-0.6.6/refinery/units/strings/repl.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/strings/snip.py` & `binary-refinery-0.6.6/refinery/units/strings/snip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/strings/stretch.py` & `binary-refinery-0.6.6/refinery/units/strings/stretch.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/strings/termfit.py` & `binary-refinery-0.6.6/refinery/units/strings/termfit.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/refinery/units/strings/trim.py` & `binary-refinery-0.6.6/refinery/units/strings/trim.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.5/setup.py` & `binary-refinery-0.6.6/setup.py`

 * *Files identical despite different names*

