# Comparing `tmp/czech_workdays_holidays-0.0.9.tar.gz` & `tmp/czech_workdays_holidays-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "czech_workdays_holidays-0.0.9.tar", last modified: Fri Apr 21 19:37:44 2023, max compression
+gzip compressed data, was "czech_workdays_holidays-0.1.0.tar", last modified: Fri Apr 21 22:15:24 2023, max compression
```

## Comparing `czech_workdays_holidays-0.0.9.tar` & `czech_workdays_holidays-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 19:37:44.449131 czech_workdays_holidays-0.0.9/
--rw-rw-rw-   0        0        0     1072 2023-04-21 15:08:04.000000 czech_workdays_holidays-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     1645 2023-04-21 19:37:44.448130 czech_workdays_holidays-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1036 2023-04-21 15:26:41.000000 czech_workdays_holidays-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 19:37:44.446130 czech_workdays_holidays-0.0.9/czech_workdays_holidays.egg-info/
--rw-rw-rw-   0        0        0     1645 2023-04-21 19:37:44.000000 czech_workdays_holidays-0.0.9/czech_workdays_holidays.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-04-21 19:37:44.000000 czech_workdays_holidays-0.0.9/czech_workdays_holidays.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 19:37:44.000000 czech_workdays_holidays-0.0.9/czech_workdays_holidays.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-21 19:37:44.000000 czech_workdays_holidays-0.0.9/czech_workdays_holidays.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10243 2023-04-21 15:43:21.000000 czech_workdays_holidays-0.0.9/czech_workdays_holidays.py
--rw-rw-rw-   0        0        0      788 2023-04-21 19:37:38.000000 czech_workdays_holidays-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-21 19:37:44.449131 czech_workdays_holidays-0.0.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-21 19:37:44.447130 czech_workdays_holidays-0.0.9/test/
--rw-rw-rw-   0        0        0        0 2023-04-21 12:09:27.000000 czech_workdays_holidays-0.0.9/test/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-21 22:15:24.155248 czech_workdays_holidays-0.1.0/
+-rw-rw-rw-   0        0        0     1072 2023-04-21 15:08:04.000000 czech_workdays_holidays-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     4807 2023-04-21 22:15:24.154248 czech_workdays_holidays-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4122 2023-04-21 22:12:28.000000 czech_workdays_holidays-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 22:15:24.152247 czech_workdays_holidays-0.1.0/czech_workdays_holidays.egg-info/
+-rw-rw-rw-   0        0        0     4807 2023-04-21 22:15:24.000000 czech_workdays_holidays-0.1.0/czech_workdays_holidays.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-04-21 22:15:24.000000 czech_workdays_holidays-0.1.0/czech_workdays_holidays.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 22:15:24.000000 czech_workdays_holidays-0.1.0/czech_workdays_holidays.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-04-21 22:15:24.000000 czech_workdays_holidays-0.1.0/czech_workdays_holidays.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-04-21 22:15:24.000000 czech_workdays_holidays-0.1.0/czech_workdays_holidays.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11557 2023-04-21 22:09:09.000000 czech_workdays_holidays-0.1.0/czech_workdays_holidays.py
+-rw-rw-rw-   0        0        0      776 2023-04-21 22:15:09.000000 czech_workdays_holidays-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-21 22:15:24.155248 czech_workdays_holidays-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-21 22:15:24.153247 czech_workdays_holidays-0.1.0/test/
+-rw-rw-rw-   0        0        0        0 2023-04-21 12:09:27.000000 czech_workdays_holidays-0.1.0/test/tests.py
```

### Comparing `czech_workdays_holidays-0.0.9/LICENSE` & `czech_workdays_holidays-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `czech_workdays_holidays-0.0.9/czech_workdays_holidays.py` & `czech_workdays_holidays-0.1.0/czech_workdays_holidays.py`

 * *Files 7% similar despite different names*

