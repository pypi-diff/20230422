# Comparing `tmp/athena_ai-0.0.3.tar.gz` & `tmp/athena_ai-0.0.4.tar.gz`

## Comparing `athena_ai-0.0.3.tar` & `athena_ai-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,16 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 athena_ai-0.0.3/.dockerignore
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 athena_ai-0.0.3/Dockerfile
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 athena_ai-0.0.3/main.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 athena_ai-0.0.3/nlu_config.yml
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 athena_ai-0.0.3/nlu_data.md
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 athena_ai-0.0.3/requirements.txt
--rw-r--r--   0        0        0    22254 2020-02-02 00:00:00.000000 athena_ai-0.0.3/conversation_history/4_21_2023.txt
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 athena_ai-0.0.3/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 athena_ai-0.0.3/LICENSE
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 athena_ai-0.0.3/README.md
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 athena_ai-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 athena_ai-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 athena_ai-0.0.4/.dockerignore
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 athena_ai-0.0.4/Dockerfile
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 athena_ai-0.0.4/main.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 athena_ai-0.0.4/nlu_config.yml
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 athena_ai-0.0.4/nlu_data.md
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 athena_ai-0.0.4/plugin_base.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 athena_ai-0.0.4/plugin_manager.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 athena_ai-0.0.4/requirements.txt
+-rw-r--r--   0        0        0    31823 2020-02-02 00:00:00.000000 athena_ai-0.0.4/conversation_history/4_21_2023.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 athena_ai-0.0.4/plugins/__init__.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 athena_ai-0.0.4/plugins/arithmetic_plugin.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 athena_ai-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 athena_ai-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 athena_ai-0.0.4/README.md
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 athena_ai-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 athena_ai-0.0.4/PKG-INFO
```

### Comparing `athena_ai-0.0.3/Dockerfile` & `athena_ai-0.0.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `athena_ai-0.0.3/main.py` & `athena_ai-0.0.4/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 from dotenv import load_dotenv
 import openai
 from rasa_nlu.training_data import load_data
 from rasa_nlu.config import RasaNLUModelConfig
 from rasa_nlu.model import Trainer
 from rasa_nlu import config
 import warnings
+from plugin_manager import PluginManager
+from plugin_base import PluginBase
+import plugins  # assuming plugins will be stored in a "plugins" directory/package
+
 warnings.filterwarnings('ignore')
 
 training_data = load_data("nlu_data.md")
 trainer = Trainer(config.load("nlu_config.yml"))
 interpreter = trainer.train(training_data)
 
 # Save the trained model for future use
@@ -37,25 +41,30 @@
     # Use the Rasa NLU interpreter to parse the user input
     parsed_input = interpreter.parse(user_input)
 
     # Extract intent and entities from the parsed input
     intent = parsed_input["intent"]["name"]
     entities = {entity["entity"]: entity["value"] for entity in parsed_input["entities"]}
 
-    # Process the user input based on the identified intent and entities
-    if intent == "greet":
-        response = "Hello! How can I help you today?"
-    elif intent == "goodbye":
-        response = "Goodbye! Have a great day!"
-    elif intent == "ask_weather":
-        location = entities.get("location", "unknown")
-        response = f"I'm not currently able to check the weather, but you asked about {location}."
-    else:
-        prompt = f"Athena, please help me with the following: {user_input}"
-        response = generate_gpt3_response(prompt)
+    # Create a PluginManager instance, discover the plugins, and process the input using the plugins
+    plugin_manager = PluginManager(PluginBase, plugins)
+    plugin_manager.discover_plugins()
+
+    response = plugin_manager.process_input(user_input)
+    if response is None:
+        if intent == "greet":
+            response = "Hello! How can I help you today?"
+        elif intent == "goodbye":
+            response = "Goodbye! Have a great day!"
+        elif intent == "ask_weather":
+            location = entities.get("location", "unknown")
+            response = f"I'm not currently able to check the weather, but you asked about {location}."
+        else:
+            prompt = f"Athena, please help me with the following: {user_input}"
+            response = generate_gpt3_response(prompt)
 
     return response
 
 
 def main():
     print("Welcome to Athena, the AI Agent. Type 'exit' to end the conversation.")
```

### Comparing `athena_ai-0.0.3/.gitignore` & `athena_ai-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `athena_ai-0.0.3/LICENSE` & `athena_ai-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `athena_ai-0.0.3/README.md` & `athena_ai-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `athena_ai-0.0.3/pyproject.toml` & `athena_ai-0.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "athena-ai"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Bill Schumacher", email="34168009+BillSchumacher@users.noreply.github.com" },
   { name="Athena", email="34168009+BillSchumacher@users.noreply.github.com" },
 ]
 description = "Athena, an AI agent built on GPT-4 architecture, is designed for continuous learning and self-reliance. Inspired by the Greek goddess of wisdom, Athena assists users with valuable insights across various subjects. Focused on knowledge acquisition, capability improvement, and security, this AI agent leverages natural language processing and a supportive human community to grow and become a trusted, versatile companion."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `athena_ai-0.0.3/PKG-INFO` & `athena_ai-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athena-ai
-Version: 0.0.3
+Version: 0.0.4
 Summary: Athena, an AI agent built on GPT-4 architecture, is designed for continuous learning and self-reliance. Inspired by the Greek goddess of wisdom, Athena assists users with valuable insights across various subjects. Focused on knowledge acquisition, capability improvement, and security, this AI agent leverages natural language processing and a supportive human community to grow and become a trusted, versatile companion.
 Project-URL: Homepage, https://github.com/BillSchumacher/Athena
 Project-URL: Bug Tracker, https://github.com/BillSchumacher/Athena
 Author-email: Bill Schumacher <34168009+BillSchumacher@users.noreply.github.com>, Athena <34168009+BillSchumacher@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

