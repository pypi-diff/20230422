# Comparing `tmp/paper2cmap-0.1.0.tar.gz` & `tmp/paper2cmap-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper2cmap-0.1.0.tar", last modified: Sat Apr 22 08:36:35 2023, max compression
+gzip compressed data, was "paper2cmap-0.1.1.tar", last modified: Sat Apr 22 08:40:39 2023, max compression
```

## Comparing `paper2cmap-0.1.0.tar` & `paper2cmap-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-22 08:36:35.504098 paper2cmap-0.1.0/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1065 2023-04-21 13:31:25.000000 paper2cmap-0.1.0/LICENSE
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       41 2023-04-22 02:05:11.000000 paper2cmap-0.1.0/MANIFEST.in
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     5405 2023-04-22 08:36:35.504098 paper2cmap-0.1.0/PKG-INFO
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     3626 2023-04-22 08:36:04.000000 paper2cmap-0.1.0/README.md
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-22 08:36:35.500098 paper2cmap-0.1.0/paper2cmap/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      179 2023-04-21 12:31:25.000000 paper2cmap-0.1.0/paper2cmap/__init__.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     4278 2023-04-22 08:36:04.000000 paper2cmap-0.1.0/paper2cmap/cmapgpt.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     2368 2023-04-21 16:55:29.000000 paper2cmap-0.1.0/paper2cmap/llm.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      409 2023-04-21 11:49:55.000000 paper2cmap-0.1.0/paper2cmap/logger.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-22 08:36:35.500098 paper2cmap-0.1.0/paper2cmap/metas/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1176 2023-04-22 08:36:04.000000 paper2cmap-0.1.0/paper2cmap/metas/examples.json
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1741 2023-04-22 08:36:04.000000 paper2cmap-0.1.0/paper2cmap/metas/prompts.yaml
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     3597 2023-04-22 08:36:04.000000 paper2cmap-0.1.0/paper2cmap/paper2cmap.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     3652 2023-04-22 08:36:04.000000 paper2cmap-0.1.0/paper2cmap/paper_reader.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-22 08:36:35.500098 paper2cmap-0.1.0/paper2cmap.egg-info/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     5405 2023-04-22 08:36:35.000000 paper2cmap-0.1.0/paper2cmap.egg-info/PKG-INFO
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      484 2023-04-22 08:36:35.000000 paper2cmap-0.1.0/paper2cmap.egg-info/SOURCES.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)        1 2023-04-22 08:36:35.000000 paper2cmap-0.1.0/paper2cmap.egg-info/dependency_links.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       53 2023-04-22 08:36:35.000000 paper2cmap-0.1.0/paper2cmap.egg-info/requires.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       11 2023-04-22 08:36:35.000000 paper2cmap-0.1.0/paper2cmap.egg-info/top_level.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      816 2023-04-22 02:11:56.000000 paper2cmap-0.1.0/pyproject.toml
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       38 2023-04-22 08:36:35.504098 paper2cmap-0.1.0/setup.cfg
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-22 08:36:35.504098 paper2cmap-0.1.0/tests/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1828 2023-04-22 08:36:04.000000 paper2cmap-0.1.0/tests/test_cmapgpt.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      420 2023-04-22 08:36:04.000000 paper2cmap-0.1.0/tests/test_paper2cmap.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      456 2023-04-22 08:36:04.000000 paper2cmap-0.1.0/tests/test_paper_reader.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-22 08:40:39.475427 paper2cmap-0.1.1/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1065 2023-04-21 13:31:25.000000 paper2cmap-0.1.1/LICENSE
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)       41 2023-04-22 02:05:11.000000 paper2cmap-0.1.1/MANIFEST.in
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     5465 2023-04-22 08:40:39.475427 paper2cmap-0.1.1/PKG-INFO
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     3686 2023-04-22 08:39:00.000000 paper2cmap-0.1.1/README.md
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-22 08:40:39.467427 paper2cmap-0.1.1/paper2cmap/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      179 2023-04-22 08:39:53.000000 paper2cmap-0.1.1/paper2cmap/__init__.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     5243 2023-04-22 08:39:00.000000 paper2cmap-0.1.1/paper2cmap/cmapgpt.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     2368 2023-04-21 16:55:29.000000 paper2cmap-0.1.1/paper2cmap/llm.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      409 2023-04-21 11:49:55.000000 paper2cmap-0.1.1/paper2cmap/logger.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-22 08:40:39.471427 paper2cmap-0.1.1/paper2cmap/metas/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1157 2023-04-22 08:39:00.000000 paper2cmap-0.1.1/paper2cmap/metas/generate_examples.json
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)        8 2023-04-22 08:39:00.000000 paper2cmap-0.1.1/paper2cmap/metas/merge_and_prune_examples.json
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     2798 2023-04-22 08:39:00.000000 paper2cmap-0.1.1/paper2cmap/metas/prompts.yaml
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     5449 2023-04-22 08:39:00.000000 paper2cmap-0.1.1/paper2cmap/paper2cmap.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     3700 2023-04-22 08:39:00.000000 paper2cmap-0.1.1/paper2cmap/paper_reader.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-22 08:40:39.471427 paper2cmap-0.1.1/paper2cmap.egg-info/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     5465 2023-04-22 08:40:39.000000 paper2cmap-0.1.1/paper2cmap.egg-info/PKG-INFO
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      540 2023-04-22 08:40:39.000000 paper2cmap-0.1.1/paper2cmap.egg-info/SOURCES.txt
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)        1 2023-04-22 08:40:39.000000 paper2cmap-0.1.1/paper2cmap.egg-info/dependency_links.txt
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)       53 2023-04-22 08:40:39.000000 paper2cmap-0.1.1/paper2cmap.egg-info/requires.txt
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)       11 2023-04-22 08:40:39.000000 paper2cmap-0.1.1/paper2cmap.egg-info/top_level.txt
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      816 2023-04-22 08:39:43.000000 paper2cmap-0.1.1/pyproject.toml
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)       38 2023-04-22 08:40:39.475427 paper2cmap-0.1.1/setup.cfg
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-22 08:40:39.475427 paper2cmap-0.1.1/tests/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1979 2023-04-22 08:39:00.000000 paper2cmap-0.1.1/tests/test_cmapgpt.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      400 2023-04-22 08:39:00.000000 paper2cmap-0.1.1/tests/test_paper2cmap.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      474 2023-04-22 08:39:00.000000 paper2cmap-0.1.1/tests/test_paper_reader.py
```

### Comparing `paper2cmap-0.1.0/LICENSE` & `paper2cmap-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paper2cmap-0.1.0/PKG-INFO` & `paper2cmap-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper2cmap
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package that automatically generates a concept map for a PDF document using LLM.
 Author-email: weitian <weitian.bnu@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tian Wei
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -53,15 +53,17 @@
 > 
 > Concept maps typically consist of nodes or boxes, which represent concepts or ideas, and lines or arrows, which show the relationships between the concepts. The nodes can be labeled with keywords or short phrases, and the lines or arrows can be labeled with connecting words, such as "leads to," "is a type of," or "causes."
 > 
 > Concept maps can be created by individuals or groups, and can be used to facilitate learning, problem-solving, decision-making, and communication. They are a flexible and powerful tool that can be adapted to many different contexts and purposes.
 
 ### What is Paper2CMap?
 
