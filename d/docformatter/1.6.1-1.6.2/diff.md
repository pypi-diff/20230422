# Comparing `tmp/docformatter-1.6.1.tar.gz` & `tmp/docformatter-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docformatter-1.6.1.tar", max compression
+gzip compressed data, was "docformatter-1.6.2.tar", max compression
```

## Comparing `docformatter-1.6.1.tar` & `docformatter-1.6.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1061 2022-07-29 13:50:28.414095 docformatter-1.6.1/LICENSE
--rw-r--r--   0        0        0     6497 2023-04-04 01:14:10.762053 docformatter-1.6.1/README.rst
--rw-r--r--   0        0        0     5618 2023-04-21 18:35:01.605152 docformatter-1.6.1/pyproject.toml
--rw-r--r--   0        0        0     1539 2023-04-12 22:55:21.288454 docformatter-1.6.1/src/docformatter/__init__.py
--rwxr-xr-x   0        0        0     2555 2023-04-12 22:55:21.294454 docformatter-1.6.1/src/docformatter/__main__.py
--rw-r--r--   0        0        0     1191 2023-04-21 18:35:01.617152 docformatter-1.6.1/src/docformatter/__pkginfo__.py
--rw-r--r--   0        0        0    11411 2023-04-12 22:55:21.304454 docformatter-1.6.1/src/docformatter/configuration.py
--rw-r--r--   0        0        0     3654 2023-04-12 22:55:21.317454 docformatter-1.6.1/src/docformatter/encode.py
--rw-r--r--   0        0        0    20483 2023-04-22 04:25:17.275941 docformatter-1.6.1/src/docformatter/format.py
--rw-r--r--   0        0        0     5552 2023-04-12 22:55:21.317454 docformatter-1.6.1/src/docformatter/strings.py
--rw-r--r--   0        0        0    14801 2023-04-12 22:55:21.318454 docformatter-1.6.1/src/docformatter/syntax.py
--rw-r--r--   0        0        0     4572 2023-04-12 22:55:21.329455 docformatter-1.6.1/src/docformatter/util.py
--rw-r--r--   0        0        0     7714 1970-01-01 00:00:00.000000 docformatter-1.6.1/setup.py
--rw-r--r--   0        0        0     8158 1970-01-01 00:00:00.000000 docformatter-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2022-07-29 13:50:28.414095 docformatter-1.6.2/LICENSE
+-rw-r--r--   0        0        0     6497 2023-04-04 01:14:10.762053 docformatter-1.6.2/README.rst
+-rw-r--r--   0        0        0     5618 2023-04-22 15:29:04.333625 docformatter-1.6.2/pyproject.toml
+-rw-r--r--   0        0        0     1539 2023-04-12 22:55:21.288454 docformatter-1.6.2/src/docformatter/__init__.py
+-rwxr-xr-x   0        0        0     2555 2023-04-12 22:55:21.294454 docformatter-1.6.2/src/docformatter/__main__.py
+-rw-r--r--   0        0        0     1191 2023-04-22 15:29:04.333625 docformatter-1.6.2/src/docformatter/__pkginfo__.py
+-rw-r--r--   0        0        0    11411 2023-04-12 22:55:21.304454 docformatter-1.6.2/src/docformatter/configuration.py
+-rw-r--r--   0        0        0     3654 2023-04-12 22:55:21.317454 docformatter-1.6.2/src/docformatter/encode.py
+-rw-r--r--   0        0        0    20665 2023-04-22 15:20:07.189864 docformatter-1.6.2/src/docformatter/format.py
+-rw-r--r--   0        0        0     5552 2023-04-12 22:55:21.317454 docformatter-1.6.2/src/docformatter/strings.py
+-rw-r--r--   0        0        0    14801 2023-04-12 22:55:21.318454 docformatter-1.6.2/src/docformatter/syntax.py
+-rw-r--r--   0        0        0     4572 2023-04-12 22:55:21.329455 docformatter-1.6.2/src/docformatter/util.py
+-rw-r--r--   0        0        0     7714 1970-01-01 00:00:00.000000 docformatter-1.6.2/setup.py
+-rw-r--r--   0        0        0     8158 1970-01-01 00:00:00.000000 docformatter-1.6.2/PKG-INFO
```

### Comparing `docformatter-1.6.1/LICENSE` & `docformatter-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `docformatter-1.6.1/README.rst` & `docformatter-1.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `docformatter-1.6.1/pyproject.toml` & `docformatter-1.6.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docformatter"
-version = "1.6.1"
+version = "1.6.2"
 description = "Formats docstrings to follow PEP 257"
 authors = ["Steven Myint"]
 maintainers = [
     "Doyle Rowland <doyle.rowland@reliaqual.com>",
 ]
 license = "Expat"
 readme = "README.rst"
