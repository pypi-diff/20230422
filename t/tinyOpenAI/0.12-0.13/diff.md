# Comparing `tmp/tinyOpenAI-0.12.tar.gz` & `tmp/tinyOpenAI-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyOpenAI-0.12.tar", last modified: Wed Mar 22 14:27:51 2023, max compression
+gzip compressed data, was "tinyOpenAI-0.13.tar", last modified: Sat Apr 22 14:42:23 2023, max compression
```

## Comparing `tinyOpenAI-0.12.tar` & `tinyOpenAI-0.13.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 laicj      (501) staff       (20)        0 2023-03-22 14:27:51.715571 tinyOpenAI-0.12/
--rw-r--r--   0 laicj      (501) staff       (20)     1130 2023-03-07 08:54:32.000000 tinyOpenAI-0.12/LICENSE
--rw-r--r--   0 laicj      (501) staff       (20)     8074 2023-03-22 14:27:51.715443 tinyOpenAI-0.12/PKG-INFO
--rw-r--r--   0 laicj      (501) staff       (20)       38 2023-03-22 14:27:51.715607 tinyOpenAI-0.12/setup.cfg
--rw-r--r--   0 laicj      (501) staff       (20)      791 2023-03-22 14:17:09.000000 tinyOpenAI-0.12/setup.py
-drwxr-xr-x   0 laicj      (501) staff       (20)        0 2023-03-22 14:27:51.714589 tinyOpenAI-0.12/tinyOpenAI/
--rw-r--r--   0 laicj      (501) staff       (20)       96 2023-03-22 14:17:40.000000 tinyOpenAI-0.12/tinyOpenAI/__init__.py
--rw-r--r--   0 laicj      (501) staff       (20)     7046 2023-03-22 13:58:51.000000 tinyOpenAI-0.12/tinyOpenAI/tinyOpenAI.py
-drwxr-xr-x   0 laicj      (501) staff       (20)        0 2023-03-22 14:27:51.715294 tinyOpenAI-0.12/tinyOpenAI.egg-info/
--rw-r--r--   0 laicj      (501) staff       (20)     8074 2023-03-22 14:27:51.000000 tinyOpenAI-0.12/tinyOpenAI.egg-info/PKG-INFO
--rw-r--r--   0 laicj      (501) staff       (20)      270 2023-03-22 14:27:51.000000 tinyOpenAI-0.12/tinyOpenAI.egg-info/SOURCES.txt
--rw-r--r--   0 laicj      (501) staff       (20)        1 2023-03-22 14:27:51.000000 tinyOpenAI-0.12/tinyOpenAI.egg-info/dependency_links.txt
--rw-r--r--   0 laicj      (501) staff       (20)       53 2023-03-22 14:27:51.000000 tinyOpenAI-0.12/tinyOpenAI.egg-info/entry_points.txt
--rw-r--r--   0 laicj      (501) staff       (20)        9 2023-03-22 14:27:51.000000 tinyOpenAI-0.12/tinyOpenAI.egg-info/requires.txt
--rw-r--r--   0 laicj      (501) staff       (20)       11 2023-03-22 14:27:51.000000 tinyOpenAI-0.12/tinyOpenAI.egg-info/top_level.txt
+drwxr-xr-x   0 laicj      (501) staff       (20)        0 2023-04-22 14:42:23.456194 tinyOpenAI-0.13/
+-rw-r--r--   0 laicj      (501) staff       (20)     1130 2023-03-07 08:54:32.000000 tinyOpenAI-0.13/LICENSE
+-rw-r--r--   0 laicj      (501) staff       (20)     8788 2023-04-22 14:42:23.456054 tinyOpenAI-0.13/PKG-INFO
+-rw-r--r--   0 laicj      (501) staff       (20)       38 2023-04-22 14:42:23.456233 tinyOpenAI-0.13/setup.cfg
+-rw-r--r--   0 laicj      (501) staff       (20)      791 2023-04-22 14:39:42.000000 tinyOpenAI-0.13/setup.py
+drwxr-xr-x   0 laicj      (501) staff       (20)        0 2023-04-22 14:42:23.455234 tinyOpenAI-0.13/tinyOpenAI/
+-rw-r--r--   0 laicj      (501) staff       (20)       96 2023-03-22 14:17:40.000000 tinyOpenAI-0.13/tinyOpenAI/__init__.py
+-rw-r--r--   0 laicj      (501) staff       (20)     8185 2023-04-22 13:57:16.000000 tinyOpenAI-0.13/tinyOpenAI/tinyOpenAI.py
+drwxr-xr-x   0 laicj      (501) staff       (20)        0 2023-04-22 14:42:23.455874 tinyOpenAI-0.13/tinyOpenAI.egg-info/
+-rw-r--r--   0 laicj      (501) staff       (20)     8788 2023-04-22 14:42:23.000000 tinyOpenAI-0.13/tinyOpenAI.egg-info/PKG-INFO
+-rw-r--r--   0 laicj      (501) staff       (20)      270 2023-04-22 14:42:23.000000 tinyOpenAI-0.13/tinyOpenAI.egg-info/SOURCES.txt
+-rw-r--r--   0 laicj      (501) staff       (20)        1 2023-04-22 14:42:23.000000 tinyOpenAI-0.13/tinyOpenAI.egg-info/dependency_links.txt
+-rw-r--r--   0 laicj      (501) staff       (20)       53 2023-04-22 14:42:23.000000 tinyOpenAI-0.13/tinyOpenAI.egg-info/entry_points.txt
+-rw-r--r--   0 laicj      (501) staff       (20)        9 2023-04-22 14:42:23.000000 tinyOpenAI-0.13/tinyOpenAI.egg-info/requires.txt
+-rw-r--r--   0 laicj      (501) staff       (20)       11 2023-04-22 14:42:23.000000 tinyOpenAI-0.13/tinyOpenAI.egg-info/top_level.txt
```

### Comparing `tinyOpenAI-0.12/LICENSE` & `tinyOpenAI-0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyOpenAI-0.12/PKG-INFO` & `tinyOpenAI-0.13/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,60 @@
 Metadata-Version: 2.1
 Name: tinyOpenAI
