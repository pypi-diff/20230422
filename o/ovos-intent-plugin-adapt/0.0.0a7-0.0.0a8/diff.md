# Comparing `tmp/ovos_intent_plugin_adapt-0.0.0a7-py3-none-any.whl.zip` & `tmp/ovos_intent_plugin_adapt-0.0.0a8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 8096 bytes, number of entries: 9
--rw-r--r--  2.0 unx     5619 b- defN 23-Apr-22 09:27 ovos_intent_plugin_adapt/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 23-Apr-22 09:27 ovos_intent_plugin_adapt/version.py
--rw-r--r--  2.0 unx    11349 b- defN 23-Apr-22 09:27 ovos_intent_plugin_adapt-0.0.0a7.dist-info/LICENSE
--rw-r--r--  2.0 unx      718 b- defN 23-Apr-22 09:27 ovos_intent_plugin_adapt-0.0.0a7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-22 09:27 ovos_intent_plugin_adapt-0.0.0a7.dist-info/WHEEL
--rw-r--r--  2.0 unx       85 b- defN 23-Apr-22 09:27 ovos_intent_plugin_adapt-0.0.0a7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       25 b- defN 23-Apr-22 09:27 ovos_intent_plugin_adapt-0.0.0a7.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-22 09:27 ovos_intent_plugin_adapt-0.0.0a7.dist-info/zip-safe
--rw-rw-r--  2.0 unx      884 b- defN 23-Apr-22 09:27 ovos_intent_plugin_adapt-0.0.0a7.dist-info/RECORD
-9 files, 18950 bytes uncompressed, 6520 bytes compressed:  65.6%
+Zip file size: 8115 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     5609 b- defN 23-Apr-22 10:19 ovos_intent_plugin_adapt/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Apr-22 10:19 ovos_intent_plugin_adapt/version.py
+-rw-r--r--  2.0 unx    11349 b- defN 23-Apr-22 10:19 ovos_intent_plugin_adapt-0.0.0a8.dist-info/LICENSE
+-rw-r--r--  2.0 unx      718 b- defN 23-Apr-22 10:19 ovos_intent_plugin_adapt-0.0.0a8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-22 10:19 ovos_intent_plugin_adapt-0.0.0a8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       85 b- defN 23-Apr-22 10:19 ovos_intent_plugin_adapt-0.0.0a8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       25 b- defN 23-Apr-22 10:19 ovos_intent_plugin_adapt-0.0.0a8.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-22 10:19 ovos_intent_plugin_adapt-0.0.0a8.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      884 b- defN 23-Apr-22 10:19 ovos_intent_plugin_adapt-0.0.0a8.dist-info/RECORD
+9 files, 18940 bytes uncompressed, 6539 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: ovos_intent_plugin_adapt/__init__.py
 Comment: 
 
 Filename: ovos_intent_plugin_adapt/version.py
 Comment: 
 
-Filename: ovos_intent_plugin_adapt-0.0.0a7.dist-info/LICENSE
+Filename: ovos_intent_plugin_adapt-0.0.0a8.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_intent_plugin_adapt-0.0.0a7.dist-info/METADATA
+Filename: ovos_intent_plugin_adapt-0.0.0a8.dist-info/METADATA
 Comment: 
 
-Filename: ovos_intent_plugin_adapt-0.0.0a7.dist-info/WHEEL
+Filename: ovos_intent_plugin_adapt-0.0.0a8.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_intent_plugin_adapt-0.0.0a7.dist-info/entry_points.txt
+Filename: ovos_intent_plugin_adapt-0.0.0a8.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_intent_plugin_adapt-0.0.0a7.dist-info/top_level.txt
+Filename: ovos_intent_plugin_adapt-0.0.0a8.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_intent_plugin_adapt-0.0.0a7.dist-info/zip-safe
+Filename: ovos_intent_plugin_adapt-0.0.0a8.dist-info/zip-safe
 Comment: 
 
-Filename: ovos_intent_plugin_adapt-0.0.0a7.dist-info/RECORD
+Filename: ovos_intent_plugin_adapt-0.0.0a8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_intent_plugin_adapt/__init__.py

