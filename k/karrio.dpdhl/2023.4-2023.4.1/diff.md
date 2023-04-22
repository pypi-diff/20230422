# Comparing `tmp/karrio.dpdhl-2023.4-py3-none-any.whl.zip` & `tmp/karrio.dpdhl-2023.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 14351 bytes, number of entries: 16
--rw-rw-r--  2.0 unx      558 b- defN 23-Apr-15 11:02 karrio/mappers/dpdhl/__init__.py
--rw-rw-r--  2.0 unx     2030 b- defN 23-Apr-01 13:34 karrio/mappers/dpdhl/mapper.py
--rw-rw-r--  2.0 unx     2304 b- defN 23-Apr-01 12:45 karrio/mappers/dpdhl/proxy.py
--rw-rw-r--  2.0 unx     1021 b- defN 23-Apr-15 11:01 karrio/mappers/dpdhl/settings.py
+Zip file size: 14414 bytes, number of entries: 16
+-rw-rw-r--  2.0 unx      558 b- defN 23-Apr-20 21:26 karrio/mappers/dpdhl/__init__.py
+-rw-rw-r--  2.0 unx     2030 b- defN 23-Apr-20 21:26 karrio/mappers/dpdhl/mapper.py
+-rw-rw-r--  2.0 unx     2387 b- defN 23-Apr-22 03:19 karrio/mappers/dpdhl/proxy.py
+-rw-rw-r--  2.0 unx     1021 b- defN 23-Apr-20 21:26 karrio/mappers/dpdhl/settings.py
 -rw-rw-r--  2.0 unx      313 b- defN 22-Nov-15 19:21 karrio/providers/dpdhl/__init__.py
 -rw-rw-r--  2.0 unx     3115 b- defN 23-Mar-29 20:04 karrio/providers/dpdhl/error.py
--rw-rw-r--  2.0 unx     3657 b- defN 23-Apr-10 06:24 karrio/providers/dpdhl/tracking.py
--rw-rw-r--  2.0 unx     7670 b- defN 23-Apr-15 11:00 karrio/providers/dpdhl/units.py
--rw-rw-r--  2.0 unx     1684 b- defN 23-Apr-15 11:02 karrio/providers/dpdhl/utils.py
+-rw-rw-r--  2.0 unx     3657 b- defN 23-Apr-20 21:26 karrio/providers/dpdhl/tracking.py
+-rw-rw-r--  2.0 unx     7670 b- defN 23-Apr-20 21:26 karrio/providers/dpdhl/units.py
+-rw-rw-r--  2.0 unx     1684 b- defN 23-Apr-20 21:26 karrio/providers/dpdhl/utils.py
 -rw-rw-r--  2.0 unx      226 b- defN 22-Nov-15 19:21 karrio/providers/dpdhl/shipment/__init__.py
--rw-rw-r--  2.0 unx     2425 b- defN 23-Apr-01 15:18 karrio/providers/dpdhl/shipment/cancel.py
--rw-rw-r--  2.0 unx    19559 b- defN 23-Apr-01 15:18 karrio/providers/dpdhl/shipment/create.py
--rw-rw-r--  2.0 unx      992 b- defN 23-Apr-18 07:09 karrio.dpdhl-2023.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 07:09 karrio.dpdhl-2023.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Apr-18 07:09 karrio.dpdhl-2023.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1411 b- defN 23-Apr-18 07:09 karrio.dpdhl-2023.4.dist-info/RECORD
-16 files, 47064 bytes uncompressed, 11991 bytes compressed:  74.5%
+-rw-rw-r--  2.0 unx     2425 b- defN 23-Apr-20 21:26 karrio/providers/dpdhl/shipment/cancel.py
+-rw-rw-r--  2.0 unx    19559 b- defN 23-Apr-20 21:26 karrio/providers/dpdhl/shipment/create.py
+-rw-rw-r--  2.0 unx      994 b- defN 23-Apr-22 03:34 karrio.dpdhl-2023.4.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-22 03:34 karrio.dpdhl-2023.4.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-22 03:34 karrio.dpdhl-2023.4.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1419 b- defN 23-Apr-22 03:34 karrio.dpdhl-2023.4.1.dist-info/RECORD
+16 files, 47157 bytes uncompressed, 12038 bytes compressed:  74.5%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: karrio/providers/dpdhl/shipment/cancel.py
 Comment: 
 
 Filename: karrio/providers/dpdhl/shipment/create.py
 Comment: 
 
-Filename: karrio.dpdhl-2023.4.dist-info/METADATA
+Filename: karrio.dpdhl-2023.4.1.dist-info/METADATA
 Comment: 
 
