# Comparing `tmp/gpttui-0.2.0.tar.gz` & `tmp/gpttui-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpttui-0.2.0.tar", last modified: Sun Apr 16 03:43:23 2023, max compression
+gzip compressed data, was "gpttui-0.3.0.tar", last modified: Fri Apr 21 22:34:14 2023, max compression
```

## Comparing `gpttui-0.2.0.tar` & `gpttui-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0      123 2023-04-07 23:28:42.202644 gpttui-0.2.0/.gitignore
--rw-r--r--   0        0        0      176 2023-04-11 01:50:25.100205 gpttui-0.2.0/Makefile
--rw-r--r--   0        0        0     2137 2023-04-11 01:50:25.100205 gpttui-0.2.0/README.md
--rw-r--r--   0        0        0      531 2023-04-16 03:42:27.404389 gpttui-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.2.0/src/gpttui/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.2.0/src/gpttui/database/__init__.py
--rw-r--r--   0        0        0     2937 2023-04-11 01:50:25.100205 gpttui-0.2.0/src/gpttui/database/base.py
--rw-r--r--   0        0        0     4103 2023-04-11 01:50:25.100205 gpttui-0.2.0/src/gpttui/database/sqlite.py
--rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.2.0/src/gpttui/models/__init__.py
--rw-r--r--   0        0        0     1851 2023-04-11 01:50:25.100205 gpttui-0.2.0/src/gpttui/models/base.py
--rw-r--r--   0        0        0     3410 2023-04-16 03:42:27.407722 gpttui-0.2.0/src/gpttui/models/openai.py
--rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.2.0/src/gpttui/tui/__init__.py
--rw-r--r--   0        0        0     6271 2023-04-16 03:42:27.407722 gpttui-0.2.0/src/gpttui/tui/app.py
--rw-r--r--   0        0        0     2644 2023-04-16 03:42:27.407722 gpttui-0.2.0/src/gpttui/tui/config.py
--rw-r--r--   0        0        0     2391 2023-04-11 01:50:25.103539 gpttui-0.2.0/src/gpttui/tui/front.py
--rw-r--r--   0        0        0      210 2023-04-11 01:50:25.103539 gpttui-0.2.0/src/gpttui/tui/main.py
--rwxr-xr-x   0        0        0      140 2023-04-11 01:50:25.103539 gpttui-0.2.0/test/main.sh
--rw-r--r--   0        0        0     1983 2023-04-11 01:50:25.103539 gpttui-0.2.0/test/test_db.py
--rw-r--r--   0        0        0     1582 2023-04-11 01:50:25.103539 gpttui-0.2.0/test/test_model.py
--rw-r--r--   0        0        0      431 1970-01-01 00:00:00.000000 gpttui-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      123 2023-04-07 23:28:42.202644 gpttui-0.3.0/.gitignore
+-rw-r--r--   0        0        0      176 2023-04-11 01:50:25.100205 gpttui-0.3.0/Makefile
+-rw-r--r--   0        0        0     2164 2023-04-21 22:33:55.636511 gpttui-0.3.0/README.md
+-rw-r--r--   0        0        0   999692 2023-04-21 22:33:55.649844 gpttui-0.3.0/docs/img/example.gif
+-rw-r--r--   0        0        0      531 2023-04-21 22:33:55.649844 gpttui-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.3.0/src/gpttui/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.3.0/src/gpttui/database/__init__.py
+-rw-r--r--   0        0        0     2937 2023-04-11 01:50:25.100205 gpttui-0.3.0/src/gpttui/database/base.py
+-rw-r--r--   0        0        0     4103 2023-04-11 01:50:25.100205 gpttui-0.3.0/src/gpttui/database/sqlite.py
+-rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.3.0/src/gpttui/models/__init__.py
+-rw-r--r--   0        0        0     1857 2023-04-21 22:33:55.649844 gpttui-0.3.0/src/gpttui/models/base.py
+-rw-r--r--   0        0        0     3377 2023-04-21 22:33:55.649844 gpttui-0.3.0/src/gpttui/models/openai.py
+-rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.3.0/src/gpttui/tui/__init__.py
+-rw-r--r--   0        0        0     7384 2023-04-21 22:33:55.649844 gpttui-0.3.0/src/gpttui/tui/app.py
+-rw-r--r--   0        0        0     2644 2023-04-21 22:14:51.392110 gpttui-0.3.0/src/gpttui/tui/config.py
+-rw-r--r--   0        0        0     2391 2023-04-11 01:50:25.103539 gpttui-0.3.0/src/gpttui/tui/front.py
+-rw-r--r--   0        0        0      210 2023-04-11 01:50:25.103539 gpttui-0.3.0/src/gpttui/tui/main.py
+-rwxr-xr-x   0        0        0      140 2023-04-11 01:50:25.103539 gpttui-0.3.0/test/main.sh
+-rw-r--r--   0        0        0     1983 2023-04-11 01:50:25.103539 gpttui-0.3.0/test/test_db.py
+-rw-r--r--   0        0        0     1582 2023-04-11 01:50:25.103539 gpttui-0.3.0/test/test_model.py
+-rw-r--r--   0        0        0      431 1970-01-01 00:00:00.000000 gpttui-0.3.0/PKG-INFO
```

### Comparing `gpttui-0.2.0/README.md` & `gpttui-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,134 +1,136 @@
-00000000: 2320 4750 5454 5549 0a0a 5455 4920 746f  # GPTTUI..TUI to
-00000010: 2069 6e74 6572 6163 7420 7769 7468 2067   interact with g
-00000020: 7074 206d 6f64 656c 732e 0a0a 5b21 5b61  pt models...[![a
-00000030: 7363 6969 6361 7374 5d28 6874 7470 733a  sciicast](https:
-00000040: 2f2f 6173 6369 696e 656d 612e 6f72 672f  //asciinema.org/
-00000050: 612f 6e33 4576 6f65 5976 3566 4363 7350  a/n3EvoeYv5fCcsP
-00000060: 3075 5177 3536 5a34 3765 7a2e 7376 6729  0uQw56Z47ez.svg)
-00000070: 5d28 6874 7470 733a 2f2f 6173 6369 696e  ](https://asciin
-00000080: 656d 612e 6f72 672f 612f 6e33 4576 6f65  ema.org/a/n3Evoe
-00000090: 5976 3566 4363 7350 3075 5177 3536 5a34  Yv5fCcsP0uQw56Z4
-000000a0: 3765 7a29 0a0a 6067 7074 7475 6960 2070  7ez)..`gpttui` p
-000000b0: 726f 7669 6465 7320 6120 7465 726d 696e  rovides a termin
-000000c0: 616c 2066 726f 6e74 656e 6420 7468 6174  al frontend that
-000000d0: 2061 6c6c 6f77 7320 7365 7373 696f 6e73   allows sessions
-000000e0: 2028 636f 6e76 6572 7361 7469 6f6e 7329   (conversations)
-000000f0: 2077 6974 6820 4c4c 4d73 2c20 7374 6f72   with LLMs, stor
-00000100: 6573 2061 6c6c 2074 6865 2069 6e66 6f72  es all the infor
-00000110: 6d61 7469 6f6e 2069 6e20 6120 6365 6e74  mation in a cent
-00000120: 7261 6c69 7a65 6420 6461 7461 6261 7365  ralized database
-00000130: 2c20 616e 6420 7072 6f76 6964 6573 2076  , and provides v
-00000140: 692d 6c69 6b65 206b 6579 6269 6e64 696e  i-like keybindin
-00000150: 6773 2e0a 0a3e 202a 2a4e 6f74 652a 2a3a  gs...> **Note**:
-00000160: 2041 7420 7468 6520 6d6f 6d65 6e74 2069   At the moment i
-00000170: 7420 6f6e 6c79 2073 7570 706f 7274 7320  t only supports 
-00000180: 2a2a 4f70 656e 4149 2a2a 206d 6f64 656c  **OpenAI** model
-00000190: 732c 2062 7574 206f 7468 6572 204c 4c4d  s, but other LLM
-000001a0: 7320 6361 6e20 6265 2065 6173 696c 7920  s can be easily 
-000001b0: 696e 7465 6772 6174 6564 2e20 5361 6d65  integrated. Same
-000001c0: 2077 6974 6820 7468 6520 6461 7461 6261   with the databa
-000001d0: 7365 732c 2063 7572 7265 6e74 6c79 2073  ses, currently s
-000001e0: 7570 706f 7274 696e 6720 6073 716c 6974  upporting `sqlit
-000001f0: 6560 2e0a 0a23 2320 496e 7374 616c 6c61  e`...## Installa
-00000200: 7469 6f6e 0a0a 596f 7520 6361 6e20 696e  tion..You can in
-00000210: 7374 616c 6c20 6067 7074 7475 6960 2077  stall `gpttui` w
-00000220: 6974 6820 6070 6970 603a 0a0a 6060 6073  ith `pip`:..```s
-00000230: 680a 7069 7020 696e 7374 616c 6c20 6770  h.pip install gp
-00000240: 7474 7569 0a60 6060 0a0a 2323 2042 6173  ttui.```..## Bas
-00000250: 6963 2043 6f6e 6365 7074 730a 0a2d 2060  ic Concepts..- `
-00000260: 7365 7373 696f 6e60 3a20 6120 636f 6e76  session`: a conv
-00000270: 6572 7361 7469 6f6e 2028 6368 6174 292e  ersation (chat).
-00000280: 0a2d 2060 636f 6e74 6578 7460 3a20 7370  .- `context`: sp
-00000290: 6563 6966 6965 7320 6120 746f 7069 6320  ecifies a topic 
-000002a0: 6f72 2061 2073 7065 6369 616c 697a 6174  or a specializat
-000002b0: 696f 6e20 666f 7220 7468 6520 6173 7369  ion for the assi
-000002c0: 7374 616e 742e 0a2d 2060 7573 6572 603a  stant..- `user`:
-000002d0: 2074 6865 2070 6572 736f 6e20 7468 6174   the person that
-000002e0: 2075 7365 7320 6067 7074 7475 6960 2e0a   uses `gpttui`..
-000002f0: 2d20 6061 7373 6973 7461 6e74 603a 2074  - `assistant`: t
-00000300: 6865 2041 4920 6173 7369 7374 616e 742e  he AI assistant.
-00000310: 0a0a 2323 2055 7361 6765 0a0a 596f 7520  ..## Usage..You 
-00000320: 6361 6e20 6765 7420 6d6f 7265 2069 6e66  can get more inf
-00000330: 6f72 6d61 7469 6f6e 2075 7369 6e67 2074  ormation using t
-00000340: 6865 2068 656c 7020 7061 6765 3a0a 0a60  he help page:..`
-00000350: 6060 7368 0a67 7074 7475 6920 2d2d 6865  ``sh.gpttui --he
-00000360: 6c70 0a60 6060 0a0a 4c69 6b65 7769 7365  lp.```..Likewise
-00000370: 2c20 796f 7520 6361 6e20 6765 7420 6865  , you can get he
-00000380: 6c70 206f 6620 7468 6520 6469 6666 6572  lp of the differ
-00000390: 656e 7420 6672 6f6e 7465 6e64 206f 7074  ent frontend opt
-000003a0: 696f 6e73 2077 6974 6820 7468 6520 666f  ions with the fo
-000003b0: 6c6c 6f77 696e 6720 636f 6d6d 616e 643a  llowing command:
-000003c0: 0a0a 6060 6073 680a 6770 7474 7569 2066  ..```sh.gpttui f
-000003d0: 726f 6e74 202d 2d68 656c 700a 6060 600a  ront --help.```.
-000003e0: 0a46 6f72 2065 7861 6d70 6c65 2c20 746f  .For example, to
-000003f0: 206c 6175 6e63 6820 7468 6520 5455 493a   launch the TUI:
-00000400: 0a0a 6060 6073 680a 6770 7474 7569 205c  ..```sh.gpttui \
-00000410: 0a20 2020 202d 2d64 6174 6162 6173 655f  .    --database_
-00000420: 6b69 6e64 2053 514c 4954 4520 5c0a 2020  kind SQLITE \.  
-00000430: 2020 2d2d 7365 7373 696f 6e20 6669 7273    --session firs
-00000440: 745f 6368 6174 205c 0a20 2020 202d 2d6d  t_chat \.    --m
-00000450: 6f64 656c 5f6b 696e 6420 4f50 454e 4149  odel_kind OPENAI
-00000460: 205c 0a20 2020 202d 2d6d 6f64 656c 5f6e   \.    --model_n
-00000470: 616d 6520 2267 7074 2d33 2e35 2d74 7572  ame "gpt-3.5-tur
-00000480: 626f 2220 5c0a 2020 2020 2d2d 636f 6e74  bo" \.    --cont
-00000490: 6578 7420 2759 6f75 2061 7265 2061 6e20  ext 'You are an 
-000004a0: 6578 7065 7274 2073 6f66 7477 6172 6520  expert software 
-000004b0: 6465 7665 6c6f 7065 7227 0a60 6060 0a0a  developer'.```..
-000004c0: 2323 2320 4f70 656e 4149 0a0a 546f 2075  ### OpenAI..To u
-000004d0: 7365 204f 7065 6e41 4920 6d6f 6465 6c73  se OpenAI models
-000004e0: 2079 6f75 206e 6565 6420 746f 2073 7065   you need to spe
-000004f0: 6369 6679 2074 6865 2066 6f6c 6c6f 7769  cify the followi
-00000500: 6e67 2065 6e76 6972 6f6e 6d65 6e74 2076  ng environment v
-00000510: 6172 6961 626c 6573 3a0a 0a60 6060 7368  ariables:..```sh
-00000520: 0a65 7870 6f72 7420 4f50 454e 4149 5f4f  .export OPENAI_O
-00000530: 5247 3d22 220a 6578 706f 7274 204f 5045  RG="".export OPE
-00000540: 4e41 495f 4150 495f 4b45 593d 2222 0a60  NAI_API_KEY="".`
-00000550: 6060 0a0a 2323 2320 4b65 7962 696e 6469  ``..### Keybindi
-00000560: 6e67 730a 0a60 6770 7474 7569 6020 6861  ngs..`gpttui` ha
-00000570: 7320 7477 6f20 6d6f 6465 733a 0a0a 2d20  s two modes:..- 
-00000580: 604e 4f52 4d41 4c60 3a20 696e 2074 6869  `NORMAL`: in thi
-00000590: 7320 6d6f 6465 2079 6f75 2063 616e 2064  s mode you can d
-000005a0: 6f20 676c 6f62 616c 206f 7065 7261 7469  o global operati
-000005b0: 6f6e 732e 2042 7920 6465 6661 756c 742c  ons. By default,
-000005c0: 2060 4e4f 524d 414c 6020 6d6f 6465 2068   `NORMAL` mode h
-000005d0: 6173 2074 6865 2066 6f6c 6c6f 7769 6e67  as the following
-000005e0: 2062 696e 6469 6e67 733a 0a20 2020 202d   bindings:.    -
-000005f0: 2060 6360 3a20 636c 6561 7220 6d65 7373   `c`: clear mess
-00000600: 6167 6573 2e0a 2020 2020 2d20 6064 603a  ages..    - `d`:
-00000610: 2064 656c 6574 6520 7072 6f6d 7074 2e0a   delete prompt..
-00000620: 2020 2020 2d20 6071 603a 2071 7569 742e      - `q`: quit.
-00000630: 0a20 2020 202d 2060 7960 3a20 7961 6e6b  .    - `y`: yank
-00000640: 2f63 6f70 7920 7468 6520 6c61 7374 206d  /copy the last m
-00000650: 6573 7361 6765 2066 726f 6d20 7468 6520  essage from the 
-00000660: 6173 7369 7374 616e 742e 0a20 2020 202d  assistant..    -
-00000670: 2060 7060 3a20 7061 7374 6520 736f 6d65   `p`: paste some
-00000680: 2074 6578 7420 6672 6f6d 2074 6865 2063   text from the c
-00000690: 6c69 7062 6f61 7264 2069 6e74 6f20 7468  lipboard into th
-000006a0: 6520 7072 6f6d 7074 2e0a 2020 2020 2d20  e prompt..    - 
-000006b0: 6069 603a 2073 7769 7463 6820 746f 2069  `i`: switch to i
-000006c0: 6e73 6572 7420 6d6f 6465 2e0a 0a2d 2060  nsert mode...- `
-000006d0: 494e 5345 5254 603a 2069 6e20 7468 6973  INSERT`: in this
-000006e0: 206d 6f64 6520 796f 7520 6361 6e20 7072   mode you can pr
-000006f0: 6f6d 7074 2074 6578 742e 2042 7920 6465  ompt text. By de
-00000700: 6661 756c 742c 2060 494e 5345 5254 6020  fault, `INSERT` 
-00000710: 6d6f 6465 2068 6173 2074 6865 2066 6f6c  mode has the fol
-00000720: 6c6f 7769 6e67 2062 696e 6469 6e67 733a  lowing bindings:
-00000730: 0a20 2020 202d 2060 6573 6360 3a20 7377  .    - `esc`: sw
-00000740: 6974 6368 2074 6f20 6e6f 726d 616c 206d  itch to normal m
-00000750: 6f64 652e 0a20 2020 202d 2060 656e 7465  ode..    - `ente
-00000760: 7260 3a20 7365 6e64 2074 6578 7420 746f  r`: send text to
-00000770: 2074 6865 2061 7373 6973 7461 6e74 2e0a   the assistant..
-00000780: 0a23 2323 2043 7573 746f 6d69 7a61 7469  .### Customizati
-00000790: 6f6e 0a0a 2d20 4966 2079 6f75 2077 616e  on..- If you wan
-000007a0: 7420 6375 7374 6f6d 206b 6579 6269 6e64  t custom keybind
-000007b0: 696e 6773 2c20 796f 7520 6361 6e20 6d6f  ings, you can mo
-000007c0: 6469 6679 2074 6865 2060 2448 4f4d 452f  dify the `$HOME/
-000007d0: 2e63 6f6e 6669 672f 6770 7474 7569 2f6b  .config/gpttui/k
-000007e0: 6579 6269 6e64 696e 6773 2e6a 736f 6e60  eybindings.json`
-000007f0: 2066 696c 652e 0a2d 2049 6620 796f 7520   file..- If you 
-00000800: 7761 6e74 2074 6f20 6368 616e 6765 2074  want to change t
-00000810: 6865 2061 7070 2073 7479 6c65 2c20 796f  he app style, yo
-00000820: 7520 6361 6e20 6d6f 6469 6679 2074 6865  u can modify the
-00000830: 2060 2448 4f4d 452f 2e63 6f6e 6669 672f   `$HOME/.config/
-00000840: 6770 7474 7569 2f73 7479 6c65 2e63 7373  gpttui/style.css
-00000850: 6020 6669 6c65 2e0a 0a                   ` file...
+00000000: 2320 4750 5454 5549 0a2d 2d2d 0a0a 3c61  # GPTTUI.---..<a
+00000010: 2068 7265 663d 2268 7474 7073 3a2f 2f70   href="https://p
+00000020: 7970 692e 7079 7468 6f6e 2e6f 7267 2f70  ypi.python.org/p
+00000030: 7970 692f 6770 7474 7569 223e 3c69 6d67  ypi/gpttui"><img
+00000040: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+00000050: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+00000060: 692f 762f 6770 7474 7569 2e73 7667 222f  i/v/gpttui.svg"/
+00000070: 3e3c 2f61 3e0a 0a54 5549 2074 6f20 696e  ></a>..TUI to in
+00000080: 7465 7261 6374 2077 6974 6820 6770 7420  teract with gpt 
+00000090: 6d6f 6465 6c73 2e0a 0a21 5b65 7861 6d70  models...![examp
+000000a0: 6c65 5d28 2e2f 646f 6373 2f69 6d67 2f65  le](./docs/img/e
+000000b0: 7861 6d70 6c65 2e67 6966 290a 0a60 6770  xample.gif)..`gp
+000000c0: 7474 7569 6020 7072 6f76 6964 6573 2061  ttui` provides a
+000000d0: 2074 6572 6d69 6e61 6c20 6672 6f6e 7465   terminal fronte
+000000e0: 6e64 2074 6861 7420 616c 6c6f 7773 2073  nd that allows s
+000000f0: 6573 7369 6f6e 7320 2863 6f6e 7665 7273  essions (convers
+00000100: 6174 696f 6e73 2920 7769 7468 204c 4c4d  ations) with LLM
+00000110: 732c 2073 746f 7265 7320 616c 6c20 7468  s, stores all th
+00000120: 6520 696e 666f 726d 6174 696f 6e20 696e  e information in
+00000130: 2061 2063 656e 7472 616c 697a 6564 2064   a centralized d
+00000140: 6174 6162 6173 652c 2061 6e64 2070 726f  atabase, and pro
+00000150: 7669 6465 7320 7669 2d6c 696b 6520 6b65  vides vi-like ke
+00000160: 7962 696e 6469 6e67 732e 0a0a 3e20 2a2a  ybindings...> **
+00000170: 4e6f 7465 2a2a 3a20 4174 2074 6865 206d  Note**: At the m
+00000180: 6f6d 656e 7420 6974 206f 6e6c 7920 7375  oment it only su
+00000190: 7070 6f72 7473 202a 2a4f 7065 6e41 492a  pports **OpenAI*
+000001a0: 2a20 6d6f 6465 6c73 2c20 6275 7420 6f74  * models, but ot
+000001b0: 6865 7220 4c4c 4d73 2063 616e 2062 6520  her LLMs can be 
+000001c0: 6561 7369 6c79 2069 6e74 6567 7261 7465  easily integrate
+000001d0: 642e 2053 616d 6520 7769 7468 2074 6865  d. Same with the
+000001e0: 2064 6174 6162 6173 6573 2c20 6375 7272   databases, curr
+000001f0: 656e 746c 7920 7375 7070 6f72 7469 6e67  ently supporting
+00000200: 2060 7371 6c69 7465 602e 0a0a 2323 2049   `sqlite`...## I
+00000210: 6e73 7461 6c6c 6174 696f 6e0a 0a59 6f75  nstallation..You
+00000220: 2063 616e 2069 6e73 7461 6c6c 2060 6770   can install `gp
+00000230: 7474 7569 6020 7769 7468 2060 7069 7060  ttui` with `pip`
+00000240: 3a0a 0a60 6060 7368 0a70 6970 2069 6e73  :..```sh.pip ins
+00000250: 7461 6c6c 2067 7074 7475 690a 6060 600a  tall gpttui.```.
+00000260: 0a23 2320 4261 7369 6320 436f 6e63 6570  .## Basic Concep
+00000270: 7473 0a0a 2d20 6073 6573 7369 6f6e 603a  ts..- `session`:
+00000280: 2061 2063 6f6e 7665 7273 6174 696f 6e20   a conversation 
+00000290: 2863 6861 7429 2e0a 2d20 6063 6f6e 7465  (chat)..- `conte
+000002a0: 7874 603a 2073 7065 6369 6669 6573 2061  xt`: specifies a
+000002b0: 2074 6f70 6963 206f 7220 6120 7370 6563   topic or a spec
+000002c0: 6961 6c69 7a61 7469 6f6e 2066 6f72 2074  ialization for t
+000002d0: 6865 2061 7373 6973 7461 6e74 2e0a 2d20  he assistant..- 
+000002e0: 6075 7365 7260 3a20 7468 6520 7065 7273  `user`: the pers
+000002f0: 6f6e 2074 6861 7420 7573 6573 2060 6770  on that uses `gp
+00000300: 7474 7569 602e 0a2d 2060 6173 7369 7374  ttui`..- `assist
+00000310: 616e 7460 3a20 7468 6520 4149 2061 7373  ant`: the AI ass
+00000320: 6973 7461 6e74 2e0a 0a23 2320 5573 6167  istant...## Usag
+00000330: 650a 0a59 6f75 2063 616e 2067 6574 206d  e..You can get m
+00000340: 6f72 6520 696e 666f 726d 6174 696f 6e20  ore information 
+00000350: 7573 696e 6720 7468 6520 6865 6c70 2070  using the help p
+00000360: 6167 653a 0a0a 6060 6073 680a 6770 7474  age:..```sh.gptt
+00000370: 7569 202d 2d68 656c 700a 6060 600a 0a4c  ui --help.```..L
+00000380: 696b 6577 6973 652c 2079 6f75 2063 616e  ikewise, you can
+00000390: 2067 6574 2068 656c 7020 6f66 2074 6865   get help of the
+000003a0: 2064 6966 6665 7265 6e74 2066 726f 6e74   different front
+000003b0: 656e 6420 6f70 7469 6f6e 7320 7769 7468  end options with
+000003c0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
+000003d0: 6f6d 6d61 6e64 3a0a 0a60 6060 7368 0a67  ommand:..```sh.g
+000003e0: 7074 7475 6920 6672 6f6e 7420 2d2d 6865  pttui front --he
+000003f0: 6c70 0a60 6060 0a0a 466f 7220 6578 616d  lp.```..For exam
+00000400: 706c 652c 2074 6f20 6c61 756e 6368 2074  ple, to launch t
+00000410: 6865 2054 5549 3a0a 0a60 6060 7368 0a67  he TUI:..```sh.g
+00000420: 7074 7475 6920 6672 6f6e 745c 0a20 2020  pttui front\.   
+00000430: 202d 2d64 6174 6162 6173 655f 6b69 6e64   --database_kind
+00000440: 2053 514c 4954 4520 5c0a 2020 2020 2d2d   SQLITE \.    --
+00000450: 7365 7373 696f 6e20 6669 7273 745f 6368  session first_ch
+00000460: 6174 205c 0a20 2020 202d 2d6d 6f64 656c  at \.    --model
+00000470: 5f6b 696e 6420 4f50 454e 4149 205c 0a20  _kind OPENAI \. 
+00000480: 2020 202d 2d6d 6f64 656c 5f6e 616d 6520     --model_name 
+00000490: 2267 7074 2d33 2e35 2d74 7572 626f 2220  "gpt-3.5-turbo" 
+000004a0: 5c0a 2020 2020 2d2d 636f 6e74 6578 7420  \.    --context 
+000004b0: 2759 6f75 2061 7265 2061 6e20 6578 7065  'You are an expe
+000004c0: 7274 2073 6f66 7477 6172 6520 6465 7665  rt software deve
+000004d0: 6c6f 7065 7227 0a60 6060 0a0a 2323 2320  loper'.```..### 
+000004e0: 4f70 656e 4149 0a0a 546f 2075 7365 204f  OpenAI..To use O
+000004f0: 7065 6e41 4920 6d6f 6465 6c73 2079 6f75  penAI models you
+00000500: 206e 6565 6420 746f 2073 7065 6369 6679   need to specify
+00000510: 2074 6865 2066 6f6c 6c6f 7769 6e67 2065   the following e
+00000520: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
+00000530: 626c 6573 3a0a 0a60 6060 7368 0a65 7870  bles:..```sh.exp
+00000540: 6f72 7420 4f50 454e 4149 5f4f 5247 3d22  ort OPENAI_ORG="
+00000550: 220a 6578 706f 7274 204f 5045 4e41 495f  ".export OPENAI_
+00000560: 4150 495f 4b45 593d 2222 0a60 6060 0a0a  API_KEY="".```..
+00000570: 2323 2320 4b65 7962 696e 6469 6e67 730a  ### Keybindings.
+00000580: 0a60 6770 7474 7569 6020 6861 7320 7477  .`gpttui` has tw
+00000590: 6f20 6d6f 6465 733a 0a0a 2d20 604e 4f52  o modes:..- `NOR
+000005a0: 4d41 4c60 3a20 696e 2074 6869 7320 6d6f  MAL`: in this mo
+000005b0: 6465 2079 6f75 2063 616e 2064 6f20 676c  de you can do gl
+000005c0: 6f62 616c 206f 7065 7261 7469 6f6e 732e  obal operations.
+000005d0: 2042 7920 6465 6661 756c 742c 2060 4e4f   By default, `NO
+000005e0: 524d 414c 6020 6d6f 6465 2068 6173 2074  RMAL` mode has t
+000005f0: 6865 2066 6f6c 6c6f 7769 6e67 2062 696e  he following bin
+00000600: 6469 6e67 733a 0a20 2020 202d 2060 6360  dings:.    - `c`
+00000610: 3a20 636c 6561 7220 6d65 7373 6167 6573  : clear messages
+00000620: 2e0a 2020 2020 2d20 6064 603a 2064 656c  ..    - `d`: del
+00000630: 6574 6520 7072 6f6d 7074 2e0a 2020 2020  ete prompt..    
+00000640: 2d20 6071 603a 2071 7569 742e 0a20 2020  - `q`: quit..   
+00000650: 202d 2060 7960 3a20 7961 6e6b 2f63 6f70   - `y`: yank/cop
+00000660: 7920 7468 6520 6c61 7374 206d 6573 7361  y the last messa
+00000670: 6765 2066 726f 6d20 7468 6520 6173 7369  ge from the assi
+00000680: 7374 616e 742e 0a20 2020 202d 2060 7060  stant..    - `p`
+00000690: 3a20 7061 7374 6520 736f 6d65 2074 6578  : paste some tex
+000006a0: 7420 6672 6f6d 2074 6865 2063 6c69 7062  t from the clipb
+000006b0: 6f61 7264 2069 6e74 6f20 7468 6520 7072  oard into the pr
+000006c0: 6f6d 7074 2e0a 2020 2020 2d20 6069 603a  ompt..    - `i`:
+000006d0: 2073 7769 7463 6820 746f 2069 6e73 6572   switch to inser
+000006e0: 7420 6d6f 6465 2e0a 0a2d 2060 494e 5345  t mode...- `INSE
+000006f0: 5254 603a 2069 6e20 7468 6973 206d 6f64  RT`: in this mod
+00000700: 6520 796f 7520 6361 6e20 7072 6f6d 7074  e you can prompt
+00000710: 2074 6578 742e 2042 7920 6465 6661 756c   text. By defaul
+00000720: 742c 2060 494e 5345 5254 6020 6d6f 6465  t, `INSERT` mode
+00000730: 2068 6173 2074 6865 2066 6f6c 6c6f 7769   has the followi
+00000740: 6e67 2062 696e 6469 6e67 733a 0a20 2020  ng bindings:.   
+00000750: 202d 2060 6573 6360 3a20 7377 6974 6368   - `esc`: switch
+00000760: 2074 6f20 6e6f 726d 616c 206d 6f64 652e   to normal mode.
+00000770: 0a20 2020 202d 2060 656e 7465 7260 3a20  .    - `enter`: 
+00000780: 7365 6e64 2074 6578 7420 746f 2074 6865  send text to the
+00000790: 2061 7373 6973 7461 6e74 2e0a 0a23 2323   assistant...###
+000007a0: 2043 7573 746f 6d69 7a61 7469 6f6e 0a0a   Customization..
+000007b0: 2d20 4966 2079 6f75 2077 616e 7420 6375  - If you want cu
+000007c0: 7374 6f6d 206b 6579 6269 6e64 696e 6773  stom keybindings
+000007d0: 2c20 796f 7520 6361 6e20 6d6f 6469 6679  , you can modify
+000007e0: 2074 6865 2060 2448 4f4d 452f 2e63 6f6e   the `$HOME/.con
+000007f0: 6669 672f 6770 7474 7569 2f6b 6579 6269  fig/gpttui/keybi
+00000800: 6e64 696e 6773 2e6a 736f 6e60 2066 696c  ndings.json` fil
+00000810: 652e 0a2d 2049 6620 796f 7520 7761 6e74  e..- If you want
+00000820: 2074 6f20 6368 616e 6765 2074 6865 2061   to change the a
+00000830: 7070 2073 7479 6c65 2c20 796f 7520 6361  pp style, you ca
+00000840: 6e20 6d6f 6469 6679 2074 6865 2060 2448  n modify the `$H
+00000850: 4f4d 452f 2e63 6f6e 6669 672f 6770 7474  OME/.config/gptt
+00000860: 7569 2f73 7479 6c65 2e63 7373 6020 6669  ui/style.css` fi
+00000870: 6c65 2e0a                                le..
```

### Comparing `gpttui-0.2.0/pyproject.toml` & `gpttui-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gpttui"
-version = "0.2.0"
+version = "0.3.0"
 authors = [{name = "Juan Lara", email = "julara@unal.edu.co"}]
 description = "TUI to interact with gpt models."
 requires-python = ">3.8"
 dependencies = [
     "openai", "textual[dev]", "pydantic", "pyperclip"
 ]