-Version: 0.12
+Version: 0.13
 Summary: Tiny OpenAI ChatGPT and Whisper API Library
 Home-page: https://github.com/wolf71/tinyOpenAI
 Author: Charles Lai
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tiny OpenAI ChatGPT and Whisper API Library
-- 2023/3     V0.12       By Charles Lai
+- 2023/4     V0.13       By Charles Lai
 
 ## Features
 - OpenAI ChatGPT and Whisper API library written in pure Python, so it can run in Python environment on M1/M2 Mac, iPad/iPhone(e.g. Pythonista, Juno, CODE, Pyto, ...), Android.
-- Supports methods that conform to the ChatGPT API JSON format for API calls. Provides an easy-to-use quick dialog method, support for contextual associations; and easy language translation method.
+- Supports methods that conform to the ChatGPT API JSON format for API calls. Provides an easy-to-use quick dialog method, support for contextual associations; and easy language translation method. 
+- ChatGPT Supports streaming output.
 - Support for Whisper API calls to recognize and parse uploaded audio files as text messages or translate them into English.
 - Support Embedding API call, Embedding vectorization of the incoming text, support string or text array
 
 ## How to Use
 ### ChatGPT
-- **__init__(self, API_Key='', Proxy='', Model='gpt-3.5-turbo', URL='https://api.openai.com/v1/chat/completions', Debug=False)**
+- **__init__(self, API_Key='', Proxy='', Model='gpt-3.5-turbo', URL='https://api.openai.com/v1/chat/completions', Debug=False, stream=False)**
   - Initialize the ChatGPT object, with the following parameters
   - API_Key: your openAI API Key
   - Proxy: If needed, set your http proxy server, e.g.: http://192.168.3.1:3128
   - Model: If needed, you can set it according to the OpenAI API documentation, e.g. change the default gpt-3.5-turbo to gpt-3.5-turbo-0301
   - URL: If OpenAI has changed the API URL address, you can change it here
   - Debug: if there is a network error or call error, whether to print out the error message, default is False.
