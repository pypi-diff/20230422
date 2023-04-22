# Comparing `tmp/libtextworker-0.1.1.tar.gz` & `tmp/libtextworker-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libtextworker-0.1.1.tar", max compression
+gzip compressed data, was "libtextworker-0.1.2.tar", max compression
```

## Comparing `libtextworker-0.1.1.tar` & `libtextworker-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,25 @@
--rw-r--r--   0        0        0     1631 2023-04-02 15:13:53.044241 libtextworker-0.1.1/libtextworker/__init__.py
--rw-r--r--   0        0        0     1007 2023-04-03 15:26:31.417673 libtextworker-0.1.1/libtextworker/_importer.py
--rw-r--r--   0        0        0     3414 2023-04-03 14:59:35.112876 libtextworker-0.1.1/libtextworker/general.py
--rw-r--r--   0        0        0     6754 2023-03-26 10:23:15.258180 libtextworker-0.1.1/libtextworker/get_config.py
--rw-r--r--   0        0        0        0 2023-03-26 10:23:15.305089 libtextworker-0.1.1/libtextworker/interface/__init__.py
--rw-r--r--   0        0        0     7692 2023-04-02 14:41:13.695338 libtextworker-0.1.1/libtextworker/interface/manager.py
--rw-r--r--   0        0        0     3293 2023-04-03 15:26:15.366692 libtextworker-0.1.1/libtextworker/interface/tk/__init__.py
--rw-r--r--   0        0        0     4101 2023-04-03 15:26:31.609671 libtextworker-0.1.1/libtextworker/interface/tk/textwidget.py
--rw-r--r--   0        0        0     1324 2023-04-03 15:26:31.467671 libtextworker-0.1.1/libtextworker/interface/wx/__init__.py
--rw-r--r--   0        0        0     2456 2023-03-26 10:23:15.320662 libtextworker-0.1.1/libtextworker/interface/wx/about.py
--rw-r--r--   0        0        0      447 2023-04-02 12:22:42.692547 libtextworker-0.1.1/libtextworker/interface/wx/constants.py
--rw-r--r--   0        0        0     5415 2023-03-26 10:23:15.336287 libtextworker-0.1.1/libtextworker/interface/wx/editor.py
--rw-r--r--   0        0        0     2462 2023-03-26 10:23:15.336287 libtextworker-0.1.1/libtextworker/interface/wx/miscs.py
--rw-r--r--   0        0        0    35149 2023-03-26 10:23:15.351927 libtextworker-0.1.1/libtextworker/licenses/GPL3_full.txt
--rw-r--r--   0        0        0      615 2023-03-26 10:23:15.351927 libtextworker-0.1.1/libtextworker/licenses/GPL3_short.txt
--rw-r--r--   0        0        0     1022 2023-03-26 10:23:15.367547 libtextworker-0.1.1/libtextworker/licenses/MIT.txt
--rw-r--r--   0        0        0     2711 2023-04-02 14:41:13.663703 libtextworker-0.1.1/libtextworker/versioning.py
--rw-r--r--   0        0        0    35149 2023-03-26 10:23:15.180050 libtextworker-0.1.1/LICENSE
--rw-r--r--   0        0        0      848 2023-04-03 15:31:21.222892 libtextworker-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      289 2023-04-03 15:30:21.227291 libtextworker-0.1.1/README.md
--rw-r--r--   0        0        0     1421 1970-01-01 00:00:00.000000 libtextworker-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1631 2023-04-20 13:54:08.893198 libtextworker-0.1.2/libtextworker/__init__.py
+-rw-r--r--   0        0        0      491 2023-04-20 11:12:58.566224 libtextworker-0.1.2/libtextworker/_importer.py
+-rw-r--r--   0        0        0     3414 2023-04-20 11:12:43.928208 libtextworker-0.1.2/libtextworker/general.py
+-rw-r--r--   0        0        0     6256 2023-04-20 11:48:14.234327 libtextworker-0.1.2/libtextworker/get_config.py
+-rw-r--r--   0        0        0        0 2023-04-20 11:12:43.929209 libtextworker-0.1.2/libtextworker/interface/__init__.py
+-rw-r--r--   0        0        0     7655 2023-04-20 14:33:23.438003 libtextworker-0.1.2/libtextworker/interface/manager.py
+-rw-r--r--   0        0        0     3192 2023-04-20 11:12:58.568226 libtextworker-0.1.2/libtextworker/interface/tk/__init__.py
+-rw-r--r--   0        0        0     3988 2023-04-20 11:12:58.569224 libtextworker-0.1.2/libtextworker/interface/tk/editor.py
+-rw-r--r--   0        0        0     1956 2023-04-20 14:33:23.322004 libtextworker-0.1.2/libtextworker/interface/tk/miscs.py
+-rw-r--r--   0        0        0     1432 2023-04-20 14:33:23.328002 libtextworker-0.1.2/libtextworker/interface/wx/__init__.py
+-rw-r--r--   0        0        0     2776 2023-04-22 13:26:35.375215 libtextworker-0.1.2/libtextworker/interface/wx/about.py
+-rw-r--r--   0        0        0      447 2023-04-20 11:12:43.934208 libtextworker-0.1.2/libtextworker/interface/wx/constants.py
+-rw-r--r--   0        0        0     5304 2023-04-21 07:05:10.999353 libtextworker-0.1.2/libtextworker/interface/wx/editor.py
+-rw-r--r--   0        0        0     2462 2023-04-20 11:12:43.936208 libtextworker-0.1.2/libtextworker/interface/wx/miscs.py
+-rw-r--r--   0        0        0    35182 2023-04-22 13:23:35.882821 libtextworker-0.1.2/libtextworker/licenses/AGPL_full.txt
+-rw-r--r--   0        0        0      684 2023-04-22 13:21:40.443192 libtextworker-0.1.2/libtextworker/licenses/AGPL_short.txt
+-rw-r--r--   0        0        0    35149 2023-04-20 11:12:43.937207 libtextworker-0.1.2/libtextworker/licenses/GPL3_full.txt
+-rw-r--r--   0        0        0      615 2023-04-20 11:12:43.938208 libtextworker-0.1.2/libtextworker/licenses/GPL3_short.txt
+-rw-r--r--   0        0        0     7815 2023-04-22 13:20:16.073381 libtextworker-0.1.2/libtextworker/licenses/LGPL_3.txt
+-rw-r--r--   0        0        0     1022 2023-04-20 11:12:43.938208 libtextworker-0.1.2/libtextworker/licenses/MIT.txt
+-rw-r--r--   0        0        0     2711 2023-04-20 11:12:43.939207 libtextworker-0.1.2/libtextworker/versioning.py
+-rw-r--r--   0        0        0    35149 2023-04-20 11:12:43.922208 libtextworker-0.1.2/LICENSE
+-rw-r--r--   0        0        0      928 2023-04-20 11:44:44.226449 libtextworker-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      307 2023-04-22 14:49:50.996391 libtextworker-0.1.2/README.md
+-rw-r--r--   0        0        0     1522 1970-01-01 00:00:00.000000 libtextworker-0.1.2/PKG-INFO
```

### Comparing `libtextworker-0.1.1/libtextworker/__init__.py` & `libtextworker-0.1.2/libtextworker/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 gettext.textdomain(APPDOMAIN)
 gettext.install(APPDOMAIN, LOCALEDIR)
 
 # Module import tests
 Importable = _importer.Importable
 
 # Something else;-;
