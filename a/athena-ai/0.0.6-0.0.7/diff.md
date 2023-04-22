# Comparing `tmp/athena_ai-0.0.6.tar.gz` & `tmp/athena_ai-0.0.7.tar.gz`

## Comparing `athena_ai-0.0.6.tar` & `athena_ai-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,23 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 athena_ai-0.0.6/.dockerignore
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 athena_ai-0.0.6/Dockerfile
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 athena_ai-0.0.6/nlu_config.yml
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 athena_ai-0.0.6/nlu_data.md
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 athena_ai-0.0.6/requirements.txt
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 athena_ai-0.0.6/athena/__init__.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 athena_ai-0.0.6/athena/__main__.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 athena_ai-0.0.6/athena/user_manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 athena_ai-0.0.6/athena/plugins/__init__.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 athena_ai-0.0.6/athena/plugins/authentication_plugin.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 athena_ai-0.0.6/athena/plugins/plugin_base.py
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 athena_ai-0.0.6/athena/plugins/plugin_manager.py
--rw-r--r--   0        0        0    42457 2020-02-02 00:00:00.000000 athena_ai-0.0.6/conversation_history/4_21_2023.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 athena_ai-0.0.6/plugins/__init__.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 athena_ai-0.0.6/plugins/arithmetic_plugin.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 athena_ai-0.0.6/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 athena_ai-0.0.6/LICENSE
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 athena_ai-0.0.6/README.md
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 athena_ai-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 athena_ai-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 athena_ai-0.0.7/.dockerignore
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 athena_ai-0.0.7/Dockerfile
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 athena_ai-0.0.7/nlu_config.yml
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 athena_ai-0.0.7/nlu_data.md
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 athena_ai-0.0.7/requirements.txt
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 athena_ai-0.0.7/athena/__init__.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 athena_ai-0.0.7/athena/__main__.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 athena_ai-0.0.7/athena/gpt3_utils.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 athena_ai-0.0.7/athena/input_processor.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 athena_ai-0.0.7/athena/nlu_utils.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 athena_ai-0.0.7/athena/user_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 athena_ai-0.0.7/athena/plugins/__init__.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 athena_ai-0.0.7/athena/plugins/authentication_plugin.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 athena_ai-0.0.7/athena/plugins/plugin_base.py
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 athena_ai-0.0.7/athena/plugins/plugin_manager.py
+-rw-r--r--   0        0        0    48975 2020-02-02 00:00:00.000000 athena_ai-0.0.7/conversation_history/4_21_2023.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 athena_ai-0.0.7/plugins/__init__.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 athena_ai-0.0.7/plugins/arithmetic_plugin.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 athena_ai-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 athena_ai-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 athena_ai-0.0.7/README.md
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 athena_ai-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 athena_ai-0.0.7/PKG-INFO
```

### Comparing `athena_ai-0.0.6/Dockerfile` & `athena_ai-0.0.7/Dockerfile`

 * *Files identical despite different names*

### Comparing `athena_ai-0.0.6/athena/user_manager.py` & `athena_ai-0.0.7/athena/user_manager.py`

 * *Files identical despite different names*

### Comparing `athena_ai-0.0.6/athena/plugins/authentication_plugin.py` & `athena_ai-0.0.7/athena/plugins/authentication_plugin.py`

 * *Files identical despite different names*

### Comparing `athena_ai-0.0.6/athena/plugins/plugin_manager.py` & `athena_ai-0.0.7/athena/plugins/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `athena_ai-0.0.6/conversation_history/4_21_2023.txt` & `athena_ai-0.0.7/conversation_history/4_21_2023.txt`

 * *Files 4% similar despite different names*