```

### Comparing `gpttui-0.2.0/src/gpttui/database/base.py` & `gpttui-0.3.0/src/gpttui/database/base.py`

 * *Files identical despite different names*

### Comparing `gpttui-0.2.0/src/gpttui/database/sqlite.py` & `gpttui-0.3.0/src/gpttui/database/sqlite.py`

 * *Files identical despite different names*

### Comparing `gpttui-0.2.0/src/gpttui/models/base.py` & `gpttui-0.3.0/src/gpttui/models/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         -------
         AbstractModel
             Instance of the model to use as a builder.
         """
         ...
 
     @abstractmethod
-    def get_answer(self, message: str) -> str:
+    async def get_answer(self, message: str) -> str:
         """
         Generates an answer given an input message.
 
         Parameters
         ----------
         message : str
             Input text.
```

### Comparing `gpttui-0.2.0/src/gpttui/models/openai.py` & `gpttui-0.3.0/src/gpttui/models/openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                     message=Message(role="system", content=self.context),
                     timestamp=int(time.time())
                     )
             self.database.add_message(msg=msg, session_name=self.session_name)
             return self.last_messages()
         return last_msgs
 
-    def get_answer(self, message: str) -> str:
+    async def get_answer(self, message: str) -> str:
         """
         Obtains an answer form any message.
 
         Parameters
         ----------
         message : str
             Input message.
@@ -80,24 +80,22 @@
                 )
         self.database.add_message(msg=new_msg, session_name=self.session_name)
         last_msgs = self.last_messages()
         response = ""
         retries = 0
         while not response and retries < self.max_retries:
             try:
-                response = str(
-                        openai.ChatCompletion.create(
+                response = await openai.ChatCompletion.acreate(
                             model = self.model_name,
                             messages = last_msgs.dict()["values"],
                             request_timeout = self.timeout
                             )
-                        .choices[0].message.content #type: ignore
-                        )
             except Timeout:
                 retries += 1
+        response = str(response.choices[0].message.content) # type: ignore
         if retries == 3:
             raise Timeout("Maximum number of retries achieved.")
         new_msg = MessageWithTime(
                 message=Message(role="assistant", content=response),
                 timestamp=int(time.time())
                 )
         self.database.add_message(msg=new_msg, session_name=self.session_name)
```

### Comparing `gpttui-0.2.0/src/gpttui/tui/app.py` & `gpttui-0.3.0/src/gpttui/tui/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 This file defines the main TUI App.
 """
