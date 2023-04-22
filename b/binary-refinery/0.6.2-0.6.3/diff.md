# Comparing `tmp/binary-refinery-0.6.2.tar.gz` & `tmp/binary-refinery-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/refinery/refinery/dist/.tmp-uvy8i5d_/binary-refinery-0.6.2.tar", last modified: Sat Apr 15 13:02:36 2023, max compression
+gzip compressed data, was "/home/runner/work/refinery/refinery/dist/.tmp-wywh22z2/binary-refinery-0.6.3.tar", last modified: Sat Apr 22 08:00:13 2023, max compression
```

## Comparing `binary-refinery-0.6.2.tar` & `binary-refinery-0.6.3.tar`

### file list

```diff
@@ -1,378 +1,379 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17604 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/binary_refinery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17604 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/binary_refinery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11708 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/binary_refinery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/binary_refinery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14980 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/binary_refinery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/binary_refinery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/binary_refinery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/
--rw-r--r--   0 runner    (1001) docker     (123)    14608 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/__init__.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/data/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49846 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/data/rich.json
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/explore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59012 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/argformats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/argparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/chunks.py
--rw-r--r--   0 runner    (1001) docker     (123)    16375 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/decompression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/deobfuscation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/dex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/lib/dotnet/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/dotnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/dotnet/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    30549 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/dotnet/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/dotnet/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/dotnet/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    19041 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/executable.py
--rw-r--r--   0 runner    (1001) docker     (123)    23050 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)    23540 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/java.py
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/magic.py
--rw-r--r--   0 runner    (1001) docker     (123)    34226 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/mime.py
--rw-r--r--   0 runner    (1001) docker     (123)     9966 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/mscrypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/murmur.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/lib/patterns/
--rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18566 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/patterns/tlds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/powershell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/ripemd128.py
--rw-r--r--   0 runner    (1001) docker     (123)    10358 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/serpent.py
--rw-r--r--   0 runner    (1001) docker     (123)    23138 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/suffixtree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/lib/thirdparty/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/thirdparty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   163388 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/thirdparty/acefile.py
--rw-r--r--   0 runner    (1001) docker     (123)    16823 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/thirdparty/batch_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)   127576 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/thirdparty/pcode2code.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/thirdparty/xxhash.py
--rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/vfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/
--rw-r--r--   0 runner    (1001) docker     (123)    69008 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/blockwise/
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/alu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/bitrev.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/byteswap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/map.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/neg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/pack.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/rev.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/rotl.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/rotr.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/shl.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/shr.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/sub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/terminate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/xor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/compression/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/ap.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/blz.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/bz2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/decompress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/jcalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/lz.py
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/lz4.py
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/lzf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/lzg.py
--rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/lzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/lzjb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/lznt1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/lzo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/mscf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/qlz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/szdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/zl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/
--rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/aes.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/blowfish.py
--rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/camellia.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/cast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/chacha.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/des.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/des3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/gost.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/hc128.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/isaac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/rabbit.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/rc2.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/rc4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/rc4mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/rc5.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/rc6.py
--rw-r--r--   0 runner    (1001) docker     (123)    48363 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/rijndael.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/rncrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/rot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9683 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/rsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/rsakey.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/salsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/seal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/secstr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/serpent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/tea.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/vigenere.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/xtea.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/xxtea.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/crypto/hash/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/hash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/hash/checksums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/hash/cryptographic.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/hash/imphash.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/hash/murmur.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/hash/password_hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/hash/xxhash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/crypto/keyderive/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/keyderive/CryptDeriveKey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/keyderive/DESDerive.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/keyderive/PasswordDeriveBytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/keyderive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/keyderive/hkdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/keyderive/hmac.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/keyderive/kblob.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/keyderive/pbkdf1.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/keyderive/pbkdf2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19518 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/keyderive/unixcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/encoding/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/atbash.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/b32.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/b58.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/b64.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/b85.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/cp1252.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/esc.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/hex.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/htmlesc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/netbios.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/ps1str.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/recode.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/u16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/url.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/uuenc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/wshenc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/formats/
--rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/a3x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/formats/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/archive/xt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/archive/xt7z.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/archive/xtace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/archive/xtasar.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/archive/xtcab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/archive/xtcpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/archive/xtiso.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/archive/xtiss.py
--rw-r--r--   0 runner    (1001) docker     (123)    46905 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/archive/xtnsis.py
--rw-r--r--   0 runner    (1001) docker     (123)    20487 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/archive/xtpyi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/archive/xttar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/archive/xtzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/bat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/deserialize_php.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/dexstr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/email.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/evtx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/formats/exe/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/exe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/exe/vaddr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/exe/vmemref.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/exe/vsect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/exe/vsnip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10787 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/exe/vstack.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/hexload.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/html.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/httpresponse.py
--rw-r--r--   0 runner    (1001) docker     (123)    30158 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/ifps.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/ifpsstr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/formats/java/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/java/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/java/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/java/jvdasm.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/java/jvstr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/msgpack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/formats/office/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/office/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/office/doctxt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/office/officecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/office/vbapc.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/office/vbastr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/office/xlmdeobf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/office/xlxtr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/office/xtdoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/office/xtone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/office/xtrtf.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/office/xtvba.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pcap_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/formats/pe/
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/dnblob.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/dncfx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/dnds.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/dnfields.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/dnhdr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/dnmr.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/dnrc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/dnstr.py
--rw-r--r--   0 runner    (1001) docker     (123)    30943 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pe/pemeta.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pe/peoverlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pe/perc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pe/pesig.py
--rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pe/pestrip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pkcs7.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pkcs7sig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/stego.py
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/winreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/malware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/malware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/malware/n40.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/meta/
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/chop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/cm.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/cull.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/dedup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/eat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/ef.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/emit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/groupby.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/iff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/iffp.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/iffs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/iffx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/max.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/min.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/mvc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/mvg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/pick.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/pop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/push.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/put.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/sep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/sorted.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/swap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/xfcc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/misc/autoxor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/misc/couple.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/misc/datefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/misc/drp.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/misc/nop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/misc/urlfix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/misc/xkey.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/obfuscation/
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/obfuscation/js/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/js/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/js/arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/js/getattr.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/js/tuples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/obfuscation/ps1/
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/ps1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/ps1/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/ps1/brackets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/ps1/cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/ps1/concat.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/ps1/escape.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/ps1/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/ps1/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/ps1/securestring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/ps1/stringreplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/ps1/typecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/ps1/uncurly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/obfuscation/vba/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/vba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/vba/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/vba/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/vba/brackets.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/vba/char.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/vba/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/vba/concat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/vba/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/vba/dummies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/vba/stringreplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/vba/stringreverse.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/vba/vba.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/pattern/
--rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/carve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/carve_7z.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/carve_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/carve_lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/carve_pe.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/carve_rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/carve_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/carve_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/defang.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/dnsdomain.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/mimewords.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/resplit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/resub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/rex.py
--rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/struct_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/subfiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/urlguards.py
--rw-r--r--   0 runner    (1001) docker     (123)    14161 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/xtp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/xtw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/sinks/
--rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/sinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/sinks/asm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/sinks/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/sinks/iemap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/sinks/peek.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/sinks/ppjscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/sinks/ppjson.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/sinks/ppxml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/strings/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/strings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/strings/cca.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/strings/ccp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/strings/cfmt.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/strings/clower.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/strings/cswap.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/strings/cupper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/strings/rep.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/strings/repl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/strings/snip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/strings/stretch.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/strings/termfit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/strings/trim.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17604 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/binary_refinery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17604 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/binary_refinery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11744 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/binary_refinery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/binary_refinery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15033 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/binary_refinery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/binary_refinery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/binary_refinery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/
+-rw-r--r--   0 runner    (1001) docker     (123)    14666 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/__init__.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49846 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/data/rich.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/explore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59012 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/argformats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/argparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/chunks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16375 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/decompression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/deobfuscation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/dex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/lib/dotnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/dotnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/dotnet/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30549 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/dotnet/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/dotnet/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/dotnet/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19041 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/executable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23050 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23540 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/java.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34226 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/mime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/mscrypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/murmur.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/lib/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)    16925 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18566 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/patterns/tlds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/powershell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/ripemd128.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10358 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/serpent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23138 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/suffixtree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/lib/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/thirdparty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   163388 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/thirdparty/acefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16823 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/thirdparty/batch_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127576 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/thirdparty/pcode2code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/thirdparty/xxhash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/vfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/
+-rw-r--r--   0 runner    (1001) docker     (123)    69083 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/blockwise/
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/alu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/bitrev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/byteswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/neg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/rev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/rotl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/rotr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/shl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/shr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/terminate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/xor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/compression/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/ap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/blz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/bz2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/decompress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/jcalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/lz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/lz4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/lzf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/lzg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/lzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/lzjb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/lznt1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/lzo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/mscf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/qlz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/szdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/zl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/
+-rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/blowfish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/camellia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/chacha.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/des.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/des3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/gost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/hc128.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/isaac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/rabbit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/rc2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/rc4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/rc4mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/rc5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/rc6.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48363 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/rijndael.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/rncrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/rot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/rsakey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/salsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/seal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/secstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/serpent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/tea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/vigenere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/xtea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/xxtea.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/crypto/hash/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/hash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/hash/checksums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/hash/cryptographic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/hash/imphash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/hash/murmur.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/hash/password_hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/hash/xxhash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/crypto/keyderive/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/keyderive/CryptDeriveKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/keyderive/DESDerive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/keyderive/PasswordDeriveBytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/keyderive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/keyderive/hkdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/keyderive/hmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/keyderive/kblob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/keyderive/pbkdf1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/keyderive/pbkdf2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19518 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/keyderive/unixcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/encoding/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/atbash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/b32.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/b58.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/b64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/b85.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/cp1252.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/esc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/htmlesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/netbios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/ps1str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/recode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/u16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/uuenc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/wshenc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/a3x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/formats/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/archive/xt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/archive/xt7z.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/archive/xtace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/archive/xtasar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/archive/xtcab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/archive/xtcpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/archive/xtiso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/archive/xtiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/archive/xtnode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46900 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/archive/xtnsis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20491 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/archive/xtpyi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/archive/xttar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/archive/xtzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/bat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/deserialize_php.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/dexstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/evtx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/formats/exe/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/exe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/exe/vaddr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/exe/vmemref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/exe/vsect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/exe/vsnip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10787 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/exe/vstack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/hexload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/httpresponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30158 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/ifps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/ifpsstr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/formats/java/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/java/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/java/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/java/jvdasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/java/jvstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/msgpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/formats/office/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/office/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/office/doctxt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/office/officecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/office/vbapc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/office/vbastr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/office/xlmdeobf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/office/xlxtr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/office/xtdoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/office/xtone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/office/xtrtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/office/xtvba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pcap_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/formats/pe/
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/dnblob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/dncfx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/dnds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/dnfields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/dnhdr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/dnmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/dnrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/dnstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30943 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pe/pemeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pe/peoverlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pe/perc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pe/pesig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pe/pestrip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pkcs7.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pkcs7sig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/stego.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/winreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/malware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/malware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/malware/n40.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/chop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/cm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/cull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/dedup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/eat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/ef.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/groupby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/iff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/iffp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/iffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/iffx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/min.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/mvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/mvg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/pick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/pop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/sep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/sorted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/swap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/xfcc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/misc/autoxor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/misc/couple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/misc/datefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/misc/drp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/misc/nop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/misc/urlfix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/misc/xkey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/obfuscation/
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/obfuscation/js/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/js/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/js/arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/js/getattr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/js/tuples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/obfuscation/ps1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/ps1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/ps1/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/ps1/brackets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/ps1/cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/ps1/concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/ps1/escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/ps1/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/ps1/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/ps1/securestring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/ps1/stringreplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/ps1/typecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/ps1/uncurly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/obfuscation/vba/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/vba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/vba/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/vba/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/vba/brackets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/vba/char.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/vba/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/vba/concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/vba/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/vba/dummies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/vba/stringreplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/vba/stringreverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/vba/vba.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/pattern/
+-rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/carve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/carve_7z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/carve_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/carve_lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/carve_pe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/carve_rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/carve_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/carve_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/defang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/dnsdomain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/mimewords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/resplit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/resub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/rex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/struct_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/subfiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/urlguards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14161 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/xtp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/xtw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/sinks/
+-rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/sinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/sinks/asm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/sinks/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/sinks/iemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/sinks/peek.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/sinks/ppjscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/sinks/ppjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/sinks/ppxml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/strings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/strings/cca.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/strings/ccp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/strings/cfmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/strings/clower.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/strings/cswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/strings/cupper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/strings/rep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/strings/repl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/strings/snip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/strings/stretch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/strings/termfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/strings/trim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/setup.py
```

### Comparing `binary-refinery-0.6.2/LICENSE` & `binary-refinery-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/PKG-INFO` & `binary-refinery-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binary-refinery
-Version: 0.6.2
+Version: 0.6.3
 Summary: A toolkit to transform and refine (mostly) binary data.
 Home-page: https://github.com/binref/refinery/
 Author: Jesko Huettenhain
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -21,15 +21,14 @@
 Provides-Extra: bitrev
 Provides-Extra: neg
 Provides-Extra: rotl
 Provides-Extra: rotr
 Provides-Extra: shl
 Provides-Extra: shr
 Provides-Extra: sub
-Provides-Extra: transpose
 Provides-Extra: xor
 Provides-Extra: chacha
 Provides-Extra: hc128
 Provides-Extra: isaac
 Provides-Extra: rabbit
 Provides-Extra: rc4mod
 Provides-Extra: salsa
@@ -39,14 +38,15 @@
 Provides-Extra: vmemref
 Provides-Extra: vstack
 Provides-Extra: vbapc
 Provides-Extra: vbastr
 Provides-Extra: xtrtf
 Provides-Extra: xtvba
 Provides-Extra: pcap
+Provides-Extra: transpose
 Provides-Extra: asm
 Provides-Extra: iemap
 Provides-Extra: peek
 Provides-Extra: ppjscript
 License-File: LICENSE
 
 # Binary Refinery
```

### Comparing `binary-refinery-0.6.2/README.md` & `binary-refinery-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/binary_refinery.egg-info/PKG-INFO` & `binary-refinery-0.6.3/binary_refinery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binary-refinery
-Version: 0.6.2
+Version: 0.6.3
 Summary: A toolkit to transform and refine (mostly) binary data.
 Home-page: https://github.com/binref/refinery/
 Author: Jesko Huettenhain
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -21,15 +21,14 @@
 Provides-Extra: bitrev
 Provides-Extra: neg
 Provides-Extra: rotl
 Provides-Extra: rotr
 Provides-Extra: shl
 Provides-Extra: shr
 Provides-Extra: sub
-Provides-Extra: transpose
 Provides-Extra: xor
 Provides-Extra: chacha
 Provides-Extra: hc128
 Provides-Extra: isaac
 Provides-Extra: rabbit
 Provides-Extra: rc4mod
 Provides-Extra: salsa
@@ -39,14 +38,15 @@
 Provides-Extra: vmemref
 Provides-Extra: vstack
 Provides-Extra: vbapc
 Provides-Extra: vbastr
 Provides-Extra: xtrtf
 Provides-Extra: xtvba
 Provides-Extra: pcap
+Provides-Extra: transpose
 Provides-Extra: asm
 Provides-Extra: iemap
 Provides-Extra: peek
 Provides-Extra: ppjscript
 License-File: LICENSE
 
 # Binary Refinery
```

### Comparing `binary-refinery-0.6.2/binary_refinery.egg-info/SOURCES.txt` & `binary-refinery-0.6.3/binary_refinery.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,14 @@
 refinery/units/blockwise/rev.py
 refinery/units/blockwise/rotl.py
 refinery/units/blockwise/rotr.py
 refinery/units/blockwise/shl.py
 refinery/units/blockwise/shr.py
 refinery/units/blockwise/sub.py
 refinery/units/blockwise/terminate.py
-refinery/units/blockwise/transpose.py
 refinery/units/blockwise/xor.py
 refinery/units/compression/__init__.py
 refinery/units/compression/ap.py
 refinery/units/compression/blz.py
 refinery/units/compression/bz2.py
 refinery/units/compression/decompress.py
 refinery/units/compression/jcalg.py
@@ -188,14 +187,15 @@
 refinery/units/formats/archive/xt7z.py
 refinery/units/formats/archive/xtace.py
 refinery/units/formats/archive/xtasar.py
 refinery/units/formats/archive/xtcab.py
 refinery/units/formats/archive/xtcpio.py
 refinery/units/formats/archive/xtiso.py
 refinery/units/formats/archive/xtiss.py
+refinery/units/formats/archive/xtnode.py
 refinery/units/formats/archive/xtnsis.py
 refinery/units/formats/archive/xtpyi.py
 refinery/units/formats/archive/xttar.py
 refinery/units/formats/archive/xtzip.py
 refinery/units/formats/exe/__init__.py
 refinery/units/formats/exe/vaddr.py
 refinery/units/formats/exe/vmemref.py
@@ -259,14 +259,15 @@
 refinery/units/meta/put.py
 refinery/units/meta/queue.py
 refinery/units/meta/reduce.py
 refinery/units/meta/scope.py
 refinery/units/meta/sep.py
 refinery/units/meta/sorted.py
 refinery/units/meta/swap.py
+refinery/units/meta/transpose.py
 refinery/units/meta/xfcc.py
 refinery/units/misc/__init__.py
 refinery/units/misc/autoxor.py
 refinery/units/misc/couple.py
 refinery/units/misc/datefix.py
 refinery/units/misc/drp.py
 refinery/units/misc/nop.py
```

### Comparing `binary-refinery-0.6.2/binary_refinery.egg-info/entry_points.txt` & `binary-refinery-0.6.3/binary_refinery.egg-info/entry_points.txt`

 * *Files 2% similar despite different names*

```diff
@@ -224,15 +224,15 @@
 sub = refinery.units.blockwise.sub:sub.run
 subfiles = refinery.units.pattern.subfiles:subfiles.run
 swap = refinery.units.meta.swap:swap.run
 szdd = refinery.units.compression.szdd:szdd.run
 tea = refinery.units.crypto.cipher.tea:tea.run
 termfit = refinery.units.strings.termfit:termfit.run
 terminate = refinery.units.blockwise.terminate:terminate.run
-transpose = refinery.units.blockwise.transpose:transpose.run
+transpose = refinery.units.meta.transpose:transpose.run
 trim = refinery.units.strings.trim:trim.run
 u16 = refinery.units.encoding.u16:u16.run
 ucrypt = refinery.units.crypto.keyderive.unixcrypt:ucrypt.run
 url = refinery.units.encoding.url:url.run
 urlfix = refinery.units.misc.urlfix:urlfix.run
 urlguards = refinery.units.pattern.urlguards:urlguards.run
 uuenc = refinery.units.encoding.uuenc:uuenc.run
@@ -262,14 +262,15 @@
 xtdoc = refinery.units.formats.office.xtdoc:xtdoc.run
 xtea = refinery.units.crypto.cipher.xtea:xtea.run
 xthtml = refinery.units.formats.html:xthtml.run
 xtiso = refinery.units.formats.archive.xtiso:xtiso.run
 xtiss = refinery.units.formats.archive.xtiss:xtiss.run
 xtjson = refinery.units.formats.json:xtjson.run
 xtmail = refinery.units.formats.email:xtmail.run
+xtnode = refinery.units.formats.archive.xtnode:xtnode.run
 xtnsis = refinery.units.formats.archive.xtnsis:xtnsis.run
 xtone = refinery.units.formats.office.xtone:xtone.run
 xtp = refinery.units.pattern.xtp:xtp.run
 xtpdf = refinery.units.formats.pdf:xtpdf.run
 xtpyi = refinery.units.formats.archive.xtpyi:xtpyi.run
 xtrtf = refinery.units.formats.office.xtrtf:xtrtf.run
 xttar = refinery.units.formats.archive.xttar:xttar.run
```

### Comparing `binary-refinery-0.6.2/binary_refinery.egg-info/requires.txt` & `binary-refinery-0.6.3/binary_refinery.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 colorama
 defusedxml
 macholib
 msgpack>=1.0.0
 pefile
-pycryptodome
+pycryptodomex
 pyelftools
 setuptools
 toml
 wheel
 python-magic
-pyperclip
-asn1crypto
-uncompyle6
-extract_msg
-xdis
+XLMMacroDeobfuscator
+phpserialize
 pycdlib
-msoffcrypto-tool
+xdis
 pyonenote
-Pillow
-phpserialize
-chardet
-olefile
-xlrd2
-capstone
-LnkParse3
 decompyle3
-python-registry
-javaobj-py3>=0.4.0.1
-pyxlsb2
 cabarchive
+pyperclip
+LnkParse3
+capstone
+xlrd2
+PyPDF2>=3.0.0
 openpyxl
+extract-msg
+asn1crypto
+chardet
 py7zr
-XLMMacroDeobfuscator
-PyPDF2>=3.0.0
+msoffcrypto-tool
+uncompyle6
+pyxlsb2
+olefile
+Pillow
+python-registry
+javaobj-py3>=0.4.0.1
 
 [add]
 numpy
 
 [all]
-capstone
-colorama
 angr
+colorama
 python-evtx
-chardet
 oletools
+jsbeautifier
+capstone
 numpy
 pypcapkit[scapy]<0.16.0
 intervaltree
+pyzipper
 unicorn
-jsbeautifier
+chardet
 
 [alu]
 numpy
 
 [asm]
 angr
 
@@ -136,8 +137,9 @@
 [xtrtf]
 oletools
 
 [xtvba]
 oletools
 
 [xtzip]
+pyzipper
 chardet
```

### Comparing `binary-refinery-0.6.2/refinery/__init__.pkl` & `binary-refinery-0.6.3/refinery/__init__.pkl`

 * *Files 3% similar despite different names*

```diff
@@ -35,322 +35,322 @@
 00000220: 7279 2e75 6e69 7473 2e62 6c6f 636b 7769  ry.units.blockwi
 00000230: 7365 2e73 6872 7118 5803 0000 0073 7562  se.shrq.X....sub
 00000240: 7119 581c 0000 0072 6566 696e 6572 792e  q.X....refinery.
 00000250: 756e 6974 732e 626c 6f63 6b77 6973 652e  units.blockwise.
 00000260: 7375 6271 1a58 0900 0000 7465 726d 696e  subq.X....termin
 00000270: 6174 6571 1b58 2200 0000 7265 6669 6e65  ateq.X"...refine
 00000280: 7279 2e75 6e69 7473 2e62 6c6f 636b 7769  ry.units.blockwi