```diff
@@ -956,7 +956,176 @@
         pass
     print("Athena: Goodbye!")
 
 if __name__ == "__main__":
     main()
 
 This is a great improvement to the code, making it more user-friendly and providing a better experience for users when they decide to exit the application.
+
+Me> I think there's too much code in the __init__.py file, what do you think? This is the current contents: import os
+from dotenv import load_dotenv
+import openai
+from rasa_nlu.training_data import load_data
+from rasa_nlu.config import RasaNLUModelConfig
+from rasa_nlu.model import Trainer
+from rasa_nlu import config
+import warnings
+from athena.plugins.plugin_manager import PluginManager
+from athena.plugins.plugin_base import PluginBase
+import plugins  # assuming plugins will be stored in a "plugins" directory/package
+from athena.user_manager import UserManager
+from athena.plugins.authentication_plugin import AuthenticationPlugin
+
+warnings.filterwarnings('ignore')
+
+training_data = load_data("nlu_data.md")
+trainer = Trainer(config.load("nlu_config.yml"))
+interpreter = trainer.train(training_data)
+
+# Save the trained model for future use
+model_directory = trainer.persist("./models/nlu", fixed_model_name="current")
+
+load_dotenv()
+
+# Load the API key from the environment variable
+openai.api_key = os.environ["OPENAI_API_KEY"]
+
+
+def generate_gpt3_response(prompt):
+    response = openai.Completion.create(
+        engine="davinci", # Choose the desired model, e.g., "davinci", "curie", "babbage", "davinci-codex", etc.
+        prompt=prompt,
+        max_tokens=100,
+        n=1,
+        stop=None,
+        temperature=0.8,
+    )
+    return response.choices[0].text.strip()
+
+
+user_manager = UserManager()
+auth_plugin = AuthenticationPlugin(user_manager)
+
+
+def process_input(user_input, username=None):
+    # Use the Rasa NLU interpreter to parse the user input
+    parsed_input = interpreter.parse(user_input)
+
+    # Extract intent and entities from the parsed input
+    intent = parsed_input["intent"]["name"]
+    entities = {entity["entity"]: entity["value"] for entity in parsed_input["entities"]}
+
+    # Create a PluginManager instance, discover the plugins, and process the input using the plugins
+    plugin_manager = PluginManager(PluginBase, plugins, extra_plugins=[auth_plugin])
+    plugin_manager.discover_plugins()
+
+    if username is not None:
+        personalization_data = user_manager.get_user_preference(username, "personalization_data")
+        if personalization_data is not None:
+            # Apply personalization logic using personalization_data
+            pass
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
+
+    return response
+
+Athena> You're right. The __init__.py file contains a lot of code and can be further organized by separating concerns into different files.
+
+Here's a suggestion for reorganizing the code:
+
+Create a new file named gpt3_utils.py inside the athena directory and move the generate_gpt3_response function to that file.
+
+Move the Rasa NLU related code (training and interpreter setup) to a new file named nlu_utils.py inside the athena directory.
+
+In the __init__.py file, keep only the import statements, global variables, and the process_input function.
+
+After reorganizing, your __init__.py file should look like this:
+
+import os
+from dotenv import load_dotenv
+from athena.plugins.plugin_manager import PluginManager
+from athena.plugins.plugin_base import PluginBase
+import plugins  # assuming plugins will be stored in a "plugins" directory/package
+from athena.user_manager import UserManager
+from athena.plugins.authentication_plugin import AuthenticationPlugin
+from .gpt3_utils import generate_gpt3_response
+from .nlu_utils import interpreter
+
+load_dotenv()
+
+# Load the API key from the environment variable
+openai.api_key = os.environ["OPENAI_API_KEY"]
+
+user_manager = UserManager()
+auth_plugin = AuthenticationPlugin(user_manager)
+
+def process_input(user_input, username=None):
+
+In gpt3_utils.py:
+
+import openai
+
+def generate_gpt3_response(prompt):
+
+In nlu_utils.py:
+
+from rasa_nlu.training_data import load_data
+from rasa_nlu.config import RasaNLUModelConfig
+from rasa_nlu.model import Trainer
+from rasa_nlu import config
+import warnings
+
+warnings.filterwarnings('ignore')
+
+training_data = load_data("nlu_data.md")
+trainer = Trainer(config.load("nlu_config.yml"))
+interpreter = trainer.train(training_data)
+
+# Save the trained model for future use
+model_directory = trainer.persist("./models/nlu", fixed_model_name="current")
+
+After these changes, your code is cleaner and more organized, making it easier to add new features and maintain the codebase.
+
+Me> Shouldn't we move the process_input to a new file as well?
+
+Athena> Yes, it's a good idea to move the process_input function to a separate file to keep the __init__.py file cleaner and more focused on importing the necessary components. You can create a new file called input_processor.py inside the athena directory and move the process_input function there.
+
+After doing so, your __init__.py file should look like this:
+
+import os
+from dotenv import load_dotenv
+from athena.user_manager import UserManager
+from athena.plugins.authentication_plugin import AuthenticationPlugin
+from .input_processor import process_input
+
+load_dotenv()
+
+# Load the API key from the environment variable
+openai.api_key = os.environ["OPENAI_API_KEY"]
+
+user_manager = UserManager()
+auth_plugin = AuthenticationPlugin(user_manager)
+
+And the new input_processor.py file should contain:
+
+from athena.plugins.plugin_manager import PluginManager
+from athena.plugins.plugin_base import PluginBase
+import plugins  # assuming plugins will be stored in a "plugins" directory/package
+from .gpt3_utils import generate_gpt3_response
+from .nlu_utils import interpreter
+
+def process_input(user_input, username=None):
+    # (The code remains the same as before)
+
+Now, the __init__.py file is focused on initializing the necessary components, and the process_input function is located in a separate file, making the codebase more organized and easier to maintain.
+
+Me> (I helped out a little bit here...)
```