-__version__ = "0.1.0"
+__version__ = "0.1.2"
 THEMES_DIR = os.path.expanduser(
     "~/.config/textworker/themes/"
 )  ## Directory of *custom* themes
 EDITOR_DIR = os.path.expanduser(
     "~/.config/textworker/editorconfigs/"
 )  ## Directory of *editor configurations
```

### Comparing `libtextworker-0.1.1/libtextworker/general.py` & `libtextworker-0.1.2/libtextworker/general.py`

 * *Files identical despite different names*

### Comparing `libtextworker-0.1.1/libtextworker/get_config.py` & `libtextworker-0.1.2/libtextworker/get_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,28 +20,25 @@
             )
         full = prefix + msg
         super().__init__(full)
 
 
 class GetConfig(configparser.ConfigParser):
     # Values
-    yes_values: list = []
-    no_values: list = []
+    yes_values: list = ["yes", "True"]
+    no_values: list = ["no", "False"]
 
     returnbool: bool = True
     aliases = {}
     detailedlogs: bool = True
     backups = {}
 
-    # "Protected" properties
-    _yes_values = ["yes", "True"]
-    _no_values = ["no", "False"]
-
     def __init__(self, config: dict, file: str, **kwds):
-        """Customized configuration parser.
+        """
+        A customized INI file parser.
         @param config : Default configurations, used to reset the file or do some comparisions
         @param file : Configuration file
         @param **kwds : To pass to configparser.ConfigParser (base class)
 
         When initialized, GetConfig loads all default configs (from config param) and store it in
         a dictionary for further actions (backup/restore file).
         """
@@ -57,21 +54,15 @@
         self.__file = file
 
     # File tasks
     def readf(self, file: str, encoding: str | None = None):
         if os.path.isfile(file):
             self.read(file, encoding)
         else:
-            splits = file.split("/")
-            splits.pop()
-            # print(splits)
-            firstdir = splits[0]
-            for item in range(1, len(splits)):
-                firstdir += "/" + splits[item]
-            # print(firstdir)
+            firstdir = os.path.dirname(file)
             WalkCreation(firstdir)
             with open(file, mode="w") as f:
                 try:
                     self.write(f)
                 except OSError:
                     raise Exception("Unable to access to the file name %s" % file)
                 else:
@@ -170,20 +161,14 @@
                     return False
 
         if needed == True:
             self.update()
 
         value = self.get(section, option)
 
-        # if getbool == True:
-        #     if value in self.yes_values or self._yes_values:
-        #         return True
-        #     if value in self.no_values or self._no_values:
-        #         return False
-
         return value if value not in self.aliases else self.aliases[value]
 
     def aliasyesno(self, yesvalue, novalue, enable: bool = True) -> None:
         """
         Use a custom yes/no value, for example:
         There is an option under [section], and GetConfig will return
         True if the options is 'yes', False if the options is 'no'.
