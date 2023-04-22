# Comparing `tmp/khl-1.0.6.tar.gz` & `tmp/khl-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khl-1.0.6.tar", max compression
+gzip compressed data, was "khl-1.0.7.tar", max compression
```

## Comparing `khl-1.0.6.tar` & `khl-1.0.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1065 2023-03-05 17:17:58.027493 khl-1.0.6/LICENSE
--rw-r--r--   0        0        0     5528 2023-03-05 17:17:58.027493 khl-1.0.6/README.md
--rw-r--r--   0        0        0     2297 2023-04-20 19:36:25.798785 khl-1.0.6/khl/__init__.py
--rw-r--r--   0        0        0     8829 2023-03-10 16:38:07.463209 khl-1.0.6/khl/preprocess.py
--rw-r--r--   0        0        0     2426 2023-03-10 17:49:51.106914 khl-1.0.6/khl/stop_words.py
--rw-r--r--   0        0        0     3274 2023-03-10 16:26:00.431309 khl-1.0.6/khl/teams_orgs.py
--rw-r--r--   0        0        0    30765 2023-04-20 19:34:54.754745 khl-1.0.6/khl/utils.py
--rw-r--r--   0        0        0     8346 2023-03-05 17:17:58.031493 khl-1.0.6/khl/wrong_lemmas.py
--rw-r--r--   0        0        0     1589 2023-04-20 19:36:32.994513 khl-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     6469 1970-01-01 00:00:00.000000 khl-1.0.6/setup.py
--rw-r--r--   0        0        0     6251 1970-01-01 00:00:00.000000 khl-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-03-05 17:17:58.027493 khl-1.0.7/LICENSE
+-rw-r--r--   0        0        0     5525 2023-04-22 10:15:25.994692 khl-1.0.7/README.md
+-rw-r--r--   0        0        0     2297 2023-04-22 10:54:10.906352 khl-1.0.7/khl/__init__.py
+-rw-r--r--   0        0        0     8829 2023-03-10 16:38:07.463209 khl-1.0.7/khl/preprocess.py
+-rw-r--r--   0        0        0     2426 2023-03-10 17:49:51.106914 khl-1.0.7/khl/stop_words.py
+-rw-r--r--   0        0        0     3274 2023-03-10 16:26:00.431309 khl-1.0.7/khl/teams_orgs.py
+-rw-r--r--   0        0        0    31173 2023-04-22 10:53:40.734066 khl-1.0.7/khl/utils.py
+-rw-r--r--   0        0        0     8346 2023-03-05 17:17:58.031493 khl-1.0.7/khl/wrong_lemmas.py
+-rw-r--r--   0        0        0     1589 2023-04-22 10:54:16.494404 khl-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     6466 1970-01-01 00:00:00.000000 khl-1.0.7/setup.py
+-rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 khl-1.0.7/PKG-INFO
```

### Comparing `khl-1.0.6/LICENSE` & `khl-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `khl-1.0.6/README.md` & `khl-1.0.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 ```python
 simplified_text = utils.simplify_text(
     text=unified_text,
     replace_ners_=True,
     replace_dates_=True,
     replace_penalties_=True,
 )
-# 'date в loc в матче финала против org per забил свой гол за карьеру. org org Голы забили: per per и per.'
+# 'date в loc в матче финала против org per забил свой гол за карьеру. org org Голы забили: per per per.'
 ```
 
 #### 6. Lemmatize
 ```python
 lemmas = preprocess.lemmatize(text=simplified_text, stop_words_=stop_words)
 # ['date', 'loc', 'матч', 'финал', 'против', 'org', 'per', 'забить', 'гол', 'карьера', '.', 'orgs', 'гол', 'забить', ':', 'pers', '.']
 ```
```

### Comparing `khl-1.0.6/khl/__init__.py` & `khl-1.0.7/khl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Подготовка русскоязычных текстов хоккейных новостей для обучения нейронных сетей."""
 
-__version__ = "1.0.6"
+__version__ = "1.0.7"
 
 from typing import Dict, List, Optional
 
 from khl import preprocess, utils
 from khl.stop_words import stop_words
