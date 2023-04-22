# Comparing `tmp/ovos_intent_plugin_adapt-0.0.0a6-py3-none-any.whl.zip` & `tmp/ovos_intent_plugin_adapt-0.0.0a7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 8027 bytes, number of entries: 9
--rw-r--r--  2.0 unx     5266 b- defN 23-Apr-22 07:21 ovos_intent_plugin_adapt/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 23-Apr-22 07:21 ovos_intent_plugin_adapt/version.py
--rw-r--r--  2.0 unx    11349 b- defN 23-Apr-22 07:21 ovos_intent_plugin_adapt-0.0.0a6.dist-info/LICENSE
--rw-r--r--  2.0 unx      718 b- defN 23-Apr-22 07:21 ovos_intent_plugin_adapt-0.0.0a6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-22 07:21 ovos_intent_plugin_adapt-0.0.0a6.dist-info/WHEEL
--rw-r--r--  2.0 unx       85 b- defN 23-Apr-22 07:21 ovos_intent_plugin_adapt-0.0.0a6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       25 b- defN 23-Apr-22 07:21 ovos_intent_plugin_adapt-0.0.0a6.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-22 07:21 ovos_intent_plugin_adapt-0.0.0a6.dist-info/zip-safe
--rw-rw-r--  2.0 unx      884 b- defN 23-Apr-22 07:21 ovos_intent_plugin_adapt-0.0.0a6.dist-info/RECORD
-9 files, 18597 bytes uncompressed, 6451 bytes compressed:  65.3%
+Zip file size: 8096 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     5619 b- defN 23-Apr-22 09:27 ovos_intent_plugin_adapt/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Apr-22 09:27 ovos_intent_plugin_adapt/version.py
+-rw-r--r--  2.0 unx    11349 b- defN 23-Apr-22 09:27 ovos_intent_plugin_adapt-0.0.0a7.dist-info/LICENSE
+-rw-r--r--  2.0 unx      718 b- defN 23-Apr-22 09:27 ovos_intent_plugin_adapt-0.0.0a7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-22 09:27 ovos_intent_plugin_adapt-0.0.0a7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       85 b- defN 23-Apr-22 09:27 ovos_intent_plugin_adapt-0.0.0a7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       25 b- defN 23-Apr-22 09:27 ovos_intent_plugin_adapt-0.0.0a7.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-22 09:27 ovos_intent_plugin_adapt-0.0.0a7.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      884 b- defN 23-Apr-22 09:27 ovos_intent_plugin_adapt-0.0.0a7.dist-info/RECORD
+9 files, 18950 bytes uncompressed, 6520 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: ovos_intent_plugin_adapt/__init__.py
 Comment: 
 
 Filename: ovos_intent_plugin_adapt/version.py
 Comment: 
 
-Filename: ovos_intent_plugin_adapt-0.0.0a6.dist-info/LICENSE
+Filename: ovos_intent_plugin_adapt-0.0.0a7.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_intent_plugin_adapt-0.0.0a6.dist-info/METADATA
+Filename: ovos_intent_plugin_adapt-0.0.0a7.dist-info/METADATA
 Comment: 
 
-Filename: ovos_intent_plugin_adapt-0.0.0a6.dist-info/WHEEL
+Filename: ovos_intent_plugin_adapt-0.0.0a7.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_intent_plugin_adapt-0.0.0a6.dist-info/entry_points.txt
+Filename: ovos_intent_plugin_adapt-0.0.0a7.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_intent_plugin_adapt-0.0.0a6.dist-info/top_level.txt
+Filename: ovos_intent_plugin_adapt-0.0.0a7.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_intent_plugin_adapt-0.0.0a6.dist-info/zip-safe
+Filename: ovos_intent_plugin_adapt-0.0.0a7.dist-info/zip-safe
 Comment: 
 
-Filename: ovos_intent_plugin_adapt-0.0.0a6.dist-info/RECORD
+Filename: ovos_intent_plugin_adapt-0.0.0a7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_intent_plugin_adapt/__init__.py

```diff
@@ -1,11 +1,11 @@
 from adapt.engine import IntentDeterminationEngine
 from adapt.intent import IntentBuilder
 from ovos_bus_client.session import SessionManager
-from ovos_plugin_manager.intents import IntentExtractor, IntentPriority, IntentDeterminationStrategy
+from ovos_plugin_manager.intents import IntentExtractor, IntentPriority, IntentDeterminationStrategy, IntentMatch
 from ovos_utils.log import LOG
 
 
 class AdaptExtractor(IntentExtractor):
     def __init__(self, config=None,
                  strategy=IntentDeterminationStrategy.SEGMENT_REMAINDER,
                  priority=IntentPriority.KEYWORDS_HIGH,
@@ -89,18 +89,22 @@
                 intent["entities"] = {}
                 for k in matches:
                     intent["entities"][k] = intent.pop(k)
                 intent["conf"] = intent.pop("confidence")
                 intent["utterance"] = utterance
                 intent["intent_engine"] = "adapt"
 
-                remainder = self.get_utterance_remainder(
-                    utterance, samples=[v for v in matches.values()])
+                remainder = self.get_utterance_remainder(utterance, samples=[v for v in matches.values()])
                 intent["utterance_remainder"] = remainder
-                return intent
+                skill_id = self.get_intent_skill_id(intent["intent_type"])
+                return IntentMatch(intent_service=intent["intent_engine"],
+                                   intent_type=intent["intent_type"],
+                                   intent_data=intent,
+                                   confidence=intent["conf"],
+                                   skill_id=skill_id)
         return None
 
     def detach_intent(self, intent_name):
         super().detach_intent(intent_name)
         LOG.debug("detaching adapt intent: " + intent_name)
         for lang in self.engines:
             new_parsers = [p for p in self.engines[lang].intent_parsers
```

## ovos_intent_plugin_adapt/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 0
-VERSION_ALPHA = 6
+VERSION_ALPHA = 7
 # END_VERSION_BLOCK
```

## Comparing `ovos_intent_plugin_adapt-0.0.0a6.dist-info/LICENSE` & `ovos_intent_plugin_adapt-0.0.0a7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ovos_intent_plugin_adapt-0.0.0a6.dist-info/METADATA` & `ovos_intent_plugin_adapt-0.0.0a7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-intent-plugin-adapt
-Version: 0.0.0a6
+Version: 0.0.0a7
 Summary: A intent plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-intent-plugin-adapt
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

