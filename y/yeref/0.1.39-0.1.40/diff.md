# Comparing `tmp/yeref-0.1.39.tar.gz` & `tmp/yeref-0.1.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.39.tar", last modified: Sat Apr 22 08:27:11 2023, max compression
+gzip compressed data, was "yeref-0.1.40.tar", last modified: Sat Apr 22 08:45:55 2023, max compression
```

## Comparing `yeref-0.1.39.tar` & `yeref-0.1.40.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-22 08:27:11.500607 yeref-0.1.39/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-22 08:27:11.500845 yeref-0.1.39/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-22 08:27:11.501542 yeref-0.1.39/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1154 2023-04-22 08:26:45.000000 yeref-0.1.39/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-22 08:27:11.493188 yeref-0.1.39/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.39/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)    47105 2023-04-22 08:13:01.000000 yeref-0.1.39/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   205201 2023-04-22 08:26:22.000000 yeref-0.1.39/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-22 08:27:11.499231 yeref-0.1.39/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-22 08:27:11.000000 yeref-0.1.39/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-04-22 08:27:11.000000 yeref-0.1.39/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-22 08:27:11.000000 yeref-0.1.39/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-04-22 08:27:11.000000 yeref-0.1.39/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-22 08:45:55.764639 yeref-0.1.40/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-22 08:45:55.764877 yeref-0.1.40/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-22 08:45:55.765781 yeref-0.1.40/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1154 2023-04-22 08:41:08.000000 yeref-0.1.40/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-22 08:45:55.758082 yeref-0.1.40/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.40/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)    53630 2023-04-22 08:39:39.000000 yeref-0.1.40/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   205201 2023-04-22 08:26:22.000000 yeref-0.1.40/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-22 08:45:55.763940 yeref-0.1.40/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-22 08:45:55.000000 yeref-0.1.40/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-04-22 08:45:55.000000 yeref-0.1.40/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-22 08:45:55.000000 yeref-0.1.40/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-04-22 08:45:55.000000 yeref-0.1.40/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.39/setup.py` & `yeref-0.1.40/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.39',
+      version='0.1.40',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -39,10 +39,10 @@
 # python setup.py bdist_wheel
 # endregion
 
 # python -m build
 
 # twine upload dist/*
 
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.37-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.40-py3-none-any.whl
 
 # python3 -m pip install --upgrade yeref
```

### Comparing `yeref-0.1.39/yeref/l_.py` & `yeref-0.1.40/yeref/l_.py`

 * *Files 6% similar despite different names*

```diff
@@ -330,14 +330,122 @@
     'fr': '👩🏽‍💻 <b>Aio/pyro-gram developer</b>\n\nTasks: dev and support all projects\nGender: girl\nAge: less than 30\nPay: share of the company',
     'zh':'👩🏽‍💻 <b>Aio/pyro-gram developer</b>\n\nTasks: dev and support all projects\nGender: girl\nAge: less than 30\nPay: share of the company',
     'ar': '👩🏽‍💻 <b>Aio/pyro-gram developer</b>\n\nTasks: dev and support all projects\nGender: girl\nAge: less than 30\nPay: share of the company',
 }
 # endregion
 
 