+  - stream: using openAI stream mode (the content returned by openAI to be displayed as a stream)
 - **call(self, data)**
   - Call ChatGPT interface, return data in JSON format (see OpenAI API documentation for JSON details)
   - data is a Python dictionary (same as JSON), see the OpenAI API documentation for details, for example:
 ``` python
   data = [ {"role": "system", "content": "You are a helpful assistant."}, {"role": "user", "content": "What is the OpenAI mission?"} ]
-```  
+```
+  - Return data:
+    - If non-stream mode, return as string
+    - If stream mode, return a constructor, can be output: for t in ret, ret is constructor, and t is a string
 - **query(data, flag=False, hcnt=0, system='You are a helpful assistant.')**
   - To simplify the operation, the query method implements the simplest and quickest dialog function, simply typing the question and returning the text of the ChatGPT answer.
   - data: your question text
   - flag: whether you need to ensure contextual coherence in the conversation. Because of the nature of ChatGPT, if you want the next question to be related to the previous one, you need to do something special and bring the previous content and answer with you. To do this, just set the flag to True
   - hcnt: The number of contextual history conversations, default is 0, which means that each conversation will pass all previous history questions and answers to ChatGPT. Set to 6, which means that only the last 6 conversations will be kept. (Note: Because of ChatGPT's limit, the maximum number of tokens per conversation is 4096, so keeping all the history will cause the limit to be exceeded)
   - system: This is used to set the system role description of ChatGPT, see the OpenAI documentation for details
+  - Returns data:
+    - The result text returned by openAI
+    - If stream mode, the results will be print out (streamed on the terminal); when all content is completed, the result text is returned
 - **translate(text, lang='simplified chinese')**
   - To simplify the operation, a quick language translation function is provided to translate the input text into the corresponding language.
   - text: the text to be translated
   - lang: the language you want to translate to, e.g. english, japan, simplified chinese, etc.
 - **cHinfo()**
   - Delete Contextual Dialog History
 - **Statistics**
@@ -55,23 +63,25 @@
 - **Conversation history data and clear**
   - Hinfo: When using the query method and setting flag=True, this list holds all the conversation history.
   - If you need to delete it, use the cHinfo() method
 - **A simple example**
 ``` python
 import tinyOpenAI
 
-g = tinyOpenAI.ChatGPT('your OpenAI API_Key')
+g = tinyOpenAI.ChatGPT('your OpenAI API_Key', stream=True))
 # g = tinyOpenAI.ChatGPT('your OpenAI API_Key','http://192.168.3.2:3128', Model='gpt-3.5-turbo-0301',Debug=True)
 # Conversation
-print( g.query('Write a rhyming poem with the sea as the title', system='You are a master of art, answer questions with emoji icons') )
+# if using stream=True mode, you don't neet print, otherwise using print()
+# print( g.query('Write a rhyming poem with the sea as the title', system='You are a master of art, answer questions with emoji icons') )
+g.query('Write a rhyming poem with the sea as the title', system='You are a master of art, answer questions with emoji icons')
 # Continuous dialogue
 print('======== continuous dialogue ============')
-print(g.query('charles has $500, tom has $300, how much money do they have in total', True, 6))
-print(g.query('charles and Tom who has more money', True, 6))
-print(g.query('Sort them in order of money', True, 6))
+g.query('charles has $500, tom has $300, how much money do they have in total', True, 6)
+g.query('charles and Tom who has more money', True, 6)
+g.query('Sort them in order of money', True, 6)
 # print history
 print(g.Hinfo)
 # clear Histroy
 g.cHinfo()
 # Statistics 
 print('Call cnt: %d, Total using tokens: %d' % (g.Call_cnt, g.Total_tokens) )
 ```
```