-import os 
+import os, re
 import pyperclip
 from pathlib import Path
 from enum import Enum, auto
-from typing import Any, Optional
+from typing import Any
 from textual.app import App, ComposeResult
 from textual.widgets import Input, Markdown, Static
 from textual.containers import Container
 from textual.events import Key
 from gpttui.models.base import AbstractModel
 from gpttui.tui.config import KeyBindings, keybindings_config
 
@@ -17,49 +17,100 @@
     """
     This enum represents the possible modes of the application.
     """
     INSERT = auto()
     NORMAL = auto()
 
 class NormalIndicator(Static):
+    """
+    Static container for the normal mode.
+    """
     ...
 
 class InsertIndicator(Static):
+    """
+    Static container for the insert mode.
+    """
     ...
 
 class UserInput(Input):
+    """
+    Represents the text input.
+    """
     ...
 
 class Prompt(Static):
+    """
+    The prompt contains the mode indicators and the text input.
+    """
     def compose(self) -> ComposeResult:
         yield NormalIndicator("NORMAL", id="normal-indicator")
         yield InsertIndicator("INSERT", id="insert-indicator")
         yield Input(placeholder="Enter some text...")
 
 class UserText(Static):
-    ...
-
-class UserMessage(Static):
+    """
+    Static container to display the sender.
+    """
     ...
 
 class Message(Static):