+# region FereyAIBot
+l_ai_btn1 = {
+    'ru': '⛰️ Вакансии',
+    'en': '⛰️ Projects',
+    'es': '⛰️ Projects',
+    'fr': '⛰️ Projects',
+    'zh': '⛰️ 團體',
+    'ar': '⛰️ مجموعات',
+}
+l_ai_btn2 = {
+    'ru': '🌬 Подписка',
+    'en': '🌬 Subcribe',
+    'es': '🌬 Sobre',
+    'fr': '🌬 À propos de',
+    'zh': '🌬 關於',
+    'ar': '🌬 حول',
+}
+l_ai_welcome = {
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>проекта</code> <b>Ferey</b>:\n\n▪️<b>вакансии</b> нашего стартапа\n▪️конкурсы и <b>мероприятия</b>\n\n❗️также можно заказать разработку чат-бота в нашей студии <a href='https://t.me/{1}'>Ferey</a>",
+    'en': "🌱 {0}, welcome to <i>landing-bot</i> for <code>administration</code> <b>Telegram</b>-channels:\n\n▪️<b>pretecting</b> channel from spy-joining of\n▪️store offers in <b>unique</b> space\n▪️defend offers form <b>auto</b> deleted* \n(*even it has stop-words)\n\n❗️to order chat-bot-development go to <a href='https://t.me/{1}'>Ferey</a>-studio",
+    'es': "🌱 {0}, Bienvenida(o) a <i>lugar de aterrizaje-bot</i> por <code>creando & publicando</code> <b>Telegram</b>-Grupos:\n\n▪️️crear <b>cualquier</b> tipo de oferta (con botones)\n▪️almacenar ofertas en un espacio <b>único</b>\n▪️️defend ofrece formulario <b>auto</b> borrado* \n(*incluso tiene palabras vacías)\n\n❗️para ordenar chat-bot-desarrollo vaya a <a href='https://t.me/{1}'>Ferey</a>-estudio",
+    'fr': "🌱 {0}, bienvenue sur <i>landing-bot</i> pour la <code>création et publication</code> <b>Télégramme</b>-channeles:\n\n▪️créer <b>tout </b> type d'offre (avec boutons)\n▪️stocker les offres dans un espace <b>unique</b>\n▪️défendre les offres sous forme <b>auto</b> supprimées* \n(*même si elles ont cessé -words)\n\n❗️pour commander le développement de chat-bot, rendez-vous sur <a href='https://t.me/{1}'>Ferey</a>-studio",
+    'zh': "🌱 {0}, 歡迎來到 <i>著陸點-bot</i> 為了 <code>創造 & 張貼</code> <b>Telegram</b>-團體:\n\n▪️️創造 <b>任何</b> 報價類型 (帶按鈕)\n▪️商店優惠在 <b>獨特的</b> 獨特的\n▪️捍衛報價表格自動刪除* \n(*捍衛自動刪除的提議)\n\n❗️訂購 Telegram-bot 去 <a href='https://t.me/{1}'>Ferey</a>-工作室",
+    'ar': "🌱 {0} ، مرحبًا بك في <i> برنامج التتبع </i> من أجل الإنشاء والنش Telegram - مجموعات: \n\n▪️ إنشاء <b> أي </b> نوع العرض (مع الأزرار) \n▪️ عروض المتجر في مساحة فريدة \n▪️ الدفاع عن نموذج عروض <b> تلقائي </b> محذوفة * \n (* حتى إذا توقفت -كلمات) \n\n لطلب تطوير chat-bot-انتقل إلى <a href='https://t.me/{1}'>Ferey</a>-studio"
+}
+l_gen_txt = {
+    'ru': "📘 Текст{0}",
+    'en': '👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+l_gen_img = {
+    'ru': "🌌 Образ",
+    'en': '👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+l_gen_tlg = {
+    'ru': "👩🏽‍💻 Анализ Telegram-канала",
+    'en': '👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+l_generate_main = {
+    'ru': '👩🏽‍💻 <b>Выбери режим</b>',
+    'en': '👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+l_generate_prompt = {
+    'ru': '👩🏽‍💻 <b>Введи</b> запрос для <b>{0}</b> 👇🏼..',
+    'en': '👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+l_generate_chn = {
+    'ru': '👩🏽‍💻 <b>Вставь</b> ссылку на Telegram канал для анализа финансовых показателей',
+    'en': '👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+l_generate_wait = {
+    'ru': '👩🏽‍💻 <b>Дождитесь</b> окончания генерации..',
+    'en': '👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+l_generate_subcribe = {
+    'ru': '👩🏽‍💻 Подождите {0}сек или оформите подписку',
+    'en': '👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+l_generate_error = {
+    'ru': '👩🏽‍💻 <b>Ошибка</b> генерации',
+    'en': '👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+l_generate_errchn = {
+    'ru': '👩🏽‍💻 <b>Ошибка</b> доступа к каналу (попробуйте позже или сделайте канал публичным)',
+    'en': '👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+# endregion
+
+
 # region post
 l_post_text = {
     'ru': "✏️ 1. Напиши мне <b>текст</b> для нового поста (не забудь использовать <i>форматирование</i>)\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
     'en': "✏️ 1. Send me <b>text</b> for new post for (don't forget to use <i>formatting</i>)\n\n(<i>or click the «➡️️/Next» to skip this step</i>)",
     'es': "✏️ 1. Envíame <b>texto</b> para una nueva publicación (no olvides usar <i>formato</i>)\n\n(<i>o haz clic en «➡️️ /Next» para omitir este paso</i>)",
     'fr': "✏️ 1. Envoyez-moi un <b>texte</b> pour un nouveau message (n'oubliez pas d'utiliser le <i>formatage</i>)\n\n(<i>ou cliquez sur le «➡️️ /Next» pour ignorer cette étape</i>)",
     'zh': "✏️ 1. 給我 <b>文本</b> 對於新職位 (不要忘記使用 <i>格式化</i>)\n\n(<i>或單擊 «➡️️/Next» 跳過這一步</i>)",
```

### Comparing `yeref-0.1.39/yeref/yeref.py` & `yeref-0.1.40/yeref/yeref.py`

 * *Files identical despite different names*

