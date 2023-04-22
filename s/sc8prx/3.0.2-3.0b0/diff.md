# Comparing `tmp/sc8prx-3.0.2.tar.gz` & `tmp/sc8prx-3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc8prx-3.0.2.tar", last modified: Sat Apr 22 16:00:15 2023, max compression
+gzip compressed data, was "sc8prx-3.0b0.tar", last modified: Sun Mar 12 13:35:34 2023, max compression
```

## Comparing `sc8prx-3.0.2.tar` & `sc8prx-3.0b0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 16:00:15.557001 sc8prx-3.0.2/
--rw-rw-rw-   0        0        0    35141 2023-04-22 15:50:28.000000 sc8prx-3.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0       38 2023-04-22 15:50:28.000000 sc8prx-3.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1016 2023-04-22 16:00:15.557001 sc8prx-3.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      171 2023-04-22 15:50:28.000000 sc8prx-3.0.2/README.md
--rw-rw-rw-   0        0        0       72 2023-04-22 15:50:28.000000 sc8prx-3.0.2/README.txt
--rw-rw-rw-   0        0        0       81 2023-04-22 15:50:28.000000 sc8prx-3.0.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-22 16:00:15.557001 sc8prx-3.0.2/sc8prx/
--rw-rw-rw-   0        0        0        0 2023-04-22 15:50:28.000000 sc8prx-3.0.2/sc8prx/__init__.py
--rw-rw-rw-   0        0        0     7858 2023-04-22 15:50:28.000000 sc8prx-3.0.2/sc8prx/ffmpeg.py
--rw-rw-rw-   0        0        0     1763 2023-04-22 15:50:28.000000 sc8prx-3.0.2/sc8prx/mpl.py
--rw-rw-rw-   0        0        0     1835 2023-04-22 15:50:28.000000 sc8prx-3.0.2/sc8prx/pil.py
-drwxrwxrwx   0        0        0        0 2023-04-22 16:00:15.557001 sc8prx-3.0.2/sc8prx.egg-info/
--rw-rw-rw-   0        0        0     1016 2023-04-22 16:00:15.000000 sc8prx-3.0.2/sc8prx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-04-22 16:00:15.000000 sc8prx-3.0.2/sc8prx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 16:00:15.000000 sc8prx-3.0.2/sc8prx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-22 16:00:15.000000 sc8prx-3.0.2/sc8prx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      102 2023-04-22 16:00:15.000000 sc8prx-3.0.2/sc8prx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-22 16:00:15.000000 sc8prx-3.0.2/sc8prx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1024 2023-04-22 16:00:15.557001 sc8prx-3.0.2/setup.cfg
--rw-rw-rw-   0        0        0       38 2023-04-22 15:50:28.000000 sc8prx-3.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-12 13:35:34.274443 sc8prx-3.0b0/
+-rw-rw-rw-   0        0        0    35141 2023-03-12 13:26:39.000000 sc8prx-3.0b0/LICENSE.txt
+-rw-rw-rw-   0        0        0       38 2023-03-12 13:26:39.000000 sc8prx-3.0b0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1004 2023-03-12 13:35:34.275453 sc8prx-3.0b0/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-03-12 13:26:39.000000 sc8prx-3.0b0/README.md
+-rw-rw-rw-   0        0        0       72 2023-03-12 13:26:39.000000 sc8prx-3.0b0/README.txt
+-rw-rw-rw-   0        0        0       81 2023-03-12 13:26:39.000000 sc8prx-3.0b0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-03-12 13:35:34.258745 sc8prx-3.0b0/sc8prx/
+-rw-rw-rw-   0        0        0        0 2023-03-12 13:26:39.000000 sc8prx-3.0b0/sc8prx/__init__.py
+-rw-rw-rw-   0        0        0     7801 2023-03-12 13:26:39.000000 sc8prx-3.0b0/sc8prx/ffmpeg.py
+-rw-rw-rw-   0        0        0     1763 2023-03-12 13:26:39.000000 sc8prx-3.0b0/sc8prx/mpl.py
+-rw-rw-rw-   0        0        0     2023 2023-03-12 13:26:39.000000 sc8prx-3.0b0/sc8prx/pil.py
+drwxrwxrwx   0        0        0        0 2023-03-12 13:35:34.274443 sc8prx-3.0b0/sc8prx.egg-info/
+-rw-rw-rw-   0        0        0     1004 2023-03-12 13:35:34.000000 sc8prx-3.0b0/sc8prx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-03-12 13:35:34.000000 sc8prx-3.0b0/sc8prx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-12 13:35:34.000000 sc8prx-3.0b0/sc8prx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-12 13:35:33.000000 sc8prx-3.0b0/sc8prx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      102 2023-03-12 13:35:34.000000 sc8prx-3.0b0/sc8prx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-03-12 13:35:34.000000 sc8prx-3.0b0/sc8prx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1012 2023-03-12 13:35:34.275453 sc8prx-3.0b0/setup.cfg
+-rw-rw-rw-   0        0        0       38 2023-03-12 13:26:39.000000 sc8prx-3.0b0/setup.py
```

### Comparing `sc8prx-3.0.2/LICENSE.txt` & `sc8prx-3.0b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sc8prx-3.0.2/PKG-INFO` & `sc8prx-3.0b0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: sc8prx
-Version: 3.0.2
+Version: 3.0b0
 Summary: Extra features for sc8pr 3
 Home-page: https://dmaccarthy.github.io/sc8pr3/?sc8prx
 Author: D.G. MacCarthy
 Author-email: sc8pr.py@gmail.com
 License: GPLv3
 Keywords: graphics animation sprite gui robotics pygame educational
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: pygame
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Education
 Classifier: Topic :: Games/Entertainment
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # sc8prx
 
