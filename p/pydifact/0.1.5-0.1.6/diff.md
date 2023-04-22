# Comparing `tmp/pydifact-0.1.5.tar.gz` & `tmp/pydifact-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydifact-0.1.5.tar", last modified: Mon Jan 24 21:25:41 2022, max compression
+gzip compressed data, was "pydifact-0.1.6.tar", last modified: Sat Apr 22 12:31:55 2023, max compression
```

## Comparing `pydifact-0.1.5.tar` & `pydifact-0.1.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2022-01-24 21:25:41.561671 pydifact-0.1.5/
--rw-r--r--   0 christian  (1000) christian  (1000)     1081 2020-10-29 21:36:06.000000 pydifact-0.1.5/LICENSE
--rw-r--r--   0 christian  (1000) christian  (1000)     4880 2022-01-24 21:25:41.561671 pydifact-0.1.5/PKG-INFO
--rw-r--r--   0 christian  (1000) christian  (1000)     4121 2021-11-01 11:14:40.000000 pydifact-0.1.5/README.md
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2022-01-24 21:25:41.555004 pydifact-0.1.5/pydifact/
--rw-r--r--   0 christian  (1000) christian  (1000)     2406 2022-01-24 21:25:41.000000 pydifact-0.1.5/pydifact/__init__.py
--rw-r--r--   0 christian  (1000) christian  (1000)      551 2020-10-29 21:40:08.000000 pydifact-0.1.5/pydifact/api.py
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2022-01-24 21:25:41.558338 pydifact-0.1.5/pydifact/control/
--rw-r--r--   0 christian  (1000) christian  (1000)       35 2020-10-29 21:36:06.000000 pydifact-0.1.5/pydifact/control/__init__.py
--rw-r--r--   0 christian  (1000) christian  (1000)     4772 2021-05-06 17:30:24.000000 pydifact-0.1.5/pydifact/control/characters.py
--rw-r--r--   0 christian  (1000) christian  (1000)     7486 2021-10-22 20:03:43.000000 pydifact-0.1.5/pydifact/parser.py
--rw-r--r--   0 christian  (1000) christian  (1000)    18227 2022-01-24 21:22:07.000000 pydifact-0.1.5/pydifact/segmentcollection.py
--rw-r--r--   0 christian  (1000) christian  (1000)     5764 2021-05-06 17:30:24.000000 pydifact-0.1.5/pydifact/segments.py
--rw-r--r--   0 christian  (1000) christian  (1000)     4200 2022-01-24 21:22:07.000000 pydifact-0.1.5/pydifact/serializer.py
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2022-01-24 21:25:41.558338 pydifact-0.1.5/pydifact/syntax/
--rw-r--r--   0 christian  (1000) christian  (1000)        1 2020-10-29 21:36:06.000000 pydifact-0.1.5/pydifact/syntax/__init__.py
--rw-r--r--   0 christian  (1000) christian  (1000)     1993 2021-11-01 10:37:02.000000 pydifact-0.1.5/pydifact/syntax/common.py
--rw-r--r--   0 christian  (1000) christian  (1000)      148 2020-10-29 21:36:06.000000 pydifact-0.1.5/pydifact/syntax/v1.py
--rw-r--r--   0 christian  (1000) christian  (1000)      148 2020-10-29 21:36:06.000000 pydifact-0.1.5/pydifact/syntax/v3.py
--rw-r--r--   0 christian  (1000) christian  (1000)      148 2020-10-29 21:36:06.000000 pydifact-0.1.5/pydifact/syntax/v4.py
--rw-r--r--   0 christian  (1000) christian  (1000)     2223 2021-05-06 18:44:29.000000 pydifact-0.1.5/pydifact/token.py
--rw-r--r--   0 christian  (1000) christian  (1000)     5446 2021-05-06 18:44:29.000000 pydifact-0.1.5/pydifact/tokenizer.py
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2022-01-24 21:25:41.558338 pydifact-0.1.5/pydifact.egg-info/
--rw-r--r--   0 christian  (1000) christian  (1000)     4880 2022-01-24 21:25:41.000000 pydifact-0.1.5/pydifact.egg-info/PKG-INFO
--rw-r--r--   0 christian  (1000) christian  (1000)      851 2022-01-24 21:25:41.000000 pydifact-0.1.5/pydifact.egg-info/SOURCES.txt
--rw-r--r--   0 christian  (1000) christian  (1000)        1 2022-01-24 21:25:41.000000 pydifact-0.1.5/pydifact.egg-info/dependency_links.txt
--rw-r--r--   0 christian  (1000) christian  (1000)       15 2022-01-24 21:25:41.000000 pydifact-0.1.5/pydifact.egg-info/top_level.txt
--rw-r--r--   0 christian  (1000) christian  (1000)      743 2022-01-24 21:25:41.565005 pydifact-0.1.5/setup.cfg
--rw-r--r--   0 christian  (1000) christian  (1000)       38 2020-10-29 21:36:06.000000 pydifact-0.1.5/setup.py
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2022-01-24 21:25:41.561671 pydifact-0.1.5/tests/
--rw-r--r--   0 christian  (1000) christian  (1000)        0 2020-10-29 21:36:06.000000 pydifact-0.1.5/tests/__init__.py
--rw-r--r--   0 christian  (1000) christian  (1000)     1488 2020-10-29 21:36:06.000000 pydifact-0.1.5/tests/test_characters.py
--rw-r--r--   0 christian  (1000) christian  (1000)     2265 2020-10-29 21:36:06.000000 pydifact-0.1.5/tests/test_controlcharacters.py
--rw-r--r--   0 christian  (1000) christian  (1000)     1280 2021-08-08 10:16:31.000000 pydifact-0.1.5/tests/test_huge_message.py
--rw-r--r--   0 christian  (1000) christian  (1000)     2178 2021-08-08 10:16:31.000000 pydifact-0.1.5/tests/test_input_output.py
--rw-r--r--   0 christian  (1000) christian  (1000)     1054 2021-10-22 20:03:53.000000 pydifact-0.1.5/tests/test_message_with_colon_at_end.py
--rw-r--r--   0 christian  (1000) christian  (1000)     6692 2020-10-29 21:40:08.000000 pydifact-0.1.5/tests/test_parser.py
--rw-r--r--   0 christian  (1000) christian  (1000)     1468 2020-10-29 21:36:06.000000 pydifact-0.1.5/tests/test_segment.py
--rw-r--r--   0 christian  (1000) christian  (1000)     8793 2021-11-03 06:16:45.000000 pydifact-0.1.5/tests/test_segmentcollection.py
--rw-r--r--   0 christian  (1000) christian  (1000)     3880 2022-01-24 21:22:07.000000 pydifact-0.1.5/tests/test_serializer.py
--rw-r--r--   0 christian  (1000) christian  (1000)      244 2020-10-29 21:36:06.000000 pydifact-0.1.5/tests/test_syntax_v1.py
--rw-r--r--   0 christian  (1000) christian  (1000)     1163 2020-10-29 21:36:06.000000 pydifact-0.1.5/tests/test_token.py
--rw-r--r--   0 christian  (1000) christian  (1000)     4762 2020-10-29 21:40:08.000000 pydifact-0.1.5/tests/test_tokenizer.py
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-22 12:31:55.451465 pydifact-0.1.6/
+-rw-r--r--   0 christian  (1000) christian  (1000)     1081 2020-10-29 21:36:06.000000 pydifact-0.1.6/LICENSE
+-rw-r--r--   0 christian  (1000) christian  (1000)     4860 2023-04-22 12:31:55.451465 pydifact-0.1.6/PKG-INFO
+-rw-r--r--   0 christian  (1000) christian  (1000)     4121 2021-11-01 11:14:40.000000 pydifact-0.1.6/README.md
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-22 12:31:55.444797 pydifact-0.1.6/pydifact/
+-rw-r--r--   0 christian  (1000) christian  (1000)     2406 2023-04-22 12:31:54.000000 pydifact-0.1.6/pydifact/__init__.py
+-rw-r--r--   0 christian  (1000) christian  (1000)      558 2023-04-22 12:23:45.000000 pydifact-0.1.6/pydifact/api.py
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-22 12:31:55.444797 pydifact-0.1.6/pydifact/control/
+-rw-r--r--   0 christian  (1000) christian  (1000)       35 2020-10-29 21:36:06.000000 pydifact-0.1.6/pydifact/control/__init__.py
+-rw-r--r--   0 christian  (1000) christian  (1000)     4772 2021-05-06 17:30:24.000000 pydifact-0.1.6/pydifact/control/characters.py
+-rw-r--r--   0 christian  (1000) christian  (1000)     7710 2023-04-22 12:23:41.000000 pydifact-0.1.6/pydifact/parser.py
+-rw-r--r--   0 christian  (1000) christian  (1000)    18814 2023-04-22 12:11:54.000000 pydifact-0.1.6/pydifact/segmentcollection.py
+-rw-r--r--   0 christian  (1000) christian  (1000)     5783 2023-04-22 12:23:45.000000 pydifact-0.1.6/pydifact/segments.py
+-rw-r--r--   0 christian  (1000) christian  (1000)     4200 2022-01-24 21:22:07.000000 pydifact-0.1.6/pydifact/serializer.py
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-22 12:31:55.448131 pydifact-0.1.6/pydifact/syntax/
+-rw-r--r--   0 christian  (1000) christian  (1000)        1 2020-10-29 21:36:06.000000 pydifact-0.1.6/pydifact/syntax/__init__.py
+-rw-r--r--   0 christian  (1000) christian  (1000)     1993 2021-11-01 10:37:02.000000 pydifact-0.1.6/pydifact/syntax/common.py
+-rw-r--r--   0 christian  (1000) christian  (1000)      148 2020-10-29 21:36:06.000000 pydifact-0.1.6/pydifact/syntax/v1.py
+-rw-r--r--   0 christian  (1000) christian  (1000)      148 2020-10-29 21:36:06.000000 pydifact-0.1.6/pydifact/syntax/v3.py
+-rw-r--r--   0 christian  (1000) christian  (1000)      148 2020-10-29 21:36:06.000000 pydifact-0.1.6/pydifact/syntax/v4.py
+-rw-r--r--   0 christian  (1000) christian  (1000)     2223 2021-05-06 18:44:29.000000 pydifact-0.1.6/pydifact/token.py
+-rw-r--r--   0 christian  (1000) christian  (1000)     5446 2021-05-06 18:44:29.000000 pydifact-0.1.6/pydifact/tokenizer.py
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-22 12:31:55.444797 pydifact-0.1.6/pydifact.egg-info/
+-rw-r--r--   0 christian  (1000) christian  (1000)     4860 2023-04-22 12:31:55.000000 pydifact-0.1.6/pydifact.egg-info/PKG-INFO
+-rw-r--r--   0 christian  (1000) christian  (1000)      851 2023-04-22 12:31:55.000000 pydifact-0.1.6/pydifact.egg-info/SOURCES.txt
+-rw-r--r--   0 christian  (1000) christian  (1000)        1 2023-04-22 12:31:55.000000 pydifact-0.1.6/pydifact.egg-info/dependency_links.txt
+-rw-r--r--   0 christian  (1000) christian  (1000)       15 2023-04-22 12:31:55.000000 pydifact-0.1.6/pydifact.egg-info/top_level.txt
+-rw-r--r--   0 christian  (1000) christian  (1000)      743 2023-04-22 12:31:55.451465 pydifact-0.1.6/setup.cfg
+-rw-r--r--   0 christian  (1000) christian  (1000)       38 2020-10-29 21:36:06.000000 pydifact-0.1.6/setup.py
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-22 12:31:55.448131 pydifact-0.1.6/tests/
+-rw-r--r--   0 christian  (1000) christian  (1000)        0 2020-10-29 21:36:06.000000 pydifact-0.1.6/tests/__init__.py
+-rw-r--r--   0 christian  (1000) christian  (1000)     1488 2020-10-29 21:36:06.000000 pydifact-0.1.6/tests/test_characters.py
+-rw-r--r--   0 christian  (1000) christian  (1000)     2265 2020-10-29 21:36:06.000000 pydifact-0.1.6/tests/test_controlcharacters.py
+-rw-r--r--   0 christian  (1000) christian  (1000)     1280 2021-08-08 10:16:31.000000 pydifact-0.1.6/tests/test_huge_message.py
+-rw-r--r--   0 christian  (1000) christian  (1000)     2178 2021-08-08 10:16:31.000000 pydifact-0.1.6/tests/test_input_output.py
+-rw-r--r--   0 christian  (1000) christian  (1000)     1054 2021-10-22 20:03:53.000000 pydifact-0.1.6/tests/test_message_with_colon_at_end.py
+-rw-r--r--   0 christian  (1000) christian  (1000)     7109 2023-04-22 12:23:41.000000 pydifact-0.1.6/tests/test_parser.py
+-rw-r--r--   0 christian  (1000) christian  (1000)     1697 2023-04-22 12:23:45.000000 pydifact-0.1.6/tests/test_segment.py
+-rw-r--r--   0 christian  (1000) christian  (1000)     9314 2023-04-22 12:23:41.000000 pydifact-0.1.6/tests/test_segmentcollection.py
+-rw-r--r--   0 christian  (1000) christian  (1000)     4532 2023-04-22 12:23:41.000000 pydifact-0.1.6/tests/test_serializer.py
+-rw-r--r--   0 christian  (1000) christian  (1000)      244 2020-10-29 21:36:06.000000 pydifact-0.1.6/tests/test_syntax_v1.py
+-rw-r--r--   0 christian  (1000) christian  (1000)     1163 2020-10-29 21:36:06.000000 pydifact-0.1.6/tests/test_token.py
+-rw-r--r--   0 christian  (1000) christian  (1000)     4762 2020-10-29 21:40:08.000000 pydifact-0.1.6/tests/test_tokenizer.py
```

### Comparing `pydifact-0.1.5/LICENSE` & `pydifact-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pydifact-0.1.5/PKG-INFO` & `pydifact-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pydifact
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python EDI file parser.
 Home-page: https://github.com/nerdocs/pydifact
 Author: Christian González
 Author-email: christian.gonzalez@nerdocs.at
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
@@ -138,9 +137,7 @@
 
 
 ## License
 
 This library is licensed under the
 *MIT* license, see the
 [LICENSE file](LICENSE).