+    """
+    A message contains the the sender and its text.
+
+    Parameters
+    ----------
+    user : str
+        Sender.
+    message : str
+        Text of the message.
+    """
 
     def __init__(self, user:str, message: str, *args: Any, **kwargs: Any):
         super(Message, self).__init__(*args, **kwargs)
         self.user = user
         self.message = message
 
     def compose(self) -> ComposeResult:
+        """
+        Generator with the message components.
+
+        Yields
+        ------
+        ComposeResult:
+            Widgets in the message.
+
+        """
         yield UserText(self.user)
-        yield UserMessage(self.message)
+        # BUG: seems like textual isn't able to render inline code compose markdowns.
+        try:
+            md = Markdown()
+            md.update(self.message)
+        except:
+            md = Static(self.message)
+        yield md
 
 class Messages(Container):
+    """
+    A container that stores all messages.
+    """
 
     def add_message(self, msg: str, user: str):
+        """
+        This method dynamically adds a message.
+
+        Parameters
+        ----------
+        msg : str
+            Message to display.
+        user : str
+            Sender of the message.
+        """
         self.mount(Message(user=user, message=msg))
+        self.scroll_end()
 
 class GptApp(App):
     """
     This class defines the TUI App.
 
     Parameters
     ----------
@@ -123,110 +174,108 @@
         ------
         ComposeResult
             TUI components.
         """
         yield Prompt()
         yield Messages()
 
