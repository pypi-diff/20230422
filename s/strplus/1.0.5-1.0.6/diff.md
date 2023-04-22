# Comparing `tmp/strplus-1.0.5.tar.gz` & `tmp/strplus-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strplus-1.0.5.tar", max compression
+gzip compressed data, was "strplus-1.0.6.tar", max compression
```

## Comparing `strplus-1.0.5.tar` & `strplus-1.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-04-14 07:41:30.953611 strplus-1.0.5/LICENSE
--rw-r--r--   0        0        0     2859 2023-04-21 05:59:45.510185 strplus-1.0.5/README.md
--rw-r--r--   0        0        0     1027 2023-04-21 05:44:22.660467 strplus-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      161 2023-04-21 05:44:22.660467 strplus-1.0.5/strplus/__init__.py
--rw-r--r--   0        0        0     6703 2023-04-21 07:04:27.239013 strplus-1.0.5/strplus/cases.py
--rw-r--r--   0        0        0     3959 2023-04-21 07:04:27.239013 strplus-1.0.5/strplus/functions.py
--rw-r--r--   0        0        0     4461 2023-04-21 07:04:27.239013 strplus-1.0.5/strplus/strplus.py
--rw-r--r--   0        0        0     3516 1970-01-01 00:00:00.000000 strplus-1.0.5/setup.py
--rw-r--r--   0        0        0     3487 1970-01-01 00:00:00.000000 strplus-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-14 07:41:30.953611 strplus-1.0.6/LICENSE
+-rw-r--r--   0        0        0     2846 2023-04-22 09:01:02.179149 strplus-1.0.6/README.md
+-rw-r--r--   0        0        0     1027 2023-04-22 09:01:02.179149 strplus-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      161 2023-04-22 09:01:02.179149 strplus-1.0.6/strplus/__init__.py
+-rw-r--r--   0        0        0     5957 2023-04-22 09:01:02.179149 strplus-1.0.6/strplus/cases.py
+-rw-r--r--   0        0        0     3886 2023-04-22 09:01:02.179149 strplus-1.0.6/strplus/functions.py
+-rw-r--r--   0        0        0     6342 2023-04-22 09:01:02.179149 strplus-1.0.6/strplus/strplus.py
+-rw-r--r--   0        0        0     3504 1970-01-01 00:00:00.000000 strplus-1.0.6/setup.py
+-rw-r--r--   0        0        0     3474 1970-01-01 00:00:00.000000 strplus-1.0.6/PKG-INFO
```

### Comparing `strplus-1.0.5/LICENSE` & `strplus-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `strplus-1.0.5/README.md` & `strplus-1.0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -50,36 +50,41 @@
 - Simple use!
 - Made with A.I. contribution 🤖 
 
 <br>
 
 ### Simple use example 😍
 ```
->>> my_string = Str('Cast_this_string_TO_Pascal')
->>> my_string.pascal
-'CastThisStringToPascal'
-
->>> my_string = Str('CastMeUseLikeANormalFunction')
->>> my_string.snake
-'cast_me_use_like_a_normal_function'
+my_string = Str('Cast_this_string_TO_Pascal')
+my_string.pascal
+```
+CastThisStringToPascal
+
+<br>
 
 ```
+my_string = Str('CastMeUseLikeANormalFunction')
+my_string.snake
+```
+cast_me_use_like_a_normal_function
+
 <br>
 
-* [More Examples !](https://wiseupdata.github.io/strplus/examples/examples_01/)
-* [Documentations examples](https://wiseupdata.github.io/strplus/index.html)! 
+* [Documentation and more examples! ](https://wiseupdata.github.io/strplus/index.html)! 
 
 <br>
 <br>
 
 # References 🌍 🗄️
 
+1. [strplus](https://wiseupdata.github.io/strplus/index.html)
+1. [Emojis](https://github.com/wiseupdata/emojis)
+1. [Pypi Deploy](https://www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-pypi-using-poetry-on-ubuntu-22-04)
 1. [Wise Up Data](https://github.com/wiseupdata)
-2. [Emojis](https://github.com/wiseupdata/emojis)
-3. [Pypi Deploy](https://www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-pypi-using-poetry-on-ubuntu-22-04)
+
 
 <br>
 <br>
 ---
 
 #### Maintainer 🤗 👨‍💻
```