-
-
```

### Comparing `pydifact-0.1.5/README.md` & `pydifact-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pydifact-0.1.5/pydifact/__init__.py` & `pydifact-0.1.6/pydifact/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 from pydifact import segmentcollection, parser, segments, serializer, token, tokenizer
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 
 from .control.characters import Characters
 from .segmentcollection import SegmentCollection
 from .parser import Parser
 from .segments import Segment
 from .serializer import Serializer
 from .token import Token
```

### Comparing `pydifact-0.1.5/pydifact/control/characters.py` & `pydifact-0.1.6/pydifact/control/characters.py`

 * *Files identical despite different names*

### Comparing `pydifact-0.1.5/pydifact/parser.py` & `pydifact-0.1.6/pydifact/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,28 +47,32 @@
         :param message: The EDI message
         :rtype:
         """
 
         # If there is a UNA, take the following 6 characters
         # unconditionally, save them, strip them, and make control Characters()
         # for further parsing
-        if message[0:3] == "UNA":
+        self.una_found = message[0:3] == "UNA"
+
+        if self.una_found:
             self.characters = Characters.from_str("UNA" + message[3:9])
 
             # remove the UNA segment from the string
             message = message[9:].lstrip("\r\n")
 
         else:
             # if no UNA header present, use default control characters
             if characters is not None:
                 self.characters = characters
 
         tokenizer = Tokenizer()
         return self.convert_tokens_to_segments(
-            tokenizer.get_tokens(message, self.characters), self.characters
+            tokenizer.get_tokens(message, self.characters),
+            self.characters,
+            with_una=self.una_found,
         )
 
     @staticmethod
     def get_control_characters(
         message: str, characters: Characters = None
     ) -> Optional[Characters]:
         """Read the UNA segment from the passed string and extract/store the control characters from it.
