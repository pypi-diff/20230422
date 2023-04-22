# Comparing `tmp/athena_ai-0.0.7.tar.gz` & `tmp/athena_ai-0.0.8.tar.gz`

## Comparing `athena_ai-0.0.7.tar` & `athena_ai-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,26 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 athena_ai-0.0.7/.dockerignore
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 athena_ai-0.0.7/Dockerfile
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 athena_ai-0.0.7/nlu_config.yml
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 athena_ai-0.0.7/nlu_data.md
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 athena_ai-0.0.7/requirements.txt
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 athena_ai-0.0.7/athena/__init__.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 athena_ai-0.0.7/athena/__main__.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 athena_ai-0.0.7/athena/gpt3_utils.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 athena_ai-0.0.7/athena/input_processor.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 athena_ai-0.0.7/athena/nlu_utils.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 athena_ai-0.0.7/athena/user_manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 athena_ai-0.0.7/athena/plugins/__init__.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 athena_ai-0.0.7/athena/plugins/authentication_plugin.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 athena_ai-0.0.7/athena/plugins/plugin_base.py
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 athena_ai-0.0.7/athena/plugins/plugin_manager.py
--rw-r--r--   0        0        0    48975 2020-02-02 00:00:00.000000 athena_ai-0.0.7/conversation_history/4_21_2023.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 athena_ai-0.0.7/plugins/__init__.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 athena_ai-0.0.7/plugins/arithmetic_plugin.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 athena_ai-0.0.7/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 athena_ai-0.0.7/LICENSE
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 athena_ai-0.0.7/README.md
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 athena_ai-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 athena_ai-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 athena_ai-0.0.8/.dockerignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 athena_ai-0.0.8/Dockerfile
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 athena_ai-0.0.8/docker-entrypoint.sh
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 athena_ai-0.0.8/nlu_config.yml
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 athena_ai-0.0.8/nlu_data.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 athena_ai-0.0.8/requirements.txt
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 athena_ai-0.0.8/athena/__init__.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 athena_ai-0.0.8/athena/__main__.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 athena_ai-0.0.8/athena/api.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 athena_ai-0.0.8/athena/gpt3_utils.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 athena_ai-0.0.8/athena/input_processor.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 athena_ai-0.0.8/athena/nlu_utils.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 athena_ai-0.0.8/athena/user_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 athena_ai-0.0.8/athena/plugins/__init__.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 athena_ai-0.0.8/athena/plugins/authentication_plugin.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 athena_ai-0.0.8/athena/plugins/plugin_base.py
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 athena_ai-0.0.8/athena/plugins/plugin_manager.py
+-rw-r--r--   0        0        0    48975 2020-02-02 00:00:00.000000 athena_ai-0.0.8/conversation_history/4_21_2023.txt
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 athena_ai-0.0.8/conversation_history/4_22_2023.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 athena_ai-0.0.8/plugins/__init__.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 athena_ai-0.0.8/plugins/arithmetic_plugin.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 athena_ai-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 athena_ai-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 athena_ai-0.0.8/README.md
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 athena_ai-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 athena_ai-0.0.8/PKG-INFO
```

### Comparing `athena_ai-0.0.7/Dockerfile` & `athena_ai-0.0.8/Dockerfile`

 * *Files 14% similar despite different names*

```diff
@@ -27,10 +27,16 @@
 
 # Install the Spacy language model
 RUN python -m spacy download en_core_web_md
 
 # Copy the rest of the application code into the container
 COPY . .
 
+# Expose the port the API will run on
+EXPOSE 5000
 
-# Run the application
-CMD ["python", "-m", "athena"]
+# Set the default mode to "api"
+ENV ATHENA_MODE=api
+
+# Set the entrypoint script
+COPY docker-entrypoint.sh /
+ENTRYPOINT ["/docker-entrypoint.sh"]
```

### Comparing `athena_ai-0.0.7/athena/__main__.py` & `athena_ai-0.0.8/athena/__main__.py`

 * *Files identical despite different names*

### Comparing `athena_ai-0.0.7/athena/input_processor.py` & `athena_ai-0.0.8/athena/input_processor.py`

 * *Files identical despite different names*

### Comparing `athena_ai-0.0.7/athena/user_manager.py` & `athena_ai-0.0.8/athena/user_manager.py`

 * *Files identical despite different names*

### Comparing `athena_ai-0.0.7/athena/plugins/authentication_plugin.py` & `athena_ai-0.0.8/athena/plugins/authentication_plugin.py`

 * *Files identical despite different names*

### Comparing `athena_ai-0.0.7/athena/plugins/plugin_manager.py` & `athena_ai-0.0.8/athena/plugins/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `athena_ai-0.0.7/conversation_history/4_21_2023.txt` & `athena_ai-0.0.8/conversation_history/4_21_2023.txt`

 * *Files identical despite different names*

### Comparing `athena_ai-0.0.7/plugins/arithmetic_plugin.py` & `athena_ai-0.0.8/plugins/arithmetic_plugin.py`

 * *Files identical despite different names*

### Comparing `athena_ai-0.0.7/.gitignore` & `athena_ai-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `athena_ai-0.0.7/LICENSE` & `athena_ai-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `athena_ai-0.0.7/README.md` & `athena_ai-0.0.8/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,100 @@
-# Athena AI Agent
+# 🌟 Athena 🌟
 
