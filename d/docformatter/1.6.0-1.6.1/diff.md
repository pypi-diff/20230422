# Comparing `tmp/docformatter-1.6.0.tar.gz` & `tmp/docformatter-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docformatter-1.6.0.tar", max compression
+gzip compressed data, was "docformatter-1.6.1.tar", max compression
```

## Comparing `docformatter-1.6.0.tar` & `docformatter-1.6.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1061 2022-07-29 13:50:28.414095 docformatter-1.6.0/LICENSE
--rw-r--r--   0        0        0     6497 2023-04-04 01:14:10.762053 docformatter-1.6.0/README.rst
--rw-r--r--   0        0        0     5618 2023-04-04 01:14:10.772053 docformatter-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     1539 2023-04-01 15:47:30.756410 docformatter-1.6.0/src/docformatter/__init__.py
--rwxr-xr-x   0        0        0     2555 2022-12-09 14:02:05.458355 docformatter-1.6.0/src/docformatter/__main__.py
--rw-r--r--   0        0        0     1191 2023-04-04 01:14:10.786054 docformatter-1.6.0/src/docformatter/__pkginfo__.py
--rw-r--r--   0        0        0    11411 2022-12-18 16:05:18.387285 docformatter-1.6.0/src/docformatter/configuration.py
--rw-r--r--   0        0        0     3642 2023-01-08 01:03:46.912729 docformatter-1.6.0/src/docformatter/encode.py
--rw-r--r--   0        0        0    19549 2023-04-04 01:14:10.798054 docformatter-1.6.0/src/docformatter/format.py
--rw-r--r--   0        0        0     5552 2023-04-04 01:14:10.812054 docformatter-1.6.0/src/docformatter/strings.py
--rw-r--r--   0        0        0    14823 2023-04-04 01:14:10.817054 docformatter-1.6.0/src/docformatter/syntax.py
--rw-r--r--   0        0        0     4572 2023-04-04 01:14:10.828054 docformatter-1.6.0/src/docformatter/util.py
--rw-r--r--   0        0        0     7714 1970-01-01 00:00:00.000000 docformatter-1.6.0/setup.py
--rw-r--r--   0        0        0     8158 1970-01-01 00:00:00.000000 docformatter-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2022-07-29 13:50:28.414095 docformatter-1.6.1/LICENSE
+-rw-r--r--   0        0        0     6497 2023-04-04 01:14:10.762053 docformatter-1.6.1/README.rst
+-rw-r--r--   0        0        0     5618 2023-04-21 18:35:01.605152 docformatter-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1539 2023-04-12 22:55:21.288454 docformatter-1.6.1/src/docformatter/__init__.py
+-rwxr-xr-x   0        0        0     2555 2023-04-12 22:55:21.294454 docformatter-1.6.1/src/docformatter/__main__.py
+-rw-r--r--   0        0        0     1191 2023-04-21 18:35:01.617152 docformatter-1.6.1/src/docformatter/__pkginfo__.py
+-rw-r--r--   0        0        0    11411 2023-04-12 22:55:21.304454 docformatter-1.6.1/src/docformatter/configuration.py
+-rw-r--r--   0        0        0     3654 2023-04-12 22:55:21.317454 docformatter-1.6.1/src/docformatter/encode.py
+-rw-r--r--   0        0        0    20483 2023-04-22 04:25:17.275941 docformatter-1.6.1/src/docformatter/format.py
+-rw-r--r--   0        0        0     5552 2023-04-12 22:55:21.317454 docformatter-1.6.1/src/docformatter/strings.py
+-rw-r--r--   0        0        0    14801 2023-04-12 22:55:21.318454 docformatter-1.6.1/src/docformatter/syntax.py
+-rw-r--r--   0        0        0     4572 2023-04-12 22:55:21.329455 docformatter-1.6.1/src/docformatter/util.py
+-rw-r--r--   0        0        0     7714 1970-01-01 00:00:00.000000 docformatter-1.6.1/setup.py
+-rw-r--r--   0        0        0     8158 1970-01-01 00:00:00.000000 docformatter-1.6.1/PKG-INFO
```

### Comparing `docformatter-1.6.0/LICENSE` & `docformatter-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `docformatter-1.6.0/README.rst` & `docformatter-1.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `docformatter-1.6.0/pyproject.toml` & `docformatter-1.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docformatter"
-version = "1.6.0"
+version = "1.6.1"
 description = "Formats docstrings to follow PEP 257"
 authors = ["Steven Myint"]
 maintainers = [
     "Doyle Rowland <doyle.rowland@reliaqual.com>",
 ]
 license = "Expat"
 readme = "README.rst"