### Comparing `tinyOpenAI-0.12/setup.py` & `tinyOpenAI-0.13/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('Readme.md', 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name = 'tinyOpenAI',
-    version = '0.12',
+    version = '0.13',
     author = 'Charles Lai',
     author_email = '',
     description = 'Tiny OpenAI ChatGPT and Whisper API Library',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/wolf71/tinyOpenAI',
     packages = ['tinyOpenAI'],   #setuptools.find_packages(),
```

### Comparing `tinyOpenAI-0.12/tinyOpenAI/tinyOpenAI.py` & `tinyOpenAI-0.13/tinyOpenAI/tinyOpenAI.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,37 @@
 '''
   # Tiny OpenAI ChatGPT and Whisper API Library
   - 2023/3     V0.1       By Charles Lai
+  - 2023/4     V0.13
 '''
-__version__ = 0.12
+__version__ = 0.13
 __author__ = 'Charles Lai'
 
-import requests
+import requests, json
 
+def get_delta(rdata):
+  ''' Return stream mode delta text '''
+  # len() > 13 by pass  b'' and b'data: [DONE]'
+  if len(rdata) > 13:
+    return json.loads(rdata.decode('utf-8')[5:]).get('choices', [{}])[0].get('delta', {}).get('content','')
+  else:
+    return ''
+    
 #
 # HTTP_Post Function
 #
 def httpPost(debug, *args, **kw):
   ''' OpenAI API httpPost function 
     debug: True/False - Display Debug info;
     *args/**kw: requests.post args;
   '''
+  # get stream mode 
+  stream_mode = kw.get('json', {}).get('stream', False) == True
+  kw['stream'] = stream_mode
+
   # init return value
   rdata = {}
   try:
     r = requests.post(*args, **kw)
   except Exception as x:
     if debug:
       if type(x) == requests.exceptions.SSLError:
@@ -26,57 +39,62 @@
       else:
         print('@ Network Error!')
     # break return 
     return rdata
   # Get Result
   if r.status_code == 200:
     try:
-      rdata = r.json()
+      if stream_mode:
+        # return a iter
+        rdata = ( get_delta(i) for i in r.iter_lines() )
+      else:
+        rdata = r.json()
     except:
       pass
   # status code not 200, print error info
   elif debug:
     # 400-File Problem, 401-API_KEY, 404-URL 
     if r.status_code == 400:
       print('@ Error, Please Check File type(mp3/m4a/wav/... audio file !')
     elif r.status_code == 401:
       print('@ Error, Please Check API_Key !')
     elif r.status_code == 404:
       print('@ Error, Please Check API_URL !')
     else:
       print('@ Error, HTTP Status_code is: %d !' % r.status_code)
-  # Return Result JSON
-  return rdata
+  # Return Result, stream_mode
+  return rdata, stream_mode
 
 #
 # ChatGPT API
 #
 class ChatGPT():
-  def __init__(self, API_Key='', Proxy='', Model='gpt-3.5-turbo', URL='https://api.openai.com/v1/chat/completions', Debug=False):
-    ''' ChatGPT API Access, args: API_Key, Proxy, Model, API_URL, Debug '''
+  def __init__(self, API_Key='', Proxy='', Model='gpt-3.5-turbo', URL='https://api.openai.com/v1/chat/completions', Debug=False, stream=False):
+    ''' ChatGPT API Access, args: API_Key, Proxy, Model, API_URL, Debug, stream '''
     self.API_Key = API_Key
     self.URL = URL
     self.Proxy = Proxy
     self.Model = Model
     self.Debug = Debug      # Debug info print
+    self.stream = stream    # openAI stream mode    
     self.Call_cnt = 0       # Total Call count
     self.Total_tokens = 0   # Total tokens count
     self.Hinfo = []         # Query History List
 
   def call(self, data):
     ''' Call ChatGPT '''
     headers = { "Content-Type": "application/json", "Authorization": f"Bearer {self.API_Key}" }
     # Call API