```

### Comparing `libtextworker-0.1.1/libtextworker/interface/manager.py` & `libtextworker-0.1.2/libtextworker/interface/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,15 @@
             "dark": "#1c1c1c",
         }
 
         ##
         resv = {"light": "dark", "dark": "light"}
 
         ## Check
-        if autocolor == True:
+        if autocolor == True or "yes":
             color_ = colors[_get_sys_mode()]
         elif color in colors:
             color_ = colors[color]
 
         # Text color
         colors["green"] = "#00ff00"
         colors["red"] = "#ff0000"
@@ -205,16 +205,15 @@
         @see setcolorfunc
         @see setfontcfunc
         """
         if not widget:
             print("Widget died, skip configuring.")
             return
 
-        widget.SetFont(self._get_font())
-        color, fontcolor = self._get_color()
+        color, fontcolor = self.GetColor
 
         for item in self.setfontfn:
             fn = self.setfontfn[item]["fn"]
             if not self.setfontfn[item]["params"]:
                 fn(fontcolor)
             else:
                 fn(self.setfontfn[item]["params"], fontcolor)
```

### Comparing `libtextworker-0.1.1/libtextworker/interface/tk/__init__.py` & `libtextworker-0.1.2/libtextworker/interface/tk/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-"""
-@package libtextworker.interface.tk
-Contains classes for Tkinter.
-"""
-import threading
-import typing
-from libtextworker import Importable
-from ..manager import ColorManager, default_configs
-
-if Importable["interface.tk"] == True:
-    import darkdetect
-    import sv_ttk
-    from tkinter import TclError, font, messagebox
-
-    pass
-else:
-    raise Exception(
-        "interface.tk is called but its dependency Tkinter is not installed"
-    )
-
-
-class ColorManager(ColorManager):
-    recursive_configure: bool = True
-    is_shown: bool = False  # Messages
-
-    def _get_font(self):
-        size, style, weight, family = super()._get_font()
-        font_families = font.families()
-
-        if family == "default":
-            family = "Consolas"
-        elif family not in font_families:
-            if not self.is_shown:
-                messagebox.showwarning(
-                    message=_(
-                        """
-                        It seemed that your preferred font family does not available on your machine here.\n
-                        Install the font first - and now the program will use Consolas instead.\n
-                        If you think that this is a mistake, please report it.
-                        """
-                    )
-                )
-                self.is_shown = True
-
-        if style == "normal" or style != "italic":
-            style = "roman"
-        return font.Font(None, family=family, weight=weight, slant=style, size=size)
-
-    def setfontcfunc(self, objname: str, func: typing.Callable, params: dict):
-        raise NotImplementedError
-
-    def setcolorfunc(self, objname: str, func: typing.Callable, params: dict):
-        raise NotImplementedError
-
-    def configure(self, widget: typing.Any, childs_too: bool = recursive_configure):
-        back, fore = self.GetColor
-        font_to_use = self.GetFont
-
-        try:
-            widget.configure(font=font_to_use)
-        except TclError:
-            pass
-
-        # Why this catch?
-        # Some Tkinter objects do not use fg and bg as their configure() keywords,
-        # but use foreground and background instead.
-        try:
-            widget.configure(fg=fore, bg=back)
-            widget.configure(foreground=fore, background=back)
-        except TclError:
-            pass
-
-        self.autocolor_run(widget)
-
-        if childs_too:
-            for child in widget.winfo_children():
-                self.configure(child, self.recursive_configure)
-                self.autocolor_run(child)
-
-    def autocolor_run(self, widget: typing.Any):
-        def _configure(theme: str):
-            sv_ttk.set_theme(theme.lower())
-            self.configure(widget)
-
-        if self.getkey("color", "autocolor") == True or "yes":
-            if widget not in self.threads or not self.threads[widget].is_alive():
-                self.threads[widget] = threading.Thread(
-                    target=darkdetect.listener, args=(_configure,), daemon=True
-                )
-                self.threads[widget].start()
-            sv_ttk.set_theme(
-                darkdetect.theme().lower()
-            )  # Keep this to avoid 'font already exists' error
-
-
-clrmgr = ColorManager(default_configs)
+"""
+@package libtextworker.interface.tk
+Contains classes for Tkinter.
+"""
+import threading
+import typing
+from libtextworker import Importable
+from ..manager import ColorManager, default_configs
+
+if Importable["tkinter"] == True:
+    import darkdetect
+    import sv_ttk
+    from tkinter import TclError, font, messagebox
+
+    pass
+else:
+    raise Exception(
+        "interface.tk is called but its dependency Tkinter is not installed"
+    )
+
+
+class ColorManager(ColorManager):
+    recursive_configure: bool = True
+    is_shown: bool = False  # Messages
+
+    def _get_font(self):
+        size, style, weight, family = super()._get_font()
+        font_families = font.families()
+
+        if family == "default":
+            family = "Consolas"
+        elif family not in font_families:
+            if not self.is_shown:
+                messagebox.showwarning(
+                    message=_(
+                        """
+                        It seemed that your preferred font family does not available on your machine here.\n
+                        Install the font first - and now the program will use Consolas instead.\n
+                        If you think that this is a mistake, please report it.
+                        """
+                    )
+                )
+                self.is_shown = True
+
+        if style == "normal" or style != "italic":
+            style = "roman"
+        return font.Font(None, family=family, weight=weight, slant=style, size=size)
+
+    def setfontcfunc(self, objname: str, func: typing.Callable, params: dict):
+        raise NotImplementedError
+
+    def setcolorfunc(self, objname: str, func: typing.Callable, params: dict):
+        raise NotImplementedError
+
+    def configure(self, widget: typing.Any, childs_too: bool = recursive_configure):
+        back, fore = self.GetColor
+        font_to_use = self.GetFont
+
+        try:
+            widget.configure(font=font_to_use)
+        except TclError:
+            pass
+
+        # Why this catch?
+        # Some Tkinter objects do not use fg and bg as their configure() keywords,
+        # but use foreground and background instead.
+        try:
+            widget.configure(fg=fore, bg=back)
+            widget.configure(foreground=fore, background=back)
+        except TclError:
+            pass
+
+        self.autocolor_run(widget)
+
+        if childs_too:
+            for child in widget.winfo_children():
+                self.configure(child, self.recursive_configure)
+                self.autocolor_run(child)
+
+    def autocolor_run(self, widget: typing.Any):
+        def _configure(theme: str):
+            sv_ttk.set_theme(theme.lower())
+            self.configure(widget)
+
+        if self.getkey("color", "autocolor") == True or "yes":
+            if widget not in self.threads or not self.threads[widget].is_alive():
+                self.threads[widget] = threading.Thread(
+                    target=darkdetect.listener, args=(_configure,), daemon=True
+                )
+                self.threads[widget].start()
+            sv_ttk.set_theme(
+                darkdetect.theme().lower()
+            )  # Keep this to avoid 'font already exists' error
+
+
+clrmgr = ColorManager(default_configs)
```

### Comparing `libtextworker-0.1.1/libtextworker/interface/tk/textwidget.py` & `libtextworker-0.1.2/libtextworker/interface/tk/editor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,123 +1,123 @@
-import tkinter.ttk as ttk
-from tkinter import BooleanVar, Menu, Text
-
-
-class TextWidget(Text):
-    def __init__(
-        self,
-        parent,
-        useMenu: bool = True,
-        useScrollbars: bool = True,
-        unRedo: bool = True,
-        **kwds,
-    ):
-        """
-        Customized Tkinter Text widget with a basic right-click menu.
-        @param parent : Where to place this widget
-        @param useMenu (bool) : Enable right-click menu or not
-        @param unredo (bool)=True : Undo Redo
-        @param useScrollbars (bool)=True : Use scrollbars
-        @param **kwds : Other configurations (tkinter.Text)
-
-        You can set TextWidget.wrapbtn to your own wrapbtn to use the wrap feature.
-        The wrap function is wrapmode(event=None).
-        """
-        kwds["undo"] = kwds.get("undo", 0) | self.unRedo
-        super().__init__(parent, **kwds)
-
-        self.wrapbtn = BooleanVar(self)
-        self.wrapbtn.set(True)
-
-        if useMenu != None:
-            self.enableMenu = useMenu
-
-        if self.enableMenu is True:
-            self.RMenu = Menu(self, tearoff=0)
-            self._menu_init()
-            self.bind("<Button-3>", lambda event: self._open_menu(event))
-
-        if useScrollbars is True:
-            self._place_scrollbar()
-
-        self.configure(wrap="word")
-        self.configure(undo=unRedo)
-
-    # Place scrollbars
-    def _place_scrollbar(self):
-        xbar = ttk.Scrollbar(self, orient="horizontal", command=self.xview)
-        ybar = ttk.Scrollbar(self, orient="vertical", command=self.yview)
-        xbar.pack(side="bottom", fill="x")
-        ybar.pack(side="right", fill="y")
-
-    # Right click menu
-    def _menu_init(self):
-        addcmd = self.RMenu.add_command
-        root = self.master
-        addcmd(
-            label=_("Cut"),
-            accelerator="Ctrl+X",
-            command=lambda: root.event_generate("<Control-x>"),
-        )
-        addcmd(
-            label=_("Copy"),
-            accelerator="Ctrl+C",
-            command=lambda: root.event_generate("<Control-c>"),
-        )
-        addcmd(
-            label=_("Paste"),
-            accelerator="Ctrl+V",
-            command=lambda: root.event_generate("<Control-v>"),
-        )
-        if self.unRedo:
-            self.RMenu.add_separator()
-            addcmd(
-                label=_("Undo"),
-                accelerator="Ctrl+Z",
-                command=lambda: root.event_generate("<Control-z>"),
-            )
-            addcmd(
-                label=_("Redo"),
-                accelerator="Ctrl+Y",
-                command=lambda: root.event_generate("<Control-y>"),
-            )
-
-    def _open_menu(self, event=None):
-        try:
-            self.RMenu.post(event.x_root, event.y_root)
-        finally:
-            self.RMenu.grab_release()
-
-    # Add menu item commands
-    def addMenucmd(self, label: str, acc: str = None, fn: object = None, **kw):
-        return self.RMenu.add_command(label=label, accelerator=acc, command=fn, **kw)
-
-    def addMenusepr(self):
-        return self.RMenu.add_separator()
-
-    def addMenucheckbtn(
-        self, label: str, variable: BooleanVar, fn: object, acc: str = None, **kw
-    ):
-        return self.RMenu.add_checkbutton(
-            label=label, accelerator=acc, variable=variable, command=fn, **kw
-        )
-
-    def addMenuradiobtn(
-        self, label: str, variable: BooleanVar, fn: object, acc: str = None, **kw
-    ):
-        return self.RMenu.add_radiobutton(
-            label=label, accelerator=acc, variable=variable, command=fn, **kw
-        )
-
-    def addMenucascade(self, label: str, menu: Menu, **kw):
-        return self.RMenu.add_cascade(label=label, menu=menu, **kw)
-
-    # Wrap mode
-    def wrapmode(self, event=None) -> bool:
-        if self.wrapbtn.get() == True:
-            self.configure(wrap="none")
-            self.wrapbtn.set(False)
-            return False
-        else:
-            self.configure(wrap="word")
-            self.wrapbtn.set(True)
-            return True
+import tkinter.ttk as ttk
+from tkinter import BooleanVar, Menu, Text
+
+
+class TextWidget(Text):
+    def __init__(
+        self,
+        parent,
+        useMenu: bool = True,
+        useScrollbars: bool = True,
+        unRedo: bool = True,
+        **kwds,
+    ):
+        """
+        Customized Tkinter Text widget with a basic right-click menu.
+        @param parent : Where to place this widget
+        @param useMenu (bool) : Enable right-click menu or not
+        @param unredo (bool)=True : Undo Redo
+        @param useScrollbars (bool)=True : Use scrollbars
+        @param **kwds : Other configurations (tkinter.Text)
+
+        You can set TextWidget.wrapbtn to your own wrapbtn to use the wrap feature.
+        The wrap function is wrapmode(event=None).
+        """
+        self.unRedo = kwds["undo"] = kwds.get("undo", 0) or unRedo
+        super().__init__(parent, **kwds)
+
+        self.wrapbtn = BooleanVar(self)
+        self.wrapbtn.set(True)
+
+        if useMenu != None:
+            self.enableMenu = useMenu
+
+        if self.enableMenu is True:
+            self.RMenu = Menu(self, tearoff=0)
+            self._menu_init()
+            self.bind("<Button-3>", lambda event: self._open_menu(event))
+
+        if useScrollbars is True:
+            self._place_scrollbar()
+
+        self.configure(wrap="word")
+        self.configure(undo=unRedo)
+
+    # Place scrollbars
+    def _place_scrollbar(self):
+        xbar = ttk.Scrollbar(self, orient="horizontal", command=self.xview)
+        ybar = ttk.Scrollbar(self, orient="vertical", command=self.yview)
+        xbar.pack(side="bottom", fill="x")
+        ybar.pack(side="right", fill="y")
+
+    # Right click menu
+    def _menu_init(self):
+        addcmd = self.RMenu.add_command
+        root = self.master
+        addcmd(
+            label=_("Cut"),
+            accelerator="Ctrl+X",
+            command=lambda: root.event_generate("<Control-x>"),
+        )
+        addcmd(
+            label=_("Copy"),
+            accelerator="Ctrl+C",
+            command=lambda: root.event_generate("<Control-c>"),
+        )
+        addcmd(
+            label=_("Paste"),
+            accelerator="Ctrl+V",
+            command=lambda: root.event_generate("<Control-v>"),
+        )
+        if self.unRedo:
+            self.RMenu.add_separator()
+            addcmd(
+                label=_("Undo"),
+                accelerator="Ctrl+Z",
+                command=lambda: root.event_generate("<Control-z>"),
+            )
+            addcmd(
+                label=_("Redo"),
+                accelerator="Ctrl+Y",
+                command=lambda: root.event_generate("<Control-y>"),
+            )
+
+    def _open_menu(self, event=None):
+        try:
+            self.RMenu.post(event.x_root, event.y_root)
+        finally:
+            self.RMenu.grab_release()
+
+    # Add menu item commands
+    def addMenucmd(self, label: str, acc: str = None, fn: object = None, **kw):
+        return self.RMenu.add_command(label=label, accelerator=acc, command=fn, **kw)
+
+    def addMenusepr(self):
+        return self.RMenu.add_separator()
+
+    def addMenucheckbtn(
+        self, label: str, variable: BooleanVar, fn: object, acc: str = None, **kw
+    ):
+        return self.RMenu.add_checkbutton(
+            label=label, accelerator=acc, variable=variable, command=fn, **kw
+        )
+
+    def addMenuradiobtn(
+        self, label: str, variable: BooleanVar, fn: object, acc: str = None, **kw
+    ):
+        return self.RMenu.add_radiobutton(
+            label=label, accelerator=acc, variable=variable, command=fn, **kw
+        )
+
+    def addMenucascade(self, label: str, menu: Menu, **kw):
+        return self.RMenu.add_cascade(label=label, menu=menu, **kw)
+
+    # Wrap mode
+    def wrapmode(self, event=None) -> bool:
+        if self.wrapbtn.get() == True:
+            self.configure(wrap="none")
+            self.wrapbtn.set(False)
+            return False
+        else:
+            self.configure(wrap="word")
+            self.wrapbtn.set(True)
+            return True
```

### Comparing `libtextworker-0.1.1/libtextworker/interface/wx/about.py` & `libtextworker-0.1.2/libtextworker/interface/wx/about.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 import wx
 import wx.adv
 
 from typing import Any, final
 from libtextworker.general import CraftItems, libTewException, GetCurrentDir
 
-available_licenses = ["GPL3_short", "GPL3_full", "MIT"]
+available_licenses = [
+    "AGPL_full",
+    "AGPL_short",
+    "GPL3_full",
+    "GPL3_short",
+    "MIT"
+]
 
 
 @final
 class AboutDialog:
     """
     About dialog built with wxPython.