@@ -101,34 +105,37 @@
         characters.decimal_point = chars[2]
         characters.escape_character = chars[3]
         characters.reserved_character = chars[4]
         characters.segment_terminator = chars[5]
 
         return characters
 
-    def convert_tokens_to_segments(self, tokens: list, characters: Characters):
+    def convert_tokens_to_segments(
+        self, tokens: list, characters: Characters, with_una: bool = False
+    ):
         """Convert the tokenized message into an array of segments.
-        :param with_una: whether the UNA segment should be included
         :param tokens: The tokens that make up the message
         :param characters: the control characters to use
+        :param with_una: whether the UNA segment should be included
         :type tokens: list of Token
         :rtype list of Segment
         """
 
         segments = []
         current_segment = []
         data_element = None
         in_segment = False
         empty_component_counter = 0
 
-        for token in tokens:
+        if with_una:
+            yield self.factory.create_segment("UNA", str(self.characters))
 
+        for token in tokens:
             # If we're in the middle of a segment, check if we've reached the end
             if in_segment:
-
                 if token.type == Token.Type.TERMINATOR:
                     in_segment = False
                     if len(data_element) == 0:  # empty element
                         data_element = ""
                     if len(data_element) == 1:
                         # use a str instead of a list
                         data_element = data_element[0]