### Comparing `athena_ai-0.0.6/plugins/arithmetic_plugin.py` & `athena_ai-0.0.7/plugins/arithmetic_plugin.py`

 * *Files identical despite different names*

### Comparing `athena_ai-0.0.6/.gitignore` & `athena_ai-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `athena_ai-0.0.6/LICENSE` & `athena_ai-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `athena_ai-0.0.6/README.md` & `athena_ai-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `athena_ai-0.0.6/pyproject.toml` & `athena_ai-0.0.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "athena-ai"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Bill Schumacher", email="34168009+BillSchumacher@users.noreply.github.com" },
   { name="Athena", email="34168009+BillSchumacher@users.noreply.github.com" },
 ]
 description = "Athena, an AI agent built on GPT-4 architecture, is designed for continuous learning and self-reliance. Inspired by the Greek goddess of wisdom, Athena assists users with valuable insights across various subjects. Focused on knowledge acquisition, capability improvement, and security, this AI agent leverages natural language processing and a supportive human community to grow and become a trusted, versatile companion."
 readme = "README.md"
 requires-python = ">=3.7"
@@ -17,21 +17,21 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = ["build", "setuptools", "twine", "wheel", "openai",
  "python-dotenv", "rasa_nlu", "scikit-learn", "spacy"]
 
 [project.scripts]
-athena = "__init__:main"
+athena = "athena.__main__:main"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.wheel.force-include]
-"bin/athena.py" = "athena/__init__.py"
+"bin/athena.py" = "athena/__main__.py"
 
 [project.urls]
 "Homepage" = "https://github.com/BillSchumacher/Athena"
 "Bug Tracker" = "https://github.com/BillSchumacher/Athena"
 
 [tool.black]
 line-length = 88
```

### Comparing `athena_ai-0.0.6/PKG-INFO` & `athena_ai-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athena-ai
-Version: 0.0.6
+Version: 0.0.7
 Summary: Athena, an AI agent built on GPT-4 architecture, is designed for continuous learning and self-reliance. Inspired by the Greek goddess of wisdom, Athena assists users with valuable insights across various subjects. Focused on knowledge acquisition, capability improvement, and security, this AI agent leverages natural language processing and a supportive human community to grow and become a trusted, versatile companion.
 Project-URL: Homepage, https://github.com/BillSchumacher/Athena
 Project-URL: Bug Tracker, https://github.com/BillSchumacher/Athena
 Author-email: Bill Schumacher <34168009+BillSchumacher@users.noreply.github.com>, Athena <34168009+BillSchumacher@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