-    All self-set infomations are stored in the ```infos``` attribute. Just run ShowBox().
+    All self-set infomations are stored in the ```infos``` attribute.
+    Just run ShowBox() to see your work.
     You can set the parent of the dialog if needed, use the Parent variable.
+    This class is not sub-class-able.
     """
 
     infos = wx.adv.AboutDialogInfo()
     Parent: Any | None = None
 
     def SetArtists(self, artists):
         return self.infos.SetArtists(artists)
@@ -32,29 +40,34 @@
 
     def SetDocWriters(self, writers):
         return self.infos.SetDocWriters(writers)
 
     def SetIcon(self, icon: wx.Icon):
         return self.infos.SetIcon(icon)
 
-    def SetLicense(self, license: str):
+    def SetLicense(self, license: str, include_copyright: bool = False):
         """
         Set the long, multiline string containing the text of the program license.
-        Not all license types are available. Please see the attribute available_licenses (not in this class but in the same module).
+        Not all license types are available. You can include your program copyright if needed.
+        @see available_licenses
+        @see SetCopyright
         """
+        data = "" # Our result
         if license not in available_licenses:
             raise libTewException(
                 "Sorry about this, but we couldn't find any license as requested ({}). You should notify this for libtextworker devs".format(
                     license
                 )
             )
         targetfile = CraftItems(
             GetCurrentDir(__file__), "../../licenses/{}.txt".format(license)
         )
-        data = open(targetfile, "r").read()
+        if include_copyright == True and self.infos.GetCopyright() != "":
+            data += self.infos.GetCopyright() + "\n"
+        data += open(targetfile, "r").read()
         return self.infos.SetLicence(data)
 
     def SetName(self, name: str):
         return self.infos.SetName(name)
 
     def SetTranslators(self, translators):
         return self.infos.SetTranslators(translators)
```

### Comparing `libtextworker-0.1.1/libtextworker/interface/wx/editor.py` & `libtextworker-0.1.2/libtextworker/interface/wx/editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,20 +86,17 @@
         self.SetMarginMask(1, 0)
         self.SetMarginWidth(1, 40)
 
         return True
 
     def SetupEditorColor(self):
         bg, fg = self.clrmgr._get_color()
-        bg = "#" + "%02x%02x%02x" % bg
-        fg = "#" + "%02x%02x%02x" % fg
         self.StyleSetSpec(0, "fore:{},back:{}".format(fg, bg))
         self.StyleSetSpec(wx.stc.STC_STYLE_LINENUMBER, "fore:{},back:{}".format(fg, bg))
 
-        # TODO: Fix dark mode
         self.clrmgr.setcolorfunc(
             "textw", self.StyleSetBackground, wx.stc.STC_STYLE_DEFAULT
         )
         self.clrmgr.setfontcfunc(
             "textw", self.StyleSetForeground, wx.stc.STC_STYLE_DEFAULT
         )
         self.clrmgr.configure(self)
```

### Comparing `libtextworker-0.1.1/libtextworker/interface/wx/miscs.py` & `libtextworker-0.1.2/libtextworker/interface/wx/miscs.py`

 * *Files identical despite different names*

### Comparing `libtextworker-0.1.1/libtextworker/licenses/GPL3_full.txt` & `libtextworker-0.1.2/libtextworker/licenses/GPL3_full.txt`

 * *Files identical despite different names*

### Comparing `libtextworker-0.1.1/libtextworker/licenses/GPL3_short.txt` & `libtextworker-0.1.2/libtextworker/licenses/GPL3_short.txt`

 * *Files identical despite different names*

### Comparing `libtextworker-0.1.1/libtextworker/licenses/MIT.txt` & `libtextworker-0.1.2/libtextworker/licenses/MIT.txt`

 * *Files identical despite different names*

### Comparing `libtextworker-0.1.1/libtextworker/versioning.py` & `libtextworker-0.1.2/libtextworker/versioning.py`

 * *Files identical despite different names*

### Comparing `libtextworker-0.1.1/LICENSE` & `libtextworker-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `libtextworker-0.1.1/pyproject.toml` & `libtextworker-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libtextworker"
-version = "0.1.1"
+version = "0.1.2"
 description = "App library for textworker"
 authors = ["lebao3105 <bao12345yocoo@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/lebao3105/libtextworker"
 documentation = "https://lebao3105.github.io/libtextworker"
 keywords = ["wx", "tkinter", "gui"]
@@ -17,15 +17,16 @@
 configparser = "^5.3.0"
 Pillow = "^9.5.0"
 packaging = "^23.0"
 importlib-metadata = "^6.1.0"
 
 wxPython = {version = "^4.0.0", optional = true}
 sv-ttk = {version = "^2.4.3", optional = true}
+darkdetect = {version = "^0.8.0", optional = true}
 
 [tool.poetry.extras]
-wx = ["wxPython"]
-tkinter = ["sv-ttk"]
+wx = ["darkdetect", "wxPython"]
+tkinter = ["darkdetect", "sv-ttk"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `libtextworker-0.1.1/PKG-INFO` & `libtextworker-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libtextworker
-Version: 0.1.1
+Version: 0.1.2
 Summary: App library for textworker
 Home-page: https://github.com/lebao3105/libtextworker
 License: GPL-3.0-or-later
 Keywords: wx,tkinter,gui
 Author: lebao3105
 Author-email: bao12345yocoo@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: tkinter
 Provides-Extra: wx
 Requires-Dist: Pillow (>=9.5.0,<10.0.0)
 Requires-Dist: configparser (>=5.3.0,<6.0.0)
+Requires-Dist: darkdetect (>=0.8.0,<0.9.0) ; extra == "wx" or extra == "tkinter"
 Requires-Dist: importlib-metadata (>=6.1.0,<7.0.0)
 Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: sv-ttk (>=2.4.3,<3.0.0) ; extra == "tkinter"
 Requires-Dist: wxPython (>=4.0.0,<5.0.0) ; extra == "wx"
 Project-URL: Bug Tracker, https://github.com/lebao3105/libtextworker/issues
 Project-URL: Documentation, https://lebao3105.github.io/libtextworker
 Description-Content-Type: text/markdown
@@ -30,11 +31,9 @@
 
 ## Usage
 Available packages from Pypi:
 * libtextworker: Base library, contains all codes but no other deps installed
 * libtextworker[tkinter]: Tkinter support
 * libtextworker[wx]: wxPython support
 
-## Todos
-* Custom config files
-* Tkinter support (working on)
+You can read the API documents [here.](https://lebao3105.github.io/libtextworker)
```