```

### Comparing `pydifact-0.1.5/pydifact/segmentcollection.py` & `pydifact-0.1.6/pydifact/segmentcollection.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
-from collections.abc import Callable, Iterable
-from typing import List, Optional, Tuple, Union
+import codecs
 import datetime
 import warnings
+from collections.abc import Callable, Iterable
+from typing import List, Optional, Tuple, Union
 
 from pydifact.api import EDISyntaxError
+from pydifact.control import Characters
 from pydifact.parser import Parser
 from pydifact.segments import Segment
 from pydifact.serializer import Serializer
-from pydifact.control import Characters
-import codecs
 
 
 class AbstractSegmentsContainer:
     """Represent a collection of EDI Segments for both reading and writing.
 
     You should not instantiate AbstractSegmentsContainer itself, but subclass it use that.
 
@@ -87,28 +87,32 @@
         """
 
         # create a new instance of AbstractSegmentsContainer and return it
         # with the added segments
         return cls().add_segments(segments)
 
     def get_segments(
-        self, name: str, predicate: Callable = None  # Python3.9+ Callable[[Segment], bool]
+        self,
+        name: str,
+        predicate: Callable = None,  # Python3.9+ Callable[[Segment], bool]
     ) -> list:
         """Get all the segments that match the requested name.
 
         :param name: The name of the segments to return
         :param predicate: Optional predicate callable that returns True if the given segment matches a condition
         :rtype: list of Segment
         """
         for segment in self.segments:
             if segment.tag == name and (predicate is None or predicate(segment)):
                 yield segment
 
     def get_segment(
-        self, name: str, predicate: Callable = None  # Python3.9+ Callable[[Segment], bool]
+        self,
+        name: str,
+        predicate: Callable = None,  # Python3.9+ Callable[[Segment], bool]
     ) -> Optional[Segment]:
         """Get the first segment that matches the requested name.
 
         :return: The requested segment, or None if not found
         :param name: The name of the segment to return
         :param predicate: Optional predicate that must match on the segments
            to return
@@ -504,16 +508,26 @@
             unb = first_segment
         else:
             raise EDISyntaxError("An interchange must start with UNB or UNA and UNB")
         # Loosy syntax check :
         if len(unb.elements) < 4:
             raise EDISyntaxError("Missing elements in UNB header")
 
+        # In syntax version 3 the year is formatted using two digits, while in version 4 four digits are used.
+        # Since some EDIFACT files in the wild don't adhere to this specification, we just use whatever format seems
+        # more appropriate according to the length of the date string.
+        if len(unb.elements[3][0]) == 6:
+            datetime_fmt = "%y%m%d-%H%M"
+        elif len(unb.elements[3][0]) == 8:
+            datetime_fmt = "%Y%m%d-%H%M"
+        else:
+            raise EDISyntaxError("Timestamp of file-creation malformed.")
+
         datetime_str = "-".join(unb.elements[3])
-        timestamp = datetime.datetime.strptime(datetime_str, "%y%m%d-%H%M")
+        timestamp = datetime.datetime.strptime(datetime_str, datetime_fmt)
         interchange = Interchange(
             syntax_identifier=unb.elements[0],
             sender=unb.elements[1],
             recipient=unb.elements[2],
             timestamp=timestamp,
             control_reference=unb.elements[4],
         )
```

### Comparing `pydifact-0.1.5/pydifact/segments.py` & `pydifact-0.1.6/pydifact/segments.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     This class is used internally. read-world implementations of specialized should subclass Segment and provide
     the `tag` and `validate` attributes.
     """
 
     # tag is not a class attribute in this case, as each Segment instance could have another tag.
     __omitted__ = True
 
