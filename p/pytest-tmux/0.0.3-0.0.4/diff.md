# Comparing `tmp/pytest_tmux-0.0.3.tar.gz` & `tmp/pytest_tmux-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_tmux-0.0.3.tar", max compression
+gzip compressed data, was "pytest_tmux-0.0.4.tar", max compression
```

## Comparing `pytest_tmux-0.0.3.tar` & `pytest_tmux-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1067 2022-08-15 21:35:58.338604 pytest_tmux-0.0.3/LICENSE
--rw-r--r--   0        0        0     2830 2023-01-30 20:55:37.497567 pytest_tmux-0.0.3/README.md
--rw-r--r--   0        0        0     2114 2023-02-15 18:20:24.572294 pytest_tmux-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      141 2023-01-30 20:55:37.501567 pytest_tmux-0.0.3/pytest_tmux/__init__.py
--rw-r--r--   0        0        0    10769 2023-02-15 18:20:18.056275 pytest_tmux-0.0.3/pytest_tmux/client.py
--rw-r--r--   0        0        0    11072 2023-01-30 20:55:37.501567 pytest_tmux-0.0.3/pytest_tmux/config.py
--rw-r--r--   0        0        0     3055 2023-01-30 20:55:37.501567 pytest_tmux-0.0.3/pytest_tmux/fixtures.py
--rw-r--r--   0        0        0     2419 2023-01-30 20:55:37.501567 pytest_tmux-0.0.3/pytest_tmux/output.py
--rw-r--r--   0        0        0     4607 2023-01-30 20:55:37.501567 pytest_tmux-0.0.3/pytest_tmux/plugin.py
--rw-r--r--   0        0        0     1662 2023-01-30 20:55:37.501567 pytest_tmux-0.0.3/pytest_tmux/rewrite.py
--rw-r--r--   0        0        0     3733 1970-01-01 00:00:00.000000 pytest_tmux-0.0.3/setup.py
--rw-r--r--   0        0        0     4364 1970-01-01 00:00:00.000000 pytest_tmux-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-22 17:58:45.430197 pytest_tmux-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2831 2023-04-22 17:58:45.430197 pytest_tmux-0.0.4/README.md
+-rw-r--r--   0        0        0     2114 2023-04-22 17:59:23.866618 pytest_tmux-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      141 2023-04-22 17:58:45.430197 pytest_tmux-0.0.4/pytest_tmux/__init__.py
+-rw-r--r--   0        0        0    11232 2023-04-22 17:58:45.430197 pytest_tmux-0.0.4/pytest_tmux/client.py
+-rw-r--r--   0        0        0    11072 2023-04-22 17:58:45.430197 pytest_tmux-0.0.4/pytest_tmux/config.py
+-rw-r--r--   0        0        0     3055 2023-04-22 17:58:45.430197 pytest_tmux-0.0.4/pytest_tmux/fixtures.py
+-rw-r--r--   0        0        0     2419 2023-04-22 17:58:45.430197 pytest_tmux-0.0.4/pytest_tmux/output.py
+-rw-r--r--   0        0        0     4607 2023-04-22 17:58:45.430197 pytest_tmux-0.0.4/pytest_tmux/plugin.py
+-rw-r--r--   0        0        0     1662 2023-04-22 17:58:45.430197 pytest_tmux-0.0.4/pytest_tmux/rewrite.py
+-rw-r--r--   0        0        0     3734 1970-01-01 00:00:00.000000 pytest_tmux-0.0.4/setup.py
+-rw-r--r--   0        0        0     4365 1970-01-01 00:00:00.000000 pytest_tmux-0.0.4/PKG-INFO
```

### Comparing `pytest_tmux-0.0.3/LICENSE` & `pytest_tmux-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_tmux-0.0.3/README.md` & `pytest_tmux-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 [![PyPI version](https://img.shields.io/pypi/v/pytest-tmux.svg)](https://pypi.org/project/pytest-tmux)
 
 [![Python versions](https://img.shields.io/pypi/pyversions/pytest-tmux.svg)](https://pypi.org/project/pytest-tmux)
 
 A pytest plugin that enables tmux driven tests
 
-This plugin is intend to help users who whant to test interrative cli.
+This plugin is intend to help users who want to test interrative cli.
 
 When using `tmux` fixture it basically :
 
-- creates a tmux server (socket created in tmux tmpdir)
+- creates a tmux server (socket created in pytest tmpdir)
 - creates a session automatically
 - attach to the window automatically
 - attach to the pane automatically
 
 ## Warnings
 
 **Until a stable release, it is greatly encouraged to specify a strict version if
```

### Comparing `pytest_tmux-0.0.3/pyproject.toml` & `pytest_tmux-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-tmux"
-version = "0.0.3"
+version = "0.0.4"
 description = "A pytest plugin that enables tmux driven tests"
 authors = ["rockandska <yoann_mac_donald@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/rockandska/pytest-tmux"
 repository = "https://github.com/rockandska/pytest-tmux.git"
 documentation = "https://pytest-tmux.readthedocs.io"
```

### Comparing `pytest_tmux-0.0.3/pytest_tmux/client.py` & `pytest_tmux-0.0.4/pytest_tmux/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from inspect import cleandoc
 from typing import TYPE_CHECKING
 
 from libtmux.pane import Pane as TmuxPane
 from libtmux.server import Server as TmuxServer
+from pytest import exit as Exit
 
 from pytest_tmux.config import TmuxConfig
 from pytest_tmux.output import TmuxOutput
 
 if TYPE_CHECKING:
     from typing import Any, Dict, Optional, Union
 
@@ -56,14 +57,15 @@
     ) -> None:
         """State"""
         self._server = server
         self._session = None  # type: Optional[ libtmux.session.Session ]
         self._window = None  # type: Optional[ libtmux.window.Window ]
         self._pane = None  # type: Optional[ libtmux.pane.Pane ]
         self._debug = None  # type: Optional[ bool ]
+        self._interrupted = False
         self.sessions = 0
 
         if server is None and tmpdir_factory is None:
             raise ValueError("tmpdir_factory is requiered if server is not provided")
 
         """ Configuration """
         self._request = request
@@ -79,27 +81,31 @@
             tmpdir_factory=self._tmpdir_factory,
             server_cfg_fixture=self._server_cfg_fixture,
             session_cfg_fixture=self._session_cfg_fixture,
             assertion_cfg_fixture=self._assertion_cfg_fixture,
         )
 
     class suspend_capture:
-        def __init__(self, request: pytest.FixtureRequest) -> None:
+        def __init__(
+            self, request: pytest.FixtureRequest, interrupted: bool = False
+        ) -> None:
             self.capmanager = request.config.pluginmanager.getplugin("capturemanager")
+            self.interrupted = interrupted
 
         def __enter__(self) -> None:
             self.capmanager.suspend_global_capture(in_=True)
 
         def __exit__(self, _1: Any, _2: Any, _3: Any) -> None:
             try:
-                input("Press enter to continue....")
-            except KeyboardInterrupt:
-                self.capmanager.resume_global_capture()
+                if not self.interrupted:
+                    input("Press enter to continue....")
             except OSError:
                 pass
+            finally:
+                self.capmanager.resume_global_capture()
 
     def debug(self, msg: str) -> None:
         """
         Display a message and ask to press enter when pytest-tmux debug is
         activated.
 
         On first call, display a command who let the user been attached to the
@@ -108,47 +114,51 @@
         Args:
             msg:    The message to display
         """
         if TYPE_CHECKING:
             assert isinstance(self.config, TmuxConfig)
             assert isinstance(self.config.plugin, TmuxConfigPlugin)
         if self.config.plugin.debug:
-            if self._debug is None:
-                with self.suspend_capture(self._request):
-                    assert isinstance(self.pane, TmuxPane)
-                    print("")
-                    print("")
-                    print(
-                        cleandoc(
-                            """
-                        pytest-tmux started with DEBUG
-
-                        ****************************************************************************************
-                        * Open a new window terminal and use the bellow command to connect to the tmux session *
-                        ****************************************************************************************
-
-                        tmux -S "{}" attach -t "{}" \\; setw force-width {} \\; setw force-height {}
-
-                        """.format(
-                                self.server.socket_path,
-                                self.config.session.session_name,
-                                self.pane.display_message(
-                                    "#{window_width}", get_text=True
-                                )[0],
-                                self.pane.display_message(
-                                    "#{window_height}", get_text=True
-                                )[0],
+            try:
+                if self._debug is None:
+                    with self.suspend_capture(self._request):
+                        assert isinstance(self.pane, TmuxPane)
+                        print("")
+                        print("")
+                        print(
+                            cleandoc(
+                                """
+                            pytest-tmux started with DEBUG
+
+                            ****************************************************************************************
+                            * Open a new window terminal and use the bellow command to connect to the tmux session *
+                            ****************************************************************************************
+
+                            tmux -S "{}" attach -t "{}" \\; setw force-width {} \\; setw force-height {}
+
+                            """.format(
+                                    self.server.socket_path,
+                                    self.config.session.session_name,
+                                    self.pane.display_message(
+                                        "#{window_width}", get_text=True
+                                    )[0],
+                                    self.pane.display_message(
+                                        "#{window_height}", get_text=True
+                                    )[0],
+                                )
                             )
                         )
-                    )
+                        print("")
+                        self._debug = True
+                with self.suspend_capture(self._request, self._interrupted):
                     print("")
-                    self._debug = True
-            with self.suspend_capture(self._request):
-                print("")
-                print(cleandoc(msg))
+                    print(cleandoc(msg))
+            except KeyboardInterrupt:
+                self._interrupted = True
+                Exit("CTRL+C detected.")
 
     @property
     def session(self) -> libtmux.session.Session:
         """
         A direct link to libtmux.session.Session created for the actual test.
 
         The object is created on the first call who need it.
@@ -223,15 +233,15 @@
         """
         Send commands to the actual pane
 
         Args:
             cmd: Text or input into pane
             kwargs: every arguments accepted by libtmux.pane.Pane.send_keys()
         """
-        if "supress_history" not in kwargs:
+        if "suppress_history" not in kwargs:
             kwargs["suppress_history"] = False
         self.debug(
             """
                     Send "{}" to tmux session
                     """.format(
                 cmd
             )
```

### Comparing `pytest_tmux-0.0.3/pytest_tmux/config.py` & `pytest_tmux-0.0.4/pytest_tmux/config.py`

 * *Files identical despite different names*

### Comparing `pytest_tmux-0.0.3/pytest_tmux/fixtures.py` & `pytest_tmux-0.0.4/pytest_tmux/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest_tmux-0.0.3/pytest_tmux/output.py` & `pytest_tmux-0.0.4/pytest_tmux/output.py`

 * *Files identical despite different names*

### Comparing `pytest_tmux-0.0.3/pytest_tmux/plugin.py` & `pytest_tmux-0.0.4/pytest_tmux/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_tmux-0.0.3/pytest_tmux/rewrite.py` & `pytest_tmux-0.0.4/pytest_tmux/rewrite.py`

 * *Files identical despite different names*

### Comparing `pytest_tmux-0.0.3/setup.py` & `pytest_tmux-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['libtmux==0.20']
 
 entry_points = \
 {'pytest11': ['pytest-tmux = pytest_tmux.plugin']}
 
 setup_kwargs = {
     'name': 'pytest-tmux',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': 'A pytest plugin that enables tmux driven tests',
-    'long_description': '# pytest-tmux\n\n[![PyPI version](https://img.shields.io/pypi/v/pytest-tmux.svg)](https://pypi.org/project/pytest-tmux)\n\n[![Python versions](https://img.shields.io/pypi/pyversions/pytest-tmux.svg)](https://pypi.org/project/pytest-tmux)\n\nA pytest plugin that enables tmux driven tests\n\nThis plugin is intend to help users who whant to test interrative cli.\n\nWhen using `tmux` fixture it basically :\n\n- creates a tmux server (socket created in tmux tmpdir)\n- creates a session automatically\n- attach to the window automatically\n- attach to the pane automatically\n\n## Warnings\n\n**Until a stable release, it is greatly encouraged to specify a strict version if\nyou use this tool in your CI since it is in its early development and could be\ngreatly changed between version.**\n\n## Docs\n\n[https://pytest-tmux.readthedocs.io/](https://pytest-tmux.readthedocs.io)\n\n## Features\n\n- Enable tmux driven tests\n- Enable screen assertion with retry\n- Enable row assertion with retry\n- Allow to debug tests interactively\n\n## Requirements\n\n- python >= 3.7\n- pytest\n- tmux\n\n## Installation\n\nYou can install "pytest-tmux" via [pip](https://pypi.org/project/pip/)\nfrom [PyPI](https://pypi.org/project):\n\n    $ pip install pytest-tmux\n\n## Configuration capabilities\n\nConfiguration could be set on different level (in order of precedence):\n\n- Server\n    - by overriding tmux_server_config (scope=\'session\') fixture\n    - env var\n    - cli args (see --tmux-* switch with pytest --help)\n- Session\n    - by overriding tmux_session_config fixture\n    - at the test level with tmux_session_cfg marker\n    - dynamically inside test with `tmux.config.session`\n    - env var\n    - cli args (see --tmux-* switch with pytest --help)\n- Assertion\n    - by overriding tmux_assertion_config fixture\n    - at the test level with tmux_assertion_cfg marker\n    - dynamically inside test with `tmux.config.session`\n    - when calling `tmux.screen() / tmux.row()` with `timeout` / `delay` argument\n    - env var\n    - cli args (see --tmux-* switch with pytest --help)\n\n\n## Usage\n\n### Basic example\n\n```python\nimport pytest\nfrom inspect import cleandoc\n\ndef test_assert(tmux):\n    # Set some options before session / windows is started\n    tmux.config.session.window_command=\'env -i PS1="$ " TERM="xterm-256color" /usr/bin/env bash --norc --noprofile\'\n    assert tmux.screen() == \'$\'\n    tmux.send_keys(r\'printf "  Hello World  .\\n\\n"\')\n    expected=r"""\n    $ printf "  Hello World  .\\n\\n"\n      Hello World  .\n\n    $\n    """\n    assert tmux.screen() == cleandoc(expected)\n```\n\n## License\n\nDistributed under the terms of the\n[MIT](http://opensource.org/licenses/MIT) license, "pytest-tmux" is free\nand open source software\n\n## Issues\n\nIf you encounter any problems, please [file an\nissue](https://github.com/rockandska/pytest-tmux/issues) along with a\ndetailed description.\n',
+    'long_description': '# pytest-tmux\n\n[![PyPI version](https://img.shields.io/pypi/v/pytest-tmux.svg)](https://pypi.org/project/pytest-tmux)\n\n[![Python versions](https://img.shields.io/pypi/pyversions/pytest-tmux.svg)](https://pypi.org/project/pytest-tmux)\n\nA pytest plugin that enables tmux driven tests\n\nThis plugin is intend to help users who want to test interrative cli.\n\nWhen using `tmux` fixture it basically :\n\n- creates a tmux server (socket created in pytest tmpdir)\n- creates a session automatically\n- attach to the window automatically\n- attach to the pane automatically\n\n## Warnings\n\n**Until a stable release, it is greatly encouraged to specify a strict version if\nyou use this tool in your CI since it is in its early development and could be\ngreatly changed between version.**\n\n## Docs\n\n[https://pytest-tmux.readthedocs.io/](https://pytest-tmux.readthedocs.io)\n\n## Features\n\n- Enable tmux driven tests\n- Enable screen assertion with retry\n- Enable row assertion with retry\n- Allow to debug tests interactively\n\n## Requirements\n\n- python >= 3.7\n- pytest\n- tmux\n\n## Installation\n\nYou can install "pytest-tmux" via [pip](https://pypi.org/project/pip/)\nfrom [PyPI](https://pypi.org/project):\n\n    $ pip install pytest-tmux\n\n## Configuration capabilities\n\nConfiguration could be set on different level (in order of precedence):\n\n- Server\n    - by overriding tmux_server_config (scope=\'session\') fixture\n    - env var\n    - cli args (see --tmux-* switch with pytest --help)\n- Session\n    - by overriding tmux_session_config fixture\n    - at the test level with tmux_session_cfg marker\n    - dynamically inside test with `tmux.config.session`\n    - env var\n    - cli args (see --tmux-* switch with pytest --help)\n- Assertion\n    - by overriding tmux_assertion_config fixture\n    - at the test level with tmux_assertion_cfg marker\n    - dynamically inside test with `tmux.config.session`\n    - when calling `tmux.screen() / tmux.row()` with `timeout` / `delay` argument\n    - env var\n    - cli args (see --tmux-* switch with pytest --help)\n\n\n## Usage\n\n### Basic example\n\n```python\nimport pytest\nfrom inspect import cleandoc\n\ndef test_assert(tmux):\n    # Set some options before session / windows is started\n    tmux.config.session.window_command=\'env -i PS1="$ " TERM="xterm-256color" /usr/bin/env bash --norc --noprofile\'\n    assert tmux.screen() == \'$\'\n    tmux.send_keys(r\'printf "  Hello World  .\\n\\n"\')\n    expected=r"""\n    $ printf "  Hello World  .\\n\\n"\n      Hello World  .\n\n    $\n    """\n    assert tmux.screen() == cleandoc(expected)\n```\n\n## License\n\nDistributed under the terms of the\n[MIT](http://opensource.org/licenses/MIT) license, "pytest-tmux" is free\nand open source software\n\n## Issues\n\nIf you encounter any problems, please [file an\nissue](https://github.com/rockandska/pytest-tmux/issues) along with a\ndetailed description.\n',
     'author': 'rockandska',
     'author_email': 'yoann_mac_donald@hotmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/rockandska/pytest-tmux',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pytest_tmux-0.0.3/PKG-INFO` & `pytest_tmux-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-tmux
-Version: 0.0.3
+Version: 0.0.4
 Summary: A pytest plugin that enables tmux driven tests
 Home-page: https://github.com/rockandska/pytest-tmux
 License: MIT
 Author: rockandska
 Author-email: yoann_mac_donald@hotmail.com
 Requires-Python: >=3.7,<=3.11.9999
 Classifier: Development Status :: 4 - Beta
@@ -37,19 +37,19 @@
 
 [![PyPI version](https://img.shields.io/pypi/v/pytest-tmux.svg)](https://pypi.org/project/pytest-tmux)
 
 [![Python versions](https://img.shields.io/pypi/pyversions/pytest-tmux.svg)](https://pypi.org/project/pytest-tmux)
 
 A pytest plugin that enables tmux driven tests
 
-This plugin is intend to help users who whant to test interrative cli.
+This plugin is intend to help users who want to test interrative cli.
 
 When using `tmux` fixture it basically :
 
-- creates a tmux server (socket created in tmux tmpdir)
+- creates a tmux server (socket created in pytest tmpdir)
 - creates a session automatically
 - attach to the window automatically
 - attach to the pane automatically
 
 ## Warnings
 
 **Until a stable release, it is greatly encouraged to specify a strict version if
```