-00000290: 7365 2e74 6572 6d69 6e61 7465 711c 5809  se.terminateq.X.
-000002a0: 0000 0074 7261 6e73 706f 7365 711d 5822  ...transposeq.X"
-000002b0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-000002c0: 732e 626c 6f63 6b77 6973 652e 7472 616e  s.blockwise.tran
-000002d0: 7370 6f73 6571 1e58 0300 0000 786f 7271  sposeq.X....xorq
-000002e0: 1f58 1c00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
-000002f0: 6e69 7473 2e62 6c6f 636b 7769 7365 2e78  nits.blockwise.x
-00000300: 6f72 7120 5805 0000 0061 706c 6962 7121  orq X....aplibq!
-00000310: 581d 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
-00000320: 6974 732e 636f 6d70 7265 7373 696f 6e2e  its.compression.
-00000330: 6170 7122 5803 0000 0062 6c7a 7123 581e  apq"X....blzq#X.
-00000340: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-00000350: 732e 636f 6d70 7265 7373 696f 6e2e 626c  s.compression.bl
-00000360: 7a71 2458 0300 0000 627a 3271 2558 1e00  zq$X....bz2q%X..
-00000370: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-00000380: 2e63 6f6d 7072 6573 7369 6f6e 2e62 7a32  .compression.bz2
-00000390: 7126 580a 0000 0064 6563 6f6d 7072 6573  q&X....decompres
-000003a0: 7371 2758 2500 0000 7265 6669 6e65 7279  sq'X%...refinery
-000003b0: 2e75 6e69 7473 2e63 6f6d 7072 6573 7369  .units.compressi
-000003c0: 6f6e 2e64 6563 6f6d 7072 6573 7371 2858  on.decompressq(X
-000003d0: 0500 0000 6a63 616c 6771 2958 2000 0000  ....jcalgq)X ...
-000003e0: 7265 6669 6e65 7279 2e75 6e69 7473 2e63  refinery.units.c
-000003f0: 6f6d 7072 6573 7369 6f6e 2e6a 6361 6c67  ompression.jcalg
-00000400: 712a 5804 0000 006c 7a6d 6171 2b58 1d00  q*X....lzmaq+X..
-00000410: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-00000420: 2e63 6f6d 7072 6573 7369 6f6e 2e6c 7a71  .compression.lzq
-00000430: 2c58 0300 0000 6c7a 3471 2d58 1e00 0000  ,X....lz4q-X....
-00000440: 7265 6669 6e65 7279 2e75 6e69 7473 2e63  refinery.units.c
-00000450: 6f6d 7072 6573 7369 6f6e 2e6c 7a34 712e  ompression.lz4q.
-00000460: 5803 0000 006c 7a66 712f 581e 0000 0072  X....lzfq/X....r
-00000470: 6566 696e 6572 792e 756e 6974 732e 636f  efinery.units.co
-00000480: 6d70 7265 7373 696f 6e2e 6c7a 6671 3058  mpression.lzfq0X
-00000490: 0300 0000 6c7a 6771 3158 1e00 0000 7265  ....lzgq1X....re
-000004a0: 6669 6e65 7279 2e75 6e69 7473 2e63 6f6d  finery.units.com
-000004b0: 7072 6573 7369 6f6e 2e6c 7a67 7132 5804  pression.lzgq2X.
-000004c0: 0000 006c 7a69 7071 3358 1f00 0000 7265  ...lzipq3X....re
-000004d0: 6669 6e65 7279 2e75 6e69 7473 2e63 6f6d  finery.units.com
-000004e0: 7072 6573 7369 6f6e 2e6c 7a69 7071 3458  pression.lzipq4X
-000004f0: 0400 0000 6c7a 6a62 7135 581f 0000 0072  ....lzjbq5X....r
-00000500: 6566 696e 6572 792e 756e 6974 732e 636f  efinery.units.co
-00000510: 6d70 7265 7373 696f 6e2e 6c7a 6a62 7136  mpression.lzjbq6
-00000520: 5805 0000 006c 7a6e 7431 7137 5820 0000  X....lznt1q7X ..
-00000530: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00000540: 636f 6d70 7265 7373 696f 6e2e 6c7a 6e74  compression.lznt
-00000550: 3171 3858 0300 0000 6c7a 6f71 3958 1e00  1q8X....lzoq9X..
-00000560: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-00000570: 2e63 6f6d 7072 6573 7369 6f6e 2e6c 7a6f  .compression.lzo
-00000580: 713a 5804 0000 006d 7363 6671 3b58 1f00  q:X....mscfq;X..
-00000590: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-000005a0: 2e63 6f6d 7072 6573 7369 6f6e 2e6d 7363  .compression.msc
-000005b0: 6671 3c58 0300 0000 716c 7a71 3d58 1e00  fq<X....qlzq=X..
-000005c0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-000005d0: 2e63 6f6d 7072 6573 7369 6f6e 2e71 6c7a  .compression.qlz
-000005e0: 713e 5804 0000 0073 7a64 6471 3f58 1f00  q>X....szddq?X..
-000005f0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-00000600: 2e63 6f6d 7072 6573 7369 6f6e 2e73 7a64  .compression.szd
-00000610: 6471 4058 0200 0000 7a6c 7141 581d 0000  dq@X....zlqAX...
-00000620: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00000630: 636f 6d70 7265 7373 696f 6e2e 7a6c 7142  compression.zlqB
-00000640: 5803 0000 0061 6573 7143 5820 0000 0072  X....aesqCX ...r
-00000650: 6566 696e 6572 792e 756e 6974 732e 6372  efinery.units.cr
-00000660: 7970 746f 2e63 6970 6865 722e 6165 7371  ypto.cipher.aesq
-00000670: 4458 0800 0000 626c 6f77 6669 7368 7145  DX....blowfishqE
-00000680: 5825 0000 0072 6566 696e 6572 792e 756e  X%...refinery.un
-00000690: 6974 732e 6372 7970 746f 2e63 6970 6865  its.crypto.ciphe
-000006a0: 722e 626c 6f77 6669 7368 7146 5808 0000  r.blowfishqFX...
-000006b0: 0063 616d 656c 6c69 6171 4758 2500 0000  .camelliaqGX%...
-000006c0: 7265 6669 6e65 7279 2e75 6e69 7473 2e63  refinery.units.c
-000006d0: 7279 7074 6f2e 6369 7068 6572 2e63 616d  rypto.cipher.cam
-000006e0: 656c 6c69 6171 4858 0400 0000 6361 7374  elliaqHX....cast
-000006f0: 7149 5821 0000 0072 6566 696e 6572 792e  qIX!...refinery.
-00000700: 756e 6974 732e 6372 7970 746f 2e63 6970  units.crypto.cip
-00000710: 6865 722e 6361 7374 714a 5806 0000 0063  her.castqJX....c
-00000720: 6861 6368 6171 4b58 2300 0000 7265 6669  hachaqKX#...refi
-00000730: 6e65 7279 2e75 6e69 7473 2e63 7279 7074  nery.units.crypt
-00000740: 6f2e 6369 7068 6572 2e63 6861 6368 6171  o.cipher.chachaq
-00000750: 4c58 0800 0000 6368 6163 6861 3230 714d  LX....chacha20qM
-00000760: 684c 5803 0000 0064 6573 714e 5820 0000  hLX....desqNX ..
-00000770: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00000780: 6372 7970 746f 2e63 6970 6865 722e 6465  crypto.cipher.de
-00000790: 7371 4f58 0400 0000 6465 7333 7150 5821  sqOX....des3qPX!
-000007a0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-000007b0: 732e 6372 7970 746f 2e63 6970 6865 722e  s.crypto.cipher.
-000007c0: 6465 7333 7151 5804 0000 0067 6f73 7471  des3qQX....gostq
-000007d0: 5258 2100 0000 7265 6669 6e65 7279 2e75  RX!...refinery.u
-000007e0: 6e69 7473 2e63 7279 7074 6f2e 6369 7068  nits.crypto.ciph
-000007f0: 6572 2e67 6f73 7471 5358 0500 0000 6863  er.gostqSX....hc
-00000800: 3132 3871 5458 2200 0000 7265 6669 6e65  128qTX"...refine
-00000810: 7279 2e75 6e69 7473 2e63 7279 7074 6f2e  ry.units.crypto.
-00000820: 6369 7068 6572 2e68 6331 3238 7155 5805  cipher.hc128qUX.
-00000830: 0000 0069 7361 6163 7156 5822 0000 0072  ...isaacqVX"...r
-00000840: 6566 696e 6572 792e 756e 6974 732e 6372  efinery.units.cr
-00000850: 7970 746f 2e63 6970 6865 722e 6973 6161  ypto.cipher.isaa
-00000860: 6371 5758 0600 0000 7261 6262 6974 7158  cqWX....rabbitqX
-00000870: 5823 0000 0072 6566 696e 6572 792e 756e  X#...refinery.un
-00000880: 6974 732e 6372 7970 746f 2e63 6970 6865  its.crypto.ciphe
-00000890: 722e 7261 6262 6974 7159 5803 0000 0072  r.rabbitqYX....r
-000008a0: 6332 715a 5820 0000 0072 6566 696e 6572  c2qZX ...refiner
-000008b0: 792e 756e 6974 732e 6372 7970 746f 2e63  y.units.crypto.c
-000008c0: 6970 6865 722e 7263 3271 5b58 0300 0000  ipher.rc2q[X....
-000008d0: 7263 3471 5c58 2000 0000 7265 6669 6e65  rc4q\X ...refine
-000008e0: 7279 2e75 6e69 7473 2e63 7279 7074 6f2e  ry.units.crypto.
-000008f0: 6369 7068 6572 2e72 6334 715d 5806 0000  cipher.rc4q]X...
-00000900: 0072 6334 6d6f 6471 5e58 2300 0000 7265  .rc4modq^X#...re
-00000910: 6669 6e65 7279 2e75 6e69 7473 2e63 7279  finery.units.cry
-00000920: 7074 6f2e 6369 7068 6572 2e72 6334 6d6f  pto.cipher.rc4mo
-00000930: 6471 5f58 0300 0000 7263 3571 6058 2000  dq_X....rc5q`X .
-00000940: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-00000950: 2e63 7279 7074 6f2e 6369 7068 6572 2e72  .crypto.cipher.r
-00000960: 6335 7161 5803 0000 0072 6336 7162 5820  c5qaX....rc6qbX 
-00000970: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-00000980: 732e 6372 7970 746f 2e63 6970 6865 722e  s.crypto.cipher.
-00000990: 7263 3671 6358 0800 0000 7269 6a6e 6461  rc6qcX....rijnda
-000009a0: 656c 7164 5825 0000 0072 6566 696e 6572  elqdX%...refiner
-000009b0: 792e 756e 6974 732e 6372 7970 746f 2e63  y.units.crypto.c
-000009c0: 6970 6865 722e 7269 6a6e 6461 656c 7165  ipher.rijndaelqe
-000009d0: 5807 0000 0072 6e63 7279 7074 7166 5824  X....rncryptqfX$
-000009e0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-000009f0: 732e 6372 7970 746f 2e63 6970 6865 722e  s.crypto.cipher.
-00000a00: 726e 6372 7970 7471 6758 0300 0000 726f  rncryptqgX....ro
-00000a10: 7471 6858 2000 0000 7265 6669 6e65 7279  tqhX ...refinery
-00000a20: 2e75 6e69 7473 2e63 7279 7074 6f2e 6369  .units.crypto.ci
-00000a30: 7068 6572 2e72 6f74 7169 5803 0000 0072  pher.rotqiX....r
-00000a40: 7361 716a 5820 0000 0072 6566 696e 6572  saqjX ...refiner
-00000a50: 792e 756e 6974 732e 6372 7970 746f 2e63  y.units.crypto.c
-00000a60: 6970 6865 722e 7273 6171 6b58 0600 0000  ipher.rsaqkX....
-00000a70: 7273 616b 6579 716c 5823 0000 0072 6566  rsakeyqlX#...ref
-00000a80: 696e 6572 792e 756e 6974 732e 6372 7970  inery.units.cryp
-00000a90: 746f 2e63 6970 6865 722e 7273 616b 6579  to.cipher.rsakey
-00000aa0: 716d 5805 0000 0073 616c 7361 716e 5822  qmX....salsaqnX"
-00000ab0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-00000ac0: 732e 6372 7970 746f 2e63 6970 6865 722e  s.crypto.cipher.
-00000ad0: 7361 6c73 6171 6f58 0700 0000 7361 6c73  salsaqoX....sals
-00000ae0: 6132 3071 7068 6f58 0400 0000 7365 616c  a20qphoX....seal
-00000af0: 7171 5821 0000 0072 6566 696e 6572 792e  qqX!...refinery.
-00000b00: 756e 6974 732e 6372 7970 746f 2e63 6970  units.crypto.cip
-00000b10: 6865 722e 7365 616c 7172 5806 0000 0073  her.sealqrX....s
-00000b20: 6563 7374 7271 7358 2300 0000 7265 6669  ecstrqsX#...refi
-00000b30: 6e65 7279 2e75 6e69 7473 2e63 7279 7074  nery.units.crypt
-00000b40: 6f2e 6369 7068 6572 2e73 6563 7374 7271  o.cipher.secstrq
-00000b50: 7458 0700 0000 7365 7270 656e 7471 7558  tX....serpentquX
-00000b60: 2400 0000 7265 6669 6e65 7279 2e75 6e69  $...refinery.uni
-00000b70: 7473 2e63 7279 7074 6f2e 6369 7068 6572  ts.crypto.cipher
-00000b80: 2e73 6572 7065 6e74 7176 5803 0000 0074  .serpentqvX....t
-00000b90: 6561 7177 5820 0000 0072 6566 696e 6572  eaqwX ...refiner
-00000ba0: 792e 756e 6974 732e 6372 7970 746f 2e63  y.units.crypto.c
-00000bb0: 6970 6865 722e 7465 6171 7858 0800 0000  ipher.teaqxX....
-00000bc0: 7669 6765 6e65 7265 7179 5825 0000 0072  vigenereqyX%...r
-00000bd0: 6566 696e 6572 792e 756e 6974 732e 6372  efinery.units.cr
-00000be0: 7970 746f 2e63 6970 6865 722e 7669 6765  ypto.cipher.vige
-00000bf0: 6e65 7265 717a 5804 0000 0078 7465 6171  nereqzX....xteaq
-00000c00: 7b58 2100 0000 7265 6669 6e65 7279 2e75  {X!...refinery.u
-00000c10: 6e69 7473 2e63 7279 7074 6f2e 6369 7068  nits.crypto.ciph
-00000c20: 6572 2e78 7465 6171 7c58 0500 0000 7878  er.xteaq|X....xx
-00000c30: 7465 6171 7d58 2200 0000 7265 6669 6e65  teaq}X"...refine
-00000c40: 7279 2e75 6e69 7473 2e63 7279 7074 6f2e  ry.units.crypto.
-00000c50: 6369 7068 6572 2e78 7874 6561 717e 5807  cipher.xxteaq~X.
-00000c60: 0000 0061 646c 6572 3332 717f 5824 0000  ...adler32q.X$..
-00000c70: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00000c80: 6372 7970 746f 2e68 6173 682e 6368 6563  crypto.hash.chec
-00000c90: 6b73 756d 7371 8058 0500 0000 6372 6333  ksumsq.X....crc3
-00000ca0: 3271 8168 8058 0600 0000 626c 6b32 3234  2q.h.X....blk224
-00000cb0: 7182 5828 0000 0072 6566 696e 6572 792e  q.X(...refinery.
-00000cc0: 756e 6974 732e 6372 7970 746f 2e68 6173  units.crypto.has
-00000cd0: 682e 6372 7970 746f 6772 6170 6869 6371  h.cryptographicq
-00000ce0: 8358 0600 0000 626c 6b32 3536 7184 6883  .X....blk256q.h.
-00000cf0: 5806 0000 0062 6c6b 3338 3471 8568 8358  X....blk384q.h.X
-00000d00: 0600 0000 626c 6b35 3132 7186 6883 5803  ....blk512q.h.X.
-00000d10: 0000 006d 6432 7187 6883 5803 0000 006d  ...md2q.h.X....m
-00000d20: 6434 7188 6883 5803 0000 006d 6435 7189  d4q.h.X....md5q.
-00000d30: 6883 5809 0000 0072 6970 656d 6431 3238  h.X....ripemd128
-00000d40: 718a 6883 5809 0000 0072 6970 656d 6431  q.h.X....ripemd1
-00000d50: 3630 718b 6883 5804 0000 0073 6861 3171  60q.h.X....sha1q
-00000d60: 8c68 8358 0600 0000 7368 6132 3234 718d  .h.X....sha224q.
-00000d70: 6883 5806 0000 0073 6861 3235 3671 8e68  h.X....sha256q.h
-00000d80: 8358 0600 0000 7368 6133 3834 718f 6883  .X....sha384q.h.
-00000d90: 5806 0000 0073 6861 3531 3271 9068 8358  X....sha512q.h.X
-00000da0: 0700 0000 696d 7068 6173 6871 9158 2200  ....imphashq.X".
+00000290: 7365 2e74 6572 6d69 6e61 7465 711c 5803  se.terminateq.X.
+000002a0: 0000 0078 6f72 711d 581c 0000 0072 6566  ...xorq.X....ref
+000002b0: 696e 6572 792e 756e 6974 732e 626c 6f63  inery.units.bloc
+000002c0: 6b77 6973 652e 786f 7271 1e58 0500 0000  kwise.xorq.X....
+000002d0: 6170 6c69 6271 1f58 1d00 0000 7265 6669  aplibq.X....refi
+000002e0: 6e65 7279 2e75 6e69 7473 2e63 6f6d 7072  nery.units.compr
+000002f0: 6573 7369 6f6e 2e61 7071 2058 0300 0000  ession.apq X....
+00000300: 626c 7a71 2158 1e00 0000 7265 6669 6e65  blzq!X....refine
+00000310: 7279 2e75 6e69 7473 2e63 6f6d 7072 6573  ry.units.compres
+00000320: 7369 6f6e 2e62 6c7a 7122 5803 0000 0062  sion.blzq"X....b
+00000330: 7a32 7123 581e 0000 0072 6566 696e 6572  z2q#X....refiner
+00000340: 792e 756e 6974 732e 636f 6d70 7265 7373  y.units.compress
+00000350: 696f 6e2e 627a 3271 2458 0a00 0000 6465  ion.bz2q$X....de
+00000360: 636f 6d70 7265 7373 7125 5825 0000 0072  compressq%X%...r
+00000370: 6566 696e 6572 792e 756e 6974 732e 636f  efinery.units.co
+00000380: 6d70 7265 7373 696f 6e2e 6465 636f 6d70  mpression.decomp
+00000390: 7265 7373 7126 5805 0000 006a 6361 6c67  ressq&X....jcalg
+000003a0: 7127 5820 0000 0072 6566 696e 6572 792e  q'X ...refinery.
+000003b0: 756e 6974 732e 636f 6d70 7265 7373 696f  units.compressio
+000003c0: 6e2e 6a63 616c 6771 2858 0400 0000 6c7a  n.jcalgq(X....lz
+000003d0: 6d61 7129 581d 0000 0072 6566 696e 6572  maq)X....refiner
+000003e0: 792e 756e 6974 732e 636f 6d70 7265 7373  y.units.compress
+000003f0: 696f 6e2e 6c7a 712a 5803 0000 006c 7a34  ion.lzq*X....lz4
+00000400: 712b 581e 0000 0072 6566 696e 6572 792e  q+X....refinery.
+00000410: 756e 6974 732e 636f 6d70 7265 7373 696f  units.compressio
+00000420: 6e2e 6c7a 3471 2c58 0300 0000 6c7a 6671  n.lz4q,X....lzfq
+00000430: 2d58 1e00 0000 7265 6669 6e65 7279 2e75  -X....refinery.u
+00000440: 6e69 7473 2e63 6f6d 7072 6573 7369 6f6e  nits.compression
+00000450: 2e6c 7a66 712e 5803 0000 006c 7a67 712f  .lzfq.X....lzgq/
+00000460: 581e 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
+00000470: 6974 732e 636f 6d70 7265 7373 696f 6e2e  its.compression.
+00000480: 6c7a 6771 3058 0400 0000 6c7a 6970 7131  lzgq0X....lzipq1
+00000490: 581f 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
+000004a0: 6974 732e 636f 6d70 7265 7373 696f 6e2e  its.compression.
+000004b0: 6c7a 6970 7132 5804 0000 006c 7a6a 6271  lzipq2X....lzjbq
+000004c0: 3358 1f00 0000 7265 6669 6e65 7279 2e75  3X....refinery.u
+000004d0: 6e69 7473 2e63 6f6d 7072 6573 7369 6f6e  nits.compression
+000004e0: 2e6c 7a6a 6271 3458 0500 0000 6c7a 6e74  .lzjbq4X....lznt
+000004f0: 3171 3558 2000 0000 7265 6669 6e65 7279  1q5X ...refinery
+00000500: 2e75 6e69 7473 2e63 6f6d 7072 6573 7369  .units.compressi
+00000510: 6f6e 2e6c 7a6e 7431 7136 5803 0000 006c  on.lznt1q6X....l
+00000520: 7a6f 7137 581e 0000 0072 6566 696e 6572  zoq7X....refiner
+00000530: 792e 756e 6974 732e 636f 6d70 7265 7373  y.units.compress
+00000540: 696f 6e2e 6c7a 6f71 3858 0400 0000 6d73  ion.lzoq8X....ms
+00000550: 6366 7139 581f 0000 0072 6566 696e 6572  cfq9X....refiner
+00000560: 792e 756e 6974 732e 636f 6d70 7265 7373  y.units.compress
+00000570: 696f 6e2e 6d73 6366 713a 5803 0000 0071  ion.mscfq:X....q
+00000580: 6c7a 713b 581e 0000 0072 6566 696e 6572  lzq;X....refiner
+00000590: 792e 756e 6974 732e 636f 6d70 7265 7373  y.units.compress
+000005a0: 696f 6e2e 716c 7a71 3c58 0400 0000 737a  ion.qlzq<X....sz
+000005b0: 6464 713d 581f 0000 0072 6566 696e 6572  ddq=X....refiner
+000005c0: 792e 756e 6974 732e 636f 6d70 7265 7373  y.units.compress
+000005d0: 696f 6e2e 737a 6464 713e 5802 0000 007a  ion.szddq>X....z
+000005e0: 6c71 3f58 1d00 0000 7265 6669 6e65 7279  lq?X....refinery
+000005f0: 2e75 6e69 7473 2e63 6f6d 7072 6573 7369  .units.compressi
+00000600: 6f6e 2e7a 6c71 4058 0300 0000 6165 7371  on.zlq@X....aesq
+00000610: 4158 2000 0000 7265 6669 6e65 7279 2e75  AX ...refinery.u
+00000620: 6e69 7473 2e63 7279 7074 6f2e 6369 7068  nits.crypto.ciph
+00000630: 6572 2e61 6573 7142 5808 0000 0062 6c6f  er.aesqBX....blo
+00000640: 7766 6973 6871 4358 2500 0000 7265 6669  wfishqCX%...refi
+00000650: 6e65 7279 2e75 6e69 7473 2e63 7279 7074  nery.units.crypt
+00000660: 6f2e 6369 7068 6572 2e62 6c6f 7766 6973  o.cipher.blowfis
+00000670: 6871 4458 0800 0000 6361 6d65 6c6c 6961  hqDX....camellia
+00000680: 7145 5825 0000 0072 6566 696e 6572 792e  qEX%...refinery.
+00000690: 756e 6974 732e 6372 7970 746f 2e63 6970  units.crypto.cip
+000006a0: 6865 722e 6361 6d65 6c6c 6961 7146 5804  her.camelliaqFX.
+000006b0: 0000 0063 6173 7471 4758 2100 0000 7265  ...castqGX!...re
+000006c0: 6669 6e65 7279 2e75 6e69 7473 2e63 7279  finery.units.cry
+000006d0: 7074 6f2e 6369 7068 6572 2e63 6173 7471  pto.cipher.castq
+000006e0: 4858 0600 0000 6368 6163 6861 7149 5823  HX....chachaqIX#
+000006f0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00000700: 732e 6372 7970 746f 2e63 6970 6865 722e  s.crypto.cipher.
+00000710: 6368 6163 6861 714a 5808 0000 0063 6861  chachaqJX....cha
+00000720: 6368 6132 3071 4b68 4a58 0300 0000 6465  cha20qKhJX....de
+00000730: 7371 4c58 2000 0000 7265 6669 6e65 7279  sqLX ...refinery
+00000740: 2e75 6e69 7473 2e63 7279 7074 6f2e 6369  .units.crypto.ci
+00000750: 7068 6572 2e64 6573 714d 5804 0000 0064  pher.desqMX....d
+00000760: 6573 3371 4e58 2100 0000 7265 6669 6e65  es3qNX!...refine
+00000770: 7279 2e75 6e69 7473 2e63 7279 7074 6f2e  ry.units.crypto.
+00000780: 6369 7068 6572 2e64 6573 3371 4f58 0400  cipher.des3qOX..
+00000790: 0000 676f 7374 7150 5821 0000 0072 6566  ..gostqPX!...ref
+000007a0: 696e 6572 792e 756e 6974 732e 6372 7970  inery.units.cryp
+000007b0: 746f 2e63 6970 6865 722e 676f 7374 7151  to.cipher.gostqQ
+000007c0: 5805 0000 0068 6331 3238 7152 5822 0000  X....hc128qRX"..
+000007d0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+000007e0: 6372 7970 746f 2e63 6970 6865 722e 6863  crypto.cipher.hc
+000007f0: 3132 3871 5358 0500 0000 6973 6161 6371  128qSX....isaacq
+00000800: 5458 2200 0000 7265 6669 6e65 7279 2e75  TX"...refinery.u
+00000810: 6e69 7473 2e63 7279 7074 6f2e 6369 7068  nits.crypto.ciph
+00000820: 6572 2e69 7361 6163 7155 5806 0000 0072  er.isaacqUX....r
+00000830: 6162 6269 7471 5658 2300 0000 7265 6669  abbitqVX#...refi
+00000840: 6e65 7279 2e75 6e69 7473 2e63 7279 7074  nery.units.crypt
+00000850: 6f2e 6369 7068 6572 2e72 6162 6269 7471  o.cipher.rabbitq
+00000860: 5758 0300 0000 7263 3271 5858 2000 0000  WX....rc2qXX ...
+00000870: 7265 6669 6e65 7279 2e75 6e69 7473 2e63  refinery.units.c
+00000880: 7279 7074 6f2e 6369 7068 6572 2e72 6332  rypto.cipher.rc2
+00000890: 7159 5803 0000 0072 6334 715a 5820 0000  qYX....rc4qZX ..
+000008a0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+000008b0: 6372 7970 746f 2e63 6970 6865 722e 7263  crypto.cipher.rc
+000008c0: 3471 5b58 0600 0000 7263 346d 6f64 715c  4q[X....rc4modq\
+000008d0: 5823 0000 0072 6566 696e 6572 792e 756e  X#...refinery.un
+000008e0: 6974 732e 6372 7970 746f 2e63 6970 6865  its.crypto.ciphe
+000008f0: 722e 7263 346d 6f64 715d 5803 0000 0072  r.rc4modq]X....r
+00000900: 6335 715e 5820 0000 0072 6566 696e 6572  c5q^X ...refiner
+00000910: 792e 756e 6974 732e 6372 7970 746f 2e63  y.units.crypto.c
+00000920: 6970 6865 722e 7263 3571 5f58 0300 0000  ipher.rc5q_X....
+00000930: 7263 3671 6058 2000 0000 7265 6669 6e65  rc6q`X ...refine
+00000940: 7279 2e75 6e69 7473 2e63 7279 7074 6f2e  ry.units.crypto.
+00000950: 6369 7068 6572 2e72 6336 7161 5808 0000  cipher.rc6qaX...
+00000960: 0072 696a 6e64 6165 6c71 6258 2500 0000  .rijndaelqbX%...
+00000970: 7265 6669 6e65 7279 2e75 6e69 7473 2e63  refinery.units.c
+00000980: 7279 7074 6f2e 6369 7068 6572 2e72 696a  rypto.cipher.rij
+00000990: 6e64 6165 6c71 6358 0700 0000 726e 6372  ndaelqcX....rncr
+000009a0: 7970 7471 6458 2400 0000 7265 6669 6e65  yptqdX$...refine
+000009b0: 7279 2e75 6e69 7473 2e63 7279 7074 6f2e  ry.units.crypto.
+000009c0: 6369 7068 6572 2e72 6e63 7279 7074 7165  cipher.rncryptqe
+000009d0: 5803 0000 0072 6f74 7166 5820 0000 0072  X....rotqfX ...r
+000009e0: 6566 696e 6572 792e 756e 6974 732e 6372  efinery.units.cr
+000009f0: 7970 746f 2e63 6970 6865 722e 726f 7471  ypto.cipher.rotq
+00000a00: 6758 0300 0000 7273 6171 6858 2000 0000  gX....rsaqhX ...
+00000a10: 7265 6669 6e65 7279 2e75 6e69 7473 2e63  refinery.units.c
+00000a20: 7279 7074 6f2e 6369 7068 6572 2e72 7361  rypto.cipher.rsa
+00000a30: 7169 5806 0000 0072 7361 6b65 7971 6a58  qiX....rsakeyqjX
+00000a40: 2300 0000 7265 6669 6e65 7279 2e75 6e69  #...refinery.uni
+00000a50: 7473 2e63 7279 7074 6f2e 6369 7068 6572  ts.crypto.cipher
+00000a60: 2e72 7361 6b65 7971 6b58 0500 0000 7361  .rsakeyqkX....sa
+00000a70: 6c73 6171 6c58 2200 0000 7265 6669 6e65  lsaqlX"...refine
+00000a80: 7279 2e75 6e69 7473 2e63 7279 7074 6f2e  ry.units.crypto.
+00000a90: 6369 7068 6572 2e73 616c 7361 716d 5807  cipher.salsaqmX.
+00000aa0: 0000 0073 616c 7361 3230 716e 686d 5804  ...salsa20qnhmX.
+00000ab0: 0000 0073 6561 6c71 6f58 2100 0000 7265  ...sealqoX!...re
+00000ac0: 6669 6e65 7279 2e75 6e69 7473 2e63 7279  finery.units.cry
+00000ad0: 7074 6f2e 6369 7068 6572 2e73 6561 6c71  pto.cipher.sealq
+00000ae0: 7058 0600 0000 7365 6373 7472 7171 5823  pX....secstrqqX#
+00000af0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00000b00: 732e 6372 7970 746f 2e63 6970 6865 722e  s.crypto.cipher.
+00000b10: 7365 6373 7472 7172 5807 0000 0073 6572  secstrqrX....ser
+00000b20: 7065 6e74 7173 5824 0000 0072 6566 696e  pentqsX$...refin
+00000b30: 6572 792e 756e 6974 732e 6372 7970 746f  ery.units.crypto
+00000b40: 2e63 6970 6865 722e 7365 7270 656e 7471  .cipher.serpentq
+00000b50: 7458 0300 0000 7465 6171 7558 2000 0000  tX....teaquX ...
+00000b60: 7265 6669 6e65 7279 2e75 6e69 7473 2e63  refinery.units.c
+00000b70: 7279 7074 6f2e 6369 7068 6572 2e74 6561  rypto.cipher.tea
+00000b80: 7176 5808 0000 0076 6967 656e 6572 6571  qvX....vigenereq
+00000b90: 7758 2500 0000 7265 6669 6e65 7279 2e75  wX%...refinery.u
+00000ba0: 6e69 7473 2e63 7279 7074 6f2e 6369 7068  nits.crypto.ciph
+00000bb0: 6572 2e76 6967 656e 6572 6571 7858 0400  er.vigenereqxX..
+00000bc0: 0000 7874 6561 7179 5821 0000 0072 6566  ..xteaqyX!...ref
+00000bd0: 696e 6572 792e 756e 6974 732e 6372 7970  inery.units.cryp
+00000be0: 746f 2e63 6970 6865 722e 7874 6561 717a  to.cipher.xteaqz
+00000bf0: 5805 0000 0078 7874 6561 717b 5822 0000  X....xxteaq{X"..
+00000c00: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00000c10: 6372 7970 746f 2e63 6970 6865 722e 7878  crypto.cipher.xx
+00000c20: 7465 6171 7c58 0700 0000 6164 6c65 7233  teaq|X....adler3
+00000c30: 3271 7d58 2400 0000 7265 6669 6e65 7279  2q}X$...refinery
+00000c40: 2e75 6e69 7473 2e63 7279 7074 6f2e 6861  .units.crypto.ha
+00000c50: 7368 2e63 6865 636b 7375 6d73 717e 5805  sh.checksumsq~X.
+00000c60: 0000 0063 7263 3332 717f 687e 5806 0000  ...crc32q.h~X...
+00000c70: 0062 6c6b 3232 3471 8058 2800 0000 7265  .blk224q.X(...re
+00000c80: 6669 6e65 7279 2e75 6e69 7473 2e63 7279  finery.units.cry
+00000c90: 7074 6f2e 6861 7368 2e63 7279 7074 6f67  pto.hash.cryptog
+00000ca0: 7261 7068 6963 7181 5806 0000 0062 6c6b  raphicq.X....blk
+00000cb0: 3235 3671 8268 8158 0600 0000 626c 6b33  256q.h.X....blk3
+00000cc0: 3834 7183 6881 5806 0000 0062 6c6b 3531  84q.h.X....blk51
+00000cd0: 3271 8468 8158 0300 0000 6d64 3271 8568  2q.h.X....md2q.h
+00000ce0: 8158 0300 0000 6d64 3471 8668 8158 0300  .X....md4q.h.X..
+00000cf0: 0000 6d64 3571 8768 8158 0900 0000 7269  ..md5q.h.X....ri
+00000d00: 7065 6d64 3132 3871 8868 8158 0900 0000  pemd128q.h.X....
+00000d10: 7269 7065 6d64 3136 3071 8968 8158 0400  ripemd160q.h.X..
+00000d20: 0000 7368 6131 718a 6881 5806 0000 0073  ..sha1q.h.X....s
+00000d30: 6861 3232 3471 8b68 8158 0600 0000 7368  ha224q.h.X....sh
+00000d40: 6132 3536 718c 6881 5806 0000 0073 6861  a256q.h.X....sha
+00000d50: 3338 3471 8d68 8158 0600 0000 7368 6135  384q.h.X....sha5
+00000d60: 3132 718e 6881 5807 0000 0069 6d70 6861  12q.h.X....impha
+00000d70: 7368 718f 5822 0000 0072 6566 696e 6572  shq.X"...refiner
+00000d80: 792e 756e 6974 732e 6372 7970 746f 2e68  y.units.crypto.h
+00000d90: 6173 682e 696d 7068 6173 6871 9058 0900  ash.imphashq.X..
+00000da0: 0000 6d6d 6831 3238 7833 3271 9158 2100  ..mmh128x32q.X!.
 00000db0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-00000dc0: 2e63 7279 7074 6f2e 6861 7368 2e69 6d70  .crypto.hash.imp
-00000dd0: 6861 7368 7192 5809 0000 006d 6d68 3132  hashq.X....mmh12
-00000de0: 3878 3332 7193 5821 0000 0072 6566 696e  8x32q.X!...refin
-00000df0: 6572 792e 756e 6974 732e 6372 7970 746f  ery.units.crypto
-00000e00: 2e68 6173 682e 6d75 726d 7572 7194 5809  .hash.murmurq.X.
-00000e10: 0000 006d 6d68 3132 3878 3634 7195 6894  ...mmh128x64q.h.
-00000e20: 5805 0000 006d 6d68 3332 7196 6894 5804  X....mmh32q.h.X.
-00000e30: 0000 006e 746c 6d71 9758 2a00 0000 7265  ...ntlmq.X*...re
-00000e40: 6669 6e65 7279 2e75 6e69 7473 2e63 7279  finery.units.cry
-00000e50: 7074 6f2e 6861 7368 2e70 6173 7377 6f72  pto.hash.passwor
-00000e60: 645f 6861 7368 6573 7198 5803 0000 0078  d_hashesq.X....x
-00000e70: 7868 7199 5821 0000 0072 6566 696e 6572  xhq.X!...refiner
-00000e80: 792e 756e 6974 732e 6372 7970 746f 2e68  y.units.crypto.h
-00000e90: 6173 682e 7878 6861 7368 719a 580e 0000  ash.xxhashq.X...
-00000ea0: 0043 7279 7074 4465 7269 7665 4b65 7971  .CryptDeriveKeyq
-00000eb0: 9b58 2e00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
-00000ec0: 6e69 7473 2e63 7279 7074 6f2e 6b65 7964  nits.crypto.keyd
-00000ed0: 6572 6976 652e 4372 7970 7444 6572 6976  erive.CryptDeriv
-00000ee0: 654b 6579 719c 5809 0000 0044 4553 4465  eKeyq.X....DESDe
-00000ef0: 7269 7665 719d 5829 0000 0072 6566 696e  riveq.X)...refin
-00000f00: 6572 792e 756e 6974 732e 6372 7970 746f  ery.units.crypto
-00000f10: 2e6b 6579 6465 7269 7665 2e44 4553 4465  .keyderive.DESDe
-00000f20: 7269 7665 719e 5813 0000 0050 6173 7377  riveq.X....Passw
-00000f30: 6f72 6444 6572 6976 6542 7974 6573 719f  ordDeriveBytesq.
-00000f40: 5833 0000 0072 6566 696e 6572 792e 756e  X3...refinery.un
-00000f50: 6974 732e 6372 7970 746f 2e6b 6579 6465  its.crypto.keyde
-00000f60: 7269 7665 2e50 6173 7377 6f72 6444 6572  rive.PasswordDer
-00000f70: 6976 6542 7974 6573 71a0 5804 0000 0048  iveBytesq.X....H
-00000f80: 4b44 4671 a158 2400 0000 7265 6669 6e65  KDFq.X$...refine
-00000f90: 7279 2e75 6e69 7473 2e63 7279 7074 6f2e  ry.units.crypto.
-00000fa0: 6b65 7964 6572 6976 652e 686b 6466 71a2  keyderive.hkdfq.
-00000fb0: 5804 0000 0068 6d61 6371 a358 2400 0000  X....hmacq.X$...
-00000fc0: 7265 6669 6e65 7279 2e75 6e69 7473 2e63  refinery.units.c
-00000fd0: 7279 7074 6f2e 6b65 7964 6572 6976 652e  rypto.keyderive.
-00000fe0: 686d 6163 71a4 5805 0000 006b 626c 6f62  hmacq.X....kblob
-00000ff0: 71a5 5825 0000 0072 6566 696e 6572 792e  q.X%...refinery.
+00000dc0: 2e63 7279 7074 6f2e 6861 7368 2e6d 7572  .crypto.hash.mur
+00000dd0: 6d75 7271 9258 0900 0000 6d6d 6831 3238  murq.X....mmh128
+00000de0: 7836 3471 9368 9258 0500 0000 6d6d 6833  x64q.h.X....mmh3
+00000df0: 3271 9468 9258 0400 0000 6e74 6c6d 7195  2q.h.X....ntlmq.
+00000e00: 582a 0000 0072 6566 696e 6572 792e 756e  X*...refinery.un
+00000e10: 6974 732e 6372 7970 746f 2e68 6173 682e  its.crypto.hash.
+00000e20: 7061 7373 776f 7264 5f68 6173 6865 7371  password_hashesq
+00000e30: 9658 0300 0000 7878 6871 9758 2100 0000  .X....xxhq.X!...
+00000e40: 7265 6669 6e65 7279 2e75 6e69 7473 2e63  refinery.units.c
+00000e50: 7279 7074 6f2e 6861 7368 2e78 7868 6173  rypto.hash.xxhas
+00000e60: 6871 9858 0e00 0000 4372 7970 7444 6572  hq.X....CryptDer
+00000e70: 6976 654b 6579 7199 582e 0000 0072 6566  iveKeyq.X....ref
+00000e80: 696e 6572 792e 756e 6974 732e 6372 7970  inery.units.cryp
+00000e90: 746f 2e6b 6579 6465 7269 7665 2e43 7279  to.keyderive.Cry
+00000ea0: 7074 4465 7269 7665 4b65 7971 9a58 0900  ptDeriveKeyq.X..
+00000eb0: 0000 4445 5344 6572 6976 6571 9b58 2900  ..DESDeriveq.X).
+00000ec0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+00000ed0: 2e63 7279 7074 6f2e 6b65 7964 6572 6976  .crypto.keyderiv
+00000ee0: 652e 4445 5344 6572 6976 6571 9c58 1300  e.DESDeriveq.X..
+00000ef0: 0000 5061 7373 776f 7264 4465 7269 7665  ..PasswordDerive
+00000f00: 4279 7465 7371 9d58 3300 0000 7265 6669  Bytesq.X3...refi
+00000f10: 6e65 7279 2e75 6e69 7473 2e63 7279 7074  nery.units.crypt
+00000f20: 6f2e 6b65 7964 6572 6976 652e 5061 7373  o.keyderive.Pass
+00000f30: 776f 7264 4465 7269 7665 4279 7465 7371  wordDeriveBytesq
+00000f40: 9e58 0400 0000 484b 4446 719f 5824 0000  .X....HKDFq.X$..
+00000f50: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00000f60: 6372 7970 746f 2e6b 6579 6465 7269 7665  crypto.keyderive
+00000f70: 2e68 6b64 6671 a058 0400 0000 686d 6163  .hkdfq.X....hmac
+00000f80: 71a1 5824 0000 0072 6566 696e 6572 792e  q.X$...refinery.
+00000f90: 756e 6974 732e 6372 7970 746f 2e6b 6579  units.crypto.key
+00000fa0: 6465 7269 7665 2e68 6d61 6371 a258 0500  derive.hmacq.X..
+00000fb0: 0000 6b62 6c6f 6271 a358 2500 0000 7265  ..kblobq.X%...re
+00000fc0: 6669 6e65 7279 2e75 6e69 7473 2e63 7279  finery.units.cry
+00000fd0: 7074 6f2e 6b65 7964 6572 6976 652e 6b62  pto.keyderive.kb
+00000fe0: 6c6f 6271 a458 0600 0000 7062 6b64 6631  lobq.X....pbkdf1
+00000ff0: 71a5 5826 0000 0072 6566 696e 6572 792e  q.X&...refinery.
 00001000: 756e 6974 732e 6372 7970 746f 2e6b 6579  units.crypto.key
