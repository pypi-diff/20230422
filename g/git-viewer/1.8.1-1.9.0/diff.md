# Comparing `tmp/git-viewer-1.8.1.tar.gz` & `tmp/git-viewer-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-viewer-1.8.1.tar", last modified: Sun Sep 25 08:00:45 2022, max compression
+gzip compressed data, was "git-viewer-1.9.0.tar", last modified: Sun Oct  2 10:35:44 2022, max compression
```

## Comparing `git-viewer-1.8.1.tar` & `git-viewer-1.9.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-09-25 08:00:45.166089 git-viewer-1.8.1/
--rw-r--r--   0 user      (1000) user      (1000)      657 2022-01-05 09:25:02.000000 git-viewer-1.8.1/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)       52 2022-01-05 18:37:55.000000 git-viewer-1.8.1/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)      972 2022-09-25 08:00:45.166089 git-viewer-1.8.1/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      262 2022-01-05 19:27:16.000000 git-viewer-1.8.1/PYPI_README.md
--rw-r--r--   0 user      (1000) user      (1000)    15807 2022-08-06 15:08:26.000000 git-viewer-1.8.1/README.md
--rw-r--r--   0 user      (1000) user      (1000)      104 2022-01-07 07:56:25.000000 git-viewer-1.8.1/pyproject.toml
--rw-r--r--   0 user      (1000) user      (1000)      992 2022-09-25 08:00:45.170089 git-viewer-1.8.1/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      154 2022-01-07 07:56:25.000000 git-viewer-1.8.1/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-09-25 08:00:45.162089 git-viewer-1.8.1/src/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-09-25 08:00:45.166089 git-viewer-1.8.1/src/git_viewer/
--rw-r--r--   0 user      (1000) user      (1000)       80 2022-01-05 16:39:05.000000 git-viewer-1.8.1/src/git_viewer/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)       84 2022-01-05 09:25:02.000000 git-viewer-1.8.1/src/git_viewer/__main__.py
--rw-r--r--   0 user      (1000) user      (1000)     6245 2022-05-10 13:54:43.000000 git-viewer-1.8.1/src/git_viewer/api_commands.py
--rw-r--r--   0 user      (1000) user      (1000)     3383 2022-09-25 08:00:36.000000 git-viewer-1.8.1/src/git_viewer/api_subprocess.py
--rw-r--r--   0 user      (1000) user      (1000)     2724 2022-03-17 12:00:54.000000 git-viewer-1.8.1/src/git_viewer/check.py
--rw-r--r--   0 user      (1000) user      (1000)     5001 2022-01-05 09:25:02.000000 git-viewer-1.8.1/src/git_viewer/color_decoder.py
--rw-r--r--   0 user      (1000) user      (1000)    55989 2022-08-06 15:08:26.000000 git-viewer-1.8.1/src/git_viewer/commands.py
--rw-r--r--   0 user      (1000) user      (1000)     1041 2022-02-28 20:16:51.000000 git-viewer-1.8.1/src/git_viewer/diff.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-09-25 08:00:45.166089 git-viewer-1.8.1/src/git_viewer/doc/
--rw-r--r--   0 user      (1000) user      (1000)     3986 2022-01-05 09:25:02.000000 git-viewer-1.8.1/src/git_viewer/doc/command_template.py
--rw-r--r--   0 user      (1000) user      (1000)    12609 2022-08-06 15:08:26.000000 git-viewer-1.8.1/src/git_viewer/doc/intro.md
--rw-r--r--   0 user      (1000) user      (1000)        6 2022-09-25 08:00:36.000000 git-viewer-1.8.1/src/git_viewer/doc/version.txt
--rw-r--r--   0 user      (1000) user      (1000)       84 2022-01-05 16:39:05.000000 git-viewer-1.8.1/src/git_viewer/log.py
--rw-r--r--   0 user      (1000) user      (1000)   124630 2022-08-06 15:08:26.000000 git-viewer-1.8.1/src/git_viewer/main.py
--rw-r--r--   0 user      (1000) user      (1000)    42990 2022-09-25 08:00:36.000000 git-viewer-1.8.1/src/git_viewer/model.py
--rw-r--r--   0 user      (1000) user      (1000)      978 2022-01-05 09:25:02.000000 git-viewer-1.8.1/src/git_viewer/model_hints.py
--rw-r--r--   0 user      (1000) user      (1000)     3412 2022-01-05 09:25:02.000000 git-viewer-1.8.1/src/git_viewer/model_input_history.py
--rw-r--r--   0 user      (1000) user      (1000)    24921 2022-05-10 13:54:43.000000 git-viewer-1.8.1/src/git_viewer/settings.py
--rw-r--r--   0 user      (1000) user      (1000)     1254 2022-02-28 20:16:51.000000 git-viewer-1.8.1/src/git_viewer/show.py
--rw-r--r--   0 user      (1000) user      (1000)     1300 2022-01-05 09:25:02.000000 git-viewer-1.8.1/src/git_viewer/string_formatter.py
--rw-r--r--   0 user      (1000) user      (1000)     4312 2022-01-05 09:25:02.000000 git-viewer-1.8.1/src/git_viewer/urwid_color_encoder.py
--rw-r--r--   0 user      (1000) user      (1000)     2633 2022-01-05 09:25:02.000000 git-viewer-1.8.1/src/git_viewer/urwid_constants.py
--rw-r--r--   0 user      (1000) user      (1000)     1555 2022-01-05 09:25:02.000000 git-viewer-1.8.1/src/git_viewer/urwid_edit_with_history.py
--rw-r--r--   0 user      (1000) user      (1000)    10340 2022-01-05 09:25:02.000000 git-viewer-1.8.1/src/git_viewer/urwid_text_layout.py
--rw-r--r--   0 user      (1000) user      (1000)     8122 2022-01-07 12:42:28.000000 git-viewer-1.8.1/src/git_viewer/utils.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-09-25 08:00:45.166089 git-viewer-1.8.1/src/git_viewer.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      972 2022-09-25 08:00:45.000000 git-viewer-1.8.1/src/git_viewer.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1026 2022-09-25 08:00:45.000000 git-viewer-1.8.1/src/git_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2022-09-25 08:00:45.000000 git-viewer-1.8.1/src/git_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       99 2022-09-25 08:00:45.000000 git-viewer-1.8.1/src/git_viewer.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) user      (1000)       16 2022-09-25 08:00:45.000000 git-viewer-1.8.1/src/git_viewer.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       11 2022-09-25 08:00:45.000000 git-viewer-1.8.1/src/git_viewer.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1001)        0 2022-10-02 10:35:44.733801 git-viewer-1.9.0/
+-rw-r--r--   0 user      (1000) user      (1001)      657 2022-01-05 09:25:02.000000 git-viewer-1.9.0/LICENSE
+-rw-r--r--   0 user      (1000) user      (1001)       52 2022-01-05 18:37:55.000000 git-viewer-1.9.0/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1001)      972 2022-10-02 10:35:44.733801 git-viewer-1.9.0/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1001)      262 2022-01-05 19:27:16.000000 git-viewer-1.9.0/PYPI_README.md
+-rw-r--r--   0 user      (1000) user      (1001)    15915 2022-10-02 09:22:23.000000 git-viewer-1.9.0/README.md
+-rw-r--r--   0 user      (1000) user      (1001)      104 2022-01-07 07:56:25.000000 git-viewer-1.9.0/pyproject.toml
+-rw-r--r--   0 user      (1000) user      (1001)      992 2022-10-02 10:35:44.733801 git-viewer-1.9.0/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1001)      154 2022-01-07 07:56:25.000000 git-viewer-1.9.0/setup.py
+drwxr-xr-x   0 user      (1000) user      (1001)        0 2022-10-02 10:35:44.727134 git-viewer-1.9.0/src/
+drwxr-xr-x   0 user      (1000) user      (1001)        0 2022-10-02 10:35:44.733801 git-viewer-1.9.0/src/git_viewer/
+-rw-r--r--   0 user      (1000) user      (1001)       80 2022-01-05 16:39:05.000000 git-viewer-1.9.0/src/git_viewer/__init__.py
+-rw-r--r--   0 user      (1000) user      (1001)       84 2022-01-05 09:25:02.000000 git-viewer-1.9.0/src/git_viewer/__main__.py
+-rw-r--r--   0 user      (1000) user      (1001)     6245 2022-05-10 13:54:43.000000 git-viewer-1.9.0/src/git_viewer/api_commands.py
+-rw-r--r--   0 user      (1000) user      (1001)     3383 2022-09-25 08:00:36.000000 git-viewer-1.9.0/src/git_viewer/api_subprocess.py
+-rw-r--r--   0 user      (1000) user      (1001)     2763 2022-10-02 09:22:23.000000 git-viewer-1.9.0/src/git_viewer/check.py
+-rw-r--r--   0 user      (1000) user      (1001)     5001 2022-01-05 09:25:02.000000 git-viewer-1.9.0/src/git_viewer/color_decoder.py
+-rw-r--r--   0 user      (1000) user      (1001)    55989 2022-08-06 15:08:26.000000 git-viewer-1.9.0/src/git_viewer/commands.py
+-rw-r--r--   0 user      (1000) user      (1001)     1107 2022-10-02 09:22:23.000000 git-viewer-1.9.0/src/git_viewer/diff.py
+drwxr-xr-x   0 user      (1000) user      (1001)        0 2022-10-02 10:35:44.733801 git-viewer-1.9.0/src/git_viewer/doc/
+-rw-r--r--   0 user      (1000) user      (1001)     3986 2022-01-05 09:25:02.000000 git-viewer-1.9.0/src/git_viewer/doc/command_template.py
+-rw-r--r--   0 user      (1000) user      (1001)    12609 2022-08-06 15:08:26.000000 git-viewer-1.9.0/src/git_viewer/doc/intro.md
+-rw-r--r--   0 user      (1000) user      (1001)        6 2022-10-02 09:23:16.000000 git-viewer-1.9.0/src/git_viewer/doc/version.txt
+-rw-r--r--   0 user      (1000) user      (1001)       84 2022-01-05 16:39:05.000000 git-viewer-1.9.0/src/git_viewer/log.py
+-rw-r--r--   0 user      (1000) user      (1001)   124982 2022-10-02 09:22:23.000000 git-viewer-1.9.0/src/git_viewer/main.py
+-rw-r--r--   0 user      (1000) user      (1001)    44267 2022-10-02 09:22:23.000000 git-viewer-1.9.0/src/git_viewer/model.py
+-rw-r--r--   0 user      (1000) user      (1001)      978 2022-01-05 09:25:02.000000 git-viewer-1.9.0/src/git_viewer/model_hints.py
+-rw-r--r--   0 user      (1000) user      (1001)     3412 2022-01-05 09:25:02.000000 git-viewer-1.9.0/src/git_viewer/model_input_history.py
+-rw-r--r--   0 user      (1000) user      (1001)    24921 2022-05-10 13:54:43.000000 git-viewer-1.9.0/src/git_viewer/settings.py
+-rw-r--r--   0 user      (1000) user      (1001)     1254 2022-02-28 20:16:51.000000 git-viewer-1.9.0/src/git_viewer/show.py
+-rw-r--r--   0 user      (1000) user      (1001)     1300 2022-01-05 09:25:02.000000 git-viewer-1.9.0/src/git_viewer/string_formatter.py
+-rw-r--r--   0 user      (1000) user      (1001)     4312 2022-01-05 09:25:02.000000 git-viewer-1.9.0/src/git_viewer/urwid_color_encoder.py
+-rw-r--r--   0 user      (1000) user      (1001)     2633 2022-01-05 09:25:02.000000 git-viewer-1.9.0/src/git_viewer/urwid_constants.py
+-rw-r--r--   0 user      (1000) user      (1001)     1555 2022-01-05 09:25:02.000000 git-viewer-1.9.0/src/git_viewer/urwid_edit_with_history.py
+-rw-r--r--   0 user      (1000) user      (1001)    10340 2022-01-05 09:25:02.000000 git-viewer-1.9.0/src/git_viewer/urwid_text_layout.py
+-rw-r--r--   0 user      (1000) user      (1001)     8122 2022-01-07 12:42:28.000000 git-viewer-1.9.0/src/git_viewer/utils.py
+drwxr-xr-x   0 user      (1000) user      (1001)        0 2022-10-02 10:35:44.733801 git-viewer-1.9.0/src/git_viewer.egg-info/
+-rw-r--r--   0 user      (1000) user      (1001)      972 2022-10-02 10:35:44.000000 git-viewer-1.9.0/src/git_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1001)     1026 2022-10-02 10:35:44.000000 git-viewer-1.9.0/src/git_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1001)        1 2022-10-02 10:35:44.000000 git-viewer-1.9.0/src/git_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1001)       99 2022-10-02 10:35:44.000000 git-viewer-1.9.0/src/git_viewer.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1000) user      (1001)       16 2022-10-02 10:35:44.000000 git-viewer-1.9.0/src/git_viewer.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1001)       11 2022-10-02 10:35:44.000000 git-viewer-1.9.0/src/git_viewer.egg-info/top_level.txt
```

### Comparing `git-viewer-1.8.1/LICENSE` & `git-viewer-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `git-viewer-1.8.1/PKG-INFO` & `git-viewer-1.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-viewer
-Version: 1.8.1
+Version: 1.9.0
 Summary: An interactive git viewer based on urwid. Similar to gitk but in a terminal.
 Home-page: https://gitlab.com/erzo/git-viewer
 Author: erzo
 Author-email: erzo@posteo.de
 Project-URL: Bug Tracker, https://gitlab.com/erzo/git-viewer/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `git-viewer-1.8.1/README.md` & `git-viewer-1.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 Advantages over `git log`/`git diff`:
 
 - interactively select a commit and look into it without needing to copy and paste a hash
 - hash ids are recognized as links which you can follow
 - separators between different files in diff for a better overview
 - easy copy of different information via keyboard (requires `wl-copy`, `xclip` or `xsel`)
 - line numbers in front of changed lines
