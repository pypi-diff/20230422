# Comparing `tmp/tklinenums-1.6.3.tar.gz` & `tmp/tklinenums-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tklinenums-1.6.3.tar", last modified: Fri Apr 14 01:18:46 2023, max compression
+gzip compressed data, was "tklinenums-1.6.4.tar", last modified: Sat Apr 22 01:22:08 2023, max compression
```

## Comparing `tklinenums-1.6.3.tar` & `tklinenums-1.6.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:18:46.815963 tklinenums-1.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-14 01:18:46.815963 tklinenums-1.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-14 01:18:31.000000 tklinenums-1.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-14 01:18:31.000000 tklinenums-1.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 01:18:46.815963 tklinenums-1.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-14 01:18:31.000000 tklinenums-1.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:18:46.811963 tklinenums-1.6.3/tklinenums/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 01:18:31.000000 tklinenums-1.6.3/tklinenums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-04-14 01:18:31.000000 tklinenums-1.6.3/tklinenums/tklinenums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:18:46.815963 tklinenums-1.6.3/tklinenums.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-14 01:18:46.000000 tklinenums-1.6.3/tklinenums.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-14 01:18:46.000000 tklinenums-1.6.3/tklinenums.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 01:18:46.000000 tklinenums-1.6.3/tklinenums.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-14 01:18:46.000000 tklinenums-1.6.3/tklinenums.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 01:22:08.842734 tklinenums-1.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-04-22 01:22:08.842734 tklinenums-1.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-22 01:21:48.000000 tklinenums-1.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-22 01:21:48.000000 tklinenums-1.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 01:22:08.842734 tklinenums-1.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-22 01:21:48.000000 tklinenums-1.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 01:22:08.842734 tklinenums-1.6.4/tklinenums/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 01:21:48.000000 tklinenums-1.6.4/tklinenums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10963 2023-04-22 01:21:48.000000 tklinenums-1.6.4/tklinenums/tklinenums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 01:22:08.842734 tklinenums-1.6.4/tklinenums.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-04-22 01:22:08.000000 tklinenums-1.6.4/tklinenums.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-22 01:22:08.000000 tklinenums-1.6.4/tklinenums.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 01:22:08.000000 tklinenums-1.6.4/tklinenums.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-22 01:22:08.000000 tklinenums-1.6.4/tklinenums.egg-info/top_level.txt
```

### Comparing `tklinenums-1.6.3/tklinenums/tklinenums.py` & `tklinenums-1.6.4/tklinenums/tklinenums.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,84 +2,98 @@
 from __future__ import annotations
 
 import platform
 from tkinter import Canvas, Event, Misc, Text
 from tkinter.font import Font
 
 system: str = str(platform.system())
-if system == "Darwin":
-    scroll_inversion: int = -1
+if system in ("Darwin" or "Windows"):
+    scroll_inversion = lambda delta: -delta
 else:
-    scroll_inversion: int = 1
+    scroll_inversion = lambda delta: int(delta / 120)
 
 
 class TkLineNumError(Exception):
     ...
 
 
 class TkLineNumbers(Canvas):
     """
     Creates a line number widget for a text widget. Options are the same as a tkinter Canvas widget and add the following:
-        * -justify (str): The justification of the line numbers. Can be "left", "right", or "center". Default is "left".
-        * -font (tuple | Font | str | None): The font of the line numbers. Default is the text widget's font.
         * -editor (Text): The text widget to attach the line numbers to. (Required) (Second argument after master)
+        * -justify (str): The justification of the line numbers. Can be "left", "right", or "center". Default is "left".
 
     Methods to be used outside externally:
         * .redraw(): Redraws the widget
         * .resize(): Calculates the required width of the widget and resizes it according to the text widget's font and the number of lines
         * .set_to_ttk_style(): Sets the foreground and background colors to the ttk style of the text widget
-        * .reload_font(): Reloads the font of the widget (Requires font as argument)
+        * .reload(): Reloads the style of the widget and redraws it.
     """
 
     def __init__(
         self,
         master: Misc,
         editor: Text,
         justify: str = "left",
         *args,
         **kwargs,
     ) -> None:
         """Initializes the widget -- Internal use only"""
-        self.textwidget = editor
-        self.master = master
-        self.justify = justify
         Canvas.__init__(
             self,
             master,
-            width=kwargs.get("width", 40),
-            highlightthickness=kwargs.get("highlightthickness", 0),
-            borderwidth=kwargs.get("borderwidth", 2),
-            relief=kwargs.get("relief", "ridge"),
+            width=kwargs.pop("width", 40),
+            highlightthickness=kwargs.pop("highlightthickness", 0),
+            borderwidth=kwargs.pop("borderwidth", 2),
+            relief=kwargs.pop("relief", "ridge"),
             *args,
             **kwargs,
         )
+    
+        # Set variable
+        self.textwidget = editor
+        self.master = master
+        self.justify = justify
+        self.click_pos: None = None
+
+        # Set style
         self.set_to_ttk_style()
 