-00001010: 6465 7269 7665 2e6b 626c 6f62 71a6 5806  derive.kblobq.X.
-00001020: 0000 0070 626b 6466 3171 a758 2600 0000  ...pbkdf1q.X&...
-00001030: 7265 6669 6e65 7279 2e75 6e69 7473 2e63  refinery.units.c
-00001040: 7279 7074 6f2e 6b65 7964 6572 6976 652e  rypto.keyderive.
-00001050: 7062 6b64 6631 71a8 5806 0000 0070 626b  pbkdf1q.X....pbk
-00001060: 6466 3271 a958 2600 0000 7265 6669 6e65  df2q.X&...refine
-00001070: 7279 2e75 6e69 7473 2e63 7279 7074 6f2e  ry.units.crypto.
-00001080: 6b65 7964 6572 6976 652e 7062 6b64 6632  keyderive.pbkdf2
-00001090: 71aa 5806 0000 0075 6372 7970 7471 ab58  q.X....ucryptq.X
-000010a0: 2900 0000 7265 6669 6e65 7279 2e75 6e69  )...refinery.uni
-000010b0: 7473 2e63 7279 7074 6f2e 6b65 7964 6572  ts.crypto.keyder
-000010c0: 6976 652e 756e 6978 6372 7970 7471 ac58  ive.unixcryptq.X
-000010d0: 0600 0000 6174 6261 7368 71ad 581e 0000  ....atbashq.X...
-000010e0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-000010f0: 656e 636f 6469 6e67 2e61 7462 6173 6871  encoding.atbashq
-00001100: ae58 0300 0000 6233 3271 af58 1b00 0000  .X....b32q.X....
-00001110: 7265 6669 6e65 7279 2e75 6e69 7473 2e65  refinery.units.e
-00001120: 6e63 6f64 696e 672e 6233 3271 b058 0300  ncoding.b32q.X..
-00001130: 0000 6235 3871 b158 1b00 0000 7265 6669  ..b58q.X....refi
-00001140: 6e65 7279 2e75 6e69 7473 2e65 6e63 6f64  nery.units.encod
-00001150: 696e 672e 6235 3871 b258 0300 0000 6236  ing.b58q.X....b6
-00001160: 3471 b358 1b00 0000 7265 6669 6e65 7279  4q.X....refinery
-00001170: 2e75 6e69 7473 2e65 6e63 6f64 696e 672e  .units.encoding.
-00001180: 6236 3471 b458 0300 0000 6238 3571 b558  b64q.X....b85q.X
-00001190: 1b00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
-000011a0: 7473 2e65 6e63 6f64 696e 672e 6238 3571  ts.encoding.b85q
-000011b0: b658 0400 0000 6261 7365 71b7 581c 0000  .X....baseq.X...
-000011c0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-000011d0: 656e 636f 6469 6e67 2e62 6173 6571 b858  encoding.baseq.X
-000011e0: 0600 0000 6370 3132 3532 71b9 581e 0000  ....cp1252q.X...
-000011f0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00001200: 656e 636f 6469 6e67 2e63 7031 3235 3271  encoding.cp1252q
-00001210: ba58 0300 0000 6573 6371 bb58 1b00 0000  .X....escq.X....
-00001220: 7265 6669 6e65 7279 2e75 6e69 7473 2e65  refinery.units.e
-00001230: 6e63 6f64 696e 672e 6573 6371 bc58 0300  ncoding.escq.X..
-00001240: 0000 6865 7871 bd58 1b00 0000 7265 6669  ..hexq.X....refi
-00001250: 6e65 7279 2e75 6e69 7473 2e65 6e63 6f64  nery.units.encod
-00001260: 696e 672e 6865 7871 be58 0700 0000 6874  ing.hexq.X....ht
-00001270: 6d6c 6573 6371 bf58 1f00 0000 7265 6669  mlescq.X....refi
-00001280: 6e65 7279 2e75 6e69 7473 2e65 6e63 6f64  nery.units.encod
-00001290: 696e 672e 6874 6d6c 6573 6371 c058 0700  ing.htmlescq.X..
-000012a0: 0000 6e65 7462 696f 7371 c158 1f00 0000  ..netbiosq.X....
-000012b0: 7265 6669 6e65 7279 2e75 6e69 7473 2e65  refinery.units.e
-000012c0: 6e63 6f64 696e 672e 6e65 7462 696f 7371  ncoding.netbiosq
-000012d0: c258 0600 0000 7073 3173 7472 71c3 581e  .X....ps1strq.X.
-000012e0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-000012f0: 732e 656e 636f 6469 6e67 2e70 7331 7374  s.encoding.ps1st
-00001300: 7271 c458 0600 0000 7265 636f 6465 71c5  rq.X....recodeq.
-00001310: 581e 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
-00001320: 6974 732e 656e 636f 6469 6e67 2e72 6563  its.encoding.rec
-00001330: 6f64 6571 c658 0300 0000 7531 3671 c758  odeq.X....u16q.X
-00001340: 1b00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
-00001350: 7473 2e65 6e63 6f64 696e 672e 7531 3671  ts.encoding.u16q
-00001360: c858 0300 0000 7572 6c71 c958 1b00 0000  .X....urlq.X....
-00001370: 7265 6669 6e65 7279 2e75 6e69 7473 2e65  refinery.units.e
-00001380: 6e63 6f64 696e 672e 7572 6c71 ca58 0500  ncoding.urlq.X..
-00001390: 0000 7575 656e 6371 cb58 1d00 0000 7265  ..uuencq.X....re
-000013a0: 6669 6e65 7279 2e75 6e69 7473 2e65 6e63  finery.units.enc
-000013b0: 6f64 696e 672e 7575 656e 6371 cc58 0600  oding.uuencq.X..
-000013c0: 0000 7773 6865 6e63 71cd 581e 0000 0072  ..wshencq.X....r
-000013d0: 6566 696e 6572 792e 756e 6974 732e 656e  efinery.units.en
-000013e0: 636f 6469 6e67 2e77 7368 656e 6371 ce58  coding.wshencq.X
-000013f0: 0300 0000 6133 7871 cf58 1a00 0000 7265  ....a3xq.X....re
-00001400: 6669 6e65 7279 2e75 6e69 7473 2e66 6f72  finery.units.for
-00001410: 6d61 7473 2e61 3378 71d0 5802 0000 0078  mats.a3xq.X....x
-00001420: 7471 d158 2100 0000 7265 6669 6e65 7279  tq.X!...refinery
-00001430: 2e75 6e69 7473 2e66 6f72 6d61 7473 2e61  .units.formats.a
-00001440: 7263 6869 7665 2e78 7471 d258 0400 0000  rchive.xtq.X....
-00001450: 7874 377a 71d3 5823 0000 0072 6566 696e  xt7zq.X#...refin
-00001460: 6572 792e 756e 6974 732e 666f 726d 6174  ery.units.format
-00001470: 732e 6172 6368 6976 652e 7874 377a 71d4  s.archive.xt7zq.
-00001480: 5805 0000 0078 7461 6365 71d5 5824 0000  X....xtaceq.X$..
-00001490: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-000014a0: 666f 726d 6174 732e 6172 6368 6976 652e  formats.archive.
-000014b0: 7874 6163 6571 d658 0600 0000 7874 6173  xtaceq.X....xtas
-000014c0: 6172 71d7 5825 0000 0072 6566 696e 6572  arq.X%...refiner
-000014d0: 792e 756e 6974 732e 666f 726d 6174 732e  y.units.formats.
-000014e0: 6172 6368 6976 652e 7874 6173 6172 71d8  archive.xtasarq.
-000014f0: 5805 0000 0078 7463 6162 71d9 5824 0000  X....xtcabq.X$..
-00001500: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00001510: 666f 726d 6174 732e 6172 6368 6976 652e  formats.archive.
-00001520: 7874 6361 6271 da58 0600 0000 7874 6370  xtcabq.X....xtcp
-00001530: 696f 71db 5825 0000 0072 6566 696e 6572  ioq.X%...refiner
-00001540: 792e 756e 6974 732e 666f 726d 6174 732e  y.units.formats.
-00001550: 6172 6368 6976 652e 7874 6370 696f 71dc  archive.xtcpioq.
-00001560: 5805 0000 0078 7469 736f 71dd 5824 0000  X....xtisoq.X$..
-00001570: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00001580: 666f 726d 6174 732e 6172 6368 6976 652e  formats.archive.
-00001590: 7874 6973 6f71 de58 0500 0000 7874 6973  xtisoq.X....xtis
-000015a0: 7371 df58 2400 0000 7265 6669 6e65 7279  sq.X$...refinery
-000015b0: 2e75 6e69 7473 2e66 6f72 6d61 7473 2e61  .units.formats.a
-000015c0: 7263 6869 7665 2e78 7469 7373 71e0 5806  rchive.xtissq.X.
+00001010: 6465 7269 7665 2e70 626b 6466 3171 a658  derive.pbkdf1q.X
+00001020: 0600 0000 7062 6b64 6632 71a7 5826 0000  ....pbkdf2q.X&..
+00001030: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00001040: 6372 7970 746f 2e6b 6579 6465 7269 7665  crypto.keyderive
+00001050: 2e70 626b 6466 3271 a858 0600 0000 7563  .pbkdf2q.X....uc
+00001060: 7279 7074 71a9 5829 0000 0072 6566 696e  ryptq.X)...refin
+00001070: 6572 792e 756e 6974 732e 6372 7970 746f  ery.units.crypto
+00001080: 2e6b 6579 6465 7269 7665 2e75 6e69 7863  .keyderive.unixc
+00001090: 7279 7074 71aa 5806 0000 0061 7462 6173  ryptq.X....atbas
+000010a0: 6871 ab58 1e00 0000 7265 6669 6e65 7279  hq.X....refinery
+000010b0: 2e75 6e69 7473 2e65 6e63 6f64 696e 672e  .units.encoding.
+000010c0: 6174 6261 7368 71ac 5803 0000 0062 3332  atbashq.X....b32
+000010d0: 71ad 581b 0000 0072 6566 696e 6572 792e  q.X....refinery.
+000010e0: 756e 6974 732e 656e 636f 6469 6e67 2e62  units.encoding.b
+000010f0: 3332 71ae 5803 0000 0062 3538 71af 581b  32q.X....b58q.X.
+00001100: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00001110: 732e 656e 636f 6469 6e67 2e62 3538 71b0  s.encoding.b58q.
+00001120: 5803 0000 0062 3634 71b1 581b 0000 0072  X....b64q.X....r
+00001130: 6566 696e 6572 792e 756e 6974 732e 656e  efinery.units.en
+00001140: 636f 6469 6e67 2e62 3634 71b2 5803 0000  coding.b64q.X...
+00001150: 0062 3835 71b3 581b 0000 0072 6566 696e  .b85q.X....refin
+00001160: 6572 792e 756e 6974 732e 656e 636f 6469  ery.units.encodi
+00001170: 6e67 2e62 3835 71b4 5804 0000 0062 6173  ng.b85q.X....bas
+00001180: 6571 b558 1c00 0000 7265 6669 6e65 7279  eq.X....refinery
+00001190: 2e75 6e69 7473 2e65 6e63 6f64 696e 672e  .units.encoding.
+000011a0: 6261 7365 71b6 5806 0000 0063 7031 3235  baseq.X....cp125
+000011b0: 3271 b758 1e00 0000 7265 6669 6e65 7279  2q.X....refinery
+000011c0: 2e75 6e69 7473 2e65 6e63 6f64 696e 672e  .units.encoding.
+000011d0: 6370 3132 3532 71b8 5803 0000 0065 7363  cp1252q.X....esc
+000011e0: 71b9 581b 0000 0072 6566 696e 6572 792e  q.X....refinery.
+000011f0: 756e 6974 732e 656e 636f 6469 6e67 2e65  units.encoding.e
+00001200: 7363 71ba 5803 0000 0068 6578 71bb 581b  scq.X....hexq.X.
+00001210: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00001220: 732e 656e 636f 6469 6e67 2e68 6578 71bc  s.encoding.hexq.
+00001230: 5807 0000 0068 746d 6c65 7363 71bd 581f  X....htmlescq.X.
+00001240: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00001250: 732e 656e 636f 6469 6e67 2e68 746d 6c65  s.encoding.htmle
+00001260: 7363 71be 5807 0000 006e 6574 6269 6f73  scq.X....netbios
+00001270: 71bf 581f 0000 0072 6566 696e 6572 792e  q.X....refinery.
+00001280: 756e 6974 732e 656e 636f 6469 6e67 2e6e  units.encoding.n
+00001290: 6574 6269 6f73 71c0 5806 0000 0070 7331  etbiosq.X....ps1
+000012a0: 7374 7271 c158 1e00 0000 7265 6669 6e65  strq.X....refine
+000012b0: 7279 2e75 6e69 7473 2e65 6e63 6f64 696e  ry.units.encodin
+000012c0: 672e 7073 3173 7472 71c2 5806 0000 0072  g.ps1strq.X....r
+000012d0: 6563 6f64 6571 c358 1e00 0000 7265 6669  ecodeq.X....refi
+000012e0: 6e65 7279 2e75 6e69 7473 2e65 6e63 6f64  nery.units.encod
+000012f0: 696e 672e 7265 636f 6465 71c4 5803 0000  ing.recodeq.X...
+00001300: 0075 3136 71c5 581b 0000 0072 6566 696e  .u16q.X....refin
+00001310: 6572 792e 756e 6974 732e 656e 636f 6469  ery.units.encodi
+00001320: 6e67 2e75 3136 71c6 5803 0000 0075 726c  ng.u16q.X....url
+00001330: 71c7 581b 0000 0072 6566 696e 6572 792e  q.X....refinery.
+00001340: 756e 6974 732e 656e 636f 6469 6e67 2e75  units.encoding.u
+00001350: 726c 71c8 5805 0000 0075 7565 6e63 71c9  rlq.X....uuencq.
+00001360: 581d 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
+00001370: 6974 732e 656e 636f 6469 6e67 2e75 7565  its.encoding.uue
+00001380: 6e63 71ca 5806 0000 0077 7368 656e 6371  ncq.X....wshencq
+00001390: cb58 1e00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
+000013a0: 6e69 7473 2e65 6e63 6f64 696e 672e 7773  nits.encoding.ws
+000013b0: 6865 6e63 71cc 5803 0000 0061 3378 71cd  hencq.X....a3xq.
+000013c0: 581a 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
+000013d0: 6974 732e 666f 726d 6174 732e 6133 7871  its.formats.a3xq
+000013e0: ce58 0200 0000 7874 71cf 5821 0000 0072  .X....xtq.X!...r
+000013f0: 6566 696e 6572 792e 756e 6974 732e 666f  efinery.units.fo
+00001400: 726d 6174 732e 6172 6368 6976 652e 7874  rmats.archive.xt
+00001410: 71d0 5804 0000 0078 7437 7a71 d158 2300  q.X....xt7zq.X#.
+00001420: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+00001430: 2e66 6f72 6d61 7473 2e61 7263 6869 7665  .formats.archive
+00001440: 2e78 7437 7a71 d258 0500 0000 7874 6163  .xt7zq.X....xtac
+00001450: 6571 d358 2400 0000 7265 6669 6e65 7279  eq.X$...refinery
+00001460: 2e75 6e69 7473 2e66 6f72 6d61 7473 2e61  .units.formats.a
+00001470: 7263 6869 7665 2e78 7461 6365 71d4 5806  rchive.xtaceq.X.
+00001480: 0000 0078 7461 7361 7271 d558 2500 0000  ...xtasarq.X%...
+00001490: 7265 6669 6e65 7279 2e75 6e69 7473 2e66  refinery.units.f
+000014a0: 6f72 6d61 7473 2e61 7263 6869 7665 2e78  ormats.archive.x
+000014b0: 7461 7361 7271 d658 0500 0000 7874 6361  tasarq.X....xtca
+000014c0: 6271 d758 2400 0000 7265 6669 6e65 7279  bq.X$...refinery
+000014d0: 2e75 6e69 7473 2e66 6f72 6d61 7473 2e61  .units.formats.a
+000014e0: 7263 6869 7665 2e78 7463 6162 71d8 5806  rchive.xtcabq.X.
+000014f0: 0000 0078 7463 7069 6f71 d958 2500 0000  ...xtcpioq.X%...
+00001500: 7265 6669 6e65 7279 2e75 6e69 7473 2e66  refinery.units.f
+00001510: 6f72 6d61 7473 2e61 7263 6869 7665 2e78  ormats.archive.x
+00001520: 7463 7069 6f71 da58 0500 0000 7874 6973  tcpioq.X....xtis
+00001530: 6f71 db58 2400 0000 7265 6669 6e65 7279  oq.X$...refinery
+00001540: 2e75 6e69 7473 2e66 6f72 6d61 7473 2e61  .units.formats.a
+00001550: 7263 6869 7665 2e78 7469 736f 71dc 5805  rchive.xtisoq.X.
+00001560: 0000 0078 7469 7373 71dd 5824 0000 0072  ...xtissq.X$...r
+00001570: 6566 696e 6572 792e 756e 6974 732e 666f  efinery.units.fo
+00001580: 726d 6174 732e 6172 6368 6976 652e 7874  rmats.archive.xt
+00001590: 6973 7371 de58 0600 0000 7874 6e6f 6465  issq.X....xtnode
+000015a0: 71df 5825 0000 0072 6566 696e 6572 792e  q.X%...refinery.
+000015b0: 756e 6974 732e 666f 726d 6174 732e 6172  units.formats.ar
+000015c0: 6368 6976 652e 7874 6e6f 6465 71e0 5806  chive.xtnodeq.X.
 000015d0: 0000 0078 746e 7369 7371 e158 2500 0000  ...xtnsisq.X%...
 000015e0: 7265 6669 6e65 7279 2e75 6e69 7473 2e66  refinery.units.f
 000015f0: 6f72 6d61 7473 2e61 7263 6869 7665 2e78  ormats.archive.x
 00001600: 746e 7369 7371 e258 0500 0000 7874 7079  tnsisq.X....xtpy
 00001610: 6971 e358 2400 0000 7265 6669 6e65 7279  iq.X$...refinery
 00001620: 2e75 6e69 7473 2e66 6f72 6d61 7473 2e61  .units.formats.a
 00001630: 7263 6869 7665 2e78 7470 7969 71e4 5805  rchive.xtpyiq.X.