```diff
@@ -525,117 +525,199 @@
 000020c0: 686f 6c69 6461 795f 6e61 6d65 5f65 6e22  holiday_name_en"
 000020d0: 5d5d 2066 6f72 2078 2069 6e20 686f 6c69  ]] for x in holi
 000020e0: 6461 7973 5d0d 0a20 2020 2020 2020 2072  days]..        r
 000020f0: 6574 7572 6e20 686f 6c69 6461 795f 6461  eturn holiday_da
 00002100: 7465 735f 656e 5f6e 616d 6573 0d0a 0d0a  tes_en_names....
 00002110: 2020 2020 7265 7475 726e 2068 6f6c 6964      return holid
 00002120: 6179 730d 0a0d 0a0d 0a64 6566 2067 6574  ays......def get
-00002130: 5f77 6f72 6b69 6e67 5f64 6179 7328 7965  _working_days(ye
-00002140: 6172 3a20 696e 742c 0d0a 2020 2020 2020  ar: int,..      
-00002150: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00002160: 6e63 6c75 6465 5f73 6174 7572 6461 793a  nclude_saturday:
-00002170: 2062 6f6f 6c20 3d20 4661 6c73 652c 0d0a   bool = False,..
-00002180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002190: 2020 2020 2069 6e63 6c75 6465 5f73 756e       include_sun
-000021a0: 6461 793a 2062 6f6f 6c20 3d20 4661 6c73  day: bool = Fals
-000021b0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-000021c0: 2020 2020 2020 2020 2069 6e63 6c75 6465           include
-000021d0: 5f73 686f 7070 696e 675f 7265 7374 7269  _shopping_restri
-000021e0: 6374 6564 5f64 6179 733a 2062 6f6f 6c20  cted_days: bool 
-000021f0: 3d20 4661 6c73 6529 202d 3e20 6c69 7374  = False) -> list
-00002200: 3a0d 0a0d 0a20 2020 2022 2222 0d0a 0d0a  :....    """....
-00002210: 2020 2020 3a70 6172 616d 2079 6561 723a      :param year:
-00002220: 2044 6573 6972 6564 2079 6561 7220 746f   Desired year to
-00002230: 2067 656e 6572 6174 6520 686f 6c69 6461   generate holida
-00002240: 7973 2028 696e 7429 0d0a 2020 2020 3a70  ys (int)..    :p
-00002250: 6172 616d 2069 6e63 6c75 6465 5f73 6174  aram include_sat
-00002260: 7572 6461 793a 2049 6e63 6c75 6465 7320  urday: Includes 
-00002270: 616c 736f 2053 6174 7572 6461 7973 2069  also Saturdays i
-00002280: 6e20 6f75 7470 7574 0d0a 2020 2020 3a70  n output..    :p
-00002290: 6172 616d 2069 6e63 6c75 6465 5f73 756e  aram include_sun
-000022a0: 6461 793a 2049 6e63 6c75 6465 7320 616c  day: Includes al
-000022b0: 736f 2053 756e 6461 7973 2069 6e20 6f75  so Sundays in ou
-000022c0: 7470 7574 0d0a 2020 2020 3a70 6172 616d  tput..    :param
-000022d0: 2069 6e63 6c75 6465 5f73 686f 7070 696e   include_shoppin
-000022e0: 675f 7265 7374 7269 6374 6564 5f64 6179  g_restricted_day
-000022f0: 733a 2049 6e63 6c75 6465 7320 616c 736f  s: Includes also
-00002300: 2073 686f 7070 696e 6720 7265 7374 7269   shopping restri
-00002310: 6374 6564 2064 6179 7320 696e 206f 7574  cted days in out
-00002320: 7075 7420 6966 206e 6f74 2077 6565 6b65  put if not weeke
-00002330: 6e64 2e0d 0a20 2020 2020 2020 2020 2020  nd...           
-00002340: 2043 616e 2062 6520 636f 6d62 696e 6564   Can be combined
-00002350: 2077 6974 6820 696e 636c 7564 655f 7361   with include_sa
-00002360: 7475 7264 6179 2f73 756e 6461 7920 7061  turday/sunday pa
-00002370: 7261 6d65 7465 720d 0a20 2020 203a 7265  rameter..    :re
-00002380: 7475 726e 3a20 4c69 7374 206f 6620 616c  turn: List of al
-00002390: 6c20 776f 726b 696e 6720 6461 7973 202d  l working days -
-000023a0: 3e20 5b64 6174 6574 696d 652e 6461 7465  > [datetime.date
-000023b0: 2832 3032 332c 2031 2c20 3229 2c20 2e2e  (2023, 1, 2), ..
-000023c0: 2e5d 0d0a 2020 2020 2222 220d 0a0d 0a20  .]..    """.... 
-000023d0: 2020 2068 6f6c 6964 6179 5f64 6174 6573     holiday_dates
-000023e0: 203d 2073 6574 2868 6f6c 6964 6179 5b22   = set(holiday["
-000023f0: 6461 7465 225d 2066 6f72 2068 6f6c 6964  date"] for holid
-00002400: 6179 2069 6e20 6765 745f 686f 6c69 6461  ay in get_holida
-00002410: 7973 2879 6561 7229 290d 0a20 2020 2069  ys(year))..    i
-00002420: 6620 696e 636c 7564 655f 7368 6f70 7069  f include_shoppi
-00002430: 6e67 5f72 6573 7472 6963 7465 645f 6461  ng_restricted_da
-00002440: 7973 3a0d 0a20 2020 2020 2020 2073 686f  ys:..        sho
-00002450: 7070 696e 675f 7265 7374 7269 6374 6564  pping_restricted
-00002460: 203d 2073 6574 2868 6f6c 6964 6179 5b22   = set(holiday["
-00002470: 6461 7465 225d 2066 6f72 2068 6f6c 6964  date"] for holid
-00002480: 6179 2069 6e20 6765 745f 686f 6c69 6461  ay in get_holida
-00002490: 7973 2879 6561 722c 2073 686f 7070 696e  ys(year, shoppin
-000024a0: 675f 7265 7374 7269 6374 6564 3d54 7275  g_restricted=Tru
-000024b0: 6529 290d 0a20 2020 2020 2020 2068 6f6c  e))..        hol
-000024c0: 6964 6179 5f64 6174 6573 2e75 6e69 6f6e  iday_dates.union
-000024d0: 2873 686f 7070 696e 675f 7265 7374 7269  (shopping_restri
-000024e0: 6374 6564 290d 0a0d 0a20 2020 2077 6565  cted)....    wee
-000024f0: 6b65 6e64 5f64 6179 7320 3d20 5b22 5361  kend_days = ["Sa
-00002500: 7475 7264 6179 222c 2022 5375 6e64 6179  turday", "Sunday
-00002510: 225d 0d0a 2020 2020 6966 2069 6e63 6c75  "]..    if inclu
-00002520: 6465 5f73 6174 7572 6461 793a 0d0a 2020  de_saturday:..  
-00002530: 2020 2020 2020 7765 656b 656e 645f 6461        weekend_da
-00002540: 7973 2e72 656d 6f76 6528 2253 6174 7572  ys.remove("Satur
-00002550: 6461 7922 290d 0a0d 0a20 2020 2069 6620  day")....    if 
-00002560: 696e 636c 7564 655f 7375 6e64 6179 3a0d  include_sunday:.
-00002570: 0a20 2020 2020 2020 2077 6565 6b65 6e64  .        weekend
-00002580: 5f64 6179 732e 7265 6d6f 7665 2822 5375  _days.remove("Su
-00002590: 6e64 6179 2229 0d0a 0d0a 2020 2020 2320  nday")....    # 
-000025a0: 7768 696c 6520 6c6f 6f70 2076 6172 6961  while loop varia
-000025b0: 626c 6573 0d0a 2020 2020 776f 726b 696e  bles..    workin
-000025c0: 675f 6461 7973 203d 206c 6973 7428 290d  g_days = list().
-000025d0: 0a20 2020 2073 7461 7274 5f64 6174 6520  .    start_date 
-000025e0: 3d20 6461 7465 2879 6561 722c 2031 2c20  = date(year, 1, 
-000025f0: 3129 0d0a 2020 2020 656e 645f 6461 7465  1)..    end_date
-00002600: 203d 2064 6174 6528 7965 6172 2c20 3132   = date(year, 12
-00002610: 2c20 3331 290d 0a0d 0a20 2020 2077 6869  , 31)....    whi
-00002620: 6c65 2073 7461 7274 5f64 6174 6520 3c3d  le start_date <=
-00002630: 2065 6e64 5f64 6174 653a 0d0a 2020 2020   end_date:..    
-00002640: 2020 2020 6966 2073 7461 7274 5f64 6174      if start_dat
-00002650: 6520 6e6f 7420 696e 2068 6f6c 6964 6179  e not in holiday
-00002660: 5f64 6174 6573 2061 6e64 2073 7461 7274  _dates and start
-00002670: 5f64 6174 652e 7374 7266 7469 6d65 2822  _date.strftime("
-00002680: 2541 2229 206e 6f74 2069 6e20 7765 656b  %A") not in week
-00002690: 656e 645f 6461 7973 3a0d 0a20 2020 2020  end_days:..     
-000026a0: 2020 2020 2020 2077 6f72 6b69 6e67 5f64         working_d
-000026b0: 6179 732e 6170 7065 6e64 2873 7461 7274  ays.append(start
-000026c0: 5f64 6174 6529 0d0a 2020 2020 2020 2020  _date)..        
-000026d0: 7374 6172 745f 6461 7465 202b 3d20 7469  start_date += ti
-000026e0: 6d65 6465 6c74 6128 6461 7973 3d31 290d  medelta(days=1).
-000026f0: 0a0d 0a20 2020 2072 6574 7572 6e20 776f  ...    return wo
-00002700: 726b 696e 675f 6461 7973 0d0a 0d0a 0d0a  rking_days......
-00002710: 6465 6620 6765 745f 686f 6c69 6461 7973  def get_holidays
-00002720: 5f64 7572 696e 675f 7765 656b 656e 6428  _during_weekend(
-00002730: 7965 6172 3a20 696e 7429 202d 3e20 6c69  year: int) -> li
-00002740: 7374 3a0d 0a20 2020 2068 6f6c 6964 6179  st:..    holiday
-00002750: 5f64 6174 6573 203d 206c 6973 7428 686f  _dates = list(ho
-00002760: 6c69 6461 795b 2264 6174 6522 5d20 666f  liday["date"] fo
-00002770: 7220 686f 6c69 6461 7920 696e 2067 6574  r holiday in get
-00002780: 5f68 6f6c 6964 6179 7328 7965 6172 290d  _holidays(year).
-00002790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000027a0: 2020 2020 2020 2020 2069 6620 686f 6c69           if holi
-000027b0: 6461 795b 2264 6174 6522 5d2e 7374 7266  day["date"].strf
-000027c0: 7469 6d65 2822 2541 2229 2069 6e20 2822  time("%A") in ("
-000027d0: 5361 7475 7264 6179 222c 2022 5375 6e64  Saturday", "Sund
-000027e0: 6179 2229 290d 0a0d 0a20 2020 2072 6574  ay"))....    ret
-000027f0: 7572 6e20 686f 6c69 6461 795f 6461 7465  urn holiday_date
-00002800: 730d 0a                                  s..
+00002130: 5f77 6f72 6b64 6179 7328 7965 6172 3a20  _workdays(year: 
+00002140: 696e 742c 0d0a 2020 2020 2020 2020 2020  int,..          
+00002150: 2020 2020 2020 2069 6e63 6c75 6465 5f73         include_s
+00002160: 6174 7572 6461 793a 2062 6f6f 6c20 3d20  aturday: bool = 
+00002170: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
+00002180: 2020 2020 2020 2020 2069 6e63 6c75 6465           include
+00002190: 5f73 756e 6461 793a 2062 6f6f 6c20 3d20  _sunday: bool = 
+000021a0: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
+000021b0: 2020 2020 2020 2020 2069 6e63 6c75 6465           include
+000021c0: 5f68 6f6c 6964 6179 733a 2062 6f6f 6c20  _holidays: bool 
+000021d0: 3d20 4661 6c73 6529 202d 3e20 6c69 7374  = False) -> list
+000021e0: 3a0d 0a0d 0a20 2020 2022 2222 0d0a 0d0a  :....    """....
+000021f0: 2020 2020 3a70 6172 616d 2079 6561 723a      :param year:
+00002200: 2044 6573 6972 6564 2079 6561 7220 746f   Desired year to
+00002210: 2067 656e 6572 6174 6520 686f 6c69 6461   generate holida
+00002220: 7973 2028 696e 7429 0d0a 2020 2020 3a70  ys (int)..    :p
+00002230: 6172 616d 2069 6e63 6c75 6465 5f73 6174  aram include_sat
+00002240: 7572 6461 793a 2049 6e63 6c75 6465 7320  urday: Includes 
+00002250: 616c 736f 2053 6174 7572 6461 7973 2069  also Saturdays i
+00002260: 6e20 6f75 7470 7574 0d0a 2020 2020 3a70  n output..    :p
+00002270: 6172 616d 2069 6e63 6c75 6465 5f73 756e  aram include_sun
+00002280: 6461 793a 2049 6e63 6c75 6465 7320 616c  day: Includes al
+00002290: 736f 2053 756e 6461 7973 2069 6e20 6f75  so Sundays in ou
+000022a0: 7470 7574 0d0a 2020 2020 3a70 6172 616d  tput..    :param
+000022b0: 2069 6e63 6c75 6465 5f68 6f6c 6964 6179   include_holiday
+000022c0: 733a 2043 6f75 6e74 7320 686f 6c69 6461  s: Counts holida
+000022d0: 7973 2061 7320 776f 726b 696e 6720 6461  ys as working da
+000022e0: 7973 0d0a 2020 2020 3a70 6172 616d 2073  ys..    :param s
+000022f0: 686f 7070 696e 675f 6461 7973 3a20 496e  hopping_days: In
+00002300: 636c 7564 6573 2061 6c73 6f20 7368 6f70  cludes also shop
+00002310: 7069 6e67 2072 6573 7472 6963 7465 6420  ping restricted 
+00002320: 6461 7973 2069 6e20 6f75 7470 7574 2069  days in output i
+00002330: 6620 6e6f 7420 7765 656b 656e 642e 0d0a  f not weekend...
+00002340: 2020 2020 2020 2020 2020 2020 4361 6e20              Can 
+00002350: 6265 2063 6f6d 6269 6e65 6420 7769 7468  be combined with
+00002360: 2069 6e63 6c75 6465 5f73 6174 7572 6461   include_saturda
+00002370: 792f 7375 6e64 6179 2070 6172 616d 6574  y/sunday paramet
+00002380: 6572 0d0a 2020 2020 3a72 6574 7572 6e3a  er..    :return:
+00002390: 204c 6973 7420 6f66 2061 6c6c 2077 6f72   List of all wor
+000023a0: 6b69 6e67 2064 6179 7320 2d3e 205b 6461  king days -> [da
+000023b0: 7465 7469 6d65 2e64 6174 6528 3230 3233  tetime.date(2023
+000023c0: 2c20 312c 2032 292c 202e 2e2e 5d0d 0a20  , 1, 2), ...].. 
+000023d0: 2020 2022 2222 0d0a 0d0a 2020 2020 686f     """....    ho
+000023e0: 6c69 6461 795f 6461 7465 7320 3d20 7365  liday_dates = se
+000023f0: 7428 686f 6c69 6461 795b 2264 6174 6522  t(holiday["date"
+00002400: 5d20 666f 7220 686f 6c69 6461 7920 696e  ] for holiday in
+00002410: 2067 6574 5f68 6f6c 6964 6179 7328 7965   get_holidays(ye
+00002420: 6172 2929 2069 6620 6e6f 7420 696e 636c  ar)) if not incl
+00002430: 7564 655f 686f 6c69 6461 7973 2065 6c73  ude_holidays els
+00002440: 6520 7365 7428 290d 0a0d 0a20 2020 2077  e set()....    w
+00002450: 6565 6b65 6e64 5f64 6179 7320 3d20 5b22  eekend_days = ["
+00002460: 5361 7475 7264 6179 222c 2022 5375 6e64  Saturday", "Sund
+00002470: 6179 225d 0d0a 2020 2020 6966 2069 6e63  ay"]..    if inc
+00002480: 6c75 6465 5f73 6174 7572 6461 793a 0d0a  lude_saturday:..
+00002490: 2020 2020 2020 2020 7765 656b 656e 645f          weekend_
+000024a0: 6461 7973 2e72 656d 6f76 6528 2253 6174  days.remove("Sat
+000024b0: 7572 6461 7922 290d 0a0d 0a20 2020 2069  urday")....    i
+000024c0: 6620 696e 636c 7564 655f 7375 6e64 6179  f include_sunday
+000024d0: 3a0d 0a20 2020 2020 2020 2077 6565 6b65  :..        weeke
+000024e0: 6e64 5f64 6179 732e 7265 6d6f 7665 2822  nd_days.remove("
+000024f0: 5375 6e64 6179 2229 0d0a 0d0a 2020 2020  Sunday")....    
+00002500: 2320 7768 696c 6520 6c6f 6f70 2076 6172  # while loop var
+00002510: 6961 626c 6573 0d0a 2020 2020 776f 726b  iables..    work
+00002520: 696e 675f 6461 7973 203d 206c 6973 7428  ing_days = list(
+00002530: 290d 0a20 2020 2073 7461 7274 5f64 6174  )..    start_dat
+00002540: 6520 3d20 6461 7465 2879 6561 722c 2031  e = date(year, 1
+00002550: 2c20 3129 0d0a 2020 2020 656e 645f 6461  , 1)..    end_da
+00002560: 7465 203d 2064 6174 6528 7965 6172 2c20  te = date(year, 
+00002570: 3132 2c20 3331 290d 0a0d 0a20 2020 2077  12, 31)....    w
+00002580: 6869 6c65 2073 7461 7274 5f64 6174 6520  hile start_date 
+00002590: 3c3d 2065 6e64 5f64 6174 653a 0d0a 2020  <= end_date:..  
+000025a0: 2020 2020 2020 6966 2073 7461 7274 5f64        if start_d
+000025b0: 6174 6520 6e6f 7420 696e 2068 6f6c 6964  ate not in holid
+000025c0: 6179 5f64 6174 6573 2061 6e64 2073 7461  ay_dates and sta
+000025d0: 7274 5f64 6174 652e 7374 7266 7469 6d65  rt_date.strftime
+000025e0: 2822 2541 2229 206e 6f74 2069 6e20 7765  ("%A") not in we
+000025f0: 656b 656e 645f 6461 7973 3a0d 0a20 2020  ekend_days:..   
+00002600: 2020 2020 2020 2020 2077 6f72 6b69 6e67           working
+00002610: 5f64 6179 732e 6170 7065 6e64 2873 7461  _days.append(sta
+00002620: 7274 5f64 6174 6529 0d0a 0d0a 2020 2020  rt_date)....    
+00002630: 2020 2020 7374 6172 745f 6461 7465 202b      start_date +
+00002640: 3d20 7469 6d65 6465 6c74 6128 6461 7973  = timedelta(days
+00002650: 3d31 290d 0a0d 0a20 2020 2072 6574 7572  =1)....    retur
+00002660: 6e20 776f 726b 696e 675f 6461 7973 0d0a  n working_days..
+00002670: 0d0a 0d0a 6465 6620 6765 745f 7368 6f70  ....def get_shop
+00002680: 7069 6e67 5f64 6179 7328 7965 6172 3a20  ping_days(year: 
+00002690: 696e 742c 0d0a 2020 2020 2020 2020 2020  int,..          
+000026a0: 2020 2020 2020 2020 2020 2020 696e 636c              incl
+000026b0: 7564 655f 7361 7475 7264 6179 3a20 626f  ude_saturday: bo
+000026c0: 6f6c 203d 2054 7275 652c 0d0a 2020 2020  ol = True,..    
+000026d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026e0: 2020 696e 636c 7564 655f 7375 6e64 6179    include_sunday
+000026f0: 3a20 626f 6f6c 203d 2054 7275 652c 0d0a  : bool = True,..
+00002700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002710: 2020 2020 2020 6578 636c 7564 655f 7368        exclude_sh
+00002720: 6f70 7069 6e67 5f72 6573 7472 6963 6564  opping_restriced
+00002730: 5f64 6179 733a 2062 6f6f 6c20 3d20 5472  _days: bool = Tr
+00002740: 7565 2920 2d3e 206c 6973 743a 0d0a 2020  ue) -> list:..  
+00002750: 2020 2222 220d 0a20 2020 2047 6574 7320    """..    Gets 
+00002760: 616c 6c20 7368 6f70 7069 6e67 2064 6179  all shopping day
+00002770: 7320 696e 2061 2067 6976 656e 2079 6561  s in a given yea
+00002780: 722e 2046 756c 6c20 7965 6172 2072 6574  r. Full year ret
+00002790: 7572 6e65 6420 6966 2061 6c6c 2070 6172  urned if all par
+000027a0: 616d 6574 6572 7320 6172 6520 5472 7565  ameters are True
+000027b0: 2e20 506f 7373 6962 696c 6974 7920 746f  . Possibility to
+000027c0: 2063 6f6d 6269 6e65 0d0a 2020 2020 7061   combine..    pa
+000027d0: 7261 6d65 7465 7273 0d0a 0d0a 2020 2020  rameters....    
+000027e0: 3a70 6172 616d 2079 6561 723a 2044 6573  :param year: Des
+000027f0: 6972 6564 2079 6561 7220 746f 2067 656e  ired year to gen
+00002800: 6572 6174 6520 686f 6c69 6461 7973 2028  erate holidays (
+00002810: 696e 7429 0d0a 2020 2020 3a70 6172 616d  int)..    :param
+00002820: 2069 6e63 6c75 6465 5f73 6174 7572 6461   include_saturda
+00002830: 793a 2049 6e63 6c75 6465 7320 616c 736f  y: Includes also
+00002840: 2053 6174 7572 6461 7973 2069 6e20 6f75   Saturdays in ou
+00002850: 7470 7574 0d0a 2020 2020 3a70 6172 616d  tput..    :param
+00002860: 2069 6e63 6c75 6465 5f73 756e 6461 793a   include_sunday:
+00002870: 2049 6e63 6c75 6465 7320 616c 736f 2053   Includes also S
+00002880: 756e 6461 7973 2069 6e20 6f75 7470 7574  undays in output
+00002890: 0d0a 2020 2020 3a70 6172 616d 2065 7863  ..    :param exc
+000028a0: 6c75 6465 5f73 686f 7070 696e 675f 7265  lude_shopping_re
+000028b0: 7374 7269 6365 645f 6461 7973 3a20 4578  striced_days: Ex
+000028c0: 636c 7564 6573 2073 686f 7070 696e 6720  cludes shopping 
+000028d0: 7265 7374 7269 6374 6564 2064 6179 7320  restricted days 
+000028e0: 696e 206f 7574 7075 740d 0a20 2020 203a  in output..    :
+000028f0: 7265 7475 726e 3a20 4c69 7374 206f 6620  return: List of 
+00002900: 616c 6c20 7368 6f70 7069 6e67 2064 6179  all shopping day
+00002910: 7320 2d3e 205b 6461 7465 7469 6d65 2e64  s -> [datetime.d
+00002920: 6174 6528 3230 3233 2c20 312c 2032 292c  ate(2023, 1, 2),
+00002930: 202e 2e2e 5d0d 0a20 2020 2022 2222 0d0a   ...]..    """..
+00002940: 0d0a 2020 2020 7765 656b 656e 645f 6461  ..    weekend_da
+00002950: 7973 203d 206c 6973 7428 290d 0a20 2020  ys = list()..   
+00002960: 2069 6620 6e6f 7420 696e 636c 7564 655f   if not include_
+00002970: 7375 6e64 6179 3a0d 0a20 2020 2020 2020  sunday:..       
+00002980: 2077 6565 6b65 6e64 5f64 6179 732e 6170   weekend_days.ap
+00002990: 7065 6e64 2822 5375 6e64 6179 2229 0d0a  pend("Sunday")..
+000029a0: 2020 2020 6966 206e 6f74 2069 6e63 6c75      if not inclu
+000029b0: 6465 5f73 6174 7572 6461 793a 0d0a 2020  de_saturday:..  
+000029c0: 2020 2020 2020 7765 656b 656e 645f 6461        weekend_da
+000029d0: 7973 2e61 7070 656e 6428 2253 6174 7572  ys.append("Satur
+000029e0: 6461 7922 290d 0a0d 0a20 2020 2069 6620  day")....    if 
+000029f0: 6578 636c 7564 655f 7368 6f70 7069 6e67  exclude_shopping
+00002a00: 5f72 6573 7472 6963 6564 5f64 6179 733a  _restriced_days:
+00002a10: 0d0a 2020 2020 2020 2020 7368 6f70 7069  ..        shoppi
+00002a20: 6e67 5f72 6573 7472 6963 7465 645f 6461  ng_restricted_da
+00002a30: 7973 203d 2073 6574 2868 6f6c 6964 6179  ys = set(holiday
+00002a40: 5b22 6461 7465 225d 2066 6f72 2068 6f6c  ["date"] for hol
+00002a50: 6964 6179 2069 6e20 6765 745f 686f 6c69  iday in get_holi
+00002a60: 6461 7973 2879 6561 722c 2073 686f 7070  days(year, shopp
+00002a70: 696e 675f 7265 7374 7269 6374 6564 3d54  ing_restricted=T
+00002a80: 7275 6529 290d 0a20 2020 2065 6c73 653a  rue))..    else:
+00002a90: 0d0a 2020 2020 2020 2020 7368 6f70 7069  ..        shoppi
+00002aa0: 6e67 5f72 6573 7472 6963 7465 645f 6461  ng_restricted_da
+00002ab0: 7973 203d 2073 6574 2829 0d0a 0d0a 2020  ys = set()....  
+00002ac0: 2020 616c 6c5f 7368 6f70 7069 6e67 5f64    all_shopping_d
+00002ad0: 6179 7320 3d20 6c69 7374 2829 0d0a 2020  ays = list()..  
+00002ae0: 2020 7374 6172 745f 6461 7465 203d 2064    start_date = d
+00002af0: 6174 6528 7965 6172 2c20 312c 2031 290d  ate(year, 1, 1).
+00002b00: 0a20 2020 2065 6e64 5f64 6174 6520 3d20  .    end_date = 
+00002b10: 6461 7465 2879 6561 722c 2031 322c 2033  date(year, 12, 3
+00002b20: 3129 0d0a 0d0a 2020 2020 7768 696c 6520  1)....    while 
+00002b30: 7374 6172 745f 6461 7465 203c 3d20 656e  start_date <= en
+00002b40: 645f 6461 7465 3a0d 0a20 2020 2020 2020  d_date:..       
+00002b50: 2069 6620 7374 6172 745f 6461 7465 2e73   if start_date.s
+00002b60: 7472 6674 696d 6528 2225 4122 2920 6e6f  trftime("%A") no
+00002b70: 7420 696e 2077 6565 6b65 6e64 5f64 6179  t in weekend_day
+00002b80: 7320 616e 6420 7374 6172 745f 6461 7465  s and start_date
+00002b90: 206e 6f74 2069 6e20 7368 6f70 7069 6e67   not in shopping
+00002ba0: 5f72 6573 7472 6963 7465 645f 6461 7973  _restricted_days
+00002bb0: 3a0d 0a20 2020 2020 2020 2020 2020 2061  :..            a
+00002bc0: 6c6c 5f73 686f 7070 696e 675f 6461 7973  ll_shopping_days
+00002bd0: 2e61 7070 656e 6428 7374 6172 745f 6461  .append(start_da
+00002be0: 7465 290d 0a20 2020 2020 2020 2073 7461  te)..        sta
+00002bf0: 7274 5f64 6174 6520 2b3d 2074 696d 6564  rt_date += timed
+00002c00: 656c 7461 2864 6179 733d 3129 0d0a 0d0a  elta(days=1)....
+00002c10: 2020 2020 7265 7475 726e 2061 6c6c 5f73      return all_s
+00002c20: 686f 7070 696e 675f 6461 7973 0d0a 0d0a  hopping_days....
+00002c30: 0d0a 6465 6620 6765 745f 686f 6c69 6461  ..def get_holida
+00002c40: 7973 5f64 7572 696e 675f 7765 656b 656e  ys_during_weeken
+00002c50: 6428 7965 6172 3a20 696e 7429 202d 3e20  d(year: int) -> 
+00002c60: 6c69 7374 3a0d 0a20 2020 2068 6f6c 6964  list:..    holid
+00002c70: 6179 5f64 6174 6573 203d 206c 6973 7428  ay_dates = list(
+00002c80: 686f 6c69 6461 795b 2264 6174 6522 5d20  holiday["date"] 
+00002c90: 666f 7220 686f 6c69 6461 7920 696e 2067  for holiday in g
+00002ca0: 6574 5f68 6f6c 6964 6179 7328 7965 6172  et_holidays(year
+00002cb0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00002cc0: 2020 2020 2020 2020 2020 2069 6620 686f             if ho
+00002cd0: 6c69 6461 795b 2264 6174 6522 5d2e 7374  liday["date"].st
+00002ce0: 7266 7469 6d65 2822 2541 2229 2069 6e20  rftime("%A") in 
+00002cf0: 2822 5361 7475 7264 6179 222c 2022 5375  ("Saturday", "Su
+00002d00: 6e64 6179 2229 290d 0a0d 0a20 2020 2072  nday"))....    r
+00002d10: 6574 7572 6e20 686f 6c69 6461 795f 6461  eturn holiday_da
+00002d20: 7465 730d 0a                             tes..
```

### Comparing `czech_workdays_holidays-0.0.9/pyproject.toml` & `czech_workdays_holidays-0.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 
 [build-system]
 requires = [
     "setuptools >= 42.0.0",
-    # Add other build system dependencies here
-    "python-dateutil >= 2.8.2",
-    "six >= 1.16.0"
+    "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "czech_workdays_holidays"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="David Gamba", email="gamba.d@seznam.cz" },
 ]
 description = "Czech Workdays and Holidays including work-restricted holidays"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
-
+dependencies = [
+    "python-dateutil >= 2.8.2",
+    "six >= 1.16.0"
+]
 
 [project.urls]
 "Homepage" = "https://github.com/david-gamba/Czech-Working-Days"
-"Bug Tracker" = "https://github.com/david-gamba/Czech-Working-Days/issues"
+"Bug Tracker" = "https://github.com/david-gamba/Czech-Working-Days/issues"
+
```