+        # Event bindings
         self.bind("<MouseWheel>", self.mouse_scroll, add=True)
-        # If I'm mouse scrolling and I am clicking on line numbers, it should select the lines from where I clicked to where I am scrolling
-        # TODO: Make it so that it selects the lines from where I clicked to where I am scrolling
-        # Not a feauture in VS Code
         self.bind("<Button-1>", self.click_see, add=True)
         self.bind("<ButtonRelease-1>", self.unclick, add=True)
         self.bind("<Double-Button-1>", self.double_click, add=True)
         self.bind("<Button1-Motion>", self.drag, add=True)
         self.bind("<Button1-Leave>", self.auto_scroll, add=True)
 
-        self.click_pos: None = None
+        # Set the yscrollcommand of the text widget to redraw the widget
+        text["yscrollcommand"] = self.redraw
 
     def redraw(self, *args) -> None:
         """Redraws the widget"""
+        # Resize the widget based on the number of lines in the editor
         self.resize()
+
+        # Delete all the old line numbers
         self.delete("all")
+
+        # Get the first and last line numbers for the editor (all other lines are in between)
         first_line, last_line = int(self.textwidget.index("@0,0").split(".")[0]), int(
             self.textwidget.index(f"@0,{self.textwidget.winfo_height()}").split(".")[0]
         )
+
+        # Draw the line numbers looping through the lines
         for lineno in range(first_line, last_line + 1):
+
+            # If the line is not visible, skip it
             if (dlineinfo := self.textwidget.dlineinfo(f"{lineno}.0")) is None:
                 continue
+
+            # Create the line number
             self.create_text(
                 0
                 if self.justify == "left"
                 else int(self["width"])
                 if self.justify == "right"
                 else int(self["width"]) / 2,
                 dlineinfo[1],
@@ -88,119 +102,142 @@
                 font=self.textwidget.cget("font"),
                 fill=self.foreground,
             )
 
     def mouse_scroll(self, event: Event) -> None:
         """Scrolls the text widget when the mouse wheel is scrolled -- Internal use only"""
         if system == "Darwin":
-            self.textwidget.yview_scroll(scroll_inversion * event.delta, "units")
+            self.textwidget.yview_scroll(scroll_inversion(event.delta), "units")
         else:
-            self.textwidget.yview_scroll(int(scroll_inversion * (event.delta / 120)), "units")
-        self.redraw()
+            self.textwidget.yview_scroll(int(scroll_inversion(event.delta)), "units")
 
     def click_see(self, event: Event) -> None:
         """When clicking on a line number it scrolls to that line if not shifting -- Internal use only"""
+
+        # If the shift key is down, redirect to self.shift_click()
         if event.state == 1:
             self.shift_click(event)
             return
+
+        #Remove the selection tag from the text widget
         self.textwidget.tag_remove("sel", "1.0", "end")
+
+        # Set the insert position to the line number clicked
         self.textwidget.mark_set(
             "insert",
             f"{self.textwidget.index(f'@{event.x},{event.y}').split('.')[0]}.0",
         )
+
+        # Scroll to the location of the insert position
         self.textwidget.see("insert")
+
+        # If the line clicked is at the edge of the screen, scroll by one line to bring it into view
         first_visible_line, last_visible_line = int(self.textwidget.index("@0,0").split(".")[0]), int(
             self.textwidget.index(f"@0,{self.textwidget.winfo_height()}").split(".")[0]
         )
         if (insert := int(self.textwidget.index("insert").split(".")[0])) == first_visible_line:
             self.textwidget.yview_scroll(-1, "units")
         elif insert == last_visible_line:
             self.textwidget.yview_scroll(1, "units")
         self.click_pos = self.textwidget.index("insert")
 
     def unclick(self, event: Event) -> None:
-        """When the mouse button is released it removes the selection -- Internal use only"""
+        """When the mouse button is released the click position is None -- Internal use only"""
         self.click_pos: None = None
 
     def double_click(self, event: Event) -> None:
         """Selects the line when double clicked -- Internal use only"""
+        # Add the selection tag to the line double clicked
         self.textwidget.tag_remove("sel", "1.0", "end")
         self.textwidget.tag_add("sel", "insert", "insert + 1 line")
 
     def auto_scroll(self, event: Event) -> None:
         """Automatically scrolls the text widget when the mouse is near the top or bottom, similar to the drag function -- Internal use only"""
+
+        # If the mouse is not down, return
         if self.click_pos is None:
             return
+
+        # Taken from the Text source: https://github.com/tcltk/tk/blob/main/library/text.tcl#L676
+        # Scrolls the widget if the cursor is off of the screen
         if event.y >= self.winfo_height():
             self.textwidget.yview_scroll(1 if system == "Darwin" else (1 / 120), "units")
         elif event.y < 0:
             self.textwidget.yview_scroll(-1 if system == "Darwin" else (-1 / 120), "units")