```

### Comparing `khl-1.0.6/khl/preprocess.py` & `khl-1.0.7/khl/preprocess.py`

 * *Files identical despite different names*

### Comparing `khl-1.0.6/khl/stop_words.py` & `khl-1.0.7/khl/stop_words.py`

 * *Files identical despite different names*

### Comparing `khl-1.0.6/khl/teams_orgs.py` & `khl-1.0.7/khl/teams_orgs.py`

 * *Files identical despite different names*

### Comparing `khl-1.0.6/khl/utils.py` & `khl-1.0.7/khl/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,14 +200,21 @@
 def replace_sdk(text: str) -> str:
     """'спортивно-дисциплинарный комитет' -> 'сдк'."""
     pattern = r"спортивн[а-я]+[ -]*дисциплинарн[а-я]+(?:\s*комитет[а-я]*)?"
     result = re.sub(pattern, "сдк", text, flags=re.IGNORECASE)
     return result
 
 
+def fix_press_conference(text: str) -> str:
+    """'Пресс конференция' -> 'Пресс-конференция'."""
+    pattern = r"(?<=пресс)[\s-]*(?=конференц)"
+    result = re.sub(pattern, "-", text, flags=re.IGNORECASE)
+    return result
+
+
 def delete_numeric_data(text: str) -> str:
     """Удаление данных типа 12:25, 2-10."""
     pattern = r"\b\d+\s*(?:[:-]\s*\d+)+\b(?!-)"
     result = re.sub(pattern, "", text)
     return result
 
 
@@ -746,39 +753,40 @@
       16. Оставляем только русское слово из связки 'английское-русское'
       17. Удаляем возрастные категории типа U-18
       18. Удаляем годы рождения
       19. Корректирум 'Иванов-Петров-Сидоров' -> 'Иванов - Петров - Сидоров'
       20. Корректируем ' -Иванов' -> ' - Иванов', 'Иванов- ' -> 'Иванов - '
       21. Преобразуем 'СДК' -> 'сдк'
       22. Преобразуем 'спортивно-дисциплинарный комитет' -> 'сдк'
