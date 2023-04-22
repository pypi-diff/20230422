# Comparing `tmp/aniemore-1.0.6.tar.gz` & `tmp/aniemore-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aniemore-1.0.6.tar", max compression
+gzip compressed data, was "aniemore-1.1.1.tar", max compression
```

## Comparing `aniemore-1.0.6.tar` & `aniemore-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1104 2023-02-10 08:04:39.193324 aniemore-1.0.6/LICENSE
--rw-r--r--   0        0        0     8854 2023-04-04 09:39:53.610124 aniemore-1.0.6/README.md
--rw-r--r--   0        0        0        0 2023-02-10 08:04:39.193598 aniemore-1.0.6/aniemore/__init__.py
--rw-r--r--   0        0        0        0 2023-03-03 13:09:52.775964 aniemore-1.0.6/aniemore/custom/__init__.py
--rw-r--r--   0        0        0     4865 2023-03-07 07:38:22.117377 aniemore-1.0.6/aniemore/custom/models.py
--rw-r--r--   0        0        0      441 2023-03-07 07:38:22.117565 aniemore-1.0.6/aniemore/datasets.py
--rw-r--r--   0        0        0     3215 2023-04-04 09:40:26.813204 aniemore-1.0.6/aniemore/models.py
--rw-r--r--   0        0        0        0 2023-03-07 07:38:22.117862 aniemore-1.0.6/aniemore/recognizers/__init__.py
--rw-r--r--   0        0        0     5243 2023-03-14 09:05:29.768189 aniemore-1.0.6/aniemore/recognizers/text.py
--rw-r--r--   0        0        0     3646 2023-03-14 09:05:29.768541 aniemore-1.0.6/aniemore/recognizers/voice.py
--rw-r--r--   0        0        0        0 2023-02-10 08:04:39.194802 aniemore-1.0.6/aniemore/utils/__init__.py
--rw-r--r--   0        0        0    13560 2023-03-14 09:05:29.768810 aniemore-1.0.6/aniemore/utils/classes.py
--rw-r--r--   0        0        0     2934 2023-03-13 13:22:51.099678 aniemore-1.0.6/aniemore/utils/speech2text.py
--rw-r--r--   0        0        0     2303 2023-04-04 09:41:00.743630 aniemore-1.0.6/pyproject.toml
--rw-r--r--   0        0        0    11130 1970-01-01 00:00:00.000000 aniemore-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-02-19 15:39:16.440064 aniemore-1.1.1/aniemore/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-09 00:36:38.168893 aniemore-1.1.1/aniemore/custom/__init__.py
+-rw-r--r--   0        0        0    19229 2023-04-15 10:55:25.882627 aniemore-1.1.1/aniemore/custom/models.py
+-rw-r--r--   0        0        0      587 2023-04-13 19:34:20.236375 aniemore-1.1.1/aniemore/datasets.py
+-rw-r--r--   0        0        0     4507 2023-04-14 23:20:44.281921 aniemore-1.1.1/aniemore/models.py
+-rw-r--r--   0        0        0        0 2023-03-09 00:36:38.169894 aniemore-1.1.1/aniemore/recognizers/__init__.py
+-rw-r--r--   0        0        0     9924 2023-04-15 01:26:46.065774 aniemore-1.1.1/aniemore/recognizers/multimodal.py
+-rw-r--r--   0        0        0     5641 2023-04-13 23:41:12.889330 aniemore-1.1.1/aniemore/recognizers/text.py
+-rw-r--r--   0        0        0     3981 2023-04-13 23:56:25.137542 aniemore-1.1.1/aniemore/recognizers/voice.py
+-rw-r--r--   0        0        0        0 2023-02-19 15:39:16.444744 aniemore-1.1.1/aniemore/utils/__init__.py
+-rw-r--r--   0        0        0    15860 2023-04-13 21:22:28.319429 aniemore-1.1.1/aniemore/utils/classes.py
+-rw-r--r--   0        0        0     3104 2023-04-12 13:02:56.273113 aniemore-1.1.1/aniemore/utils/speech2text.py
+-rw-r--r--   0        0        0     1125 2023-02-19 15:39:16.439561 aniemore-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2303 2023-04-22 09:56:21.195121 aniemore-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    11294 2023-04-14 10:29:39.799959 aniemore-1.1.1/README.md
+-rw-r--r--   0        0        0    13402 1970-01-01 00:00:00.000000 aniemore-1.1.1/PKG-INFO
```

### Comparing `aniemore-1.0.6/LICENSE` & `aniemore-1.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022  Artem Amentes, Ilya Lubenets, Nikita Davidchuk
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022  Artem Amentes, Ilya Lubenets, Nikita Davidchuk
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `aniemore-1.0.6/README.md` & `aniemore-1.1.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,123 +1,168 @@
-![Aniemore Logo](images/logo.png)
-
- **Aniemore** - это открытая библиотека искусственного интеллекта для потоковой аналитики эмоциональных оттенков речи человека.
-
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1_W2ngr_ShrLdTLVTBP3XF176JW1zdChl)
-
-[![PyPI version](https://img.shields.io/pypi/v/aniemore)](https://img.shields.io/pypi/v/aniemore)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aniemore)](https://img.shields.io/pypi/pyversions/aniemore)
-[![PyPI - Wheel](https://img.shields.io/pypi/wheel/aniemore)](https://img.shields.io/pypi/wheel/aniemore)
-[![PyPI - License](https://img.shields.io/pypi/l/aniemore)](https://img.shields.io/pypi/l/aniemore)
-[![PyPI - Status](https://img.shields.io/pypi/status/aniemore)](https://img.shields.io/pypi/status/aniemore)
-[![Downloads](https://img.shields.io/pypi/dm/aniemore)](https://pypistats.org/packages/aniemore)
-[![CodeQL](https://github.com/aniemore/Aniemore/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/aniemore/Aniemore/actions/workflows/github-code-scanning/codeql)
-[![Bandit](https://github.com/aniemore/Aniemore/actions/workflows/bandit.yml/badge.svg)](https://github.com/aniemore/Aniemore/actions/workflows/bandit.yml)
-
-#### Основные технические параметры
-
-- Объем набора данных Russian Emotional Speech Dialogues содержит более 3000 аудиофрагментов представляющих 200 различных людей;
-- Модели способны распознавать эмоции в зашумленных аудиофайлах длительностью в 3 секунды;
-- Скорость обработки и ответа модели составляет не более 5 секунд;
-- Пословная ошибка модели WER 30%;
-- Совокупная точность модели 75%
-- Диапазон распознавания эмоций: злость, отвращение, страх, счастье, интерес, грусть, нейтрально;
-- Акустические возможности - 3 уровня.
-
-
-## Описание
-Aniemore - это библиотека для Python, которая позволяет добавить в ваше 
-программное обеспечение возможность определять эмоциональный фон речи человека, как в голосе, 
-так и в тексте. Для этого в библиотеке разработано два соответсвующих модуля - Voice и Text.
-
-Aniemore содержит свой собственный датасет RESD (Russian Emotional Speech Dialogues) и другие 
-наборы данных разного объема, которые вы можете использовать для обучения своих моделей.
-
-| Датасет        | Примечание                                                                  |
-|----------------|-----------------------------------------------------------------------------|
-| RESD           | 7 эмоций, 4 часа аудиозаписей диалогов **студийное качество**               |
-| RESD_Annotated | RESD + speech-to-text аннотации                                             |
-| REPV           | 2000 голосовых сообщений (.ogg), 200 актеров, 2 нейтральные фразы, 5 эмоций |
-| REPV-S         | 140 голосовых сообщений (.ogg) "Привет, как дела?" с разными эмоциями       |
-
-Вы можете использовать готовые предобученные модели из библиотеки: 
-
-| Модель                                                                                                                          | Точность |
-|---------------------------------------------------------------------------------------------------------------------------------|----------|
-| Голосовые модели                                                                                                                |          |
-| [**wav2vec2-xlsr-53-russian-emotion-recognition**](https://huggingface.co/Aniemore/wav2vec2-xlsr-53-russian-emotion-recognition) | 73%      |
-| [**wav2vec2-emotion-russian-resd**](https://huggingface.co/Aniemore/wav2vec2-emotion-russian-resd)                              | 75%      |
-| [**wavlm-emotion-russian-resd**](https://huggingface.co/Aniemore/wavlm-emotion-russian-resd)                                    | 82%      |
-| [**hubert-emotion-russian-resd**](https://huggingface.co/Aniemore/hubert-emotion-russian-resd)                                  | 75%      |
-| [**unispeech-sat-emotion-russian-resd Copied**](https://huggingface.co/Aniemore/unispeech-sat-emotion-russian-resd)             | 72%      |
-| Текстовые модели                                                                                                                |          |
-| [**rubert-base-emotion-russian-cedr-m7**](https://huggingface.co/Aniemore/rubert-base-emotion-russian-cedr-m7)                  | 74%      |
-| [**rubert-tiny2-russian-emotion-detection**](https://huggingface.co/Aniemore/rubert-tiny2-russian-emotion-detection)            | 85%      |
-| [**rubert-large-emotion-russian-cedr-m7**](https://huggingface.co/Aniemore/rubert-large-emotion-russian-cedr-m7)                | 76%      |
-| [**rubert-tiny-emotion-russian-cedr-m7**](https://huggingface.co/Aniemore/rubert-tiny-emotion-russian-cedr-m7)                  | 72%      |
-
-#### Показатели моделей в разрезе эмоций
-![показатели моделей.jpg](images/model_sota.jpg)
-
-
-## <a name="Install"></a>	Установка
-```shell
-pip install aniemore
-```
-<hr>
-
-### Пример использования
-
-Ниже приведены простые примеры использования библиотеки. Для более детальных примеров, в том числе **загрузка cобственной модели** - смотрите сделанный для этого *Google Colab*
-
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1_W2ngr_ShrLdTLVTBP3XF176JW1zdChl)
-#### Распознавание эмоций в тексте
-```python
-# @title Text - Recognize: single text - single label
-import torch
-from aniemore.recognizers.text import TextRecognizer
-from aniemore.models import HuggingFaceModel
-
-model=HuggingFaceModel.Text.Bert_Tiny2
-device = 'cuda' if torch.cuda.is_available() else 'cpu'
-tr = TextRecognizer(model=model, device=device)
-
-tr.recognize('это работает? :(', return_single_label=True)
-```
-#### Распознавание эмоций в голосе
-
-```python
-# @title Voice - Recognize: signle audio - single label
-import torch
-from aniemore.recognizers.voice import VoiceRecognizer
-from aniemore.models import HuggingFaceModel
-
-model=HuggingFaceModel.Voice.WavLM
-device = 'cuda' if torch.cuda.is_available() else 'cpu'
-vr = VoiceRecognizer(model=model, device=device)
-vr.recognize('/content/ваш-звуковой-файл.wav', return_single_label=True)
-```
-<hr>
-
-## Доп. ссылки
-
-Все модели и датасеты, а так же примеры их использования вы можете посмотреть в нашем [HuggingFace профиле](https://huggingface.co/Aniemore)
-
-## Аффилированость
-**Aniemore (Artem Nikita Ilya EMOtion REcognition)**
-
-Разработка открытой библиотеки произведена коллективом авторов на базе ООО "Социальный код".
-Результаты работы получены за счет гранта Фонда содействия развитию малых форм предприятий в научно-технической сфере (Договор №1ГУКодИИС12-D7/72697
-от 22.12.2021).
-
-## Цитирование
-```
-@misc{Aniemore,
-  author = {Артем Аментес, Илья Лубенец, Никита Давидчук},
-  title = {Открытая библиотека искусственного интеллекта для анализа и выявления эмоциональных оттенков речи человека},
-  year = {2022},
-  publisher = {GitHub},
-  journal = {GitHub repository},
-  howpublished = {\url{https://github.com/aniemore/Aniemore}},
-  email = {hello@socialcode.ru}
-}
-```
+![Aniemore Logo](images/logo.png)
+
+ **Aniemore** - это открытая библиотека искусственного интеллекта для потоковой аналитики эмоциональных оттенков речи человека.
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1_W2ngr_ShrLdTLVTBP3XF176JW1zdChl)
+
+[![PyPI version](https://img.shields.io/pypi/v/aniemore)](https://img.shields.io/pypi/v/aniemore)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aniemore)](https://img.shields.io/pypi/pyversions/aniemore)
+[![PyPI - Wheel](https://img.shields.io/pypi/wheel/aniemore)](https://img.shields.io/pypi/wheel/aniemore)
+[![PyPI - License](https://img.shields.io/pypi/l/aniemore)](https://img.shields.io/pypi/l/aniemore)
+[![PyPI - Status](https://img.shields.io/pypi/status/aniemore)](https://img.shields.io/pypi/status/aniemore)
+[![Downloads](https://img.shields.io/pypi/dm/aniemore)](https://pypistats.org/packages/aniemore)
+[![CodeQL](https://github.com/aniemore/Aniemore/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/aniemore/Aniemore/actions/workflows/github-code-scanning/codeql)
+[![Bandit](https://github.com/aniemore/Aniemore/actions/workflows/bandit.yml/badge.svg)](https://github.com/aniemore/Aniemore/actions/workflows/bandit.yml)
+
+#### Основные технические параметры
+
+- Объем набора данных Russian Emotional Speech Dialogues содержит более 3000 аудиофрагментов представляющих 200 различных людей;
+- Модели способны распознавать эмоции в зашумленных аудиофайлах длительностью в 3 секунды;
+- Скорость обработки и ответа модели составляет не более 5 секунд;
+- Пословная ошибка модели WER 30%;
+- Совокупная точность модели 75%
+- Диапазон распознавания эмоций: злость, отвращение, страх, счастье, интерес, грусть, нейтрально;
+- Акустические возможности - 3 уровня.
+
+
+## Описание
+Aniemore - это библиотека для Python, которая позволяет добавить в ваше 
+программное обеспечение возможность определять эмоциональный фон речи человека, как в голосе, 
+так и в тексте. Для этого в библиотеке разработано два соответсвующих модуля - Voice и Text.
+
+Aniemore содержит свой собственный датасет RESD (Russian Emotional Speech Dialogues) и другие 
+наборы данных разного объема, которые вы можете использовать для обучения своих моделей.
+
+| Датасет        | Примечание                                                                  |
+|----------------|-----------------------------------------------------------------------------|
+| RESD           | 7 эмоций, 4 часа аудиозаписей диалогов **студийное качество**               |
+| RESD_Annotated | RESD + speech-to-text аннотации                                             |
+| REPV           | 2000 голосовых сообщений (.ogg), 200 актеров, 2 нейтральные фразы, 5 эмоций |
+| REPV-S         | 140 голосовых сообщений (.ogg) "Привет, как дела?" с разными эмоциями       |
+
+Вы можете использовать готовые предобученные модели из библиотеки: 
+
+| Модель                                                                                                                            | Точность |
+|-----------------------------------------------------------------------------------------------------------------------------------|----------|
+| Голосовые модели                                                                                                                  |          |
+| [**wav2vec2-xlsr-53-russian-emotion-recognition**](https://huggingface.co/Aniemore/wav2vec2-xlsr-53-russian-emotion-recognition)  | 73%      |
+| [**wav2vec2-emotion-russian-resd**](https://huggingface.co/Aniemore/wav2vec2-emotion-russian-resd)                                | 75%      |
+| [**wavlm-emotion-russian-resd**](https://huggingface.co/Aniemore/wavlm-emotion-russian-resd)                                      | 82%      |
+| [**hubert-emotion-russian-resd**](https://huggingface.co/Aniemore/hubert-emotion-russian-resd)                                    | 75%      |
+| [**unispeech-sat-emotion-russian-resd Copied**](https://huggingface.co/Aniemore/unispeech-sat-emotion-russian-resd)               | 72%      |
+| Текстовые модели                                                                                                                  |          |
+| [**rubert-base-emotion-russian-cedr-m7**](https://huggingface.co/Aniemore/rubert-base-emotion-russian-cedr-m7)                    | 74%      |
+| [**rubert-tiny2-russian-emotion-detection**](https://huggingface.co/Aniemore/rubert-tiny2-russian-emotion-detection)              | 85%      |
+| [**rubert-large-emotion-russian-cedr-m7**](https://huggingface.co/Aniemore/rubert-large-emotion-russian-cedr-m7)                  | 76%      |
+| [**rubert-tiny-emotion-russian-cedr-m7**](https://huggingface.co/Aniemore/rubert-tiny-emotion-russian-cedr-m7)                    | 72%      |
+
+#### Показатели моделей в разрезе эмоций
+![показатели моделей.jpg](images/model_sota.jpg)
+
+
+## <a name="Install"></a>	Установка
+```shell
+pip install aniemore
+```
+## <a name="Install"></a>	Минимальные требования к оборудованию
+
+| Архитектура              | ЦПУ      | ОЗУ   | SSD   |
+|--------------------------|----------|-------|-------|
+| **Wave2Vec2**            | 2 ядра   | 8 ГБ  | 40 ГБ |
+| **WaveLM**               | 2 ядра   | 8 ГБ  | 40 ГБ |
+| **Hubert**               | 2 ядра   | 8 ГБ  | 40 ГБ |
+| **UniSpeechSAT**         | 2 ядра   | 8 ГБ  | 40 ГБ |
+| **Bert_Tiny/Bert_Tiny2** | 2 ядра   | 4 ГБ  | 40 ГБ |
+| **Bert_Base**            | 2 ядра   | 4 ГБ  | 40 ГБ |
+| **Bert_Large**           | 2 ядра   | 8 ГБ  | 40 ГБ |
+| **Whisper Tiny**         | 2 ядра   | 4 ГБ  | 40 ГБ |
+| **Whisper Base**         | 2 ядра   | 4 ГБ  | 40 ГБ |
+| **Whisper Small**        | 2 ядра   | 4 ГБ  | 40 ГБ |
+| **Whisper Medium**       | 2 ядра   | 8 ГБ  | 40 ГБ |
+| **Whisper Large**        | 2 ядра   | 16 ГБ | 40 ГБ |
+| **TextEnhancer**         | 2 ядра   | 4 ГБ  | 40 ГБ |
+<hr>
+
+### Пример использования
+
+Ниже приведены простые примеры использования библиотеки. Для более детальных примеров, в том числе **загрузка cобственной модели** - смотрите сделанный для этого *Google Colab*
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1_W2ngr_ShrLdTLVTBP3XF176JW1zdChl)
+#### Распознавание эмоций в тексте
+```python
+import torch
+from aniemore.recognizers.text import TextRecognizer
+from aniemore.models import HuggingFaceModel
+
+model = HuggingFaceModel.Text.Bert_Tiny2
+device = 'cuda' if torch.cuda.is_available() else 'cpu'
+tr = TextRecognizer(model=model, device=device)
+
+tr.recognize('это работает? :(', return_single_label=True)
+```
+#### Распознавание эмоций в голосе
+
+```python
+import torch
+from aniemore.recognizers.voice import VoiceRecognizer
+from aniemore.models import HuggingFaceModel
+
+model = HuggingFaceModel.Voice.WavLM
+device = 'cuda' if torch.cuda.is_available() else 'cpu'
+vr = VoiceRecognizer(model=model, device=device)
+vr.recognize('/content/ваш-звуковой-файл.wav', return_single_label=True)
+```
+#### Распознавание эмоций (мультимодальный метод)
+
+```python
+import torch
+from aniemore.recognizers.multimodal import VoiceTextRecognizer
+from aniemore.utils.speech2text import SmallSpeech2Text
+from aniemore.models import HuggingFaceModel
+
+model = HuggingFaceModel.MultiModal.WavLMBertBase
+s2t_model = SmallSpeech2Text()
+
+text = SmallSpeech2Text.recognize('/content/ваш-звуковой-файл.wav').text
+device = 'cuda' if torch.cuda.is_available() else 'cpu'
+
+vtr = VoiceTextRecognizer(model=model, device=device)
+vtr.recognize(('/content/ваш-звуковой-файл.wav', text), return_single_label=True)
+```
+#### Распознавание эмоций (мультимодальный метод с автоматическим распознаванием речи)
+
+```python
+import torch
+from aniemore.recognizers.multimodal import MultiModalRecognizer
+from aniemore.utils.speech2text import SmallSpeech2Text
+from aniemore.models import HuggingFaceModel
+
+model = HuggingFaceModel.MultiModal.WavLMBertBase
+device = 'cuda' if torch.cuda.is_available() else 'cpu'
+mr = MultiModalRecognizer(model=model, s2t_model=SmallSpeech2Text(), device=device)
+mr.recognize('/content/ваш-звуковой-файл.wav', return_single_label=True)
+```
+<hr>
+
+## Доп. ссылки
+
+Все модели и датасеты, а так же примеры их использования вы можете посмотреть в нашем [HuggingFace профиле](https://huggingface.co/Aniemore)
+
+## Аффилированость
+**Aniemore (Artem Nikita Ilya EMOtion REcognition)**
+
+Разработка открытой библиотеки произведена коллективом авторов на базе ООО "Социальный код".
+Результаты работы получены за счет гранта Фонда содействия развитию малых форм предприятий в научно-технической сфере (Договор №1ГУКодИИС12-D7/72697
+от 22.12.2021).
+
+## Цитирование
+```
+@misc{Aniemore,
+  author = {Артем Аментес, Илья Лубенец, Никита Давидчук},
+  title = {Открытая библиотека искусственного интеллекта для анализа и выявления эмоциональных оттенков речи человека},
+  year = {2022},
+  publisher = {GitHub},
+  journal = {GitHub repository},
+  howpublished = {\url{https://github.com/aniemore/Aniemore}},
+  email = {hello@socialcode.ru}
+}
+```
```

### Comparing `aniemore-1.0.6/aniemore/recognizers/voice.py` & `aniemore-1.1.1/aniemore/recognizers/voice.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,120 +1,127 @@
-from typing import Union, List
-import numpy
-import torch
-import torchaudio
-
-from aniemore.utils.classes import (
-    BaseRecognizer,
-    RecognizerOutputOne,
-    RecognizerOutputMany,
-)
-
-
-# noinspection PyUnresolvedReferences
-class VoiceRecognizer(BaseRecognizer):
-    @classmethod
-    def speech_file_to_array_fn(cls, path):
-        """Загружаем аудиофайл в массив
-
-        Args:
-          path: путь к файлу
-
-        Returns:
-          numpy.ndarray
-
-        """
-        speech_array, _sampling_rate = torchaudio.load(path)
-        resampler = torchaudio.transforms.Resample(_sampling_rate)
-        speech = resampler(speech_array).squeeze().numpy()
-        return speech
-
-    def _get_torch_scores(self, speech: Union[List[torch.Tensor], torch.Tensor, numpy.ndarray]) -> torch.Tensor:
-        """Получаем выход модели
-
-        Args:
-          speech: ndarray
-
-        Returns:
-          torch.Tensor
-
-        """
-        sampling_rate = self.feature_extractor.sampling_rate
-        inputs = self.feature_extractor(speech, sampling_rate=sampling_rate, return_tensors="pt", padding=True)
-        inputs = {key: inputs[key].to(self._model.device) for key in inputs}
-
-        with torch.no_grad():
-            logits = self._model(**inputs).logits
-
-        # move inputs to cpu back
-        for key in inputs:
-            inputs[key] = inputs[key].cpu()
-
-        del inputs
-
-        scores = torch.softmax(logits, dim=1)
-        return scores
-
-    def _recognize_one(self, path: str) -> RecognizerOutputOne:
-        """Исполнение рантайма для одного файла
-
-        Args:
-          path: путь к файлу
-
-        Returns:
-          RecognizerOutputOne
-
-        """
-        speech = self.speech_file_to_array_fn(path)
-        scores = self._get_torch_scores(speech)
-
-        scores = {k: v for k, v in zip(self.config.id2label.values(), scores[0].tolist())}
-
-        return RecognizerOutputOne(**scores)
-
-    def _recognize_many(self, paths: List[str]) -> RecognizerOutputMany:
-        """Прогнозируем несколько файлов
-
-        Args:
-          paths: список путей к файлам
-
-        Returns:
-          словарь с выходами модели
-
-        """
-        speeches = []
-        for path in paths:
-            speech = self.speech_file_to_array_fn(path)
-            speeches.append(speech)
-        scores: torch.Tensor = self._get_torch_scores(speeches)
-        results: RecognizerOutputMany = self._get_many_results(paths, scores)
-        return results
-
-    # TODO: add single_label option
-
-    def recognize(self, paths: Union[List[str], str], return_single_label: bool = False) -> \
-            Union[RecognizerOutputOne, RecognizerOutputMany]:
-        """Прогнозируем файлы
-
-        Args:
-          paths: путь к файлу или список путей к файлам
-          return_single_label: если True, то возвращаем только один лейбл
-
-        Returns:
-          выход модели
-
-        """
-        if self._model is None:
-            self._setup_variables()
-
-        if isinstance(paths, str):
-            if return_single_label:
-                return self._get_single_label(self._recognize_one(paths))
-            return self._recognize_one(paths)
-
-        elif isinstance(paths, list):
-            if return_single_label:
-                return self._get_single_label(self._recognize_many(paths))
-            return self._recognize_many(paths)
-
-        else:
-            raise ValueError('paths must be str or list')
+from typing import Union, List
+import numpy
+import torch
+import torchaudio
+
+from aniemore.utils.classes import (
+    BaseRecognizer,
+    RecognizerOutputOne,
+    RecognizerOutputMany,
+)
+
+
+class VoiceRecognizer(BaseRecognizer):
+    @classmethod
+    def speech_file_to_array_fn(cls, path):
+        """Загружаем аудиофайл в массив
+
+        Args:
+          path: путь к файлу
+
+        Returns:
+          numpy.ndarray
+
+        """
+        speech_array, _sampling_rate = torchaudio.load(path)
+        resampler = torchaudio.transforms.Resample(_sampling_rate)
+        speech = resampler(speech_array).squeeze().numpy()
+        return speech
+
+    def _get_torch_scores(self, speech: Union[List[torch.Tensor], torch.Tensor, numpy.ndarray]) -> torch.Tensor:
+        """Получаем выход модели
+
+        Args:
+          speech: ndarray
+
+        Returns:
+          torch.Tensor
+
+        """
+        sampling_rate = self.feature_extractor.sampling_rate
+        inputs = self.feature_extractor(speech, sampling_rate=sampling_rate, return_tensors="pt", padding=True)
+        inputs = {key: inputs[key].to(self._model.device) for key in inputs}
+
+        with torch.no_grad():
+            logits = self._model(**inputs).logits
+
+        # move inputs to cpu back
+        for key in inputs:
+            inputs[key] = inputs[key].cpu()
+
+        del inputs
+
+        if self._logistic_fct is torch.sigmoid:
+            scores = self._logistic_fct(logits)
+        elif self._logistic_fct is torch.softmax:
+            scores = self._logistic_fct(logits, dim=1)
+        else:
+            raise ValueError('logistic_fct must be torch.sigmoid or torch.softmax')
+
+        return scores
+
+    def _recognize_one(self, path: str) -> RecognizerOutputOne:
+        """Исполнение рантайма для одного файла
+
+        Args:
+          path: путь к файлу
+
+        Returns:
+          RecognizerOutputOne
+
+        """
+        speech = self.speech_file_to_array_fn(path)
+        scores = self._get_torch_scores(speech)
+
+        scores = {k: v for k, v in zip(self.config.id2label.values(), scores[0].tolist())}
+
+        return RecognizerOutputOne(**scores)
+
+    def _recognize_many(self, paths: List[str]) -> RecognizerOutputMany:
+        """Прогнозируем несколько файлов
+
+        Args:
+          paths: список путей к файлам
+
+        Returns:
+          словарь с выходами модели
+
+        """
+        speeches = []
+        for path in paths:
+            speech = self.speech_file_to_array_fn(path)
+            speeches.append(speech)
+        scores: torch.Tensor = self._get_torch_scores(speeches)
+        results: RecognizerOutputMany = self._get_many_results(paths, scores)
+
+        return results
+
+    def recognize(
+            self,
+            paths: Union[List[str], str],
+            return_single_label: bool = False
+    ) -> Union[RecognizerOutputOne, RecognizerOutputMany]:
+        """Прогнозируем файлы
+
+        Args:
+          paths: путь к файлу или список путей к файлам
+          return_single_label: если True, то возвращаем только один лейбл
+
+        Returns:
+          выход модели
+
+        """
+        if self._model is None:
+            self._setup_variables()
+
+        if isinstance(paths, str):
+            if return_single_label:
+                return self._get_single_label(self._recognize_one(paths))
+            return self._recognize_one(paths)
+
+        elif isinstance(paths, list):
+            if return_single_label:
+                return self._get_single_label(self._recognize_many(paths))
+            return self._recognize_many(paths)
+
+        else:
+            raise ValueError('paths must be str or list')
```

### Comparing `aniemore-1.0.6/pyproject.toml` & `aniemore-1.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "aniemore"
-version = "1.0.6"
+version = "1.1.1"
 authors = [
     "Ilya Lubenets <lii291001@gmail.com>",
     "Nikita Davidchuk <ar4ikov228@gmail.com>",
     "Artem Amentes <artem@socialcode.ru>",
 ]
 maintainers = [
     "Ilya Lubenets <lii291001@gmail.com>",
```

### Comparing `aniemore-1.0.6/PKG-INFO` & `aniemore-1.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aniemore
-Version: 1.0.6
+Version: 1.1.1
 Summary: Aniemore (Artem Nikita Ilya EMOtion REcognition) is a library for emotion recognition in voice and text for russian language.
 License: MIT
 Author: Ilya Lubenets
 Author-email: lii291001@gmail.com
 Maintainer: Ilya Lubenets
 Maintainer-email: lii291001@gmail.com
 Requires-Python: >=3.8,<3.12
@@ -85,69 +85,114 @@
 | RESD           | 7 эмоций, 4 часа аудиозаписей диалогов **студийное качество**               |
 | RESD_Annotated | RESD + speech-to-text аннотации                                             |
 | REPV           | 2000 голосовых сообщений (.ogg), 200 актеров, 2 нейтральные фразы, 5 эмоций |
 | REPV-S         | 140 голосовых сообщений (.ogg) "Привет, как дела?" с разными эмоциями       |
 
 Вы можете использовать готовые предобученные модели из библиотеки: 
 
-| Модель                                                                                                                          | Точность |
-|---------------------------------------------------------------------------------------------------------------------------------|----------|
-| Голосовые модели                                                                                                                |          |
-| [**wav2vec2-xlsr-53-russian-emotion-recognition**](https://huggingface.co/Aniemore/wav2vec2-xlsr-53-russian-emotion-recognition) | 73%      |
-| [**wav2vec2-emotion-russian-resd**](https://huggingface.co/Aniemore/wav2vec2-emotion-russian-resd)                              | 75%      |
-| [**wavlm-emotion-russian-resd**](https://huggingface.co/Aniemore/wavlm-emotion-russian-resd)                                    | 82%      |
-| [**hubert-emotion-russian-resd**](https://huggingface.co/Aniemore/hubert-emotion-russian-resd)                                  | 75%      |
-| [**unispeech-sat-emotion-russian-resd Copied**](https://huggingface.co/Aniemore/unispeech-sat-emotion-russian-resd)             | 72%      |
-| Текстовые модели                                                                                                                |          |
-| [**rubert-base-emotion-russian-cedr-m7**](https://huggingface.co/Aniemore/rubert-base-emotion-russian-cedr-m7)                  | 74%      |
-| [**rubert-tiny2-russian-emotion-detection**](https://huggingface.co/Aniemore/rubert-tiny2-russian-emotion-detection)            | 85%      |
-| [**rubert-large-emotion-russian-cedr-m7**](https://huggingface.co/Aniemore/rubert-large-emotion-russian-cedr-m7)                | 76%      |
-| [**rubert-tiny-emotion-russian-cedr-m7**](https://huggingface.co/Aniemore/rubert-tiny-emotion-russian-cedr-m7)                  | 72%      |
+| Модель                                                                                                                            | Точность |
+|-----------------------------------------------------------------------------------------------------------------------------------|----------|
+| Голосовые модели                                                                                                                  |          |
+| [**wav2vec2-xlsr-53-russian-emotion-recognition**](https://huggingface.co/Aniemore/wav2vec2-xlsr-53-russian-emotion-recognition)  | 73%      |
+| [**wav2vec2-emotion-russian-resd**](https://huggingface.co/Aniemore/wav2vec2-emotion-russian-resd)                                | 75%      |
+| [**wavlm-emotion-russian-resd**](https://huggingface.co/Aniemore/wavlm-emotion-russian-resd)                                      | 82%      |
+| [**hubert-emotion-russian-resd**](https://huggingface.co/Aniemore/hubert-emotion-russian-resd)                                    | 75%      |
+| [**unispeech-sat-emotion-russian-resd Copied**](https://huggingface.co/Aniemore/unispeech-sat-emotion-russian-resd)               | 72%      |
+| Текстовые модели                                                                                                                  |          |
+| [**rubert-base-emotion-russian-cedr-m7**](https://huggingface.co/Aniemore/rubert-base-emotion-russian-cedr-m7)                    | 74%      |
+| [**rubert-tiny2-russian-emotion-detection**](https://huggingface.co/Aniemore/rubert-tiny2-russian-emotion-detection)              | 85%      |
+| [**rubert-large-emotion-russian-cedr-m7**](https://huggingface.co/Aniemore/rubert-large-emotion-russian-cedr-m7)                  | 76%      |
+| [**rubert-tiny-emotion-russian-cedr-m7**](https://huggingface.co/Aniemore/rubert-tiny-emotion-russian-cedr-m7)                    | 72%      |
 
 #### Показатели моделей в разрезе эмоций
 ![показатели моделей.jpg](images/model_sota.jpg)
 
 
 ## <a name="Install"></a>	Установка
 ```shell
 pip install aniemore
 ```
+## <a name="Install"></a>	Минимальные требования к оборудованию
+
+| Архитектура              | ЦПУ      | ОЗУ   | SSD   |
+|--------------------------|----------|-------|-------|
+| **Wave2Vec2**            | 2 ядра   | 8 ГБ  | 40 ГБ |
+| **WaveLM**               | 2 ядра   | 8 ГБ  | 40 ГБ |
+| **Hubert**               | 2 ядра   | 8 ГБ  | 40 ГБ |
+| **UniSpeechSAT**         | 2 ядра   | 8 ГБ  | 40 ГБ |
+| **Bert_Tiny/Bert_Tiny2** | 2 ядра   | 4 ГБ  | 40 ГБ |
+| **Bert_Base**            | 2 ядра   | 4 ГБ  | 40 ГБ |
+| **Bert_Large**           | 2 ядра   | 8 ГБ  | 40 ГБ |
+| **Whisper Tiny**         | 2 ядра   | 4 ГБ  | 40 ГБ |
+| **Whisper Base**         | 2 ядра   | 4 ГБ  | 40 ГБ |
+| **Whisper Small**        | 2 ядра   | 4 ГБ  | 40 ГБ |
+| **Whisper Medium**       | 2 ядра   | 8 ГБ  | 40 ГБ |
+| **Whisper Large**        | 2 ядра   | 16 ГБ | 40 ГБ |
+| **TextEnhancer**         | 2 ядра   | 4 ГБ  | 40 ГБ |
 <hr>
 
 ### Пример использования
 
 Ниже приведены простые примеры использования библиотеки. Для более детальных примеров, в том числе **загрузка cобственной модели** - смотрите сделанный для этого *Google Colab*
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1_W2ngr_ShrLdTLVTBP3XF176JW1zdChl)
 #### Распознавание эмоций в тексте
 ```python
-# @title Text - Recognize: single text - single label
 import torch
 from aniemore.recognizers.text import TextRecognizer
 from aniemore.models import HuggingFaceModel
 
-model=HuggingFaceModel.Text.Bert_Tiny2
+model = HuggingFaceModel.Text.Bert_Tiny2
 device = 'cuda' if torch.cuda.is_available() else 'cpu'
 tr = TextRecognizer(model=model, device=device)
 
 tr.recognize('это работает? :(', return_single_label=True)
 ```
 #### Распознавание эмоций в голосе
 
 ```python
-# @title Voice - Recognize: signle audio - single label
 import torch
 from aniemore.recognizers.voice import VoiceRecognizer
 from aniemore.models import HuggingFaceModel
 
-model=HuggingFaceModel.Voice.WavLM
+model = HuggingFaceModel.Voice.WavLM
 device = 'cuda' if torch.cuda.is_available() else 'cpu'
 vr = VoiceRecognizer(model=model, device=device)
 vr.recognize('/content/ваш-звуковой-файл.wav', return_single_label=True)
 ```
+#### Распознавание эмоций (мультимодальный метод)
+
+```python
+import torch
+from aniemore.recognizers.multimodal import VoiceTextRecognizer
+from aniemore.utils.speech2text import SmallSpeech2Text
+from aniemore.models import HuggingFaceModel
+
+model = HuggingFaceModel.MultiModal.WavLMBertBase
+s2t_model = SmallSpeech2Text()
+
+text = SmallSpeech2Text.recognize('/content/ваш-звуковой-файл.wav').text
+device = 'cuda' if torch.cuda.is_available() else 'cpu'
+
+vtr = VoiceTextRecognizer(model=model, device=device)
+vtr.recognize(('/content/ваш-звуковой-файл.wav', text), return_single_label=True)
+```
+#### Распознавание эмоций (мультимодальный метод с автоматическим распознаванием речи)
+
+```python
+import torch
+from aniemore.recognizers.multimodal import MultiModalRecognizer
+from aniemore.utils.speech2text import SmallSpeech2Text
+from aniemore.models import HuggingFaceModel
+
+model = HuggingFaceModel.MultiModal.WavLMBertBase
+device = 'cuda' if torch.cuda.is_available() else 'cpu'
+mr = MultiModalRecognizer(model=model, s2t_model=SmallSpeech2Text(), device=device)
+mr.recognize('/content/ваш-звуковой-файл.wav', return_single_label=True)
+```
 <hr>
 
 ## Доп. ссылки
 
 Все модели и датасеты, а так же примеры их использования вы можете посмотреть в нашем [HuggingFace профиле](https://huggingface.co/Aniemore)
 
 ## Аффилированость
```