-    def on_key(self, event: Key) -> None:
+    async def on_key(self, event: Key) -> None:
         """
         Callback that is called when a key is pressed.
 
         Parameters
         ----------
         event : Key
             Event related to the key that was pressed.
         """
         if self.mode == ModeEnum.NORMAL:
-            self.handle_normal(event)
+            await self.handle_normal(event)
         elif self.mode == ModeEnum.INSERT:
-            self.handle_insert(event)
+            await self.handle_insert(event)
 
-    def handle_normal(self, event: Key) -> None:
+    async def handle_normal(self, event: Key) -> None:
         """
         Determines what to do in normal mode.
 
         Parameters
         ----------
         event : Key
             Event related to the key that was pressed.
         """
         f = self.normal_commands.get(event.key)
-        if f is not None: f()
+        if f is not None: await f()
 
-    def handle_insert(self, event: Key) -> None:
+    async def handle_insert(self, event: Key) -> None:
         """
         Determines what to do in insert mode.
 
         Parameters
         ----------
         event : Key
             Event related to the key that was pressed.
         """
         f = self.insert_commands.get(event.key)
-        if f is not None: f()
+        if f is not None: await f()
 
-    def insert(self):
+    async def insert(self):
         """
         Changes to insert mode.
         """
         self.add_class("insert-mode")
         self.query_one(Input).focus()
         self.mode = ModeEnum.INSERT
 