-      23. Обобщаем ТОП
-      24. Заменяем ner'ы (если необходимо)
-      25. Заменяем даты (если необходимо)
-      26. Заменяем удаления (если необходимо)
-      27. Удаляем пометки годов
-      28. Разделяем слипшиеся ner'ы
-      29. Удаляем ссылки
-      30. Удаляем кавычки с одним символом внутри
-      31. Удаляем английские слова, состоящие только из одной буквы
-      32. Удаляем числовые данные
-      33. Удаляем порядковые числительные
-      34. Удаляем формат игры ('5x5', '3 на 4' и т.д.)
-      35. Заменяем восклицательные знаки на точки
-      36. Оставляем только нужные символы
-      37. 'org loc' -> 'org'
-      38. Схлопываем пробелы
-      39. Схлопываем тире
-      40. Заменяем тире между ner'ами на пробел
-      41. Удаление тире в начале или в конце слова
-      42. Корректируем точки
-      43. Корректируем вопросительные знаки
-      44. Корректируем '?..' -> '?'
-      45. Корректируем '..?' -> '?'
-      46. Удаляем тире и двоеточия в конце текста (rstrip)
-      47. Корректируем ' :' -> ':'
+      23. Правим 'пресс конференция' -> 'пресс-конференция'
+      24. Обобщаем ТОП
+      25. Заменяем ner'ы (если необходимо)
+      26. Заменяем даты (если необходимо)
+      27. Заменяем удаления (если необходимо)
+      28. Удаляем пометки годов
+      29. Разделяем слипшиеся ner'ы
+      30. Удаляем ссылки
+      31. Удаляем кавычки с одним символом внутри
+      32. Удаляем английские слова, состоящие только из одной буквы
+      33. Удаляем числовые данные
+      34. Удаляем порядковые числительные
+      35. Удаляем формат игры ('5x5', '3 на 4' и т.д.)
+      36. Заменяем восклицательные знаки на точки
+      37. Оставляем только нужные символы
+      38. 'org loc' -> 'org'
+      39. Схлопываем пробелы
+      40. Схлопываем тире
+      41. Заменяем тире между ner'ами на пробел
+      42. Удаление тире в начале или в конце слова
+      43. Корректируем точки
+      44. Корректируем вопросительные знаки
+      45. Корректируем '?..' -> '?'
+      46. Корректируем '..?' -> '?'
+      47. Удаляем тире и двоеточия в конце текста (rstrip)
+      48. Корректируем ' :' -> ':'
     """
     text = delete_parentheses_content(text)
     text = replace_tak_kak(text)
     text = replace_to_est(text)
     text = delete_letter_dot_letter_dot(text)
     text = fix_b_o_lshii(text)
     text = delete_shutouts(text)
@@ -794,14 +802,15 @@
     text = fix_english_dash_russian_words(text)
     text = delete_age_category(text)
     text = delete_birth_mark(text)
     text = fix_surname_dash_surname_dash_surname(text)
     text = fix_dash_word(text)
     text = lowercase_sdk(text)
     text = replace_sdk(text)
+    text = fix_press_conference(text)
     text = generalize_top(text)
     if replace_ners_:
         text = replace_ners(text)
     if replace_dates_:
         text = replace_dates(text)
     if replace_penalties_:
         text = replace_penalty(text)
```

### Comparing `khl-1.0.6/khl/wrong_lemmas.py` & `khl-1.0.7/khl/wrong_lemmas.py`

 * *Files identical despite different names*

### Comparing `khl-1.0.6/pyproject.toml` & `khl-1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "khl"
-version = "1.0.6"
+version = "1.0.7"
 description = "Preparing russian hockey news for machine learning"
 readme = "README.md"
 license = "MIT"
 authors = ["Rishat Fayzullin <nilluziaf@gmail.com>"]
 repository = "https://github.com/Rishat-F/khl"
 keywords = ["khl", "news", "nlp", "preprocessing", "ml"]
```

### Comparing `khl-1.0.6/setup.py` & `khl-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['natasha==1.4.0']
 
 setup_kwargs = {
     'name': 'khl',
-    'version': '1.0.6',
+    'version': '1.0.7',
     'description': 'Preparing russian hockey news for machine learning',
-    'long_description': '![Khl Logo](https://raw.githubusercontent.com/Rishat-F/khl/master/data/logo.png)\n\n<h1 align="center">No Water - Ice Only</h1>\n\nPreparing russian hockey news for machine learning.\n\n**Unify -> Simplify -> Preprocess** text and feed your neural model.\n\n## Installation\n\n*Khl* is available on PyPI:\n\n```console\n$ pip install khl\n```\nIt requires Python 3.8+ to run.\n\n## Usage\n\nTo get started right away with basic usage:\n\n```python\nfrom khl import text_to_codes\n\nlemmas_coder = {\n    \'\': 0,     # placeholder\n    \'???\': 1,  # unknown\n    \'.\': 2,\n    \'и\': 3,\n    \'в\': 4,\n    \'-\': 5,\n    \':\': 6,\n    \'матч\': 7,\n    \'за\': 8,\n    \'забить\': 9,\n    \'гол\': 10,\n    \'per\': 11,   # person entity\n    \'org\': 12,   # organization entity\n    \'loc\': 13,   # location entity\n    \'date\': 14,  # date entity\n    \'против\': 15,\n    \'год\': 16,\n    \'pers\': 17,  # few persons entity\n    \'orgs\': 18,  # few organizations entity\n    \'свой\': 19\n}\n\ntext = """\n    1 апреля 2023 года в Москве в матче ⅛ финала против „Спартака” Иван Иванов забил свой 100—й гол за карьеру.\n    «Динамо Мск» - «Спартак» 2:1 ОТ (1:0 0:1 0:0 1:0) Голы забили: Иванов, Петров и Сидоров.\n"""\n\ncodes = text_to_codes(\n    text=text,\n    lemmas_coder=lemmas_coder,\n    stop_words_=["в", "за", "и", "свой"],  # stop words to drop\n    replace_ners_=True,                    # replace named entities ("Иван Иванов" -> "per", "Спартак" -> "org", "Москва" -> "loc")\n    replace_dates_=True,                   # replace dates ("1 апреля 2023 года" -> "date")\n    replace_penalties_=True,               # replace penalties ("5+20" -> "pen")\n    exclude_unknown=True,                  # drop lemma that not presented in lemmas_coder\n    max_len=20,                            # get sequence of codes of length 20\n)\n# codes = [0, 0, 0, 0, 0, 14, 13, 7, 15, 12, 11, 9, 10, 2, 18, 10, 9, 6, 17, 2]\n```\n\n```text_to_codes``` is a very high level function. What\'s happens under hood see in [Lower level usage](#lower-level-usage).\n\n## What is `lemmas_coder`?\n`lemmas_coder` is just a dictionary where each lemma is represented with unique integer code.\nNote that first two elements are reserved for *placeholder* and *unknown* elements.\n\nIt is possible to get `lemmas_coder` from frequency dictionary file (see in [Get lemmas coder](#2-get-lemmas-coder)).\nFrequency dictionary file is a **json**-file with dictionary where key is lemma and value is how many times this lemma occurred in your whole dataset.\nPreferably it should be sorted in descending order of values.  \n`example_frequency_dictionary.json`:\n\n```json\n{\n  ".": 1000,\n  "и": 500,\n  "в": 400,\n  "-": 300,\n  ":": 300,\n  "матч": 290,\n  "за": 250,\n  "забить": 240,\n  "гол": 230,\n  "per": 200,\n  "org": 150,\n  "loc": 150,\n  "date": 100,\n  "против": 90,\n  "год": 70,\n  "pers": 40,\n  "orgs": 30,\n  "свой": 20\n}\n```\n\nYou could make and use your own frequency dictionary or download [this dictionary](https://github.com/Rishat-F/khl/blob/master/data/frequency_dictionary.json) created by myself.\n\n## Lower level usage<a id="lower-level-usage"></a>\n\n#### 1. Make imports\n```python\nfrom khl import stop_words\nfrom khl import utils\nfrom khl import preprocess\n```\n\n#### 2. Get lemmas coder<a id="2-get-lemmas-coder"></a>\n```python\nlemmas_coder = preprocess.get_lemmas_coder("example_frequency_dictionary.json")\n```\n\n#### 3. Define text\n```python\ntext = """\n    1 апреля 2023 года в Москве в матче ⅛ финала против „Спартака” Иван Иванов забил свой 100—й гол за карьеру.\n    «Динамо Мск» - «Спартак» 2:1 ОТ (1:0 0:1 0:0 1:0) Голы забили: Иванов, Петров и Сидоров.\n"""\n```\n\n#### 4. Unify\n```python\nunified_text = utils.unify_text(text)\n# "1 апреля 2023 года в Москве в матче 1/8 финала против \'Спартака\' Иван Иванов забил свой 100-й гол за карьеру. \'Динамо Мск\' - \'Спартак\' 2:1 ОТ (1:0 0:1 0:0 1:0) Голы забили: Иванов, Петров и Сидоров."\n```\n\n#### 5. Simplify\n```python\nsimplified_text = utils.simplify_text(\n    text=unified_text,\n    replace_ners_=True,\n    replace_dates_=True,\n    replace_penalties_=True,\n)\n# \'date в loc в матче финала против org per забил свой гол за карьеру. org org Голы забили: per per и per.\'\n```\n\n#### 6. Lemmatize\n```python\nlemmas = preprocess.lemmatize(text=simplified_text, stop_words_=stop_words)\n# [\'date\', \'loc\', \'матч\', \'финал\', \'против\', \'org\', \'per\', \'забить\', \'гол\', \'карьера\', \'.\', \'orgs\', \'гол\', \'забить\', \':\', \'pers\', \'.\']\n```\n\n#### 7. Transform to codes\n```python\ncodes = preprocess.lemmas_to_codes(\n    lemmas=lemmas,\n    lemmas_coder=lemmas_coder,\n    exclude_unknown=True,\n    max_len=20,\n)\n# [0, 0, 0, 0, 0, 14, 13, 7, 15, 12, 11, 9, 10, 2, 18, 10, 9, 6, 17, 2]\n```\n\n#### 8. Transform to lemmas back (just to look which lemmas are presented in codes sequence)\n```python\nprint(\n    preprocess.codes_to_lemmas(codes=codes, lemmas_coder=lemmas_coder)\n)\n# [\'\', \'\', \'\', \'\', \'\', \'date\', \'loc\', \'матч\', \'против\', \'org\', \'per\', \'забить\', \'гол\', \'.\', \'orgs\', \'гол\', \'забить\', \':\', \'pers\', \'.\']\n```\n',
+    'long_description': '![Khl Logo](https://raw.githubusercontent.com/Rishat-F/khl/master/data/logo.png)\n\n<h1 align="center">No Water - Ice Only</h1>\n\nPreparing russian hockey news for machine learning.\n\n**Unify -> Simplify -> Preprocess** text and feed your neural model.\n\n## Installation\n\n*Khl* is available on PyPI:\n\n```console\n$ pip install khl\n```\nIt requires Python 3.8+ to run.\n\n## Usage\n\nTo get started right away with basic usage:\n\n```python\nfrom khl import text_to_codes\n\nlemmas_coder = {\n    \'\': 0,     # placeholder\n    \'???\': 1,  # unknown\n    \'.\': 2,\n    \'и\': 3,\n    \'в\': 4,\n    \'-\': 5,\n    \':\': 6,\n    \'матч\': 7,\n    \'за\': 8,\n    \'забить\': 9,\n    \'гол\': 10,\n    \'per\': 11,   # person entity\n    \'org\': 12,   # organization entity\n    \'loc\': 13,   # location entity\n    \'date\': 14,  # date entity\n    \'против\': 15,\n    \'год\': 16,\n    \'pers\': 17,  # few persons entity\n    \'orgs\': 18,  # few organizations entity\n    \'свой\': 19\n}\n\ntext = """\n    1 апреля 2023 года в Москве в матче ⅛ финала против „Спартака” Иван Иванов забил свой 100—й гол за карьеру.\n    «Динамо Мск» - «Спартак» 2:1 ОТ (1:0 0:1 0:0 1:0) Голы забили: Иванов, Петров и Сидоров.\n"""\n\ncodes = text_to_codes(\n    text=text,\n    lemmas_coder=lemmas_coder,\n    stop_words_=["в", "за", "и", "свой"],  # stop words to drop\n    replace_ners_=True,                    # replace named entities ("Иван Иванов" -> "per", "Спартак" -> "org", "Москва" -> "loc")\n    replace_dates_=True,                   # replace dates ("1 апреля 2023 года" -> "date")\n    replace_penalties_=True,               # replace penalties ("5+20" -> "pen")\n    exclude_unknown=True,                  # drop lemma that not presented in lemmas_coder\n    max_len=20,                            # get sequence of codes of length 20\n)\n# codes = [0, 0, 0, 0, 0, 14, 13, 7, 15, 12, 11, 9, 10, 2, 18, 10, 9, 6, 17, 2]\n```\n\n```text_to_codes``` is a very high level function. What\'s happens under hood see in [Lower level usage](#lower-level-usage).\n\n## What is `lemmas_coder`?\n`lemmas_coder` is just a dictionary where each lemma is represented with unique integer code.\nNote that first two elements are reserved for *placeholder* and *unknown* elements.\n\nIt is possible to get `lemmas_coder` from frequency dictionary file (see in [Get lemmas coder](#2-get-lemmas-coder)).\nFrequency dictionary file is a **json**-file with dictionary where key is lemma and value is how many times this lemma occurred in your whole dataset.\nPreferably it should be sorted in descending order of values.  \n`example_frequency_dictionary.json`:\n\n```json\n{\n  ".": 1000,\n  "и": 500,\n  "в": 400,\n  "-": 300,\n  ":": 300,\n  "матч": 290,\n  "за": 250,\n  "забить": 240,\n  "гол": 230,\n  "per": 200,\n  "org": 150,\n  "loc": 150,\n  "date": 100,\n  "против": 90,\n  "год": 70,\n  "pers": 40,\n  "orgs": 30,\n  "свой": 20\n}\n```\n\nYou could make and use your own frequency dictionary or download [this dictionary](https://github.com/Rishat-F/khl/blob/master/data/frequency_dictionary.json) created by myself.\n\n## Lower level usage<a id="lower-level-usage"></a>\n\n#### 1. Make imports\n```python\nfrom khl import stop_words\nfrom khl import utils\nfrom khl import preprocess\n```\n\n#### 2. Get lemmas coder<a id="2-get-lemmas-coder"></a>\n```python\nlemmas_coder = preprocess.get_lemmas_coder("example_frequency_dictionary.json")\n```\n\n#### 3. Define text\n```python\ntext = """\n    1 апреля 2023 года в Москве в матче ⅛ финала против „Спартака” Иван Иванов забил свой 100—й гол за карьеру.\n    «Динамо Мск» - «Спартак» 2:1 ОТ (1:0 0:1 0:0 1:0) Голы забили: Иванов, Петров и Сидоров.\n"""\n```\n\n#### 4. Unify\n```python\nunified_text = utils.unify_text(text)\n# "1 апреля 2023 года в Москве в матче 1/8 финала против \'Спартака\' Иван Иванов забил свой 100-й гол за карьеру. \'Динамо Мск\' - \'Спартак\' 2:1 ОТ (1:0 0:1 0:0 1:0) Голы забили: Иванов, Петров и Сидоров."\n```\n\n#### 5. Simplify\n```python\nsimplified_text = utils.simplify_text(\n    text=unified_text,\n    replace_ners_=True,\n    replace_dates_=True,\n    replace_penalties_=True,\n)\n# \'date в loc в матче финала против org per забил свой гол за карьеру. org org Голы забили: per per per.\'\n```\n\n#### 6. Lemmatize\n```python\nlemmas = preprocess.lemmatize(text=simplified_text, stop_words_=stop_words)\n# [\'date\', \'loc\', \'матч\', \'финал\', \'против\', \'org\', \'per\', \'забить\', \'гол\', \'карьера\', \'.\', \'orgs\', \'гол\', \'забить\', \':\', \'pers\', \'.\']\n```\n\n#### 7. Transform to codes\n```python\ncodes = preprocess.lemmas_to_codes(\n    lemmas=lemmas,\n    lemmas_coder=lemmas_coder,\n    exclude_unknown=True,\n    max_len=20,\n)\n# [0, 0, 0, 0, 0, 14, 13, 7, 15, 12, 11, 9, 10, 2, 18, 10, 9, 6, 17, 2]\n```\n\n#### 8. Transform to lemmas back (just to look which lemmas are presented in codes sequence)\n```python\nprint(\n    preprocess.codes_to_lemmas(codes=codes, lemmas_coder=lemmas_coder)\n)\n# [\'\', \'\', \'\', \'\', \'\', \'date\', \'loc\', \'матч\', \'против\', \'org\', \'per\', \'забить\', \'гол\', \'.\', \'orgs\', \'гол\', \'забить\', \':\', \'pers\', \'.\']\n```\n',
     'author': 'Rishat Fayzullin',
     'author_email': 'nilluziaf@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Rishat-F/khl',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `khl-1.0.6/PKG-INFO` & `khl-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khl
-Version: 1.0.6
+Version: 1.0.7
 Summary: Preparing russian hockey news for machine learning
 Home-page: https://github.com/Rishat-F/khl
 License: MIT
 Keywords: khl,news,nlp,preprocessing,ml
 Author: Rishat Fayzullin
 Author-email: nilluziaf@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -151,15 +151,15 @@
 ```python
 simplified_text = utils.simplify_text(
     text=unified_text,
     replace_ners_=True,
     replace_dates_=True,
     replace_penalties_=True,
 )
-# 'date в loc в матче финала против org per забил свой гол за карьеру. org org Голы забили: per per и per.'
+# 'date в loc в матче финала против org per забил свой гол за карьеру. org org Голы забили: per per per.'
 ```
 
 #### 6. Lemmatize
 ```python
 lemmas = preprocess.lemmatize(text=simplified_text, stop_words_=stop_words)
 # ['date', 'loc', 'матч', 'финал', 'против', 'org', 'per', 'забить', 'гол', 'карьера', '.', 'orgs', 'гол', 'забить', ':', 'pers', '.']
 ```
```