@@ -634,280 +634,284 @@
 00002790: 696e 6572 792e 756e 6974 732e 6d65 7461  inery.units.meta
 000027a0: 2e73 6570 728a 0100 0058 0600 0000 736f  .sepr....X....so
 000027b0: 7274 6564 728b 0100 0058 1a00 0000 7265  rtedr....X....re
 000027c0: 6669 6e65 7279 2e75 6e69 7473 2e6d 6574  finery.units.met
 000027d0: 612e 736f 7274 6564 728c 0100 0058 0400  a.sortedr....X..
 000027e0: 0000 7377 6170 728d 0100 0058 1800 0000  ..swapr....X....
 000027f0: 7265 6669 6e65 7279 2e75 6e69 7473 2e6d  refinery.units.m
-00002800: 6574 612e 7377 6170 728e 0100 0058 0400  eta.swapr....X..
-00002810: 0000 7866 6363 728f 0100 0058 1800 0000  ..xfccr....X....
-00002820: 7265 6669 6e65 7279 2e75 6e69 7473 2e6d  refinery.units.m
-00002830: 6574 612e 7866 6363 7290 0100 0058 0700  eta.xfccr....X..
-00002840: 0000 6175 746f 786f 7272 9101 0000 581b  ..autoxorr....X.
-00002850: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-00002860: 732e 6d69 7363 2e61 7574 6f78 6f72 7292  s.misc.autoxorr.
-00002870: 0100 0058 0600 0000 636f 7570 6c65 7293  ...X....coupler.
-00002880: 0100 0058 1a00 0000 7265 6669 6e65 7279  ...X....refinery
-00002890: 2e75 6e69 7473 2e6d 6973 632e 636f 7570  .units.misc.coup
-000028a0: 6c65 7294 0100 0058 0700 0000 6461 7465  ler....X....date
-000028b0: 6669 7872 9501 0000 581b 0000 0072 6566  fixr....X....ref
-000028c0: 696e 6572 792e 756e 6974 732e 6d69 7363  inery.units.misc
-000028d0: 2e64 6174 6566 6978 7296 0100 0058 0300  .datefixr....X..
-000028e0: 0000 6472 7072 9701 0000 5817 0000 0072  ..drpr....X....r
-000028f0: 6566 696e 6572 792e 756e 6974 732e 6d69  efinery.units.mi
-00002900: 7363 2e64 7270 7298 0100 0058 0300 0000  sc.drpr....X....
-00002910: 6e6f 7072 9901 0000 5817 0000 0072 6566  nopr....X....ref
-00002920: 696e 6572 792e 756e 6974 732e 6d69 7363  inery.units.misc
-00002930: 2e6e 6f70 729a 0100 0058 0600 0000 7572  .nopr....X....ur
-00002940: 6c66 6978 729b 0100 0058 1a00 0000 7265  lfixr....X....re
-00002950: 6669 6e65 7279 2e75 6e69 7473 2e6d 6973  finery.units.mis
-00002960: 632e 7572 6c66 6978 729c 0100 0058 0400  c.urlfixr....X..
-00002970: 0000 786b 6579 729d 0100 0058 1800 0000  ..xkeyr....X....
-00002980: 7265 6669 6e65 7279 2e75 6e69 7473 2e6d  refinery.units.m
-00002990: 6973 632e 786b 6579 729e 0100 0058 0e00  isc.xkeyr....X..
-000029a0: 0000 6465 6f62 5f6a 735f 6172 7261 7973  ..deob_js_arrays
-000029b0: 729f 0100 0058 2400 0000 7265 6669 6e65  r....X$...refine
-000029c0: 7279 2e75 6e69 7473 2e6f 6266 7573 6361  ry.units.obfusca
-000029d0: 7469 6f6e 2e6a 732e 6172 7261 7973 72a0  tion.js.arraysr.
-000029e0: 0100 0058 0f00 0000 6465 6f62 5f6a 735f  ...X....deob_js_
-000029f0: 6765 7461 7474 7272 a101 0000 5825 0000  getattrr....X%..
-00002a00: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00002a10: 6f62 6675 7363 6174 696f 6e2e 6a73 2e67  obfuscation.js.g
-00002a20: 6574 6174 7472 72a2 0100 0058 0e00 0000  etattrr....X....
-00002a30: 6465 6f62 5f6a 735f 7475 706c 6573 72a3  deob_js_tuplesr.
-00002a40: 0100 0058 2400 0000 7265 6669 6e65 7279  ...X$...refinery
-00002a50: 2e75 6e69 7473 2e6f 6266 7573 6361 7469  .units.obfuscati
-00002a60: 6f6e 2e6a 732e 7475 706c 6573 72a4 0100  on.js.tuplesr...
-00002a70: 0058 0800 0000 6465 6f62 5f70 7331 72a5  .X....deob_ps1r.
-00002a80: 0100 0058 2200 0000 7265 6669 6e65 7279  ...X"...refinery
-00002a90: 2e75 6e69 7473 2e6f 6266 7573 6361 7469  .units.obfuscati
-00002aa0: 6f6e 2e70 7331 2e61 6c6c 72a6 0100 0058  on.ps1.allr....X
-00002ab0: 1100 0000 6465 6f62 5f70 7331 5f62 7261  ....deob_ps1_bra
-00002ac0: 636b 6574 7372 a701 0000 5827 0000 0072  cketsr....X'...r
-00002ad0: 6566 696e 6572 792e 756e 6974 732e 6f62  efinery.units.ob
-00002ae0: 6675 7363 6174 696f 6e2e 7073 312e 6272  fuscation.ps1.br
-00002af0: 6163 6b65 7473 72a8 0100 0058 0e00 0000  acketsr....X....
-00002b00: 6465 6f62 5f70 7331 5f63 6173 6573 72a9  deob_ps1_casesr.
-00002b10: 0100 0058 2400 0000 7265 6669 6e65 7279  ...X$...refinery
-00002b20: 2e75 6e69 7473 2e6f 6266 7573 6361 7469  .units.obfuscati
-00002b30: 6f6e 2e70 7331 2e63 6173 6573 72aa 0100  on.ps1.casesr...
-00002b40: 0058 0f00 0000 6465 6f62 5f70 7331 5f63  .X....deob_ps1_c
-00002b50: 6f6e 6361 7472 ab01 0000 5825 0000 0072  oncatr....X%...r
-00002b60: 6566 696e 6572 792e 756e 6974 732e 6f62  efinery.units.ob
-00002b70: 6675 7363 6174 696f 6e2e 7073 312e 636f  fuscation.ps1.co
-00002b80: 6e63 6174 72ac 0100 0058 0f00 0000 6465  ncatr....X....de
-00002b90: 6f62 5f70 7331 5f65 7363 6170 6572 ad01  ob_ps1_escaper..
-00002ba0: 0000 5825 0000 0072 6566 696e 6572 792e  ..X%...refinery.
-00002bb0: 756e 6974 732e 6f62 6675 7363 6174 696f  units.obfuscatio
-00002bc0: 6e2e 7073 312e 6573 6361 7065 72ae 0100  n.ps1.escaper...
-00002bd0: 0058 0f00 0000 6465 6f62 5f70 7331 5f66  .X....deob_ps1_f
-00002be0: 6f72 6d61 7472 af01 0000 5825 0000 0072  ormatr....X%...r
-00002bf0: 6566 696e 6572 792e 756e 6974 732e 6f62  efinery.units.ob
-00002c00: 6675 7363 6174 696f 6e2e 7073 312e 666f  fuscation.ps1.fo
-00002c10: 726d 6174 72b0 0100 0058 0f00 0000 6465  rmatr....X....de
-00002c20: 6f62 5f70 7331 5f69 6e76 6f6b 6572 b101  ob_ps1_invoker..
-00002c30: 0000 5825 0000 0072 6566 696e 6572 792e  ..X%...refinery.
-00002c40: 756e 6974 732e 6f62 6675 7363 6174 696f  units.obfuscatio
-00002c50: 6e2e 7073 312e 696e 766f 6b65 72b2 0100  n.ps1.invoker...
-00002c60: 0058 0f00 0000 6465 6f62 5f70 7331 5f73  .X....deob_ps1_s
-00002c70: 6563 7374 7272 b301 0000 582b 0000 0072  ecstrr....X+...r
-00002c80: 6566 696e 6572 792e 756e 6974 732e 6f62  efinery.units.ob
-00002c90: 6675 7363 6174 696f 6e2e 7073 312e 7365  fuscation.ps1.se
-00002ca0: 6375 7265 7374 7269 6e67 72b4 0100 0058  curestringr....X
-00002cb0: 1600 0000 6465 6f62 5f70 7331 5f73 7472  ....deob_ps1_str
-00002cc0: 696e 6772 6570 6c61 6365 72b5 0100 0058  ingreplacer....X
-00002cd0: 2c00 0000 7265 6669 6e65 7279 2e75 6e69  ,...refinery.uni
-00002ce0: 7473 2e6f 6266 7573 6361 7469 6f6e 2e70  ts.obfuscation.p
-00002cf0: 7331 2e73 7472 696e 6772 6570 6c61 6365  s1.stringreplace
-00002d00: 72b6 0100 0058 1100 0000 6465 6f62 5f70  r....X....deob_p
-00002d10: 7331 5f74 7970 6563 6173 7472 b701 0000  s1_typecastr....
-00002d20: 5827 0000 0072 6566 696e 6572 792e 756e  X'...refinery.un
-00002d30: 6974 732e 6f62 6675 7363 6174 696f 6e2e  its.obfuscation.
-00002d40: 7073 312e 7479 7065 6361 7374 72b8 0100  ps1.typecastr...
-00002d50: 0058 1000 0000 6465 6f62 5f70 7331 5f75  .X....deob_ps1_u
-00002d60: 6e63 7572 6c79 72b9 0100 0058 2600 0000  ncurlyr....X&...
-00002d70: 7265 6669 6e65 7279 2e75 6e69 7473 2e6f  refinery.units.o
-00002d80: 6266 7573 6361 7469 6f6e 2e70 7331 2e75  bfuscation.ps1.u
-00002d90: 6e63 7572 6c79 72ba 0100 0058 0800 0000  ncurlyr....X....
-00002da0: 6465 6f62 5f76 6261 72bb 0100 0058 2200  deob_vbar....X".
-00002db0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-00002dc0: 2e6f 6266 7573 6361 7469 6f6e 2e76 6261  .obfuscation.vba
-00002dd0: 2e61 6c6c 72bc 0100 0058 1300 0000 6465  .allr....X....de
-00002de0: 6f62 5f76 6261 5f61 7269 7468 6d65 7469  ob_vba_arithmeti
-00002df0: 6372 bd01 0000 5829 0000 0072 6566 696e  cr....X)...refin
-00002e00: 6572 792e 756e 6974 732e 6f62 6675 7363  ery.units.obfusc
-00002e10: 6174 696f 6e2e 7662 612e 6172 6974 686d  ation.vba.arithm
-00002e20: 6574 6963 72be 0100 0058 1100 0000 6465  eticr....X....de
-00002e30: 6f62 5f76 6261 5f62 7261 636b 6574 7372  ob_vba_bracketsr
-00002e40: bf01 0000 5827 0000 0072 6566 696e 6572  ....X'...refiner
-00002e50: 792e 756e 6974 732e 6f62 6675 7363 6174  y.units.obfuscat
-00002e60: 696f 6e2e 7662 612e 6272 6163 6b65 7473  ion.vba.brackets
-00002e70: 72c0 0100 0058 1600 0000 6465 6f62 5f76  r....X....deob_v
-00002e80: 6261 5f63 6861 725f 6675 6e63 7469 6f6e  ba_char_function
-00002e90: 72c1 0100 0058 2300 0000 7265 6669 6e65  r....X#...refine
-00002ea0: 7279 2e75 6e69 7473 2e6f 6266 7573 6361  ry.units.obfusca
-00002eb0: 7469 6f6e 2e76 6261 2e63 6861 7272 c201  tion.vba.charr..
-00002ec0: 0000 5811 0000 0064 656f 625f 7662 615f  ..X....deob_vba_
-00002ed0: 636f 6d6d 656e 7473 72c3 0100 0058 2700  commentsr....X'.
-00002ee0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-00002ef0: 2e6f 6266 7573 6361 7469 6f6e 2e76 6261  .obfuscation.vba
-00002f00: 2e63 6f6d 6d65 6e74 7372 c401 0000 580f  .commentsr....X.
-00002f10: 0000 0064 656f 625f 7662 615f 636f 6e63  ...deob_vba_conc
-00002f20: 6174 72c5 0100 0058 2500 0000 7265 6669  atr....X%...refi
-00002f30: 6e65 7279 2e75 6e69 7473 2e6f 6266 7573  nery.units.obfus
-00002f40: 6361 7469 6f6e 2e76 6261 2e63 6f6e 6361  cation.vba.conca
-00002f50: 7472 c601 0000 5812 0000 0064 656f 625f  tr....X....deob_
-00002f60: 7662 615f 636f 6e73 7461 6e74 7372 c701  vba_constantsr..
-00002f70: 0000 5828 0000 0072 6566 696e 6572 792e  ..X(...refinery.
-00002f80: 756e 6974 732e 6f62 6675 7363 6174 696f  units.obfuscatio
-00002f90: 6e2e 7662 612e 636f 6e73 7461 6e74 7372  n.vba.constantsr
-00002fa0: c801 0000 5818 0000 0064 656f 625f 7662  ....X....deob_vb
-00002fb0: 615f 6475 6d6d 795f 7661 7269 6162 6c65  a_dummy_variable
-00002fc0: 7372 c901 0000 5826 0000 0072 6566 696e  sr....X&...refin
-00002fd0: 6572 792e 756e 6974 732e 6f62 6675 7363  ery.units.obfusc
-00002fe0: 6174 696f 6e2e 7662 612e 6475 6d6d 6965  ation.vba.dummie
-00002ff0: 7372 ca01 0000 5816 0000 0064 656f 625f  sr....X....deob_
-00003000: 7662 615f 7374 7269 6e67 7265 706c 6163  vba_stringreplac
-00003010: 6572 cb01 0000 582c 0000 0072 6566 696e  er....X,...refin
-00003020: 6572 792e 756e 6974 732e 6f62 6675 7363  ery.units.obfusc
-00003030: 6174 696f 6e2e 7662 612e 7374 7269 6e67  ation.vba.string
-00003040: 7265 706c 6163 6572 cc01 0000 5816 0000  replacer....X...
-00003050: 0064 656f 625f 7662 615f 7374 7269 6e67  .deob_vba_string
-00003060: 7265 7665 7273 6572 cd01 0000 582c 0000  reverser....X,..
-00003070: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00003080: 6f62 6675 7363 6174 696f 6e2e 7662 612e  obfuscation.vba.
-00003090: 7374 7269 6e67 7265 7665 7273 6572 ce01  stringreverser..
-000030a0: 0000 5815 0000 0064 656f 625f 7662 615f  ..X....deob_vba_
-000030b0: 6368 725f 6c69 7465 7261 6c73 72cf 0100  chr_literalsr...
-000030c0: 0058 2200 0000 7265 6669 6e65 7279 2e75  .X"...refinery.u
-000030d0: 6e69 7473 2e6f 6266 7573 6361 7469 6f6e  nits.obfuscation
-000030e0: 2e76 6261 2e76 6261 72d0 0100 0058 0500  .vba.vbar....X..
-000030f0: 0000 6361 7276 6572 d101 0000 581c 0000  ..carver....X...
-00003100: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00003110: 7061 7474 6572 6e2e 6361 7276 6572 d201  pattern.carver..
-00003120: 0000 5808 0000 0063 6172 7665 5f37 7a72  ..X....carve_7zr
-00003130: d301 0000 581f 0000 0072 6566 696e 6572  ....X....refiner
-00003140: 792e 756e 6974 732e 7061 7474 6572 6e2e  y.units.pattern.
-00003150: 6361 7276 655f 377a 72d4 0100 0058 0a00  carve_7zr....X..
-00003160: 0000 6361 7276 655f 6a73 6f6e 72d5 0100  ..carve_jsonr...
-00003170: 0058 2100 0000 7265 6669 6e65 7279 2e75  .X!...refinery.u
-00003180: 6e69 7473 2e70 6174 7465 726e 2e63 6172  nits.pattern.car
-00003190: 7665 5f6a 736f 6e72 d601 0000 5809 0000  ve_jsonr....X...
-000031a0: 0063 6172 7665 5f6c 6e6b 72d7 0100 0058  .carve_lnkr....X
-000031b0: 2000 0000 7265 6669 6e65 7279 2e75 6e69   ...refinery.uni
-000031c0: 7473 2e70 6174 7465 726e 2e63 6172 7665  ts.pattern.carve
-000031d0: 5f6c 6e6b 72d8 0100 0058 0800 0000 6361  _lnkr....X....ca
-000031e0: 7276 655f 7065 72d9 0100 0058 1f00 0000  rve_per....X....
-000031f0: 7265 6669 6e65 7279 2e75 6e69 7473 2e70  refinery.units.p
-00003200: 6174 7465 726e 2e63 6172 7665 5f70 6572  attern.carve_per
-00003210: da01 0000 5809 0000 0063 6172 7665 5f72  ....X....carve_r
-00003220: 7466 72db 0100 0058 2000 0000 7265 6669  tfr....X ...refi
-00003230: 6e65 7279 2e75 6e69 7473 2e70 6174 7465  nery.units.patte
-00003240: 726e 2e63 6172 7665 5f72 7466 72dc 0100  rn.carve_rtfr...
-00003250: 0058 0900 0000 6361 7276 655f 786d 6c72  .X....carve_xmlr
-00003260: dd01 0000 5820 0000 0072 6566 696e 6572  ....X ...refiner
-00003270: 792e 756e 6974 732e 7061 7474 6572 6e2e  y.units.pattern.
-00003280: 6361 7276 655f 786d 6c72 de01 0000 5809  carve_xmlr....X.
-00003290: 0000 0063 6172 7665 5f7a 6970 72df 0100  ...carve_zipr...
-000032a0: 0058 2000 0000 7265 6669 6e65 7279 2e75  .X ...refinery.u
-000032b0: 6e69 7473 2e70 6174 7465 726e 2e63 6172  nits.pattern.car
-000032c0: 7665 5f7a 6970 72e0 0100 0058 0600 0000  ve_zipr....X....
-000032d0: 6465 6661 6e67 72e1 0100 0058 1d00 0000  defangr....X....
+00002800: 6574 612e 7377 6170 728e 0100 0058 0900  eta.swapr....X..
+00002810: 0000 7472 616e 7370 6f73 6572 8f01 0000  ..transposer....
+00002820: 581d 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
+00002830: 6974 732e 6d65 7461 2e74 7261 6e73 706f  its.meta.transpo
+00002840: 7365 7290 0100 0058 0400 0000 7866 6363  ser....X....xfcc
+00002850: 7291 0100 0058 1800 0000 7265 6669 6e65  r....X....refine
+00002860: 7279 2e75 6e69 7473 2e6d 6574 612e 7866  ry.units.meta.xf
+00002870: 6363 7292 0100 0058 0700 0000 6175 746f  ccr....X....auto
+00002880: 786f 7272 9301 0000 581b 0000 0072 6566  xorr....X....ref
+00002890: 696e 6572 792e 756e 6974 732e 6d69 7363  inery.units.misc
+000028a0: 2e61 7574 6f78 6f72 7294 0100 0058 0600  .autoxorr....X..
+000028b0: 0000 636f 7570 6c65 7295 0100 0058 1a00  ..coupler....X..
+000028c0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+000028d0: 2e6d 6973 632e 636f 7570 6c65 7296 0100  .misc.coupler...
+000028e0: 0058 0700 0000 6461 7465 6669 7872 9701  .X....datefixr..
+000028f0: 0000 581b 0000 0072 6566 696e 6572 792e  ..X....refinery.
+00002900: 756e 6974 732e 6d69 7363 2e64 6174 6566  units.misc.datef
+00002910: 6978 7298 0100 0058 0300 0000 6472 7072  ixr....X....drpr
+00002920: 9901 0000 5817 0000 0072 6566 696e 6572  ....X....refiner
+00002930: 792e 756e 6974 732e 6d69 7363 2e64 7270  y.units.misc.drp
+00002940: 729a 0100 0058 0300 0000 6e6f 7072 9b01  r....X....nopr..
+00002950: 0000 5817 0000 0072 6566 696e 6572 792e  ..X....refinery.
+00002960: 756e 6974 732e 6d69 7363 2e6e 6f70 729c  units.misc.nopr.
+00002970: 0100 0058 0600 0000 7572 6c66 6978 729d  ...X....urlfixr.
+00002980: 0100 0058 1a00 0000 7265 6669 6e65 7279  ...X....refinery
+00002990: 2e75 6e69 7473 2e6d 6973 632e 7572 6c66  .units.misc.urlf
+000029a0: 6978 729e 0100 0058 0400 0000 786b 6579  ixr....X....xkey
+000029b0: 729f 0100 0058 1800 0000 7265 6669 6e65  r....X....refine
+000029c0: 7279 2e75 6e69 7473 2e6d 6973 632e 786b  ry.units.misc.xk
+000029d0: 6579 72a0 0100 0058 0e00 0000 6465 6f62  eyr....X....deob
+000029e0: 5f6a 735f 6172 7261 7973 72a1 0100 0058  _js_arraysr....X
+000029f0: 2400 0000 7265 6669 6e65 7279 2e75 6e69  $...refinery.uni
+00002a00: 7473 2e6f 6266 7573 6361 7469 6f6e 2e6a  ts.obfuscation.j
+00002a10: 732e 6172 7261 7973 72a2 0100 0058 0f00  s.arraysr....X..
+00002a20: 0000 6465 6f62 5f6a 735f 6765 7461 7474  ..deob_js_getatt
+00002a30: 7272 a301 0000 5825 0000 0072 6566 696e  rr....X%...refin
+00002a40: 6572 792e 756e 6974 732e 6f62 6675 7363  ery.units.obfusc
+00002a50: 6174 696f 6e2e 6a73 2e67 6574 6174 7472  ation.js.getattr
+00002a60: 72a4 0100 0058 0e00 0000 6465 6f62 5f6a  r....X....deob_j
+00002a70: 735f 7475 706c 6573 72a5 0100 0058 2400  s_tuplesr....X$.
+00002a80: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+00002a90: 2e6f 6266 7573 6361 7469 6f6e 2e6a 732e  .obfuscation.js.
+00002aa0: 7475 706c 6573 72a6 0100 0058 0800 0000  tuplesr....X....
+00002ab0: 6465 6f62 5f70 7331 72a7 0100 0058 2200  deob_ps1r....X".
+00002ac0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+00002ad0: 2e6f 6266 7573 6361 7469 6f6e 2e70 7331  .obfuscation.ps1
+00002ae0: 2e61 6c6c 72a8 0100 0058 1100 0000 6465  .allr....X....de
+00002af0: 6f62 5f70 7331 5f62 7261 636b 6574 7372  ob_ps1_bracketsr
+00002b00: a901 0000 5827 0000 0072 6566 696e 6572  ....X'...refiner
+00002b10: 792e 756e 6974 732e 6f62 6675 7363 6174  y.units.obfuscat
+00002b20: 696f 6e2e 7073 312e 6272 6163 6b65 7473  ion.ps1.brackets
+00002b30: 72aa 0100 0058 0e00 0000 6465 6f62 5f70  r....X....deob_p
+00002b40: 7331 5f63 6173 6573 72ab 0100 0058 2400  s1_casesr....X$.
+00002b50: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+00002b60: 2e6f 6266 7573 6361 7469 6f6e 2e70 7331  .obfuscation.ps1
+00002b70: 2e63 6173 6573 72ac 0100 0058 0f00 0000  .casesr....X....
+00002b80: 6465 6f62 5f70 7331 5f63 6f6e 6361 7472  deob_ps1_concatr
+00002b90: ad01 0000 5825 0000 0072 6566 696e 6572  ....X%...refiner
+00002ba0: 792e 756e 6974 732e 6f62 6675 7363 6174  y.units.obfuscat
+00002bb0: 696f 6e2e 7073 312e 636f 6e63 6174 72ae  ion.ps1.concatr.
+00002bc0: 0100 0058 0f00 0000 6465 6f62 5f70 7331  ...X....deob_ps1
+00002bd0: 5f65 7363 6170 6572 af01 0000 5825 0000  _escaper....X%..
+00002be0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00002bf0: 6f62 6675 7363 6174 696f 6e2e 7073 312e  obfuscation.ps1.
+00002c00: 6573 6361 7065 72b0 0100 0058 0f00 0000  escaper....X....
+00002c10: 6465 6f62 5f70 7331 5f66 6f72 6d61 7472  deob_ps1_formatr
+00002c20: b101 0000 5825 0000 0072 6566 696e 6572  ....X%...refiner
+00002c30: 792e 756e 6974 732e 6f62 6675 7363 6174  y.units.obfuscat
+00002c40: 696f 6e2e 7073 312e 666f 726d 6174 72b2  ion.ps1.formatr.
+00002c50: 0100 0058 0f00 0000 6465 6f62 5f70 7331  ...X....deob_ps1
+00002c60: 5f69 6e76 6f6b 6572 b301 0000 5825 0000  _invoker....X%..
+00002c70: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00002c80: 6f62 6675 7363 6174 696f 6e2e 7073 312e  obfuscation.ps1.
+00002c90: 696e 766f 6b65 72b4 0100 0058 0f00 0000  invoker....X....
+00002ca0: 6465 6f62 5f70 7331 5f73 6563 7374 7272  deob_ps1_secstrr
+00002cb0: b501 0000 582b 0000 0072 6566 696e 6572  ....X+...refiner
+00002cc0: 792e 756e 6974 732e 6f62 6675 7363 6174  y.units.obfuscat
+00002cd0: 696f 6e2e 7073 312e 7365 6375 7265 7374  ion.ps1.securest
+00002ce0: 7269 6e67 72b6 0100 0058 1600 0000 6465  ringr....X....de
+00002cf0: 6f62 5f70 7331 5f73 7472 696e 6772 6570  ob_ps1_stringrep
+00002d00: 6c61 6365 72b7 0100 0058 2c00 0000 7265  lacer....X,...re
+00002d10: 6669 6e65 7279 2e75 6e69 7473 2e6f 6266  finery.units.obf
+00002d20: 7573 6361 7469 6f6e 2e70 7331 2e73 7472  uscation.ps1.str
+00002d30: 696e 6772 6570 6c61 6365 72b8 0100 0058  ingreplacer....X
+00002d40: 1100 0000 6465 6f62 5f70 7331 5f74 7970  ....deob_ps1_typ
+00002d50: 6563 6173 7472 b901 0000 5827 0000 0072  ecastr....X'...r
+00002d60: 6566 696e 6572 792e 756e 6974 732e 6f62  efinery.units.ob
+00002d70: 6675 7363 6174 696f 6e2e 7073 312e 7479  fuscation.ps1.ty
+00002d80: 7065 6361 7374 72ba 0100 0058 1000 0000  pecastr....X....
+00002d90: 6465 6f62 5f70 7331 5f75 6e63 7572 6c79  deob_ps1_uncurly
+00002da0: 72bb 0100 0058 2600 0000 7265 6669 6e65  r....X&...refine
+00002db0: 7279 2e75 6e69 7473 2e6f 6266 7573 6361  ry.units.obfusca
+00002dc0: 7469 6f6e 2e70 7331 2e75 6e63 7572 6c79  tion.ps1.uncurly
+00002dd0: 72bc 0100 0058 0800 0000 6465 6f62 5f76  r....X....deob_v
+00002de0: 6261 72bd 0100 0058 2200 0000 7265 6669  bar....X"...refi
+00002df0: 6e65 7279 2e75 6e69 7473 2e6f 6266 7573  nery.units.obfus
+00002e00: 6361 7469 6f6e 2e76 6261 2e61 6c6c 72be  cation.vba.allr.
+00002e10: 0100 0058 1300 0000 6465 6f62 5f76 6261  ...X....deob_vba
+00002e20: 5f61 7269 7468 6d65 7469 6372 bf01 0000  _arithmeticr....
+00002e30: 5829 0000 0072 6566 696e 6572 792e 756e  X)...refinery.un
+00002e40: 6974 732e 6f62 6675 7363 6174 696f 6e2e  its.obfuscation.
+00002e50: 7662 612e 6172 6974 686d 6574 6963 72c0  vba.arithmeticr.
+00002e60: 0100 0058 1100 0000 6465 6f62 5f76 6261  ...X....deob_vba
+00002e70: 5f62 7261 636b 6574 7372 c101 0000 5827  _bracketsr....X'
+00002e80: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00002e90: 732e 6f62 6675 7363 6174 696f 6e2e 7662  s.obfuscation.vb
+00002ea0: 612e 6272 6163 6b65 7473 72c2 0100 0058  a.bracketsr....X
+00002eb0: 1600 0000 6465 6f62 5f76 6261 5f63 6861  ....deob_vba_cha
+00002ec0: 725f 6675 6e63 7469 6f6e 72c3 0100 0058  r_functionr....X
+00002ed0: 2300 0000 7265 6669 6e65 7279 2e75 6e69  #...refinery.uni
+00002ee0: 7473 2e6f 6266 7573 6361 7469 6f6e 2e76  ts.obfuscation.v
+00002ef0: 6261 2e63 6861 7272 c401 0000 5811 0000  ba.charr....X...
+00002f00: 0064 656f 625f 7662 615f 636f 6d6d 656e  .deob_vba_commen
+00002f10: 7473 72c5 0100 0058 2700 0000 7265 6669  tsr....X'...refi
+00002f20: 6e65 7279 2e75 6e69 7473 2e6f 6266 7573  nery.units.obfus
+00002f30: 6361 7469 6f6e 2e76 6261 2e63 6f6d 6d65  cation.vba.comme
+00002f40: 6e74 7372 c601 0000 580f 0000 0064 656f  ntsr....X....deo
+00002f50: 625f 7662 615f 636f 6e63 6174 72c7 0100  b_vba_concatr...
+00002f60: 0058 2500 0000 7265 6669 6e65 7279 2e75  .X%...refinery.u
+00002f70: 6e69 7473 2e6f 6266 7573 6361 7469 6f6e  nits.obfuscation
+00002f80: 2e76 6261 2e63 6f6e 6361 7472 c801 0000  .vba.concatr....
+00002f90: 5812 0000 0064 656f 625f 7662 615f 636f  X....deob_vba_co
+00002fa0: 6e73 7461 6e74 7372 c901 0000 5828 0000  nstantsr....X(..
+00002fb0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00002fc0: 6f62 6675 7363 6174 696f 6e2e 7662 612e  obfuscation.vba.
+00002fd0: 636f 6e73 7461 6e74 7372 ca01 0000 5818  constantsr....X.
+00002fe0: 0000 0064 656f 625f 7662 615f 6475 6d6d  ...deob_vba_dumm
+00002ff0: 795f 7661 7269 6162 6c65 7372 cb01 0000  y_variablesr....
+00003000: 5826 0000 0072 6566 696e 6572 792e 756e  X&...refinery.un
+00003010: 6974 732e 6f62 6675 7363 6174 696f 6e2e  its.obfuscation.
+00003020: 7662 612e 6475 6d6d 6965 7372 cc01 0000  vba.dummiesr....
+00003030: 5816 0000 0064 656f 625f 7662 615f 7374  X....deob_vba_st
+00003040: 7269 6e67 7265 706c 6163 6572 cd01 0000  ringreplacer....
+00003050: 582c 0000 0072 6566 696e 6572 792e 756e  X,...refinery.un
+00003060: 6974 732e 6f62 6675 7363 6174 696f 6e2e  its.obfuscation.
+00003070: 7662 612e 7374 7269 6e67 7265 706c 6163  vba.stringreplac
+00003080: 6572 ce01 0000 5816 0000 0064 656f 625f  er....X....deob_
+00003090: 7662 615f 7374 7269 6e67 7265 7665 7273  vba_stringrevers
+000030a0: 6572 cf01 0000 582c 0000 0072 6566 696e  er....X,...refin
+000030b0: 6572 792e 756e 6974 732e 6f62 6675 7363  ery.units.obfusc
+000030c0: 6174 696f 6e2e 7662 612e 7374 7269 6e67  ation.vba.string
+000030d0: 7265 7665 7273 6572 d001 0000 5815 0000  reverser....X...
+000030e0: 0064 656f 625f 7662 615f 6368 725f 6c69  .deob_vba_chr_li
+000030f0: 7465 7261 6c73 72d1 0100 0058 2200 0000  teralsr....X"...
+00003100: 7265 6669 6e65 7279 2e75 6e69 7473 2e6f  refinery.units.o
+00003110: 6266 7573 6361 7469 6f6e 2e76 6261 2e76  bfuscation.vba.v
+00003120: 6261 72d2 0100 0058 0500 0000 6361 7276  bar....X....carv
+00003130: 6572 d301 0000 581c 0000 0072 6566 696e  er....X....refin
+00003140: 6572 792e 756e 6974 732e 7061 7474 6572  ery.units.patter
+00003150: 6e2e 6361 7276 6572 d401 0000 5808 0000  n.carver....X...
+00003160: 0063 6172 7665 5f37 7a72 d501 0000 581f  .carve_7zr....X.
+00003170: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00003180: 732e 7061 7474 6572 6e2e 6361 7276 655f  s.pattern.carve_
+00003190: 377a 72d6 0100 0058 0a00 0000 6361 7276  7zr....X....carv
+000031a0: 655f 6a73 6f6e 72d7 0100 0058 2100 0000  e_jsonr....X!...
+000031b0: 7265 6669 6e65 7279 2e75 6e69 7473 2e70  refinery.units.p
+000031c0: 6174 7465 726e 2e63 6172 7665 5f6a 736f  attern.carve_jso
+000031d0: 6e72 d801 0000 5809 0000 0063 6172 7665  nr....X....carve
+000031e0: 5f6c 6e6b 72d9 0100 0058 2000 0000 7265  _lnkr....X ...re
+000031f0: 6669 6e65 7279 2e75 6e69 7473 2e70 6174  finery.units.pat
+00003200: 7465 726e 2e63 6172 7665 5f6c 6e6b 72da  tern.carve_lnkr.
+00003210: 0100 0058 0800 0000 6361 7276 655f 7065  ...X....carve_pe
+00003220: 72db 0100 0058 1f00 0000 7265 6669 6e65  r....X....refine
+00003230: 7279 2e75 6e69 7473 2e70 6174 7465 726e  ry.units.pattern
+00003240: 2e63 6172 7665 5f70 6572 dc01 0000 5809  .carve_per....X.
+00003250: 0000 0063 6172 7665 5f72 7466 72dd 0100  ...carve_rtfr...
+00003260: 0058 2000 0000 7265 6669 6e65 7279 2e75  .X ...refinery.u
+00003270: 6e69 7473 2e70 6174 7465 726e 2e63 6172  nits.pattern.car
+00003280: 7665 5f72 7466 72de 0100 0058 0900 0000  ve_rtfr....X....
+00003290: 6361 7276 655f 786d 6c72 df01 0000 5820  carve_xmlr....X 
+000032a0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+000032b0: 732e 7061 7474 6572 6e2e 6361 7276 655f  s.pattern.carve_
+000032c0: 786d 6c72 e001 0000 5809 0000 0063 6172  xmlr....X....car
+000032d0: 7665 5f7a 6970 72e1 0100 0058 2000 0000  ve_zipr....X ...
 000032e0: 7265 6669 6e65 7279 2e75 6e69 7473 2e70  refinery.units.p
-000032f0: 6174 7465 726e 2e64 6566 616e 6772 e201  attern.defangr..
-00003300: 0000 5809 0000 0064 6e73 646f 6d61 696e  ..X....dnsdomain
-00003310: 72e3 0100 0058 2000 0000 7265 6669 6e65  r....X ...refine
+000032f0: 6174 7465 726e 2e63 6172 7665 5f7a 6970  attern.carve_zip
+00003300: 72e2 0100 0058 0600 0000 6465 6661 6e67  r....X....defang
+00003310: 72e3 0100 0058 1d00 0000 7265 6669 6e65  r....X....refine
 00003320: 7279 2e75 6e69 7473 2e70 6174 7465 726e  ry.units.pattern
-00003330: 2e64 6e73 646f 6d61 696e 72e4 0100 0058  .dnsdomainr....X
-00003340: 0900 0000 6d69 6d65 776f 7264 7372 e501  ....mimewordsr..
-00003350: 0000 5820 0000 0072 6566 696e 6572 792e  ..X ...refinery.
-00003360: 756e 6974 732e 7061 7474 6572 6e2e 6d69  units.pattern.mi
-00003370: 6d65 776f 7264 7372 e601 0000 5807 0000  mewordsr....X...
-00003380: 0072 6573 706c 6974 72e7 0100 0058 1e00  .resplitr....X..
-00003390: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-000033a0: 2e70 6174 7465 726e 2e72 6573 706c 6974  .pattern.resplit
-000033b0: 72e8 0100 0058 0500 0000 7265 7375 6272  r....X....resubr
-000033c0: e901 0000 581c 0000 0072 6566 696e 6572  ....X....refiner
-000033d0: 792e 756e 6974 732e 7061 7474 6572 6e2e  y.units.pattern.
-000033e0: 7265 7375 6272 ea01 0000 5803 0000 0072  resubr....X....r
-000033f0: 6578 72eb 0100 0058 1a00 0000 7265 6669  exr....X....refi
-00003400: 6e65 7279 2e75 6e69 7473 2e70 6174 7465  nery.units.patte
-00003410: 726e 2e72 6578 72ec 0100 0058 0600 0000  rn.rexr....X....
-00003420: 7374 7275 6374 72ed 0100 0058 2400 0000  structr....X$...
-00003430: 7265 6669 6e65 7279 2e75 6e69 7473 2e70  refinery.units.p
-00003440: 6174 7465 726e 2e73 7472 7563 745f 7061  attern.struct_pa
-00003450: 7273 6572 72ee 0100 0058 0800 0000 7375  rserr....X....su
-00003460: 6266 696c 6573 72ef 0100 0058 1f00 0000  bfilesr....X....
-00003470: 7265 6669 6e65 7279 2e75 6e69 7473 2e70  refinery.units.p
-00003480: 6174 7465 726e 2e73 7562 6669 6c65 7372  attern.subfilesr
-00003490: f001 0000 5809 0000 0075 726c 6775 6172  ....X....urlguar
-000034a0: 6473 72f1 0100 0058 2000 0000 7265 6669  dsr....X ...refi
-000034b0: 6e65 7279 2e75 6e69 7473 2e70 6174 7465  nery.units.patte
-000034c0: 726e 2e75 726c 6775 6172 6473 72f2 0100  rn.urlguardsr...
-000034d0: 0058 0300 0000 7874 7072 f301 0000 581a  .X....xtpr....X.
-000034e0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-000034f0: 732e 7061 7474 6572 6e2e 7874 7072 f401  s.pattern.xtpr..
-00003500: 0000 5803 0000 0078 7477 72f5 0100 0058  ..X....xtwr....X
-00003510: 1a00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
-00003520: 7473 2e70 6174 7465 726e 2e78 7477 72f6  ts.pattern.xtwr.
-00003530: 0100 0058 0300 0000 6173 6d72 f701 0000  ...X....asmr....
-00003540: 5818 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
-00003550: 6974 732e 7369 6e6b 732e 6173 6d72 f801  its.sinks.asmr..
-00003560: 0000 5804 0000 0064 756d 7072 f901 0000  ..X....dumpr....
-00003570: 5819 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
-00003580: 6974 732e 7369 6e6b 732e 6475 6d70 72fa  its.sinks.dumpr.
-00003590: 0100 0058 0500 0000 6965 6d61 7072 fb01  ...X....iemapr..
-000035a0: 0000 581a 0000 0072 6566 696e 6572 792e  ..X....refinery.
-000035b0: 756e 6974 732e 7369 6e6b 732e 6965 6d61  units.sinks.iema
-000035c0: 7072 fc01 0000 5804 0000 0070 6565 6b72  pr....X....peekr
-000035d0: fd01 0000 5819 0000 0072 6566 696e 6572  ....X....refiner
-000035e0: 792e 756e 6974 732e 7369 6e6b 732e 7065  y.units.sinks.pe
-000035f0: 656b 72fe 0100 0058 0900 0000 7070 6a73  ekr....X....ppjs
-00003600: 6372 6970 7472 ff01 0000 581e 0000 0072  criptr....X....r
-00003610: 6566 696e 6572 792e 756e 6974 732e 7369  efinery.units.si
-00003620: 6e6b 732e 7070 6a73 6372 6970 7472 0002  nks.ppjscriptr..
-00003630: 0000 5806 0000 0070 706a 736f 6e72 0102  ..X....ppjsonr..
-00003640: 0000 581b 0000 0072 6566 696e 6572 792e  ..X....refinery.
-00003650: 756e 6974 732e 7369 6e6b 732e 7070 6a73  units.sinks.ppjs
-00003660: 6f6e 7202 0200 0058 0500 0000 7070 786d  onr....X....ppxm
-00003670: 6c72 0302 0000 581a 0000 0072 6566 696e  lr....X....refin
-00003680: 6572 792e 756e 6974 732e 7369 6e6b 732e  ery.units.sinks.
-00003690: 7070 786d 6c72 0402 0000 5803 0000 0063  ppxmlr....X....c
-000036a0: 6361 7205 0200 0058 1a00 0000 7265 6669  car....X....refi
-000036b0: 6e65 7279 2e75 6e69 7473 2e73 7472 696e  nery.units.strin
-000036c0: 6773 2e63 6361 7206 0200 0058 0300 0000  gs.ccar....X....
-000036d0: 6363 7072 0702 0000 581a 0000 0072 6566  ccpr....X....ref
-000036e0: 696e 6572 792e 756e 6974 732e 7374 7269  inery.units.stri
-000036f0: 6e67 732e 6363 7072 0802 0000 5804 0000  ngs.ccpr....X...
-00003700: 0063 666d 7472 0902 0000 581b 0000 0072  .cfmtr....X....r
-00003710: 6566 696e 6572 792e 756e 6974 732e 7374  efinery.units.st
-00003720: 7269 6e67 732e 6366 6d74 720a 0200 0058  rings.cfmtr....X
-00003730: 0600 0000 636c 6f77 6572 720b 0200 0058  ....clowerr....X
-00003740: 1d00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
-00003750: 7473 2e73 7472 696e 6773 2e63 6c6f 7765  ts.strings.clowe
-00003760: 7272 0c02 0000 5805 0000 0063 7377 6170  rr....X....cswap
-00003770: 720d 0200 0058 1c00 0000 7265 6669 6e65  r....X....refine
-00003780: 7279 2e75 6e69 7473 2e73 7472 696e 6773  ry.units.strings
-00003790: 2e63 7377 6170 720e 0200 0058 0600 0000  .cswapr....X....
-000037a0: 6375 7070 6572 720f 0200 0058 1d00 0000  cupperr....X....
-000037b0: 7265 6669 6e65 7279 2e75 6e69 7473 2e73  refinery.units.s
-000037c0: 7472 696e 6773 2e63 7570 7065 7272 1002  trings.cupperr..
-000037d0: 0000 5803 0000 0072 6570 7211 0200 0058  ..X....repr....X
-000037e0: 1a00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
-000037f0: 7473 2e73 7472 696e 6773 2e72 6570 7212  ts.strings.repr.
-00003800: 0200 0058 0400 0000 7265 706c 7213 0200  ...X....replr...
-00003810: 0058 1b00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
-00003820: 6e69 7473 2e73 7472 696e 6773 2e72 6570  nits.strings.rep
-00003830: 6c72 1402 0000 5804 0000 0073 6e69 7072  lr....X....snipr
-00003840: 1502 0000 581b 0000 0072 6566 696e 6572  ....X....refiner
-00003850: 792e 756e 6974 732e 7374 7269 6e67 732e  y.units.strings.
-00003860: 736e 6970 7216 0200 0058 0700 0000 7374  snipr....X....st
-00003870: 7265 7463 6872 1702 0000 581e 0000 0072  retchr....X....r
-00003880: 6566 696e 6572 792e 756e 6974 732e 7374  efinery.units.st
-00003890: 7269 6e67 732e 7374 7265 7463 6872 1802  rings.stretchr..
-000038a0: 0000 5807 0000 0074 6572 6d66 6974 7219  ..X....termfitr.
-000038b0: 0200 0058 1e00 0000 7265 6669 6e65 7279  ...X....refinery
-000038c0: 2e75 6e69 7473 2e73 7472 696e 6773 2e74  .units.strings.t
-000038d0: 6572 6d66 6974 721a 0200 0058 0400 0000  ermfitr....X....
-000038e0: 7472 696d 721b 0200 0058 1b00 0000 7265  trimr....X....re
-000038f0: 6669 6e65 7279 2e75 6e69 7473 2e73 7472  finery.units.str
-00003900: 696e 6773 2e74 7269 6d72 1c02 0000 752e  ings.trimr....u.
+00003330: 2e64 6566 616e 6772 e401 0000 5809 0000  .defangr....X...
+00003340: 0064 6e73 646f 6d61 696e 72e5 0100 0058  .dnsdomainr....X
+00003350: 2000 0000 7265 6669 6e65 7279 2e75 6e69   ...refinery.uni
+00003360: 7473 2e70 6174 7465 726e 2e64 6e73 646f  ts.pattern.dnsdo
+00003370: 6d61 696e 72e6 0100 0058 0900 0000 6d69  mainr....X....mi
+00003380: 6d65 776f 7264 7372 e701 0000 5820 0000  mewordsr....X ..
+00003390: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+000033a0: 7061 7474 6572 6e2e 6d69 6d65 776f 7264  pattern.mimeword
+000033b0: 7372 e801 0000 5807 0000 0072 6573 706c  sr....X....respl
+000033c0: 6974 72e9 0100 0058 1e00 0000 7265 6669  itr....X....refi
+000033d0: 6e65 7279 2e75 6e69 7473 2e70 6174 7465  nery.units.patte
+000033e0: 726e 2e72 6573 706c 6974 72ea 0100 0058  rn.resplitr....X
+000033f0: 0500 0000 7265 7375 6272 eb01 0000 581c  ....resubr....X.
+00003400: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00003410: 732e 7061 7474 6572 6e2e 7265 7375 6272  s.pattern.resubr
+00003420: ec01 0000 5803 0000 0072 6578 72ed 0100  ....X....rexr...
+00003430: 0058 1a00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
+00003440: 6e69 7473 2e70 6174 7465 726e 2e72 6578  nits.pattern.rex
+00003450: 72ee 0100 0058 0600 0000 7374 7275 6374  r....X....struct
+00003460: 72ef 0100 0058 2400 0000 7265 6669 6e65  r....X$...refine
+00003470: 7279 2e75 6e69 7473 2e70 6174 7465 726e  ry.units.pattern
+00003480: 2e73 7472 7563 745f 7061 7273 6572 72f0  .struct_parserr.
+00003490: 0100 0058 0800 0000 7375 6266 696c 6573  ...X....subfiles
+000034a0: 72f1 0100 0058 1f00 0000 7265 6669 6e65  r....X....refine
+000034b0: 7279 2e75 6e69 7473 2e70 6174 7465 726e  ry.units.pattern
+000034c0: 2e73 7562 6669 6c65 7372 f201 0000 5809  .subfilesr....X.
+000034d0: 0000 0075 726c 6775 6172 6473 72f3 0100  ...urlguardsr...
+000034e0: 0058 2000 0000 7265 6669 6e65 7279 2e75  .X ...refinery.u
+000034f0: 6e69 7473 2e70 6174 7465 726e 2e75 726c  nits.pattern.url
+00003500: 6775 6172 6473 72f4 0100 0058 0300 0000  guardsr....X....
+00003510: 7874 7072 f501 0000 581a 0000 0072 6566  xtpr....X....ref
+00003520: 696e 6572 792e 756e 6974 732e 7061 7474  inery.units.patt
+00003530: 6572 6e2e 7874 7072 f601 0000 5803 0000  ern.xtpr....X...
+00003540: 0078 7477 72f7 0100 0058 1a00 0000 7265  .xtwr....X....re
+00003550: 6669 6e65 7279 2e75 6e69 7473 2e70 6174  finery.units.pat
+00003560: 7465 726e 2e78 7477 72f8 0100 0058 0300  tern.xtwr....X..
+00003570: 0000 6173 6d72 f901 0000 5818 0000 0072  ..asmr....X....r
+00003580: 6566 696e 6572 792e 756e 6974 732e 7369  efinery.units.si
+00003590: 6e6b 732e 6173 6d72 fa01 0000 5804 0000  nks.asmr....X...
+000035a0: 0064 756d 7072 fb01 0000 5819 0000 0072  .dumpr....X....r
+000035b0: 6566 696e 6572 792e 756e 6974 732e 7369  efinery.units.si
+000035c0: 6e6b 732e 6475 6d70 72fc 0100 0058 0500  nks.dumpr....X..
+000035d0: 0000 6965 6d61 7072 fd01 0000 581a 0000  ..iemapr....X...
+000035e0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+000035f0: 7369 6e6b 732e 6965 6d61 7072 fe01 0000  sinks.iemapr....
+00003600: 5804 0000 0070 6565 6b72 ff01 0000 5819  X....peekr....X.
+00003610: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00003620: 732e 7369 6e6b 732e 7065 656b 7200 0200  s.sinks.peekr...
+00003630: 0058 0900 0000 7070 6a73 6372 6970 7472  .X....ppjscriptr
+00003640: 0102 0000 581e 0000 0072 6566 696e 6572  ....X....refiner
+00003650: 792e 756e 6974 732e 7369 6e6b 732e 7070  y.units.sinks.pp
+00003660: 6a73 6372 6970 7472 0202 0000 5806 0000  jscriptr....X...
+00003670: 0070 706a 736f 6e72 0302 0000 581b 0000  .ppjsonr....X...
+00003680: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00003690: 7369 6e6b 732e 7070 6a73 6f6e 7204 0200  sinks.ppjsonr...
+000036a0: 0058 0500 0000 7070 786d 6c72 0502 0000  .X....ppxmlr....
+000036b0: 581a 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
+000036c0: 6974 732e 7369 6e6b 732e 7070 786d 6c72  its.sinks.ppxmlr
+000036d0: 0602 0000 5803 0000 0063 6361 7207 0200  ....X....ccar...
+000036e0: 0058 1a00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
+000036f0: 6e69 7473 2e73 7472 696e 6773 2e63 6361  nits.strings.cca
+00003700: 7208 0200 0058 0300 0000 6363 7072 0902  r....X....ccpr..
+00003710: 0000 581a 0000 0072 6566 696e 6572 792e  ..X....refinery.
+00003720: 756e 6974 732e 7374 7269 6e67 732e 6363  units.strings.cc
+00003730: 7072 0a02 0000 5804 0000 0063 666d 7472  pr....X....cfmtr
+00003740: 0b02 0000 581b 0000 0072 6566 696e 6572  ....X....refiner
+00003750: 792e 756e 6974 732e 7374 7269 6e67 732e  y.units.strings.
+00003760: 6366 6d74 720c 0200 0058 0600 0000 636c  cfmtr....X....cl
+00003770: 6f77 6572 720d 0200 0058 1d00 0000 7265  owerr....X....re
+00003780: 6669 6e65 7279 2e75 6e69 7473 2e73 7472  finery.units.str
+00003790: 696e 6773 2e63 6c6f 7765 7272 0e02 0000  ings.clowerr....
+000037a0: 5805 0000 0063 7377 6170 720f 0200 0058  X....cswapr....X
+000037b0: 1c00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
+000037c0: 7473 2e73 7472 696e 6773 2e63 7377 6170  ts.strings.cswap
+000037d0: 7210 0200 0058 0600 0000 6375 7070 6572  r....X....cupper
+000037e0: 7211 0200 0058 1d00 0000 7265 6669 6e65  r....X....refine
+000037f0: 7279 2e75 6e69 7473 2e73 7472 696e 6773  ry.units.strings
+00003800: 2e63 7570 7065 7272 1202 0000 5803 0000  .cupperr....X...
+00003810: 0072 6570 7213 0200 0058 1a00 0000 7265  .repr....X....re
+00003820: 6669 6e65 7279 2e75 6e69 7473 2e73 7472  finery.units.str
+00003830: 696e 6773 2e72 6570 7214 0200 0058 0400  ings.repr....X..
+00003840: 0000 7265 706c 7215 0200 0058 1b00 0000  ..replr....X....
+00003850: 7265 6669 6e65 7279 2e75 6e69 7473 2e73  refinery.units.s
+00003860: 7472 696e 6773 2e72 6570 6c72 1602 0000  trings.replr....
+00003870: 5804 0000 0073 6e69 7072 1702 0000 581b  X....snipr....X.
+00003880: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00003890: 732e 7374 7269 6e67 732e 736e 6970 7218  s.strings.snipr.
+000038a0: 0200 0058 0700 0000 7374 7265 7463 6872  ...X....stretchr
+000038b0: 1902 0000 581e 0000 0072 6566 696e 6572  ....X....refiner
+000038c0: 792e 756e 6974 732e 7374 7269 6e67 732e  y.units.strings.
+000038d0: 7374 7265 7463 6872 1a02 0000 5807 0000  stretchr....X...
+000038e0: 0074 6572 6d66 6974 721b 0200 0058 1e00  .termfitr....X..
+000038f0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+00003900: 2e73 7472 696e 6773 2e74 6572 6d66 6974  .strings.termfit
+00003910: 721c 0200 0058 0400 0000 7472 696d 721d  r....X....trimr.
+00003920: 0200 0058 1b00 0000 7265 6669 6e65 7279  ...X....refinery
+00003930: 2e75 6e69 7473 2e73 7472 696e 6773 2e74  .units.strings.t
+00003940: 7269 6d72 1e02 0000 752e                 rimr....u.
```

### Comparing `binary-refinery-0.6.2/refinery/__init__.py` & `binary-refinery-0.6.3/refinery/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 1. `refinery.lib.frame`: framing syntax for working on lists of binary chunks
 2. `refinery.lib.argformats`: the multibin syntax for refinery arguments
 3. `refinery.lib.meta`: defining and using metadata variables within frames
 4. `refinery.units`: writing custom units, add command-line arguments, and how to use refinery
    units within Python code.
 """
-__version__ = '0.6.2'
+__version__ = '0.6.3'
 __distribution__ = 'binary-refinery'
 
 from typing import Dict, List, Optional, Type
 from importlib import resources
 from datetime import datetime
 
 import pickle
```

### Comparing `binary-refinery-0.6.2/refinery/data/rich.json` & `binary-refinery-0.6.3/refinery/data/rich.json`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/explore.py` & `binary-refinery-0.6.3/refinery/explore.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/argformats.py` & `binary-refinery-0.6.3/refinery/lib/argformats.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/argparser.py` & `binary-refinery-0.6.3/refinery/lib/argparser.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/chunks.py` & `binary-refinery-0.6.3/refinery/lib/chunks.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/crypto.py` & `binary-refinery-0.6.3/refinery/lib/crypto.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/decompression.py` & `binary-refinery-0.6.3/refinery/lib/decompression.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/decorators.py` & `binary-refinery-0.6.3/refinery/lib/decorators.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/deobfuscation.py` & `binary-refinery-0.6.3/refinery/lib/deobfuscation.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/dex.py` & `binary-refinery-0.6.3/refinery/lib/dex.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/dotnet/deserialize.py` & `binary-refinery-0.6.3/refinery/lib/dotnet/deserialize.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/dotnet/header.py` & `binary-refinery-0.6.3/refinery/lib/dotnet/header.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/dotnet/resources.py` & `binary-refinery-0.6.3/refinery/lib/dotnet/resources.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/dotnet/types.py` & `binary-refinery-0.6.3/refinery/lib/dotnet/types.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/environment.py` & `binary-refinery-0.6.3/refinery/lib/environment.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/executable.py` & `binary-refinery-0.6.3/refinery/lib/executable.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/frame.py` & `binary-refinery-0.6.3/refinery/lib/frame.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/inline.py` & `binary-refinery-0.6.3/refinery/lib/inline.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/java.py` & `binary-refinery-0.6.3/refinery/lib/java.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/json.py` & `binary-refinery-0.6.3/refinery/lib/json.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/loader.py` & `binary-refinery-0.6.3/refinery/lib/loader.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/magic.py` & `binary-refinery-0.6.3/refinery/lib/magic.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/meta.py` & `binary-refinery-0.6.3/refinery/lib/meta.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/mime.py` & `binary-refinery-0.6.3/refinery/lib/mime.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/mscrypto.py` & `binary-refinery-0.6.3/refinery/lib/mscrypto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Microsoft Crypto API structures
 """
 import enum
 
-from Crypto.PublicKey import RSA
-from Crypto.Math.Numbers import Integer
+from Cryptodome.PublicKey import RSA
+from Cryptodome.Math.Numbers import Integer
 
 from refinery.lib.structures import Struct, StructReader
 
 
 class _ENUM(enum.IntEnum):
     def __str__(self): return self.name
     def __repr__(self): return self.name
```

### Comparing `binary-refinery-0.6.2/refinery/lib/murmur.py` & `binary-refinery-0.6.3/refinery/lib/murmur.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/patterns/__init__.py` & `binary-refinery-0.6.3/refinery/lib/patterns/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -193,14 +193,17 @@
 _pattern_vbaint = R'(?:&[bB][01]+|&[hH][0-9a-fA-F]+|&[oO][0-7]*|[-+]?(?:[1-9][0-9]*|0))(?=\b|$)'
 _pattern_string = R'''(?:"(?:[^"\\\r\n]|\\[^\r\n])*"|'(?:[^'\\\r\n]|\\[^\r\n])*')'''
 _pattern_string_multiline = R'''(?:"(?:[^"\\]|\\.)*"|'(?:[^'\\]|\\.)*')'''
 _pattern_urlenc_coarse = R'''(?:%[0-9a-fA-F]{2}|[0-9a-zA-Z\-\._~\?!$&=:\/#\[\]@'\(\)\*\+,;])+'''
 _pattern_urlenc = R'''(?:%[0-9a-fA-F]{2}|[0-9a-zA-Z\-\._~\?!$&=])+'''
 _pattern_urlenc_narrow = R'''(?:%[0-9a-fA-F]{2})+'''
 
+_pattern_json = R'''[\[\{](?:"(?:[^"\\\r\n]|\\[^\r\n])*"(?:\s*[:,])?|(?:none|true|false|%s|%s|\]|\})(?:\s*,)?|[,\]\}\[\{\s]+)*[\]\}]''' % (
+    _pattern_integer, _pattern_float)
+
 _pattern_wshenc = R'''#@~\^[ -~]{6}==(?:.*?)[ -~]{6}==\^#~@'''
 
 _part_url_credentials = (
     R'(?:(?P<url_username>[^"\'\s\x00-\x20\x7E-\xFF]{1,256})?'
     R'(?::(?P<url_password>[^"\'\s\x00-\x20\x7E-\xFF]{0,256})?)?@)?'
 )
 _prefix_serrated_url = R'(?P<url_scheme>(?P<url_protocol>[a-zA-Z]{2,20}:)?\/\/)' + _part_url_credentials
@@ -262,14 +265,19 @@
     'formats',
     'indicators',
     'wallets',
     'defanged'
 ]
 
 