-    def __init__(self, tag: str, *elements: Union[str, List[str]]):
+    def __init__(self, tag: str, *elements: Union[str, List[str], None]):
         """Create a new Segment instance.
 
         :param str tag: The code/tag of the segment. Must not be empty.
         :param list elements: The data elements for this segment, as (possibly empty) list.
 
         """
         self.tag = tag
@@ -137,22 +137,23 @@
             raise EDISyntaxError(
                 "Tag '{}': A tag name must only contain alphanumeric characters.".format(
                     name
                 )
             )
 
         for Plugin in SegmentProvider.plugins:
-            if Plugin().tag == name:
+            if getattr(Plugin, "tag", "") == name:
                 s = Plugin(name, *elements)
+                break
         else:
             # we don't support this kind of EDIFACT segment (yet), so
             # just create a generic Segment()
             s = Segment(name, *elements)
 
         if validate:
             if not s.validate():
                 raise EDISyntaxError(
                     "could not create '{}' Segment. Validation failed.".format(name)
                 )
 
         # FIXME: characters is not used!
-        return Segment(name, *elements)
+        return s
```

### Comparing `pydifact-0.1.5/pydifact/serializer.py` & `pydifact-0.1.6/pydifact/serializer.py`

 * *Files identical despite different names*

### Comparing `pydifact-0.1.5/pydifact/syntax/common.py` & `pydifact-0.1.6/pydifact/syntax/common.py`

 * *Files identical despite different names*

### Comparing `pydifact-0.1.5/pydifact/token.py` & `pydifact-0.1.6/pydifact/token.py`

 * *Files identical despite different names*

### Comparing `pydifact-0.1.5/pydifact/tokenizer.py` & `pydifact-0.1.6/pydifact/tokenizer.py`

 * *Files identical despite different names*

### Comparing `pydifact-0.1.5/pydifact.egg-info/PKG-INFO` & `pydifact-0.1.6/pydifact.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pydifact
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python EDI file parser.
 Home-page: https://github.com/nerdocs/pydifact
 Author: Christian González
 Author-email: christian.gonzalez@nerdocs.at
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
@@ -138,9 +137,7 @@
 
 
 ## License
 
 This library is licensed under the
 *MIT* license, see the
 [LICENSE file](LICENSE).
