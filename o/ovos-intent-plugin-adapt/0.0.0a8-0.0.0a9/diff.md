# Comparing `tmp/ovos_intent_plugin_adapt-0.0.0a8-py3-none-any.whl.zip` & `tmp/ovos_intent_plugin_adapt-0.0.0a9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 8115 bytes, number of entries: 9
--rw-r--r--  2.0 unx     5609 b- defN 23-Apr-22 10:19 ovos_intent_plugin_adapt/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 23-Apr-22 10:19 ovos_intent_plugin_adapt/version.py
--rw-r--r--  2.0 unx    11349 b- defN 23-Apr-22 10:19 ovos_intent_plugin_adapt-0.0.0a8.dist-info/LICENSE
--rw-r--r--  2.0 unx      718 b- defN 23-Apr-22 10:19 ovos_intent_plugin_adapt-0.0.0a8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-22 10:19 ovos_intent_plugin_adapt-0.0.0a8.dist-info/WHEEL
--rw-r--r--  2.0 unx       85 b- defN 23-Apr-22 10:19 ovos_intent_plugin_adapt-0.0.0a8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       25 b- defN 23-Apr-22 10:19 ovos_intent_plugin_adapt-0.0.0a8.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-22 10:19 ovos_intent_plugin_adapt-0.0.0a8.dist-info/zip-safe
--rw-rw-r--  2.0 unx      884 b- defN 23-Apr-22 10:19 ovos_intent_plugin_adapt-0.0.0a8.dist-info/RECORD
-9 files, 18940 bytes uncompressed, 6539 bytes compressed:  65.5%
+Zip file size: 8119 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     5620 b- defN 23-Apr-22 20:17 ovos_intent_plugin_adapt/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Apr-22 20:17 ovos_intent_plugin_adapt/version.py
+-rw-r--r--  2.0 unx    11349 b- defN 23-Apr-22 20:17 ovos_intent_plugin_adapt-0.0.0a9.dist-info/LICENSE
+-rw-r--r--  2.0 unx      718 b- defN 23-Apr-22 20:17 ovos_intent_plugin_adapt-0.0.0a9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-22 20:17 ovos_intent_plugin_adapt-0.0.0a9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       85 b- defN 23-Apr-22 20:17 ovos_intent_plugin_adapt-0.0.0a9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       25 b- defN 23-Apr-22 20:17 ovos_intent_plugin_adapt-0.0.0a9.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-22 20:17 ovos_intent_plugin_adapt-0.0.0a9.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      884 b- defN 23-Apr-22 20:17 ovos_intent_plugin_adapt-0.0.0a9.dist-info/RECORD
+9 files, 18951 bytes uncompressed, 6543 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: ovos_intent_plugin_adapt/__init__.py
 Comment: 
 
 Filename: ovos_intent_plugin_adapt/version.py
 Comment: 
 
-Filename: ovos_intent_plugin_adapt-0.0.0a8.dist-info/LICENSE
+Filename: ovos_intent_plugin_adapt-0.0.0a9.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_intent_plugin_adapt-0.0.0a8.dist-info/METADATA
+Filename: ovos_intent_plugin_adapt-0.0.0a9.dist-info/METADATA
 Comment: 
 
-Filename: ovos_intent_plugin_adapt-0.0.0a8.dist-info/WHEEL
+Filename: ovos_intent_plugin_adapt-0.0.0a9.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_intent_plugin_adapt-0.0.0a8.dist-info/entry_points.txt
+Filename: ovos_intent_plugin_adapt-0.0.0a9.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_intent_plugin_adapt-0.0.0a8.dist-info/top_level.txt
+Filename: ovos_intent_plugin_adapt-0.0.0a9.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_intent_plugin_adapt-0.0.0a8.dist-info/zip-safe
+Filename: ovos_intent_plugin_adapt-0.0.0a9.dist-info/zip-safe
 Comment: 
 
-Filename: ovos_intent_plugin_adapt-0.0.0a8.dist-info/RECORD
+Filename: ovos_intent_plugin_adapt-0.0.0a9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_intent_plugin_adapt/__init__.py