-    rdata = httpPost(self.Debug, self.URL, headers = headers, proxies={"http": self.Proxy, "https": self.Proxy}, json = {"model": self.Model, "messages": data})
+    rdata, stream_mode = httpPost(self.Debug, self.URL, headers = headers, proxies={"http": self.Proxy, "https": self.Proxy}, json = {"model": self.Model, "messages": data, "stream": self.stream})
     # add total_tokens, call times
-    if rdata:
+    self.Call_cnt += 1        
+    if not stream_mode and rdata:
       self.Total_tokens += rdata.get('usage', {}).get('total_tokens', 0)
-      self.Call_cnt += 1
     # return result
-    return rdata
+    return rdata, stream_mode
   
   def get_text(self, rdata):
     ''' Return only message text, rdata = chatGPT return json '''
     if rdata:
       # get rdata['choices'][0]['message']['content']
       return rdata.get('choices', [{}])[0].get('message', {}).get('content', '').encode('utf8').decode()
     else:
@@ -86,27 +104,41 @@
     ''' Quick ask ChatGPT, data = Query string 
       flag: Using Query History flag  (Using obj.Hinfo = [] clean history.)
       hcnt: History count, 0:all, >0 last n (etc: 3-last 3, 10-last 10)
       system: ChatGPT system role content
     '''
     if flag:
       # Using Query History [abs to avoid negative numbers, *2 for Q&A paired]
-      ret = self.get_text( self.call([{"role": "system", "content": system}] + self.Hinfo[-abs(hcnt*2):] + [{"role": "user", "content": data}]) )
-      # add Query + Answer to History list
-      self.Hinfo.append({"role": "user", "content": data})
-      self.Hinfo.append({"role": "assistant", "content": ret})
+      qdata = [{"role": "system", "content": system}] + self.Hinfo[-abs(hcnt*2):] + [{"role": "user", "content": data}]
     else:
-      ret = self.get_text( self.call([{"role": "system", "content": system}, {"role": "user","content": data}]) )
+      qdata = [{"role": "system", "content": system}, {"role": "user","content": data}]
+    # query openAI
+    r, stream_mode = self.call(qdata)
+    if not stream_mode:
+      ret = self.get_text(r)
+    else:
+      # stream mode, print out and then return result
+      ret = []
+      for t in r:
+        print(t, end='', flush=True)
+        ret.append(t)
+        # calc tokens (data is not available and only be estimated)
+        self.Total_tokens += 1
+      print()
+      ret = ''.join(ret)
+    # add Query + Answer to History list
+    self.Hinfo.append({"role": "user", "content": data})
+    self.Hinfo.append({"role": "assistant", "content": ret})
     return ret
 
   def translate(self, text, lang='simplified chinese'):
     ''' Translate text to Simple Chinese or other '''
     text = text.strip()
     if text:
-      return self.get_text( self.call([{"role": "user", "content": f"Please help me to translate,`{text}` to {lang}, please return only translated content not include the origin text"}]) )
+      return self.query( f"Please help me to translate,`{text}` to {lang}, please return only translated content not include the origin text", False, 0, '')
     else:
       return ''
 
   def cHinfo(self):
     ''' Clean query History '''
     self.Hinfo = []
 
@@ -130,15 +162,15 @@
       file: file name
       Type: 0.transcribes in source language  1.transcribes into English
     '''
     # check type
     if Type > len(self.URL): Type = len(self.URL) - 1
     # # Call ChatGPT API
     try:
-      rdata = httpPost(self.Debug, self.URL[Type], headers = { "Authorization": f"Bearer {self.API_Key}" }, proxies = {"http": self.Proxy, "https": self.Proxy}, data = {'model': self.Model}, files = {'file': (file, open(file,'rb'))} )
+      rdata, _ = httpPost(self.Debug, self.URL[Type], headers = { "Authorization": f"Bearer {self.API_Key}" }, proxies = {"http": self.Proxy, "https": self.Proxy}, data = {'model': self.Model}, files = {'file': (file, open(file,'rb'))} )
     except FileNotFoundError:
       print('@ Error, File Not Found!')
       rdata = ''
     # get result
     if rdata:
       rdata = rdata.get('text', '')
       # add total_tokens, call times
@@ -168,15 +200,15 @@
       How to using return value?
       1. ret[0]['embedding'] 
       2. for v in ret:
           v.get('embedding')
     '''
     headers = { "Content-Type": "application/json", "Authorization": f"Bearer {self.API_Key}" }
     # Call API