-
-
```

### Comparing `pydifact-0.1.5/pydifact.egg-info/SOURCES.txt` & `pydifact-0.1.6/pydifact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydifact-0.1.5/setup.cfg` & `pydifact-0.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `pydifact-0.1.5/tests/test_characters.py` & `pydifact-0.1.6/tests/test_characters.py`

 * *Files identical despite different names*

### Comparing `pydifact-0.1.5/tests/test_controlcharacters.py` & `pydifact-0.1.6/tests/test_controlcharacters.py`

 * *Files identical despite different names*

### Comparing `pydifact-0.1.5/tests/test_huge_message.py` & `pydifact-0.1.6/tests/test_huge_message.py`

 * *Files identical despite different names*

### Comparing `pydifact-0.1.5/tests/test_input_output.py` & `pydifact-0.1.6/tests/test_input_output.py`

 * *Files identical despite different names*

### Comparing `pydifact-0.1.5/tests/test_message_with_colon_at_end.py` & `pydifact-0.1.6/tests/test_message_with_colon_at_end.py`

 * *Files identical despite different names*

### Comparing `pydifact-0.1.5/tests/test_parser.py` & `pydifact-0.1.6/tests/test_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -109,113 +109,116 @@
         a is not b
     ), "Two separatedly, but visually identically created Segment objects may not be the same object."
 
 
 def test_una_parser1(parser):
     # UNA headers are a special parsing task and must be processed correctly.
     tokens = parser.parse("UNA:+,? 'TEST'")
+    assert next(tokens) == Segment("UNA",":+,? '")
     assert next(tokens) == Segment("TEST")
 
 
 def test_una_parser2(parser):
     # UNA headers are a special parsing task and must be processed correctly.
     tokens = parser.parse("UNA123456TEST6")
+    assert next(tokens) == Segment("UNA","123456")
     assert next(tokens) == Segment("TEST")
 
 
 def test_una_parser3(parser):
     # UNA headers are a special parsing task and must be processed correctly.
     tokens = parser.parse("UNA12345'TEST'")