-Paper2CMap is a package that automatically generates a concept map for a PDF document using LLM. It will first extract the text from the PDF document, then cut the text into sections, and finally generate concept map based on the sections. Currently the generated concept map is in JSON format:
+Paper2CMap is a package that automatically generates a concept map for a PDF document using LLM. It will first cut the text of the PDF document into sections, then generate concept maps for each section, and finally merge and prune these concept maps to generate a final map for the whole document.
+
+Currently the generated concept map is in JSON format:
 ```JSON
 [{"source": "source concept", "target": "target concept", "relationship": "relationship between source and target"}]
 ```
 In future, we will support more formats export, such as LNKG/CXL/SVG.
 
 ## Quick Start
```

### Comparing `paper2cmap-0.1.0/README.md` & `paper2cmap-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 > 
 > Concept maps typically consist of nodes or boxes, which represent concepts or ideas, and lines or arrows, which show the relationships between the concepts. The nodes can be labeled with keywords or short phrases, and the lines or arrows can be labeled with connecting words, such as "leads to," "is a type of," or "causes."
 > 
 > Concept maps can be created by individuals or groups, and can be used to facilitate learning, problem-solving, decision-making, and communication. They are a flexible and powerful tool that can be adapted to many different contexts and purposes.
 
 ### What is Paper2CMap?
 