-    rdata = httpPost(self.Debug, self.URL, headers = headers, proxies={"http": self.Proxy, "https": self.Proxy}, json = {"model": self.Model, "input": data})
+    rdata, _ = httpPost(self.Debug, self.URL, headers = headers, proxies={"http": self.Proxy, "https": self.Proxy}, json = {"model": self.Model, "input": data})
     # add total_tokens, call times
     if rdata:
       self.Total_tokens += rdata.get('usage', {}).get('total_tokens', 0)
       self.Call_cnt += 1
     # return result
     return rdata.get('data', [])
 
@@ -189,23 +221,26 @@
     # get API_Key
     API_Key = sys.argv[1]
     # get Proxy
     if len(sys.argv) > 2:
       Proxy = sys.argv[2]
     else:
       Proxy = ''
-    r = ChatGPT(API_Key, Proxy, Debug=True)
+    r = ChatGPT(API_Key, Proxy, Debug=True, stream=True)
     print('>>> ChatGPT Query <<<')
     while True:
       try:
         cmd = input('> ').strip()
-        if cmd:
+        if cmd == '?':
+          print(f'Call Time: {r.Call_cnt}, Total Tokens: {r.Total_tokens}.')
+        elif cmd:
           print('= '*36)
-          print( r.query(cmd, True, 6) )
+          r.query(cmd, True, 6)
           print()
       except KeyboardInterrupt:
+        print()
         break
   else:
     print('> Using python tinyOpenAI.py your_OpenAI_Key Proxy')
 
 if __name__ == "__main__":
   QueryDemo()
```

### Comparing `tinyOpenAI-0.12/tinyOpenAI.egg-info/PKG-INFO` & `tinyOpenAI-0.13/tinyOpenAI.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,60 @@
 Metadata-Version: 2.1
 Name: tinyOpenAI
-Version: 0.12
+Version: 0.13
 Summary: Tiny OpenAI ChatGPT and Whisper API Library
 Home-page: https://github.com/wolf71/tinyOpenAI
 Author: Charles Lai
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tiny OpenAI ChatGPT and Whisper API Library
-- 2023/3     V0.12       By Charles Lai
+- 2023/4     V0.13       By Charles Lai
 
 ## Features
 - OpenAI ChatGPT and Whisper API library written in pure Python, so it can run in Python environment on M1/M2 Mac, iPad/iPhone(e.g. Pythonista, Juno, CODE, Pyto, ...), Android.
-- Supports methods that conform to the ChatGPT API JSON format for API calls. Provides an easy-to-use quick dialog method, support for contextual associations; and easy language translation method.
+- Supports methods that conform to the ChatGPT API JSON format for API calls. Provides an easy-to-use quick dialog method, support for contextual associations; and easy language translation method. 
+- ChatGPT Supports streaming output.
 - Support for Whisper API calls to recognize and parse uploaded audio files as text messages or translate them into English.
 - Support Embedding API call, Embedding vectorization of the incoming text, support string or text array
 
 ## How to Use
 ### ChatGPT
-- **__init__(self, API_Key='', Proxy='', Model='gpt-3.5-turbo', URL='https://api.openai.com/v1/chat/completions', Debug=False)**
+- **__init__(self, API_Key='', Proxy='', Model='gpt-3.5-turbo', URL='https://api.openai.com/v1/chat/completions', Debug=False, stream=False)**
   - Initialize the ChatGPT object, with the following parameters
   - API_Key: your openAI API Key
   - Proxy: If needed, set your http proxy server, e.g.: http://192.168.3.1:3128
   - Model: If needed, you can set it according to the OpenAI API documentation, e.g. change the default gpt-3.5-turbo to gpt-3.5-turbo-0301
   - URL: If OpenAI has changed the API URL address, you can change it here
   - Debug: if there is a network error or call error, whether to print out the error message, default is False.
