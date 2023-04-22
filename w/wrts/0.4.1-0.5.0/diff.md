# Comparing `tmp/wrts-0.4.1.tar.gz` & `tmp/wrts-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wrts-0.4.1.tar", max compression
+gzip compressed data, was "wrts-0.5.0.tar", max compression
```

## Comparing `wrts-0.4.1.tar` & `wrts-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1065 2023-03-22 16:12:04.429969 wrts-0.4.1/LICENSE
--rw-r--r--   0        0        0       37 2023-03-22 16:18:26.368042 wrts-0.4.1/README.md
--rw-r--r--   0        0        0      318 2023-04-02 09:32:22.836034 wrts-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2248 2023-04-02 09:21:48.956589 wrts-0.4.1/wrts/Session.py
--rw-r--r--   0        0        0     1938 2023-03-31 18:17:12.044475 wrts-0.4.1/wrts/Session.py.save
--rw-r--r--   0        0        0       23 2023-03-29 14:33:45.440163 wrts-0.4.1/wrts/__init__.py
--rw-r--r--   0        0        0      812 2023-04-01 13:24:15.351409 wrts-0.4.1/wrts/types/Notif.py
--rw-r--r--   0        0        0     3059 2023-04-02 09:31:25.286074 wrts-0.4.1/wrts/types/Question.py
--rw-r--r--   0        0        0     1770 2023-03-30 08:03:44.912149 wrts-0.4.1/wrts/types/Subject.py
--rw-r--r--   0        0        0      894 2023-03-31 15:45:23.648318 wrts-0.4.1/wrts/types/User.py
--rw-r--r--   0        0        0     1993 2023-04-01 13:27:38.571992 wrts-0.4.1/wrts/types/__pycache__/Notif.cpython-311.pyc
--rw-r--r--   0        0        0     6002 2023-04-02 09:31:28.466072 wrts-0.4.1/wrts/types/__pycache__/Question.cpython-311.pyc
--rw-r--r--   0        0        0     2740 2023-03-30 08:07:02.020367 wrts-0.4.1/wrts/types/__pycache__/Subject.cpython-311.pyc
--rw-r--r--   0        0        0     2244 2023-03-31 15:45:28.728299 wrts-0.4.1/wrts/types/__pycache__/User.cpython-311.pyc
--rw-r--r--   0        0        0      670 1970-01-01 00:00:00.000000 wrts-0.4.1/setup.py
--rw-r--r--   0        0        0      596 1970-01-01 00:00:00.000000 wrts-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-03-22 16:12:04.429969 wrts-0.5.0/LICENSE
+-rw-r--r--   0        0        0       37 2023-03-22 16:18:26.368042 wrts-0.5.0/README.md
+-rw-r--r--   0        0        0      318 2023-04-22 09:57:36.344570 wrts-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2873 2023-04-22 09:57:05.594546 wrts-0.5.0/wrts/Session.py
+-rw-r--r--   0        0        0     1938 2023-03-31 18:17:12.044475 wrts-0.5.0/wrts/Session.py.save
+-rw-r--r--   0        0        0       23 2023-03-29 14:33:45.440163 wrts-0.5.0/wrts/__init__.py
+-rw-r--r--   0        0        0      812 2023-04-01 13:24:15.351409 wrts-0.5.0/wrts/types/Notif.py
+-rw-r--r--   0        0        0     3059 2023-04-02 09:31:25.286074 wrts-0.5.0/wrts/types/Question.py
+-rw-r--r--   0        0        0     1770 2023-03-30 08:03:44.912149 wrts-0.5.0/wrts/types/Subject.py
+-rw-r--r--   0        0        0      894 2023-03-31 15:45:23.648318 wrts-0.5.0/wrts/types/User.py
+-rw-r--r--   0        0        0     1993 2023-04-01 13:27:38.571992 wrts-0.5.0/wrts/types/__pycache__/Notif.cpython-311.pyc
+-rw-r--r--   0        0        0     6002 2023-04-02 09:31:28.466072 wrts-0.5.0/wrts/types/__pycache__/Question.cpython-311.pyc
+-rw-r--r--   0        0        0     2740 2023-03-30 08:07:02.020367 wrts-0.5.0/wrts/types/__pycache__/Subject.cpython-311.pyc
+-rw-r--r--   0        0        0     2244 2023-03-31 15:45:28.728299 wrts-0.5.0/wrts/types/__pycache__/User.cpython-311.pyc
+-rw-r--r--   0        0        0      670 1970-01-01 00:00:00.000000 wrts-0.5.0/setup.py
+-rw-r--r--   0        0        0      596 1970-01-01 00:00:00.000000 wrts-0.5.0/PKG-INFO
```

### Comparing `wrts-0.4.1/LICENSE` & `wrts-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wrts-0.4.1/wrts/Session.py` & `wrts-0.5.0/wrts/Session.py.save`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from .types.Question import Question
 from .types.Subject import Subject
-from .types.Notif import Notif
 import requests, json
 
 class LoginFailure(Exception):
 	pass
 
 class QuestionFailure(Exception):
 	pass
 
+class Notif:
+	def __init__(self, obj):
+
+
 class Session:
 	loggedin = False
 	renew = 0
 	expiration = 0
 	token = ""
 	subjects = None
 	def __init__(self, user, passwd):
@@ -30,25 +33,21 @@
 		if not resp["success"]:
 			raise LoginFailure(resp["info"])
 		self.loggedin = True
 		self.renew = resp["renew_from"]
 		self.expiration = resp["expires_at"]
 		self.token = resp["auth_token"]
 	def get_notifs(self, page, per_page=10):
-		def generator(objs, token):
-			for obj in objs:
-				yield Notif(obj, token)
-		resp = requests.get(f"https://api.wrts.nl/api/v3/users/notifications?page={page}&per_page={per_page}", headers={"x-auth-token": self.token}).json()
-		return resp["total_count"], generator(resp["notifications"],self.token)
+		
 	def get_questions(self):
 		resp = requests.get("https://api.wrts.nl/api/v3/public/qna/questions", headers={"x-auth-token": self.token}).json()
 		def gen(questions, token):
 			for q in questions:
 				yield Question(q["id"],self.token)
-		return resp["total_count"], gen(resp["results"], self.token)
+		return gen(resp["results"], self.token)
 	def get_question(self, id):
 		return Question(id, self.token)
 	def post_question(self, contents, subject, topic=None, attachments=[]):
 		data = {"contents": contents, "subject_id": subject.id, "qna_attachments_attributes": attachments}
 		if not topic == None:  data["topic_id"] = topic.id
 		resp = requests.post("https://api.wrts.nl/api/v3/qna/questions",headers={"x-auth-token": self.token},json=json.dumps({"qna_question":data})).json()
 		if "success" in resp:
```