+    assert next(tokens) == Segment("UNA","12345'")
     assert next(tokens) == Segment("TEST")
 
 
 def test_basic1(parser, default_una_segment):
     _assert_segments(
-        parser, default_una_segment, "RFF+PD:50515", [Segment("RFF", ["PD", "50515"])]
+        parser, default_una_segment, "RFF+PD:50515", [Segment("UNA",":+,? '"),Segment("RFF", ["PD", "50515"])]
     )
 
 
 def test_basic2(parser, default_una_segment):
 
     _assert_segments(
-        parser, default_una_segment, "RFF+PD+50515", [Segment("RFF", "PD", "50515")]
+        parser, default_una_segment, "RFF+PD+50515", [Segment("UNA",":+,? '"),Segment("RFF", "PD", "50515")]
     )
 
 
 def test_escape_character(parser, default_una_segment):
     _assert_segments(
         parser,
         default_una_segment,
         "ERC+10:The message does not make sense??",
-        [Segment("ERC", ["10", "The message does not make sense?"])],
+        [Segment("UNA",":+,? '"),Segment("ERC", ["10", "The message does not make sense?"])],
     )
 
 
 def test_escape_component_separator(parser, default_una_segment):
 
     _assert_segments(
         parser,
         default_una_segment,
         "ERC+10:Name?: Craig",
-        [Segment("ERC", ["10", "Name: Craig"])],
+        [Segment("UNA",":+,? '"),Segment("ERC", ["10", "Name: Craig"])],
     )
 
 
 def test_escape_data_separator(parser, default_una_segment):
 
     _assert_segments(
         parser,
         default_una_segment,
         "DTM+735:?+0000:406",
-        [Segment("DTM", ["735", "+0000", "406"])],
+        [Segment("UNA",":+,? '"),Segment("DTM", ["735", "+0000", "406"])],
     )
 
 
 def test_escape_decimal_point(parser, default_una_segment):
 
     _assert_segments(
         parser,
         default_una_segment,
         "QTY+136:12,235",
-        [Segment("QTY", ["136", "12,235"])],
+        [Segment("UNA",":+,? '"),Segment("QTY", ["136", "12,235"])],
     )
 
 
 def test_escape_segment_terminator(parser, default_una_segment):
 
     _assert_segments(
         parser,
         default_una_segment,
         "ERC+10:Craig?'s",
-        [Segment("ERC", ["10", "Craig's"])],
+        [Segment("UNA",":+,? '"),Segment("ERC", ["10", "Craig's"])],
     )
 
 
 def test_escape_sequence(parser, default_una_segment):
 
     _assert_segments(
         parser,
         default_una_segment,
         "ERC+10:?:?+???' - ?:?+???' - ?:?+???'",
-        [Segment("ERC", ["10", ":+?' - :+?' - :+?'"])],
+        [Segment("UNA",":+,? '"),Segment("ERC", ["10", ":+?' - :+?' - :+?'"])],
     )
 
 
 def test_compound_starts_with_skipped(parser, default_una_segment):
 
     _assert_segments(
-        parser, default_una_segment, "IMD+::A", [Segment("IMD", ["", "", "A"])]
+        parser, default_una_segment, "IMD+::A", [Segment("UNA",":+,? '"),Segment("IMD", ["", "", "A"])]
     )
 
 
 def test_compound_contains_one_skipped(parser, default_una_segment):
 
     _assert_segments(
-        parser, default_una_segment, "IMD+A::B", [Segment("IMD", ["A", "", "B"])]
+        parser, default_una_segment, "IMD+A::B", [Segment("UNA",":+,? '"),Segment("IMD", ["A", "", "B"])]
     )
 
 
 def test_compound_contains_two_skipped(parser, default_una_segment):
 
     _assert_segments(
-        parser, default_una_segment, "IMD+A:::B", [Segment("IMD", ["A", "", "", "B"])]
+        parser, default_una_segment, "IMD+A:::B", [Segment("UNA",":+,? '"),Segment("IMD", ["A", "", "", "B"])]
     )
```

### Comparing `pydifact-0.1.5/tests/test_segment.py` & `pydifact-0.1.6/tests/test_segment.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU Lesser General Public License for more details.
 #
 #    You should have received a copy of the GNU Lesser General Public License
 #    along with this program.  If not, see <http://www.gnu.org/licenses/>.
 import pytest
 