#### html2text {}

```diff
@@ -14,26 +14,26 @@
 
 
 
 
 [Documentation](https://wiseupdata.github.io/strplus/index.html) ð
 ## Features â¨ï¸ - Wrapper Class - +234 test in 32 Tests files! - Simple use!
 - Made with A.I. contribution ð¤
-### Simple use example ð ``` >>> my_string = Str
-('Cast_this_string_TO_Pascal') >>> my_string.pascal 'CastThisStringToPascal'
->>> my_string = Str('CastMeUseLikeANormalFunction') >>> my_string.snake
-'cast_me_use_like_a_normal_function' ```
-* [More Examples !](https://wiseupdata.github.io/strplus/examples/examples_01/
-) * [Documentations examples](https://wiseupdata.github.io/strplus/index.html)!
-
-
-# References ð ðï¸ 1. [Wise Up Data](https://github.com/wiseupdata) 2.
-[Emojis](https://github.com/wiseupdata/emojis) 3. [Pypi Deploy](https://
-www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-
-pypi-using-poetry-on-ubuntu-22-04)
+### Simple use example ð ``` my_string = Str('Cast_this_string_TO_Pascal')
+my_string.pascal ``` CastThisStringToPascal
+``` my_string = Str('CastMeUseLikeANormalFunction') my_string.snake ```
+cast_me_use_like_a_normal_function
+* [Documentation and more examples! ](https://wiseupdata.github.io/strplus/
+index.html)!
+
+# References ð ðï¸ 1. [strplus](https://wiseupdata.github.io/strplus/
+index.html) 1. [Emojis](https://github.com/wiseupdata/emojis) 1. [Pypi Deploy]
+(https://www.digitalocean.com/community/tutorials/how-to-publish-python-
+packages-to-pypi-using-poetry-on-ubuntu-22-04) 1. [Wise Up Data](https://
+github.com/wiseupdata)
 
 --- #### Maintainer ð¤ ð¨âð» Sivio Liborio ð§
 silvio.liborio@wiseupdata.com silvio-de-melo-liborio_[LinkedIN]
```