+- special characters in file names are decoded (instead of displayed as three digit octal escape sequences)
 
 Why not use [tig](https://jonas.github.io/tig/)?
 
 Well, if I had known about tig I probably would have never started this project.
 It appears to be a pretty powerful and well documented program.
 However, git-viewer has a few features that I have not seen in tig.
 Some of them can probably be added via configuration, some of them maybe not.
```

### Comparing `git-viewer-1.8.1/setup.cfg` & `git-viewer-1.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `git-viewer-1.8.1/src/git_viewer/api_commands.py` & `git-viewer-1.9.0/src/git_viewer/api_commands.py`

 * *Files identical despite different names*

### Comparing `git-viewer-1.8.1/src/git_viewer/api_subprocess.py` & `git-viewer-1.9.0/src/git_viewer/api_subprocess.py`

 * *Files identical despite different names*

### Comparing `git-viewer-1.8.1/src/git_viewer/check.py` & `git-viewer-1.9.0/src/git_viewer/check.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,15 +90,16 @@
 	sys.stderr.write("\n")
 
 def error(error_number, error_message):
 	sys.stderr.write(error_message)
 	sys.stderr.write("\n")
 	exit(error_number)
 
-def run_all_checks():
+def run_all_checks(ignore_repo=False):
 	assert_python_new_enough()
-	assert_git_repo()
+	if not ignore_repo:
+		assert_git_repo()
 	check_urwid_version()
 
 
 if __name__ == '__main__':
 	run_all_checks()
```

### Comparing `git-viewer-1.8.1/src/git_viewer/color_decoder.py` & `git-viewer-1.9.0/src/git_viewer/color_decoder.py`

 * *Files identical despite different names*

### Comparing `git-viewer-1.8.1/src/git_viewer/commands.py` & `git-viewer-1.9.0/src/git_viewer/commands.py`

 * *Files identical despite different names*

### Comparing `git-viewer-1.8.1/src/git_viewer/doc/command_template.py` & `git-viewer-1.9.0/src/git_viewer/doc/command_template.py`

 * *Files identical despite different names*

### Comparing `git-viewer-1.8.1/src/git_viewer/doc/intro.md` & `git-viewer-1.9.0/src/git_viewer/doc/intro.md`

 * *Files identical despite different names*

### Comparing `git-viewer-1.8.1/src/git_viewer/main.py` & `git-viewer-1.9.0/src/git_viewer/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1676,22 +1676,22 @@
 	iter_commandmap_keys = staticmethod(iter_commandmap_keys)
 	iter_commandmap_items = staticmethod(iter_commandmap_items)
 	clear_commandmap = staticmethod(clear_commandmap)
 
 
 	# ------- app.init -------
 
-	def __init__(self, diff=None, show=None, show_unreachable=False, log_args=[], unreachable_args=[], diff_args=[], config_file=None, command_pipe=None, open_always=False):
+	def __init__(self, diff=None, show=None, show_unreachable=False, log_args=[], unreachable_args=[], diff_args=[], config_file=None, command_pipe=None, open_always=False, ignore_repo=False):
 		error = None
 		if open_always:
 			def on_error(error_number, error_message):
 				raise CheckError(error_number, error_message)
 			check.error = on_error
 		try:
-			check.run_all_checks()
+			check.run_all_checks(ignore_repo=ignore_repo)
 		except CheckError as e:
 			error = e
 
 		self._config_file = config_file
 		self.continue_running = False
 		self.state = self.STATE_BEFORE_INIT
 		self.messages = []
@@ -2406,15 +2406,15 @@
 		fn = self.parse_config_file_name(fn, prefer_existing=not ignore_existing, default_path=default_path)
 
 		if not os.path.exists(fn):
 			os.makedirs(os.path.split(fn)[0], exist_ok=True)
 			self.export_config(fn, comment_out=True)
 
 		def do():
-			model.open_file_in_editor(fn, line_number=None, create_dirs=True)
+			self.open_file_in_editor(fn, line_number=None, create_dirs=True)
 			if self.is_auto_reload_config_enabled:
 				self.load_config(fn)
 
 		self._run_external = do
 		self._reload_after_run_external = False
 		raise urwid.ExitMainLoop()
 
@@ -3042,34 +3042,41 @@
 				self.show_error(_("no file selected"))
 				return
 
 			commit = view.get_current_hash_id()[0]
 			if which == self.OPEN_NOW:
 				fn = model.get_relative_path(fn)
 				line_number = view.get_current_line_number(which)
-				self._run_external = lambda: model.open_file_in_editor(fn, line_number=line_number)
+				self._run_external = lambda: self.open_file_in_editor(fn, line_number=line_number)
 				self._reload_after_run_external = commit == self.ID_UNSTAGED
 			else:
 				if commit in (self.ID_UNSTAGED, self.ID_UNTRACKED) and which == self.OPEN_AFTER:
 					fn = model.get_relative_path(fn)
 					line_number = view.get_current_line_number(which)
-					self._run_external = lambda: model.open_file_in_editor(fn, line_number=line_number, read_only=True)
+					self._run_external = lambda: self.open_file_in_editor(fn, line_number=line_number, read_only=True)
 					self._reload_after_run_external = False
 				else:
 					object_id = view.get_current_object_id(which)
 					if object_id is None:
 						self.show_error(_("I have no object id for the version {which}").format(which=which))
 						return
 					line_number = view.get_current_line_number(which)
 					self._run_external = lambda: model.open_old_version_in_editor(fn, commit, object_id, which, line_number=line_number)
 					self._reload_after_run_external = False
 			raise urwid.ExitMainLoop()
 		else:
 			self.show_error(_("open is only implemented for details view"))
 
+	def open_file_in_editor(self, fn, line_number, read_only=False, create_dirs=False):
+		if os.path.exists(fn):
+			model.open_file_in_editor(fn, line_number, read_only=read_only, create_dirs=create_dirs)
+		else:
+			self.show_error('file %s does not exist, maybe decryption of special characters has failed' % fn)
+
+
 	def run_external_if_requested(self):
 		if self._run_external:
 			self._run_external()
 			self._run_external = None
 			self.continue_running = True
 			if self.is_auto_open_enabled and self._reload_after_run_external:
 				self.reload()
```

### Comparing `git-viewer-1.8.1/src/git_viewer/model.py` & `git-viewer-1.9.0/src/git_viewer/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,19 @@
 
 # ---------- model classes ----------
 
 class NameSpace:
 	pass
 
 class FileInfo:
-	__slots__ = ('fn', 'object_id_before_left', 'object_id_before_right', 'object_id_after')
+
+	# original_fn: the file name as printed by git, with special characters encoded as three digit octal numbers
+	# fn: the real file name
+
+	__slots__ = ('fn', 'original_fn', 'object_id_before_left', 'object_id_before_right', 'object_id_after')
 
 	def __init__(self, fn=None):
 		self.fn = fn
 		self.object_id_before_left = None
 		self.object_id_before_right = None
 		self.object_id_after = None
 
@@ -652,16 +656,18 @@
 	linenumber_sep = " "
 	linenumber_off = ""
 	linenumber_suffix = " "
 	linenumber = linenumber_new
 	min_line_number_width = 3
 
 	re_ansi_esscape_sequence = "(\[[0-9;]*m)?"
-	reo_start_new_file = re.compile(re_ansi_esscape_sequence + "diff (--git a/(?P<fn1>.*?) b/|--cc (?P<fn2>[^]*)|--combined (?P<fn3>[^]*))")
+	reo_start_new_file = re.compile(re_ansi_esscape_sequence + "diff (--git \"?a/(?P<fn1>.*?)\"? \"?b/|--cc \"?(?P<fn2>[^\"]*)\"?|--combined \"?(?P<fn3>[^\"]*))")
+	reo_escape = re.compile(r'(\\[0-7][0-7][0-7])+')
 	reo_object_id = re.compile(re_ansi_esscape_sequence + "index ((?P<beforeleft>[0-9a-f]+),)?(?P<before>[0-9a-f]+)\.\.(?P<after>[0-9a-f]+)")
+	reo_filename = re.compile(re_ansi_esscape_sequence + "(\+\+\+|---) ")
 	reo_linenumber = re.compile(re_ansi_esscape_sequence +
 		r"(@@@ -(?P<start_before_left>\d+)(,(?P<number_before_left>\d+))? -(?P<start_before_right>\d+)(,(?P<number_before_right>\d+))?"
 		r"|@@ -(?P<start_before>\d+)(,(?P<number_before>\d+))?) "
 		r"\+(?P<start_after>\d+)(,(?P<number_after>\d+))? @@"
 	)
 	reo_normal_line_exists_after = re.compile(re_ansi_esscape_sequence + r"[+ ]")
 	reo_normal_line_existed_before = re.compile(re_ansi_esscape_sequence + r"[- ]")
@@ -784,14 +790,22 @@
 		return out
 
 	def format_untracked(self, pattern, filenames):
 		path = lambda x: x
 		if self.cmd_untracked == ['$untracked']:
 			if self.untracked_relative == settings.RELATIVE_CWD:
 				path = os.path.abspath
+
+		for i in range(len(filenames)):
+			fn = filenames[i]
+			if fn.startswith('"') and fn.endswith('"'):
+				fn = fn[1:-1]
+			fn = self.decode_filename(fn)
+			filenames[i] = fn
+
 		return [([(settings.COLOR_DETAILS_UNTRACKED, utils.colored_str_to_markup(formatter.format(pattern, filename=fn), self.app.define_color))], TYPE_UNTRACKED, FileInfo(path(fn))) for fn in filenames]
 
 	def format_command_error(self, e, action=None, setting=None):
 		cmd = "cmd = %r\n" % (e.cmd,)
 		err = e.err
 		if action:
 			err += "\n" + _("while trying to {do_action}").format(do_action=action)
@@ -847,19 +861,24 @@
 			ns.look_for_hint = False
 		else:
 			m = self.reo_object_id.match(ln)
 			if m:
 				self.file_info.object_id_before_left = m.group('beforeleft')
 				self.file_info.object_id_before_right = m.group('before')
 				self.file_info.object_id_after = m.group('after')
+			elif self.reo_filename.match(ln):
+				if self.file_info.fn != self.file_info.original_fn:
+					ns.out[ns.i] = ns.out[ns.i].replace(self.file_info.original_fn, self.file_info.fn)
 
 
 		if self.insert_align_character:
-			ns.out[ns.i] = ALIGN_CHAR + ln
+			ns.out[ns.i] = ALIGN_CHAR + ns.out[ns.i]
 		if self.is_start_new_file(ln):
+			if self.file_info.fn != self.file_info.original_fn:
+				ns.out[ns.i] = ns.out[ns.i].replace(self.file_info.original_fn, self.file_info.fn)
 			ns.out[ns.i] = (ns.out[ns.i], TYPE_START_OF_FILE, self.file_info)
 
 	def _set_linenumber(self, ns, ns_name, match, re_name):
 		linenumber = match.group('start_'+re_name)
 		linenumber = int(linenumber)
 		number_lines = match.group('number_'+re_name)
 		if number_lines is None:
@@ -956,20 +975,43 @@
 		m = self.reo_start_new_file.match(ln)
 		if m:
 			fn = m.group('fn1')
 			if fn is None:
 				fn = m.group('fn2')
 				if fn is None:
 					fn = m.group('fn3')
+
+			original_fn = fn
+			fn = self.decode_filename(fn)
+
 			self.file_info = FileInfo()
 			self.file_info.fn = fn
+			self.file_info.original_fn = original_fn
+
 			return True
 		else:
 			return False
 
+	def decode_filename(self, fn: str) -> str:
+		def replace(m: re.Match) -> str:
+			original = m.group()
+			ls = original.split('\\')
+			assert ls[0] == ''
+			ls = ls[1:]
+			li = [int(n, base=8) for n in ls]
+			return bytes(li).decode()
+
+		if self.reo_escape.search(fn):
+			try:
+				fn = self.reo_escape.sub(replace, fn)
+			except unicodedecodeerror:
+				pass
+
+		return fn
+
 
 	# ------- command functions ------
 
 	def referencedby(self, args):
 		assert len(args) == 1
 		hash_id = args[0]
```

### Comparing `git-viewer-1.8.1/src/git_viewer/model_hints.py` & `git-viewer-1.9.0/src/git_viewer/model_hints.py`

 * *Files identical despite different names*

### Comparing `git-viewer-1.8.1/src/git_viewer/model_input_history.py` & `git-viewer-1.9.0/src/git_viewer/model_input_history.py`

 * *Files identical despite different names*

### Comparing `git-viewer-1.8.1/src/git_viewer/settings.py` & `git-viewer-1.9.0/src/git_viewer/settings.py`

 * *Files identical despite different names*

### Comparing `git-viewer-1.8.1/src/git_viewer/show.py` & `git-viewer-1.9.0/src/git_viewer/show.py`

 * *Files identical despite different names*

### Comparing `git-viewer-1.8.1/src/git_viewer/string_formatter.py` & `git-viewer-1.9.0/src/git_viewer/string_formatter.py`

 * *Files identical despite different names*

### Comparing `git-viewer-1.8.1/src/git_viewer/urwid_color_encoder.py` & `git-viewer-1.9.0/src/git_viewer/urwid_color_encoder.py`

 * *Files identical despite different names*

### Comparing `git-viewer-1.8.1/src/git_viewer/urwid_constants.py` & `git-viewer-1.9.0/src/git_viewer/urwid_constants.py`

 * *Files identical despite different names*

### Comparing `git-viewer-1.8.1/src/git_viewer/urwid_edit_with_history.py` & `git-viewer-1.9.0/src/git_viewer/urwid_edit_with_history.py`

 * *Files identical despite different names*

### Comparing `git-viewer-1.8.1/src/git_viewer/urwid_text_layout.py` & `git-viewer-1.9.0/src/git_viewer/urwid_text_layout.py`

 * *Files identical despite different names*

### Comparing `git-viewer-1.8.1/src/git_viewer/utils.py` & `git-viewer-1.9.0/src/git_viewer/utils.py`

 * *Files identical despite different names*

### Comparing `git-viewer-1.8.1/src/git_viewer.egg-info/PKG-INFO` & `git-viewer-1.9.0/src/git_viewer.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-viewer
-Version: 1.8.1
+Version: 1.9.0
 Summary: An interactive git viewer based on urwid. Similar to gitk but in a terminal.
 Home-page: https://gitlab.com/erzo/git-viewer
 Author: erzo
 Author-email: erzo@posteo.de
 Project-URL: Bug Tracker, https://gitlab.com/erzo/git-viewer/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `git-viewer-1.8.1/src/git_viewer.egg-info/SOURCES.txt` & `git-viewer-1.9.0/src/git_viewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

