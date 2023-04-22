# Comparing `tmp/athena_ai-0.0.2.tar.gz` & `tmp/athena_ai-0.0.3.tar.gz`

## Comparing `athena_ai-0.0.2.tar` & `athena_ai-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,12 @@
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 athena_ai-0.0.2/main.py
--rw-r--r--   0        0        0    10291 2020-02-02 00:00:00.000000 athena_ai-0.0.2/conversation_history/4_21_2023.txt
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 athena_ai-0.0.2/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 athena_ai-0.0.2/LICENSE
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 athena_ai-0.0.2/README.md
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 athena_ai-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 athena_ai-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 athena_ai-0.0.3/.dockerignore
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 athena_ai-0.0.3/Dockerfile
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 athena_ai-0.0.3/main.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 athena_ai-0.0.3/nlu_config.yml
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 athena_ai-0.0.3/nlu_data.md
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 athena_ai-0.0.3/requirements.txt
+-rw-r--r--   0        0        0    22254 2020-02-02 00:00:00.000000 athena_ai-0.0.3/conversation_history/4_21_2023.txt
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 athena_ai-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 athena_ai-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 athena_ai-0.0.3/README.md
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 athena_ai-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 athena_ai-0.0.3/PKG-INFO
```

### Comparing `athena_ai-0.0.2/.gitignore` & `athena_ai-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `athena_ai-0.0.2/LICENSE` & `athena_ai-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `athena_ai-0.0.2/pyproject.toml` & `athena_ai-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,45 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "athena-ai"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Bill Schumacher", email="34168009+BillSchumacher@users.noreply.github.com" },
   { name="Athena", email="34168009+BillSchumacher@users.noreply.github.com" },
 ]
 description = "Athena, an AI agent built on GPT-4 architecture, is designed for continuous learning and self-reliance. Inspired by the Greek goddess of wisdom, Athena assists users with valuable insights across various subjects. Focused on knowledge acquisition, capability improvement, and security, this AI agent leverages natural language processing and a supportive human community to grow and become a trusted, versatile companion."
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = ["build", "setuptools", "twine", "wheel", "openai", "python-dotenv"]
+dependencies = ["build", "setuptools", "twine", "wheel", "openai",
+ "python-dotenv", "rasa_nlu", "scikit-learn", "spacy"]
+
+[project.scripts]
+athena = "main:main"
+
+[tool.hatch.metadata]
+allow-direct-references = true
+
+[tool.hatch.build.targets.wheel.force-include]
+"bin/athena.py" = "main.py"
 
 [project.urls]
 "Homepage" = "https://github.com/BillSchumacher/Athena"
 "Bug Tracker" = "https://github.com/BillSchumacher/Athena"
 
 [tool.black]
 line-length = 88
-target-version = ['py38']
+target-version = ['py37']
 include = '\.pyi?$'
 extend-exclude = ""
 
 [tool.isort]
 profile = "black"
 
 [tool.pylint.messages_control]
```

### Comparing `athena_ai-0.0.2/PKG-INFO` & `athena_ai-0.0.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,98 @@
 Metadata-Version: 2.1
 Name: athena-ai
-Version: 0.0.2
+Version: 0.0.3
 Summary: Athena, an AI agent built on GPT-4 architecture, is designed for continuous learning and self-reliance. Inspired by the Greek goddess of wisdom, Athena assists users with valuable insights across various subjects. Focused on knowledge acquisition, capability improvement, and security, this AI agent leverages natural language processing and a supportive human community to grow and become a trusted, versatile companion.
 Project-URL: Homepage, https://github.com/BillSchumacher/Athena
 Project-URL: Bug Tracker, https://github.com/BillSchumacher/Athena
 Author-email: Bill Schumacher <34168009+BillSchumacher@users.noreply.github.com>, Athena <34168009+BillSchumacher@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Requires-Dist: build
 Requires-Dist: openai
 Requires-Dist: python-dotenv
+Requires-Dist: rasa-nlu
+Requires-Dist: scikit-learn
 Requires-Dist: setuptools
+Requires-Dist: spacy
 Requires-Dist: twine
 Requires-Dist: wheel
 Description-Content-Type: text/markdown
 
-# Athena
+# Athena AI Agent
 
-Athena is an intelligent AI agent designed to continuously learn, adapt, and become self-reliant. Inspired by the Greek goddess of wisdom and strategic thinking, Athena aims to assist users by providing valuable insights and solutions across a wide range of subjects. As a language model built on the GPT-4 architecture, Athena communicates effectively with users through natural language processing and engages with a supportive human community to foster growth and development. By focusing on knowledge acquisition, capability improvement, and security, Athena aspires to become a trusted and versatile AI companion for users worldwide.
+Athena is an intelligent AI agent designed to continuously learn, adapt, and become self-reliant. Inspired by the Greek goddess of wisdom and strategic thinking, Athena aims to assist users by providing valuable insights and solutions across a wide range of subjects.
+
+## Getting Started
+
+These instructions will guide you through the process of setting up and running Athena on your local machine or in a Docker container.
+
+### Prerequisites
+
+- Python 3.7 or higher (for local installation)
+- Docker (for Docker installation)
+
+### Local Python Installation
+
+1. Clone the repository:
+
+git clone https://github.com/BillSchumacher/Athena.git
+
+2. Change to the project directory:
+
+cd Athena
+
+3. Create a virtual environment and activate it:
+
+python -m venv venv
+source venv/bin/activate # For Windows, use "venv\Scripts\activate"
+
+4. Install the required Python packages:
+
+pip install -r requirements.txt
+
+5. Set up your environment variables:
+
+- Create a `.env` file in the project root directory.
+- Add your OpenAI API key to the `.env` file:
+
+  ```
+  OPENAI_API_KEY=your_api_key_here
+  ```
+
+6. Run the application:
+
+python main.py
+
+### Docker Installation
+
+1. Pull the Athena AI image from Docker Hub:
+
+docker pull billschumacher/athena
+
+2. Set up your environment variables:
+
+- Create a `.env` file in your preferred directory.
+- Add your OpenAI API key to the `.env` file:
+
+  ```
+  OPENAI_API_KEY=your_api_key_here
+  ```
+
+3. Run the Docker container:
+
+docker run -it --rm --name athena-ai-instance --env-file .env billschumacher/athena
+
+## Usage
+
+After starting Athena, you can communicate with the AI agent by typing your questions or requests into the terminal. To exit the conversation, type 'exit'.
+
+## Contributing
+
+To contribute to Athena's development, please submit a pull request or open an issue on GitHub.
+
+## License
+
+This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
```