-Paper2CMap is a package that automatically generates a concept map for a PDF document using LLM. It will first extract the text from the PDF document, then cut the text into sections, and finally generate concept map based on the sections. Currently the generated concept map is in JSON format:
+Paper2CMap is a package that automatically generates a concept map for a PDF document using LLM. It will first cut the text of the PDF document into sections, then generate concept maps for each section, and finally merge and prune these concept maps to generate a final map for the whole document.
+
+Currently the generated concept map is in JSON format:
 ```JSON
 [{"source": "source concept", "target": "target concept", "relationship": "relationship between source and target"}]
 ```
 In future, we will support more formats export, such as LNKG/CXL/SVG.
 
 ## Quick Start
```

### Comparing `paper2cmap-0.1.0/paper2cmap/cmapgpt.py` & `paper2cmap-0.1.1/paper2cmap/cmapgpt.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,100 +10,116 @@
 from langchain import PromptTemplate
 from langchain.prompts.chat import (
     ChatPromptTemplate,
     SystemMessagePromptTemplate,
     AIMessagePromptTemplate,
     HumanMessagePromptTemplate,
 )
-from langchain.schema import BaseMessage
 
 from paper2cmap import logger
 
 
 class CMapGPT():
     def __init__(self, chatbot: ChatOpenAI | AzureChatOpenAI) -> None:
-        self.prompt_config = yaml.load(
+        self._prompt_config = yaml.load(
             open(pkg_resources.resource_filename('paper2cmap', 'metas/prompts.yaml'), "r"),
             Loader=yaml.FullLoader
             )
-        self.system_prompt = self.prompt_config["system_prompt"]
-        self.user_prompt = self.prompt_config["user_prompt"]
+        self._generate_system_prompt = self._prompt_config["generate"]["system"]
+        self._generate_user_prompt = self._prompt_config["generate"]["user"]
+        self._merge_and_prune_system_prompt = self._prompt_config["merge_and_prune"]["system"]
+        self._merge_and_prune_user_prompt = self._prompt_config["merge_and_prune"]["user"]
 
-        self.examples = json.load(
-            open(pkg_resources.resource_filename('paper2cmap', 'metas/examples.json'), "r")
+        self._generate_examples = json.load(
+            open(pkg_resources.resource_filename('paper2cmap', 'metas/generate_examples.json'), "r")
+            )
+        self._merge_and_prune_examples = json.load(
+            open(pkg_resources.resource_filename('paper2cmap', 'metas/merge_and_prune_examples.json'), "r")
             )
 
-        self.cmap_prompt = self.create_cmap_prompt()
+        self.generate_prompt = self._create_prompt(
+            system_prompt=self._generate_system_prompt,
+            user_prompt=self._generate_user_prompt,
+            user_prompt_vars=["text", "max_num_concepts", "max_num_relationships"],
+            examples=self._generate_examples
+        )
+        self.merge_and_prune_prompt = self._create_prompt(
+            system_prompt=self._merge_and_prune_system_prompt,
+            user_prompt=self._merge_and_prune_user_prompt,
+            user_prompt_vars=["cmap", "max_num_concepts", "max_num_relationships"],
+            examples=self._merge_and_prune_examples
+        )
         
         self.chatbot = chatbot
 
-    def create_cmap_prompt(self) -> ChatPromptTemplate:
-        """
-        Create the concept map prompt.
-
-        :return: The concept map prompt.
-        """
+    def _create_prompt(self, 
+                       system_prompt: str = "", system_prompt_vars: List[str] = [],
+                       user_prompt: str = "", user_prompt_vars: List[str] = [], 
+                       examples: List[Dict] = []) -> ChatPromptTemplate:
         system_message_prompt = SystemMessagePromptTemplate(
             prompt=PromptTemplate(
-                template=self.system_prompt,
-                input_variables=[],
+                template=system_prompt,
+                input_variables=system_prompt_vars,
                 template_format="jinja2"
             )
         )
 
         human_message_prompt = HumanMessagePromptTemplate(
             prompt=PromptTemplate(
-                template=self.user_prompt,
-                input_variables=["text_input", "cmap_input", "max_num_concepts", "max_num_relationships"],
+                template=user_prompt,
+                input_variables=user_prompt_vars,
                 template_format="jinja2"
             )
         )
 
         examples_message_prompts = []
-        for example in self.examples:
+        for example in examples:
             role_message_prompt_template = AIMessagePromptTemplate if example["role"] == "assistant" else HumanMessagePromptTemplate
             examples_message_prompts.append(
                 role_message_prompt_template(
                     prompt=PromptTemplate(
                         template=example["content"],
                         input_variables=[],
                         template_format="jinja2"
                     )
                 )
             )
 
         return ChatPromptTemplate.from_messages([system_message_prompt, *examples_message_prompts, human_message_prompt])
 
-    def format_cmap_prompt(self, text_input: str, cmap_input: List[Dict], 
-                           max_num_concepts: int = 10, max_num_relationships: int = 30) -> List[BaseMessage]:
+    def generate(self, text: str, max_num_concepts: int = 10, max_num_relationships: int = 30) -> List[Dict]:
         """
-        Format the concept map prompt.
+        Generate a concept map from the given text.
 
-        :param text_input: str, the text input to the model.
-        :param cmap_input: List[Dict], a json that represents the concept map input to the model.
+        :param text: str, the text input to the model.
         :param max_num_concepts: int, the maximum number of concepts to generate.
         :param max_num_relationships: int, the maximum number of relationships to generate.
-        :return: List[BaseMessage], the formatted concept map prompt.
+        :return: List[Dict], the generated concept map.
         """
-        return self.cmap_prompt.format_prompt(
-            text_input=text_input,
-            cmap_input=cmap_input,
+        inputs = self.generate_prompt.format_prompt(
+            text=text,
             max_num_concepts=max_num_concepts,
             max_num_relationships=max_num_relationships
-        ).to_messages()
+        )
+        logger.debug(f"[CMapGPT] Prompt: {inputs.to_string()}")
+        response = self.chatbot(inputs.to_messages()).content
+        logger.debug(f"[CMapGPT] Result: {response}")
+        return json.loads(response)
 
-    def chat(self, text_input: str, cmap_input: List[Dict] = [],
-             max_num_concepts: int = 10, max_num_relationships: int = 30) -> List[Dict]:
+    def merge_and_prune(self, cmap: List[Dict], max_num_concepts: int = 10, max_num_relationships: int = 30) -> List[Dict]:
         """
-        Chat with the model to generate a concept map.
+        Merge and prune the given concept map.
 
-        :param text_input: str, the text input to the model.
-        :param cmap_input: List[Dict], a json that represents the concept map input to the model.
+        :param cmap: List[Dict], the concept map to merge and prune.
         :param max_num_concepts: int, the maximum number of concepts to generate.
         :param max_num_relationships: int, the maximum number of relationships to generate.
-        :return: List[Dict], the generated concept map output.
+        :return: List[Dict], the merged and pruned concept map.
         """
-        inputs = self.format_cmap_prompt(text_input, cmap_input, max_num_concepts, max_num_relationships)
-        logger.debug(f"[CMapGPT] Prompt: {inputs}")
-        response = self.chatbot(inputs).content
+        inputs = self.merge_and_prune_prompt.format_prompt(
+            cmap=cmap,
+            max_num_concepts=max_num_concepts,
+            max_num_relationships=max_num_relationships
+        )
+        logger.debug(f"[CMapGPT] Prompt: {inputs.to_string()}")
+        response = self.chatbot(inputs.to_messages()).content
         logger.debug(f"[CMapGPT] Result: {response}")
         return json.loads(response)
```

### Comparing `paper2cmap-0.1.0/paper2cmap/llm.py` & `paper2cmap-0.1.1/paper2cmap/llm.py`

 * *Files identical despite different names*

### Comparing `paper2cmap-0.1.0/paper2cmap/metas/examples.json` & `paper2cmap-0.1.1/paper2cmap/metas/generate_examples.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {'0': "{'content': 'Text input: { Journal classification systems play an important role in "*

 * *      'bibliometric analyses. The two most important bibliographic databases, Web of Science and '*

 * *      'Scopus, each provide a journal classification system. However, no study has systematically '*

 * *      'investigated the accuracy of these classification systems. To examine and compare the '*

 * *      'accuracy of journal classification systems, we define two criteria on the basis of direct '*

 * *      "citation relations  […]*

```diff
@@ -1,10 +1,10 @@
 [
     {
-        "content": "Text input: { Journal classification systems play an important role in bibliometric analyses. The two most important bibliographic databases, Web of Science and Scopus, each provide a journal classification system. However, no study has systematically investigated the accuracy of these classification systems. To examine and compare the accuracy of journal classification systems, we define two criteria on the basis of direct citation relations between journals and categories. } Existing CMap: { }",
+        "content": "Text input: { Journal classification systems play an important role in bibliometric analyses. The two most important bibliographic databases, Web of Science and Scopus, each provide a journal classification system. However, no study has systematically investigated the accuracy of these classification systems. To examine and compare the accuracy of journal classification systems, we define two criteria on the basis of direct citation relations between journals and categories. }",
         "role": "user"
     },
     {
         "content": "[{\"source\": \"journal classification system\", \"target\": \"bibliometric analyses\", \"relationship\": \"play an important role in\"}, {\"source\": \"Web of Science\", \"target\": \"journal classification system\", \"relationship\": \"provide\"}, {\"source\": \"Scopus\", \"target\": \"journal classification system\", \"relationship\": \"provide\"}, {\"source\": \"criteria\", \"target\": \"accuracy\", \"relationship\": \"examine and compare\"}, {\"source\": \"accuracy\", \"target\": \"journal classification system\", \"relationship\": \"of\"}]",
         "role": "assistant"
     }
 ]
```

### Comparing `paper2cmap-0.1.0/paper2cmap/paper_reader.py` & `paper2cmap-0.1.1/paper2cmap/paper_reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,42 +17,42 @@
 from paper2cmap import logger
 
 
 class PaperReader():
     def __init__(self, chatbot: ChatOpenAI | AzureChatOpenAI) -> None:
         self.chatbot = chatbot
 
-        self.title_max_len = 50
-        self.title_min_len = 5
+        self._title_max_len = 50
+        self._title_min_len = 5
 
         # Acknowledge to https://github.com/talkingwallace/ChatGPT-Paper-Reader for sharing the prompt
-        self.system_prompt_for_catelogue = """
+        self._catelogue_system_prompt = """
 You are a researcher helper bot. Now I will give several texts and you help me to find out which of them are the section titles of a research paper.
 You must return me in this json format:
 {
     "titles": ["section title text", "section title text", ...]
 }
 If the title has a number, the number MUST be retained!!!!
         """
 
     def _extract_candidate_catelogue(self, paper_path: str) -> List[str]:
         cand_cate = []
         for page_layout in extract_pages(paper_path):
             for element in page_layout:
                 if isinstance(element, LTTextContainer):
                     title = element.get_text()
-                    if len(title) <= self.title_max_len and len(title) > self.title_min_len:
+                    if len(title) <= self._title_max_len and len(title) > self._title_min_len:
                         cand_cate.append(title)
 
         logger.debug(f"[PaperReader] Extracted candidate catelogue: {cand_cate}")
         return cand_cate
 
     def _extract_catelogue_with_LLM(self, cand_cate: List[str]) -> List[str]:
         messages = [
-            SystemMessage(content=self.system_prompt_for_catelogue),
+            SystemMessage(content=self._catelogue_system_prompt),
             HumanMessage(content=f"These are the texts: {cand_cate}")
         ]
         response = self.chatbot(messages).content
         logger.debug(f"[PaperReader] Raw response from LLM: {response}")
 
         return json.loads(response)["titles"]
 
@@ -79,14 +79,16 @@
         sections.append(full_text[split_pos_list[-1]:].strip())
 
         return sections
 
     def load(self, paper_path: str) -> None:
         """
         Load the paper and extract the catelogue and sections
+
+        :param paper_path: The path of the paper
         """
         self.paper = PdfReader(paper_path)
         self.full_text = ""
         for page in self.paper.pages:
             self.full_text += page.extract_text()
         logger.info(f"[PaperReader] Full Text Size: {len(self.full_text)}")
```

### Comparing `paper2cmap-0.1.0/paper2cmap.egg-info/PKG-INFO` & `paper2cmap-0.1.1/paper2cmap.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper2cmap
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package that automatically generates a concept map for a PDF document using LLM.
 Author-email: weitian <weitian.bnu@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tian Wei
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -53,15 +53,17 @@
 > 
 > Concept maps typically consist of nodes or boxes, which represent concepts or ideas, and lines or arrows, which show the relationships between the concepts. The nodes can be labeled with keywords or short phrases, and the lines or arrows can be labeled with connecting words, such as "leads to," "is a type of," or "causes."
 > 
 > Concept maps can be created by individuals or groups, and can be used to facilitate learning, problem-solving, decision-making, and communication. They are a flexible and powerful tool that can be adapted to many different contexts and purposes.
 
 ### What is Paper2CMap?
 
-Paper2CMap is a package that automatically generates a concept map for a PDF document using LLM. It will first extract the text from the PDF document, then cut the text into sections, and finally generate concept map based on the sections. Currently the generated concept map is in JSON format:
+Paper2CMap is a package that automatically generates a concept map for a PDF document using LLM. It will first cut the text of the PDF document into sections, then generate concept maps for each section, and finally merge and prune these concept maps to generate a final map for the whole document.
+
+Currently the generated concept map is in JSON format:
 ```JSON
 [{"source": "source concept", "target": "target concept", "relationship": "relationship between source and target"}]
 ```
 In future, we will support more formats export, such as LNKG/CXL/SVG.
 
 ## Quick Start
```

### Comparing `paper2cmap-0.1.0/pyproject.toml` & `paper2cmap-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "paper2cmap"
-version = "0.1.0"
+version = "0.1.1"
 description = "A package that automatically generates a concept map for a PDF document using LLM."
 readme = "README.md"
 authors = [{ name = "weitian", email = "weitian.bnu@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `paper2cmap-0.1.0/tests/test_cmapgpt.py` & `paper2cmap-0.1.1/tests/test_cmapgpt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import sys
 sys.path.insert(0, './')
 
-from paper2cmap import CMapGPT, LLMManager
+from paper2cmap import CMapGPT, LLMManager, logger
 
+logger.setLevel("DEBUG")
 
 if __name__ == "__main__":
-    chatbot = LLMManager(temperature=0.2).LLM
+    chatbot = LLMManager().LLM
     
     cmap_gpt = CMapGPT(chatbot=chatbot)
 
     text_input = """
     A large language model (LLM) is a language model consisting of a neural network with many parameters (typically billions of weights or more), trained on large quantities of unlabelled text using self-supervised learning. 
     LLMs emerged around 2018 and perform well at a wide variety of tasks.
     This has shifted the focus of natural language processing research away from the previous paradigm of training specialized supervised models for specific tasks.
     Large language models have most commonly used the transformer architecture, which, since 2018, has become the standard deep learning technique for sequential data (previously, recurrent architectures such as the LSTM were most common).
     LLMs are trained in an unsupervised manner on unannotated text. A left-to-right transformer is trained to maximize the probability assigned to the next word in the training data, given the previous context.
     Alternatively, an LLM may use a bidirectional transformer (as in the example of BERT), which assigns a probability distribution over words given access to both preceding and following context.
     In addition to the task of predicting the next word or "filling in the blanks", LLMs may be trained on auxiliary tasks which test their understanding of the data distribution, such as Next Sentence Prediction (NSP), in which pairs of sentences are presented and the model must predict whether they appear side-by-side in the training corpus.
     """
-    cmap_input = []
 
-    print(cmap_gpt.chat(text_input, cmap_input,
-                        max_num_concepts=5, max_num_relationships=10))
+    cmap = cmap_gpt.generate(text_input, max_num_concepts=5, max_num_relationships=10)
+    print(f"Generated concept map: {cmap}")
+
+    cmap = cmap_gpt.merge_and_prune(cmap, max_num_concepts=5, max_num_relationships=10)
+    print(f"Merged and pruned concept map: {cmap}")
```