```

### Comparing `docformatter-1.6.1/src/docformatter/__init__.py` & `docformatter-1.6.2/src/docformatter/__init__.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.6.1/src/docformatter/__main__.py` & `docformatter-1.6.2/src/docformatter/__main__.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.6.1/src/docformatter/__pkginfo__.py` & `docformatter-1.6.2/src/docformatter/__pkginfo__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
 # BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
 # ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """Package information for docformatter."""
 
-__version__ = "1.6.1"
+__version__ = "1.6.2"
```

### Comparing `docformatter-1.6.1/src/docformatter/configuration.py` & `docformatter-1.6.2/src/docformatter/configuration.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.6.1/src/docformatter/encode.py` & `docformatter-1.6.2/src/docformatter/encode.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.6.1/src/docformatter/format.py` & `docformatter-1.6.2/src/docformatter/format.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 
 # Standard Library Imports
 import argparse
 import collections
 import contextlib
 import io
+import re
 import tokenize
 from typing import TextIO, Tuple
 
 # Third Party Imports
 import untokenize
 
 # docformatter Package Imports
@@ -583,19 +584,23 @@
                 _after_docstring = modified_tokens[_idx - 5][
                     4
                 ].strip().endswith('"""') or modified_tokens[_idx - 5][
                     4
                 ].strip().startswith(
                     '"""'
                 )
+                _comment_follows = re.search(
+                    r"\"\"\" *#", modified_tokens[_idx - 4][4]
+                )
 
                 if (
                     _token[0] == 1
                     and not _is_definition
                     and not _is_docstring
+                    and not _comment_follows
                     and _after_definition
                     and _after_docstring
                 ):
                     j = 1
                     while modified_tokens[_idx - j][4] == "\n":
                         modified_tokens.pop(_idx - j)
                         j += 1