### Comparing `wrts-0.4.1/wrts/Session.py.save` & `wrts-0.5.0/wrts/Session.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from .types.Question import Question
 from .types.Subject import Subject
-import requests, json
+from .types.Notif import Notif
+import requests, json, platform
 
 class LoginFailure(Exception):
 	pass
 
 class QuestionFailure(Exception):
 	pass
 
-class Notif:
-	def __init__(self, obj):
-
+class UploadError(Exception):
+	pass
 
 class Session:
 	loggedin = False
 	renew = 0
 	expiration = 0
 	token = ""
 	subjects = None
@@ -32,22 +32,38 @@
 		#print(resp)
 		if not resp["success"]:
 			raise LoginFailure(resp["info"])
 		self.loggedin = True
 		self.renew = resp["renew_from"]
 		self.expiration = resp["expires_at"]
 		self.token = resp["auth_token"]
+	def upload(self, path, mimetype="image/png"):
+		f = open(path, "rb")
+		data = f.read()
+		f.close()
+		Sep = "/"
+		if platform.system() == "Windows": Sep = "\\"
+		resp = requests.get("https://api.wrts.nl/api/v3/qna/questions/presigned_image_url", headers={"x-auth-token": self.token}).json()
+		stat = requests.put(resp["signed_url"],headers={"x-auth-token":self.token,"Content-type":mimetype},data=data).status_code
+		if stat == 200:
+			return {"file_name": path.split(Sep)[-1], "image": resp["signed_url"].split("?")[0]}
+		else:
+			raise UploadError(f"Failed to upload {path}")
 	def get_notifs(self, page, per_page=10):
-		
+		def generator(objs, token):
+			for obj in objs:
+				yield Notif(obj, token)
+		resp = requests.get(f"https://api.wrts.nl/api/v3/users/notifications?page={page}&per_page={per_page}", headers={"x-auth-token": self.token}).json()
+		return resp["total_count"], generator(resp["notifications"],self.token)
 	def get_questions(self):
 		resp = requests.get("https://api.wrts.nl/api/v3/public/qna/questions", headers={"x-auth-token": self.token}).json()
 		def gen(questions, token):
 			for q in questions:
 				yield Question(q["id"],self.token)
-		return gen(resp["results"], self.token)
+		return resp["total_count"], gen(resp["results"], self.token)
 	def get_question(self, id):
 		return Question(id, self.token)
 	def post_question(self, contents, subject, topic=None, attachments=[]):
 		data = {"contents": contents, "subject_id": subject.id, "qna_attachments_attributes": attachments}
 		if not topic == None:  data["topic_id"] = topic.id
 		resp = requests.post("https://api.wrts.nl/api/v3/qna/questions",headers={"x-auth-token": self.token},json=json.dumps({"qna_question":data})).json()
 		if "success" in resp:
```

### Comparing `wrts-0.4.1/wrts/types/Notif.py` & `wrts-0.5.0/wrts/types/Notif.py`

 * *Files identical despite different names*

### Comparing `wrts-0.4.1/wrts/types/Question.py` & `wrts-0.5.0/wrts/types/Question.py`

 * *Files identical despite different names*

### Comparing `wrts-0.4.1/wrts/types/Subject.py` & `wrts-0.5.0/wrts/types/Subject.py`

 * *Files identical despite different names*

### Comparing `wrts-0.4.1/wrts/types/User.py` & `wrts-0.5.0/wrts/types/User.py`

 * *Files identical despite different names*

### Comparing `wrts-0.4.1/wrts/types/__pycache__/Notif.cpython-311.pyc` & `wrts-0.5.0/wrts/types/__pycache__/Notif.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wrts-0.4.1/wrts/types/__pycache__/Question.cpython-311.pyc` & `wrts-0.5.0/wrts/types/__pycache__/Question.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wrts-0.4.1/wrts/types/__pycache__/Subject.cpython-311.pyc` & `wrts-0.5.0/wrts/types/__pycache__/Subject.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wrts-0.4.1/wrts/types/__pycache__/User.cpython-311.pyc` & `wrts-0.5.0/wrts/types/__pycache__/User.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wrts-0.4.1/setup.py` & `wrts-0.5.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'wrts',
-    'version': '0.4.1',
+    'version': '0.5.0',
     'description': 'A small lil library for using the WRTS API ',
     'long_description': 'still in development pls wait xdddzs\n',
     'author': 'BadPythonCoder',
     'author_email': 'no@no.no',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `wrts-0.4.1/PKG-INFO` & `wrts-0.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wrts
-Version: 0.4.1
+Version: 0.5.0
 Summary: A small lil library for using the WRTS API 
 Author: BadPythonCoder
 Author-email: no@no.no
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