### Comparing `strplus-1.0.5/pyproject.toml` & `strplus-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strplus"
-version = "1.0.5"
+version = "1.0.6"
 authors = ["Silvio Liborio <silvio.liborio@wiseupdata.com>"]
 readme = "README.md"
 
 description = "Python extra functions for strings"
 
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `strplus-1.0.5/strplus/cases.py` & `strplus-1.0.6/strplus/cases.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,59 +5,56 @@
 logger = logging.getLogger(__name__)
 
 import re
 
 
 def to_pascal(text: str) -> str:
     """
+
     Simple and efficient method to converts a string to PascalCase.
 
     Args:
     text (str): The input string.
 
     Returns:
         str: The PascalCase version of the input string.
 
-    Examples:
-        !!! example "Converting strings to PascalCase"
-            This example shows how to use `to_pascal()` to convert strings to PascalCase.
-
-            === "Example 1"
-                ```python
-                to_pascal('hello_world')
-                'HelloWorld'
-                ```
-
-            === "Example 2"
-                ```python
-                to_pascal('CamelCase')
-                'CamelCase'
-                ```
-
-            === "Example 3"
-                ```python
-                to_pascal('some-mixed_string With spaces_underscores-and-hyphens')
-                'SomeMixedStringWithSpacesUnderscoresAndHyphens'
-                ```
-
-            === "Example 4"
-                ```python
-                to_pascal('123abc')
-                '123abc'
-                ```
-    warning:
+    !!! Example "Converting strings to PascalCase"
+        This examples shows how to use `to_pascal()` to convert strings to PascalCase.
+
+        === "Example 1"
+            ```python
+            to_pascal('hello_world')
+            ```
+            HelloWorld
+
+        === "Example 2"
+            ```python
+            to_pascal('CamelCase')
+            ```
+            CamelCase
+
+        === "Example 3"
+            ```python
+            to_pascal('some-mixed_string With spaces_underscores-and-hyphens')
+            ```
+            SomeMixedStringWithSpacesUnderscoresAndHyphens
+
+        === "Example 4"
+            ```python
+            to_pascal('123abc')
+            ```
+            123abc
+
+    Info: Important
         - For best results, avoid using punctuation or non-alphanumeric characters in the input string.
         - This function will preserve any digits in the input string.
         - If the input string already has PascalCase formatting, the function will return it unchanged.
         - This function uses regular expressions to identify words in the input string.
 
-    tip: "See also"
-        - `to_camel()` - Converts a string to camelCase formatting.
-        - `to_snake()` - Converts a string to snake_case formatting.
-
     """
     text = text.strip()
 
     if not text:  # If the input string is empty or only whitespace, return an empty string
         return ""
 
     # Remove any underscores, hyphens, or spaces and split the string into words
@@ -73,59 +70,57 @@
 
     # Join the words back together to form the CamelCase string
     return "".join(capitalized_words)
 
 
 def to_camel(text) -> str:
     """
+
     Simple and efficient method to converts a string to camelCase.
 
     Args:
         text (str): The input string.
 
     Returns:
         str: The camelCase version of the input string.
 
-    Examples:
-        !!! example "Converting strings to camelCase"
-            This example shows how to use `to_camel()` to convert strings to camelCase.
-
-            === "Example 1"
-                ```python
-                to_camel('hello_world')
-                'helloWorld'
-                ```
-
-            === "Example 2"
-                ```python
-                to_camel('PascalCase')
-                'pascalCase'
-                ```
-
-            === "Example 3"
-                ```python
-                to_camel('some-mixed_string With spaces_underscores-and-hyphens')
-                'someMixedStringWithSpacesUnderscoresAndHyphens'
-                ```
-
-            === "Example 4"
-                ```python
-                to_camel('123abc')
-                '123abc'
-                ```
+    !!! Example "Converting strings to camelCase"
 
-    warning:
+        This example shows how to use `to_camel()` to convert strings to camelCase.
+
+        === "Example 1"
+            ```python
+            to_camel('hello_world')
+            ```
+            helloWorld
+
+        === "Example 2"
+            ```python
+            to_camel('PascalCase')
+            ```
+            pascalCase
+
+        === "Example 3"
+            ```python
+            to_camel('some-mixed_string With spaces_underscores-and-hyphens')
+            ```
+            someMixedStringWithSpacesUnderscoresAndHyphens
+
+        === "Example 4"
+            ```python
+            to_camel('123abc')
+            ```
+            123abc
+
+    Info: Important
         - For best results, avoid using punctuation or non-alphanumeric characters in the input string.
         - This function will preserve any digits in the input string.
         - If the input string already has camelCase formatting, the function will return it unchanged.
         - This function uses regular expressions to identify words in the input string.
 
-    tip: "See also"
-        - `to_pascal()` - Converts a string to PascalCase formatting.
-        - `to_snake()` - Converts a string to snake_case formatting.
     """
 
     text: str = text.strip()
 
     if not text:  # If the input string is empty, return an empty string
         return ""
 
@@ -142,53 +137,50 @@
     words: str = re.split("[-_]", check_01)
 
     return words[0] + "".join(word.capitalize() for word in words[1:]).replace("_", "")
 
 
 def to_snake(text) -> str:
     """
+
     Converts a string to snake_case.
 
     Args:
         text (str): The input string.
 
     Returns:
         str: The snake_case version of the input string.
 
-    Examples:
-        !!! example "Converting strings to snake_case"
-            This example shows how to use `to_snake()` to convert strings to snake_case.
-
-            === "Example 1"
-                ```python
-                to_snake('helloWorld')
-                'hello_world'
-                ```
-
-            === "Example 2"
-                ```python
-                to_snake('Some-Mixed_string With spaces-underscores-and-hyphens')
-                'some_mixed_string_with_spaces_underscores_and_hyphens'
-                ```
-
-            === "Example 3"
-                ```python
-                to_snake('CamelCase')
-                'camel_case'
-                ```
+    !!! Example "Converting strings to snake_case"
+        This example shows how to use `to_snake()` to convert strings to snake_case.
+
+        === "Example 1"
+            ```python
+            to_snake('helloWorld')
+            ```
+            hello_world
+
+        === "Example 2"
+            ```python
+            to_snake('Some-Mixed_string With spaces-underscores-and-hyphens')
+            ```
+            some_mixed_string_with_spaces_underscores_and_hyphens
+
+        === "Example 3"
+            ```python
+            to_snake('CamelCase')
+            ```
+            camel_case
 
-    Warning:
+    Info: Important
         - For best results, avoid using punctuation or non-alphanumeric characters in the input string.
         - This function will convert any uppercase letters to lowercase, and separate words with underscores.
         - If the input string already has snake_case formatting, the function will return it unchanged.
         - This function uses regular expressions to identify words in the input string.
 
-    Tips:
-        - `to_camel()` - Converts a string to camelCase formatting.
-        - `to_pascal()` - Converts a string to PascalCase formatting.
     """
 
     text: str = text.strip()
 
     if not text:
         # If the input string is empty or only whitespace, return an empty string
         return ""
```