```

### Comparing `docformatter-1.6.1/src/docformatter/strings.py` & `docformatter-1.6.2/src/docformatter/strings.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.6.1/src/docformatter/syntax.py` & `docformatter-1.6.2/src/docformatter/syntax.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.6.1/src/docformatter/util.py` & `docformatter-1.6.2/src/docformatter/util.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.6.1/setup.py` & `docformatter-1.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 {'tomli': ['tomli>=2.0.0,<3.0.0']}
 
 entry_points = \
 {'console_scripts': ['docformatter = docformatter.__main__:main']}
 
 setup_kwargs = {
     'name': 'docformatter',
-    'version': '1.6.1',
+    'version': '1.6.2',
     'description': 'Formats docstrings to follow PEP 257',
     'long_description': '============\ndocformatter\n============\n\n.. |CI| image:: https://img.shields.io/github/actions/workflow/status/PyCQA/docformatter/ci.yml?branch=master\n    :target: https://github.com/PyCQA/docformatter/actions/workflows/ci.yml\n.. |COVERALLS| image:: https://img.shields.io/coveralls/github/PyCQA/docformatter\n    :target: https://coveralls.io/github/PyCQA/docformatter\n.. |CONTRIBUTORS| image:: https://img.shields.io/github/contributors/PyCQA/docformatter\n    :target: https://github.com/PyCQA/docformatter/graphs/contributors\n.. |COMMIT| image:: https://img.shields.io/github/last-commit/PyCQA/docformatter\n.. |BLACK| image:: https://img.shields.io/badge/%20style-black-000000.svg\n    :target: https://github.com/psf/black\n.. |ISORT| image:: https://img.shields.io/badge/%20imports-isort-%231674b1\n    :target: https://pycqa.github.io/isort/\n.. |SELF| image:: https://img.shields.io/badge/%20formatter-docformatter-fedcba.svg\n    :target: https://github.com/PyCQA/docformatter\n.. |SPHINXSTYLE| image:: https://img.shields.io/badge/%20style-sphinx-0a507a.svg\n    :target: https://www.sphinx-doc.org/en/master/usage/index.html\n.. |NUMPSTYLE| image:: https://img.shields.io/badge/%20style-numpy-459db9.svg\n    :target: https://numpydoc.readthedocs.io/en/latest/format.html\n.. |GOOGSTYLE| image:: https://img.shields.io/badge/%20style-google-3666d6.svg\n    :target: https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings\n\n.. |VERSION| image:: https://img.shields.io/pypi/v/docformatter\n.. |LICENSE| image:: https://img.shields.io/pypi/l/docformatter\n.. |PYVERS| image:: https://img.shields.io/pypi/pyversions/docformatter\n.. |PYMAT| image:: https://img.shields.io/pypi/format/docformatter\n.. |DD| image:: https://img.shields.io/pypi/dd/docformatter\n\n+----------------+----------------------------------------------------------+\n| **Code**       + |BLACK| |ISORT|                                          +\n+----------------+----------------------------------------------------------+\n| **Docstrings** + |SELF| |NUMPSTYLE|                                       +\n+----------------+----------------------------------------------------------+\n| **GitHub**     + |CI| |CONTRIBUTORS| |COMMIT|                             +\n+----------------+----------------------------------------------------------+\n| **PyPi**       + |VERSION| |LICENSE| |PYVERS| |PYMAT| |DD|                +\n+----------------+----------------------------------------------------------+\n\nFormats docstrings to follow `PEP 257`_.\n\n.. _`PEP 257`: http://www.python.org/dev/peps/pep-0257/\n\nFeatures\n========\n\n``docformatter`` automatically formats docstrings to follow a subset of the PEP\n257 conventions. Below are the relevant items quoted from PEP 257.\n\n- For consistency, always use triple double quotes around docstrings.\n- Triple quotes are used even though the string fits on one line.\n- Multi-line docstrings consist of a summary line just like a one-line\n  docstring, followed by a blank line, followed by a more elaborate\n  description.\n- Unless the entire docstring fits on a line, place the closing quotes\n  on a line by themselves.\n\n``docformatter`` also handles some of the PEP 8 conventions.\n\n- Don\'t write string literals that rely on significant trailing\n  whitespace. Such trailing whitespace is visually indistinguishable\n  and some editors (or more recently, reindent.py) will trim them.\n\nSee the the full documentation at `read-the-docs`_, especially the\n`requirements`_ section for a more detailed discussion of PEP 257 and other\nrequirements.\n\n.. _read-the-docs: https://docformatter.readthedocs.io\n.. _requirements: https://docformatter.readthedocs.io/en/latest/requirements.html\n\nInstallation\n============\n\nFrom pip::\n\n    $ pip install --upgrade docformatter\n\nOr, if you want to use pyproject.toml to configure docformatter::\n\n    $ pip install --upgrade docformatter[tomli]\n\nOr, if you want to use a release candidate (or any other tag)::\n\n    $ pip install git+https://github.com/PyCQA/docformatter.git@<RC_TAG>\n\nWhere <RC_TAG> is the release candidate tag you\'d like to install.  Release\ncandidate tags will have the format v1.6.0-rc1  Release candidates will also be\nmade available as a Github Release.\n\nExample\n=======\n\nAfter running::\n\n    $ docformatter --in-place example.py\n\nthis code\n\n.. code-block:: python\n\n    """   Here are some examples.\n\n        This module docstring should be dedented."""\n\n\n    def launch_rocket():\n        """Launch\n    the\n    rocket. Go colonize space."""\n\n\n    def factorial(x):\n        \'\'\'\n\n        Return x factorial.\n\n        This uses math.factorial.\n\n        \'\'\'\n        import math\n        return math.factorial(x)\n\n\n    def print_factorial(x):\n        """Print x factorial"""\n        print(factorial(x))\n\n\n    def main():\n        """Main\n        function"""\n        print_factorial(5)\n        if factorial(10):\n            launch_rocket()\n\n\ngets formatted into this\n\n.. code-block:: python\n\n    """Here are some examples.\n\n    This module docstring should be dedented.\n    """\n\n\n    def launch_rocket():\n        """Launch the rocket.\n\n        Go colonize space.\n        """\n\n\n    def factorial(x):\n        """Return x factorial.\n\n        This uses math.factorial.\n        """\n        import math\n        return math.factorial(x)\n\n\n    def print_factorial(x):\n        """Print x factorial."""\n        print(factorial(x))\n\n\n    def main():\n        """Main function."""\n        print_factorial(5)\n        if factorial(10):\n            launch_rocket()\n\nMarketing\n=========\nDo you use *docformatter*?  What style docstrings do you use?  Add some badges to your project\'s **README** and let everyone know.\n\n|SELF|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20formatter-docformatter-fedcba.svg\n        :target: https://github.com/PyCQA/docformatter\n\n|SPHINXSTYLE|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20style-sphinx-0a507a.svg\n        :target: https://www.sphinx-doc.org/en/master/usage/index.html\n\n|NUMPSTYLE|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20style-numpy-459db9.svg\n        :target: https://numpydoc.readthedocs.io/en/latest/format.html\n\n|GOOGSTYLE|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20style-google-3666d6.svg\n        :target: https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings\n\nIssues\n======\n\nBugs and patches can be reported on the `GitHub page`_.\n\n.. _`GitHub page`: https://github.com/PyCQA/docformatter/issues\n',
     'author': 'Steven Myint',
     'author_email': 'None',
     'maintainer': 'Doyle Rowland',
     'maintainer_email': 'doyle.rowland@reliaqual.com',
     'url': 'https://github.com/PyCQA/docformatter',
```

### Comparing `docformatter-1.6.1/PKG-INFO` & `docformatter-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docformatter
-Version: 1.6.1
+Version: 1.6.2
 Summary: Formats docstrings to follow PEP 257
 Home-page: https://github.com/PyCQA/docformatter
 License: Expat
 Keywords: PEP 257,pep257,style,formatter,docstrings
 Author: Steven Myint
 Maintainer: Doyle Rowland
 Maintainer-email: doyle.rowland@reliaqual.com
```