-Filename: karrio.dpdhl-2023.4.dist-info/WHEEL
+Filename: karrio.dpdhl-2023.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.dpdhl-2023.4.dist-info/top_level.txt
+Filename: karrio.dpdhl-2023.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.dpdhl-2023.4.dist-info/RECORD
+Filename: karrio.dpdhl-2023.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/mappers/dpdhl/proxy.py

```diff
@@ -46,18 +46,19 @@
         return lib.Deserializable(response, to_element)
 
     def get_tracking(self, requests: lib.Serializable) -> lib.Deserializable:
         def _track(data):
             return lib.request(
                 url=f"{self.settings.server_url}/rest/sendungsverfolgung",
                 trace=self.trace_as("xml"),
+                data=dict(xml=data),
                 method="POST",
-                data=data,
                 headers={
                     "Authorization": f"Basic {self.settings.basic_authentication}",
+                    "Content-Type": "application/x-www-form-urlencoded",
                 },
             )
 
         responses = lib.run_concurently(_track, requests.serialize())
 
         return lib.Deserializable(
             responses, lambda results: [lib.to_element(res) for res in results]
```

## Comparing `karrio.dpdhl-2023.4.dist-info/METADATA` & `karrio.dpdhl-2023.4.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karrio.dpdhl
-Version: 2023.4
+Version: 2023.4.1
 Summary: Karrio - Deutsche Post DHL Shipping extension
 Home-page: https://github.com/karrioapi/karrio
 Author: karrio
 Author-email: hello@karrio.io
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

## Comparing `karrio.dpdhl-2023.4.dist-info/RECORD` & `karrio.dpdhl-2023.4.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 karrio/mappers/dpdhl/__init__.py,sha256=hI9K0SVajo90niTvmU5BP9iV2QoOFh8tEbtZfVRax_c,558
 karrio/mappers/dpdhl/mapper.py,sha256=PX1mAMSFl8JmtAQ-SaKr8xDrV0eybOXzNLJbrUGKLfM,2030
-karrio/mappers/dpdhl/proxy.py,sha256=vb326Ib_UphV7npB_YfNis1vr-0tt1gv4o1Efao3nCo,2304
+karrio/mappers/dpdhl/proxy.py,sha256=YxIR8gxYUfnEYmQMopojo3CHnfUI3uPsYq84Y4DDM3E,2387
 karrio/mappers/dpdhl/settings.py,sha256=nRq7QoFa8Amrg1glJy_UmZ9fQUxuseC8KNKPltbifm0,1021
 karrio/providers/dpdhl/__init__.py,sha256=XtaZQrNssm_oho6v6SAYEH3cViuOZ3VFAPhHgW6f-yw,313
 karrio/providers/dpdhl/error.py,sha256=VoSZ2pyx3nUudmqX3L0nIMQ2yOVlvfr_GJ8DrlczDj4,3115
 karrio/providers/dpdhl/tracking.py,sha256=Qn2luGRnyIlJkaa2JSRjlawLVq-jMnAkfFGRcJFugqc,3657
 karrio/providers/dpdhl/units.py,sha256=DDQX6MIFiYqMXl6exNkXfRbolbRD2czyMqeAcvMSk1w,7670
 karrio/providers/dpdhl/utils.py,sha256=Hdf1-fC0uK3SlNJlVb5ZlHshn2nC6hH61wO-EFvvCws,1684
 karrio/providers/dpdhl/shipment/__init__.py,sha256=5tF7dih8kTSVa5pw4UXU8_byCMnuvtsJIz_h7VAOOyY,226
 karrio/providers/dpdhl/shipment/cancel.py,sha256=1Z_h5EUUNLS7LAiLLU04dkEPufmXSJGavvn543FGxQE,2425
 karrio/providers/dpdhl/shipment/create.py,sha256=AKmTE_tcKX3n7wStuyFZGJXU5H8J40WgqZqLVSV96gg,19559
-karrio.dpdhl-2023.4.dist-info/METADATA,sha256=UntfvEJxvKqL1raSR0Jn_hSSprXZ1rrAgv1AhXTxN24,992
-karrio.dpdhl-2023.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-karrio.dpdhl-2023.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
-karrio.dpdhl-2023.4.dist-info/RECORD,,
+karrio.dpdhl-2023.4.1.dist-info/METADATA,sha256=ziwQbGnRnZ4AqdzsvEcVFgDuEX0YW4vZbIMAdbBJWrk,994
+karrio.dpdhl-2023.4.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+karrio.dpdhl-2023.4.1.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
+karrio.dpdhl-2023.4.1.dist-info/RECORD,,
```