### Comparing `strplus-1.0.5/strplus/functions.py` & `strplus-1.0.6/strplus/functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,106 +1,108 @@
 from strplus.cases import *
 
 
 def to_list(text: str) -> List[str]:
     """
+
     Converts a string to a list of strings, where each word is a separate element in the list.
 
     Args:
         text (str): The input string.
 
     Returns:
         List[str]: A list of strings, where each word in the input string is a separate element in the list.
 
-    Examples:
-        !!! example "Converting a string to a list"
-            This example shows how to use `to_list()` to convert a string to a list.
-
-            === "Example 1"
-                ```python
-                to_list('hello world')
-                ['hello', 'world']
-                ```
-
-            === "Example 2"
-                ```python
-                to_list('HelloWorld')
-                ['Hello', 'World']
-                ```
-
-            === "Example 3"
-                ```python
-                to_list('some-mixed_string With spaces_underscores-and-hyphens')
-                ['some', 'mixed', 'string', 'With', 'spaces', 'underscores', 'and', 'hyphens']
-                ```
-
-            === "Example 4"
-                ```python
-                to_list('123abc')
-                ['123abc']
-                ```
+    !!! Example "Converting a string to a list"
+        This example shows how to use `to_list()` to convert a string to a list.
 
-    Warning:
-        - For best results, avoid using punctuation or non-alphanumeric characters in the input string.
-        - This function uses regular expressions to identify words in the input string.
+        === "Example 1"
+            ```python
+            to_list('hello world')
+            ```
+            ['hello', 'world']
+
+        === "Example 2"
+            ```python
+            to_list('HelloWorld')
+            ```
+            ['Hello', 'World']
+
+        === "Example 3"
+            ```python
+            to_list('some-mixed_string With spaces_underscores-and-hyphens')
+            ```
+            ['some', 'mixed', 'string', 'With', 'spaces', 'underscores', 'and', 'hyphens']
+
+        === "Example 4"
+            ```python
+            to_list('123abc')
+            ```
+            ['123abc']
 
-    Tips:
+    Tip: Use tips
         - If you need to convert a string to a list of integers or floats, you can use list comprehension to convert each element to the desired type.
         - If you need to remove duplicates from the list, you can convert it to a set and then back to a list.
+
+    Info: Important
+        - For best results, avoid using punctuation or non-alphanumeric characters in the input string.
+        - This function uses regular expressions to identify words in the input string.
+
     """
     text = text.strip()
 
     if not text:  # If the input string is empty or only whitespace, return an empty list
         return []
 
     # Remove any non-alphanumeric characters and split the string into words
     word_list = sum([re.findall(r"[a-zA-Z0-9]+", word) for word in re.sub("([A-Z][a-z]+)", r"_\1", re.sub("([A-Z]+)", r"_\1", text)).split()], [])
 
     return word_list
 
 
 def get_separator(input_string):
     """
+
     Finds the most common separator in a given input string.
 
     Args:
         input_string (str): The input string to search for separators.
 
     Returns:
         str or None: The most common separator found in the input string, or None if no separators are found.
 
-
-    !!! example "Finding the most common separator"
+    !!! Example "Finding the most common separator"
         This example shows how to use `get_separator()` to find the most common separator in a string.
 
         === "Example 1"
             ```python
             get_separator('This is a sample sentence, separated by commas')
-            ','
             ```
+            ,
 
         === "Example 2"
             ```python
             get_separator('This string has no separators')
-            None
             ```
+            None
 
         === "Example 3"
             ```python
             get_separator('This string has multiple separators: ;, |, and /')
-            ';'
             ```
+            ;
 
-    Warning:
+    Tip: Use tips
+        - This function can be used to split a string into a list using the most common separator, like so: `input_string.split(get_separator(input_string))`.
+        - To split a string into a list using all possible separators, use the `re.split()` function instead.
+
+    Info: Important
         - This function assumes that the input string contains only valid separators.
         - If multiple separators are tied for the most common, the first one encountered in the list of separators is returned.
 
-    Tips:
-        - This function can be used to split a string into a list using the most common separator, like so: `input_string.split(get_separator(input_string))`.
-        - To split a string into a list using all possible separators, use the `re.split()` function instead.
     """
 
     separators = [",", ";", "|", " ", "\t", ":", "/", "\\", "\n"]
 
     # check each separator in the order of priority
     for sep in [",", ";", "|", " ", "\t", ":", "/", "\\", "\n"]:
         if sep in input_string:
```

### Comparing `strplus-1.0.5/setup.py` & `strplus-1.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['strplus']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'strplus',
-    'version': '1.0.5',
+    'version': '1.0.6',
     'description': 'Python extra functions for strings',
-    'long_description': '<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="Wise Up Data\'s Instagram" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/instagram.png" />   \n</a> \n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s Discord" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/discord.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data | Twitter" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/twitter.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s LinkedIN" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/linkedin.png" />\n</a>\n\n![visitors](https://visitor-badge.glitch.me/badge?page_id=wiseupdata.strplus&left_color=green&right_color=black)\n![license](https://img.shields.io/github/license/wiseupdata/strplus)\n[![pypi](https://img.shields.io/pypi/v/strplus?color=green)](https://pypi.python.org/pypi/strplus)\n[![downloads](https://pepy.tech/badge/strplus/month)](https://pepy.tech/project/strplus)\n[![versions](https://img.shields.io/pypi/pyversions/strplus.svg)](https://github.com/wiseupdata/strplus)\n\n\n\n---\n\n<br>\n<br>\n\n<a href="https://github.com/wiseupdata/wiseupdata">\n<img align="left" alt="img" src="https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/imgs/python.png" width="300" />\n</a>\n\n<h1>\nPython extra functions for strings ❤️\n</h1>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n<br>\n\n[Documentation](https://wiseupdata.github.io/strplus/index.html)  🚀\n\n<br>\n\n## Features ✨️\n\n- Wrapper Class\n- +234 test in 32 Tests files!\n- Simple use!\n- Made with A.I. contribution 🤖 \n\n<br>\n\n### Simple use example 😍\n```\n>>> my_string = Str(\'Cast_this_string_TO_Pascal\')\n>>> my_string.pascal\n\'CastThisStringToPascal\'\n\n>>> my_string = Str(\'CastMeUseLikeANormalFunction\')\n>>> my_string.snake\n\'cast_me_use_like_a_normal_function\'\n\n```\n<br>\n\n* [More Examples !](https://wiseupdata.github.io/strplus/examples/examples_01/)\n* [Documentations examples](https://wiseupdata.github.io/strplus/index.html)! \n\n<br>\n<br>\n\n# References 🌍 🗄️\n\n1. [Wise Up Data](https://github.com/wiseupdata)\n2. [Emojis](https://github.com/wiseupdata/emojis)\n3. [Pypi Deploy](https://www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-pypi-using-poetry-on-ubuntu-22-04)\n\n<br>\n<br>\n---\n\n#### Maintainer 🤗 👨\u200d💻\n\nSivio Liborio\n\n📧 silvio.liborio@wiseupdata.com\n\n<a href="https://www.linkedin.com/in/silvio-de-melo-liborio">silvio-de-melo-liborio <img align="left" alt="LinkedIN" width="18px" src="https://raw.githubusercontent.com/wiseupdata/wsl-latest/main/assets/linkedin.svg" />\n</a>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n\n> WiseUpData\n',
+    'long_description': '<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="Wise Up Data\'s Instagram" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/instagram.png" />   \n</a> \n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s Discord" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/discord.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data | Twitter" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/twitter.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s LinkedIN" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/linkedin.png" />\n</a>\n\n![visitors](https://visitor-badge.glitch.me/badge?page_id=wiseupdata.strplus&left_color=green&right_color=black)\n![license](https://img.shields.io/github/license/wiseupdata/strplus)\n[![pypi](https://img.shields.io/pypi/v/strplus?color=green)](https://pypi.python.org/pypi/strplus)\n[![downloads](https://pepy.tech/badge/strplus/month)](https://pepy.tech/project/strplus)\n[![versions](https://img.shields.io/pypi/pyversions/strplus.svg)](https://github.com/wiseupdata/strplus)\n\n\n\n---\n\n<br>\n<br>\n\n<a href="https://github.com/wiseupdata/wiseupdata">\n<img align="left" alt="img" src="https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/imgs/python.png" width="300" />\n</a>\n\n<h1>\nPython extra functions for strings ❤️\n</h1>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n<br>\n\n[Documentation](https://wiseupdata.github.io/strplus/index.html)  🚀\n\n<br>\n\n## Features ✨️\n\n- Wrapper Class\n- +234 test in 32 Tests files!\n- Simple use!\n- Made with A.I. contribution 🤖 \n\n<br>\n\n### Simple use example 😍\n```\nmy_string = Str(\'Cast_this_string_TO_Pascal\')\nmy_string.pascal\n```\nCastThisStringToPascal\n\n<br>\n\n```\nmy_string = Str(\'CastMeUseLikeANormalFunction\')\nmy_string.snake\n```\ncast_me_use_like_a_normal_function\n\n<br>\n\n* [Documentation and more examples! ](https://wiseupdata.github.io/strplus/index.html)! \n\n<br>\n<br>\n\n# References 🌍 🗄️\n\n1. [strplus](https://wiseupdata.github.io/strplus/index.html)\n1. [Emojis](https://github.com/wiseupdata/emojis)\n1. [Pypi Deploy](https://www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-pypi-using-poetry-on-ubuntu-22-04)\n1. [Wise Up Data](https://github.com/wiseupdata)\n\n\n<br>\n<br>\n---\n\n#### Maintainer 🤗 👨\u200d💻\n\nSivio Liborio\n\n📧 silvio.liborio@wiseupdata.com\n\n<a href="https://www.linkedin.com/in/silvio-de-melo-liborio">silvio-de-melo-liborio <img align="left" alt="LinkedIN" width="18px" src="https://raw.githubusercontent.com/wiseupdata/wsl-latest/main/assets/linkedin.svg" />\n</a>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n\n> WiseUpData\n',
     'author': 'Silvio Liborio',
     'author_email': 'silvio.liborio@wiseupdata.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['strplus']
 package_data = \ {'': ['*']} setup_kwargs = { 'name': 'strplus', 'version':
-'1.0.5', 'description': 'Python extra functions for strings',
+'1.0.6', 'description': 'Python extra functions for strings',
 'long_description': '\n_[Wise_Up_Data\'s_Instagram]_\n \n\n_[wise_Up_Data\'s
 Discord]\n\n\n_[wise_Up_Data_|_Twitter]\n\n\n_[wise_Up_Data\'s_LinkedIN]\n\n\n!
 [visitors](https://visitor-badge.glitch.me/
 badge?page_id=wiseupdata.strplus&left_color=green&right_color=black)\n!
 [license](https://img.shields.io/github/license/wiseupdata/strplus)\n[![pypi]
 (https://img.shields.io/pypi/v/strplus?color=green)](https://pypi.python.org/
 pypi/strplus)\n[![downloads](https://pepy.tech/badge/strplus/month)](https://
@@ -18,27 +18,26 @@
 \n
 \n
 \n
 \n
 \n\n[Documentation](https://wiseupdata.github.io/strplus/index.html) ð\n\n
 \n\n## Features â¨ï¸\n\n- Wrapper Class\n- +234 test in 32 Tests files!\n-
 Simple use!\n- Made with A.I. contribution ð¤ \n\n
-\n\n### Simple use example ð\n```\n>>> my_string = Str
-(\'Cast_this_string_TO_Pascal\')\n>>>
-my_string.pascal\n\'CastThisStringToPascal\'\n\n>>> my_string = Str
-(\'CastMeUseLikeANormalFunction\')\n>>>
-my_string.snake\n\'cast_me_use_like_a_normal_function\'\n\n```\n
-\n\n* [More Examples !](https://wiseupdata.github.io/strplus/examples/
-examples_01/)\n* [Documentations examples](https://wiseupdata.github.io/
-strplus/index.html)! \n\n
-\n
-\n\n# References ð ðï¸\n\n1. [Wise Up Data](https://github.com/
-wiseupdata)\n2. [Emojis](https://github.com/wiseupdata/emojis)\n3. [Pypi
-Deploy](https://www.digitalocean.com/community/tutorials/how-to-publish-python-
-packages-to-pypi-using-poetry-on-ubuntu-22-04)\n\n
+\n\n### Simple use example ð\n```\nmy_string = Str
+(\'Cast_this_string_TO_Pascal\')\nmy_string.pascal\n```\nCastThisStringToPascal\n\n
+\n\n```\nmy_string = Str
+(\'CastMeUseLikeANormalFunction\')\nmy_string.snake\n```\ncast_me_use_like_a_normal_function\n\n
+\n\n* [Documentation and more examples! ](https://wiseupdata.github.io/strplus/
+index.html)! \n\n
+\n
+\n\n# References ð ðï¸\n\n1. [strplus](https://wiseupdata.github.io/
+strplus/index.html)\n1. [Emojis](https://github.com/wiseupdata/emojis)\n1.
+[Pypi Deploy](https://www.digitalocean.com/community/tutorials/how-to-publish-
+python-packages-to-pypi-using-poetry-on-ubuntu-22-04)\n1. [Wise Up Data](https:
+//github.com/wiseupdata)\n\n\n
 \n
 \n---\n\n#### Maintainer ð¤ ð¨\u200dð»\n\nSivio Liborio\n\nð§
 silvio.liborio@wiseupdata.com\n\nsilvio-de-melo-liborio_[LinkedIN]\n\n\n
 \n
 \n
 \n
 \n
```

### Comparing `strplus-1.0.5/PKG-INFO` & `strplus-1.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strplus
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python extra functions for strings
 Author: Silvio Liborio
 Author-email: silvio.liborio@wiseupdata.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -67,36 +67,41 @@
 - Simple use!
 - Made with A.I. contribution 🤖 
 
 <br>
 
 ### Simple use example 😍
 ```
->>> my_string = Str('Cast_this_string_TO_Pascal')
->>> my_string.pascal
-'CastThisStringToPascal'
-
->>> my_string = Str('CastMeUseLikeANormalFunction')
->>> my_string.snake
-'cast_me_use_like_a_normal_function'
+my_string = Str('Cast_this_string_TO_Pascal')
+my_string.pascal
+```
+CastThisStringToPascal
+
+<br>
 
 ```
+my_string = Str('CastMeUseLikeANormalFunction')
+my_string.snake
+```
+cast_me_use_like_a_normal_function
+
 <br>
 
-* [More Examples !](https://wiseupdata.github.io/strplus/examples/examples_01/)
-* [Documentations examples](https://wiseupdata.github.io/strplus/index.html)! 
+* [Documentation and more examples! ](https://wiseupdata.github.io/strplus/index.html)! 
 
 <br>
 <br>
 
 # References 🌍 🗄️
 
+1. [strplus](https://wiseupdata.github.io/strplus/index.html)
+1. [Emojis](https://github.com/wiseupdata/emojis)
+1. [Pypi Deploy](https://www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-pypi-using-poetry-on-ubuntu-22-04)
 1. [Wise Up Data](https://github.com/wiseupdata)
-2. [Emojis](https://github.com/wiseupdata/emojis)
-3. [Pypi Deploy](https://www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-pypi-using-poetry-on-ubuntu-22-04)
+
 
 <br>
 <br>
 ---
 
 #### Maintainer 🤗 👨‍💻
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: strplus Version: 1.0.5 Summary: Python extra
+Metadata-Version: 2.1 Name: strplus Version: 1.0.6 Summary: Python extra
 functions for strings Author: Silvio Liborio Author-email:
 silvio.liborio@wiseupdata.com Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3
@@ -23,26 +23,26 @@
 
 
 
 
 [Documentation](https://wiseupdata.github.io/strplus/index.html) ð
 ## Features â¨ï¸ - Wrapper Class - +234 test in 32 Tests files! - Simple use!
 - Made with A.I. contribution ð¤
-### Simple use example ð ``` >>> my_string = Str
-('Cast_this_string_TO_Pascal') >>> my_string.pascal 'CastThisStringToPascal'
->>> my_string = Str('CastMeUseLikeANormalFunction') >>> my_string.snake
-'cast_me_use_like_a_normal_function' ```
-* [More Examples !](https://wiseupdata.github.io/strplus/examples/examples_01/
-) * [Documentations examples](https://wiseupdata.github.io/strplus/index.html)!
-
-
-# References ð ðï¸ 1. [Wise Up Data](https://github.com/wiseupdata) 2.
-[Emojis](https://github.com/wiseupdata/emojis) 3. [Pypi Deploy](https://
-www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-
-pypi-using-poetry-on-ubuntu-22-04)
+### Simple use example ð ``` my_string = Str('Cast_this_string_TO_Pascal')
+my_string.pascal ``` CastThisStringToPascal
+``` my_string = Str('CastMeUseLikeANormalFunction') my_string.snake ```
+cast_me_use_like_a_normal_function
+* [Documentation and more examples! ](https://wiseupdata.github.io/strplus/
+index.html)!
+
+# References ð ðï¸ 1. [strplus](https://wiseupdata.github.io/strplus/
+index.html) 1. [Emojis](https://github.com/wiseupdata/emojis) 1. [Pypi Deploy]
+(https://www.digitalocean.com/community/tutorials/how-to-publish-python-
+packages-to-pypi-using-poetry-on-ubuntu-22-04) 1. [Wise Up Data](https://
+github.com/wiseupdata)
 
 --- #### Maintainer ð¤ ð¨âð» Sivio Liborio ð§
 silvio.liborio@wiseupdata.com silvio-de-melo-liborio_[LinkedIN]
```