-    def clear(self):
+    async def clear(self):
         """
         Clears the historical messages.
         """
-        self.chat_text = ""
-        self.query_one(Markdown).update(self.chat_text)
+        self.query_one(Messages) #TODO
 
-    def yank(self):
+    async def yank(self):
         """
         Copies the last message into the clipboard.
         """
         msgs = self.model.database.get_messages(self.model.session_name)
         pyperclip.copy(msgs.values[-1].content)
 
-    def paste(self):
+    async def paste(self):
         """
         Pastes the clipboard into the prompt.
         """
         clipboard_text = pyperclip.paste()
         self.query_one(Input).insert_text_at_cursor(clipboard_text)
 
-    def normal(self):
+    async def normal(self):
         """
         Switch to normal mode.
         """
         self.remove_class("insert-mode")
         self.query_one(Input).reset_focus()
         self.mode = ModeEnum.NORMAL
 
-    def quit(self):
+    async def quit(self):
         """
         Exit the app.
         """
         self.model.database.close()
         self.exit()
 
-    def delete(self):
+    async def delete(self):
         """
         Deletes the prompt.
         """
         inp = self.query_one(Input)
         inp.action_delete_right_all()
         inp.action_delete_left_all()
 
-    def send(self):
+    async def send(self):
         """
         Sends the text in the prompt to the model and shows the response.
         """
         inp = self.query_one(Input)
         text = inp.value
+        messages = self.query_one(Messages)
         inp.action_delete_right_all()
         inp.action_delete_left_all()
-        answer = self.model.get_answer(text)
-        messages = self.query_one(Messages)
         messages.add_message(msg=text, user="User")
+        answer = await self.model.get_answer(text)
         messages.add_message(msg=answer, user="Assistant")
-        messages.scroll_end()
```

### Comparing `gpttui-0.2.0/src/gpttui/tui/config.py` & `gpttui-0.3.0/src/gpttui/tui/config.py`

 * *Files identical despite different names*

### Comparing `gpttui-0.2.0/src/gpttui/tui/front.py` & `gpttui-0.3.0/src/gpttui/tui/front.py`

 * *Files identical despite different names*

### Comparing `gpttui-0.2.0/test/test_db.py` & `gpttui-0.3.0/test/test_db.py`

 * *Files identical despite different names*

### Comparing `gpttui-0.2.0/test/test_model.py` & `gpttui-0.3.0/test/test_model.py`

 * *Files identical despite different names*