```diff
@@ -1,14 +1,22 @@
 from adapt.engine import IntentDeterminationEngine
 from adapt.intent import IntentBuilder
 from ovos_bus_client.session import SessionManager
 from ovos_plugin_manager.intents import IntentExtractor, IntentPriority, IntentDeterminationStrategy, IntentMatch
 from ovos_utils.log import LOG
 
 
+def _munge(name, skill_id):
+    return f"{name}:{skill_id}"
+
+
+def _unmunge(munged):
+    return munged.split(":", 2)
+
+
 class AdaptExtractor(IntentExtractor):
     def __init__(self, config=None,
                  strategy=IntentDeterminationStrategy.SEGMENT_REMAINDER,
                  priority=IntentPriority.KEYWORDS_HIGH,
                  segmenter=None):
         super().__init__(config, strategy=strategy, priority=priority, segmenter=segmenter)
         self.engines = {}  # lang: IntentDeterminationEngine
@@ -17,49 +25,54 @@
 
     def _get_engine(self, lang=None):
         lang = lang or self.lang
         if lang not in self.engines:
             self.engines[lang] = IntentDeterminationEngine()
         return self.engines[lang]
 
-    def register_entity(self, entity_name, samples=None, lang=None):
+    def register_entity(self, skill_id, entity_name, samples=None, lang=None):
         samples = samples or [entity_name]
+        super().register_entity(skill_id, entity_name, samples, lang)
         engine = self._get_engine(lang)
         for kw in samples:
             engine.register_entity(kw, entity_name)
-        super().register_entity(entity_name, samples, lang)
 
-    def register_regex_entity(self, entity_name, samples, lang=None):
+    def register_regex_entity(self, skill_id, entity_name, samples, lang=None):
+        lang = lang or self._excludes
+        super().register_regex_entity(skill_id, entity_name, samples, lang)
         engine = self._get_engine(lang)
         if isinstance(samples, str):
             engine.register_regex_entity(samples)
         if isinstance(samples, list):
             for s in samples:
                 engine.register_regex_entity(s)
-        super().register_regex_entity(entity_name, samples, lang)
 
-    def register_regex_intent(self, intent_name, samples, lang=None):
-        self.register_regex_entity(intent_name, samples)
-        self.register_keyword_intent(intent_name, [intent_name])
-        super().register_regex_intent(intent_name, samples, lang)
+    def register_regex_intent(self, skill_id, intent_name, samples, lang=None):
+        self.register_regex_entity(skill_id, intent_name, samples)
+        self.register_keyword_intent(skill_id, intent_name, [intent_name])
+        super().register_regex_intent(skill_id, intent_name, samples, lang)
 
-    def register_keyword_intent(self, intent_name,
+    def register_keyword_intent(self, skill_id, intent_name,
                                 keywords=None,
                                 optional=None,
                                 at_least_one=None,
                                 excluded=None,
                                 lang=None):
+        lang = lang or self.lang
+        super().register_keyword_intent(skill_id, intent_name, keywords, optional, at_least_one, excluded, lang)
+
         engine = self._get_engine(lang)
+        intent_name = _munge(intent_name, skill_id)
+
         if not keywords:
             keywords = keywords or [intent_name]
             self.register_entity(intent_name, keywords)
         optional = optional or []
         excluded = excluded or []
         at_least_one = at_least_one or []
-        super().register_keyword_intent(intent_name, keywords, optional, at_least_one, excluded, lang)
 
         # structure intent
         intent = IntentBuilder(intent_name)
         for kw in keywords:
             intent.require(kw)
         for kw in optional:
             intent.optionally(kw)
@@ -91,32 +104,23 @@
                     intent["entities"][k] = intent.pop(k)
                 intent["conf"] = intent.pop("confidence")
                 intent["utterance"] = utterance
                 intent["intent_engine"] = "adapt"
 
                 remainder = self.get_utterance_remainder(utterance, samples=[v for v in matches.values()])
                 intent["utterance_remainder"] = remainder
-                skill_id = self.get_intent_skill_id(intent["intent_type"])
+                intent_type, skill_id = _unmunge(intent["intent_type"])
                 return IntentMatch(intent_service=intent["intent_engine"],
-                                   intent_type=intent["intent_type"],
+                                   intent_type=intent_type,
                                    intent_data=intent,
                                    confidence=intent["conf"],
                                    skill_id=skill_id)
         return None
 
-    def detach_intent(self, intent_name):
+    def detach_intent(self, skill_id, intent_name):
         super().detach_intent(intent_name)
         LOG.debug("detaching adapt intent: " + intent_name)
+        intent_name = _munge(intent_name, skill_id)
         for lang in self.engines:
             new_parsers = [p for p in self.engines[lang].intent_parsers
                            if p.name != intent_name]
             self.engines[lang].intent_parsers = new_parsers
-
-    def detach_skill(self, skill_id):
-        super().detach_skill(skill_id)
-        LOG.debug("detaching adapt skill: " + skill_id)
-        for lang in self.engines:
-            new_parsers = [
-                p.name for p in self.engines[lang].intent_parsers if
-                p.name.startswith(skill_id)]
-            for intent_name in new_parsers:
-                self.detach_intent(intent_name)
```