+class checks(PatternEnum):
+    json = pattern(_pattern_json)
+    "Data that consists of JSON-like tokens; cannot detect actual JSON data."
+
+
 class formats(PatternEnum):
     """
     An enumeration of patterns for certain formats.
     """
     integer = pattern(_pattern_integer)
     "Integer expressions"
     float = pattern(_pattern_float)
@@ -302,19 +310,21 @@
     "Sequences of alphabetic characters"
     wshenc = pattern(_pattern_wshenc)
     "Encoded Windows Scripting Host Scripts (JS/VBS)"
     alphanumeric = alphabet(R'[a-zA-Z0-9]')
     "Sequences of alpha-numeric characters"
     b32 = pattern('[A-Z2-7]+|[a-z2-7+]')
     "Base32 encoded strings"
-    b64 = alphabet(R'(?:[-\w\+/]{4})', postfix=R'(?:(?:[-\w\+/]{2,3})={0,3})?')
+    b64 = alphabet(R'(?:[0-9a-zA-Z\+/]{4})', postfix=R'(?:(?:[0-9a-zA-Z\+/]{2,3})={0,3})?')
     "Base64 encoded strings"
+    b64any = alphabet(R'(?:[-\w\+/]{4})', postfix=R'(?:(?:[-\w\+/]{2,3})={0,3})?')
+    "Both URL-safe and normal Base64 alphabets."
     b64space = alphabet(R'[-\s\w\+/]', postfix=R'(?:={0,3})?')
     "Base64 encoded strings, separated by whitespace"
