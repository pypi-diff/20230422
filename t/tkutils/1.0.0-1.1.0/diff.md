# Comparing `tmp/tkutils-1.0.0.tar.gz` & `tmp/tkutils-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkutils-1.0.0.tar", max compression
+gzip compressed data, was "tkutils-1.1.0.tar", max compression
```

## Comparing `tkutils-1.0.0.tar` & `tkutils-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rwxr-xr-x   0        0        0     2821 2023-01-15 21:51:08.238749 tkutils-1.0.0/README.md
--rwxr-xr-x   0        0        0      752 2023-01-15 21:51:08.254950 tkutils-1.0.0/pyproject.toml
--rwxr-xr-x   0        0        0     3575 2023-01-15 21:51:12.744650 tkutils-1.0.0/src/tkutils/__init__.py
--rwxr-xr-x   0        0        0      101 2022-12-22 16:54:42.632637 tkutils-1.0.0/src/tkutils/__main__.py
--rwxr-xr-x   0        0        0       22 2023-01-15 21:51:12.745938 tkutils-1.0.0/src/tkutils/__version__.py
--rwxr-xr-x   0        0        0     8949 2022-12-22 16:54:42.645033 tkutils-1.0.0/src/tkutils/grid_layout.py
--rwxr-xr-x   0        0        0        0 2022-12-22 16:54:42.645734 tkutils-1.0.0/src/tkutils/helpers/__init__.py
--rwxr-xr-x   0        0        0     4317 2022-12-22 16:54:42.658071 tkutils-1.0.0/src/tkutils/helpers/event_provider.py
--rwxr-xr-x   0        0        0     5287 2022-12-22 16:54:42.710835 tkutils-1.0.0/src/tkutils/helpers/keysym.py
--rwxr-xr-x   0        0        0    10267 2022-12-22 16:54:42.727324 tkutils-1.0.0/src/tkutils/images.py
--rwxr-xr-x   0        0        0       37 2022-12-22 16:54:42.728682 tkutils-1.0.0/src/tkutils/menu_builder/__init__.py
--rwxr-xr-x   0        0        0     2271 2022-12-22 16:54:42.749677 tkutils-1.0.0/src/tkutils/menu_builder/bases.py
--rwxr-xr-x   0        0        0     5046 2022-12-22 16:54:42.783801 tkutils-1.0.0/src/tkutils/menu_builder/menu_builder.py
--rwxr-xr-x   0        0        0     8294 2022-12-22 16:54:42.801555 tkutils-1.0.0/src/tkutils/menu_builder/menu_builder_options.py
--rwxr-xr-x   0        0        0      220 2022-12-22 16:54:42.802957 tkutils-1.0.0/src/tkutils/two_way_binding/__init__.py
--rwxr-xr-x   0        0        0    24893 2023-01-11 21:11:59.213365 tkutils-1.0.0/src/tkutils/two_way_binding/binder.py
--rwxr-xr-x   0        0        0    13629 2023-01-15 16:32:13.825748 tkutils-1.0.0/src/tkutils/two_way_binding/binding_descriptor.py
--rwxr-xr-x   0        0        0        0 2022-12-22 16:54:42.814650 tkutils-1.0.0/src/tkutils/two_way_binding/configuration/__init__.py
--rwxr-xr-x   0        0        0     9067 2022-12-22 16:54:42.826259 tkutils-1.0.0/src/tkutils/two_way_binding/configuration/_binder_config.py
--rwxr-xr-x   0        0        0    10710 2022-12-22 16:54:42.838147 tkutils-1.0.0/src/tkutils/two_way_binding/configuration/_configuration.py
--rwxr-xr-x   0        0        0     2856 2022-12-22 16:54:42.849190 tkutils-1.0.0/src/tkutils/two_way_binding/configuration/_configurer_image_factory.py
--rwxr-xr-x   0        0        0      565 2022-12-22 16:54:42.850410 tkutils-1.0.0/src/tkutils/two_way_binding/errors.py
--rwxr-xr-x   0        0        0       55 2022-12-22 16:54:42.863360 tkutils-1.0.0/src/tkutils/utilities/__init__.py
--rwxr-xr-x   0        0        0    12657 2022-12-22 16:54:42.896203 tkutils-1.0.0/src/tkutils/utilities/singleton_namespace.py
--rw-r--r--   0        0        0     3967 1970-01-01 00:00:00.000000 tkutils-1.0.0/setup.py
--rw-r--r--   0        0        0     3574 1970-01-01 00:00:00.000000 tkutils-1.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0     2817 2023-04-13 15:35:19.622223 tkutils-1.1.0/README.md
+-rwxr-xr-x   0        0        0      752 2023-04-22 21:02:30.094308 tkutils-1.1.0/pyproject.toml
+-rwxr-xr-x   0        0        0     3571 2023-04-22 21:02:32.868476 tkutils-1.1.0/src/tkutils/__init__.py
+-rwxr-xr-x   0        0        0      101 2022-12-22 16:54:42.632637 tkutils-1.1.0/src/tkutils/__main__.py
+-rwxr-xr-x   0        0        0       22 2023-04-22 21:02:32.870438 tkutils-1.1.0/src/tkutils/__version__.py
+-rwxr-xr-x   0        0        0     9327 2023-01-16 21:22:40.730857 tkutils-1.1.0/src/tkutils/grid_layout.py
+-rwxr-xr-x   0        0        0        0 2022-12-22 16:54:42.645734 tkutils-1.1.0/src/tkutils/helpers/__init__.py
+-rwxr-xr-x   0        0        0     4316 2023-01-16 18:36:26.640113 tkutils-1.1.0/src/tkutils/helpers/event_provider.py
+-rwxr-xr-x   0        0        0     5290 2023-01-16 18:38:03.163623 tkutils-1.1.0/src/tkutils/helpers/keysym.py
+-rwxr-xr-x   0        0        0    10198 2023-04-22 18:41:55.827669 tkutils-1.1.0/src/tkutils/images.py
+-rwxr-xr-x   0        0        0       37 2022-12-22 16:54:42.728682 tkutils-1.1.0/src/tkutils/menu_builder/__init__.py
+-rwxr-xr-x   0        0        0     2261 2023-01-15 23:06:06.313331 tkutils-1.1.0/src/tkutils/menu_builder/bases.py
+-rwxr-xr-x   0        0        0     5047 2023-01-16 18:40:13.861655 tkutils-1.1.0/src/tkutils/menu_builder/menu_builder.py
+-rwxr-xr-x   0        0        0     8300 2023-01-16 18:42:42.691137 tkutils-1.1.0/src/tkutils/menu_builder/menu_builder_options.py
+-rwxr-xr-x   0        0        0      220 2022-12-22 16:54:42.802957 tkutils-1.1.0/src/tkutils/two_way_binding/__init__.py
+-rwxr-xr-x   0        0        0    28483 2023-04-22 20:11:30.692562 tkutils-1.1.0/src/tkutils/two_way_binding/binder.py
+-rwxr-xr-x   0        0        0    13926 2023-04-22 18:41:55.830751 tkutils-1.1.0/src/tkutils/two_way_binding/binding_descriptor.py
+-rwxr-xr-x   0        0        0        0 2022-12-22 16:54:42.814650 tkutils-1.1.0/src/tkutils/two_way_binding/configuration/__init__.py
+-rwxr-xr-x   0        0        0     9282 2023-04-22 18:41:55.832202 tkutils-1.1.0/src/tkutils/two_way_binding/configuration/_binder_config.py
+-rwxr-xr-x   0        0        0    10709 2023-01-16 18:23:18.891984 tkutils-1.1.0/src/tkutils/two_way_binding/configuration/_configuration.py
+-rwxr-xr-x   0        0        0     2856 2022-12-22 16:54:42.849190 tkutils-1.1.0/src/tkutils/two_way_binding/configuration/_configurer_image_factory.py
+-rwxr-xr-x   0        0        0      565 2022-12-22 16:54:42.850410 tkutils-1.1.0/src/tkutils/two_way_binding/errors.py
+-rwxr-xr-x   0        0        0       55 2022-12-22 16:54:42.863360 tkutils-1.1.0/src/tkutils/utilities/__init__.py
+-rwxr-xr-x   0        0        0    12657 2022-12-22 16:54:42.896203 tkutils-1.1.0/src/tkutils/utilities/singleton_namespace.py
+-rw-r--r--   0        0        0     3570 1970-01-01 00:00:00.000000 tkutils-1.1.0/PKG-INFO
```

### Comparing `tkutils-1.0.0/README.md` & `tkutils-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Welcome to TkUtils
 