```diff
@@ -1,11 +1,11 @@
 from adapt.engine import IntentDeterminationEngine
 from adapt.intent import IntentBuilder
 from ovos_bus_client.session import SessionManager
-from ovos_plugin_manager.intents import IntentExtractor, IntentPriority, IntentDeterminationStrategy, IntentMatch
+from ovos_plugin_manager.templates.intents import IntentExtractor, IntentPriority, IntentDeterminationStrategy, IntentMatch
 from ovos_utils.log import LOG
 
 
 def _munge(name, skill_id):
     return f"{name}:{skill_id}"
 
 
@@ -76,18 +76,19 @@
             intent.require(kw)
         for kw in optional:
             intent.optionally(kw)
         # TODO exclude functionality not yet merged
         #  https://github.com/MycroftAI/adapt/pull/156
         if excluded:
             self._excludes[intent_name] = excluded
+
         engine.register_intent_parser(intent.build())
         return intent
 
-    def calc_intent(self, utterance, min_conf=0.5, lang=None, session=None):
+    def calc_intent(self, utterance, min_conf=0.2, lang=None, session=None):
         utterance = utterance.strip()
         engine = self._get_engine(lang)
         session = session or SessionManager.get()
         for intent in engine.determine_intent(utterance, 100,
                                               include_tags=True,
                                               context_manager=session.context):
             # workaround "excludes" keyword, just drop the intent match if we find an excluded keyword in utt
```

## ovos_intent_plugin_adapt/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 0
-VERSION_ALPHA = 8
+VERSION_ALPHA = 9
 # END_VERSION_BLOCK
```

## Comparing `ovos_intent_plugin_adapt-0.0.0a8.dist-info/LICENSE` & `ovos_intent_plugin_adapt-0.0.0a9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ovos_intent_plugin_adapt-0.0.0a8.dist-info/METADATA` & `ovos_intent_plugin_adapt-0.0.0a9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-intent-plugin-adapt
-Version: 0.0.0a8
+Version: 0.0.0a9
 Summary: A intent plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-intent-plugin-adapt
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `ovos_intent_plugin_adapt-0.0.0a8.dist-info/RECORD` & `ovos_intent_plugin_adapt-0.0.0a9.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-ovos_intent_plugin_adapt/__init__.py,sha256=7yqg4mN26g9RVEJ633OkNceJdDDaPfu5oLP9bRgnWSU,5609
-ovos_intent_plugin_adapt/version.py,sha256=jROWGT-Mw8cV_AbHNBA76Qf4fFCUPjxw7CsgxvHHiAA,177
-ovos_intent_plugin_adapt-0.0.0a8.dist-info/LICENSE,sha256=fYHkowW9JcaEcqCPTXYBayNJ9J1lGdYVb7Mf9oy6oEY,11349
-ovos_intent_plugin_adapt-0.0.0a8.dist-info/METADATA,sha256=jI73VbJ05dk7QLnOFWoeIG0YwWwczLst2TvZ84eBxAM,718
-ovos_intent_plugin_adapt-0.0.0a8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ovos_intent_plugin_adapt-0.0.0a8.dist-info/entry_points.txt,sha256=xmLxLIuOBqpzb7-OotaCjDd6qd77Q296YoC_XRkBvIY,85
-ovos_intent_plugin_adapt-0.0.0a8.dist-info/top_level.txt,sha256=9MnjpB7sRpiWg2yL3L6ov8iCQrpRcGIj5TgZRVygz6U,25
-ovos_intent_plugin_adapt-0.0.0a8.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-ovos_intent_plugin_adapt-0.0.0a8.dist-info/RECORD,,
+ovos_intent_plugin_adapt/__init__.py,sha256=wEOEf4-2-UQHuBow2nXn47GrfYNmGB7fCCcdG3vQSsI,5620
+ovos_intent_plugin_adapt/version.py,sha256=Kb5BPEyIPDXlOdSV3KpYAyBQCSjGCVRDt5UYJ6ugCfI,177
+ovos_intent_plugin_adapt-0.0.0a9.dist-info/LICENSE,sha256=fYHkowW9JcaEcqCPTXYBayNJ9J1lGdYVb7Mf9oy6oEY,11349
+ovos_intent_plugin_adapt-0.0.0a9.dist-info/METADATA,sha256=NV2eNxJ70rupuhqs58z4Jii7STYT9V-xTH9vFy-EoeI,718
+ovos_intent_plugin_adapt-0.0.0a9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ovos_intent_plugin_adapt-0.0.0a9.dist-info/entry_points.txt,sha256=xmLxLIuOBqpzb7-OotaCjDd6qd77Q296YoC_XRkBvIY,85
+ovos_intent_plugin_adapt-0.0.0a9.dist-info/top_level.txt,sha256=9MnjpB7sRpiWg2yL3L6ov8iCQrpRcGIj5TgZRVygz6U,25
+ovos_intent_plugin_adapt-0.0.0a9.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+ovos_intent_plugin_adapt-0.0.0a9.dist-info/RECORD,,
```