-    b64url = alphabet(R'[0-9a-zA-Z\_\-]{4}', postfix=R'(?:[0-9a-zA-Z\_\-]{2,3}={0,3})?')
+    b64url = alphabet(R'[-\w]{4}', postfix=R'(?:[-\w]{2,3}={0,3})?')
     "Base64 encoded strings using URL-safe alphabet"
     hex = alphabet(R'[0-9a-fA-F]{2}')
     "Hexadecimal strings"
     uppercase_hex = alphabet(R'[0-9A-F]{2}')
     "Uppercase hexadecimal strings"
     utf8 = pattern(_pattern_utf8)
     "A sequence of bytes that can be decoded as UTF8."
@@ -334,24 +344,35 @@
 
     @classmethod
     def from_dashname(cls, key):
         return getattr(cls, key.replace('-', '_'))
 
 
 class wallets(PatternEnum):
-    LTC = pattern("[LM3][a-km-zA-HJ-NP-Z1-9]{26,33}")
-    DASH = pattern("X[1-9A-HJ-NP-Za-km-z]{33}")
-    XMR = pattern("4[0-9AB][1-9A-HJ-NP-Za-km-z]{90,120}")
+    ADA = pattern("addr1[a-z0-9]+")
+    ATOM = pattern("cosmos[-\\w\\.]{10,}")
+    BCH = pattern("(bitcoincash:)?(q|p)[a-z0-9]{41}|(BITCOINCASH:)?(Q|P)[A-Z0-9]{41}")
     BTC = pattern("[13][a-km-zA-HJ-NP-Z1-9]{25,34}")
     BTCP = pattern("5[HJK][1-9A-Za-z][^OIl]{48}")
+    DASH = pattern("X[1-9A-HJ-NP-Za-km-z]{33}")
+    DOGE = pattern("D{1}[5-9A-HJ-NP-U]{1}[1-9A-HJ-NP-Za-km-z]{32}")
+    DOT = pattern("1[0-9a-zA-Z]{47}")
     ETH = pattern("0x[a-fA-F0-9]{40}")
+    IOTA = pattern("iota[a-z0-9]{10,}")
+    LSK = pattern("[0-9]{19}L")
+    LTC = pattern("[LM3][a-km-zA-HJ-NP-Z1-9]{26,33}")
+    NEO = pattern("N[0-9a-zA-Z]{33}")
+    ONE = pattern("(?:bnb|one)1[a-z0-9]{38}")
+    ONT = pattern("A[0-9a-zA-Z]{33}")
+    RONIN = pattern("ronin:[a-fA-F0-9]{40}")
+    TERRA = pattern("terra1[a-z0-9]{38}")
+    XEM = pattern("N[A-Za-z0-9]{4,7}-[A-Za-z0-9]{4,7}-[A-Za-z0-9]{4,7}-[A-Za-z0-9]{4,7}-[A-Za-z0-9]{4,7}-[A-Za-z0-9]{4,7}-[A-Za-z0-9]{4,7}")
+    XLM = pattern("G[0-9A-Z]{40,60}")
+    XMR = pattern("4[0-9AB][1-9A-HJ-NP-Za-km-z]{90,120}")
     XRP = pattern("r[0-9a-zA-Z]{24,34}")
-    NEO = pattern("A[0-9a-zA-Z]{33}")
-    BCH = pattern("(bitcoincash:)?(q|p)[a-z0-9]{41}|(BITCOINCASH:)?(Q|P)[A-Z0-9]{41}")
-    DOGE = pattern("D{1}[5-9A-HJ-NP-U]{1}[1-9A-HJ-NP-Za-km-z]{32}")
 
 
 class indicators(PatternEnum):
     """
     An enumeration of patterns for indicators.
     """
     domain = pattern(_pattern_serrated_domain)
```

### Comparing `binary-refinery-0.6.2/refinery/lib/patterns/tlds.py` & `binary-refinery-0.6.3/refinery/lib/patterns/tlds.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/powershell.py` & `binary-refinery-0.6.3/refinery/lib/powershell.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/ripemd128.py` & `binary-refinery-0.6.3/refinery/lib/ripemd128.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/serpent.py` & `binary-refinery-0.6.3/refinery/lib/serpent.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/structures.py` & `binary-refinery-0.6.3/refinery/lib/structures.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/suffixtree.py` & `binary-refinery-0.6.3/refinery/lib/suffixtree.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/thirdparty/acefile.py` & `binary-refinery-0.6.3/refinery/lib/thirdparty/acefile.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/thirdparty/batch_interpreter.py` & `binary-refinery-0.6.3/refinery/lib/thirdparty/batch_interpreter.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/thirdparty/pcode2code.py` & `binary-refinery-0.6.3/refinery/lib/thirdparty/pcode2code.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/thirdparty/xxhash.py` & `binary-refinery-0.6.3/refinery/lib/thirdparty/xxhash.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/tools.py` & `binary-refinery-0.6.3/refinery/lib/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             last = True
         yield last, item
 
 
 def get_terminal_size(default=0):
     """
     Returns the size of the currently attached terminal. If the environment variable
-    `REFINERY_TERMSIZE` is set to an integer value, it takes prescedence. If the width
+    `REFINERY_TERM_SIZE` is set to an integer value, it takes prescedence. If the width
     of the terminal cannot be determined of if the width is less than 8 characters,
     the function returns zero.
     """
     from refinery.lib.environment import environment
     ev_terminal_size = environment.term_size.value
     if ev_terminal_size > 0:
         return ev_terminal_size