+  - stream: using openAI stream mode (the content returned by openAI to be displayed as a stream)
 - **call(self, data)**
   - Call ChatGPT interface, return data in JSON format (see OpenAI API documentation for JSON details)
   - data is a Python dictionary (same as JSON), see the OpenAI API documentation for details, for example:
 ``` python
   data = [ {"role": "system", "content": "You are a helpful assistant."}, {"role": "user", "content": "What is the OpenAI mission?"} ]
-```  
+```
+  - Return data:
+    - If non-stream mode, return as string
+    - If stream mode, return a constructor, can be output: for t in ret, ret is constructor, and t is a string
 - **query(data, flag=False, hcnt=0, system='You are a helpful assistant.')**
   - To simplify the operation, the query method implements the simplest and quickest dialog function, simply typing the question and returning the text of the ChatGPT answer.
   - data: your question text
   - flag: whether you need to ensure contextual coherence in the conversation. Because of the nature of ChatGPT, if you want the next question to be related to the previous one, you need to do something special and bring the previous content and answer with you. To do this, just set the flag to True
   - hcnt: The number of contextual history conversations, default is 0, which means that each conversation will pass all previous history questions and answers to ChatGPT. Set to 6, which means that only the last 6 conversations will be kept. (Note: Because of ChatGPT's limit, the maximum number of tokens per conversation is 4096, so keeping all the history will cause the limit to be exceeded)
   - system: This is used to set the system role description of ChatGPT, see the OpenAI documentation for details
+  - Returns data:
+    - The result text returned by openAI
+    - If stream mode, the results will be print out (streamed on the terminal); when all content is completed, the result text is returned
 - **translate(text, lang='simplified chinese')**
   - To simplify the operation, a quick language translation function is provided to translate the input text into the corresponding language.
   - text: the text to be translated
   - lang: the language you want to translate to, e.g. english, japan, simplified chinese, etc.
 - **cHinfo()**
   - Delete Contextual Dialog History
 - **Statistics**
@@ -55,23 +63,25 @@
 - **Conversation history data and clear**
   - Hinfo: When using the query method and setting flag=True, this list holds all the conversation history.
   - If you need to delete it, use the cHinfo() method
 - **A simple example**
 ``` python
 import tinyOpenAI
 
-g = tinyOpenAI.ChatGPT('your OpenAI API_Key')
+g = tinyOpenAI.ChatGPT('your OpenAI API_Key', stream=True))
 # g = tinyOpenAI.ChatGPT('your OpenAI API_Key','http://192.168.3.2:3128', Model='gpt-3.5-turbo-0301',Debug=True)
 # Conversation
-print( g.query('Write a rhyming poem with the sea as the title', system='You are a master of art, answer questions with emoji icons') )
+# if using stream=True mode, you don't neet print, otherwise using print()
+# print( g.query('Write a rhyming poem with the sea as the title', system='You are a master of art, answer questions with emoji icons') )
+g.query('Write a rhyming poem with the sea as the title', system='You are a master of art, answer questions with emoji icons')
 # Continuous dialogue
 print('======== continuous dialogue ============')
-print(g.query('charles has $500, tom has $300, how much money do they have in total', True, 6))
-print(g.query('charles and Tom who has more money', True, 6))
-print(g.query('Sort them in order of money', True, 6))
+g.query('charles has $500, tom has $300, how much money do they have in total', True, 6)
+g.query('charles and Tom who has more money', True, 6)
+g.query('Sort them in order of money', True, 6)
 # print history
 print(g.Hinfo)
 # clear Histroy
 g.cHinfo()
 # Statistics 
 print('Call cnt: %d, Total using tokens: %d' % (g.Call_cnt, g.Total_tokens) )
 ```
```