-        elif event.x >= self.winfo_width():
-            self.textwidget.xview_scroll(2 if system == "Darwin" else (2 / 120), "units")
-        elif event.x < 0:
-            self.textwidget.xview_scroll(-2 if system == "Darwin" else (-2 / 120), "units")
         else:
             return
+
+        #  Set the selection tag and insert position
         start, end = self.textwidget.index("insert"), self.click_pos
         if self.textwidget.compare("insert", ">", self.click_pos):
             start, end = end, str(float(start) + 1)
         else:
             end = str(float(end) + 1)
         self.textwidget.tag_remove("sel", "1.0", "end")
         self.textwidget.tag_add("sel", start, end)
         self.textwidget.mark_set("insert", f"@{event.x},{event.y}")
+
+        # Call the function recursively using the after method with a delay of 50 milliseconds
+        # Also stolen from the Text source: https://github.com/tcltk/tk/blob/main/library/text.tcl#L704
         self.after(50, self.auto_scroll, event)
 
     def drag(self, event: Event) -> None:
         """When click dragging it selects the text -- Internal use only"""
+
+        # If the mouse is not down or outside of the widget, return
         if (
             self.click_pos is None
             or event.x < 0
             or event.x >= self.winfo_width()
             or event.y < 0
             or event.y >= self.winfo_height()
         ):
             return
+
+        # Set the selection tag and insert position
         start, end = self.textwidget.index("insert"), self.click_pos
         if self.textwidget.compare("insert", ">", self.click_pos):
-            start, end = start, str(float(end) + 1)
+            start, end = end, str(float(start) + 1)
+        else:
+            end = str(float(end) + 1)
 
-        if self.textwidget.compare(start, ">", end):
-            start, end = end, start
         self.textwidget.tag_remove("sel", "1.0", "end")
-        self.textwidget.tag_add("sel", start, end)
-        self.textwidget.mark_set("insert", self.textwidget.index(f"@{event.x},{event.y} linestart"))
-        self.redraw()
+        self.textwidget.tag_add("sel", start.split(".")[0] + ".0", end.split(".")[0] + ".0")
+        self.textwidget.mark_set("insert", self.textwidget.index(f"@{event.x},{event.y} linestart + 1 line"))
 
-        """
-        Issues:
-         - Once it starts going it's hard to stop drag clicking (because most people pull back up when done but this is still
-           considered dragging and it remembers the direction meaning it will continue to drag in that direction)unless you unclick
-         - Once it goes past the end of the text widget it will continue to drag in that direction until unclicked
-        """  # TODO: Fix issues
+        # Redraw the widget
+        self.redraw()
 
     def shift_click(self, event: Event) -> None:
         """When shift clicking it selects the text between the click and the cursor -- Internal use only"""
+
+        # Add the selection tag to the text between the click and the cursor
         start_pos, end_pos = self.textwidget.index("insert"), self.textwidget.index(f"@0,{event.y}")
         self.textwidget.tag_remove("sel", "1.0", "end")
         if self.textwidget.compare(start_pos, ">", end_pos):
             start_pos, end_pos = end_pos, start_pos
         self.textwidget.tag_add("sel", start_pos, end_pos)
 
     def resize(self) -> None:
         """Resizes the widget to fit the text widget"""
+
+        # Get amount of lines in the text widget
         end = self.textwidget.index("end").split(".")[0]
+
+        # Set the width of the widget to the required width to display the biggest line number
         self.config(width=Font(font=(temp_font := self.textwidget.cget("font"))).measure(" 1234 ")) if int(
             end
         ) <= 1000 else self.config(width=temp_font.measure(f" {end} "))
 
     def set_to_ttk_style(self) -> None:
         """Sets the widget to the ttk style"""
+
+        # Set the background and foreground to the ttk style
         self["bg"] = self.tk.eval("ttk::style lookup TLineNumbers -background")
-        self.foreground = self.tk.eval("ttk::style lookup TLineNumbers -foreground")
+        self["fg"] = self.tk.eval("ttk::style lookup TLineNumbers -foreground")
 
     def reload(self) -> None:
         """Reloads the widget"""
         self.set_to_ttk_style()
         self.redraw()
 
 
@@ -231,11 +268,10 @@
 
     linenums = TkLineNumbers(root, text)
     linenums.pack(fill="y", side="left", expand=True)
 
     text.bind("<Key>", lambda event: root.after_idle(linenums.redraw), add=True)
     text.bind(f"<BackSpace>", lambda event: root.after_idle(linenums.redraw), add=True)
     text.bind(f"<{contmand}-v>", lambda event: root.after_idle(linenums.redraw), add=True)
-    text["yscrollcommand"] = linenums.redraw
-    text.config(font=("Courier New bold", 13))
+    text.config(font=("Courier New bold", 15))
 
     root.mainloop()
```