```

### Comparing `docformatter-1.6.0/src/docformatter/__init__.py` & `docformatter-1.6.1/src/docformatter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 #
-# Copyright (C) 2012-2022 Steven Myint
+# Copyright (C) 2012-2023 Steven Myint
 #
 # Permission is hereby granted, free of charge, to any person obtaining
 # a copy of this software and associated documentation files (the
 # "Software"), to deal in the Software without restriction, including
 # without limitation the rights to use, copy, modify, merge, publish,
 # distribute, sublicense, and/or sell copies of the Software, and to
 # permit persons to whom the Software is furnished to do so, subject to
```

### Comparing `docformatter-1.6.0/src/docformatter/__main__.py` & `docformatter-1.6.1/src/docformatter/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 #
-# Copyright (C) 2012-2022 Steven Myint
+# Copyright (C) 2012-2023 Steven Myint
 #
 # Permission is hereby granted, free of charge, to any person obtaining
 # a copy of this software and associated documentation files (the
 # "Software"), to deal in the Software without restriction, including
 # without limitation the rights to use, copy, modify, merge, publish,
 # distribute, sublicense, and/or sell copies of the Software, and to
 # permit persons to whom the Software is furnished to do so, subject to
```

### Comparing `docformatter-1.6.0/src/docformatter/__pkginfo__.py` & `docformatter-1.6.1/src/docformatter/__pkginfo__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 #
-# Copyright (C) 2012-2022 Steven Myint
+# Copyright (C) 2012-2023 Steven Myint
 #
 # Permission is hereby granted, free of charge, to any person obtaining
 # a copy of this software and associated documentation files (the
 # "Software"), to deal in the Software without restriction, including
 # without limitation the rights to use, copy, modify, merge, publish,
 # distribute, sublicense, and/or sell copies of the Software, and to
 # permit persons to whom the Software is furnished to do so, subject to
@@ -19,8 +19,8 @@
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
 # BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
 # ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """Package information for docformatter."""
 
-__version__ = "1.6.0"
+__version__ = "1.6.1"
```

### Comparing `docformatter-1.6.0/src/docformatter/configuration.py` & `docformatter-1.6.1/src/docformatter/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 #
-# Copyright (C) 2012-2022 Steven Myint
+# Copyright (C) 2012-2023 Steven Myint
 #
 # Permission is hereby granted, free of charge, to any person obtaining
 # a copy of this software and associated documentation files (the
 # "Software"), to deal in the Software without restriction, including
 # without limitation the rights to use, copy, modify, merge, publish,
 # distribute, sublicense, and/or sell copies of the Software, and to
 # permit persons to whom the Software is furnished to do so, subject to
```

### Comparing `docformatter-1.6.0/src/docformatter/encode.py` & `docformatter-1.6.1/src/docformatter/encode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 #
-# Copyright (C) 2012-2022 Steven Myint
+# Copyright (C) 2012-2023 Steven Myint
 #
 # Permission is hereby granted, free of charge, to any person obtaining
 # a copy of this software and associated documentation files (the
 # "Software"), to deal in the Software without restriction, including
 # without limitation the rights to use, copy, modify, merge, publish,
 # distribute, sublicense, and/or sell copies of the Software, and to
 # permit persons to whom the Software is furnished to do so, subject to
@@ -24,15 +24,15 @@
 """This module provides docformatter's Encoder class."""
 
 # Standard Library Imports
 import collections
 import io
 import locale
 import sys
-from typing import Dict
+from typing import Dict, List
 
 # Third Party Imports
 from charset_normalizer import from_path  # pylint: disable=import-error
 
 unicode = str
 
 
@@ -63,15 +63,15 @@
 
             # Check for correctness of encoding.
             with self.do_open_with_encoding(filename) as check_file:
                 check_file.read()
         except (SyntaxError, LookupError, UnicodeDecodeError):
             self.encoding = "latin-1"
 