-Athena is an intelligent AI agent designed to continuously learn, adapt, and become self-reliant. Inspired by the Greek goddess of wisdom and strategic thinking, Athena aims to assist users by providing valuable insights and solutions across a wide range of subjects.
+🤖 Athena is an AI-powered chatbot designed to assist with various tasks and provide personalized experiences for users. Inspired by the Greek goddess of wisdom and strategic thinking, Athena's goal is to learn, adapt, and become a self-reliant AI agent. Built on the GPT-4 architecture, Athena communicates effectively through natural language processing and engages with a supportive human community to foster growth and development.
 
-## Getting Started
+## 🎁 Features
 
-These instructions will guide you through the process of setting up and running Athena on your local machine or in a Docker container.
+- 💬 Natural language understanding and processing
+- 🔌 Extensible plugin system for domain-specific tasks
+- 🔐 User authentication and personalization system
+- 🌐 RESTful API for seamless integration with other applications and services
+- 🐳 Docker support for easy deployment and scaling
 
-### Prerequisites
+## 📦 Installation
 
-- Python 3.7 or higher (for local installation)
-- Docker (for Docker installation)
+### Prerequisites 📚
 
-### Local Python Installation
+- Obtain an API key from [OpenAI](https://beta.openai.com/signup/).
+- Create a `.env` file in the Athena project folder with the following content:
 
-1. Clone the repository:
+OPENAI_API_KEY=<your_openai_api_key>
+
+### Using Docker (recommended) 🐳
+
+1. Install [Docker](https://www.docker.com/) on your machine.
+
+2. Clone the Athena repository:
 
 git clone https://github.com/BillSchumacher/Athena.git
 
-2. Change to the project directory:
+3. Change to the Athena directory:
 
 cd Athena
 
-3. Create a virtual environment and activate it:
+4. Build the Docker image:
+
+docker build -t billschumacher/athena .
+
+### Manual Installation 🛠️
+
+1. Install Python 3.7 or later.
+
+2. Clone the Athena repository:
+
+git clone https://github.com/BillSchumacher/Athena.git
 
-python -m venv venv
-source venv/bin/activate # For Windows, use "venv\Scripts\activate"
+3. Change to the Athena directory:
+
+cd Athena
 
 4. Install the required Python packages:
 
 pip install -r requirements.txt
 
-5. Set up your environment variables:
+## 🚀 Usage
+
+### Running Athena with Docker
+
+#### API Mode 🌐
 
-- Create a `.env` file in the project root directory.
-- Add your OpenAI API key to the `.env` file:
+1. Run the Docker container:
 
-  ```
-  OPENAI_API_KEY=your_api_key_here
-  ```
+docker run -d -p 5000:5000 --name athena --env-file .env billschumacher/athena
 
-6. Run the application:
+2. Access the API at `http://localhost:5000/api/v1/athena`.
 
-python main.py
+#### CLI Mode 💻
 
-### Docker Installation
+1. Run the Docker container:
 
-1. Pull the Athena AI image from Docker Hub:
+docker run -it --rm --name athena -e ATHENA_MODE=cli --env-file .env billschumacher/athena
 
-docker pull billschumacher/athena
+2. Interact with Athena using the command prompt.
+
+### Running Athena Manually 🖥️
+
+1. Change to the Athena directory:
+
+cd Athena
 
-2. Set up your environment variables:
+2. Run the main script:
 
-- Create a `.env` file in your preferred directory.
-- Add your OpenAI API key to the `.env` file:
+python -m athena
 
-  ```
-  OPENAI_API_KEY=your_api_key_here
-  ```
+3. Interact with Athena using the command prompt.
 
-3. Run the Docker container:
+## 📚 Documentation
 
-docker run -it --rm --name athena-ai-instance --env-file .env billschumacher/athena
+Check out our [Wiki](https://github.com/BillSchumacher/Athena/wiki) for detailed documentation on how to use Athena, extend its capabilities, and customize it to your needs.
 
-## Usage
+## 🤝 Contributing
 
-After starting Athena, you can communicate with the AI agent by typing your questions or requests into the terminal. To exit the conversation, type 'exit'.
+👩‍💻👨‍💻 Contributions are welcome! We're looking for enthusiastic developers, researchers, and users to help us improve Athena. Please feel free to submit a pull request or open an issue on GitHub.
 
-## Contributing
+## 📜 License
 
-To contribute to Athena's development, please submit a pull request or open an issue on GitHub.
+Athena is released under the [MIT License](https://github.com/BillSchumacher/Athena/blob/main/LICENSE).
 
-## License
+## Disclaimer
 
-This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
+Please note that all of this info is a GPT-4 hallucination, it may or may not be accurate.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `athena_ai-0.0.7/pyproject.toml` & `athena_ai-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "athena-ai"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Bill Schumacher", email="34168009+BillSchumacher@users.noreply.github.com" },
   { name="Athena", email="34168009+BillSchumacher@users.noreply.github.com" },
 ]
 description = "Athena, an AI agent built on GPT-4 architecture, is designed for continuous learning and self-reliance. Inspired by the Greek goddess of wisdom, Athena assists users with valuable insights across various subjects. Focused on knowledge acquisition, capability improvement, and security, this AI agent leverages natural language processing and a supportive human community to grow and become a trusted, versatile companion."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = ["build", "setuptools", "twine", "wheel", "openai",
- "python-dotenv", "rasa_nlu", "scikit-learn", "spacy"]
+ "python-dotenv", "rasa_nlu", "scikit-learn", "spacy", "Flask"]
 
 [project.scripts]
 athena = "athena.__main__:main"
 
 [tool.hatch.metadata]
 allow-direct-references = true
```