-from pydifact.segments import Segment
+from pydifact.segments import Segment, SegmentProvider
 
 
 elements = ["field1", ["field2", "extra"], "stuff"]
 
 
 def test_get_segment_code():
     segment = Segment("OMD")
@@ -41,7 +41,20 @@
     assert segment.elements[1] == ["field2", "extra"]
 
 
 def test_get_non_existing_element():
     segment = Segment("OMD", *elements)
     with pytest.raises(IndexError):
         segment.elements[7]
+
+
+def test_has_plugin():
+    class TestSegment(Segment):
+
+        tag = "TES"
+
+        __omitted__ = False
+
+        def validate(self) -> bool:
+            pass
+
+    assert TestSegment in SegmentProvider.plugins
```

### Comparing `pydifact-0.1.5/tests/test_segmentcollection.py` & `pydifact-0.1.6/tests/test_segmentcollection.py`

 * *Files 3% similar despite different names*

```diff
@@ -238,14 +238,36 @@
         "UNB+UNOC:1+1234+3333+200102:2212+42'"
         "UNH+42z42+PAORES:93:1:IA'"
         "UNT+2+42z42'"
         "UNZ+1+42'"
     )
 
 
+def test_interchange_with_una():
+    i = Interchange.from_str(
+        "UNA:+,? '"
+        "UNB+UNOC:1+1234+3333+200102:2212+42'"
+        "UNH+42z42+PAORES:93:1:IA'"
+        "UNT+2+42z42'"
+        "UNZ+1+42'"
+    )
+    assert i.has_una_segment
+
+
+def test_interchange_with_custom_character():
+    i = Interchange.from_str(
+        "UNA:+.? '"
+        "UNB+UNOC:1+1234+3333+200102:2212+42'"
+        "UNH+42z42+PAORES:93:1:IA'"
+        "UNT+2+42z42'"
+        "UNZ+1+42'"
+    )
+    assert i.characters.decimal_point == "."
+
+
 def test_faulty_interchange__UNH_not_closed():
     """creates a message with an opening UNH message, without closing UNT"""
     i = Interchange.from_str(
         "UNB+UNOC:1+1234+3333+200102:2212+42'" "UNH+42z42+PAORES:93:1:IA'" "UNZ+2+42'"
     )
 
     with pytest.raises(EDISyntaxError):
```

### Comparing `pydifact-0.1.5/tests/test_serializer.py` & `pydifact-0.1.6/tests/test_serializer.py`

 * *Files 13% similar despite different names*

```diff
@@ -72,14 +72,18 @@
     assert_segments(serializer, "RFF+PD:50515", [Segment("RFF", ["PD", "50515"])])
 
 
 def test_basic2(serializer):
     assert_segments(serializer, "RFF+PD+50515", [Segment("RFF", "PD", "50515")])
 
 
+def test_empty_segment(serializer):
+    assert_segments(serializer, "RFF+PD++50515", [Segment("RFF", "PD", None, "50515")])
+
+
 def test_with_una_in_segments(serializer):
     assert_segments(
         serializer,
         "RFF+PD+45761",
         [Segment("UNA", ":+,? '"), Segment("RFF", "PD", "45761")],
     )
 
@@ -121,7 +125,27 @@
 
 
 def test_no_mutation(serializer):
     segments1 = [Segment("ERC", [":+?'"])]
     segments2 = copy.deepcopy(segments1)
     serializer.serialize(segments1, with_una_header=True)
     assert segments1 == segments2
+
+
+@pytest.fixture
+def interchange_str():
+    return (
+        "UNB+UNOC:1+1234+3333+200102:2212+42'"
+        "UNH+42z42+PAORES:93:1:IA'"
+        "UNT+2+42z42'"
+        "UNZ+1+42'"
+    )
+
+
+def test_interchange_serialization_with_una(interchange_str):
+    i = Interchange.from_str("UNA:+.? '" + interchange_str)
+    assert i.serialize() == "UNA:+.? '" + interchange_str
+
+
+def test_interchange_serialization_with_out_una(interchange_str):
+    i = Interchange.from_str(interchange_str)
+    assert i.serialize() == interchange_str
```

### Comparing `pydifact-0.1.5/tests/test_token.py` & `pydifact-0.1.6/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `pydifact-0.1.5/tests/test_tokenizer.py` & `pydifact-0.1.6/tests/test_tokenizer.py`

 * *Files identical despite different names*