-`tkutils` is a package offering some additional logic and syntactic sugar when using tkinter.
+`tkutils` is a package offering some additional logic and syntactic sugar when using `tkinter`.
 The main goal is to fill some gaps of tkinter, which might make it very annoying to use.
 
 Online version of the help documentation: http://frederic.zinelli.gitlab.io/tkutils/
 
 
 
 ## Features
 
 
-### Additional logic: two-way binding with [`Binder`](http://frederic.zinelli.gitlab.io/tkutils/binder/binder_overview/)
+### Additional logic: two-way binding, with [`Binder`](http://frederic.zinelli.gitlab.io/tkutils/binder/binder_overview/)
 
-The [`Binder`](http://frederic.zinelli.gitlab.io/tkutils/binder/binder_overview/) class is an utility to setup a transparent two-way
+The [`Binder`](http://frederic.zinelli.gitlab.io/tkutils/binder/binder_overview/) class is  to setup a transparent two-way
 binding reactivity between widgets and underlying object properties from the model/logic layer
 of the application.
 
 Several advantages come with this:
 
 * Changes of bound properties in the model layer are cascading in the GUI automatically.
 * The model layer of the application becomes (finally) totally independent from the presentation
@@ -33,35 +33,34 @@
 A grid layout manager which is abstracting away all the naughty `widget.grid(...)` calls and
 rows/columns grid configuration. Positioning widgets in the grid and controlling their "spanning"
 becomes very easy, without extra typing.
 
 
 #### [`MenuBuilder`](http://frederic.zinelli.gitlab.io/tkutils/menu_builder/menu_builder/)
 
-A helper to build menus and to abstract away all the technicalities, when creating menus through
-`tkinter`, which quickly make the declarations very unclear. Using the [`MenuBuilder`](http://frederic.zinelli.gitlab.io/tkutils/menu_builder/menu_builder/),
-the actual Menu hierarchy becomes very obvious: "what you see is what you get".
+A helper to build menus and to abstract away all the technicalities encountered when creating menus through
+`tkinter`, which quickly make the declarations very unclear. Using the [`MenuBuilder`](http://frederic.zinelli.gitlab.io/tkutils/menu_builder/menu_builder/), the actual `Menu` hierarchy becomes very obvious: "what you see is what you get".
 
 
 #### [`Event`](http://frederic.zinelli.gitlab.io/tkutils/event/)
 
-An utility to build event strings with autocompletion/IDE suggestions support.
+A utility to build event strings with auto-completion/IDE suggestions support.
 
 
 #### [`KeySym`](http://frederic.zinelli.gitlab.io/tkutils/key_sym/)
 
-An utility to get all keysym informations with autocompletion/IDE suggestions (providing string,
+A utility to get all keysym information with auto-completion/IDE suggestions (providing string,
 keycode and keysym_num values).
 
 
 #### [`images`](http://frederic.zinelli.gitlab.io/tkutils/images/images/)
 
 Various factories related to images to:
 
-* Simplify and reduce the syntaxes/typing needed,
+* Simplify and reduce the typing needed,
 * Handle file conversions automatically,
 * Register automatically the image object on the host for the user (to avoid garbage collection).
 
 
 
 
 ## Requirements
```

### Comparing `tkutils-1.0.0/pyproject.toml` & `tkutils-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tkutils"
-version = "1.0.0"
+version = "1.1.0"
 description = "Python tkinter utilities."
 authors = ["Frédéric Zinelli <frederic.zinelli@gmail.com>"]
 license = "FreeBSD"
 readme = "README.md"
 repository = "https://gitlab.com/frederic.zinelli/tkutils"
 homepage = "http://frederic.zinelli.gitlab.io/tkutils/"
```

### Comparing `tkutils-1.0.0/src/tkutils/__init__.py` & `tkutils-1.1.0/src/tkutils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
 # Welcome to TkUtils
 
-`tkutils` is a package offering some additional logic and syntactic sugar when using tkinter.
+`tkutils` is a package offering some additional logic and syntactic sugar when using `tkinter`.
 The main goal is to fill some gaps of tkinter, which might make it very annoying to use.
 
 Online version of the help documentation: http://frederic.zinelli.gitlab.io/tkutils/
 
 
 
 ## Features
 
 
-### Additional logic: two-way binding with [`Binder`](http://frederic.zinelli.gitlab.io/tkutils/binder/binder_overview/)
+### Additional logic: two-way binding, with [`Binder`](http://frederic.zinelli.gitlab.io/tkutils/binder/binder_overview/)
 
-The [`Binder`](http://frederic.zinelli.gitlab.io/tkutils/binder/binder_overview/) class is an utility to setup a transparent two-way
+The [`Binder`](http://frederic.zinelli.gitlab.io/tkutils/binder/binder_overview/) class is  to setup a transparent two-way
 binding reactivity between widgets and underlying object properties from the model/logic layer
 of the application.
 
 Several advantages come with this:
 
 * Changes of bound properties in the model layer are cascading in the GUI automatically.
 * The model layer of the application becomes (finally) totally independent from the presentation
@@ -34,35 +34,34 @@
 A grid layout manager which is abstracting away all the naughty `widget.grid(...)` calls and
 rows/columns grid configuration. Positioning widgets in the grid and controlling their "spanning"
 becomes very easy, without extra typing.
 
 
 #### [`MenuBuilder`](http://frederic.zinelli.gitlab.io/tkutils/menu_builder/menu_builder/)
 
-A helper to build menus and to abstract away all the technicalities, when creating menus through
-`tkinter`, which quickly make the declarations very unclear. Using the [`MenuBuilder`](http://frederic.zinelli.gitlab.io/tkutils/menu_builder/menu_builder/),
-the actual Menu hierarchy becomes very obvious: "what you see is what you get".
+A helper to build menus and to abstract away all the technicalities encountered when creating menus through
+`tkinter`, which quickly make the declarations very unclear. Using the [`MenuBuilder`](http://frederic.zinelli.gitlab.io/tkutils/menu_builder/menu_builder/), the actual `Menu` hierarchy becomes very obvious: "what you see is what you get".
 
 
 #### [`Event`](http://frederic.zinelli.gitlab.io/tkutils/event/)
 
-An utility to build event strings with autocompletion/IDE suggestions support.
+A utility to build event strings with auto-completion/IDE suggestions support.
 
 
 #### [`KeySym`](http://frederic.zinelli.gitlab.io/tkutils/key_sym/)
 
-An utility to get all keysym informations with autocompletion/IDE suggestions (providing string,
+A utility to get all keysym information with auto-completion/IDE suggestions (providing string,
 keycode and keysym_num values).
 
 
 #### [`images`](http://frederic.zinelli.gitlab.io/tkutils/images/images/)
 
 Various factories related to images to:
 
-* Simplify and reduce the syntaxes/typing needed,
+* Simplify and reduce the typing needed,
 * Handle file conversions automatically,
 * Register automatically the image object on the host for the user (to avoid garbage collection).
 
 
 
 
 ## Requirements
```

### Comparing `tkutils-1.0.0/src/tkutils/grid_layout.py` & `tkutils-1.1.0/src/tkutils/grid_layout.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 
 
 import tkinter as T
 from dataclasses import dataclass
 from typing import Any, Dict, NewType, Sequence, Tuple, Union
-from typing_extensions import Self
 
 
 
 
 LayOut2D = NewType('LayOut2D', Sequence[Sequence[ Union[None,T.Widget] ]])
 
 
@@ -20,63 +19,85 @@
         Create a helper to manage the grid of the widget passed to the constructor. Can handle
         rows and columns characteristics, widgets placement and spanning.
     """
 
     holder: T.Widget
 
 
-    def col_weights(self, *weights:int) -> Self :
-        """ Define the weight for each column of the grid, using varargs. """
+    def col_weights(self, *weights:int) -> 'GridLayout' :
+        """ Define the weight for each column of the grid, using varargs.
+
+            Returns:
+                Self
+        """
         return self.__applier('columnconfigure', 'weight', weights)
 
-    def row_weights(self, *weights:int) -> Self :
-        """ Define the weight for each row of the grid, using varargs. """
+    def row_weights(self, *weights:int) -> 'GridLayout' :
+        """ Define the weight for each row of the grid, using varargs.
+
+            Returns:
+                Self
+        """
         return self.__applier('rowconfigure', 'weight', weights)
 
-    def col_minsizes(self, *minsizes:int) -> Self :
-        """ Define the minsizes for each column of the grid, using varargs. """
+    def col_minsizes(self, *minsizes:int) -> 'GridLayout' :
+        """ Define the minsizes for each column of the grid, using varargs.
+
+            Returns:
+                Self
+        """
         return self.__applier('columnconfigure', 'minsize', minsizes)
 
-    def row_minsizes(self, *minsizes:int) -> Self :
-        """ Define the minsizes for each row of the grid, using varargs. """
+    def row_minsizes(self, *minsizes:int) -> 'GridLayout' :
+        """ Define the minsizes for each row of the grid, using varargs.
+
+            Returns:
+                Self
+        """
         return self.__applier('rowconfigure', 'minsize', minsizes)
 
 
-    def __applier(self, row_or_col:str, option:str, values:Sequence) -> Self :
+    def __applier(self, row_or_col:str, option:str, values:Sequence) -> 'GridLayout' :
         grid_method = getattr(self.holder, row_or_col)
         for i,value in enumerate(values):
             grid_method(i, **{option:value})
         return self
 
 
-    def weights(self, *, cols:Tuple[int]=(1,), rows:Tuple[int]=(1,)) -> Self :
+    def weights(self, *, cols:Tuple[int,...]=(1,), rows:Tuple[int,...]=(1,)) -> 'GridLayout' :
         """ Alternative to do both `GridLayout.col_weights` and `GridLayout.row_weights` calls
             one shot.
 
             Parameters:
                 cols: tuple of weights for the columns
                 rows: tuple of weights for the rows
 
             !!! note
                 On the contrary of the isolated calls through [col_weights]
                 [src.tkutils.grid_layout.GridLayout.col_weights] and [row_weights]
                 [src.tkutils.grid_layout.GridLayout.row_weights], if one of the dimensions isn't given, it
                 will be automatically handled to make it one row/column filling with a weight of 1.
+
+            Returns:
+                Self
         """
         self.col_weights(*cols)
         self.row_weights(*rows)
         return self
 
 
-    def minsizes(self, *, cols:Tuple[int]=(None,), rows:Tuple[int]=(None,)) -> Self :
+    def minsizes(self, *, cols:Tuple[int,...]=(None,), rows:Tuple[int,...]=(None,)) -> 'GridLayout' :
         """ Alternative to do `GridLayout.col_minsizes` and `GridLayout.row_minsizes` one shot.
 
             Parameters:
                 cols: tuple of minimal sizes (in pixels) for the columns
                 rows: tuple of minimal sizes (in pixels) for the rows
+
+            Returns:
+                Self
         """
         self.col_minsizes(*cols)
         self.row_minsizes(*rows)
         return self
 
 
 
@@ -84,15 +105,15 @@
         self,
         grid:LayOut2D,
         *,
         pad:int = 5,
         sticky:str = T.EW,
         specials:Dict[T.Widget, Dict]=None,
         **options:Any,
-    ) -> Self :
+    ) -> 'GridLayout' :
         """ Given a grid of widgets as a 2D-array (`Layout2D`) and a bunch of options, determine
             automatically  the placement of all the widgets in the grid (and their "spanning" if
             any), and apply automatically the wanted options on each widget.
 
             !!! tip
                 If some cells of the LayOut2D grid must stay empty, use `None` for them.
 
@@ -127,14 +148,17 @@
                             are overriding `pad` and `sticky` related options. `options` are applied
                             to all the widgets in the grid.
 
             Raises:
                 ValueError: If the `grid` isn't rectangular.
                 ValueError: If some spanning widgets aren't covering a rectangular area of the grid
                             (`w * h` references).
+
+            Returns:
+                Self
         """
 
         lengths = set(map(len,grid))
         if len(lengths) != 1:
             raise ValueError(f"Some row lengths are mismatched: {lengths}")
```

### Comparing `tkutils-1.0.0/src/tkutils/helpers/event_provider.py` & `tkutils-1.1.0/src/tkutils/helpers/event_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     TplClick = EventStr('<Triple-Button>')
     """ Mouse triple click """
 
     TriClick = EventStr('<Triple-Button>')
     """ Mouse triple click """
 
     Deactivate = EventStr('<Deactivate>')
-    """ Widget gets deeactivated """
+    """ Widget gets deactivated """
 
     Destroy = EventStr('<Destroy>')
     """ Widget gets destroyed """
 
     Enter = EventStr('<Enter>')
     """ Mouse enters the Widget """
```

### Comparing `tkutils-1.0.0/src/tkutils/helpers/keysym.py` & `tkutils-1.1.0/src/tkutils/helpers/keysym.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 # Overview
 
-`KeySym` is a helper to provide autocompletion for all `tkinter KeySym` strings, as well as their
+`KeySym` is a helper to provide auto-completion for all `tkinter KeySym` strings, as well as their
 `keycode` and `keysym_num` values (as properties of the inner Key string object itself).
 
 # Examples
 
 * `KeySym.Escape             ->  "Escape"`
 * `KeySym.Escape.keycode     ->  9`
 * `KeySym.Escape.keysym_num  ->  65307`
@@ -39,17 +39,17 @@
             obj.keysym_num = num
             return obj
 
 
     @dataclass
     class KeyDesc:
         """ Descriptor to DRY the KeySym definition.
-            If the name is not provided to the constructor, the attribut name will be automatically
+            If the name is not provided to the constructor, the attribute name will be automatically
             used as value, through the __set_name__ method.
-            It the constructor receives a name, it will be used instead. This allows to decorelate
+            It the constructor receives a name, it will be used instead. This allows to decorrelate
             the attribute name from its value, where needed.
         """
         keycode:    int
         keysym_num: int
         name:       Optional[str] = None
         key:        Optional[Key] = None
```

### Comparing `tkutils-1.0.0/src/tkutils/images.py` & `tkutils-1.1.0/src/tkutils/images.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,27 +52,28 @@
             A [`build_image_from`][src.fake_for_docs.build_image_from] factory function.
     """
 
     if any_file_in_project is None:
         any_file_in_project = inspect.stack()[1].filename
 
     # Cut the leaves as long as the root project directory isn't reached:
-    while len(any_file_in_project) > 1:
-        root,name = os.path.split(any_file_in_project)
+    searching = any_file_in_project
+    while True:
+        root,name = os.path.split(searching)
         if name == project_name:
             break
-        any_file_in_project = root
-    project_root = any_file_in_project
 
-    if len(project_root)<2:                 # forbid hdd root as well (not possible from a project)
-        raise FileNotFoundError(
-            f"Couldn't find the project name { project_name !r} in the given path:\n"
-            f"{ any_file_in_project !r}"
-        )
+        if root == searching:
+            raise FileNotFoundError(
+                f"Couldn't find the project name { project_name !r} in the given path:\n"
+                f"{ any_file_in_project !r}"
+            )
+        searching = root
 
+    project_root     = searching
     images_directory = os.path.join(project_root, *path_to_images)
 
     if not os.path.isdir(images_directory):
         raise FileNotFoundError(f"{ images_directory !r} isn't a valid directory location")
 
 
     def build_image_from(
@@ -89,15 +90,15 @@
                         image factory
                 width:  Define the width to use for the image
                 height: Define the height to use for the image
                 size:   Define the width and height one shot (square)
 
             Raises:
                 ValueError: For invalid dimensions arguments, or FileNotFoundError if the
-                            filename or the path is invalide.
+                            filename or the path is invalid.
 
             Returns:
                 The image itself, or a tuple `(image, width, height)`, depending on the `image_only` argument of [`images_factory`][src.tkutils.images.images_factory].
         """
         filepath = os.path.join(images_directory, file)
         data     = _tk_image_from(filepath, width, height, size)
         return data[0] if image_only else data
```

### Comparing `tkutils-1.0.0/src/tkutils/menu_builder/bases.py` & `tkutils-1.1.0/src/tkutils/menu_builder/bases.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,17 +43,17 @@
 
 
     def bind(self, widget:T.Widget, event_str:str) -> Self:
         """ Bind the given widget widget to the given event, using the callback of the current
             instance (Cmd, CheckBtn or RadioGrp).
 
             !!! tip "Number of arguments of `self.cbk` and their type"
-                The callback will never receive see the `T.Event` argument that triggered it, but
-                 it will receive the new state of the control variable of this instance, if any,
-                 or no argument at all (for callbacks hold by a `Cmd` instance).
+                The callback will never see the `T.Event` argument that triggered it, but it
+                will receive the new state of the control variable of this instance, if any,
+                or no argument at all (for callbacks hold by a `Cmd` instance).
 
             Parameters:
                 widget:    Widget to bind
                 event_str: Event string identifying the event.
         """
         widget.bind(event_str, self.cbk)
         return self
```

### Comparing `tkutils-1.0.0/src/tkutils/menu_builder/menu_builder.py` & `tkutils-1.1.0/src/tkutils/menu_builder/menu_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 
 
 
 
 class MenuBuilder(Singleton):
     """ Utility to build the menus. This is a singleton/namespace,
-        providing autocompletion support to build `tkinter` menus:
+        providing auto-completion support to build `tkinter` menus:
 
         | Property                                                             | Use case                               |
         |:---------------------------------------------------------------------|:---------------------------------------|
         | `sep`                                                                | Menu separator instance (ready to use) |
         | [`Sep`][src.tkutils.menu_builder.menu_builder_options.Sep]           | Relay constructor for `T.Menu.add_separator` (if customized behaviors are needed)|
         | [`Cmd`][src.tkutils.menu_builder.menu_builder_options.Cmd]           | Relay constructor for `T.Menu.add_command` items |
         | [`COption`][src.tkutils.menu_builder.menu_builder_options.COption]   | Handle various options that could be needed at some point for sub widgets |
```

### Comparing `tkutils-1.0.0/src/tkutils/menu_builder/menu_builder_options.py` & `tkutils-1.1.0/src/tkutils/menu_builder/menu_builder_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
 class Cmd(MenuElementWithCbk):
     """ Wrapper for `T.Menu.add_command`.
 
         Parameters:
             label:      Name of the item
             cbk:        Callback taking no argument, to execute on selection of this option
-            c_options:  Additional config options for the menu item. See:
+            c_options:  Additional configuration options for the menu item. See:
                         `T.Menu.add_command(..., coption, ...)`
     """
 
     def __init__(self, label:str, cbk:Callable[[],None], c_options:COption=None):
         self.label = label
         self.cbk   = lambda *_: cbk()
         self.c_options = c_options.kw_c_options if c_options else {}
@@ -133,15 +133,15 @@
 
         Takes a command callback expecting a boolean argument (the value of the underlying control
         variable). The control variable is automatically built by the function, unless an instance
         is passed through the constructor arguments.
 
         Parameters:
             label:     Name of the item
-            cbk:       Callback taking a bool argument (the state of the check button when clicked)
+            cbk:       Callback taking a boolean argument (state of the check button when clicked)
             ctrl_var:  A `T.BooleanVar` instance that will be used for the internal check button.
                        If not given, one will be instantiated automatically and will be accessible
                        through the `self.ctrl_var` property.
             c_options: COptions that can be used when building the check button item.
                        See: `T.Menu.add_check_button(..., coptions, ...)`
     """
```

### Comparing `tkutils-1.0.0/src/tkutils/two_way_binding/binder.py` & `tkutils-1.1.0/src/tkutils/two_way_binding/binder.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 
 import tkinter as T
 
 from inspect import Parameter, signature
 from functools import wraps
-from typing import Any, Callable, Type, TypeVar
+from typing import Any, Callable, Literal, Type, TypeVar
 from PIL import ImageTk
 
 
 from .errors import BinderError, BinderLockedError, BindingCtrlVarError, BindingError
 from .configuration._configuration import (
     CtrlVarTypeForWidget,
     CtrlVarHolderAttribute,
@@ -33,15 +33,15 @@
 
 def unbound_only(meth):
     """ Decorator to ensure that a locked/used Binder instance isn't several times after
         a binding as been set with it.
     """
     @wraps(meth)
     def wrapper(self:'Binder',*a,**kw):
-        if self.bound:
+        if self._bound:                     # pylint: disable=protected-access
             raise BinderLockedError("This object already created a two-way binding...")
         return meth(self, *a,**kw)
     return wrapper
 
 
 
 
@@ -81,86 +81,102 @@
         prop:   property name to bind
     """
 
     def __init__(self, obj:Any=None, prop:str=None):
         if obj is not None:
             check_hashable(obj)
 
-        self.obj  = obj
-        self.prop = prop
+        self._bound = False
 
-        self.bound = False
-
-        self.widget:           Widget = None
-        self.ctrl_var:         T.Variable = None
-        self.after_change_cbk: Callable = None
-        self.cbk_n_args:       int = None
-
-        self.image:            ImageTk.PhotoImage = None
-        self.image_width:      int = None
-        self.image_height:     int = None
-        self.attr_chain_to_holder: str = None
-        self.widget_attribute: str = None
-        self.widget_option:    str = None
+        self._obj  = obj
+        self._prop = prop
+        self._widget:           Widget = None
+        self._ctrl_var:         T.Variable = None
+        self._after_change_cbk: Callable = None
+        self._cbk_n_args:       int = None
+
+        self._image:            ImageTk.PhotoImage = None
+        self._image_width:      int = None
+        self._image_height:     int = None
+        self._attr_chain_to_holder: str = None
+        self._widget_attribute: str = None
+        self._widget_option:    str = None
         # self.auto_resize_widget_on_image: bool = None
 
 
     def __make_fresh_binder(self, **kw) -> 'Binder':
+        # NO DOCSTRING otherwise the method shows up in the docs
         # Create  copy of the current instance, adding the given arguments.
         # Ensure that no previous arguments are overridden.
-        #
+        # Any keyword argument associated to None will be ignored.
         # NOTE: the fresh instance is mutated to keep as few arguments as possible for the
         #      __init__ method (makes it easier to use with IDE suggestions).
-        #
+
         fresh  = Binder()
         stored = {
-            'obj': self.obj,
-            'prop': self.prop,
-            'bound': self.bound,
-            'widget': self.widget,
-            'ctrl_var': self.ctrl_var,
-            'after_change_cbk': self.after_change_cbk,
-            'cbk_n_args': self.cbk_n_args,
-            'image': self.image,
-            'image_width': self.image_width,
-            'image_height': self.image_height,
-            # 'auto_resize_widget_on_image': self.auto_resize_widget_on_image,
-            'attr_chain_to_holder': self.attr_chain_to_holder,
-            'widget_attribute': self.widget_attribute,
-            'widget_option': self.widget_option,
+            'obj': self._obj,
+            'prop': self._prop,
+            'bound': self._bound,
+            'widget': self._widget,
+            'ctrl_var': self._ctrl_var,
+            'after_change_cbk': self._after_change_cbk,
+            'cbk_n_args': self._cbk_n_args,
+            'image': self._image,
+            'image_width': self._image_width,
+            'image_height': self._image_height,
+            'attr_chain_to_holder': self._attr_chain_to_holder,
+            'widget_attribute': self._widget_attribute,
+            'widget_option': self._widget_option,
+            # 'auto_resize_widget_on_image': self.auto_resize_widget_on_image,  # doesn't work...
         }
-        if not all(stored[k] is None for k in kw):
-            raise BinderError("Cannot redefine one of those arguments: "+', '.join(map(repr,kw)))
 
-        for k,value in {**stored, **kw}.items():
-            setattr(fresh, k, value)
+        valid_kw     = {k:v for k,v in kw.items() if v is not None}
+        already_done = [k for k in valid_kw if stored[k] is not None]
+        if already_done:
+            raise BinderError(
+                "Those arguments/properties have already been defined: "
+                + ', '.join(already_done)
+            )
+
+        for k,value in {**stored, **valid_kw}.items():
+            setattr(fresh, '_'+k, value)
         return fresh
 
 
     #----------------------------------------------------------------------
 
 
-
     @unbound_only
     def of(self, obj:Any) -> 'Binder':      # pylint: disable=invalid-name
-        """ Register the targeted object (model layer of the application), when not given through
-            the constructor.
+        """ Legacy behavior. See [Binder.for_][src.tkutils.two_way_binding.binder.Binder.for_].
+        """
+        check_hashable(obj)
+        return self.__make_fresh_binder(obj=obj)
+
+
+
+    @unbound_only
+    def for_(self, obj:Any, prop:str=None) -> 'Binder':
+        """ Register the targeted object (model layer of the application) when not given through
+            the constructor, and possibly the target property.
 
             Parameters:
                 obj: The object instance to bind (must be hashable).
+                prop: Name of the property to bind.
 
             Raises:
                 BinderError:    If the object instance has already been registered
+                BinderError:    If the property name has already been registered
                 BindingError:   If the object it is not hashable
 
             Returns:
                 A new `Binder` instance with the property name added.
         """
         check_hashable(obj)
-        return self.__make_fresh_binder(obj=obj)
+        return self.__make_fresh_binder(obj=obj, prop=prop)
 
 
 
     @unbound_only
     def for_property(self, prop:str) -> 'Binder':
         """ Register the property name info (for the targeted object), when not given
             through the constructor.
@@ -299,85 +315,128 @@
             widget_attribute=widget_attribute,
             widget_option=widget_option,
         )
 
 
 
     @unbound_only
-    def after_change(self, after_change_cbk:Callable) -> 'Binder':
-        """ Register the "after change" callback that will update the GUI.
+    def after_change(
+        self,
+        after_change_cbk: Callable,
+        *,
+        chain: Literal['after','before'] = None,
+    ) -> 'Binder':
+        """ Register an "after change" callback that will propagate updates after a modification.
+            If a callback has already been registered for the current Binder instance, it is
+            possible to cumulate it with a new one by using the optional `chain` argument, which
+            will determine the order of executions of the two callbacks.
 
             Different signatures can be used:
 
-            * `after_change() -> None`
-
-                No argument
-
-            * `after_change(new_value:Any) -> None`
-
-                Receives the value  of the bound property after it has been updated
-
-            * `after_change(new_value:Any, model:Object, widget:T.Widget) -> None`
-
-                Receives the value  of the bound property after it has been updated
+            | Call signature | Type |
+            |:-|:-|
+            | `after_change()`                         | `Callable[[],None]` |
+            | `after_change(new_value)`                | `Callable[[Any],None]` |
+            | `after_change(new_value, model, widget)` | `Callable[[Any,Object,Widget],None]` |
 
             The correct signature to use will be determined through inspection, so the user does
             not have to care about putting default arguments when defining a callback of the
             simplest form.
 
-            Arguments will always be passed as positional arguments, so you can use keyword only
-            arguments to pass extra constant values to the function if you need it.
-
-            !!! warning
-                Positional arguments with default value _will_ be overwritten at call time, if they
-                are in first, second or third position. Enforce the use of keyword arguments to
-                avoid this behavior: `cbk(value, *, my_default=42)`.
+            ??? tip "Passing extra values to the callbacks"
+                * The arguments that will be passed at call time will always be positional
+                arguments, so you can use keyword __only__ arguments to pass extra constant
+                values to the function if you need it:
+
+                    `def after_change(new_value, model, widget, *, cte=42): ...`
+
+                * Any positional arguments with default value _will_ be overwritten at call time,
+                if they are in first, second or third position. If you want to use less than three
+                explicit arguments, or no varargs, enforce the use of a _keyword only_ arguments
+                to avoid this problem: `cbk(value, *, my_default=42)`.
 
             Parameters:
                 after_change_cbk:
                     Consumer callback, to apply various updates that should occur after
                     a change, either `Callable[[],None]`, `Callable[[Any],None]` or
                     `Callable[[Any,Object,T.Widget],None]`.
+                chain:
+                    If used, an after_change callback must have been already registered on the
+                    Binder and the new callback will be called before or after it.
 
             Raises:
-                BinderError: If the callback has already been registered
-                ValueError:  If the `after_change_cbk` argument is not callable
-                ValueError:  If the callback signature cannot be determined or is not compatible
+                BinderError: If the callback has already been registered and `chain` isn't used.
+                ValueError:  If the `after_change_cbk` argument is not callable.
+                ValueError:  If the callback signature cannot be determined or is not compatible.
+                ValueError:  If the `chain` argument is used but is not `"before"` or `"after"`.
+                ValueError:  If the `chain` argument is used but no callback is already set.
 
             Returns:
                 A new `Binder` instance with the callback added.
         """
+        if chain is None and self._after_change_cbk:
+            raise BinderError(
+                "An after_change callback has already been registered, but the chain argument "
+                "has not been used with the given callback. this is either a mistake, or the "
+                'chain argument must be used (possible values: "before", "after").'
+            )
         if not callable(after_change_cbk):
             raise ValueError("after_change_cbk must be callable")
 
         counted_param_kinds = (
             Parameter.POSITIONAL_ONLY,
             Parameter.POSITIONAL_OR_KEYWORD,
             Parameter.VAR_POSITIONAL,
         )
-        cbk_n_args = 0
-        if after_change_cbk:
-            cbk_params = signature(after_change_cbk).parameters
-            args       = [ p for p in cbk_params.values() if p.kind in counted_param_kinds ]
-
-            cbk_n_args = len(args)
-            if args and args[-1].kind == Parameter.VAR_POSITIONAL:
-                # If vararg are used, always pass the 3 arguments
-                cbk_n_args = max(3, cbk_n_args)
+
+        cbk_params = signature(after_change_cbk).parameters
+        args       = [ p for p in cbk_params.values() if p.kind in counted_param_kinds ]
+        cbk_n_args = len(args)
+
+        # If varargs are used, always pass 3 arguments:
+        if args and args[-1].kind == Parameter.VAR_POSITIONAL:
+            cbk_n_args = max(3, cbk_n_args)
 
         if cbk_n_args==2 or cbk_n_args>3:
             raise ValueError(
-                "The after_change callback should take either 0, 1 or 3 positional arguments, "
+               "The after_change callback should take either 0, 1 or 3 positional arguments, "
             + f"but those where found for the callback { after_change_cbk.__name__ }:"
-            + "".join(f'\n\t{p.name}: {p.kind}' for p in args)
-            + '\nOther arguments present:'
+            +  "".join(f'\n\t{p.name}: {p.kind}' for p in args)
+            +  '\nOther arguments present:'
             + ( "".join(f'\n\t{p.name}: {p.kind}' for p in args if p not in args)
                 or "\n\tNone" )
             )
 
+        if chain is not None:
+            if chain not in ('before','after'):
+                raise ValueError(f"Invalid chain argument value: { chain !r}")
+            if not self._after_change_cbk:
+                raise ValueError(
+                    "Cannot chain after_change_cbk without any previously registered callback"
+                )
+
+            # Define merged behaviors:
+            def merged_cbk(val, obj, widget):
+                """ Merged after_change callback """
+                if chain=='before':
+                    self.__run_after_change_cbk(after_change_cbk, cbk_n_args, val, obj, widget)
+
+                self.__run_after_change_cbk(
+                    self._after_change_cbk, self._cbk_n_args, val, obj, widget
+                )
+
+                if chain=='after':
+                    self.__run_after_change_cbk(after_change_cbk, cbk_n_args, val, obj, widget)
+
+            # Create and return the appropriated Binder, but without mutating the current instance:
+            binder                  = self.__make_fresh_binder()
+            binder._after_change_cbk = merged_cbk               # pylint: disable=protected-access
+            binder._cbk_n_args       = 3                        # pylint: disable=protected-access
+            return binder
+
         return self.__make_fresh_binder(
             after_change_cbk = after_change_cbk,
             cbk_n_args       = cbk_n_args,
         )
 
 
 
@@ -407,17 +466,18 @@
                 ValueError: For invalid dimensions arguments, or FileNotFoundError if the
                             filename or the path is invalide.
 
             Returns:
                 A new `Binder` instance with the callback added.
         """
         image_from = get_image_factory()
-        image, width, height = image_from(          # pylint: disable=not-callable   # dafuck!?! x/
+        out = image_from(          # pylint: disable=not-callable   # dafuck!?! x/
             file, width=width, height=height, size=size
         )
+        image, width, height = out
         return self.__make_fresh_binder(
             image=image, image_width=width, image_height=height,
             # auto_resize_widget_on_image=auto_resize_widget_on_image
         )
 
 
 
@@ -464,32 +524,32 @@
                                            parent, or if some information cannot be found for the
                                            widget/object.
 
             Returns:
                 The bound widget instance, with the initial value set to the bound object property.
 
         """
-        if self.obj is None:
+        if self._obj is None:
             raise BinderError("No object instance to bind to.")
 
-        if self.prop is None:
+        if self._prop is None:
             raise BinderError("No property to bind to.")
 
-        if self.widget is None:
+        if self._widget is None:
             raise BinderError("No widget to bind to.")
 
-        if not isinstance(self.ctrl_var, T.Variable):
+        if not isinstance(self._ctrl_var, T.Variable):
             raise BindingCtrlVarError(
-                f"Couldn't extract or build a control variable instance: ctrl_var={self.ctrl_var}"
+                f"Couldn't extract or build a control variable instance: ctrl_var={self._ctrl_var}"
             )
 
-        self.bound = True           # Lock the Binder instance
+        self._bound = True           # Lock the Binder instance
         self.__attach_image()
         self.__handle_ctrl_var_and_reactivity()
-        return self.widget
+        return self._widget
 
 
 
 
 
 
 
@@ -497,37 +557,37 @@
 
 
 
 
 
 
     def __attach_image(self):
-        if not self.image: return                       # pylint: disable=multiple-statements
+        if not self._image: return                       # pylint: disable=multiple-statements
 
-        self.widget._image_ref_to_avoid_GC = self.image   # pylint: disable=protected-access
-        self.widget.config(image=self.image)
+        self._widget._image_ref_to_avoid_GC = self._image   # pylint: disable=protected-access
+        self._widget.config(image=self._image)
 
         # Doesn't work
         # if self.auto_resize_widget_on_image:
         #     self.widget.config(width = self.image_width,
         #                        height= self.image_height)
 
 
 
     def __handle_ctrl_var_and_reactivity(self):
 
         ctrl_var_holder = CtrlVarWidgetPathToHolder.extract(
-            self.widget, attr_chain_to_holder=self.attr_chain_to_holder
+            self._widget, attr_chain_to_holder=self._attr_chain_to_holder
         )
 
         CtrlVarHolderAttribute.assign(
             ctrl_var_holder,
-            self.ctrl_var,
-            self.widget_attribute,
-            self.widget_option,
+            self._ctrl_var,
+            self._widget_attribute,
+            self._widget_option,
         )
 
         flash_on_error = flasher(ctrl_var_holder, 2, 100)
         stack_level = 0
 
         def two_ways_setter(val):
             """ Multi-setter callback: allow to update the control variable and/or the targeted
@@ -538,90 +598,95 @@
             """
             nonlocal stack_level
 
             if not BinderConfig.limit_stack:
                 stack_level = 1
             else:
                 stack_level += 1
-                if stack_level>2:
+                if stack_level > BinderConfig.stack_max_depth:
                     raise OverflowError(
                         '\nIt looks like the two-way binding will run into infinite recursion. '
                         'If you are certain it will not be the case, you can set '
                         'BinderConfig.limit_stack to False.\n'
                         'Binding involving:\n'
-                        f'\tModel: { self.obj.__class__.__name__ }.{ self.prop }\n'
-                        f'\tGUI: { self.widget.__class__.__name__ }\n'
+                        f'\tModel: { self._obj.__class__.__name__ }.{ self._prop }\n'
+                        f'\tGUI element: { self._widget.__class__.__name__ }\n'
                     )
 
             try:
                 changed = False
-                current_ctrl = self.ctrl_var.get()
+                current_ctrl = self._ctrl_var.get()
                 if current_ctrl != val:
                     changed = True
-                    self.ctrl_var.set(val)
+                    self._ctrl_var.set(val)
                     # print(f'set {self.prop} ctrl_var to: {val}')
 
-                current_obj = getattr(self.obj, self.prop)
+                current_obj = getattr(self._obj, self._prop)
                 if current_obj != val:
                     changed = True
-                    setattr(self.obj, self.prop, val)
+                    setattr(self._obj, self._prop, val)
                     # print(f'set {self.obj.__class__.__name__}.{self.prop} to: {val}')
 
-                if changed and self.after_change_cbk:
-                    # pylint: disable=not-callable
-                    if not self.cbk_n_args:
-                        self.after_change_cbk()
-                    elif self.cbk_n_args==1:
-                        self.after_change_cbk(val)
-                    else:
-                        self.after_change_cbk(val, self.obj, self.widget)
+                if changed and self._after_change_cbk:
+                    self.__run_after_change_cbk(
+                        self._after_change_cbk, self._cbk_n_args, val, self._obj, self._widget
+                    )
 
             except T.TclError:
                 flash_on_error()
             stack_level -= 1
 
 
         #----------------------------------------------------
 
 
         def safe_tracer(*_):
             """ Relay callback used for ctrl_var.trace_add (which stupidly receives useless
                 arguments instead of the value itself...)
             """
             try:
-                val = self.ctrl_var.get()
+                val = self._ctrl_var.get()
                 two_ways_setter(val)
             except T.TclError:
                 flash_on_error()
 
 
         # Bind, way 1: the control variable itself:
-        self.ctrl_var.trace_add('write', callback=safe_tracer)
+        self._ctrl_var.trace_add('write', callback=safe_tracer)
 
 
         # Bind, way 2: put the Descriptor in place on the object property, or update it:
-        desc = BindingDescriptor.bind(self.obj, self.prop, two_ways_setter, self.widget)
+        desc = BindingDescriptor.bind(self._obj, self._prop, two_ways_setter, self._widget)
 
 
         # Hack the widget destroy method to automatically unsubscribe from the BindingDescriptor:
         def two_ways_destroyer():
-            desc.unsubscribe_on_destroy(self.widget)
+            desc.unsubscribe_on_destroy(self._widget)
             old_destroy()
 
-        old_destroy = self.widget.destroy
-        self.widget.destroy = two_ways_destroyer
+        old_destroy = self._widget.destroy
+        self._widget.destroy = two_ways_destroyer
 
 
         # Set initial state, triggering the control variable with the current object value:
-        value = getattr(self.obj,self.prop)
-        self.ctrl_var.set(value)
+        value = getattr(self._obj,self._prop)
+        self._ctrl_var.set(value)
+
 
 
 
 
+    @staticmethod
+    def __run_after_change_cbk(cbk:Callable, n_args:int, val:Any, obj:Any, widget:T.Widget):
+        if not n_args:
+            cbk()
+        elif n_args==1:
+            cbk(val)
+        else:
+            cbk(val, obj, widget)
```

### Comparing `tkutils-1.0.0/src/tkutils/two_way_binding/binding_descriptor.py` & `tkutils-1.1.0/src/tkutils/two_way_binding/binding_descriptor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 
 
-
 import tkinter as T
+import inspect
+from contextlib import suppress
 
 from typing import Any, Callable, Dict, DefaultDict, Set
 from collections import defaultdict
 
 from .errors import BindingError
 
 
@@ -185,15 +186,15 @@
                 raise AttributeError(f'Cannot delete attribute {self.patched_property} on {obj}')
 
 
 
 
     # WEAKREFS!?
     def subscribe(self, obj, widget, two_ways_cbk):
-        """ Register the two way bindig for the given association ("model -> GUI way") """
+        """ Register the two way binding for the given association ("model -> GUI way") """
         self._bindings[obj][widget] = two_ways_cbk
         self._unbindings[widget].add(obj)
 
 
     def unsubscribe(self, obj:Any, widget:T.Widget):
         """ Remove the update callback for the given association from the descriptor register """
         del self._bindings[obj][widget]
@@ -213,15 +214,16 @@
 
     @classmethod
     def bind(cls,                       # pylint: disable=too-many-locals
              instance:Any,
              prop:str,
              two_ways_cbk:Callable[[Any],None],
              widget:T.Widget
-    ) -> 'BindingDescriptor':
+    # ) -> 'BindingDescriptor':
+    ):
         """ Set up the two-way binding logic for the given object/class and widget, meaning:
 
             - patch the class property with a BindingDescriptor if not already done
             - secure current state of this property to not lose any data
             - set up the callback so that the widget is updated after a property update
             - return the BindingDescriptor so that the widget.destroy method can be
                 hacked to trigger unsubscription (this isn't done in the current function
@@ -237,84 +239,91 @@
                 f"Attempt to bind {instance.__name__}.{prop}:\n"
                 "Binding a class level property isn't allowed if the class is directly derived "
                 "from the builtin type function. An intermediate metaclass has to be defined."
             )
 
         kls = instance.__class__
 
-        # State of what's currently on the class body and on the instance itself
+        # State of what's currently on the on the instance itself:
         instance_attributes      = vars(instance)
         has_instance_level_value = prop in instance_attributes
         instance_level_value     = instance_attributes.get(prop,None)
 
-        kls_attributes        = vars(kls)
-        has_kls_level_value   = prop in kls_attributes
-        kls_level_value       = kls_attributes.get(prop,None)
-
-        is_descriptor = has_kls_level_value and bool(
-            cls.DESCRIPTOR_SPECIFIC_METHODS_SET & set( dir(kls_attributes[prop]) )
-        )
-        is_binder_descriptor  = isinstance(kls_level_value, BindingDescriptor)
-        is_kls_level_property = not is_descriptor and has_kls_level_value
+
+        # State of what's currently on the on the parent class (strictly):
+        kls_attributes         = vars(kls)
+        has_something_on_class = prop in kls_attributes
+        kls_level_value        = kls_attributes.get(prop,None)
+        already_bound          = isinstance(kls_level_value, BindingDescriptor)
+
+        # Search for any descriptor at a parent level of the instance (any depth):
+        upper_value    = None
+        has_descriptor = False
+        with suppress(AttributeError):
+            upper_value = inspect.getattr_static(instance,prop)
+            has_descriptor = bool(
+                cls.DESCRIPTOR_SPECIFIC_METHODS_SET & set( dir(upper_value) )
+            )
+
+        is_kls_level_value = has_something_on_class and not already_bound
 
 
         # Binder descriptor to use:
-        binder = kls_level_value if is_binder_descriptor else cls(prop, kls)
+        binder = kls_level_value if already_bound else cls(prop, kls)
 
 
-        if not is_binder_descriptor:        # No Binding yet!
+        if not already_bound:        # No Binding yet!
 
-            if is_descriptor:               # Just archive it for __get__ accesses...
-                binder.inner_descriptor = kls_level_value
+            if has_descriptor:               # Just archive it for __get__/... access
+                binder.inner_descriptor = upper_value
 
             else:
                 # Enforce prefixed property name availability:
-                prefixed_name_defined   = binder.prefixed_property in instance_attributes
+                defined_prefixed_name   = binder.prefixed_property in instance_attributes
                 annotations             = kls_attributes.get('__annotations__', ())
                 annotated_prefixed_name = binder.prefixed_property in annotations
-                if prefixed_name_defined or annotated_prefixed_name:
+                if defined_prefixed_name or annotated_prefixed_name:
                     raise BindingError(
                         f"{binder.prefixed_property} must be available on the class/instance "
                         "without collisions to put a two-way binding in place."
                     )
 
-                # Backup any existing instance level value:
+                # Backup any existing instance level value then remove so that property access will
+                # reach the BindingDescriptor :
                 if has_instance_level_value:
-                    # WARNING: an instance could have overridden the class level definition!
-                    # So prepare instance level prefixed property as well, if needed
                     setattr(instance, binder.prefixed_property, instance_level_value)
-
                     delattr(instance, binder.patched_property)
-                    # ^ <<< "clean up the place"
-                    # NOTE: implementation of __get__ was using `super(typ,typ)` => doesn't work.
 
-                # Backup default value defined at class level if any:
-                if is_kls_level_property:
+
+                # An instance could have overridden a class level definition which would get removed
+                # by the BindingDescriptor, or could be needed as default for unbound instances
+                # => backup default value defined at class level (strictly) if any:
+                if is_kls_level_value:
                     setattr(kls, binder.prefixed_property, kls_level_value)
                     # No need to delete the class attribute: replaced with the binder anyway...
 
 
-            parent_dct   = dict(vars(kls.__class__))
-            parent_level = parent_dct.get(prop)
-            is_lower_level_binding = isinstance(parent_level, BindingDescriptor)
+            # Check for any "multilevel binding" (ie. doing instance level binding now, while
+            # a class level binding has already been done before on the same property):
+            meta_dct         = dict(vars(kls.__class__))    # dict(mappingproxy) ...
+            meta_value       = meta_dct.get(prop)
+            has_meta_binding = isinstance(meta_value, BindingDescriptor)
 
             # Hot patch the new descriptor on the class:
-            if is_lower_level_binding:
-                # Currently trying to setup a binding on an instance of the currently bound class
-                # (meaning a class level binding is currently running, and an instance level is
-                # being setup right now). The current descriptor logic forbids to put in place the
-                # new binding, so:
-                #       - Remove temporarily the current BindingDescriptor on the metaclass
-                #       - Put the wanted binding in place
-                #       - Put back the BindingDescriptor (ie. self!) on the metaclass
-
+            if has_meta_binding:
+                # The current setup (descriptor on the parent class of kls, ie a metaclass)
+                # forbids to put in place the new binding, so:
+                #   - Remove temporarily the current BindingDescriptor on the metaclass
+                #   - Put the wanted binding in place
+                #   - Put back the BindingDescriptor on the metaclass
                 delattr(kls.__class__, prop)
                 setattr(kls, prop, binder)
-                setattr(kls.__class__, prop, parent_level)
+                setattr(kls.__class__, prop, meta_value)
 
             else:
                 setattr(kls, prop, binder)
 
 
-        # Activate the Model -> GUI binding, at last:
+        # Activate the Model -> GUI binding:
         binder.subscribe(instance, widget, two_ways_cbk)
+
         return binder
```

### Comparing `tkutils-1.0.0/src/tkutils/two_way_binding/configuration/_binder_config.py` & `tkutils-1.1.0/src/tkutils/two_way_binding/configuration/_binder_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,19 @@
 
 
     limit_stack = True
     """ If True, an OverflowError is raised if an infinite recursion is suspected during the
         two-way binding updates. This behavior can be turned off by updating this attribute.
     """
 
+    stack_max_depth = 2
+    """ Define the stack depth that is triggering the error, when the two_way_binding
+        callback is running.
+    """
+
 
 
     @staticmethod
     def nested_component(widget_type:Type, attr_chain_to_holder:str):
         """ Register a configuration for a custom component/widget whose one of the children is
             actually holding the desired control variable.
 
@@ -99,15 +104,15 @@
         default_ctrl_var_type:    Type[T.Variable],
         *,
         widget_attribute: str = None,
         widget_option:   str = None,
     ) -> None :
         """ For a custom widget/component that _is holding_ (directly) a control variable.
 
-            This method allows to register the informations to know how/where the `Binder` has to
+            This method allows to register the information to know how/where the `Binder` has to
             "plug in" the control variable instance on the widget.
 
             !!! warning
                 * The object _directly holding_ the control variable is to be configured (see
                   [`BinderConfig.nested_component`][src.tkutils.two_way_binding.configuration._binder_config.BinderConfig.nested_component]).
                 * Settings are identified using the class name of the registered widget
                   (`widget_type.__name__`)
@@ -214,19 +219,19 @@
 
 
     @staticmethod
     def show_images_location(returns=False):
         """ Print the current image factory configuration to the console or return it if
             `returns=True`.
         """
+        location = repr(get_image_factory_config_location())
+        location = location.replace('\\\\', '\\')               # windows specific
         msg = (
             _title("Current images location for Binder.with_image(...) factory", returns)
-                    + '\n\n    '
-                    + repr(get_image_factory_config_location())
-                    + "\n"
+                    + f'\n\n    { location }\n'
         )
         print(msg)
         return msg if returns else None
```

### Comparing `tkutils-1.0.0/src/tkutils/two_way_binding/configuration/_configuration.py` & `tkutils-1.1.0/src/tkutils/two_way_binding/configuration/_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
 
 class CtrlVarWidgetPathToHolder(_CtrlVarHandler):
     """ Gives the "path" to the nested widget holding the control variable to assign to,
         for the binding operations.
 
         All usual widgets are defined (even if they hold the default value as path: "") so that
-        they are locked and the user would have to create custom components to bve able to do
+        they are locked and the user would have to create custom components to be able to do
         something unexpected.
     """
     _configurer_arg_name = "BinderConfig.nested_component(..., attr_chain_to_holder)"
 
     Button            = ''
     Checkbutton       = ''
     Combobox          = ''
```

### Comparing `tkutils-1.0.0/src/tkutils/two_way_binding/configuration/_configurer_image_factory.py` & `tkutils-1.1.0/src/tkutils/two_way_binding/configuration/_configurer_image_factory.py`

 * *Files identical despite different names*

### Comparing `tkutils-1.0.0/src/tkutils/two_way_binding/errors.py` & `tkutils-1.1.0/src/tkutils/two_way_binding/errors.py`

 * *Files identical despite different names*

### Comparing `tkutils-1.0.0/src/tkutils/utilities/singleton_namespace.py` & `tkutils-1.1.0/src/tkutils/utilities/singleton_namespace.py`

 * *Files identical despite different names*

### Comparing `tkutils-1.0.0/setup.py` & `tkutils-1.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,109 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: tkutils
+Version: 1.1.0
+Summary: Python tkinter utilities.
+Home-page: http://frederic.zinelli.gitlab.io/tkutils/
+License: FreeBSD
+Author: Frédéric Zinelli
+Author-email: frederic.zinelli@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Pillow (>=9.3.0,<10.0.0)
+Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
+Project-URL: Repository, https://gitlab.com/frederic.zinelli/tkutils
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# Welcome to TkUtils
 
-packages = \
-['tkutils',
- 'tkutils.helpers',
- 'tkutils.menu_builder',
- 'tkutils.two_way_binding',
- 'tkutils.two_way_binding.configuration',
- 'tkutils.utilities']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['Pillow>=9.3.0,<10.0.0', 'typing-extensions>=4.4.0,<5.0.0']
-
-entry_points = \
-{'console_scripts': ['essai = project_debug:routing',
-                     'main = tkutils.__main__:main']}
-
-setup_kwargs = {
-    'name': 'tkutils',
-    'version': '1.0.0',
-    'description': 'Python tkinter utilities.',
-    'long_description': '# Welcome to TkUtils\n\n`tkutils` is a package offering some additional logic and syntactic sugar when using tkinter.\nThe main goal is to fill some gaps of tkinter, which might make it very annoying to use.\n\nOnline version of the help documentation: http://frederic.zinelli.gitlab.io/tkutils/\n\n\n\n## Features\n\n\n### Additional logic: two-way binding with [`Binder`](http://frederic.zinelli.gitlab.io/tkutils/binder/binder_overview/)\n\nThe [`Binder`](http://frederic.zinelli.gitlab.io/tkutils/binder/binder_overview/) class is an utility to setup a transparent two-way\nbinding reactivity between widgets and underlying object properties from the model/logic layer\nof the application.\n\nSeveral advantages come with this:\n\n* Changes of bound properties in the model layer are cascading in the GUI automatically.\n* The model layer of the application becomes (finally) totally independent from the presentation\n  layer. This means it becomes very easy to build and test the model layer, without any need to\n  think about its integration with `tkinter` itself.\n\n\n\n### Syntactic sugar\n\n\n#### [`GridLayout`](http://frederic.zinelli.gitlab.io/tkutils/grid_layout/grid_layout/)\n\nA grid layout manager which is abstracting away all the naughty `widget.grid(...)` calls and\nrows/columns grid configuration. Positioning widgets in the grid and controlling their "spanning"\nbecomes very easy, without extra typing.\n\n\n#### [`MenuBuilder`](http://frederic.zinelli.gitlab.io/tkutils/menu_builder/menu_builder/)\n\nA helper to build menus and to abstract away all the technicalities, when creating menus through\n`tkinter`, which quickly make the declarations very unclear. Using the [`MenuBuilder`](http://frederic.zinelli.gitlab.io/tkutils/menu_builder/menu_builder/),\nthe actual Menu hierarchy becomes very obvious: "what you see is what you get".\n\n\n#### [`Event`](http://frederic.zinelli.gitlab.io/tkutils/event/)\n\nAn utility to build event strings with autocompletion/IDE suggestions support.\n\n\n#### [`KeySym`](http://frederic.zinelli.gitlab.io/tkutils/key_sym/)\n\nAn utility to get all keysym informations with autocompletion/IDE suggestions (providing string,\nkeycode and keysym_num values).\n\n\n#### [`images`](http://frederic.zinelli.gitlab.io/tkutils/images/images/)\n\nVarious factories related to images to:\n\n* Simplify and reduce the syntaxes/typing needed,\n* Handle file conversions automatically,\n* Register automatically the image object on the host for the user (to avoid garbage collection).\n\n\n\n\n## Requirements\n\n- python 3.8+\n- Pillow\n\n\n\n## Installation\n\n* Through [PyPi](https://pypi.org/project/tkutils/):\n\n```bash\npip install tkutils\n```\n\n* Using an archive file (with the appropriate version number):\n\n```bash\npip install tkutils.1.0.2.tar.gz\n```\n\n* Cloning the [GitLab repository](https://gitlab.com/frederic.zinelli/tkutils).\n\n',
-    'author': 'Frédéric Zinelli',
-    'author_email': 'frederic.zinelli@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'http://frederic.zinelli.gitlab.io/tkutils/',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+`tkutils` is a package offering some additional logic and syntactic sugar when using `tkinter`.
+The main goal is to fill some gaps of tkinter, which might make it very annoying to use.
+
+Online version of the help documentation: http://frederic.zinelli.gitlab.io/tkutils/
+
+
+
+## Features
+
+
+### Additional logic: two-way binding, with [`Binder`](http://frederic.zinelli.gitlab.io/tkutils/binder/binder_overview/)
+
+The [`Binder`](http://frederic.zinelli.gitlab.io/tkutils/binder/binder_overview/) class is  to setup a transparent two-way
+binding reactivity between widgets and underlying object properties from the model/logic layer
+of the application.
+
+Several advantages come with this:
+
+* Changes of bound properties in the model layer are cascading in the GUI automatically.
+* The model layer of the application becomes (finally) totally independent from the presentation
+  layer. This means it becomes very easy to build and test the model layer, without any need to
+  think about its integration with `tkinter` itself.
+
+
+
+### Syntactic sugar
+
+
+#### [`GridLayout`](http://frederic.zinelli.gitlab.io/tkutils/grid_layout/grid_layout/)
+
+A grid layout manager which is abstracting away all the naughty `widget.grid(...)` calls and
+rows/columns grid configuration. Positioning widgets in the grid and controlling their "spanning"
+becomes very easy, without extra typing.
+
+
+#### [`MenuBuilder`](http://frederic.zinelli.gitlab.io/tkutils/menu_builder/menu_builder/)
+
+A helper to build menus and to abstract away all the technicalities encountered when creating menus through
+`tkinter`, which quickly make the declarations very unclear. Using the [`MenuBuilder`](http://frederic.zinelli.gitlab.io/tkutils/menu_builder/menu_builder/), the actual `Menu` hierarchy becomes very obvious: "what you see is what you get".
+
+
+#### [`Event`](http://frederic.zinelli.gitlab.io/tkutils/event/)
+
+A utility to build event strings with auto-completion/IDE suggestions support.
+
+
+#### [`KeySym`](http://frederic.zinelli.gitlab.io/tkutils/key_sym/)
+
+A utility to get all keysym information with auto-completion/IDE suggestions (providing string,
+keycode and keysym_num values).
+
+
+#### [`images`](http://frederic.zinelli.gitlab.io/tkutils/images/images/)
+
+Various factories related to images to:
+
+* Simplify and reduce the typing needed,
+* Handle file conversions automatically,
+* Register automatically the image object on the host for the user (to avoid garbage collection).
+
+
+
+
+## Requirements
+
+- python 3.8+
+- Pillow
+
+
+
+## Installation
+
+* Through [PyPi](https://pypi.org/project/tkutils/):
+
+```bash
+pip install tkutils
+```
+
+* Using an archive file (with the appropriate version number):
+
+```bash
+pip install tkutils.1.0.2.tar.gz
+```
+
+* Cloning the [GitLab repository](https://gitlab.com/frederic.zinelli/tkutils).
 
 
-setup(**setup_kwargs)
```