-    def do_find_newline(self, source: str) -> Dict[int, int]:
+    def do_find_newline(self, source: List[str]) -> Dict[int, int]:
         """Return type of newline used in source.
 
         Parameters
         ----------
         source : list
             A list of lines.
```

### Comparing `docformatter-1.6.0/src/docformatter/format.py` & `docformatter-1.6.1/src/docformatter/format.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 #
-# Copyright (C) 2012-2022 Steven Myint
+# Copyright (C) 2012-2023 Steven Myint
 #
 # Permission is hereby granted, free of charge, to any person obtaining
 # a copy of this software and associated documentation files (the
 # "Software"), to deal in the Software without restriction, including
 # without limitation the rights to use, copy, modify, merge, publish,
 # distribute, sublicense, and/or sell copies of the Software, and to
 # permit persons to whom the Software is furnished to do so, subject to
@@ -225,21 +225,21 @@
 
         Parameters
         ----------
         source: str
             The text from the source file.
         """
         try:
-            original_newline = self.encodor.do_find_newline(
+            _original_newline = self.encodor.do_find_newline(
                 source.splitlines(True)
             )
-            code = self._format_code(source)
+            _code = self._format_code(source)
 
             return _strings.normalize_line_endings(
-                code.splitlines(True), original_newline
+                _code.splitlines(True), _original_newline
             )
         except (tokenize.TokenError, IndentationError):
             return source
 
     def _format_code(
         self,
         source,
@@ -306,37 +306,24 @@
                     tokenize.COMMENT,
                     tokenize.NEWLINE,
                     tokenize.NL,
                 ]:
                     only_comments_so_far = False
 
                 previous_token_type = token_type
+                modified_tokens.append(
+                    (token_type, token_string, start, end, line)
+                )
 
-                # If the current token is a newline, the previous token was a
-                # newline or a comment, and these two sequential newlines
-                # follow a function or method definition, ignore the blank
-                # line before the docstring.
-                if (
-                    len(modified_tokens) <= 2
-                    or token_type not in {tokenize.NL, tokenize.NEWLINE}
-                    or modified_tokens[-1][0]
-                    not in {tokenize.NL, tokenize.NEWLINE}
-                    or modified_tokens[-2][1] != ":"
-                    and modified_tokens[-2][0] != tokenize.COMMENT
-                    or not modified_tokens[-2][4].lstrip().startswith(("def"))
-                ):
-                    modified_tokens.append(
-                        (token_type, token_string, start, end, line)
-                    )
-                    modified_tokens = self._do_remove_blank_lines_after_method(
-                        modified_tokens
-                    )
-                    modified_tokens = self._do_remove_blank_lines_before_class(
-                        modified_tokens
-                    )
+            modified_tokens = self._do_remove_blank_lines_after_definitions(
+                modified_tokens
+            )
+            modified_tokens = self._do_remove_blank_lines_after_docstring(
+                modified_tokens
+            )
 
             return untokenize.untokenize(modified_tokens)
         except tokenize.TokenError:
             return source
 
     def _do_format_docstring(
         self,
@@ -517,61 +504,106 @@
 {open_quote}{pre_summary}{summary}
 
 {description}{post_description}
 {indentation}"""\
 '''
 
     @staticmethod
-    def _do_remove_blank_lines_after_method(modified_tokens):
-        """Remove blank lines after method docstring.
+    def _do_remove_blank_lines_after_definitions(modified_tokens):
+        """Remove blank lines between definitions and docstrings.
+
+        Blank lines between class, method, function, and variable
+        definitions and the docstring will be removed.
 
         Parameters
         ----------
         modified_tokens: list
             The list of tokens created from the docstring.
 
         Returns
         -------
         modified_tokens: list
-            The list of tokens with any blank lines following a method
-            docstring removed.
+            The list of tokens with any blank lines following a variable
+            definition removed.
         """
-        with contextlib.suppress(IndexError):
-            if (
-                modified_tokens[-1][4] == "\n"
-                and modified_tokens[-2][4].lstrip().startswith('"""')
-                and modified_tokens[-5][4].lstrip().startswith("def")
-            ):
-                modified_tokens.pop(-1)
+        for _idx, _token in enumerate(modified_tokens):
+            if _token[0] == 3:
+                # Remove newline between variable definition and docstring.
+                j = 1
+                while modified_tokens[_idx - j][
+                    4
+                ] == "\n" and not modified_tokens[_idx - j - 1][
+                    4
+                ].strip().endswith(
+                    '"""'
+                ):
+                    modified_tokens.pop(_idx - j)
+                    j += 1
+
+                # Remove newline between class, method, and function
+                # definitions and docstring.
+                j = 2
+                while modified_tokens[_idx - j][4] == "\n" and modified_tokens[
+                    _idx - j - 2
+                ][4].strip().startswith(("def", "class")):
+                    modified_tokens.pop(_idx - j)
+                    j += 1
+
         return modified_tokens
 
     @staticmethod
-    def _do_remove_blank_lines_before_class(modified_tokens):
-        """Remove blank lines before class docstring.
-
-        If there is no class docstring, leave any blank lines as is.
+    def _do_remove_blank_lines_after_docstring(modified_tokens):
+        """Remove blank lines between docstring and first Python statement.
 
         Parameters
         ----------
         modified_tokens: list
             The list of tokens created from the docstring.
 
         Returns
         -------
         modified_tokens: list
-            The list of tokens with any blank lines following a method
-            docstring removed.
+            The list of tokens with any blank lines following a docstring
+            removed.
         """
-        with contextlib.suppress(IndexError):
-            if (
-                modified_tokens[-3][4] == "\n"
-                and modified_tokens[-2][4].lstrip().startswith('"""')
-                and modified_tokens[-6][4].lstrip().startswith("class")
-            ):
-                modified_tokens.pop(-3)
+        # Remove all newlines between docstring and first Python
+        # statement as long as it's not a stub function.
+        for _idx, _token in enumerate(modified_tokens):
+            with contextlib.suppress(IndexError):
+                _is_definition = (
+                    _token[4].lstrip().startswith(("class ", "def ", "@"))
+                )
+                _is_docstring = (
+                    modified_tokens[_idx - 2][4].strip().endswith('"""')
+                )
+                _after_definition = (
+                    modified_tokens[_idx - 6][4]
+                    .lstrip()
+                    .startswith(("class", "def", "@"))
+                )
+                _after_docstring = modified_tokens[_idx - 5][
+                    4
+                ].strip().endswith('"""') or modified_tokens[_idx - 5][
+                    4
+                ].strip().startswith(
+                    '"""'
+                )
+
+                if (
+                    _token[0] == 1
+                    and not _is_definition
+                    and not _is_docstring
+                    and _after_definition
+                    and _after_docstring
+                ):
+                    j = 1
+                    while modified_tokens[_idx - j][4] == "\n":
+                        modified_tokens.pop(_idx - j)
+                        j += 1
+
         return modified_tokens
 
     def _do_strip_docstring(self, docstring: str) -> Tuple[str, str]:
         """Return contents of docstring and opening quote type.
 
         Strips the docstring of its triple quotes, trailing white space,
         and line returns.  Determines type of docstring quote (either string,
```

### Comparing `docformatter-1.6.0/src/docformatter/strings.py` & `docformatter-1.6.1/src/docformatter/strings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 #
-# Copyright (C) 2012-2022 Steven Myint
+# Copyright (C) 2012-2023 Steven Myint
 #
 # Permission is hereby granted, free of charge, to any person obtaining
 # a copy of this software and associated documentation files (the
 # "Software"), to deal in the Software without restriction, including
 # without limitation the rights to use, copy, modify, merge, publish,
 # distribute, sublicense, and/or sell copies of the Software, and to
 # permit persons to whom the Software is furnished to do so, subject to
```

### Comparing `docformatter-1.6.0/src/docformatter/syntax.py` & `docformatter-1.6.1/src/docformatter/syntax.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,17 +321,15 @@
         # Skip URL if it is simply a quoted pattern.
         if do_skip_link(text, _idx):
             continue
 
         # If the text including the URL is longer than the wrap length,
         # we need to split the description before the URL, wrap the pre-URL
         # text, and add the URL as a separate line.
-        if len(text[_text_idx : _idx[1]]) > (
-            wrap_length - len(indentation)
-        ):
+        if len(text[_text_idx : _idx[1]]) > (wrap_length - len(indentation)):
             # Wrap everything in the description before the first URL.
             _lines.extend(
                 description_to_list(
                     text[_text_idx : _idx[0]],
                     indentation,
                     wrap_length,
                 )
```

### Comparing `docformatter-1.6.0/src/docformatter/util.py` & `docformatter-1.6.1/src/docformatter/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 #
-# Copyright (C) 2012-2022 Steven Myint
+# Copyright (C) 2012-2023 Steven Myint
 #
 # Permission is hereby granted, free of charge, to any person obtaining
 # a copy of this software and associated documentation files (the
 # "Software"), to deal in the Software without restriction, including
 # without limitation the rights to use, copy, modify, merge, publish,
 # distribute, sublicense, and/or sell copies of the Software, and to
 # permit persons to whom the Software is furnished to do so, subject to
```

### Comparing `docformatter-1.6.0/setup.py` & `docformatter-1.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 {'tomli': ['tomli>=2.0.0,<3.0.0']}
 
 entry_points = \
 {'console_scripts': ['docformatter = docformatter.__main__:main']}
 
 setup_kwargs = {
     'name': 'docformatter',
-    'version': '1.6.0',
+    'version': '1.6.1',
     'description': 'Formats docstrings to follow PEP 257',
     'long_description': '============\ndocformatter\n============\n\n.. |CI| image:: https://img.shields.io/github/actions/workflow/status/PyCQA/docformatter/ci.yml?branch=master\n    :target: https://github.com/PyCQA/docformatter/actions/workflows/ci.yml\n.. |COVERALLS| image:: https://img.shields.io/coveralls/github/PyCQA/docformatter\n    :target: https://coveralls.io/github/PyCQA/docformatter\n.. |CONTRIBUTORS| image:: https://img.shields.io/github/contributors/PyCQA/docformatter\n    :target: https://github.com/PyCQA/docformatter/graphs/contributors\n.. |COMMIT| image:: https://img.shields.io/github/last-commit/PyCQA/docformatter\n.. |BLACK| image:: https://img.shields.io/badge/%20style-black-000000.svg\n    :target: https://github.com/psf/black\n.. |ISORT| image:: https://img.shields.io/badge/%20imports-isort-%231674b1\n    :target: https://pycqa.github.io/isort/\n.. |SELF| image:: https://img.shields.io/badge/%20formatter-docformatter-fedcba.svg\n    :target: https://github.com/PyCQA/docformatter\n.. |SPHINXSTYLE| image:: https://img.shields.io/badge/%20style-sphinx-0a507a.svg\n    :target: https://www.sphinx-doc.org/en/master/usage/index.html\n.. |NUMPSTYLE| image:: https://img.shields.io/badge/%20style-numpy-459db9.svg\n    :target: https://numpydoc.readthedocs.io/en/latest/format.html\n.. |GOOGSTYLE| image:: https://img.shields.io/badge/%20style-google-3666d6.svg\n    :target: https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings\n\n.. |VERSION| image:: https://img.shields.io/pypi/v/docformatter\n.. |LICENSE| image:: https://img.shields.io/pypi/l/docformatter\n.. |PYVERS| image:: https://img.shields.io/pypi/pyversions/docformatter\n.. |PYMAT| image:: https://img.shields.io/pypi/format/docformatter\n.. |DD| image:: https://img.shields.io/pypi/dd/docformatter\n\n+----------------+----------------------------------------------------------+\n| **Code**       + |BLACK| |ISORT|                                          +\n+----------------+----------------------------------------------------------+\n| **Docstrings** + |SELF| |NUMPSTYLE|                                       +\n+----------------+----------------------------------------------------------+\n| **GitHub**     + |CI| |CONTRIBUTORS| |COMMIT|                             +\n+----------------+----------------------------------------------------------+\n| **PyPi**       + |VERSION| |LICENSE| |PYVERS| |PYMAT| |DD|                +\n+----------------+----------------------------------------------------------+\n\nFormats docstrings to follow `PEP 257`_.\n\n.. _`PEP 257`: http://www.python.org/dev/peps/pep-0257/\n\nFeatures\n========\n\n``docformatter`` automatically formats docstrings to follow a subset of the PEP\n257 conventions. Below are the relevant items quoted from PEP 257.\n\n- For consistency, always use triple double quotes around docstrings.\n- Triple quotes are used even though the string fits on one line.\n- Multi-line docstrings consist of a summary line just like a one-line\n  docstring, followed by a blank line, followed by a more elaborate\n  description.\n- Unless the entire docstring fits on a line, place the closing quotes\n  on a line by themselves.\n\n``docformatter`` also handles some of the PEP 8 conventions.\n\n- Don\'t write string literals that rely on significant trailing\n  whitespace. Such trailing whitespace is visually indistinguishable\n  and some editors (or more recently, reindent.py) will trim them.\n\nSee the the full documentation at `read-the-docs`_, especially the\n`requirements`_ section for a more detailed discussion of PEP 257 and other\nrequirements.\n\n.. _read-the-docs: https://docformatter.readthedocs.io\n.. _requirements: https://docformatter.readthedocs.io/en/latest/requirements.html\n\nInstallation\n============\n\nFrom pip::\n\n    $ pip install --upgrade docformatter\n\nOr, if you want to use pyproject.toml to configure docformatter::\n\n    $ pip install --upgrade docformatter[tomli]\n\nOr, if you want to use a release candidate (or any other tag)::\n\n    $ pip install git+https://github.com/PyCQA/docformatter.git@<RC_TAG>\n\nWhere <RC_TAG> is the release candidate tag you\'d like to install.  Release\ncandidate tags will have the format v1.6.0-rc1  Release candidates will also be\nmade available as a Github Release.\n\nExample\n=======\n\nAfter running::\n\n    $ docformatter --in-place example.py\n\nthis code\n\n.. code-block:: python\n\n    """   Here are some examples.\n\n        This module docstring should be dedented."""\n\n\n    def launch_rocket():\n        """Launch\n    the\n    rocket. Go colonize space."""\n\n\n    def factorial(x):\n        \'\'\'\n\n        Return x factorial.\n\n        This uses math.factorial.\n\n        \'\'\'\n        import math\n        return math.factorial(x)\n\n\n    def print_factorial(x):\n        """Print x factorial"""\n        print(factorial(x))\n\n\n    def main():\n        """Main\n        function"""\n        print_factorial(5)\n        if factorial(10):\n            launch_rocket()\n\n\ngets formatted into this\n\n.. code-block:: python\n\n    """Here are some examples.\n\n    This module docstring should be dedented.\n    """\n\n\n    def launch_rocket():\n        """Launch the rocket.\n\n        Go colonize space.\n        """\n\n\n    def factorial(x):\n        """Return x factorial.\n\n        This uses math.factorial.\n        """\n        import math\n        return math.factorial(x)\n\n\n    def print_factorial(x):\n        """Print x factorial."""\n        print(factorial(x))\n\n\n    def main():\n        """Main function."""\n        print_factorial(5)\n        if factorial(10):\n            launch_rocket()\n\nMarketing\n=========\nDo you use *docformatter*?  What style docstrings do you use?  Add some badges to your project\'s **README** and let everyone know.\n\n|SELF|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20formatter-docformatter-fedcba.svg\n        :target: https://github.com/PyCQA/docformatter\n\n|SPHINXSTYLE|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20style-sphinx-0a507a.svg\n        :target: https://www.sphinx-doc.org/en/master/usage/index.html\n\n|NUMPSTYLE|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20style-numpy-459db9.svg\n        :target: https://numpydoc.readthedocs.io/en/latest/format.html\n\n|GOOGSTYLE|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20style-google-3666d6.svg\n        :target: https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings\n\nIssues\n======\n\nBugs and patches can be reported on the `GitHub page`_.\n\n.. _`GitHub page`: https://github.com/PyCQA/docformatter/issues\n',
     'author': 'Steven Myint',
     'author_email': 'None',
     'maintainer': 'Doyle Rowland',
     'maintainer_email': 'doyle.rowland@reliaqual.com',
     'url': 'https://github.com/PyCQA/docformatter',
```

### Comparing `docformatter-1.6.0/PKG-INFO` & `docformatter-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docformatter
-Version: 1.6.0
+Version: 1.6.1
 Summary: Formats docstrings to follow PEP 257
 Home-page: https://github.com/PyCQA/docformatter
 License: Expat
 Keywords: PEP 257,pep257,style,formatter,docstrings
 Author: Steven Myint
 Maintainer: Doyle Rowland
 Maintainer-email: doyle.rowland@reliaqual.com
```