-“Extras” for the sc8pr 3 package that have additional dependencies. Please see the [documentation](https://dmaccarthy.github.io/sc8pr/?sc8prx) for details.
+“Extras” for the sc8pr 3 package that have additional dependencies. Please see the [documentation](https://dmaccarthy.github.io/sc8pr3/?sc8prx) for details.
```

### Comparing `sc8prx-3.0.2/sc8prx/ffmpeg.py` & `sc8prx-3.0b0/sc8prx/ffmpeg.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,17 +171,14 @@
 
 
 class Movie(CostumeImage):
 
     @property
     def cycle(self): return False
 
-    @property
-    def meta(self): return self._ffr.meta
-
     def __init__(self, src, skip=0, frames=None, alpha=False, **kwargs):
         self._alpha = alpha
         self._skip = skip
         self._frames = frames
         self._reader = lambda: Reader(src, **kwargs)
         self._size = kwargs.get("size", None)
         self.restart()
```

### Comparing `sc8prx-3.0.2/sc8prx/mpl.py` & `sc8prx-3.0b0/sc8prx/mpl.py`

 * *Files identical despite different names*

### Comparing `sc8prx-3.0.2/sc8prx/pil.py` & `sc8prx-3.0b0/sc8prx/pil.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,14 +23,18 @@
 
 def pil_image(srf, mode=None):
     "Convert surface to PIL.Image"
     srf = surface(srf)
     if mode is None: mode = "RGBA" if hasAlpha(srf) else "RGB"
     return PIL.Image.frombytes(mode, srf.get_size(), pygame.image.tostring(srf, mode))
 
+# def pil_to_surface(pil_img):
+#     "Convert PIL.Image to surface"
+#     return pygame.image.fromstring(pil_img.tobytes(), pil_img.size, pil_img.mode)
+
 
 class Grabber:
     "A class for performing screen captures using PIL.ImageGrab.grab"
 
     def __init__(self, rect=None):
         self.grab = PIL.ImageGrab.grab
         if rect and not isinstance(rect, pygame.Rect):
@@ -44,14 +48,14 @@
         r = self.rect
         if r: return [r.left, r.top, r.right, r.bottom]
 
     @property
     def pil(self): return self.grab(self.bbox)
 
     @property
-    def img(self): return Image(self.srf)
+    def img(self): return Image(pil_to_surface(self.grab(self.bbox)))
 
     @property
     def rgba(self): return self.img.rgba
 
     @property
-    def srf(self): return surface(self.grab(self.bbox))
+    def srf(self): return pil_to_surface(self.grab(self.bbox))
```

### Comparing `sc8prx-3.0.2/sc8prx.egg-info/PKG-INFO` & `sc8prx-3.0b0/sc8prx.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: sc8prx
-Version: 3.0.2
+Version: 3.0b0
 Summary: Extra features for sc8pr 3
 Home-page: https://dmaccarthy.github.io/sc8pr3/?sc8prx
 Author: D.G. MacCarthy
 Author-email: sc8pr.py@gmail.com
 License: GPLv3
 Keywords: graphics animation sprite gui robotics pygame educational
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: pygame
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Education
 Classifier: Topic :: Games/Entertainment
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # sc8prx
 
-“Extras” for the sc8pr 3 package that have additional dependencies. Please see the [documentation](https://dmaccarthy.github.io/sc8pr/?sc8prx) for details.
+“Extras” for the sc8pr 3 package that have additional dependencies. Please see the [documentation](https://dmaccarthy.github.io/sc8pr3/?sc8prx) for details.
```

### Comparing `sc8prx-3.0.2/setup.cfg` & `sc8prx-3.0b0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 6338 7072 780d 0a76 6572 7369   = sc8prx..versi
-00000020: 6f6e 203d 2033 2e30 2e32 0d0a 6175 7468  on = 3.0.2..auth
-00000030: 6f72 203d 2044 2e47 2e20 4d61 6343 6172  or = D.G. MacCar
-00000040: 7468 790d 0a61 7574 686f 725f 656d 6169  thy..author_emai
-00000050: 6c20 3d20 7363 3870 722e 7079 4067 6d61  l = sc8pr.py@gma
-00000060: 696c 2e63 6f6d 0d0a 7572 6c20 3d20 6874  il.com..url = ht
-00000070: 7470 733a 2f2f 646d 6163 6361 7274 6879  tps://dmaccarthy
-00000080: 2e67 6974 6875 622e 696f 2f73 6338 7072  .github.io/sc8pr
-00000090: 332f 3f73 6338 7072 780d 0a64 6573 6372  3/?sc8prx..descr
-000000a0: 6970 7469 6f6e 203d 2045 7874 7261 2066  iption = Extra f
-000000b0: 6561 7475 7265 7320 666f 7220 7363 3870  eatures for sc8p
-000000c0: 7220 330d 0a6c 6f6e 675f 6465 7363 7269  r 3..long_descri
-000000d0: 7074 696f 6e20 3d20 6669 6c65 3a20 5245  ption = file: RE
-000000e0: 4144 4d45 2e6d 640d 0a6c 6f6e 675f 6465  ADME.md..long_de
-000000f0: 7363 7269 7074 696f 6e5f 636f 6e74 656e  scription_conten
-00000100: 745f 7479 7065 203d 2074 6578 742f 6d61  t_type = text/ma
-00000110: 726b 646f 776e 0d0a 6b65 7977 6f72 6473  rkdown..keywords
-00000120: 203d 2067 7261 7068 6963 7320 616e 696d   = graphics anim
-00000130: 6174 696f 6e20 7370 7269 7465 2067 7569  ation sprite gui
-00000140: 2072 6f62 6f74 6963 7320 7079 6761 6d65   robotics pygame
-00000150: 2065 6475 6361 7469 6f6e 616c 0d0a 6c69   educational..li
-00000160: 6365 6e73 6520 3d20 4750 4c76 330d 0a63  cense = GPLv3..c
-00000170: 6c61 7373 6966 6965 7273 203d 200d 0a09  lassifiers = ...
-00000180: 4465 7665 6c6f 706d 656e 7420 5374 6174  Development Stat
-00000190: 7573 203a 3a20 3520 2d20 5072 6f64 7563  us :: 5 - Produc
-000001a0: 7469 6f6e 2f53 7461 626c 650d 0a09 496e  tion/Stable...In
-000001b0: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
-000001c0: 3a3a 2044 6576 656c 6f70 6572 730d 0a09  :: Developers...
-000001d0: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
-000001e0: 6520 3a3a 2045 6475 6361 7469 6f6e 0d0a  e :: Education..
-000001f0: 094c 6963 656e 7365 203a 3a20 4f53 4920  .License :: OSI 
-00000200: 4170 7072 6f76 6564 203a 3a20 474e 5520  Approved :: GNU 
-00000210: 4765 6e65 7261 6c20 5075 626c 6963 204c  General Public L
-00000220: 6963 656e 7365 2076 3320 2847 504c 7633  icense v3 (GPLv3
-00000230: 290d 0a09 5072 6f67 7261 6d6d 696e 6720  )...Programming 
-00000240: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000250: 6f6e 203a 3a20 330d 0a09 546f 7069 6320  on :: 3...Topic 
-00000260: 3a3a 2053 6f66 7477 6172 6520 4465 7665  :: Software Deve
-00000270: 6c6f 706d 656e 7420 3a3a 204c 6962 7261  lopment :: Libra
-00000280: 7269 6573 203a 3a20 7079 6761 6d65 0d0a  ries :: pygame..
-00000290: 0954 6f70 6963 203a 3a20 4d75 6c74 696d  .Topic :: Multim
-000002a0: 6564 6961 203a 3a20 4772 6170 6869 6373  edia :: Graphics
-000002b0: 0d0a 0954 6f70 6963 203a 3a20 4564 7563  ...Topic :: Educ
-000002c0: 6174 696f 6e0d 0a09 546f 7069 6320 3a3a  ation...Topic ::
-000002d0: 2047 616d 6573 2f45 6e74 6572 7461 696e   Games/Entertain
-000002e0: 6d65 6e74 0d0a 0d0a 5b6f 7074 696f 6e73  ment....[options
-000002f0: 5d0d 0a7a 6970 5f73 6166 6520 3d20 4661  ]..zip_safe = Fa
-00000300: 6c73 650d 0a69 6e63 6c75 6465 5f70 6163  lse..include_pac
-00000310: 6b61 6765 5f64 6174 6120 3d20 5472 7565  kage_data = True
-00000320: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
-00000330: 643a 0d0a 696e 7374 616c 6c5f 7265 7175  d:..install_requ
-00000340: 6972 6573 203d 200d 0a09 7363 3870 723d  ires = ...sc8pr=
-00000350: 3d33 2e30 2e32 0d0a 0969 6d61 6765 696f  =3.0.2...imageio
-00000360: 3e3d 322e 382c 3c33 0d0a 0969 6d61 6765  >=2.8,<3...image
-00000370: 696f 2d66 666d 7065 673e 3d30 2e34 2c3c  io-ffmpeg>=0.4,<
-00000380: 310d 0a09 6e75 6d70 793e 3d31 2e32 302c  1...numpy>=1.20,
-00000390: 3c32 0d0a 096d 6174 706c 6f74 6c69 623e  <2...matplotlib>
-000003a0: 3d33 2e30 2c3c 340d 0a09 7069 6c6c 6f77  =3.0,<4...pillow
-000003b0: 3e3d 392e 302c 3c31 300d 0a70 7974 686f  >=9.0,<10..pytho
-000003c0: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-000003d0: 2e37 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  .7....[egg_info]
-000003e0: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-000003f0: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+00000020: 6f6e 203d 2033 2e30 2e62 300d 0a61 7574  on = 3.0.b0..aut
+00000030: 686f 7220 3d20 442e 472e 204d 6163 4361  hor = D.G. MacCa
+00000040: 7274 6879 0d0a 6175 7468 6f72 5f65 6d61  rthy..author_ema
+00000050: 696c 203d 2073 6338 7072 2e70 7940 676d  il = sc8pr.py@gm
+00000060: 6169 6c2e 636f 6d0d 0a75 726c 203d 2068  ail.com..url = h
+00000070: 7474 7073 3a2f 2f64 6d61 6363 6172 7468  ttps://dmaccarth
+00000080: 792e 6769 7468 7562 2e69 6f2f 7363 3870  y.github.io/sc8p
+00000090: 7233 2f3f 7363 3870 7278 0d0a 6465 7363  r3/?sc8prx..desc
+000000a0: 7269 7074 696f 6e20 3d20 4578 7472 6120  ription = Extra 
+000000b0: 6665 6174 7572 6573 2066 6f72 2073 6338  features for sc8
+000000c0: 7072 2033 0d0a 6c6f 6e67 5f64 6573 6372  pr 3..long_descr
+000000d0: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
+000000e0: 4541 444d 452e 6d64 0d0a 6c6f 6e67 5f64  EADME.md..long_d
+000000f0: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
+00000100: 6e74 5f74 7970 6520 3d20 7465 7874 2f6d  nt_type = text/m
+00000110: 6172 6b64 6f77 6e0d 0a6b 6579 776f 7264  arkdown..keyword
+00000120: 7320 3d20 6772 6170 6869 6373 2061 6e69  s = graphics ani
+00000130: 6d61 7469 6f6e 2073 7072 6974 6520 6775  mation sprite gu
+00000140: 6920 726f 626f 7469 6373 2070 7967 616d  i robotics pygam
+00000150: 6520 6564 7563 6174 696f 6e61 6c0d 0a6c  e educational..l
+00000160: 6963 656e 7365 203d 2047 504c 7633 0d0a  icense = GPLv3..
+00000170: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
+00000180: 0944 6576 656c 6f70 6d65 6e74 2053 7461  .Development Sta
+00000190: 7475 7320 3a3a 2034 202d 2042 6574 610d  tus :: 4 - Beta.
+000001a0: 0a09 496e 7465 6e64 6564 2041 7564 6965  ..Intended Audie
+000001b0: 6e63 6520 3a3a 2044 6576 656c 6f70 6572  nce :: Developer
+000001c0: 730d 0a09 496e 7465 6e64 6564 2041 7564  s...Intended Aud
+000001d0: 6965 6e63 6520 3a3a 2045 6475 6361 7469  ience :: Educati
+000001e0: 6f6e 0d0a 094c 6963 656e 7365 203a 3a20  on...License :: 
+000001f0: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
+00000200: 474e 5520 4765 6e65 7261 6c20 5075 626c  GNU General Publ
+00000210: 6963 204c 6963 656e 7365 2076 3320 2847  ic License v3 (G
+00000220: 504c 7633 290d 0a09 5072 6f67 7261 6d6d  PLv3)...Programm
+00000230: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000240: 5079 7468 6f6e 203a 3a20 330d 0a09 546f  Python :: 3...To
+00000250: 7069 6320 3a3a 2053 6f66 7477 6172 6520  pic :: Software 
+00000260: 4465 7665 6c6f 706d 656e 7420 3a3a 204c  Development :: L
+00000270: 6962 7261 7269 6573 203a 3a20 7079 6761  ibraries :: pyga
+00000280: 6d65 0d0a 0954 6f70 6963 203a 3a20 4d75  me...Topic :: Mu
+00000290: 6c74 696d 6564 6961 203a 3a20 4772 6170  ltimedia :: Grap
+000002a0: 6869 6373 0d0a 0954 6f70 6963 203a 3a20  hics...Topic :: 
+000002b0: 4564 7563 6174 696f 6e0d 0a09 546f 7069  Education...Topi
+000002c0: 6320 3a3a 2047 616d 6573 2f45 6e74 6572  c :: Games/Enter
+000002d0: 7461 696e 6d65 6e74 0d0a 0d0a 5b6f 7074  tainment....[opt
+000002e0: 696f 6e73 5d0d 0a7a 6970 5f73 6166 6520  ions]..zip_safe 
+000002f0: 3d20 4661 6c73 650d 0a69 6e63 6c75 6465  = False..include
+00000300: 5f70 6163 6b61 6765 5f64 6174 6120 3d20  _package_data = 
+00000310: 5472 7565 0d0a 7061 636b 6167 6573 203d  True..packages =
+00000320: 2066 696e 643a 0d0a 696e 7374 616c 6c5f   find:..install_
+00000330: 7265 7175 6972 6573 203d 200d 0a09 7363  requires = ...sc
+00000340: 3870 723d 3d33 2e30 6230 0d0a 0969 6d61  8pr==3.0b0...ima
+00000350: 6765 696f 3e3d 322e 382c 3c33 0d0a 0969  geio>=2.8,<3...i
+00000360: 6d61 6765 696f 2d66 666d 7065 673e 3d30  mageio-ffmpeg>=0
+00000370: 2e34 2c3c 310d 0a09 6e75 6d70 793e 3d31  .4,<1...numpy>=1
+00000380: 2e32 302c 3c32 0d0a 096d 6174 706c 6f74  .20,<2...matplot
+00000390: 6c69 623e 3d33 2e30 2c3c 340d 0a09 7069  lib>=3.0,<4...pi
+000003a0: 6c6c 6f77 3e3d 392e 302c 3c31 300d 0a70  llow>=9.0,<10..p
+000003b0: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
+000003c0: 203e 3d33 2e37 0d0a 0d0a 5b65 6767 5f69   >=3.7....[egg_i
+000003d0: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
+000003e0: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
+000003f0: 0d0a 0d0a                                ....
```