## ovos_intent_plugin_adapt/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 0
-VERSION_ALPHA = 7
+VERSION_ALPHA = 8
 # END_VERSION_BLOCK
```

## Comparing `ovos_intent_plugin_adapt-0.0.0a7.dist-info/LICENSE` & `ovos_intent_plugin_adapt-0.0.0a8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ovos_intent_plugin_adapt-0.0.0a7.dist-info/METADATA` & `ovos_intent_plugin_adapt-0.0.0a8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-intent-plugin-adapt
-Version: 0.0.0a7
+Version: 0.0.0a8
 Summary: A intent plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-intent-plugin-adapt
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `ovos_intent_plugin_adapt-0.0.0a7.dist-info/RECORD` & `ovos_intent_plugin_adapt-0.0.0a8.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-ovos_intent_plugin_adapt/__init__.py,sha256=6eV4SFQRDDn27JnDeg45AONhaPE6cWI_OrpdFWZ5HQk,5619
-ovos_intent_plugin_adapt/version.py,sha256=o2Kw6ltw3pS_eY-5DpR5D4-wD7S7FycR-UAJvetFWDQ,177
-ovos_intent_plugin_adapt-0.0.0a7.dist-info/LICENSE,sha256=fYHkowW9JcaEcqCPTXYBayNJ9J1lGdYVb7Mf9oy6oEY,11349
-ovos_intent_plugin_adapt-0.0.0a7.dist-info/METADATA,sha256=X8xc8n9mQ4b8fHVjnwe32bJoJlrEmLb8Y_8QJW9oIp4,718
-ovos_intent_plugin_adapt-0.0.0a7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ovos_intent_plugin_adapt-0.0.0a7.dist-info/entry_points.txt,sha256=xmLxLIuOBqpzb7-OotaCjDd6qd77Q296YoC_XRkBvIY,85
-ovos_intent_plugin_adapt-0.0.0a7.dist-info/top_level.txt,sha256=9MnjpB7sRpiWg2yL3L6ov8iCQrpRcGIj5TgZRVygz6U,25
-ovos_intent_plugin_adapt-0.0.0a7.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-ovos_intent_plugin_adapt-0.0.0a7.dist-info/RECORD,,
+ovos_intent_plugin_adapt/__init__.py,sha256=7yqg4mN26g9RVEJ633OkNceJdDDaPfu5oLP9bRgnWSU,5609
+ovos_intent_plugin_adapt/version.py,sha256=jROWGT-Mw8cV_AbHNBA76Qf4fFCUPjxw7CsgxvHHiAA,177
+ovos_intent_plugin_adapt-0.0.0a8.dist-info/LICENSE,sha256=fYHkowW9JcaEcqCPTXYBayNJ9J1lGdYVb7Mf9oy6oEY,11349
+ovos_intent_plugin_adapt-0.0.0a8.dist-info/METADATA,sha256=jI73VbJ05dk7QLnOFWoeIG0YwWwczLst2TvZ84eBxAM,718
+ovos_intent_plugin_adapt-0.0.0a8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ovos_intent_plugin_adapt-0.0.0a8.dist-info/entry_points.txt,sha256=xmLxLIuOBqpzb7-OotaCjDd6qd77Q296YoC_XRkBvIY,85
+ovos_intent_plugin_adapt-0.0.0a8.dist-info/top_level.txt,sha256=9MnjpB7sRpiWg2yL3L6ov8iCQrpRcGIj5TgZRVygz6U,25
+ovos_intent_plugin_adapt-0.0.0a8.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+ovos_intent_plugin_adapt-0.0.0a8.dist-info/RECORD,,
```