```

### Comparing `binary-refinery-0.6.2/refinery/lib/types.py` & `binary-refinery-0.6.3/refinery/lib/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Exports two singletons `refinery.lib.types.INF` and `refinery.lib.types.AST`.
 Used by `refinery.units.pattern.PatternExtractorBase` as the default values
 for certain command line arguments.
 """
-from typing import Union, Tuple, Type, Dict, Any
+from typing import Union, Tuple, Type, Dict, Any, Optional, List
 
 __all__ = ['INF', 'AST', 'Singleton', 'ByteStr']
 
 
 ByteStr = Union[bytes, bytearray, memoryview]
 
+JSON = Optional[Union[str, int, float, bool, Type[None], Dict[str, 'JSON'], List['JSON']]]
+JSONDict = Dict[str, JSON]
+
 
 class Singleton(type):
     """
     A metaclass that can be used to define singleton classes.
     """
 
     def __new__(meta, name: str, bases: Tuple[Type, ...], namespace: Dict[str, Any]):
```

### Comparing `binary-refinery-0.6.2/refinery/lib/vfs.py` & `binary-refinery-0.6.3/refinery/lib/vfs.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/lib/xml.py` & `binary-refinery-0.6.3/refinery/lib/xml.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/__init__.py` & `binary-refinery-0.6.3/refinery/units/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,17 +217,18 @@
         self.rest = rest
 
     def __str__(self):
         return self.message
 
 
 class RefineryImportMissing(ImportError):
-    def __init__(self, *dependencies: str):
+    def __init__(self, missing: str, *dependencies: str):
         super().__init__()
         import shlex
+        self.missing = missing
         self.install = ' '.join(shlex.quote(dist) for dist in dependencies)
         self.dependencies = dependencies
 
 
 class RefineryCriticalException(RuntimeError):
     """
     If this exception is thrown, processing of the entire input stream
@@ -1145,16 +1146,16 @@
 
             def __get__(self, unit: Optional[Type[Unit]], tp: Optional[Type[Executable]] = None):
                 if self.module is not None:
                     return self.module
                 try:
                     self.module = module = self.fget()
                 except ImportError as E:
-                    args = unit.optional_dependencies or (self.dependency,)
-                    raise RefineryImportMissing(*args) from E
+                    args = unit.optional_dependencies or ()
+                    raise RefineryImportMissing(self.dependency, *args) from E
                 except Exception as E:
                     raise AttributeError(F'module import for distribution "{distribution}" failed: {E!s}')
                 else:
                     return module
 
         return Requirement
 
@@ -1235,15 +1236,15 @@
             raise exception
         elif isinstance(exception, VariableMissing):
             self.log_warn('critical error:', exception.args[0])
             abort_execution = True
         elif isinstance(exception, GeneratorExit):
             raise exception
         elif isinstance(exception, RefineryImportMissing):
-            self.log_fail(F'dependencies missing; install {exception.install}')
+            self.log_fail(F'dependency {exception.missing} is missing; run pip install {exception.install}')
         else:
             try:
                 explanation = exception.args[0]
             except (AttributeError, IndexError):
                 explanation = exception
             if not isinstance(explanation, str):
                 explanation = exception
```

### Comparing `binary-refinery-0.6.2/refinery/units/blockwise/__init__.py` & `binary-refinery-0.6.3/refinery/units/blockwise/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/blockwise/alu.py` & `binary-refinery-0.6.3/refinery/units/blockwise/alu.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/blockwise/bitrev.py` & `binary-refinery-0.6.3/refinery/units/blockwise/bitrev.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/blockwise/byteswap.py` & `binary-refinery-0.6.3/refinery/units/blockwise/byteswap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/blockwise/map.py` & `binary-refinery-0.6.3/refinery/units/blockwise/map.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/blockwise/pack.py` & `binary-refinery-0.6.3/refinery/units/blockwise/pack.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/blockwise/rev.py` & `binary-refinery-0.6.3/refinery/units/blockwise/rev.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/blockwise/terminate.py` & `binary-refinery-0.6.3/refinery/units/blockwise/terminate.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/blockwise/xor.py` & `binary-refinery-0.6.3/refinery/units/blockwise/xor.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Form the exclusive or of the input data with the given argument.
     """
     def _fastblock(self, data):
         try:
             return super()._fastblock(data)
         except FastBlockError as E:
             try:
-                from Crypto.Util.strxor import strxor
+                from Cryptodome.Util.strxor import strxor
             except ModuleNotFoundError:
                 raise E
             else:
                 from itertools import islice, cycle
                 take = len(data) // self.args.blocksize + 1
                 argb = self.unchunk(islice(cycle(x & self.fmask for x in self.args.argument[0]), take))
                 return strxor(data, argb[:len(data)])
```

### Comparing `binary-refinery-0.6.2/refinery/units/compression/ap.py` & `binary-refinery-0.6.3/refinery/units/compression/ap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/compression/blz.py` & `binary-refinery-0.6.3/refinery/units/compression/blz.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/compression/bz2.py` & `binary-refinery-0.6.3/refinery/units/compression/bz2.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/compression/decompress.py` & `binary-refinery-0.6.3/refinery/units/compression/decompress.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/compression/jcalg.py` & `binary-refinery-0.6.3/refinery/units/compression/jcalg.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/compression/lz.py` & `binary-refinery-0.6.3/refinery/units/compression/lz.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/compression/lz4.py` & `binary-refinery-0.6.3/refinery/units/compression/lz4.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/compression/lzf.py` & `binary-refinery-0.6.3/refinery/units/compression/lzf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/compression/lzg.py` & `binary-refinery-0.6.3/refinery/units/compression/lzg.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/compression/lzip.py` & `binary-refinery-0.6.3/refinery/units/compression/lzip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/compression/lzjb.py` & `binary-refinery-0.6.3/refinery/units/compression/lzjb.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/compression/lznt1.py` & `binary-refinery-0.6.3/refinery/units/compression/lznt1.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/compression/lzo.py` & `binary-refinery-0.6.3/refinery/units/compression/lzo.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/compression/mscf.py` & `binary-refinery-0.6.3/refinery/units/compression/mscf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/compression/qlz.py` & `binary-refinery-0.6.3/refinery/units/compression/qlz.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/compression/szdd.py` & `binary-refinery-0.6.3/refinery/units/compression/szdd.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/compression/zl.py` & `binary-refinery-0.6.3/refinery/units/compression/zl.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/cipher/__init__.py` & `binary-refinery-0.6.3/refinery/units/crypto/cipher/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,25 +148,25 @@
         return self.args.padding
 
     def reverse(self, data: ByteString) -> ByteString:
         padding = self._default_padding()
         if padding is not None:
             self.log_info('padding method:', padding)
             if padding in PADDINGS_LIB:
-                from Crypto.Util.Padding import pad
+                from Cryptodome.Util.Padding import pad
                 data = pad(data, self.block_size, padding)
         return super().reverse(data)
 
     def process(self, data: ByteString) -> ByteString:
         padding = self._default_padding()
         result = super().process(data)
         if padding is None:
             return result
 
-        from Crypto.Util.Padding import unpad
+        from Cryptodome.Util.Padding import unpad
         padding = [padding, *(p for p in PADDINGS_LIB if p != padding)]
 
         for p in padding:
             if p == PADDING_NONE:
                 return result
             try:
                 unpadded = unpad(result, self.block_size, p.lower())
@@ -311,15 +311,15 @@
         return provider.key_size.fget(self)
 
     def _new_cipher(self, **optionals) -> CipherInterface:
         mode = self.args.mode.name
         if mode != 'ECB':
             iv = bytes(self.iv)
             if mode == 'CTR' and len(iv) == self.block_size:
-                from Crypto.Util import Counter
+                from Cryptodome.Util import Counter
                 counter = Counter.new(self.block_size * 8,
                     initial_value=int.from_bytes(iv, 'big'))
                 optionals['counter'] = counter
             elif mode in ('CCM', 'EAX', 'GCM', 'SIV', 'OCB', 'CTR'):
                 if mode in ('CCM', 'EAX', 'GCM', 'OCB'):
                     ml = self.args.mac_len
                     if ml > 0:
```

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/cipher/camellia.py` & `binary-refinery-0.6.3/refinery/units/crypto/cipher/camellia.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/cipher/chacha.py` & `binary-refinery-0.6.3/refinery/units/crypto/cipher/chacha.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-from Crypto.Cipher import ChaCha20
+from Cryptodome.Cipher import ChaCha20
 from typing import List, Iterable
 
 from refinery.units.crypto.cipher.salsa import LatinCipher
 from refinery.units.crypto.cipher import LatinCipherUnit, LatinCipherStandardUnit
 from refinery.lib.crypto import rotl32, PyCryptoFactoryWrapper
```

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/cipher/gost.py` & `binary-refinery-0.6.3/refinery/units/crypto/cipher/gost.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/cipher/hc128.py` & `binary-refinery-0.6.3/refinery/units/crypto/cipher/hc128.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/cipher/isaac.py` & `binary-refinery-0.6.3/refinery/units/crypto/cipher/isaac.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/cipher/rabbit.py` & `binary-refinery-0.6.3/refinery/units/crypto/cipher/rabbit.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/cipher/rc2.py` & `binary-refinery-0.6.3/refinery/units/crypto/cipher/rc2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-from Crypto.Cipher import ARC2
+from Cryptodome.Cipher import ARC2
 
 from refinery.lib.crypto import PyCryptoFactoryWrapper
 from refinery.units.crypto.cipher import StandardBlockCipherUnit, CipherInterface
 
 
 class rc2(StandardBlockCipherUnit, cipher=PyCryptoFactoryWrapper(ARC2)):
     """
```

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/cipher/rc4mod.py` & `binary-refinery-0.6.3/refinery/units/crypto/cipher/rc4mod.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/cipher/rc5.py` & `binary-refinery-0.6.3/refinery/units/crypto/cipher/rc5.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/cipher/rc6.py` & `binary-refinery-0.6.3/refinery/units/crypto/cipher/rc6.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/cipher/rijndael.py` & `binary-refinery-0.6.3/refinery/units/crypto/cipher/rijndael.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/cipher/rncrypt.py` & `binary-refinery-0.6.3/refinery/units/crypto/cipher/rncrypt.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,18 +33,18 @@
 RNCryptor is Copyright (C) 2013-2016 Rob Napier, Yan Kalchevskiy, Brant Young.
 """
 from refinery.units import Unit
 
 import hashlib
 import hmac
 
-from Crypto import Random
-from Crypto.Cipher import AES
-from Crypto.Protocol import KDF
-from Crypto.Util.Padding import unpad, pad
+from Cryptodome import Random
+from Cryptodome.Cipher import AES
+from Cryptodome.Protocol import KDF
+from Cryptodome.Util.Padding import unpad, pad
 
 
 class rncrypt(Unit):
     """
     Implements encryption and decryption using the RNCryptor specification.
     See also: https://github.com/RNCryptor
     """
```

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/cipher/rot.py` & `binary-refinery-0.6.3/refinery/units/crypto/cipher/rot.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/cipher/rsa.py` & `binary-refinery-0.6.3/refinery/units/crypto/cipher/rsa.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from refinery.lib.tools import splitchunks
 from refinery.lib.mscrypto import BCRYPT_RSAKEY_BLOB, CRYPTOKEY, TYPES
 from refinery.lib.xml import ForgivingParse
 
 from base64 import b64decode, b16decode
 from contextlib import suppress
 from enum import IntEnum
-from Crypto.Random import get_random_bytes
-from Crypto.Cipher import PKCS1_OAEP
-from Crypto.PublicKey import RSA
-from Crypto.Util import number
+from Cryptodome.Random import get_random_bytes
+from Cryptodome.Cipher import PKCS1_OAEP
+from Cryptodome.PublicKey import RSA
+from Cryptodome.Util import number
 
 
 def normalize_rsa_key(key: bytes, force_public=False):
     try:
         mod, colon, exp = key.partition(B':')
         if colon == B':':
             mod = number.bytes_to_long(b16decode(mod, casefold=True))
```

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/cipher/rsakey.py` & `binary-refinery-0.6.3/refinery/units/crypto/cipher/rsakey.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import json
 import textwrap
 
 from refinery.units import Arg, Unit
 from refinery.lib.json import flattened
 from refinery.units.crypto.cipher.rsa import normalize_rsa_key
 
-from Crypto.Util.asn1 import DerSequence
-from Crypto.Util import number
+from Cryptodome.Util.asn1 import DerSequence
+from Cryptodome.Util import number
 
 
 class RSAFormat(str, enum.Enum):
     PEM = 'PEM'
     DER = 'DER'
     XKMS = 'XKMS'
     TEXT = 'TEXT'
```

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/cipher/salsa.py` & `binary-refinery-0.6.3/refinery/units/crypto/cipher/salsa.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 import struct
 
-from Crypto.Cipher import Salsa20
+from Cryptodome.Cipher import Salsa20
 from abc import ABC, abstractmethod
 from typing import List, ByteString, Optional, Iterable
 
 from refinery.units.crypto.cipher import LatinCipherUnit, LatinCipherStandardUnit
 from refinery.lib.crypto import rotl32, PyCryptoFactoryWrapper
```

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/cipher/seal.py` & `binary-refinery-0.6.3/refinery/units/crypto/cipher/seal.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/cipher/secstr.py` & `binary-refinery-0.6.3/refinery/units/crypto/cipher/secstr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 import base64
 
-from Crypto.Cipher import AES
-from Crypto.Random import urandom
-from Crypto.Util.Padding import pad, unpad
+from Cryptodome.Cipher import AES
+from Cryptodome.Random import urandom
+from Cryptodome.Util.Padding import pad, unpad
 
 from refinery.units import Arg, Unit
 
 
 class secstr(Unit):
     """
     Implements the AES-based encryption scheme used by the PowerShell commands
```

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/cipher/serpent.py` & `binary-refinery-0.6.3/refinery/units/crypto/cipher/serpent.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/cipher/tea.py` & `binary-refinery-0.6.3/refinery/units/crypto/cipher/tea.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/cipher/vigenere.py` & `binary-refinery-0.6.3/refinery/units/crypto/cipher/vigenere.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/cipher/xtea.py` & `binary-refinery-0.6.3/refinery/units/crypto/cipher/xtea.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/cipher/xxtea.py` & `binary-refinery-0.6.3/refinery/units/crypto/cipher/xxtea.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/hash/__init__.py` & `binary-refinery-0.6.3/refinery/units/crypto/hash/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/hash/checksums.py` & `binary-refinery-0.6.3/refinery/units/crypto/hash/checksums.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/hash/cryptographic.py` & `binary-refinery-0.6.3/refinery/units/crypto/hash/cryptographic.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 
 
 class md4(HashUnit):
     """
     Returns the MD4 hash of the input data.
     """
     def _algorithm(self, data):
-        from Crypto.Hash import MD4
+        from Cryptodome.Hash import MD4
         return MD4.new(data)
 
 
 class md2(HashUnit):
     """
     Returns the MD2 hash of the input data.
     """
     def _algorithm(self, data):
-        from Crypto.Hash import MD2
+        from Cryptodome.Hash import MD2
         return MD2.new(data)
 
 
 class md5(HashUnit):
     """
     Returns the MD5 hash of the input data.
     """
@@ -107,15 +107,15 @@
 
 
 class ripemd160(HashUnit):
     """
     Returns the RIPEMD-160 hash of the input data.
     """
     def _algorithm(self, data):
-        from Crypto.Hash import RIPEMD160
+        from Cryptodome.Hash import RIPEMD160
         return RIPEMD160.new(data)
 
 
 class ripemd128(HashUnit):
     """
     Returns the RIPEMD-128 hash of the input data.
     """
```

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/hash/imphash.py` & `binary-refinery-0.6.3/refinery/units/crypto/hash/imphash.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/hash/murmur.py` & `binary-refinery-0.6.3/refinery/units/crypto/hash/murmur.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/hash/xxhash.py` & `binary-refinery-0.6.3/refinery/units/crypto/hash/xxhash.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/keyderive/CryptDeriveKey.py` & `binary-refinery-0.6.3/refinery/units/crypto/keyderive/CryptDeriveKey.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/keyderive/DESDerive.py` & `binary-refinery-0.6.3/refinery/units/crypto/keyderive/DESDerive.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,16 +13,16 @@
     converts a string to an 8 byte DES key with odd byte parity, per FIPS
     specification. This is not a modern key derivation function.
     """
     def __init__(self, size: Arg(help='The number of bytes to generate, default is the maximum of 8.') = 8):
         super().__init__(size=size, salt=None)
 
     def process(self, password):
-        from Crypto.Cipher import DES
-        from Crypto.Util.strxor import strxor
+        from Cryptodome.Cipher import DES
+        from Cryptodome.Util.strxor import strxor
 
         key = bytearray(8)
 
         for i, j in enumerate(password):
             if ((i % 16) < 8):
                 key[i % 8] ^= (j << 1) & 0xFF
             else:
```

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/keyderive/PasswordDeriveBytes.py` & `binary-refinery-0.6.3/refinery/units/crypto/keyderive/PasswordDeriveBytes.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/keyderive/__init__.py` & `binary-refinery-0.6.3/refinery/units/crypto/keyderive/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,12 +48,12 @@
         hash: Arg.Option(choices=HASH, metavar='hash',
             help='Specify one of these algorithms (default is {default}): {choices}') = None,
         iter: Arg.Number(metavar='iter', help='Number of iterations; default is {default}.') = None,
         **kw
     ):
         if hash is not None:
             name = Arg.AsOption(hash, HASH).value
-            hash = importlib.import_module(F'Crypto.Hash.{name}')
+            hash = importlib.import_module(F'Cryptodome.Hash.{name}')
         return super().__init__(salt=salt, size=size, iter=iter, hash=hash, **kw)
 
     @property
     def hash(self): return self.args.hash
```

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/keyderive/kblob.py` & `binary-refinery-0.6.3/refinery/units/crypto/keyderive/kblob.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/keyderive/pbkdf1.py` & `binary-refinery-0.6.3/refinery/units/crypto/keyderive/pbkdf1.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,11 +7,11 @@
     """PBKDF1 Key derivation"""
 
     @Arg('salt', help='Salt for the derivation; default are 8 null bytes.')
     def __init__(self, size, salt=bytes(8), iter=1000, hash='SHA1'):
         self.superinit(super(), **vars())
 
     def process(self, data):
-        from Crypto.Protocol.KDF import PBKDF1
+        from Cryptodome.Protocol.KDF import PBKDF1
         return multidecode(data, lambda pwd: (
             PBKDF1(pwd, self.args.salt, dkLen=self.args.size, count=self.args.iter, hashAlgo=self.hash)
         ))
```

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/keyderive/pbkdf2.py` & `binary-refinery-0.6.3/refinery/units/crypto/keyderive/pbkdf2.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     binaries.
     """
 
     def __init__(self, size, salt, iter=1000, hash='SHA1'):
         self.superinit(super(), **vars())
 
     def process(self, data: ByteStr):
-        from Crypto.Protocol.KDF import PBKDF2
+        from Cryptodome.Protocol.KDF import PBKDF2
         return multidecode(data, partial(
             PBKDF2,
             salt=self.args.salt,
             dkLen=self.args.size,
             hmac_hash_module=self.hash,
             count=self.args.iter
         ))
```

### Comparing `binary-refinery-0.6.2/refinery/units/crypto/keyderive/unixcrypt.py` & `binary-refinery-0.6.3/refinery/units/crypto/keyderive/unixcrypt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/encoding/atbash.py` & `binary-refinery-0.6.3/refinery/units/encoding/atbash.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/encoding/b32.py` & `binary-refinery-0.6.3/refinery/units/encoding/b32.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/encoding/b64.py` & `binary-refinery-0.6.3/refinery/units/encoding/b64.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/encoding/base.py` & `binary-refinery-0.6.3/refinery/units/encoding/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,16 +94,18 @@
                     index += 1
             self.log_info(F'stripped {len(data)-index} invalid digits from input data')
             del data[index:]
         if len(alphabet) <= len(_DEFAULT_ALPHABET):
             defaults = _DEFAULT_ALPHABET[:base]
             if alphabet != defaults:
                 self.log_info('translating input data to a default alphabet for faster conversion')
-                data = data.translate(bytes.maketrans(alphabet, defaults))
-            result = int(data, self.args.base)
+                data_translated = data.translate(bytes.maketrans(alphabet, defaults))
+                result = int(data_translated, base)
+            else:
+                result = int(data, base)
         elif len(alphabet) == 64:
             import base64
             _b64_alphabet = _LARGER_ALPHABETS[64]
             if alphabet != _b64_alphabet:
                 data = data.translate(bytes.maketrans(alphabet, _b64_alphabet))
             return base64.b64decode(data + b'===', validate=self.args.strict_digits)
         elif len(alphabet) == 85:
```

### Comparing `binary-refinery-0.6.2/refinery/units/encoding/esc.py` & `binary-refinery-0.6.3/refinery/units/encoding/esc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/encoding/hex.py` & `binary-refinery-0.6.3/refinery/units/encoding/hex.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/encoding/netbios.py` & `binary-refinery-0.6.3/refinery/units/encoding/netbios.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/encoding/ps1str.py` & `binary-refinery-0.6.3/refinery/units/encoding/ps1str.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/encoding/recode.py` & `binary-refinery-0.6.3/refinery/units/encoding/recode.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/encoding/url.py` & `binary-refinery-0.6.3/refinery/units/encoding/url.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/encoding/uuenc.py` & `binary-refinery-0.6.3/refinery/units/encoding/uuenc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/encoding/wshenc.py` & `binary-refinery-0.6.3/refinery/units/encoding/wshenc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/__init__.py` & `binary-refinery-0.6.3/refinery/units/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/a3x.py` & `binary-refinery-0.6.3/refinery/units/formats/a3x.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/archive/__init__.py` & `binary-refinery-0.6.3/refinery/units/formats/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/archive/xt.py` & `binary-refinery-0.6.3/refinery/units/formats/archive/xt.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,40 +20,44 @@
         yield xtpdf
         from refinery.units.formats.archive.xtasar import xtasar
         yield xtasar
         from refinery.units.formats.office.xtrtf import xtrtf
         yield xtrtf
         from refinery.units.formats.archive.xtnsis import xtnsis
         yield xtnsis
-        from refinery.units.formats.archive.xtzip import xtzip
-        yield xtzip
-        from refinery.units.formats.archive.xt7z import xt7z
-        yield xt7z
+        from refinery.units.formats.archive.xtnode import xtnode
+        yield xtnode
         from refinery.units.formats.archive.xtace import xtace
         yield xtace
         from refinery.units.formats.archive.xtcab import xtcab
         yield xtcab
         from refinery.units.formats.archive.xtcpio import xtcpio
         yield xtcpio
         from refinery.units.formats.archive.xtiso import xtiso
         yield xtiso
         from refinery.units.formats.archive.xtpyi import xtpyi
         yield xtpyi
         from refinery.units.formats.archive.xttar import xttar
         yield xttar
-        from refinery.units.formats.office.xtdoc import xtdoc
-        yield xtdoc
         from refinery.units.formats.archive.xtiss import xtiss
         yield xtiss
+        from refinery.units.formats.archive.xtzip import xtzip
+        yield xtzip
+        from refinery.units.formats.archive.xt7z import xt7z
+        yield xt7z
+        from refinery.units.formats.office.xtdoc import xtdoc
+        yield xtdoc
+        from refinery.units.formats.json import xtjson
+        yield xtjson
         from refinery.units.formats.exe.vsect import vsect
         yield vsect
 
     def unpack(self, data):
         fallback: List[Type[ArchiveUnit]] = []
-        errors = []
+        errors = {}
         pos_args = self.args.paths
         key_args = dict(
             list=self.args.list,
             path=self.args.path,
             date=self.args.date,
             join_path=self.args.join,
             drop_path=self.args.drop,
@@ -69,48 +73,54 @@
             def __init__(self, handler: Type[ArchiveUnit], fallback: bool):
                 self.success = False
                 self.handler = handler
                 self.fallback = fallback
 
             def __iter__(self):
                 handler = self.handler
-                verdict = True if self.fallback else handler.handles(data)
-                if verdict is True:
+                if self.fallback:
+                    verdict = True
+                else:
+                    verdict = handler.handles(data)
+                if verdict is False:
+                    self.unit.log_info(F'handler {handler.name} cannot handle this data')
+                elif verdict is True:
                     try:
                         unit = handler(*pos_args, **key_args)
                     except TypeError as error:
                         self.unit.log_debug(F'handler {handler.name} failed: {error!s}')
                         return
                     if not self.fallback:
                         self.unit.log_info(F'handler {handler.name} can handle this input data')
                     try:
                         yield from unit.unpack(data)
                     except Exception as E:
                         if not self.fallback:
-                            errors.append(E)
+                            errors[handler.name] = E
                         self.unit.log_info(F'unpacking with {handler.name} failed: {E!s}')
                         return
                     else:
                         self.success = True
                         return
-                if verdict is None:
+                elif verdict is None:
                     fallback.append(handler)
 
         for handler in self._handlers():
             self._custom_path_separator = handler._custom_path_separator
             it = unpacker(handler, fallback=False)
             yield from it
             if it.success:
                 return
 
-        self.log_debug(F'fallback order: {list(fallback)}')
+        self.log_debug('fallback order:', lambda: ', '.join(h.name for h in fallback))
 
         for handler in fallback:
             it = unpacker(handler, fallback=True)
             yield from it
             if it.success:
                 return
 
-        if len(errors) == 1:
-            raise errors[0]
-
-        raise ValueError(F'Input data did not match any known archive format ({len(errors)} errors occurred).')
+        if not errors:
+            raise ValueError('input data did not match any known archive format')
+        for name, error in errors.items():
+            self.log_info(F'error when trying to unpack with {name}', error)
+        raise ValueError('failed to unpack with all known methods')
```

### Comparing `binary-refinery-0.6.2/refinery/units/formats/archive/xt7z.py` & `binary-refinery-0.6.3/refinery/units/formats/archive/xt7z.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/archive/xtace.py` & `binary-refinery-0.6.3/refinery/units/formats/archive/xtace.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/archive/xtasar.py` & `binary-refinery-0.6.3/refinery/units/formats/archive/xtasar.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/archive/xtcab.py` & `binary-refinery-0.6.3/refinery/units/formats/archive/xtcab.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/archive/xtcpio.py` & `binary-refinery-0.6.3/refinery/units/formats/archive/xtcpio.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/archive/xtiso.py` & `binary-refinery-0.6.3/refinery/units/formats/archive/xtiso.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/archive/xtiss.py` & `binary-refinery-0.6.3/refinery/units/formats/archive/xtiss.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/archive/xtnsis.py` & `binary-refinery-0.6.3/refinery/units/formats/archive/xtnsis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1237,8 +1237,8 @@
 
         for item in arc.header.items:
             yield self._pack(item.path, item.mtime, lambda i=item: arc._extract_item_data(i))
         yield self._pack('setup.nsis', None, arc.script.encode(self.codec))
 
     @classmethod
     def handles(cls, data: bytearray) -> bool:
-        return cls._find_archive_offset(data, flawmax=1) is not None
+        return any(magic in data for magic in NSArchive.MAGICS)
```

### Comparing `binary-refinery-0.6.2/refinery/units/formats/archive/xtpyi.py` & `binary-refinery-0.6.3/refinery/units/formats/archive/xtpyi.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from importlib.util import MAGIC_NUMBER
 
 from refinery.units.formats.archive import Arg, ArchiveUnit
 from refinery.units.pattern.carve import carve
 from refinery.lib.structures import EOF, MemoryFile, StreamDetour, Struct, StructReader
 from refinery.lib.tools import NoLogging
 
-from Crypto.Cipher import AES
+from Cryptodome.Cipher import AES
 
 
 class Unmarshal(enum.IntEnum):
     No = 0
     Yes = 1
     YesAndDecompile = 2
```

### Comparing `binary-refinery-0.6.2/refinery/units/formats/archive/xttar.py` & `binary-refinery-0.6.3/refinery/units/formats/archive/xttar.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/archive/xtzip.py` & `binary-refinery-0.6.3/refinery/units/formats/archive/xtzip.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 from typing import Optional
 
 from datetime import datetime
-from zipfile import ZipInfo, ZipFile
 
 from refinery.units.formats.archive import ArchiveUnit
 from refinery.lib.structures import MemoryFile
 from refinery.units.pattern.carve_zip import ZipEndOfCentralDirectory, carve_zip
 
 ZIP_FILENAME_UTF8_FLAG = 0x800
 
@@ -17,32 +16,46 @@
     Extract files from a Zip archive.
     """
     @ArchiveUnit.Requires('chardet', optional=True)
     def _chardet():
         import chardet
         return chardet
 
+    @ArchiveUnit.Requires('pyzipper', optional=True)
+    def _pyzipper():
+        import pyzipper
+        return pyzipper
+
     def unpack(self, data: bytearray):
         if not data.startswith(B'PK'):
             self.log_info('input file is not a zip file, attempting to carve one')
             data = next(data | carve_zip)
             offset = data['offset']
             self.log_debug(F'carved a zip file from 0x{offset:X}')
 
+        from zipfile import ZipFile, ZipInfo
+
         password = bytes(self.args.pwd)
         archive = ZipFile(MemoryFile(data))
 
         if password:
             archive.setpassword(password)
         else:
-            def password_invalid(pwd: Optional[str]):
+            def password_invalid(pwd: Optional[str], pyzipper=False):
+                nonlocal archive
                 if pwd is not None:
                     archive.setpassword(pwd.encode(self.codec))
                 try:
                     archive.testzip()
+                except NotImplementedError:
+                    if pyzipper:
+                        raise
+                    self.log_debug('compression method unsupported, switching to pyzipper')
+                    archive = self._pyzipper.AESZipFile(MemoryFile(data))
+                    return password_invalid(pwd, True)
                 except RuntimeError as E:
                     if 'password' not in str(E):
                         raise
                     return True
                 else:
                     if pwd:
                         self.log_debug('using password:', pwd)
```

### Comparing `binary-refinery-0.6.2/refinery/units/formats/bat.py` & `binary-refinery-0.6.3/refinery/units/formats/bat.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/csv.py` & `binary-refinery-0.6.3/refinery/units/formats/csv.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/deserialize_php.py` & `binary-refinery-0.6.3/refinery/units/formats/deserialize_php.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/email.py` & `binary-refinery-0.6.3/refinery/units/formats/email.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             jh[key].append(mw(''.join(t.lstrip() for t in value.splitlines(False))))
         jh = {k: v[0] if len(v) == 1 else [t for t in v if t] for k, v in jh.items()}
         yield UnpackResult('headers.txt',
             lambda h=head: '\n'.join(F'{k}: {v}' for k, v in h).encode(self.codec))
         yield UnpackResult('headers.json',
             lambda jsn=jh: json.dumps(jsn, indent=4).encode(self.codec))
 
-    @PathExtractorUnit.Requires('extract_msg', optional=False)
+    @PathExtractorUnit.Requires('extract-msg', optional=False)
     def _extract_msg():
         import extract_msg.message
         return extract_msg.message
 
     def _get_parts_outlook(self, data):
         def ensure_bytes(data):
             return data if isinstance(data, bytes) else data.encode(self.codec)
```

### Comparing `binary-refinery-0.6.2/refinery/units/formats/evtx.py` & `binary-refinery-0.6.3/refinery/units/formats/evtx.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/exe/vaddr.py` & `binary-refinery-0.6.3/refinery/units/formats/exe/vaddr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/exe/vmemref.py` & `binary-refinery-0.6.3/refinery/units/formats/exe/vmemref.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/exe/vsect.py` & `binary-refinery-0.6.3/refinery/units/formats/exe/vsect.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/exe/vsnip.py` & `binary-refinery-0.6.3/refinery/units/formats/exe/vsnip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/exe/vstack.py` & `binary-refinery-0.6.3/refinery/units/formats/exe/vstack.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/hexload.py` & `binary-refinery-0.6.3/refinery/units/formats/hexload.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/html.py` & `binary-refinery-0.6.3/refinery/units/formats/html.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/httpresponse.py` & `binary-refinery-0.6.3/refinery/units/formats/httpresponse.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/ifps.py` & `binary-refinery-0.6.3/refinery/units/formats/ifps.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/ifpsstr.py` & `binary-refinery-0.6.3/refinery/units/formats/ifpsstr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/java/deserialize.py` & `binary-refinery-0.6.3/refinery/units/formats/java/deserialize.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/java/jvdasm.py` & `binary-refinery-0.6.3/refinery/units/formats/java/jvdasm.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/json.py` & `binary-refinery-0.6.3/refinery/units/formats/json.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 from __future__ import annotations
-from typing import Union
+from typing import Union, Optional
 
 import json
 
 from refinery.units.formats import PathExtractorUnit, UnpackResult, Unit
 from refinery.lib.meta import is_valid_variable_name
+from refinery.lib.patterns import checks
 
 
 class xtjson(PathExtractorUnit):
     """
     Extract values from a JSON document.
     """
     _custom_path_separator = '.'
@@ -35,14 +36,18 @@
                 if isinstance(item, (list, dict)):
                     dumped = json.dumps(item, indent=4)
                 else:
                     dumped = str(item)
                 return dumped.encode(self.codec)
             yield UnpackResult(path, extract, type=typename)
 
+    @classmethod
+    def handles(self, data: bytearray) -> Optional[bool]:
+        return bool(checks.json.fullmatch(data))
+
 
 class xj0(Unit):
     """
     Extracts a single field from a JSON document at depth 0. By default, the unit applies a heuristic to
     extract remaining fields as metadata: String values are extracted only if they do not exceed 80
     characters in length and do not contain any line breaks. Floating-point, integer, boolean values, and
     lists of the latter are also extracted.
```

### Comparing `binary-refinery-0.6.2/refinery/units/formats/lnk.py` & `binary-refinery-0.6.3/refinery/units/formats/lnk.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/msgpack.py` & `binary-refinery-0.6.3/refinery/units/formats/msgpack.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/office/doctxt.py` & `binary-refinery-0.6.3/refinery/units/formats/office/doctxt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/office/officecrypt.py` & `binary-refinery-0.6.3/refinery/units/formats/office/officecrypt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/office/vbapc.py` & `binary-refinery-0.6.3/refinery/units/formats/office/vbapc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/office/vbastr.py` & `binary-refinery-0.6.3/refinery/units/formats/office/vbastr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/office/xlmdeobf.py` & `binary-refinery-0.6.3/refinery/units/formats/office/xlmdeobf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/office/xlxtr.py` & `binary-refinery-0.6.3/refinery/units/formats/office/xlxtr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/office/xtdoc.py` & `binary-refinery-0.6.3/refinery/units/formats/office/xtdoc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/office/xtone.py` & `binary-refinery-0.6.3/refinery/units/formats/office/xtone.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/office/xtrtf.py` & `binary-refinery-0.6.3/refinery/units/formats/office/xtrtf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/office/xtvba.py` & `binary-refinery-0.6.3/refinery/units/formats/office/xtvba.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/pcap.py` & `binary-refinery-0.6.3/refinery/units/formats/pcap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/pcap_http.py` & `binary-refinery-0.6.3/refinery/units/formats/pcap_http.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/pdf.py` & `binary-refinery-0.6.3/refinery/units/formats/pdf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/pe/__init__.py` & `binary-refinery-0.6.3/refinery/units/formats/pe/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/__init__.py` & `binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/dncfx.py` & `binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/dncfx.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 import struct
 import re
 
-from Crypto.Util.strxor import strxor
+from Cryptodome.Util.strxor import strxor
 
 from refinery.units import Unit
 from refinery.units.compression.lz import lzma
 from refinery.lib import chunks
 from refinery.lib.dotnet.header import DotNetHeader, StreamReader, StringPrimitive, UInt32, ParserEOF
```

### Comparing `binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/dnds.py` & `binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/dnds.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/dnfields.py` & `binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/dnfields.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/dnhdr.py` & `binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/dnhdr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/dnmr.py` & `binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/dnmr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/dnrc.py` & `binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/dnrc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/dnstr.py` & `binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/dnstr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/pe/pemeta.py` & `binary-refinery-0.6.3/refinery/units/formats/pe/pemeta.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/pe/peoverlay.py` & `binary-refinery-0.6.3/refinery/units/formats/pe/peoverlay.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/pe/perc.py` & `binary-refinery-0.6.3/refinery/units/formats/pe/perc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/pe/pesig.py` & `binary-refinery-0.6.3/refinery/units/formats/pe/pesig.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/pe/pestrip.py` & `binary-refinery-0.6.3/refinery/units/formats/pe/pestrip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/pkcs7.py` & `binary-refinery-0.6.3/refinery/units/formats/pkcs7.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/pkcs7sig.py` & `binary-refinery-0.6.3/refinery/units/formats/pkcs7sig.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/stego.py` & `binary-refinery-0.6.3/refinery/units/formats/stego.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/winreg.py` & `binary-refinery-0.6.3/refinery/units/formats/winreg.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/formats/xml.py` & `binary-refinery-0.6.3/refinery/units/formats/xml.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/malware/n40.py` & `binary-refinery-0.6.3/refinery/units/malware/n40.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/meta/__init__.py` & `binary-refinery-0.6.3/refinery/units/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/meta/chop.py` & `binary-refinery-0.6.3/refinery/units/meta/chop.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/meta/cm.py` & `binary-refinery-0.6.3/refinery/units/meta/cm.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/meta/cull.py` & `binary-refinery-0.6.3/refinery/units/meta/cull.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/meta/dedup.py` & `binary-refinery-0.6.3/refinery/units/meta/dedup.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/meta/eat.py` & `binary-refinery-0.6.3/refinery/units/meta/eat.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/meta/ef.py` & `binary-refinery-0.6.3/refinery/units/meta/ef.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/meta/emit.py` & `binary-refinery-0.6.3/refinery/units/meta/emit.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/meta/group.py` & `binary-refinery-0.6.3/refinery/units/meta/group.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/meta/groupby.py` & `binary-refinery-0.6.3/refinery/units/meta/groupby.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/meta/iff.py` & `binary-refinery-0.6.3/refinery/units/meta/iff.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/meta/iffp.py` & `binary-refinery-0.6.3/refinery/units/meta/iffp.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/meta/iffs.py` & `binary-refinery-0.6.3/refinery/units/meta/iffs.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/meta/iffx.py` & `binary-refinery-0.6.3/refinery/units/meta/iffx.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/meta/max.py` & `binary-refinery-0.6.3/refinery/units/meta/max.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+from typing import Iterable
 from refinery.units import Arg, Unit, Chunk
 from refinery.lib.meta import metavars
 
 
 class max_(Unit):
     """
     Picks the maximum of all elements in the current `refinery.lib.frame`.
@@ -11,32 +12,37 @@
 
     def __init__(
         self,
         key: Arg('key', type=str, help='A meta variable expression to sort by instead of sorting the content.') = None,
     ):
         super().__init__(key=key)
 
-    def filter(self, chunks):
+    def filter(self, chunks: Iterable[Chunk]):
         def get_value(chunk: Chunk):
             if key is None:
                 return chunk
             return metavars(chunk).get(key)
 
         key = self.args.key
         it = iter(chunks)
 
-        try:
-            max_chunk = next(it)
-        except StopIteration:
-            return None
+        for max_chunk in it:
+            if not max_chunk.visible:
+                yield max_chunk
+            else:
+                max_index = 0
+                max_value = get_value(max_chunk)
+                break
         else:
-            max_index = 0
-            max_value = get_value(max_chunk)
+            return
 
         for index, chunk in enumerate(chunks, 1):
+            if not chunk.visible:
+                yield chunk
+                continue
             value = get_value(chunk)
             try:
                 is_max = value > max_value
             except TypeError:
                 if max_value is None:
                     self.log_info(
                         F'Discarding chunk {max_index} in favor of {index} because {key} was not '
```

### Comparing `binary-refinery-0.6.2/refinery/units/meta/min.py` & `binary-refinery-0.6.3/refinery/units/meta/min.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+from typing import Iterable
 from refinery.units import Arg, Unit, Chunk
 from refinery.lib.meta import metavars
 
 
 class min_(Unit):
     """
     Picks the minimum of all elements in the current `refinery.lib.frame`.
@@ -11,32 +12,37 @@
 
     def __init__(
         self,
         key: Arg('key', type=str, help='A meta variable expression to sort by instead of sorting the content.') = None,
     ):
         super().__init__(key=key)
 
-    def filter(self, chunks):
+    def filter(self, chunks: Iterable[Chunk]):
         def get_value(chunk: Chunk):
             if key is None:
                 return chunk
             return metavars(chunk).get(key)
 
         key = self.args.key
         it = iter(chunks)
 
-        try:
-            min_chunk = next(it)
-        except StopIteration:
-            return None
+        for min_chunk in it:
+            if not min_chunk.visible:
+                yield min_chunk
+            else:
+                min_index = 0
+                min_value = get_value(min_chunk)
+                break
         else:
-            min_index = 0
-            min_value = get_value(min_chunk)
+            return
 
         for index, chunk in enumerate(chunks, 1):
+            if not chunk.visible:
+                yield chunk
+                continue
             value = get_value(chunk)
             try:
                 is_min = value < min_value
             except TypeError:
                 if min_value is None:
                     self.log_info(
                         F'Discarding chunk {min_index} in favor of {index} because {key} was not '
```

### Comparing `binary-refinery-0.6.2/refinery/units/meta/mvc.py` & `binary-refinery-0.6.3/refinery/units/meta/mvc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/meta/mvg.py` & `binary-refinery-0.6.3/refinery/units/meta/mvg.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/meta/pad.py` & `binary-refinery-0.6.3/refinery/units/meta/pad.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/meta/pick.py` & `binary-refinery-0.6.3/refinery/units/meta/pick.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/meta/pop.py` & `binary-refinery-0.6.3/refinery/units/meta/pop.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/meta/push.py` & `binary-refinery-0.6.3/refinery/units/meta/push.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/meta/put.py` & `binary-refinery-0.6.3/refinery/units/meta/put.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/meta/queue.py` & `binary-refinery-0.6.3/refinery/units/meta/queue.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/meta/reduce.py` & `binary-refinery-0.6.3/refinery/units/meta/reduce.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/meta/scope.py` & `binary-refinery-0.6.3/refinery/units/meta/scope.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/meta/sep.py` & `binary-refinery-0.6.3/refinery/units/meta/sep.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/meta/sorted.py` & `binary-refinery-0.6.3/refinery/units/meta/sorted.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/meta/swap.py` & `binary-refinery-0.6.3/refinery/units/meta/swap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/meta/xfcc.py` & `binary-refinery-0.6.3/refinery/units/meta/xfcc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/misc/autoxor.py` & `binary-refinery-0.6.3/refinery/units/misc/autoxor.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/misc/couple.py` & `binary-refinery-0.6.3/refinery/units/misc/couple.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/misc/datefix.py` & `binary-refinery-0.6.3/refinery/units/misc/datefix.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/misc/drp.py` & `binary-refinery-0.6.3/refinery/units/misc/drp.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/misc/nop.py` & `binary-refinery-0.6.3/refinery/units/misc/nop.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/misc/urlfix.py` & `binary-refinery-0.6.3/refinery/units/misc/urlfix.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/misc/xkey.py` & `binary-refinery-0.6.3/refinery/units/misc/xkey.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/obfuscation/__init__.py` & `binary-refinery-0.6.3/refinery/units/obfuscation/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/obfuscation/js/arrays.py` & `binary-refinery-0.6.3/refinery/units/obfuscation/js/arrays.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/obfuscation/js/getattr.py` & `binary-refinery-0.6.3/refinery/units/obfuscation/js/getattr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/obfuscation/js/tuples.py` & `binary-refinery-0.6.3/refinery/units/obfuscation/js/tuples.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/obfuscation/ps1/__init__.py` & `binary-refinery-0.6.3/refinery/units/obfuscation/ps1/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/obfuscation/ps1/all.py` & `binary-refinery-0.6.3/refinery/units/obfuscation/ps1/all.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/obfuscation/ps1/brackets.py` & `binary-refinery-0.6.3/refinery/units/obfuscation/ps1/brackets.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/obfuscation/ps1/cases.py` & `binary-refinery-0.6.3/refinery/units/obfuscation/ps1/cases.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/obfuscation/ps1/concat.py` & `binary-refinery-0.6.3/refinery/units/obfuscation/ps1/concat.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/obfuscation/ps1/format.py` & `binary-refinery-0.6.3/refinery/units/obfuscation/ps1/format.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/obfuscation/ps1/invoke.py` & `binary-refinery-0.6.3/refinery/units/obfuscation/ps1/invoke.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/obfuscation/ps1/securestring.py` & `binary-refinery-0.6.3/refinery/units/obfuscation/ps1/securestring.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/obfuscation/ps1/stringreplace.py` & `binary-refinery-0.6.3/refinery/units/obfuscation/ps1/stringreplace.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/obfuscation/ps1/typecast.py` & `binary-refinery-0.6.3/refinery/units/obfuscation/ps1/typecast.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/obfuscation/ps1/uncurly.py` & `binary-refinery-0.6.3/refinery/units/obfuscation/ps1/uncurly.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/obfuscation/vba/all.py` & `binary-refinery-0.6.3/refinery/units/obfuscation/vba/all.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/obfuscation/vba/arithmetic.py` & `binary-refinery-0.6.3/refinery/units/obfuscation/vba/arithmetic.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/obfuscation/vba/brackets.py` & `binary-refinery-0.6.3/refinery/units/obfuscation/vba/brackets.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/obfuscation/vba/char.py` & `binary-refinery-0.6.3/refinery/units/obfuscation/vba/char.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/obfuscation/vba/concat.py` & `binary-refinery-0.6.3/refinery/units/obfuscation/vba/concat.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/obfuscation/vba/constants.py` & `binary-refinery-0.6.3/refinery/units/obfuscation/vba/constants.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/obfuscation/vba/dummies.py` & `binary-refinery-0.6.3/refinery/units/obfuscation/vba/dummies.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/obfuscation/vba/stringreplace.py` & `binary-refinery-0.6.3/refinery/units/obfuscation/vba/stringreplace.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/obfuscation/vba/stringreverse.py` & `binary-refinery-0.6.3/refinery/units/obfuscation/vba/stringreverse.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/pattern/__init__.py` & `binary-refinery-0.6.3/refinery/units/pattern/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/pattern/carve.py` & `binary-refinery-0.6.3/refinery/units/pattern/carve.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             decoder = hex()
         elif self.args.format is formats.hexdump:
             from ..formats.hexload import hexload
             decoder = hexload()
         elif self.args.format is formats.intarray:
             from ..blockwise.pack import pack
             decoder = pack()
-        elif self.args.format is formats.b64:
+        elif self.args.format in (formats.b64, formats.b64any, formats.b64space):
             from ..encoding.b64 import b64
             decoder = b64()
         elif self.args.format is formats.b64url:
             from ..encoding.b64 import b64
             decoder = b64(urlsafe=True)
         elif self.args.format is formats.b32:
             from ..encoding.b32 import b32
```

### Comparing `binary-refinery-0.6.2/refinery/units/pattern/carve_7z.py` & `binary-refinery-0.6.3/refinery/units/pattern/carve_7z.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/pattern/carve_lnk.py` & `binary-refinery-0.6.3/refinery/units/pattern/carve_lnk.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/pattern/carve_pe.py` & `binary-refinery-0.6.3/refinery/units/pattern/carve_pe.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/pattern/carve_rtf.py` & `binary-refinery-0.6.3/refinery/units/pattern/carve_rtf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/pattern/carve_xml.py` & `binary-refinery-0.6.3/refinery/units/pattern/carve_xml.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/pattern/carve_zip.py` & `binary-refinery-0.6.3/refinery/units/pattern/carve_zip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/pattern/defang.py` & `binary-refinery-0.6.3/refinery/units/pattern/defang.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/pattern/dnsdomain.py` & `binary-refinery-0.6.3/refinery/units/pattern/dnsdomain.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/pattern/mimewords.py` & `binary-refinery-0.6.3/refinery/units/pattern/mimewords.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/pattern/resplit.py` & `binary-refinery-0.6.3/refinery/units/pattern/resplit.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/pattern/resub.py` & `binary-refinery-0.6.3/refinery/units/pattern/resub.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/pattern/rex.py` & `binary-refinery-0.6.3/refinery/units/pattern/rex.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/pattern/struct_parser.py` & `binary-refinery-0.6.3/refinery/units/pattern/struct_parser.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/pattern/subfiles.py` & `binary-refinery-0.6.3/refinery/units/pattern/subfiles.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/pattern/urlguards.py` & `binary-refinery-0.6.3/refinery/units/pattern/urlguards.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/pattern/xtp.py` & `binary-refinery-0.6.3/refinery/units/pattern/xtp.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/pattern/xtw.py` & `binary-refinery-0.6.3/refinery/units/pattern/xtw.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/sinks/__init__.py` & `binary-refinery-0.6.3/refinery/units/sinks/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/sinks/asm.py` & `binary-refinery-0.6.3/refinery/units/sinks/asm.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/sinks/dump.py` & `binary-refinery-0.6.3/refinery/units/sinks/dump.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/sinks/iemap.py` & `binary-refinery-0.6.3/refinery/units/sinks/iemap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/sinks/peek.py` & `binary-refinery-0.6.3/refinery/units/sinks/peek.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/sinks/ppjscript.py` & `binary-refinery-0.6.3/refinery/units/sinks/ppjscript.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/sinks/ppjson.py` & `binary-refinery-0.6.3/refinery/units/sinks/ppjson.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/sinks/ppxml.py` & `binary-refinery-0.6.3/refinery/units/sinks/ppxml.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/strings/cfmt.py` & `binary-refinery-0.6.3/refinery/units/strings/cfmt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/strings/cswap.py` & `binary-refinery-0.6.3/refinery/units/strings/cswap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/strings/rep.py` & `binary-refinery-0.6.3/refinery/units/strings/rep.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/strings/repl.py` & `binary-refinery-0.6.3/refinery/units/strings/repl.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/strings/snip.py` & `binary-refinery-0.6.3/refinery/units/strings/snip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/strings/stretch.py` & `binary-refinery-0.6.3/refinery/units/strings/stretch.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/strings/termfit.py` & `binary-refinery-0.6.3/refinery/units/strings/termfit.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/refinery/units/strings/trim.py` & `binary-refinery-0.6.3/refinery/units/strings/trim.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.2/setup.py` & `binary-refinery-0.6.3/setup.py`

 * *Files identical despite different names*

