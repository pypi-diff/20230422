# Comparing `tmp/SunsetSettings-0.4.0.tar.gz` & `tmp/SunsetSettings-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SunsetSettings-0.4.0.tar", last modified: Thu Mar 23 00:24:24 2023, max compression
+gzip compressed data, was "SunsetSettings-0.5.0.tar", last modified: Sat Apr 22 19:52:25 2023, max compression
```

## Comparing `SunsetSettings-0.4.0.tar` & `SunsetSettings-0.5.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1698 2023-01-16 00:48:03.487746 SunsetSettings-0.4.0/.github/workflows/python-build.yml
--rw-r--r--   0        0        0       59 2022-08-04 10:12:23.781547 SunsetSettings-0.4.0/.gitignore
--rw-r--r--   0        0        0      233 2022-12-14 00:54:21.154949 SunsetSettings-0.4.0/.readthedocs.yml
--rw-r--r--   0        0        0    32422 2022-03-24 23:57:25.474661 SunsetSettings-0.4.0/LICENSE
--rw-r--r--   0        0        0     6009 2023-03-17 15:03:13.303453 SunsetSettings-0.4.0/README.md
--rw-r--r--   0        0        0      638 2022-08-04 10:11:43.364138 SunsetSettings-0.4.0/docs/Makefile
--rw-r--r--   0        0        0      804 2022-08-04 10:11:43.364138 SunsetSettings-0.4.0/docs/make.bat
--rw-r--r--   0        0        0     1123 2023-03-22 17:17:46.547875 SunsetSettings-0.4.0/docs/source/api.rst
--rw-r--r--   0        0        0     1598 2023-03-23 00:18:12.232742 SunsetSettings-0.4.0/docs/source/changelog.rst
--rw-r--r--   0        0        0     2476 2022-12-19 01:40:30.636872 SunsetSettings-0.4.0/docs/source/conf.py
--rw-r--r--   0        0        0      788 2023-01-16 22:21:36.070670 SunsetSettings-0.4.0/docs/source/index.rst
--rw-r--r--   0        0        0      613 2022-11-20 03:11:09.133654 SunsetSettings-0.4.0/docs/source/installation.rst
--rw-r--r--   0        0        0    15649 2023-03-22 22:27:10.846045 SunsetSettings-0.4.0/docs/source/usage.rst
--rw-r--r--   0        0        0     1314 2022-12-19 15:06:00.615479 SunsetSettings-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1015 2023-03-23 00:23:33.468601 SunsetSettings-0.4.0/sunset/__init__.py
--rw-r--r--   0        0        0     7757 2023-03-17 16:41:24.564662 SunsetSettings-0.4.0/sunset/autosaver.py
--rw-r--r--   0        0        0    10220 2023-03-17 15:03:15.059518 SunsetSettings-0.4.0/sunset/bunch.py
--rw-r--r--   0        0        0     4153 2022-12-19 19:56:34.571579 SunsetSettings-0.4.0/sunset/exporter.py
--rw-r--r--   0        0        0    11970 2022-12-28 19:48:13.732822 SunsetSettings-0.4.0/sunset/key.py
--rw-r--r--   0        0        0    15017 2023-03-17 15:09:28.953390 SunsetSettings-0.4.0/sunset/list.py
--rw-r--r--   0        0        0      942 2022-12-14 00:56:18.711048 SunsetSettings-0.4.0/sunset/lockable.py
--rw-r--r--   0        0        0     1975 2022-10-03 01:11:58.016811 SunsetSettings-0.4.0/sunset/non_hashable_set.py
--rw-r--r--   0        0        0     4448 2023-03-22 18:31:19.752117 SunsetSettings-0.4.0/sunset/protocols.py
--rw-r--r--   0        0        0        0 2022-04-05 17:36:11.873451 SunsetSettings-0.4.0/sunset/py.typed
--rw-r--r--   0        0        0     2392 2022-12-14 00:56:18.711048 SunsetSettings-0.4.0/sunset/registry.py
--rw-r--r--   0        0        0     6558 2023-03-22 23:47:32.257564 SunsetSettings-0.4.0/sunset/serializable_enum.py
--rw-r--r--   0        0        0     2446 2022-12-19 01:41:49.063710 SunsetSettings-0.4.0/sunset/serializers.py
--rw-r--r--   0        0        0    18206 2023-03-17 19:19:31.127671 SunsetSettings-0.4.0/sunset/settings.py
--rw-r--r--   0        0        0     1161 2022-12-21 23:15:34.123599 SunsetSettings-0.4.0/sunset/timer.py
--rw-r--r--   0        0        0        0 2022-03-15 15:31:18.747300 SunsetSettings-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0     6015 2022-12-28 17:41:47.581714 SunsetSettings-0.4.0/tests/test_autosaver.py
--rw-r--r--   0        0        0     9591 2023-03-17 15:09:28.881387 SunsetSettings-0.4.0/tests/test_bunch.py
--rw-r--r--   0        0        0     4709 2023-03-17 18:56:27.854625 SunsetSettings-0.4.0/tests/test_concurrency.py
--rw-r--r--   0        0        0     3404 2022-12-14 00:56:18.711048 SunsetSettings-0.4.0/tests/test_exporter.py
--rw-r--r--   0        0        0    14475 2023-03-22 22:25:25.358118 SunsetSettings-0.4.0/tests/test_key.py
--rw-r--r--   0        0        0    18187 2023-03-17 15:09:29.065394 SunsetSettings-0.4.0/tests/test_list.py
--rw-r--r--   0        0        0     1469 2022-10-01 12:15:33.604100 SunsetSettings-0.4.0/tests/test_non_hashable_set.py
--rw-r--r--   0        0        0     3876 2022-10-01 12:15:58.356993 SunsetSettings-0.4.0/tests/test_registry.py
--rw-r--r--   0        0        0     1836 2023-03-22 23:05:04.339400 SunsetSettings-0.4.0/tests/test_serializable_enum.py
--rw-r--r--   0        0        0     2046 2022-10-05 13:12:55.346092 SunsetSettings-0.4.0/tests/test_serializers.py
--rw-r--r--   0        0        0    22705 2023-03-17 18:16:28.583712 SunsetSettings-0.4.0/tests/test_settings.py
--rw-r--r--   0        0        0     1373 2022-12-21 23:39:20.575092 SunsetSettings-0.4.0/tests/test_timer.py
--rw-r--r--   0        0        0      251 2022-12-19 01:40:30.636872 SunsetSettings-0.4.0/tox.ini
--rw-r--r--   0        0        0     7092 1970-01-01 00:00:00.000000 SunsetSettings-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1698 2023-01-16 00:48:03.487746 SunsetSettings-0.5.0/.github/workflows/python-build.yml
+-rw-r--r--   0        0        0       59 2022-08-04 10:12:23.781547 SunsetSettings-0.5.0/.gitignore
+-rw-r--r--   0        0        0      233 2022-12-14 00:54:21.154949 SunsetSettings-0.5.0/.readthedocs.yml
+-rw-r--r--   0        0        0    32422 2022-03-24 23:57:25.474661 SunsetSettings-0.5.0/LICENSE
+-rw-r--r--   0        0        0     6132 2023-04-22 18:12:13.008561 SunsetSettings-0.5.0/README.md
+-rw-r--r--   0        0        0      638 2022-08-04 10:11:43.364138 SunsetSettings-0.5.0/docs/Makefile
+-rw-r--r--   0        0        0      804 2022-08-04 10:11:43.364138 SunsetSettings-0.5.0/docs/make.bat
+-rw-r--r--   0        0        0     1168 2023-04-22 17:44:14.428052 SunsetSettings-0.5.0/docs/source/api.rst
+-rw-r--r--   0        0        0     2176 2023-04-22 19:37:56.782226 SunsetSettings-0.5.0/docs/source/changelog.rst
+-rw-r--r--   0        0        0     2476 2022-12-19 01:40:30.636872 SunsetSettings-0.5.0/docs/source/conf.py
+-rw-r--r--   0        0        0      788 2023-01-16 22:21:36.070670 SunsetSettings-0.5.0/docs/source/index.rst
+-rw-r--r--   0        0        0      613 2022-11-20 03:11:09.133654 SunsetSettings-0.5.0/docs/source/installation.rst
+-rw-r--r--   0        0        0    16965 2023-04-22 18:11:35.827153 SunsetSettings-0.5.0/docs/source/usage.rst
+-rw-r--r--   0        0        0     1314 2022-12-19 15:06:00.615479 SunsetSettings-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1043 2023-04-22 19:17:46.521114 SunsetSettings-0.5.0/sunset/__init__.py
+-rw-r--r--   0        0        0     8180 2023-04-22 11:08:18.204704 SunsetSettings-0.5.0/sunset/autosaver.py
+-rw-r--r--   0        0        0    10354 2023-04-22 18:12:30.373219 SunsetSettings-0.5.0/sunset/bunch.py
+-rw-r--r--   0        0        0     4799 2023-04-22 16:01:00.879583 SunsetSettings-0.5.0/sunset/enum_serializer.py
+-rw-r--r--   0        0        0     4186 2023-04-22 10:51:57.496111 SunsetSettings-0.5.0/sunset/exporter.py
+-rw-r--r--   0        0        0    15412 2023-04-22 19:10:03.411616 SunsetSettings-0.5.0/sunset/key.py
+-rw-r--r--   0        0        0    14951 2023-04-22 18:13:28.415418 SunsetSettings-0.5.0/sunset/list.py
+-rw-r--r--   0        0        0      993 2023-04-22 10:45:58.950590 SunsetSettings-0.5.0/sunset/lockable.py
+-rw-r--r--   0        0        0     1961 2023-04-22 00:48:12.340576 SunsetSettings-0.5.0/sunset/non_hashable_set.py
+-rw-r--r--   0        0        0     5620 2023-04-22 17:56:56.225696 SunsetSettings-0.5.0/sunset/protocols.py
+-rw-r--r--   0        0        0        0 2022-04-05 17:36:11.873451 SunsetSettings-0.5.0/sunset/py.typed
+-rw-r--r--   0        0        0     2366 2023-04-22 10:18:32.648125 SunsetSettings-0.5.0/sunset/registry.py
+-rw-r--r--   0        0        0     2149 2023-04-22 15:22:51.676899 SunsetSettings-0.5.0/sunset/serializers.py
+-rw-r--r--   0        0        0    18809 2023-04-22 18:14:03.188735 SunsetSettings-0.5.0/sunset/settings.py
+-rw-r--r--   0        0        0     1155 2023-04-22 00:45:06.565561 SunsetSettings-0.5.0/sunset/timer.py
+-rw-r--r--   0        0        0        0 2022-03-15 15:31:18.747300 SunsetSettings-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     6001 2023-04-22 00:45:13.261814 SunsetSettings-0.5.0/tests/test_autosaver.py
+-rw-r--r--   0        0        0     9958 2023-04-22 00:45:17.709982 SunsetSettings-0.5.0/tests/test_bunch.py
+-rw-r--r--   0        0        0     4709 2023-04-22 00:45:18.942028 SunsetSettings-0.5.0/tests/test_concurrency.py
+-rw-r--r--   0        0        0     2763 2023-04-22 15:48:31.311277 SunsetSettings-0.5.0/tests/test_enum_serializer.py
+-rw-r--r--   0        0        0     3453 2023-04-22 00:45:19.878064 SunsetSettings-0.5.0/tests/test_exporter.py
+-rw-r--r--   0        0        0    18091 2023-04-22 19:15:30.535976 SunsetSettings-0.5.0/tests/test_key.py
+-rw-r--r--   0        0        0    18679 2023-04-22 18:42:49.545885 SunsetSettings-0.5.0/tests/test_list.py
+-rw-r--r--   0        0        0     1498 2023-04-22 00:45:22.574165 SunsetSettings-0.5.0/tests/test_non_hashable_set.py
+-rw-r--r--   0        0        0     3949 2023-04-22 00:45:23.574203 SunsetSettings-0.5.0/tests/test_registry.py
+-rw-r--r--   0        0        0     2766 2023-04-22 00:45:26.182301 SunsetSettings-0.5.0/tests/test_serializers.py
+-rw-r--r--   0        0        0    23284 2023-04-22 18:10:01.511578 SunsetSettings-0.5.0/tests/test_settings.py
+-rw-r--r--   0        0        0     1387 2023-04-22 00:45:30.914480 SunsetSettings-0.5.0/tests/test_timer.py
+-rw-r--r--   0        0        0      251 2022-12-19 01:40:30.636872 SunsetSettings-0.5.0/tox.ini
+-rw-r--r--   0        0        0     7215 1970-01-01 00:00:00.000000 SunsetSettings-0.5.0/PKG-INFO
```

### Comparing `SunsetSettings-0.4.0/.github/workflows/python-build.yml` & `SunsetSettings-0.5.0/.github/workflows/python-build.yml`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.4.0/LICENSE` & `SunsetSettings-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.4.0/README.md` & `SunsetSettings-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -116,57 +116,61 @@
 >>> from sunset import Key
 
 >>> # Types can be inferred from the provided default value:
 >>> number_of_ponies = Key(default=0)
 >>> number_of_ponies
 <Key[int]:(0)>
 >>> number_of_ponies.set(6)  # Works!
+True
 >>> number_of_ponies.set("six")  # Type error!
+False
 >>> number_of_ponies.get()  # Value is unchanged.
 6
 >>> from typing import TYPE_CHECKING
 >>> if TYPE_CHECKING:
 ...     reveal_type(number_of_ponies.get())
 >>> # Revealed type is "builtins.int"
 
 ```
 
 
 ### Extensibility
 
-You can store arbitrary types in your SunsetSettings provided they implement a
-simple serialization protocol. (See [the API
-reference](https://sunsetsettings.rtfd.io/en/stable/api.html#sunset.Serializable).)
+You can store arbitrary types in your SunsetSettings provided that you also
+provide a serializer for that type. (See [the API
+reference](https://sunsetsettings.rtfd.io/en/stable/api.html#sunset.Serializer).)
 
 ```python
 >>> import re
 >>> from typing import Optional, TYPE_CHECKING
 
 >>> class Coordinates:
 ...     def __init__(self, x: int, y: int) -> None:
-...         self._x = x
-...         self._y = y
-...
-...     def toStr(self) -> str:
-...         return f"{self._x},{self._y}"
+...         self.x = x
+...         self.y = y
+
+>>> class CoordinatesSerializer:
+...     def toStr(self, coord: Coordinates) -> str:
+...         return f"{coord.x},{coord.y}"
 ...
-...     @classmethod
-...     def fromStr(cls, value: str) -> Optional["Coordinates"]:
-...         m = re.match(r"(\d+),(\d+)", value)
-...         if m is None:
+...     def fromStr(self, string: str) -> Optional[Coordinates]:
+...         x, y = string.split(",", 1)
+...         if not x.isdigit() or not y.isdigit():
 ...             return None
-...         x = int(m.group(1))
-...         y = int(m.group(2))
-...         return cls(x, y)
+...         return Coordinates(int(x), int(y))
 
 >>> from sunset import Key
->>> coordinates = Key(default=Coordinates(0, 0))
+>>> coordinates = Key(
+...     default=Coordinates(0, 0), serializer=CoordinatesSerializer()
+... )
 >>> if TYPE_CHECKING:
 ...     reveal_type(coordinates.get())
 >>> # Revealed type is "Coordinates"
+>>> print(repr(coordinates))
+<Key[Coordinates]:(0,0)>
 
 ```
 
 
 ### Inheritance
 
 SunsetSettings lets the user have a general set of settings that can be
@@ -181,14 +185,15 @@
 ...     limbs: Key[int] = Key(default=4)
 ... 
 >>> animals = Animals()
 >>> octopuses = animals.newSection(name="octopuses")
 >>> octopuses.limbs.get()
 4
 >>> octopuses.limbs.set(8)
+True
 >>> octopuses.limbs.get()
 8
 >>> animals.limbs.get()
 4
 >>> octopuses.limbs.clear()
 >>> octopuses.limbs.get()
 4
@@ -205,14 +210,15 @@
 
 >>> number_of_ponies = Key(default=0)
 >>> def callback(value):
 ...     print("Pony count updated:", value)
 >>> number_of_ponies.onValueChangeCall(callback)
 >>> number_of_ponies.set(6)
 Pony count updated: 6
+True
 
 ```
 
 
 ## Requirements
 
 - Python 3.9 or later.
```

### Comparing `SunsetSettings-0.4.0/docs/Makefile` & `SunsetSettings-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.4.0/docs/make.bat` & `SunsetSettings-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.4.0/docs/source/api.rst` & `SunsetSettings-0.5.0/docs/source/api.rst`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 
     .. automethod:: isSet
 
     .. automethod:: updateValue
 
     .. automethod:: clear
 
+    .. automethod:: setValidator
+
     .. automethod:: onValueChangeCall
 
     .. automethod:: onUpdateCall
 
 .. autoclass:: sunset.Bunch
 
     .. automethod:: onUpdateCall
@@ -57,16 +59,18 @@
 
     .. automethod:: doLoad
 
     .. automethod:: doSave
 
     .. automethod:: saveIfNeeded
 
-.. autoclass:: sunset.Serializable
+.. autoclass:: sunset.Serializer
 
     .. automethod:: toStr
 
     .. automethod:: fromStr
 
-.. autoclass:: sunset.SerializableEnum
+.. autoclass:: sunset.Serializable
+
+    .. automethod:: toStr
 
-.. autoclass:: sunset.SerializableFlag
+    .. automethod:: fromStr
```

### Comparing `SunsetSettings-0.4.0/docs/source/changelog.rst` & `SunsetSettings-0.5.0/docs/source/changelog.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 Changelog
 =========
 
-Latest
-------
+SunsetSettings 0.5.0 (2023-04-22)
+---------------------------------
+
+  - Added ability to set a validator on Keys to limit their possible values.
+  - Making a typo in a value when editing a settings file manually no longer causes the entry to be deleted on save.
+  - Added ability to serialize Enum subclasses natively.
+  - Deprecated now unnecessary SerializableEnum and -Flag classes.
+  - Added ability to pass a custom serializer when instantiating a Key.
+  - Added ability to store any type in a Key.
+  - onUpdateCall() and onValueChangeCall() now accept callbacks with any return value.
 
 SunsetSettings 0.4.0 (2023-03-22)
 ---------------------------------
 
   - Renamed Bundle to Bunch. Just makes more sense for something that holds Keys.
   - Added serializable Enum and Flag subclasses.
   - AutoSaver now expands '~' to the current user's home directory.
```

### Comparing `SunsetSettings-0.4.0/docs/source/conf.py` & `SunsetSettings-0.5.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.4.0/docs/source/index.rst` & `SunsetSettings-0.5.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.4.0/docs/source/installation.rst` & `SunsetSettings-0.5.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.4.0/docs/source/usage.rst` & `SunsetSettings-0.5.0/docs/source/usage.rst`

 * *Files 8% similar despite different names*

```diff
@@ -54,29 +54,18 @@
     ...     port: Key[int]   = Key(default=80)
     ...     ssl: Key[bool]   = Key(default=False)
 
 The benefit of using explicit type annotations is that they serve as a
 declaration of intention for what the Keys will hold, and will cause a type
 error if a given default does not match the intended type of its Key.
 
-By default, a Key can contain a `str`, an `int`, a `float`, or a `bool`. But
-Keys can also contain any type that implements the
-:class:`~sunset.Serializable` protocol. See
-:ref:`storing-custom-types`.
-
-As a convenience, SunsetSettings provides the :class:`~sunset.SerializableEnum`
-and :class:`~sunset.SerializableFlag` classes, which are subclasses of
-respectively `enum.Enum` and `enum.Flag` that implement the
-:class:`~sunset.Serializable` protocol. 
-
-.. note::
-
-    Key values are limited to `str`, `int`, `float` and `bool` and types that
-    implement the `Serializable` protocol, because SunsetSettings needs to know
-    how to safely and reliably load them from and save them to text.
+By default, a Key can contain a `str`, an `int`, a `float`, a `bool`, or an
+`enum.Enum` subclass. But Keys can also contain any arbitrary type, so long as
+they are instantiated with a :class:`~sunset.Serializer` argument for that type.
+See :ref:`storing-custom-types`.
 
 Related keys can be grouped together with the :class:`~sunset.Bunch` class.
 
 
 Bunches
 ~~~~~~~
 
@@ -87,33 +76,33 @@
 
 For example:
 
 .. code-block:: python
 
     >>> from sunset import Bunch, Key, Settings
 
-    >>> class UI(Bunch):
+    >>> class Font(Bunch):
     ...     font_name: Key[str] = Key(default="Arial")
     ...     font_size: Key[int] = Key(default=14)
 
     >>> class Network(Bunch):
     ...     server: Key[str] = Key(default="127.0.0.1")
     ...     port: Key[int]   = Key(default=80)
     ...     ssl: Key[bool]   = Key(default=False)
 
     >>> class MySettings(Settings):
-    ...     ui      = UI()
+    ...     font    = Font()
     ...     network = Network()
 
 Here too, type annotations are optional, but can be used, and are a good idea:
 
 .. code-block:: python
 
     >>> class MySettings(Settings):
-    ...     ui:      UI      = UI()
+    ...     font: Font       = Font()
     ...     network: Network = Network()
 
 .. warning::
 
     Note that the Bunch fields *have* to be instantiated in the Settings class
     definition, else you will encounter strange bugs that will confuse you. If
     you encounter problems where modifying the value of a Key in a Bunch also
@@ -207,50 +196,99 @@
 
 
 .. _storing-custom-types:
 
 Storing custom types in Keys
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-You can also store in a Key any type that implements the
-:class:`~sunset.Serializable` protocol. This protocol requires the
-implementation of only two methods: :meth:`~sunset.Serializable.fromStr()` and
-:meth:`~sunset.Serializable.toStr()`. Note that
-:meth:`~sunset.Serializable.fromStr()` is a class method. SunsetSettings uses
-these methods to save your type to a file and load it again reliably and safely.
+You can store any arbitrary type in a Key. There are two ways to do so.
+
+The first way is to provide a serializer when instantiating the Key. A
+serializer is an object that implements the :class:`~sunset.Serializer` protocol
+for the type you want to store in a Key.
+
+For example:
+
+.. code-block:: python
+
+    >>> from typing import Optional
+    >>> from sunset import Key, Settings
+
+    >>> class Coordinates:
+    ...     def __init__(self, x: int, y: int) -> None:
+    ...         self.x = x
+    ...         self.y = y
+
+    >>> class CoordinatesSerializer:
+    ...     def toStr(self, coord: Coordinates) -> str:
+    ...         return f"{coord.x},{coord.x}"
+    ...
+    ...     def fromStr(self, string: str) -> Optional[Coordinates]:
+    ...         x, y = string.split(",", 1)
+    ...         if not x.isdigit() or not y.isdigit():
+    ...             return None
+    ...         return Coordinates(int(x), int(y))
+
+    >>> class MySettings(Settings):
+    ...     origin: Key[Coordinates] = Key(
+    ...         Coordinates(0, 0), serializer=CoordinatesSerializer()
+    ...     )
+
+    >>> settings = MySettings()
+    >>> print(repr(settings.origin))
+    <Key[Coordinates]:(0,0)>
+
+
+The second way is to have the type you want to store in a Key implement the
+:class:`~sunset.Serializable` protocol. Note that the methods of this protocol
+are pretty similar to that of :class:`~sunset.Serializer`. The difference is
+that in the case of :class:`~sunset.Serializable`, the methods are implemented
+directly on the type that will be stored in the Key.
 
 For example:
 
 .. code-block:: python
 
     >>> import re
     >>> from typing import Optional
 
     >>> from sunset import Key, Settings
 
     >>> class Coordinates:
     ...     def __init__(self, x: int, y: int) -> None:
-    ...         self._x = x
-    ...         self._y = y
+    ...         self.x = x
+    ...         self.y = y
     ...
     ...     def toStr(self) -> str:
-    ...         return f"{self._x},{self._y}"
+    ...         return f"{self.x},{self.y}"
     ...
     ...     @classmethod
-    ...     def fromStr(cls, value: str) -> Optional["Coordinates"]:
-    ...         m = re.match(r"(\d+),(\d+)", value)
-    ...         if m is None:
+    ...     def fromStr(cls, string: str) -> Optional["Coordinates"]:
+    ...         x, y = string.split(",", 1)
+    ...         if not x.isdigit() or not y.isdigit():
     ...             return None
-    ...         x = int(m.group(1))
-    ...         y = int(m.group(2))
-    ...         return cls(x, y)
+    ...         return cls(int(x), int(y))
 
     >>> class MySettings(Settings):
     ...     origin: Key[Coordinates] = Key(Coordinates(0, 0))
 
+    >>> settings = MySettings()
+    >>> print(repr(settings.origin))
+    <Key[Coordinates]:(0,0)>
+
+
+Note also that in the latter case, :meth:`~sunset.Serializable.fromStr()` must
+be a class method.
+
+Both approaches to providing serialization and deserialization methods for your
+custom types are valid. :class:`~sunset.Serializer` requires a more verbose
+instantiation for your Keys, but allows for the concern of serialization to be
+kept separate from your custom type. If you don't care either way, use
+:class:`~sunset.Serializer`.
+
 
 Using settings
 --------------
 
 Overview
 ~~~~~~~~
 
@@ -333,26 +371,33 @@
     >>> class BackupSettings(Settings):
     ...     path: Key[str]         = Key(default="/")
     ...     destination: Key[str]  = Key(default="/")
     ...     compression: Key[bool] = Key(default=False)
 
     >>> settings = BackupSettings()
     >>> settings.compression.set(True)
+    True
 
     >>> user1section = settings.newSection("User 1")
     >>> user1section.path.set("/home/user1/")
+    True
     >>> user1section.destination.set("/var/backups/user1/")
+    True
 
     >>> user1videossection = user1section.newSection("Videos")
     >>> user1videossection.path.set("/home/user1/Videos/")
+    True
     >>> user1videossection.compression.set(False)
+    True
 
     >>> mailssection = settings.newSection("Mails")
     >>> mailssection.path.set("/var/mail/")
+    True
     >>> mailssection.destination.set("/var/backups/mails/")
+    True
 
 Here is what these Settings would look like when saved to a file:
 
 .. code-block:: python
 
     >>> import io
     >>> text = io.StringIO()
@@ -409,20 +454,25 @@
     ...         Key(default="*"), order=List.PARENT_FIRST
     ...     )
 
     >>> settings = BackupSettings()    
 
     >>> user1section = settings.newSection("User 1")
     >>> user1section.path.set("/home/user1/")
+    True
     >>> user1section.ignore_patterns.appendOne().set("*.tmp")
+    True
 
     >>> user1codesection = user1section.newSection("Code")
     >>> user1codesection.path.set("/home/user1/Code/Python/")
+    True
     >>> user1codesection.ignore_patterns.appendOne().set("*.py")
+    True
     >>> user1codesection.ignore_patterns.appendOne().set("__pycache__")
+    True
 
     >>> print([
     ...     pattern.get() for pattern in user1codesection.ignore_patterns.iter()
     ... ])
     ['*.tmp', '*.py', '__pycache__']
```

### Comparing `SunsetSettings-0.4.0/pyproject.toml` & `SunsetSettings-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.4.0/sunset/__init__.py` & `SunsetSettings-0.5.0/sunset/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 "SunsetSettings: a type-safe, extensible settings system with inheritance."
 
 __project__ = "SunsetSettings"
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 __author__ = "P. Varet"
 __copyright__ = "2022-2023, P. Varet"
 
 from . import exporter, non_hashable_set, serializers
 
 from .autosaver import AutoSaver
 from .bunch import Bunch
 from .key import Key
 from .list import List
-from .protocols import Serializable
+from .protocols import Serializable, Serializer
 from .registry import CallbackRegistry
-from .serializable_enum import (
+from .enum_serializer import (
     SerializableEnum,
     SerializableFlag,
 )
 from .settings import Settings, normalize
 from .timer import PersistentTimer
 
 # Backward compatibility: Bunch used to be called Bundle. Retain compatibility
@@ -31,13 +31,14 @@
     "CallbackRegistry",
     "Key",
     "List",
     "PersistentTimer",
     "Serializable",
     "SerializableEnum",
     "SerializableFlag",
+    "Serializer",
     "Settings",
     "exporter",
     "non_hashable_set",
     "normalize",
     "serializers",
 ]
```

### Comparing `SunsetSettings-0.4.0/sunset/autosaver.py` & `SunsetSettings-0.5.0/sunset/autosaver.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,37 @@
 import logging
 import os
 import pathlib
 import tempfile
 
 from types import TracebackType
 
-from typing import Any, Optional, TypeVar, Union
+from typing import Any, Callable, IO, Optional, Protocol, TypeVar, Union
 
-from .settings import Settings
 from .timer import PersistentTimer, TimerProtocol
 
 _TimerT = TypeVar("_TimerT", bound=TimerProtocol)
 
 
+class _SavableProtocol(Protocol):
+    """
+    This protocol lets AutoSaver know how to use a Settings instance without
+    having to import the actual Settings class.
+    """
+
+    def load(self, file: IO[str]) -> None:
+        ...
+
+    def save(self, file: IO[str], blanklines: bool = False) -> None:
+        ...
+
+    def onUpdateCall(self, callback: Callable[[Any], Any]) -> None:
+        ...
+
+
 class AutoSaver:
     """
     AutoSaver is a helper class that can take care of loading and saving
     settings automatically and safely.
 
     On instantiation, it automatically loads settings from the given file path,
     if that file exists, unless the `load_on_init` argument is set to False.
@@ -73,25 +88,25 @@
     """
 
     _DIR_MODE: int = 0o755
     _FILE_MODE: int = 0o644
     _ENCODING: str = "UTF-8"
 
     _path: pathlib.Path
-    _settings: Settings
+    _settings: _SavableProtocol
     _dirty: bool
     _save_on_update: bool
     _save_on_delete: bool
     _save_delay: float
     _save_timer: TimerProtocol
     _logger: logging.Logger
 
     def __init__(
         self,
-        settings: Settings,
+        settings: _SavableProtocol,
         path: Union[pathlib.Path, str],
         *,
         save_on_update: bool = True,
         save_on_delete: bool = True,
         load_on_init: bool = True,
         save_delay: float = 0.0,
         logger: Optional[logging.Logger] = None,
@@ -173,20 +188,20 @@
         Returns:
             True if saving succeeded, else False. If False, the error will be
             logged using the logger passed during initialization.
         """
 
         self._save_timer.cancel()
 
-        dir = self._path.parent
-        dir.mkdir(parents=True, mode=self._DIR_MODE, exist_ok=True)
+        directory = self._path.parent
+        directory.mkdir(parents=True, mode=self._DIR_MODE, exist_ok=True)
 
         try:
             with tempfile.NamedTemporaryFile(
-                dir=dir,
+                dir=directory,
                 prefix=self._path.name,
                 mode="xt",
                 encoding=self._ENCODING,
                 delete=False,
             ) as tmp:
                 self._settings.save(tmp.file, blanklines=True)
                 os.chmod(tmp.name, self._FILE_MODE)
```

### Comparing `SunsetSettings-0.4.0/sunset/bunch.py` & `SunsetSettings-0.5.0/sunset/bunch.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,17 @@
     ...     secondary_font: Font = Font()
     >>> appearance = Appearance()
     >>> appearance.main_font.name.get()
     'Arial'
     >>> appearance.secondary_font.name.get()
     'Arial'
     >>> appearance.main_font.name.set("Times New Roman")
+    True
     >>> appearance.secondary_font.name.set("Calibri")
+    True
     >>> appearance.main_font.name.get()
     'Times New Roman'
     >>> appearance.secondary_font.name.get()
     'Calibri'
     """
 
     _parent: Optional[weakref.ref["Bunch"]]
@@ -182,20 +184,22 @@
 
         if parent is not None:
             if type(self) is not type(parent):
                 return
 
         old_parent = self.parent()
         if old_parent is not None:
+            # pylint: disable=protected-access
             old_parent._children.discard(self)
 
         if parent is None:
             self._parent = None
         else:
             self._parent = weakref.ref(parent)
+            # pylint: disable=protected-access
             parent._children.add(self)
 
         for label, field in self._fields.items():
             if parent is None:
                 field.setParent(None)
                 continue
 
@@ -235,26 +239,26 @@
 
         # Note that we iterate on a copy so that this will not break if a
         # different thread updates the contents during the iteration.
 
         for child in list(self._children):
             yield cast(Self, child)
 
-    def onUpdateCall(self, callback: Callable[[Any], None]) -> None:
+    def onUpdateCall(self, callback: Callable[[Any], Any]) -> None:
         """
         Adds a callback to be called whenever this Bunch is updated. A Bunch
         is considered updated when any of its fields is updated.
 
         The callback will be called with as its argument whichever field was
         just updated.
 
         Args:
             callback: A callable that will be called with one argument of type
                 :class:`~sunset.List`, :class:`~sunset.Bunch` or
-                :class:`~sunset.Key`, and returns None.
+                :class:`~sunset.Key`.
 
         Returns:
             None.
 
         Note:
             This method does not increase the reference count of the given
             callback.
@@ -277,29 +281,31 @@
         Internal.
         """
 
         if not self.isPrivate():
             for _, field in sorted(self._fields.items()):
                 yield from field.dumpFields()
 
-    def restoreField(self, path: str, value: Optional[str]) -> None:
+    def restoreField(self, path: str, value: Optional[str]) -> bool:
         """
         Internal.
         """
 
         if self._PATH_SEPARATOR not in path:
-            return
+            return False
 
         field_label, path = path.split(self._PATH_SEPARATOR, 1)
         if self.fieldLabel() != field_label:
-            return
+            return False
 
         field_label, *_ = path.split(self._PATH_SEPARATOR, 1)
         if (field := self._fields.get(field_label)) is not None:
-            field.restoreField(path, value)
+            return field.restoreField(path, value)
+
+        return False
 
     def triggerUpdateNotification(
         self, field: Optional[UpdateNotifier]
     ) -> None:
         """
         Internal.
         """
```

### Comparing `SunsetSettings-0.4.0/sunset/exporter.py` & `SunsetSettings-0.5.0/sunset/exporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 from typing import Iterable, Optional, IO
 
 
 _SECTION_SEPARATOR = "/"
 _PATH_SEPARATOR = "."
 
 
-def normalize(input: str, to_lower: bool = True) -> str:
-
+def normalize(string: str, to_lower: bool = True) -> str:
     ret = ""
-    for c in input:
+    for c in string:
         if c.isalnum() or c in ("-", "_"):
             ret += c
     return ret.lower() if to_lower else ret
 
 
 def maybe_escape(value: str) -> str:
-
     if (
+        # pylint: disable-next=too-many-boolean-expressions
         len(value) == 0
         or '"' in value
         or "\\" in value
         or "\n" in value
         or value[0].isspace()
         or value[-1].isspace()
     ):
-
         ret = ""
         for c in value:
             if c == '"':
                 ret += r"\""
             elif c == "\n":
                 ret += r"\n"
             elif c == "\\":
@@ -37,16 +35,15 @@
                 ret += c
 
         return '"' + ret + '"'
 
     return value
 
 
-def unescape(value: str):
-
+def unescape(value: str) -> str:
     if '"' not in value and "\\" not in value:
         return value
 
     if len(value) < 2:
         return value
 
     if value[0] == '"':
@@ -55,34 +52,32 @@
     if value[-1] == '"':
         value = value[:-1]
 
     ret = ""
     escaped = False
 
     for c in value:
-
         if not escaped:
             if c == "\\":
                 escaped = True
                 continue
-            else:
-                ret += c
+
+            ret += c
 
         else:
             if c == "n":
                 ret += "\n"
             else:
                 ret += c
             escaped = False
 
     return ret
 
 
 def cleanup_string(string: str, /, sep: str, to_lower: bool) -> str:
-
     replacements = (
         (f" {sep}", f"{sep}"),
         (f"{sep} ", f"{sep}"),
         (f"{sep}{sep}", f"{sep}"),
     )
 
     for from_, to in replacements:
@@ -93,54 +88,48 @@
         normalize(fragment.strip(), to_lower) for fragment in string.split(sep)
     )
 
     return string.strip(sep)
 
 
 def cleanup_section(section: str) -> str:
-
     return cleanup_string(section, sep=_SECTION_SEPARATOR, to_lower=True)
 
 
 def cleanup_path(path: str) -> str:
-
     return cleanup_string(path, sep=_PATH_SEPARATOR, to_lower=False)
 
 
 # TODO: turn into a function (like dump_to_ini maybe) that takes the data and
 # yields lines of text, and then use file.writelines.
 def save_to_file(
     file: IO[str],
     data: Iterable[tuple[str, Optional[str]]],
     *,
     blanklines: bool,
 ):
-
     need_space = False
     current_section = ""
 
     def extract_section(path: str) -> tuple[str, str]:
-
         if _SECTION_SEPARATOR not in path:
             return "", ""
 
         section, path = path.rsplit(_SECTION_SEPARATOR, 1)
         if _SECTION_SEPARATOR in section:
             _, section = section.split(_SECTION_SEPARATOR, 1)
 
         return section, path
 
     for path, dump in data:
-
         section, path = extract_section(path.strip())
         if not section:
             continue
 
         if section != current_section:
-
             current_section = section
 
             if need_space and blanklines:
                 file.write("\n")
             need_space = True
 
             file.write(f"[{current_section}]\n")
@@ -151,37 +140,34 @@
                 file.write(f" {maybe_escape(dump)}")
             file.write("\n")
 
 
 def load_from_file(
     file: IO[str], main: str
 ) -> Iterable[tuple[str, Optional[str]]]:
-
     main = normalize(main)
 
     current_section = ""
 
     for line in file:
         line = line.strip()
 
         if not line:
             continue
 
         if line[0] == "[" and line[-1] == "]":
-
             current_section = cleanup_section(line[1:-1])
             if not current_section:
                 continue
 
             if current_section != main:
                 current_section = main + _SECTION_SEPARATOR + current_section
 
             yield current_section + _SECTION_SEPARATOR, ""
 
         elif "=" in line:
-
             path, dump = line.split("=", 1)
             path = cleanup_path(path)
             dump = dump.strip()
             if path and current_section:
                 payload = unescape(dump) if dump else None
                 yield (current_section + _SECTION_SEPARATOR + path, payload)
```

### Comparing `SunsetSettings-0.4.0/sunset/key.py` & `SunsetSettings-0.5.0/sunset/key.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,112 +1,151 @@
+import logging
 import weakref
 
 from typing import (
     Any,
     Callable,
     Generic,
     Iterable,
     Iterator,
     Optional,
-    Type,
     TypeVar,
     cast,
 )
 
 from .exporter import maybe_escape
 from .lockable import Lockable
-from .protocols import ContainableImpl
+from .protocols import ContainableImpl, Serializer
 from .registry import CallbackRegistry
-from .serializers import AnySerializableType, deserialize, serialize
+from .serializers import lookup
 
 
 # TODO: Replace with typing.Self when mypy finally supports that.
 Self = TypeVar("Self", bound="Key[Any]")
+_T = TypeVar("_T")
 
 
-class Key(Generic[AnySerializableType], ContainableImpl, Lockable):
+class Key(Generic[_T], ContainableImpl, Lockable):
     """
     A single setting key containing a typed value.
 
     Keys support inheritance. If a Key does not have a value explicitly set, and
     it has a parent, then its value will be that of its parent. Else its value
     if unset is the default value it was instantiated with.
 
-    Keys can call a callback when their value changes, regardless of if its
+    Keys can call a callback when their reported value changes, whether it's
     their own value that changed, or that inherited from a parent. Set this
     callback with the :meth:`onValueChangeCall()` method.
 
+    You can control the values that can be set on this Key by passing a
+    `validator` argument when instantiating it.
+
     Args:
-        default: (str, int, bool, float, or any type that implements the
-            :class:`~sunset.Serializable` protocol) The value that this Key will
-            return when not otherwise set; the type of this default determines
-            the type of the values that can be set on this Key.
+        default: The value that this Key will return when not otherwise set; the
+            type of this default determines the type of the values that can be
+            set on this Key.
+
+            If the type of the default is not one of bool, int, float, str, or
+            an `enum.Enum` subclass, and is also not a class that implements the
+            :class:`~sunset.Serializable` protocol, then a serializer argument
+            must also be passed.
+
+        serializer: An implementation of the :class:`~sunset.Serializer`
+            protocol for the type of this Key's values. This argument must be
+            passed if the type in question is not supported by a native
+            SunsetSettings serializer. If a serializer is passed, it will be
+            used even if SunsetSettings has its own serializer for that type.
+
+        validator: A function that returns True if the given value can be set on
+            this Key, else False. This allows you to control what values are
+            allowable for this Key. Default: None.
 
     Example:
 
     >>> from sunset import Key
     >>> key: Key[int] = Key(default=0)
     >>> key.get()
     0
     >>> key.set(42)
+    True
     >>> key.get()
     42
     >>> child_key: Key[int] = Key(default=0)
     >>> child_key.setParent(key)
     >>> child_key.get()
     42
     >>> child_key.set(101)
+    True
     >>> child_key.get()
     101
     >>> key.set(36)
+    True
     >>> key.get()
     36
     >>> child_key.get()
     101
     >>> child_key.clear()
     >>> child_key.get()
     36
     """
 
-    _default: AnySerializableType
-    _value: Optional[AnySerializableType]
-    _value_change_callbacks: CallbackRegistry[AnySerializableType]
-    _update_notification_callbacks: CallbackRegistry["Key[AnySerializableType]"]
+    _default: _T
+    _value: Optional[_T]
+    _serializer: Serializer[_T]
+    _validator: Callable[[_T], bool]
+    _bad_value_string: Optional[str]
+    _value_change_callbacks: CallbackRegistry[_T]
+    _update_notification_callbacks: CallbackRegistry["Key[_T]"]
     _update_notification_enabled: bool
-    _parent: Optional[weakref.ref["Key[AnySerializableType]"]]
-    _children: weakref.WeakSet["Key[AnySerializableType]"]
-    _type: Type[AnySerializableType]
-
-    def __init__(self, default: AnySerializableType):
-
-        # serialize() raises an exception if the given value is not
-        # serializable, so this call guarantees that the provided default is of
-        # a type allowed in a Key. In case the user went ahead and ignored the
-        # typechecker error when instantiating their Key with a bad default.
+    _parent: Optional[weakref.ref["Key[_T]"]]
+    _children: weakref.WeakSet["Key[_T]"]
+    _type: type[_T]
+
+    def __init__(
+        self,
+        default: _T,
+        serializer: Optional[Serializer[_T]] = None,
+        validator: Optional[Callable[[_T], bool]] = None,
+    ) -> None:
+        super().__init__()
 
-        serialize(default)
+        # Keep a runtime reference to the practical type contained in this
+        # key.
 
-        super().__init__()
+        self._type = cast(type[_T], default.__class__)
 
         self._default = default
         self._value = None
+        self._bad_value_string = None
+
+        if serializer is None:
+            serializer = lookup(self._type)
+            if serializer is None:
+                raise TypeError(
+                    f"Default Key value '{default}' has type"
+                    f" '{self._type.__name__}', which is not"
+                    " supported by a native serializer. Please construct"
+                    " the Key with an explicit serializer argument."
+                )
+
+        if validator is not None:
+            self._validator = validator
+        else:
+            self._validator = lambda _: True
+
+        self._serializer = serializer
 
         self._value_change_callbacks = CallbackRegistry()
         self._update_notification_callbacks = CallbackRegistry()
         self._update_notification_enabled = True
 
         self._parent = None
         self._children = weakref.WeakSet()
 
-        # Keep a runtime reference to the practical type contained in this
-        # key.
-
-        self._type = cast(Type[AnySerializableType], default.__class__)
-
-    def get(self) -> AnySerializableType:
+    def get(self) -> _T:
         """
         Returns the current value of this Key.
 
         If this Key does not currently have a value set on it, return that of
         its parent if any. If it does not have a parent, return the default
         value for this Key.
 
@@ -118,70 +157,89 @@
             return value
 
         if (parent := self.parent()) is not None:
             return parent.get()
 
         return self._default
 
-    def set(self, value: AnySerializableType) -> None:
+    def set(self, value: _T) -> bool:
         """
         Sets the given value on this Key.
 
         Args:
             value: The value that this Key will now hold. Must be of the type
                 bound to this Key, i.e. the same type as this Key's default
                 value.
 
         Returns:
-            None.
+            True if the value was successfully set, else False, for instance if
+            the validator refused the value.
         """
 
         # Safety check in case the user is holding it wrong.
 
         if not isinstance(value, self._type):
-            return
+            return False
+
+        if not self._validator(value):
+            logging.debug(
+                "Validator rejected value for Key %s: %r",
+                self.fieldPath(),
+                value,
+            )
+            return False
+
+        # Setting a Key's value programmatically always resets bad values.
+
+        self._bad_value_string = None
 
         previously_set = self.isSet()
         prev_value = self.get()
 
         self._value = value
 
         if prev_value != self.get():
             self._value_change_callbacks.callAll(self.get())
             for child in self.children():
+                # pylint: disable=protected-access
                 child._notifyParentValueChanged()
 
         if not previously_set or prev_value != self.get():
             self.triggerUpdateNotification()
 
+        return True
+
     def clear(self) -> None:
         """
         Clears the value currently set on this Key, if any.
 
         Returns:
             None.
         """
 
+        # Clearing the Key always resets bad values.
+
+        self._bad_value_string = None
+
         if not self.isSet():
             return
 
         prev_value = self.get()
         self._value = None
 
         if prev_value != self.get():
             self._value_change_callbacks.callAll(self.get())
             for child in self.children():
+                # pylint: disable=protected-access
                 child._notifyParentValueChanged()
 
         self.triggerUpdateNotification()
 
     @Lockable.with_lock
-    def updateValue(
-        self, updater: Callable[[AnySerializableType], AnySerializableType]
-    ) -> None:
+    def updateValue(self, updater: Callable[[_T], _T]) -> None:
         """
         Atomically updates this Key's value using the given update function. The
         function will be called with the Key's current value, and the value it
         returns will be set as the Key's new value.
 
         Args:
             updater: A function that takes an argument of the same type held in
@@ -199,17 +257,15 @@
 
         Returns:
             True if a value is set on this Key, else False.
         """
 
         return self._value is not None
 
-    def onValueChangeCall(
-        self, callback: Callable[[AnySerializableType], None]
-    ) -> None:
+    def onValueChangeCall(self, callback: Callable[[_T], Any]) -> None:
         """
         Adds a callback to be called whenever the value returned by calling
         :meth:`get()` on this Key would change, even if this Key itself was not
         updated; for instance, this will happen if there is no value currently
         set on it and its parent's value changed.
 
         The callback will be called with the new value as its argument.
@@ -219,30 +275,28 @@
         instead. For example, if you call :meth:`set()` with a value of `0` on a
         Key newly created with a default value of `0`, callbacks added with
         :meth:`onUpdateCall()` are called and callbacks added with
         :meth:`onValueChangeCall()` are not.
 
 
         Args:
-            callback: A callable that takes one argument of the same type of the
-                values held by this Key, and that returns None.
+            callback: A callable that takes one argument of the same type as the
+                values held by this Key.
 
         Returns:
             None.
 
         Note:
             This method does not increase the reference count of the given
             callback.
         """
 
         self._value_change_callbacks.add(callback)
 
-    def onUpdateCall(
-        self, callback: Callable[["Key[AnySerializableType]"], None]
-    ) -> None:
+    def onUpdateCall(self, callback: Callable[["Key[_T]"], Any]) -> None:
         """
         Adds a callback to be called whenever this Key is updated, even if the
         value returned by :meth:`get()` does not end up changing.
 
         The callback will be called with this Key instance as its argument.
 
         If you want a callback to be called only when the apparent value of this
@@ -262,14 +316,29 @@
         Note:
             This method does not increase the reference count of the given
             callback.
         """
 
         self._update_notification_callbacks.add(callback)
 
+    def setValidator(self, validator: Callable[[_T], bool]) -> None:
+        """
+        Replaces this Key's validator.
+
+        Args:
+            validator: A function that returns True if the given value can be
+                set on this Key, else False. This allows you to control what
+                values are allowable for this Key.
+
+        Returns:
+            None.
+        """
+
+        self._validator = validator
+
     def setParent(self: Self, parent: Optional[Self]) -> None:
         """
         Makes the given Key the parent of this one. If None, remove this
         Key's parent, if any.
 
         A Key with a parent will inherit its parent's value when this
         Key's own value is not currently set.
@@ -292,24 +361,25 @@
 
         # Runtime check to affirm the type check of the method.
 
         if parent is not None:
             if type(self) is not type(parent):
                 return
 
+        # pylint: disable=protected-access
+
         old_parent = self.parent()
         if old_parent is not None:
             old_parent._children.discard(self)
 
         if parent is None:
             self._parent = None
             return
 
         if parent._type is not self._type:
-
             # This should not happen... unless the user is holding it wrong.
             # So, better safe than sorry.
 
             return
 
         parent._children.add(self)
         self._parent = weakref.ref(parent)
@@ -336,41 +406,66 @@
             An iterator over Keys of the same type as this one.
         """
 
         for child in self._children:
             yield cast(Self, child)
 
     def dumpFields(self) -> Iterable[tuple[str, Optional[str]]]:
+        if not self.isPrivate():
+            if self.isSet():
+                yield self.fieldPath(), self._serializer.toStr(self.get())
+
+            elif self._bad_value_string is not None:
+                # If a bad value was set in the settings file for this Key, and
+                # the Key was not modified since, then save the bad value again.
+                # This way, typos in the settings file don't outright destroy
+                # the entry.
 
-        if self.isSet() and not self.isPrivate():
-            yield self.fieldPath(), serialize(self.get())
-
-    def restoreField(self, path: str, value: Optional[str]) -> None:
+                yield self.fieldPath(), self._bad_value_string
 
+    def restoreField(self, path: str, value: Optional[str]) -> bool:
         if value is None:
-            return
+            # Note that doing nothing when the given value is None, is
+            # considered a success.
+
+            return True
+
+        success: bool = False
 
         self._update_notification_enabled = False
 
         if path == self.fieldLabel():
-            if (val := deserialize(self._type, value)) is not None:
-                self.set(val)
+            if (val := self._serializer.fromStr(value)) is not None:
+                success = self.set(val)
+
+            else:
+                # Keep track of the value that failed to restore, so that we can
+                # dump it again when saving. That way, if a user makes a typo
+                # while editing the settings file, the faulty entry is not
+                # entirely lost when we save.
+
+                logging.error(
+                    "Invalid value for Key %s: %s", self.fieldPath(), value
+                )
+                self._bad_value_string = value
 
         self._update_notification_enabled = True
 
-    def _notifyParentValueChanged(self):
+        return success
 
+    def _notifyParentValueChanged(self) -> None:
         if self.isSet():
             return
 
         self._value_change_callbacks.callAll(self.get())
         for child in self.children():
+            # pylint: disable=protected-access
             child._notifyParentValueChanged()
 
-    def triggerUpdateNotification(self):
+    def triggerUpdateNotification(self) -> None:
         """
         Internal.
         """
 
         if not self._update_notification_enabled:
             return
 
@@ -384,16 +479,17 @@
         Internal. Returns a new instance of this Key with the same default
         value.
 
         Returns:
             A new Key.
         """
 
-        return self.__class__(default=self._default)
+        return self.__class__(
+            default=self._default, serializer=self._serializer
+        )
 
     def __repr__(self) -> str:
-
         type_name = self._type.__name__
-        value = maybe_escape(serialize(self.get()))
+        value = maybe_escape(self._serializer.toStr(self.get()))
         if not self.isSet():
             value = f"({value})"
         return f"<Key[{type_name}]:{value}>"
```

### Comparing `SunsetSettings-0.4.0/sunset/list.py` & `SunsetSettings-0.5.0/sunset/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,15 @@
 
 from .bunch import Bunch
 from .key import Key
 from .non_hashable_set import WeakNonHashableSet
 from .protocols import Containable, ContainableImpl, UpdateNotifier
 from .registry import CallbackRegistry
 
-ListItemT = TypeVar(
-    "ListItemT",
-    # Note that we match on Key[Any] and not Key[SerializableT], because a
-    # TypeVar cannot be defined in terms of another TypeVar. This is fine,
-    # because Keys can only be created bound to a SerializableT type anyway.
-    bound=Union[Bunch, Key[Any]],
-)
+ListItemT = TypeVar("ListItemT", bound=Union[Bunch, Key[Any]])
 
 
 class IterOrder(Enum):
     NO_PARENT = auto()
     PARENT_FIRST = auto()
     PARENT_LAST = auto()
 
@@ -75,19 +69,21 @@
     ...         a: Key[str] = Key(default="")
     ...     key_list: List[Key[int]]         = List(Key(default=0))
     ...     bunch_list: List[ExampleBunch] = List(ExampleBunch())
     >>> settings = ExampleSettings()
     >>> settings.bunch_list
     []
     >>> settings.bunch_list.appendOne().a.set("demo")
+    True
     >>> settings.bunch_list
     [ExampleSettings.ExampleBunch(a=<Key[str]:demo>)]
     >>> settings.key_list
     []
     >>> settings.key_list.appendOne().set(12)
+    True
     >>> settings.key_list
     [<Key[int]:12>]
     """
 
     NO_PARENT = IterOrder.NO_PARENT
     PARENT_FIRST = IterOrder.PARENT_FIRST
     PARENT_LAST = IterOrder.PARENT_LAST
@@ -288,14 +284,16 @@
 
         # Runtime check to affirm the type check of the method.
 
         if parent is not None:
             if type(self) is not type(parent):
                 return
 
+        # pylint: disable=protected-access
+
         old_parent = self.parent()
         if old_parent is not None:
             old_parent._children.discard(self)
 
         if parent is None:
             self._parent = None
         else:
@@ -331,18 +329,22 @@
 
         Example:
 
         >>> from sunset import Key, List
         >>> show = lambda l: [key.get() for key in l]
         >>> parent = List(Key(default=0))
         >>> parent.appendOne().set(1)
+        True
         >>> parent.appendOne().set(2)
+        True
         >>> child = List(Key(default=0))
         >>> child.appendOne().set(3)
+        True
         >>> child.appendOne().set(4)
+        True
         >>> show(parent)
         [1, 2]
         >>> show(child)
         [3, 4]
         >>> child.setParent(parent)
         >>> show(child.iter())
         [3, 4]
@@ -387,29 +389,29 @@
         Returns:
             An iterator over List instances of the same type as this one.
         """
 
         for child in self._children:
             yield cast(Self, child)
 
-    def onUpdateCall(self, callback: Callable[[Any], None]) -> None:
+    def onUpdateCall(self, callback: Callable[[Any], Any]) -> None:
         """
         Adds a callback to be called whenever this List, *or* any item contained
         in this List, is updated.
 
         The callback will be called with whichever entity was updated as its
         argument: this List, or one of its items or sub-items.
 
         Adding new items to or deleting items from a List is considered an
         update of that List, not of the elements in question.
 
         Args:
             callback: A callable that will be called with one argument of type
                 :class:`~sunset.List`, :class:`~sunset.Bunch` or
-                :class:`~sunset.Key`, and returns None.
+                :class:`~sunset.Key`.
 
         Returns:
             None.
 
         Note:
             This method does not increase the reference count of the given
             callback.
@@ -425,37 +427,41 @@
         if not self.isPrivate():
             for item in self._contents:
                 if not item.isSet():
                     yield self.fieldPath() + item.fieldLabel(), None
                 else:
                     yield from item.dumpFields()
 
-    def restoreField(self, path: str, value: Optional[str]) -> None:
+    def restoreField(self, path: str, value: Optional[str]) -> bool:
         """
         Internal.
         """
 
         if self._PATH_SEPARATOR not in path:
-            return
+            return False
 
         field_label, path = path.split(self._PATH_SEPARATOR, 1)
         if self.fieldLabel() != field_label:
-            return
+            return False
+
+        success: bool = False
 
         _update_notification_enabled = self._update_notification_enabled
         self._update_notification_enabled = False
 
         field_label, *_ = path.split(self._PATH_SEPARATOR, 1)
         index = self._indexForLabel(field_label)
         if index is not None and index >= 0:
             self._ensureMinimumLength(index + 1)
-            self[index].restoreField(path, value)
+            success = self[index].restoreField(path, value)
 
         self._update_notification_enabled = _update_notification_enabled
 
+        return success
+
     def _ensureMinimumLength(self, length: int) -> None:
         missing_count = length - len(self)
 
         if missing_count > 0:
             self.extend((self._newItem() for _ in range(missing_count)))
 
     def triggerUpdateNotification(
```

### Comparing `SunsetSettings-0.4.0/sunset/lockable.py` & `SunsetSettings-0.5.0/sunset/lockable.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,24 +19,24 @@
     A helper mixin that provides a context manager to lock a class method's
     against one another.
     """
 
     _lock: threading.RLock
 
     def __init__(self) -> None:
-
         super().__init__()
 
         self._lock = threading.RLock()
 
     @staticmethod
     def with_lock(
         method: Callable[Concatenate[_Self, _P], _R]
     ) -> Callable[Concatenate[_Self, _P], _R]:
         @wraps(method)
         def locked_method(
             self: _Self, *args: _P.args, **kwargs: _P.kwargs
         ) -> _R:
+            # pylint: disable-next=protected-access
             with self._lock:
                 return method(self, *args, **kwargs)
 
         return locked_method
```

### Comparing `SunsetSettings-0.4.0/sunset/non_hashable_set.py` & `SunsetSettings-0.5.0/sunset/non_hashable_set.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,61 +13,53 @@
     """
 
     _contents: MutableMapping[int, _T]
 
     def __init__(
         self, mapping_type: Type[MutableMapping[int, _T]] = dict
     ) -> None:
-
         super().__init__()
 
         self._contents = mapping_type()
 
     def _computeHash(self, value: Any) -> int:
-
         # Try to return the normal hash for the value if possible. This is
         # because hash is more selective than id. For instance! If value is a
         # weakref, then hash properly identifies two distinct weakrefs to the
         # same object as equivalent, whereas id does not.
         # Sadly testing whether the value implements the Hashable proto does not
         # suffice. Dataclasses, for instance, implement the Hashable proto but
         # are not necessarily hashable.
 
         try:
             return hash(value)
         except TypeError:
             return id(value)
 
     def add(self, value: _T) -> None:
-
         self._contents[self._computeHash(value)] = value
 
     def discard(self, value: _T) -> None:
-
         try:
             del self._contents[self._computeHash(value)]
         except KeyError:
             pass
 
-    def __contains__(self, object: Any) -> bool:
-
-        return self._computeHash(object) in self._contents
+    def __contains__(self, obj: Any) -> bool:
+        return self._computeHash(obj) in self._contents
 
     def __iter__(self) -> Iterator[_T]:
-
         yield from self._contents.values()
 
     def __len__(self) -> int:
-
         return len(self._contents)
 
 
 class WeakNonHashableSet(NonHashableSet[_T]):
     """
     An implementation of a weak set that can contain non-hashable elements.
 
     Elements that are not hashable are distinguished by their id.
     """
 
     def __init__(self) -> None:
-
         super().__init__(mapping_type=weakref.WeakValueDictionary)
```

### Comparing `SunsetSettings-0.4.0/sunset/protocols.py` & `SunsetSettings-0.5.0/sunset/protocols.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 import weakref
 
 from typing import (
     Any,
     Callable,
+    Generic,
     Iterable,
     Iterator,
     Optional,
     Protocol,
-    Type,
     TypeVar,
     runtime_checkable,
 )
 
 
 Self = TypeVar("Self")
+_T = TypeVar("_T")
+
+
+# pylint: disable=unnecessary-ellipsis
+# The ellipses in the protocol definitions below are in fact necessary: they let
+# the type checker know it's fine we're not returning values.
 
 
 @runtime_checkable
 class Serializable(Protocol):
     """
     A protocol to be implemented by a class in order to enable storing instances
     of that class in a Key.
@@ -27,24 +33,53 @@
     """
 
     def toStr(self) -> str:
         """
         Returns a string representation of this instance that can be used by
         :meth:`fromStr()` to reconstruct a copy of this instance.
         """
-        ...  # noqa  # Else pylint complains of useless ellipsis.
+        ...
 
     @classmethod
-    def fromStr(cls: Type[Self], value: str) -> Optional[Self]:
+    def fromStr(cls: type[Self], string: str) -> Optional[Self]:
         """
         Takes a string that represents a serialized instance of this class, and
         returns a newly created instance that corresponds to that
         representation, or None if the string is not a valid serialized
         representation of an instance of this class.
         """
+        ...
+
+
+class Serializer(Generic[_T], Protocol):
+    """
+    A protocol that describes a way to serialize and deserialize an arbitrary
+    type.
+
+    SunsetSettings provides its own serializers for common types (int, float,
+    bool, str, enum.Enum). In order to store an arbitrary type in a Key, users
+    need to provide a serializer for that type when instantiating a Key. That
+    serializer should be an implementation of this protocol.
+    """
+
+    def toStr(self, value: _T) -> str:
+        """
+        Returns a string representation of the given value, that can be used by
+        :meth:`fromStr()` to reconstruct a copy of that value.
+        """
+        ...
+
+    def fromStr(self, string: str) -> Optional[_T]:
+        """
+        Takes a string that represents a serialized instance of a value, and
+        returns a newly created instance that corresponds to that string, or
+        None if the string is not a valid representation of a value for this
+        serializer's type.
+        """
+        ...
 
 
 @runtime_checkable
 class Inheriter(Protocol):
     def setParent(self: Self, parent: Optional[Self]) -> None:
         ...
 
@@ -56,36 +91,35 @@
 
 
 @runtime_checkable
 class Dumpable(Protocol):
     def dumpFields(self) -> Iterable[tuple[str, Optional[str]]]:
         ...
 
-    def restoreField(self, path: str, value: Optional[str]) -> None:
+    def restoreField(self, path: str, value: Optional[str]) -> bool:
         ...
 
     def isSet(self) -> bool:
         ...
 
 
 @runtime_checkable
 class UpdateNotifier(Protocol):
-    def onUpdateCall(self, callback: Callable[[Any], None]) -> None:
+    def onUpdateCall(self, callback: Callable[[Any], Any]) -> None:
         ...
 
 
 @runtime_checkable
 class ItemTemplate(Protocol):
     def newInstance(self: Self) -> Self:
         ...
 
 
 @runtime_checkable
 class Containable(Protocol):
-
     _PATH_SEPARATOR: str
 
     def setContainer(
         self, label: str, container: Optional["Container"]
     ) -> None:
         ...
 
@@ -120,15 +154,14 @@
 
     _PATH_SEPARATOR: str = "."
 
     _field_label: str
     _container: Optional[weakref.ref[Container]]
 
     def __init__(self) -> None:
-
         super().__init__()
 
         self._field_label = ""
         self._container = None
 
     def setContainer(self, label: str, container: Optional[Container]) -> None:
         """
```

### Comparing `SunsetSettings-0.4.0/sunset/registry.py` & `SunsetSettings-0.5.0/sunset/registry.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,82 +6,70 @@
 
 from .non_hashable_set import NonHashableSet
 
 _T = TypeVar("_T")
 
 
 class CallbackRegistry(MutableSet[Callable[[_T], None]]):
-
     _content: NonHashableSet[weakref.ref[Callable[[_T], None]]]
 
     def __init__(self) -> None:
-
         super().__init__()
 
         # We can't just use a WeakNonHashableSet because it does not know how to
         # take references to methods. Instead we use a regular NonHashableSet
         # and manually take the proper type of weak reference when adding a
         # callable to the set.
 
         self._content = NonHashableSet()
 
     def add(self, value: Callable[[_T], None]) -> None:
-
         if isinstance(value, MethodType):
-
             # Note: WeakMethod has incorrect type annotations, so we have to
             # ignore types here.
 
             r = weakref.WeakMethod(value, self._onExpire)  # type: ignore
 
         else:
             r = weakref.ref(value, self._onExpire)
 
         self._content.add(r)
 
     def __contains__(self, value: Any) -> bool:
-
         return any(self._isSameCallable(candidate, value) for candidate in self)
 
     def __iter__(self) -> Iterator[Callable[[_T], None]]:
-
         for ref in self._content:
             value = ref()
             if value is not None:
                 yield value
 
     def __len__(self) -> int:
-
         return len(self._content)
 
     def discard(self, value: Callable[[_T], None]) -> None:
-
         refs = list(self._content)
         for ref in refs:
-            callable = ref()
-            if callable is not None and self._isSameCallable(callable, value):
+            callable_ = ref()
+            if callable_ is not None and self._isSameCallable(callable_, value):
                 self._content.discard(ref)
 
     def callAll(self, value: _T) -> None:
-
         for callback in self:
             callback(value)
 
     @staticmethod
     def _isSameCallable(
         callable1: Callable[[_T], None], callable2: Callable[[_T], None]
     ) -> bool:
-
         if isinstance(callable1, MethodType) and isinstance(
             callable2, MethodType
         ):
             return (
                 callable1.__self__ is callable2.__self__
                 and callable1.__name__ == callable2.__name__
             )
 
-        else:
-            return callable1 is callable2
+        return callable1 is callable2
 
     def _onExpire(self, ref: weakref.ref[Callable[[_T], None]]) -> None:
-
         self._content.discard(ref)
```

### Comparing `SunsetSettings-0.4.0/sunset/settings.py` & `SunsetSettings-0.5.0/sunset/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     Iterator,
     MutableSet,
     Optional,
     TypeVar,
     Union,
 )
 
+from .autosaver import AutoSaver
 from .bunch import Bunch
 from .exporter import normalize, load_from_file, save_to_file
 from .lockable import Lockable
 from .non_hashable_set import NonHashableSet
 from .protocols import UpdateNotifier
 
 _MAIN = "main"
@@ -58,26 +59,35 @@
     >>> class AnimalSettings(Settings):
     ...     hearts: Key[int] = Key(default=0)
     ...     legs: Key[int]   = Key(default=0)
     ...     wings: Key[int]  = Key(default=0)
     ...     fur: Key[bool]   = Key(default=False)
     >>> animals = AnimalSettings()
     >>> animals.hearts.set(1)
+    True
     >>> mammals = animals.newSection(name="mammals")
     >>> mammals.fur.set(True)
+    True
     >>> mammals.legs.set(4)
+    True
     >>> humans = mammals.newSection(name="humans")
     >>> humans.legs.set(2)
+    True
     >>> humans.fur.set(False)
+    True
     >>> birds = animals.newSection(name="birds")
     >>> birds.legs.set(2)
+    True
     >>> birds.wings.set(2)
+    True
     >>> aliens = animals.newSection()  # No name given!
     >>> aliens.hearts.set(2)
+    True
     >>> aliens.legs.set(7)
+    True
     >>> print(mammals.hearts.get())
     1
     >>> print(mammals.legs.get())
     4
     >>> print(mammals.wings.get())
     0
     >>> print(mammals.fur.get())
@@ -126,25 +136,27 @@
     MAIN: str = _MAIN
 
     _SECTION_SEPARATOR = "/"
 
     _section_name: str
     _children: MutableSet[Bunch]
     _autosaver: Optional[ContextManager[Any]] = None
+    _autosaver_class: type[AutoSaver]
 
     def __post_init__(self) -> None:
         super().__post_init__()
 
         self._section_name = ""
 
         # Note that this overrides the similarly named attribute from the parent
         # class. In the parent class, the set does not keep references to its
         # items; in this class, it does.
 
         self._children = NonHashableSet()
+        self._autosaver_class = AutoSaver
 
     @Lockable.with_lock
     def newSection(self: Self, name: Optional[str] = None) -> Self:
         """
         Creates and returns a new instance of this class. Each key of the new
         instance will inherit from the key of the same name on the parent
         instance.
@@ -283,14 +295,15 @@
         if name == previous_name:
             return name
 
         if (parent := self.parent()) is None:
             self._section_name = name
 
         else:
+            # pylint: disable-next=protected-access
             parent._setUniqueNameForSection(name, self)
 
         if self.sectionName() != previous_name:
             self.triggerUpdateNotification(self)
 
         return self.sectionName()
 
@@ -304,14 +317,15 @@
             )
 
             i = 0
             while candidate in other_names:
                 i += 1
                 candidate = f"{name}_{i}"
 
+        # pylint: disable=protected-access
         section._section_name = candidate
 
     def sectionName(self) -> str:
         """
         Returns the current name of this Settings instance. This name will be
         used to generate the heading under which this Settings instance will be
         persisted by the :meth:`save()` method.
@@ -347,29 +361,33 @@
         """
 
         super().setParent(parent)
 
         # Ensure that this section's name is unique in its parent.
 
         if parent is not None:
+            # pylint: disable=protected-access
             parent._setUniqueNameForSection(self._section_name, self)
 
-    def onUpdateCall(self, callback: Callable[[Any], None]) -> None:
+    # Not actually useless. This lets us override the docstring with
+    # Settings-specific info.
+    # pylint: disable-next=useless-parent-delegation
+    def onUpdateCall(self, callback: Callable[[Any], Any]) -> None:
         """
         Adds a callback to be called whenever this Settings instance is updated.
         A Settings instance is considered updated when any of its fields is
         updated, or when its name is updated.
 
         The callback will be called with as its argument whichever field was
         just updated.
 
         Args:
             callback: A callable that will be called with one argument of type
                 :class:`~sunset.List`, :class:`~sunset.Bunch` or
-                :class:`~sunset.Key`, and returns None.
+                :class:`~sunset.Key`.
 
         Returns:
             None.
 
         Note:
             This method does not increase the reference count of the given
             callback.
@@ -426,42 +444,46 @@
                 yield self.fieldPath(), None
             else:
                 yield from super().dumpFields()
 
             for section in sorted(self.sections()):
                 yield from section.dumpFields()
 
-    def restoreField(self, path: str, value: Optional[str]) -> None:
+    def restoreField(self, path: str, value: Optional[str]) -> bool:
         """
         Internal.
         """
 
         if self._SECTION_SEPARATOR not in path:
-            return
+            return False
 
         section_name, path = path.split(self._SECTION_SEPARATOR, 1)
         if self.sectionName() != section_name:
-            return
+            return False
+
+        success: bool = False
 
         _update_notification_enabled = self._update_notification_enabled
         self._update_notification_enabled = False
 
         if self._SECTION_SEPARATOR in path:
             subsection_name, _ = path.split(self._SECTION_SEPARATOR, 1)
             if subsection_name:
                 section = self.getOrCreateSection(subsection_name)
-                section.restoreField(path, value)
+                success = section.restoreField(path, value)
 
         else:
             field_label, *_ = path.split(self._PATH_SEPARATOR, 1)
             if (field := self._fields.get(field_label)) is not None:
-                field.restoreField(path, value)
+                success = field.restoreField(path, value)
 
         self._update_notification_enabled = _update_notification_enabled
 
+        return success
+
     def save(self, file: IO[str], blanklines: bool = False) -> None:
         """
         Writes the contents of this Settings instance and its subsections in
         text form to the given file object.
 
         Args:
             file: A text file object where to save this Settings instance.
@@ -503,14 +525,20 @@
         Returns:
             None.
         """
 
         for path, dump in load_from_file(file, self.sectionName()):
             self.restoreField(path, dump)
 
+    def setAutosaverClass(self, class_: type[AutoSaver]) -> None:
+        """
+        Internal.
+        """
+        self._autosaver_class = class_
+
     def autosave(
         self,
         path: Union[str, pathlib.Path],
         save_on_update: bool = True,
         save_delay: int = 0,
         logger: Optional[logging.Logger] = None,
     ) -> ContextManager[Any]:
@@ -542,22 +570,18 @@
                 any, while loading or saving settings. If none is given, the
                 default root logger will be used.
 
         Returns:
             An AutoSaver context manager.
         """
 
-        # Only do the import here in order to avoid cyclical imports.
-
-        from .autosaver import AutoSaver
-
         # Keep a reference to the AutoSaver instance, so that its lifetime is
         # bound to that of this Settings instance.
 
-        self._autosaver = AutoSaver(
+        self._autosaver = self._autosaver_class(
             self,
             path,
             save_on_update=save_on_update,
             save_delay=save_delay,
             logger=logger,
         )
         return self._autosaver
```

### Comparing `SunsetSettings-0.4.0/sunset/timer.py` & `SunsetSettings-0.5.0/sunset/timer.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,44 +11,38 @@
         ...
 
     def cancel(self) -> None:
         ...
 
 
 class PersistentTimer:
-
     _timer: Optional[threading.Timer]
     _function: Callable[[], Any]
     _lock: threading.Lock
 
     def __init__(self, function: Callable[[], Any]) -> None:
-
         self._timer = None
         self._function = function
         self._lock = threading.Lock()
 
     def start(self, interval: float) -> None:
-
         if interval <= 0.0:
             self._timeout()
             return
 
         with self._lock:
             if self._timer is None:
                 self._timer = threading.Timer(interval, self._timeout)
                 self._timer.start()
 
     def cancel(self) -> None:
-
         with self._lock:
             if self._timer is not None:
                 self._timer.cancel()
                 self._timer = None
 
     def _timeout(self) -> None:
-
         self.cancel()
         self._function()
 
     def __del__(self) -> None:
-
         self.cancel()
```

### Comparing `SunsetSettings-0.4.0/tests/test_autosaver.py` & `SunsetSettings-0.5.0/tests/test_autosaver.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,105 +7,95 @@
 
 from pytest_mock import MockerFixture
 
 from sunset import AutoSaver, Key, Settings
 
 
 class MockTimer:
-
     _clock: float
     _interval: float
     _function: Callable[[], None]
 
     def __init__(self, function: Callable[[], Any]) -> None:
-
         self._function = function
         self._interval = 0
         self._clock = -1.0
 
     def cancel(self) -> None:
-
         self._clock = -1.0
 
     def start(self, interval: float) -> None:
-
         if self._clock < 0:
             self._interval = interval
             self._clock = 0.0
 
     def advanceTime(self, time: float) -> None:
-
         if self._clock >= 0:
             self._clock += time
             if self._clock >= self._interval:
                 self._function()
 
 
 class ExampleSettings(Settings):
     key_str = Key(default="")
 
 
 class TestAutosaver:
     def test_load_on_init(self, tmp_path: pathlib.Path) -> None:
-
         settings_file = tmp_path / "test.conf"
         settings_file.write_text("[main]\nkey_str = test\n")
 
         settings = ExampleSettings()
 
         assert settings.key_str.get() == ""
 
         AutoSaver(settings, settings_file)
 
         assert settings.key_str.get() == "test"
 
     def test_no_load_on_init(self, tmp_path: pathlib.Path) -> None:
-
         settings_file = tmp_path / "test.conf"
         settings_file.write_text("[main]\nkey_str = test\n")
 
         settings = ExampleSettings()
 
         assert settings.key_str.get() == ""
 
         AutoSaver(settings, settings_file, load_on_init=False)
 
         assert settings.key_str.get() == ""
 
     def test_no_unneeded_saving(self, tmp_path: pathlib.Path) -> None:
-
         settings_file = tmp_path / "test.conf"
         settings = ExampleSettings()
         autosaver = AutoSaver(
             settings, settings_file, save_on_update=True, save_on_delete=True
         )
 
         assert not settings_file.exists()
 
         autosaver.__del__()  # Simulate garbage collection.
 
         assert not settings_file.exists()
 
     def test_autosave_on_update(self, tmp_path: pathlib.Path) -> None:
-
         settings_file = tmp_path / "test.conf"
         settings = ExampleSettings()
         autosaver = AutoSaver(settings, settings_file, save_on_delete=False)
 
         assert not settings_file.exists()
 
         settings.key_str.set("test")
 
         assert settings_file.exists()
         assert settings_file.read_text() == "[main]\nkey_str = test\n"
 
         del autosaver  # So that it's not unused.
 
     def test_autosave_on_delete(self, tmp_path: pathlib.Path) -> None:
-
         settings_file = tmp_path / "test.conf"
         settings = ExampleSettings()
         autosaver = AutoSaver(settings, settings_file, save_on_update=False)
 
         settings.key_str.set("test")
 
         assert not settings_file.exists()
@@ -114,42 +104,39 @@
 
         assert settings_file.exists()
         assert settings_file.read_text() == "[main]\nkey_str = test\n"
 
     def test_autosave_creates_missing_dirs(
         self, tmp_path: pathlib.Path
     ) -> None:
-
         settings = ExampleSettings()
         settings_file = tmp_path / "multiple" / "levels" / "deep" / "test.conf"
         autosaver = AutoSaver(
             settings, settings_file, save_on_update=False, save_on_delete=False
         )
 
         assert not settings_file.parent.exists()
 
         autosaver.doSave()
 
         assert settings_file.parent.exists()
 
     def test_context_manager(self, tmp_path: pathlib.Path) -> None:
-
         settings = ExampleSettings()
         settings_file = tmp_path / "test.conf"
         with AutoSaver(
             settings, settings_file, save_on_update=False, save_on_delete=False
         ):
             settings.key_str.set("test")
             assert not settings_file.exists()
 
         assert settings_file.exists()
         assert settings_file.read_text() == "[main]\nkey_str = test\n"
 
     def test_delayed_save(self, tmp_path: pathlib.Path) -> None:
-
         settings_file = tmp_path / "test.conf"
         settings = ExampleSettings()
         autosaver = AutoSaver(
             settings, settings_file, save_on_delete=False, save_delay=2.0
         )
 
         mock_timer = autosaver.setSaveTimerClass(MockTimer)
@@ -186,15 +173,14 @@
             ExampleSettings(), "~/with/tilde", load_on_init=False
         )
         assert str(saver2.path()) == "HOME/with/tilde"
 
     def test_exceptions(
         self, tmp_path: pathlib.Path, mocker: MockerFixture
     ) -> None:
-
         settings_file = tmp_path / "actually_a_folder"
         settings_file.mkdir(parents=True)
 
         logger_stub = mocker.MagicMock(logging.Logger)
 
         saver = AutoSaver(
             ExampleSettings(),
```

### Comparing `SunsetSettings-0.4.0/tests/test_bunch.py` & `SunsetSettings-0.5.0/tests/test_bunch.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,80 +15,80 @@
     a = Key("default a")
     inner_bunch = InnerBunch()
     list = List(Item(), order=List.PARENT_LAST)
     _private = Key("private")
 
 
 class TestBunch:
-    def test_protocol_implementation(self):
+    def test_protocol_implementation(self) -> None:
         bunch = ExampleBunch()
         assert isinstance(bunch, protocols.Field)
         assert isinstance(bunch, protocols.Container)
 
-    def test_creation(self):
+    def test_creation(self) -> None:
         bunch = ExampleBunch()
         bunch.list.appendOne()
         assert bunch.a.get() == "default a"
         assert bunch.inner_bunch.b.get() == 42
         assert bunch.list[0].c.get() == "default c"
 
-    def test_uninstantiated_field_fails(self):
+    def test_uninstantiated_field_fails(self) -> None:
         class InnerBunch(Bunch):
             pass
 
         class FaultyBunch(Bunch):
             inner = InnerBunch
 
         with pytest.raises(TypeError):
             FaultyBunch()
 
-    def test_inner_bunch_definition_is_fine(self):
+    def test_inner_bunch_definition_is_fine(self) -> None:
         class FineBunch(Bunch):
             class InnerBunch(Bunch):
                 pass
 
             inner = InnerBunch()
 
         FineBunch()
 
-    def test_fields_cant_override_existing_attributes(self):
+    def test_fields_cant_override_existing_attributes(self) -> None:
         # "__init__" is an attribute that happens to exist on the class.
 
         assert getattr(Bunch, "__init__", None) is not None
 
         class FaultyBunch(Bunch):
             __init__ = Key(default="test")  # type: ignore[assignment]
 
         with pytest.raises(TypeError):
             FaultyBunch()
 
-    def test_inheritance(self):
+    def test_inheritance(self) -> None:
         parent_bunch = ExampleBunch()
         child_bunch = ExampleBunch()
 
         assert child_bunch not in parent_bunch.children()
         assert child_bunch.parent() is None
 
         child_bunch.setParent(parent_bunch)
         assert child_bunch in parent_bunch.children()
         assert child_bunch.parent() is parent_bunch
 
         child_bunch.setParent(None)
         assert child_bunch not in parent_bunch.children()
         assert child_bunch.parent() is None
 
-    def test_parenting(self):
+    def test_parenting(self) -> None:
         parent_bunch = ExampleBunch()
         child_bunch = ExampleBunch()
         child_bunch.setParent(parent_bunch)
 
         assert child_bunch.parent() is parent_bunch
         assert child_bunch in parent_bunch.children()
 
-    def test_reparenting(self):
+    def test_reparenting(self) -> None:
         bunch1 = ExampleBunch()
         bunch2 = ExampleBunch()
         child_bunch = ExampleBunch()
 
         assert child_bunch not in bunch1.children()
         assert child_bunch not in bunch2.children()
         assert child_bunch.parent() is None
@@ -104,25 +104,25 @@
         assert child_bunch.parent() is bunch2
 
         child_bunch.setParent(None)
         assert child_bunch not in bunch1.children()
         assert child_bunch not in bunch2.children()
         assert child_bunch.parent() is None
 
-    def test_inheritance_propagation(self):
+    def test_inheritance_propagation(self) -> None:
         parent_bunch = ExampleBunch()
         child_bunch = ExampleBunch()
         child_bunch.setParent(parent_bunch)
 
         assert child_bunch.a.parent() is parent_bunch.a
         assert child_bunch.inner_bunch.parent() is parent_bunch.inner_bunch
         assert child_bunch.inner_bunch.b.parent() is parent_bunch.inner_bunch.b
         assert child_bunch.list.parent() is parent_bunch.list
 
-    def test_inheritance_values(self):
+    def test_inheritance_values(self) -> None:
         parent_bunch = ExampleBunch()
         child_bunch = ExampleBunch()
         child_bunch.setParent(parent_bunch)
 
         parent_bunch.a.set("test parent")
         assert child_bunch.a.get() == "test parent"
         child_bunch.a.set("test child")
@@ -152,33 +152,33 @@
         ]
         del parent_bunch.list[0]
         assert [item.c.get() for item in parent_bunch.list.iter()] == []
         assert [item.c.get() for item in child_bunch.list.iter()] == [
             "test child"
         ]
 
-    def test_field_label(self):
+    def test_field_label(self) -> None:
         bunch = ExampleBunch()
 
         assert bunch.fieldLabel() == ""
         assert bunch.inner_bunch.fieldLabel() == "inner_bunch"
 
-    def test_field_path(self):
+    def test_field_path(self) -> None:
         bunch = ExampleBunch()
         assert bunch.fieldPath() == "."
         assert bunch.a.fieldPath() == ".a"
         assert bunch.inner_bunch.fieldPath() == ".inner_bunch."
         assert bunch.inner_bunch.b.fieldPath() == ".inner_bunch.b"
         assert bunch.inner_bunch.b.fieldPath() == ".inner_bunch.b"
         assert bunch.list.fieldPath() == ".list."
         bunch.list.appendOne()
         assert bunch.list[0].fieldPath() == ".list.1."
         assert bunch.list[0].c.fieldPath() == ".list.1.c"
 
-    def test_dump_fields(self):
+    def test_dump_fields(self) -> None:
         bunch = ExampleBunch()
         assert list(bunch.dumpFields()) == []
 
         bunch.a.set("test dump a")
         bunch.inner_bunch.b.set(101)
         bunch.list.appendOne().c.set("test dump c 1")
         bunch.list.appendOne()
@@ -189,15 +189,15 @@
             (".a", "test dump a"),
             (".inner_bunch.b", "101"),
             (".list.1.c", "test dump c 1"),
             (".list.2", None),
             (".list.3.c", "test dump c 3"),
         ]
 
-    def test_restore_field(self, mocker: MockerFixture):
+    def test_restore_field(self, mocker: MockerFixture) -> None:
         callback = mocker.stub()
 
         # Test all flavors of valid paths. Also, restoring a field should not
         # trigger a callbacak.
 
         bunch = ExampleBunch()
         bunch.onUpdateCall(callback)
@@ -244,15 +244,15 @@
 
         other_bunch.restoreField(".invalid", "invalid path")
         assert not other_bunch.isSet()
 
         other_bunch.restoreField("", "invalid path")
         assert not other_bunch.isSet()
 
-    def test_persistence(self):
+    def test_persistence(self) -> None:
         # A Bunch does not keep a reference to its parent or children.
 
         bunch = ExampleBunch()
         level1 = ExampleBunch()
         level2 = ExampleBunch()
         level1.setParent(bunch)
         level2.setParent(level1)
@@ -261,15 +261,15 @@
         assert len(list(level1.children())) == 1
 
         del bunch
         del level2
         assert level1.parent() is None
         assert len(list(level1.children())) == 0
 
-    def test_key_updated_notification(self, mocker: MockerFixture):
+    def test_key_updated_notification(self, mocker: MockerFixture) -> None:
         callback = mocker.stub()
 
         bunch = ExampleBunch()
         bunch.onUpdateCall(callback)
 
         child = ExampleBunch()
         child.setParent(bunch)
@@ -289,7 +289,18 @@
         bunch.list[0].c.set("test 2")
         callback.assert_called_once_with(bunch.list[0].c)
         callback.reset_mock()
 
         child.a.set("test 3")
         callback.assert_not_called()
         callback.reset_mock()
+
+    def test_callback_type_is_flexible(self) -> None:
+        bunch = ExampleBunch()
+
+        class Dummy:
+            pass
+
+        def callback(_: ExampleBunch) -> Dummy:
+            return Dummy()
+
+        bunch.onUpdateCall(callback)
```

### Comparing `SunsetSettings-0.4.0/tests/test_concurrency.py` & `SunsetSettings-0.5.0/tests/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.4.0/tests/test_exporter.py` & `SunsetSettings-0.5.0/tests/test_exporter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 import io
 
 from sunset import exporter
 
 
-def test_escape():
-
+def test_escape() -> None:
     assert exporter.maybe_escape("") == '""'
     assert exporter.maybe_escape("123") == "123"
     assert exporter.maybe_escape("test test") == "test test"
     assert exporter.maybe_escape("   ") == '"   "'
     assert exporter.maybe_escape(" a") == '" a"'
     assert exporter.maybe_escape("a ") == '"a "'
     assert exporter.maybe_escape('"') == r'"\""'
     assert exporter.maybe_escape("test\ntest") == r'"test\ntest"'
     assert exporter.maybe_escape(r"test\test") == r'"test\\test"'
 
 
-def test_unescape():
-
+def test_unescape() -> None:
     assert exporter.unescape("") == ""
     assert exporter.unescape('""') == ""
     assert exporter.unescape('"') == '"'
     assert exporter.unescape('"test') == "test"
     assert exporter.unescape('test"') == "test"
     assert exporter.unescape("123") == "123"
     assert exporter.unescape("test \ttest") == "test \ttest"
@@ -29,32 +27,30 @@
     assert exporter.unescape('" a"') == " a"
     assert exporter.unescape('"a "') == "a "
     assert exporter.unescape(r'"\""') == '"'
     assert exporter.unescape(r'"test\ntest"') == "test\ntest"
     assert exporter.unescape(r'"test\\test"') == r"test\test"
 
 
-def test_escape_reversible():
-
+def test_escape_reversible() -> None:
     for string in (
         "",
         "123",
         "test test",
         "   ",
         " a",
         "a ",
         '"',
         "test\ntest",
         r"test\test",
     ):
         assert exporter.unescape(exporter.maybe_escape(string)) == string
 
 
-def test_save():
-
+def test_save() -> None:
     input = [
         ("main/a", "1"),
         ("main/b.c", "test"),
         ("main/d.1.e", "test 2\ntest 2"),
         ("main/d.2.e", "  "),
         ("main/level1/b.c", "sub test"),
         ("main/level1/level2/a", "sub sub test"),
@@ -77,17 +73,16 @@
 
 [level1/level2]
 a = sub sub test
 """
     )
 
 
-def test_load():
-
-    MAIN = "main"
+def test_load() -> None:
+    _main = "main"
 
     input = io.StringIO(
         """\
 [main]
 a = 1
 b.c = test
 d.1.e = "test 2\\ntest 2"
@@ -99,49 +94,45 @@
 [level1/level2]
 a = sub sub test
 
 [empty]
 """
     )
 
-    assert list(exporter.load_from_file(input, MAIN)) == [
+    assert list(exporter.load_from_file(input, _main)) == [
         ("main/", ""),
         ("main/a", "1"),
         ("main/b.c", "test"),
         ("main/d.1.e", "test 2\ntest 2"),
         ("main/d.2.e", "  "),
         ("main/level1/", ""),
         ("main/level1/b.c", "sub test"),
         ("main/level1/level2/", ""),
         ("main/level1/level2/a", "sub sub test"),
         ("main/empty/", ""),
     ]
 
 
-def test_section_cleanup():
-
+def test_section_cleanup() -> None:
     for input, expected in (
         ("", ""),
         (" // / ", ""),
         (" test 1 / test 2 ", "test1/test2"),
         ("test1///test2", "test1/test2"),
         ("/test", "test"),
         ("test/", "test"),
         ("  //   / I'snt This a Test? / // Yes! / // / ", "isntthisatest/yes"),
     ):
-
         assert exporter.cleanup_section(input) == expected
 
 
-def test_path_cleanup():
-
+def test_path_cleanup() -> None:
     for input, expected in (
         ("", ""),
         (" .. . ", ""),
         (" test 1 . test 2 ", "test1.test2"),
         ("test1...test2", "test1.test2"),
         (".test", "test"),
         ("test.", "test"),
         ("  ..   . I'snt This a Test? . .. Yes! . .. . ", "IsntThisaTest.Yes"),
     ):
-
         assert exporter.cleanup_path(input) == expected
```

### Comparing `SunsetSettings-0.4.0/tests/test_key.py` & `SunsetSettings-0.5.0/tests/test_key.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,69 +11,137 @@
     def __init__(self, value: str) -> None:
         self._value = value
 
     def toStr(self) -> str:
         return self._value
 
     @staticmethod
-    def fromStr(value: str) -> Optional["ExampleSerializable"]:
-        return ExampleSerializable(value)
+    def fromStr(string: str) -> Optional["ExampleSerializable"]:
+        return ExampleSerializable(string)
 
 
 class ExampleEnum(SerializableEnum):
     ONE = 1
     TWO = 2
 
 
 class ExampleFlag(SerializableFlag):
     ONE = 1
     TWO = 2
     THREE = ONE | TWO
 
 
 class TestKey:
-    def test_protocol_implementation(self):
+    def test_protocol_implementation(self) -> None:
         key = Key(default="")
         assert isinstance(key, protocols.Field)
 
-    def test_default(self):
+    def test_default(self) -> None:
         assert Key(default="default").get() == "default"
         assert Key(default=0).get() == 0
         assert type(Key(default=False).get()) is bool
         assert not Key(default=False).get()
         assert Key(default=12.345e-67).get() == 12.345e-67
         assert Key(default=ExampleEnum.ONE).get() == ExampleEnum.ONE
         assert (
             Key(default=ExampleFlag.ONE | ExampleFlag.TWO).get()
             == ExampleFlag.THREE
         )
         with pytest.raises(TypeError):
             Key(default=object())  # type: ignore # It's the point!
 
-    def test_set(self):
+    def test_set(self) -> None:
         key = Key(default="test")
         key.set("other")
         assert key.get() == "other"
 
-    def test_clear(self):
+    def test_clear(self) -> None:
         key = Key(default="default")
         key.set("other")
         assert key.get() != "default"
 
         key.clear()
         assert key.get() == "default"
 
-    def test_serializable_type(self):
+    def test_serializable_type(self) -> None:
         value = ExampleSerializable.fromStr("dummy")
         assert value is not None
         key: Key[ExampleSerializable] = Key(default=value)
 
         assert key.get().toStr() == "dummy"
 
-    def test_value_change_callback(self, mocker: MockerFixture):
+    def test_missing_serializer(self) -> None:
+        class NotSerializable:
+            pass
+
+        with pytest.raises(TypeError):
+            Key(default=NotSerializable())
+
+    def test_explicit_serializer(self) -> None:
+        class NotSerializable:
+            pass
+
+        class Serializer:
+            def toStr(self, value: NotSerializable) -> str:
+                return "test"
+
+            def fromStr(self, string: str) -> NotSerializable:
+                return NotSerializable()
+
+        key = Key(default=NotSerializable(), serializer=Serializer())
+        key.set(NotSerializable())
+        assert list(key.dumpFields()) == [("", "test")]
+
+    def test_serializer_override(self) -> None:
+        class Serializer:
+            def toStr(self, value: str) -> str:
+                return value + "-TEST"
+
+            def fromStr(self, string: str) -> Optional[str]:
+                if string.endswith("-TEST"):
+                    return string[:-5]
+                return None
+
+        key = Key(default="", serializer=Serializer())
+        key.set("value")
+        assert list(key.dumpFields()) == [("", "value-TEST")]
+
+        key.restoreField("", "other value-TEST")
+        assert key.get() == "other value"
+
+    def test_validator(self) -> None:
+        def isEven(i: int) -> bool:
+            return i % 2 == 0
+
+        key: Key[int] = Key(default=0, validator=isEven)
+
+        assert not key.set(1)
+        assert key.get() == 0
+
+        assert key.set(2)
+        assert key.get() == 2
+
+        assert not key.restoreField("", "3")
+        assert key.get() == 2
+
+        assert key.restoreField("", "4")
+        assert key.get() == 4
+
+        def isOdd(i: int) -> bool:
+            return i % 2 == 1
+
+        key.setValidator(isOdd)
+
+        assert key.set(5)
+        assert key.get() == 5
+
+        assert not key.set(6)
+        assert key.get() == 5
+
+    def test_value_change_callback(self, mocker: MockerFixture) -> None:
         callback = mocker.stub()
 
         key = Key(default="default")
 
         key.onValueChangeCall(callback)
 
         key.set("default")
@@ -87,15 +155,17 @@
         key.clear()
         callback.assert_called_once_with("default")
         callback.reset_mock()
 
         key.clear()
         callback.assert_not_called()
 
-    def test_value_change_callback_inheritance(self, mocker: MockerFixture):
+    def test_value_change_callback_inheritance(
+        self, mocker: MockerFixture
+    ) -> None:
         callback_sub_child1 = mocker.stub()
         callback_sub_child2 = mocker.stub()
 
         # Set up keys so that one parent key has two children key, each with one
         # child of its own.
 
         parent_key = Key(default="default")
@@ -148,15 +218,15 @@
 
         # Clearing the parent does change the value inherited by the grandchild.
 
         parent_key.clear()
         callback_sub_child1.assert_called_once_with("default")
         callback_sub_child1.reset_mock()
 
-    def test_key_updated_callback(self, mocker: MockerFixture):
+    def test_key_updated_callback(self, mocker: MockerFixture) -> None:
         callback = mocker.stub()
 
         key = Key(default="default")
         assert isinstance(key, protocols.UpdateNotifier)
 
         key.onUpdateCall(callback)
 
@@ -176,27 +246,42 @@
         callback.assert_called_once_with(key)
         callback.reset_mock()
 
         key.clear()
         callback.assert_not_called()
         callback.reset_mock()
 
-    def test_updater(self):
+    def test_callback_type_is_flexible(self) -> None:
+        key = Key("")
+
+        class Dummy:
+            pass
+
+        def callback1(_: Key[str]) -> Dummy:
+            return Dummy()
+
+        def callback2(_: str) -> Dummy:
+            return Dummy()
+
+        key.onUpdateCall(callback1)
+        key.onValueChangeCall(callback2)
+
+    def test_updater(self) -> None:
         key = Key("")
 
         def updater(value: str) -> str:
             return value + "x"
 
         assert key.get() == ""
         key.updateValue(updater)
         assert key.get() == "x"
         key.updateValue(updater)
         assert key.get() == "xx"
 
-    def test_inheritance(self):
+    def test_inheritance(self) -> None:
         parent_key = Key(default="default a")
         child_key = Key(default="")
 
         assert child_key not in parent_key.children()
         child_key.setParent(parent_key)
         assert child_key in parent_key.children()
 
@@ -210,25 +295,25 @@
 
         parent_key.clear()
         assert child_key.get() == "new b"
 
         child_key.clear()
         assert child_key.get() == "default a"
 
-    def test_inherit_wrong_type(self):
+    def test_inherit_wrong_type(self) -> None:
         parent_key = Key(default="str")
         child_key = Key(default=0)
 
         # Ignore the type error, as it's the whole point of the test.
 
         child_key.setParent(parent_key)  # type: ignore
 
         assert child_key.parent() is None
 
-    def test_inherit_revert(self):
+    def test_inherit_revert(self) -> None:
         parent_key = Key(default="default a")
         child_key = Key(default="default b")
 
         assert child_key not in parent_key.children()
         assert child_key.parent() is None
 
         child_key.setParent(parent_key)
@@ -237,15 +322,15 @@
         assert child_key.parent() is parent_key
 
         child_key.setParent(None)
 
         assert child_key not in parent_key.children()
         assert child_key.parent() is None
 
-    def test_repr(self):
+    def test_repr(self) -> None:
         key1 = Key(default="test")
         key2 = Key(default=12)
         key3 = Key(default="  test\ntest  ")
 
         assert repr(key1) == "<Key[str]:(test)>"
         assert repr(key2) == "<Key[int]:(12)>"
         assert repr(key3) == '<Key[str]:("  test\\ntest  ")>'
@@ -254,15 +339,15 @@
         key2.set(12)
         key3.set("  test\ntest  ")
 
         assert repr(key1) == "<Key[str]:test>"
         assert repr(key2) == "<Key[int]:12>"
         assert repr(key3) == '<Key[str]:"  test\\ntest  ">'
 
-    def test_reparenting(self):
+    def test_reparenting(self) -> None:
         key1 = Key(default="default a")
         key2 = Key(default="default b")
         child_key = Key(default="default c")
 
         assert child_key not in key1.children()
         assert child_key not in key2.children()
 
@@ -276,15 +361,15 @@
 
         child_key.setParent(None)
         assert child_key not in key1.children()
         assert child_key not in key2.children()
 
     def test_callback_triggered_on_parent_value_change(
         self, mocker: MockerFixture
-    ):
+    ) -> None:
         stub = mocker.stub()
 
         parent_key = Key(default="default a")
         child_key = Key(default="default b")
         child_key.setParent(parent_key)
 
         child_key.onValueChangeCall(stub)
@@ -300,38 +385,38 @@
         parent_key.set("test 2")
         stub.assert_called_once_with("test 2")
         stub.reset_mock()
 
         parent_key.clear()
         stub.assert_called_once_with("default a")
 
-    def test_field_label(self):
+    def test_field_label(self) -> None:
         class TestBunch(Bunch):
             key1 = Key("test")
             key2 = Key("test")
 
         bunch = TestBunch()
         assert bunch.key1.fieldLabel() == "key1"
         assert bunch.key2.fieldLabel() == "key2"
 
         key = Key("test")
         assert key.fieldLabel() == ""
 
-    def test_field_path(self):
+    def test_field_path(self) -> None:
         assert Key("").fieldPath() == ""
 
         class TestBunch(Bunch):
             key1 = Key("test")
             key2 = Key("test")
 
         bunch = TestBunch()
         assert bunch.key1.fieldPath() == ".key1"
         assert bunch.key2.fieldPath() == ".key2"
 
-    def test_dump_fields(self):
+    def test_dump_fields(self) -> None:
         # An unattached Key should get dumped. It just doesn't have a label.
 
         key = Key("")
         assert list(key.dumpFields()) == []
         key.set("test")
         assert list(key.dumpFields()) == [("", "test")]
 
@@ -358,110 +443,127 @@
 
         # A Key with a private label should not get dumped.
 
         assert list(bunch._private.dumpFields()) == []  # type: ignore
         bunch._private.set(111)  # type: ignore
         assert list(bunch._private.dumpFields()) == []  # type: ignore
 
-    def test_restore_field(self, mocker: MockerFixture):
+    def test_restore_field(self, mocker: MockerFixture) -> None:
         key: Key[int] = Key(0)
         callback = mocker.stub()
         key.onUpdateCall(callback)
 
         # The value should be set if the given label matches that of the Key. In
         # this case, "". In all other cases the value should not be set. As
         # well, restoring a field should not trigger a callback.
 
         assert not key.isSet()
-        key.restoreField("", "1")
+        assert key.restoreField("", "1")
         assert key.isSet()
         assert key.get() == 1
         callback.assert_not_called()
 
         key.clear()
         callback.reset_mock()
-        key.restoreField("invalid", "1")
+        assert not key.restoreField("invalid", "1")
         assert not key.isSet()
         callback.assert_not_called()
-        key.restoreField(".invalid", "1")
+        assert not key.restoreField(".invalid", "1")
         assert not key.isSet()
         callback.assert_not_called()
-        key.restoreField("invalid.", "1")
+        assert not key.restoreField("invalid.", "1")
         assert not key.isSet()
         callback.assert_not_called()
-        key.restoreField(".", "1")
+        assert not key.restoreField(".", "1")
         assert not key.isSet()
         callback.assert_not_called()
 
         # If multiple values are set, the last one sticks.
 
         key.clear()
         callback.reset_mock()
-        key.restoreField("", "1")
-        key.restoreField("", "2")
+        assert key.restoreField("", "1")
+        assert key.restoreField("", "2")
         assert key.get() == 2
         callback.assert_not_called()
 
         # Invalid values do not update the Key.
 
         key.clear()
         callback.reset_mock()
-        key.restoreField("", "?")
+        assert not key.restoreField("", "?")
         assert not key.isSet()
         callback.assert_not_called()
-        key.restoreField("", "")
+        assert not key.restoreField("", "")
         assert not key.isSet()
         callback.assert_not_called()
-        key.restoreField("", None)
+        assert key.restoreField("", None)
         assert not key.isSet()
         callback.assert_not_called()
 
         class TestBunch(Bunch):
             str_key = Key("")
 
         # Same as the above when the Key has a non-empty label.
 
         bunch = TestBunch()
-        bunch.str_key.restoreField("", "test")
+        assert not bunch.str_key.restoreField("", "test")
         assert not bunch.str_key.isSet()
-        bunch.str_key.restoreField("test", "test")
+        assert not bunch.str_key.restoreField("test", "test")
         assert not bunch.str_key.isSet()
-        bunch.str_key.restoreField(".str_key", "test")
+        assert not bunch.str_key.restoreField(".str_key", "test")
         assert not bunch.str_key.isSet()
-        bunch.str_key.restoreField("str_key.", "test")
+        assert not bunch.str_key.restoreField("str_key.", "test")
         assert not bunch.str_key.isSet()
 
-        bunch.str_key.restoreField("str_key", "test")
+        assert bunch.str_key.restoreField("str_key", "test")
         assert bunch.str_key.isSet()
         assert bunch.str_key.get() == "test"
 
-    def test_restore_field_serialization(self):
+    def test_restore_field_serialization(self) -> None:
         key_str: Key[str] = Key(default="")
-        key_str.restoreField("", "test")
+        assert key_str.restoreField("", "test")
         assert key_str.get() == "test"
 
         key_int: Key[int] = Key(default=0)
-        key_int.restoreField("", "12")
+        assert key_int.restoreField("", "12")
         assert key_int.get() == 12
 
         key_float: Key[float] = Key(default=1.2)
-        key_float.restoreField("", "3.4")
+        assert key_float.restoreField("", "3.4")
         assert key_float.get() == 3.4
 
         key_bool: Key[bool] = Key(default=False)
-        key_bool.restoreField("", "true")
+        assert key_bool.restoreField("", "true")
         assert key_bool.get()
 
         key_custom: Key[ExampleSerializable] = Key(
             default=ExampleSerializable("")
         )
-        key_custom.restoreField("", "test")
+        assert key_custom.restoreField("", "test")
         assert key_custom.get().toStr() == "test"
 
-    def test_persistence(self):
+    def test_invalid_restore_value_is_still_dumped(self) -> None:
+        key = Key[int](default=0)
+
+        assert not key.restoreField("", "12error")
+        assert key.get() == 0
+
+        assert list(key.dumpFields()) == [("", "12error")]
+
+        # Clearing or setting the Key also clears the bad value.
+
+        key.clear()
+        assert list(key.dumpFields()) == []
+
+        assert not key.restoreField("", "12error")
+        key.set(0)
+        assert list(key.dumpFields()) == [("", "0")]
+
+    def test_persistence(self) -> None:
         # A Key does not keep a reference to its parent or children.
 
         key: Key[str] = Key(default="")
         level1: Key[str] = Key(default="")
         level1.setParent(key)
         level2: Key[str] = Key(default="")
         level2.setParent(level1)
@@ -469,7 +571,24 @@
         assert level1.parent() is not None
         assert len(list(level1.children())) == 1
 
         del key
         del level2
         assert level1.parent() is None
         assert len(list(level1.children())) == 0
+
+    def test_new_instance_non_serializable(self) -> None:
+        class NotSerializable:
+            pass
+
+        class Serializer:
+            def toStr(self, value: NotSerializable) -> str:
+                return "test"
+
+            def fromStr(self, string: str) -> NotSerializable:
+                return NotSerializable()
+
+        key = Key(default=NotSerializable(), serializer=Serializer())
+        other_key = key.newInstance()
+        other_key.set(NotSerializable())
+
+        assert list(other_key.dumpFields()) == [("", "test")]
```

### Comparing `SunsetSettings-0.4.0/tests/test_list.py` & `SunsetSettings-0.5.0/tests/test_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,48 +6,48 @@
 
 
 class ExampleBunch(Bunch):
     test = Key("")
 
 
 class TestList:
-    def test_protocol_implementation(self):
+    def test_protocol_implementation(self) -> None:
         list_key: List[Key[int]] = List(Key(default=0))
         assert isinstance(list_key, protocols.Field)
         assert isinstance(list_key, protocols.Container)
 
-    def test_add_pop(self):
+    def test_add_pop(self) -> None:
         list_key: List[Key[str]] = List(Key(default=""))
         list_key.appendOne()
 
         assert len(list_key) == 1
 
         list_key[0].set("test")
         assert list_key[0].get() == "test"
 
         list_key.pop()
 
         assert len(list_key) == 0
 
-    def test_inheritance(self):
+    def test_inheritance(self) -> None:
         parent_list: List[Key[int]] = List(Key(default=0))
         child_list: List[Key[int]] = List(Key(default=0))
 
         assert child_list not in parent_list.children()
         assert child_list.parent() is None
 
         child_list.setParent(parent_list)
         assert child_list in parent_list.children()
         assert child_list.parent() is parent_list
 
         child_list.setParent(None)
         assert child_list not in parent_list.children()
         assert child_list.parent() is None
 
-    def test_reparenting(self):
+    def test_reparenting(self) -> None:
         list1: List[Key[int]] = List(Key(default=0))
         list2: List[Key[int]] = List(Key(default=0))
         child_list: List[Key[int]] = List(Key(default=0))
 
         assert child_list not in list1.children()
         assert child_list not in list2.children()
         assert child_list.parent() is None
@@ -63,15 +63,15 @@
         assert child_list.parent() is list2
 
         child_list.setParent(None)
         assert child_list not in list1.children()
         assert child_list not in list2.children()
         assert child_list.parent() is None
 
-    def test_iter_inheritance(self):
+    def test_iter_inheritance(self) -> None:
         def flatten(keys: Iterator[Key[str]]) -> list[str]:
             return [key.get() for key in keys]
 
         parent: List[Key[str]] = List(Key(default=""))
         child_default: List[Key[str]] = List(Key(default=""))
         child_iter_no_parent: List[Key[str]] = List(
             Key(default=""), order=List.NO_PARENT
@@ -106,15 +106,15 @@
             "child",
         ]
         assert flatten(child_default.iter(order=List.PARENT_LAST)) == [
             "child",
             "parent",
         ]
 
-    def test_dump_fields(self):
+    def test_dump_fields(self) -> None:
         key_list = List(Key(""))
         key_list.appendOne().set("test 1")
         key_list.appendOne()
         key_list.appendOne().set("test 3")
         assert list(key_list.dumpFields()) == [
             (".1", "test 1"),
             (".2", None),
@@ -150,104 +150,104 @@
         bunch = TestBunch()
         bunch.key_list.appendOne().set("test public")
         bunch._private.appendOne().set("test private")  # type: ignore
         assert list(bunch.dumpFields()) == [
             (".key_list.1", "test public"),
         ]
 
-    def test_restore_field(self, mocker: MockerFixture):
+    def test_restore_field(self, mocker: MockerFixture) -> None:
         callback = mocker.stub()
 
         # Test restoring one value. Also, restoring a field should not trigger a
         # callback.
 
         test_list1 = List(Key("default"))
         test_list1.onUpdateCall(callback)
-        test_list1.restoreField(".1", "test")
+        assert test_list1.restoreField(".1", "test")
         assert len(test_list1) == 1
         assert test_list1[0].get() == "test"
         callback.assert_not_called()
 
         # Test overwriting a restored value.
 
-        test_list1.restoreField(".1", "other test")
+        assert test_list1.restoreField(".1", "other test")
         assert len(test_list1) == 1
         assert test_list1[0].get() == "other test"
         callback.assert_not_called()
 
         # Test restoring a value that requires extending the List.
 
-        test_list1.restoreField(".5", "extension test")
+        assert test_list1.restoreField(".5", "extension test")
         assert len(test_list1) == 5
         assert test_list1[4].get() == "extension test"
         callback.assert_not_called()
 
         # Test different kinds of invalid restore paths.
 
         test_list2 = List(Key("default"))
         test_list2.onUpdateCall(callback)
 
-        test_list2.restoreField("", "test")
+        assert not test_list2.restoreField("", "test")
         assert len(test_list2) == 0
         callback.assert_not_called()
 
-        test_list2.restoreField("invalid", "test")
+        assert not test_list2.restoreField("invalid", "test")
         assert len(test_list2) == 0
         callback.assert_not_called()
 
-        test_list2.restoreField("invalid.1", "test")
+        assert not test_list2.restoreField("invalid.1", "test")
         assert len(test_list2) == 0
         callback.assert_not_called()
 
-        test_list2.restoreField("1.invalid", "test")
+        assert not test_list2.restoreField("1.invalid", "test")
         assert len(test_list2) == 0
         callback.assert_not_called()
 
-        test_list2.restoreField(".", "test")
+        assert not test_list2.restoreField(".", "test")
         assert len(test_list2) == 0
         callback.assert_not_called()
 
-        test_list2.restoreField(".0", "test")
+        assert not test_list2.restoreField(".0", "test")
         assert len(test_list2) == 0
         callback.assert_not_called()
 
         # Test indirect restore path.
 
         class TestBunch(Bunch):
             str_list = List(Key("default"))
 
         bunch = TestBunch()
         bunch.str_list.onUpdateCall(callback)
-        bunch.str_list.restoreField("str_list.1", "test")
+        assert bunch.str_list.restoreField("str_list.1", "test")
         assert len(bunch.str_list) == 1
         assert bunch.str_list[0].get() == "test"
         callback.assert_not_called()
 
         # Test an invalid restore value.
 
         test_list3 = List(Key("default"))
         test_list3.onUpdateCall(callback)
-        test_list3.restoreField(".size", "invalid")
+        assert not test_list3.restoreField(".size", "invalid")
         assert len(test_list3) == 0
         callback.assert_not_called()
 
         # Test restoring a List with empty items.
 
         test_list4 = List(Key("default"))
         test_list4.onUpdateCall(callback)
-        test_list4.restoreField(".1", None)
-        test_list4.restoreField(".2", "")
-        test_list4.restoreField(".3", None)
+        assert test_list4.restoreField(".1", None)
+        assert test_list4.restoreField(".2", "")
+        assert test_list4.restoreField(".3", None)
         assert len(test_list4) == 3
         assert not test_list4[0].isSet()
         assert test_list4[1].isSet() and test_list4[1].get() == ""
         assert not test_list4[2].isSet()
         callback.assert_not_called()
 
-    def test_persistence(self):
+    def test_persistence(self) -> None:
         # A List does not keep a reference to its parent or children.
 
         bunch_list: List[Key[int]] = List(Key(default=0))
         level1: List[Key[int]] = List(Key(default=0))
         level1.setParent(bunch_list)
         level2: List[Key[int]] = List(Key(default=0))
         level2.setParent(level1)
@@ -256,17 +256,28 @@
         assert len(list(level1.children())) == 1
 
         del bunch_list
         del level2
         assert level1.parent() is None
         assert len(list(level1.children())) == 0
 
+    def test_callback_type_is_flexible(self) -> None:
+        key_list = List(Key(""))
+
+        class Dummy:
+            pass
+
+        def callback(_: List[Key[str]]) -> Dummy:
+            return Dummy()
+
+        key_list.onUpdateCall(callback)
+
     def test_update_callback_called_on_list_contents_changed(
         self, mocker: MockerFixture
-    ):
+    ) -> None:
         callback = mocker.stub()
 
         key_list: List[Key[int]] = List(Key(default=0))
 
         key_list.onUpdateCall(callback)
 
         key_list.appendOne()
@@ -323,15 +334,15 @@
         assert len(key_list) > 1
         key_list.clear()
         callback.assert_called_once_with(key_list)
         callback.reset_mock()
 
     def test_update_callback_called_on_contained_item_update(
         self, mocker: MockerFixture
-    ):
+    ) -> None:
         callback = mocker.stub()
 
         bunch_list: List[ExampleBunch] = List(ExampleBunch())
         bunch_list.onUpdateCall(callback)
 
         bunch1 = ExampleBunch()
         bunch_list.append(bunch1)
@@ -379,15 +390,15 @@
         callback.assert_called_once_with(bunch8.test)
         callback.reset_mock()
         bunch9.test.set("test")
         callback.assert_called_once_with(bunch9.test)
 
     def test_update_callback_not_called_for_removed_items(
         self, mocker: MockerFixture
-    ):
+    ) -> None:
         bunch_list: List[ExampleBunch] = List(ExampleBunch())
 
         bunch1 = ExampleBunch()
         bunch2 = ExampleBunch()
 
         callback = mocker.stub()
         bunch_list.onUpdateCall(callback)
@@ -433,15 +444,15 @@
         bunch_list.remove(bunch1)
         assert bunch1 not in bunch_list
 
         callback.reset_mock()
         bunch1.test.set("test")
         callback.assert_not_called()
 
-    def test_label_set_on_contained_items(self):
+    def test_label_set_on_contained_items(self) -> None:
         # Testing List.appendOne()
 
         key_list = List(Key(""))
         key = key_list.appendOne()
         assert key.fieldLabel() == "1"
 
         # Testing List.insertOne()
@@ -498,15 +509,15 @@
 
         # Testing assignment order
 
         key_list[2], key_list[4] = key_list[4], key_list[2]
         assert key_list[2].fieldLabel() == "3"
         assert key_list[4].fieldLabel() == "5"
 
-    def test_label_unset_on_removed_items(self):
+    def test_label_unset_on_removed_items(self) -> None:
         key_list = List(Key(""))
         for _ in range(15):
             key_list.appendOne()
 
         # Test List.__delitem__(index)
 
         key = key_list[3]
@@ -544,15 +555,15 @@
 
         # Test List.clear()
 
         keys = key_list[:]
         key_list.clear()
         assert all(key.fieldLabel() == "" for key in keys)
 
-    def test_field_path(self):
+    def test_field_path(self) -> None:
         test_list1 = List(Key(""))
         assert test_list1.fieldPath() == "."
         test_list1.appendOne()
         test_list1.appendOne()
         assert test_list1[0].fieldPath() == ".1"
         assert test_list1[1].fieldPath() == ".2"
 
@@ -561,15 +572,15 @@
         test_list2.appendOne()
         test_list2.appendOne()
         assert test_list2[0].fieldPath() == ".1."
         assert test_list2[1].fieldPath() == ".2."
         assert test_list2[0].test.fieldPath() == ".1.test"
         assert test_list2[1].test.fieldPath() == ".2.test"
 
-    def test_repr(self):
+    def test_repr(self) -> None:
         parent = List(Key(default=0))
         list_iter_no_parent = List(Key(default=0), order=List.NO_PARENT)
         list_iter_parent_first = List(Key(default=0), order=List.PARENT_FIRST)
         list_iter_parent_last = List(Key(default=0), order=List.PARENT_LAST)
 
         list_iter_no_parent.setParent(parent)
         list_iter_parent_first.setParent(parent)
```

### Comparing `SunsetSettings-0.4.0/tests/test_registry.py` & `SunsetSettings-0.5.0/tests/test_registry.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import pytest
 
 from sunset import CallbackRegistry
 
 
 class TestCallbackRegistry:
-    def test_function(self):
-
+    def test_function(self) -> None:
         call_args: list[str] = []
 
         def test(value: str) -> None:
             call_args.append(value)
 
         reg: CallbackRegistry[str] = CallbackRegistry()
 
@@ -24,16 +23,15 @@
         assert call_args == ["added"]
 
         del test
         assert len(reg) == 0
         reg.callAll("not added either")
         assert call_args == ["added"]
 
-    def test_method(self):
-
+    def test_method(self) -> None:
         call_args: list[str] = []
 
         class Test:
             def test(self, value: str) -> None:
                 call_args.append(value)
 
         reg: CallbackRegistry[str] = CallbackRegistry()
@@ -50,53 +48,52 @@
         assert call_args == ["added"]
 
         del t
         assert len(reg) == 0
         reg.callAll("not added")
         assert call_args == ["added"]
 
-    def test_discard_function(self):
+    def test_discard_function(self) -> None:
         def test(_: int) -> None:
             pass
 
         reg: CallbackRegistry[int] = CallbackRegistry()
 
         reg.add(test)
         assert test in reg
         reg.discard(test)
         assert test not in reg
 
-    def test_discard_method(self):
+    def test_discard_method(self) -> None:
         class Test:
             def test(self, _: int) -> None:
                 pass
 
         t = Test()
 
         reg: CallbackRegistry[int] = CallbackRegistry()
 
         reg.add(t.test)
         assert t.test in reg
         reg.discard(t.test)
         assert t.test not in reg
 
-    def test_pop(self):
-        def test(_: bool):
+    def test_pop(self) -> None:
+        def test(_: bool) -> None:
             pass
 
         reg: CallbackRegistry[bool] = CallbackRegistry()
 
         reg.add(test)
         assert test in reg
         other = reg.pop()
         assert test not in reg
         assert other is test
 
-    def test_function_added_once(self):
-
+    def test_function_added_once(self) -> None:
         call_args: list[str] = []
 
         def test(value: str) -> None:
             call_args.append(value)
 
         reg: CallbackRegistry[str] = CallbackRegistry()
 
@@ -104,16 +101,15 @@
         assert len(reg) == 1
         reg.add(test)
         assert len(reg) == 1
 
         reg.callAll("once")
         assert call_args == ["once"]
 
-    def test_same_method_added_once(self):
-
+    def test_same_method_added_once(self) -> None:
         call_args: list[str] = []
 
         class Test:
             def test(self, value: str) -> None:
                 call_args.append(value)
 
         reg: CallbackRegistry[str] = CallbackRegistry()
@@ -124,42 +120,39 @@
         assert len(reg) == 1
         reg.add(t.test)
         assert len(reg) == 1
 
         reg.callAll("once")
         assert call_args == ["once"]
 
-    def test_non_hashable_element(self):
+    def test_non_hashable_element(self) -> None:
         class Test(list[int]):
             def __init__(self) -> None:
-
                 super().__init__()
 
                 self.value = 0
 
             def test(self, value: int) -> None:
                 self.value = value
 
         t = Test()
 
         with pytest.raises(TypeError):
-
             # Prove that type Test is not hashable.
 
             hash(t)
 
         reg: CallbackRegistry[int] = CallbackRegistry()
 
         reg.add(t.test)
         reg.callAll(42)
 
         assert t.value == 42
 
-    def test_different_method_added_twice(self):
-
+    def test_different_method_added_twice(self) -> None:
         call_args: list[str] = []
 
         class Test:
             def test(self, value: str) -> None:
                 call_args.append(value)
 
         reg: CallbackRegistry[str] = CallbackRegistry()
```

### Comparing `SunsetSettings-0.4.0/tests/test_serializers.py` & `SunsetSettings-0.5.0/tests/test_serializers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,97 @@
 from typing import Optional
 
 from sunset import serializers
 
 
 class ExampleSerializable:
     def __init__(self, value: str) -> None:
-
         self._value = value
 
     def toStr(self) -> str:
-
         return self._value
 
     @staticmethod
-    def fromStr(value: str) -> Optional["ExampleSerializable"]:
-
-        return ExampleSerializable(value)
-
-
-def test_serialize_int():
-
-    assert serializers.serialize(42) == "42"
-
-
-def test_serialize_str():
+    def fromStr(string: str) -> Optional["ExampleSerializable"]:
+        return ExampleSerializable(string)
 
-    assert serializers.serialize(" !! test !!") == " !! test !!"
 
+def test_serialize_int() -> None:
+    serializer = serializers.lookup(int)
+    assert serializer is not None
+    assert serializer.toStr(42) == "42"
 
-def test_serialize_bool():
 
-    assert serializers.serialize(True) == "true"
-    assert serializers.serialize(False) == "false"
+def test_serialize_str() -> None:
+    serializer = serializers.lookup(str)
+    assert serializer is not None
+    assert serializer.toStr(" !! test !!") == " !! test !!"
 
 
-def test_serialize_float():
+def test_serialize_bool() -> None:
+    serializer = serializers.lookup(bool)
+    assert serializer is not None
+    assert serializer.toStr(True) == "true"
+    assert serializer.toStr(False) == "false"
 
-    assert serializers.serialize(1.0) == "1.0"
-    assert serializers.serialize(2.34e-56) == "2.34e-56"
 
+def test_serialize_float() -> None:
+    serializer = serializers.lookup(float)
+    assert serializer is not None
+    assert serializer.toStr(1.0) == "1.0"
+    assert serializer.toStr(2.34e-56) == "2.34e-56"
 
-def test_serialize_serializable():
 
+def test_serialize_serializable() -> None:
     t = ExampleSerializable("serializable")
-    assert serializers.serialize(t) == "serializable"
+    serializer = serializers.lookup(type(t))
+    assert serializer is not None
+    assert serializer.toStr(t) == "serializable"
 
 
-def test_deserialize_str():
+def test_deserialize_str() -> None:
+    serializer = serializers.lookup(str)
+    assert serializer is not None
+    assert serializer.fromStr("test") == "test"
 
-    assert serializers.deserialize(str, "test") == "test"
 
+def test_deserialize_int() -> None:
+    serializer = serializers.lookup(int)
+    assert serializer is not None
+    assert serializer.fromStr("test") is None
+    assert serializer.fromStr("   -32 ") == -32
+    assert serializer.fromStr("00017") == 17
 
-def test_deserialize_int():
 
-    assert serializers.deserialize(int, "test") is None
-    assert serializers.deserialize(int, "   -32 ") == -32
-    assert serializers.deserialize(int, "00017") == 17
+def test_deserialize_float() -> None:
+    serializer = serializers.lookup(float)
+    assert serializer is not None
+    assert serializer.fromStr("test") is None
+    assert serializer.fromStr("   -32.10 ") == -32.1
+    assert serializer.fromStr("2.34e-56") == 2.34e-56
 
 
-def test_deserialize_float():
+def test_deserialize_bool() -> None:
+    serializer = serializers.lookup(bool)
+    assert serializer is not None
+    assert serializer.fromStr("YES")
+    assert serializer.fromStr("  1 ")
+    assert serializer.fromStr("true")
 
-    assert serializers.deserialize(float, "test") is None
-    assert serializers.deserialize(float, "   -32.10 ") == -32.1
-    assert serializers.deserialize(float, "2.34e-56") == 2.34e-56
+    assert not serializer.fromStr("NO")
+    assert not serializer.fromStr("  0 ")
+    assert not serializer.fromStr("false")
 
+    assert serializer.fromStr("garbage") is None
 
-def test_deserialize_bool():
 
-    assert serializers.deserialize(bool, "YES")
-    assert serializers.deserialize(bool, "  1 ")
-    assert serializers.deserialize(bool, "true")
-
-    assert not serializers.deserialize(bool, "NO")
-    assert not serializers.deserialize(bool, "  0 ")
-    assert not serializers.deserialize(bool, "false")
-
-    assert serializers.deserialize(bool, "garbage") is None
-
-
-def test_deserialize_serializable():
-
-    t = serializers.deserialize(ExampleSerializable, "this is a test")
+def test_deserialize_serializable() -> None:
+    serializer = serializers.lookup(ExampleSerializable)
+    assert serializer is not None
+    t = serializer.fromStr("this is a test")
     assert t is not None
     assert isinstance(t, ExampleSerializable)
     assert t.toStr() == "this is a test"
+
+
+def test_serializer_not_found() -> None:
+    assert serializers.lookup(object) is None
```

### Comparing `SunsetSettings-0.4.0/tests/test_settings.py` & `SunsetSettings-0.5.0/tests/test_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import io
 
 from pytest_mock import MockerFixture
 
 from sunset import Bunch, Key, List, Settings, normalize
 
 
-def test_normalize():
+def test_normalize() -> None:
     assert normalize("") == ""
     assert normalize("     ") == ""
     assert normalize("  A  B  ") == "ab"
     assert normalize("(a):?/b") == "ab"
     assert normalize("a-b_c") == "a-b_c"
 
 
@@ -23,15 +23,15 @@
     key_list = List(Key(default=""))
 
     a = Key(default="")
     b = Key(default="")
 
 
 class TestSettings:
-    def test_new_section(self):
+    def test_new_section(self) -> None:
         settings = ExampleSettings()
         assert settings.fieldPath() == "main/"
 
         section1 = settings.newSection(name="One level down")
         assert section1.fieldPath() == "main/oneleveldown/"
 
         section2 = settings.newSection(name="One level down too")
@@ -47,28 +47,28 @@
             name="Not anonymous itself but in a anonymous hierachy"
         )
         assert (
             anonymous2.fieldPath()
             == "main/?/notanonymousitselfbutinaanonymoushierachy/"
         )
 
-    def test_new_named_section(self):
+    def test_new_named_section(self) -> None:
         settings = ExampleSettings()
 
         assert len(list(settings.sections())) == 0
 
         section = settings.newSection(name="same name")
         assert len(list(settings.sections())) == 1
 
         othersection = settings.getOrCreateSection(name="same name")
         assert len(list(settings.sections())) == 1
 
         assert othersection is section
 
-    def test_field_path(self):
+    def test_field_path(self) -> None:
         settings = ExampleSettings()
 
         assert settings.fieldPath() == "main/"
         assert settings.a.fieldPath() == "main/a"
         assert settings.inner_bunch.fieldPath() == "main/inner_bunch."
         assert settings.inner_bunch.c.fieldPath() == "main/inner_bunch.c"
         settings.bunch_list.appendOne()
@@ -117,15 +117,15 @@
         assert settings.fieldPath() == "renamed/"
         assert settings.a.fieldPath() == "renamed/a"
 
         settings.setSectionName("")
         assert settings.fieldPath() == "main/"
         assert settings.a.fieldPath() == "main/a"
 
-    def test_dump_fields(self):
+    def test_dump_fields(self) -> None:
         # When no field is set, the name of the section should still be dumped.
 
         settings = ExampleSettings()
         assert list(settings.dumpFields()) == [
             ("main/", None),
         ]
 
@@ -217,110 +217,112 @@
         assert list(settings.dumpFields()) == [
             ("main/", None),
             ("main/aaa/", None),
             ("main/mm/", None),
             ("main/z/", None),
         ]
 
-    def test_restore_field(self, mocker: MockerFixture):
+    def test_restore_field(self, mocker: MockerFixture) -> None:
         callback = mocker.stub()
 
         # Test restorting a field. As well, restoring a field should not trigger
         # a callback.
 
         settings = ExampleSettings()
         settings.onUpdateCall(callback)
         assert settings.a.get() == ""
-        settings.restoreField("main/a", "test main a")
+        assert settings.restoreField("main/a", "test main a")
         assert settings.a.get() == "test main a"
         callback.assert_not_called()
 
         # Test restoring a field on an inner Bunch.
 
         assert settings.inner_bunch.c.get() == 0
-        settings.restoreField("main/inner_bunch.c", "123")
+        assert settings.restoreField("main/inner_bunch.c", "123")
         assert settings.inner_bunch.c.get() == 123
         callback.assert_not_called()
 
         # Test restoring a field on a subsection.
 
         assert settings.getSection("section1") is None
-        settings.restoreField("main/section1/a", "test section1 a")
+        assert settings.restoreField("main/section1/a", "test section1 a")
         section1 = settings.getSection("section1")
         assert section1 is not None
         assert section1.a.get() == "test section1 a"
         callback.assert_not_called()
 
-        settings.restoreField("main/section2/subsection/a", "test subsection a")
+        assert settings.restoreField(
+            "main/section2/subsection/a", "test subsection a"
+        )
         section2 = settings.getSection("section2")
         assert section2 is not None
         subsection = section2.getSection("subsection")
         assert subsection is not None
         assert subsection.a.get() == "test subsection a"
         callback.assert_not_called()
 
         # Test restoring fields on a renamed Settings.
 
         renamed_settings = ExampleSettings()
         renamed_settings.setSectionName("renamed")
         renamed_settings.onUpdateCall(callback)
-        renamed_settings.restoreField("renamed/a", "test renamed a")
+        assert renamed_settings.restoreField("renamed/a", "test renamed a")
         assert renamed_settings.a.get() == "test renamed a"
         callback.assert_not_called()
 
         assert renamed_settings.b.get() == ""
-        renamed_settings.restoreField("main/b", "test invalid b")
+        assert not renamed_settings.restoreField("main/b", "test invalid b")
         assert renamed_settings.b.get() == ""
         callback.assert_not_called()
 
         # Test restorting with an invalid path.
 
         other_settings = ExampleSettings()
         other_settings.onUpdateCall(callback)
         assert not other_settings.isSet()
-        other_settings.restoreField("invalid/a", "test invalid a")
+        assert not other_settings.restoreField("invalid/a", "test invalid a")
         assert not other_settings.isSet()
         callback.assert_not_called()
 
-        other_settings.restoreField("main/invalid", "test invalid a")
+        assert not other_settings.restoreField("main/invalid", "test invalid a")
         assert not other_settings.isSet()
         callback.assert_not_called()
 
-        other_settings.restoreField("invalid", "test invalid a")
+        assert not other_settings.restoreField("invalid", "test invalid a")
         assert not other_settings.isSet()
         callback.assert_not_called()
 
-        other_settings.restoreField("/a", "test invalid a")
+        assert not other_settings.restoreField("/a", "test invalid a")
         assert not other_settings.isSet()
         callback.assert_not_called()
 
-        other_settings.restoreField("a/invalid", "test invalid a")
+        assert not other_settings.restoreField("a/invalid", "test invalid a")
         assert not other_settings.isSet()
         callback.assert_not_called()
 
-        other_settings.restoreField("a", "test invalid a")
+        assert not other_settings.restoreField("a", "test invalid a")
         assert not other_settings.isSet()
         callback.assert_not_called()
 
-    def test_persistence(self):
+    def test_persistence(self) -> None:
         # Settings keep a reference to their sections, but not to their parent.
 
         settings = ExampleSettings()
         level1 = settings.newSection(name="level 1")
         level2 = level1.newSection(name="level 2")
 
         assert level1.parent() is not None
         assert len(list(level1.sections())) == 1
 
         del settings
         del level2
         assert level1.parent() is None
         assert len(list(level1.sections())) == 1
 
-    def test_save(self):
+    def test_save(self) -> None:
         settings = ExampleSettings()
         settings.a.set("a")
         settings.bunch_list.appendOne().c.set(100)
 
         section1 = settings.newSection(name="Level 1")
         section1.a.set("sub a")
         section1.b.set("sub b")
@@ -367,15 +369,15 @@
 inner_bunch.c = 200
 
 [otherlevel1]
 inner_bunch.d = false
 """
         )
 
-    def test_load(self, mocker: MockerFixture):
+    def test_load(self, mocker: MockerFixture) -> None:
         settings = ExampleSettings()
         callback = mocker.stub()
         settings.onUpdateCall(callback)
         settings.load(
             io.StringIO(
                 """\
 [main]
@@ -426,41 +428,41 @@
         level1_sections = {s.sectionName(): s for s in level1.sections()}
         assert len(level1_sections) == 1
         assert "level2" in level1_sections
         level2 = level1_sections["level2"]
 
         assert level2.inner_bunch.c.get() == 200
 
-    def test_load_invalid_no_section(self):
+    def test_load_invalid_no_section(self) -> None:
         settings = ExampleSettings()
         settings.load(
             io.StringIO(
                 """\
 a = no bunch header
 """
             )
         )
 
         assert settings.a.get() == ""
 
-    def test_load_invalid_repeated_key(self):
+    def test_load_invalid_repeated_key(self) -> None:
         settings = ExampleSettings()
         settings.load(
             io.StringIO(
                 """\
 [main]
 a = repeated key
 a = last value should be used
 """
             )
         )
 
         assert settings.a.get() == "last value should be used"
 
-    def test_load_invalid_repeated_section(self):
+    def test_load_invalid_repeated_section(self) -> None:
         settings = ExampleSettings()
         settings.load(
             io.StringIO(
                 """\
 [main]
 a = repeated bunch
 
@@ -471,15 +473,15 @@
         )
 
         assert (
             settings.a.get()
             == "bunch values will be merged, last takes precedence"
         )
 
-    def test_load_invalid_missing_main(self):
+    def test_load_invalid_missing_main(self) -> None:
         settings = ExampleSettings()
         settings.load(
             io.StringIO(
                 """\
 [level1]
 a = main bunch is implicitly created if needed
 """
@@ -488,15 +490,15 @@
 
         sections = list(settings.sections())
         assert len(sections) == 1
         assert (
             sections[0].a.get() == "main bunch is implicitly created if needed"
         )
 
-    def test_load_invalid_extra_section_separators(self):
+    def test_load_invalid_extra_section_separators(self) -> None:
         settings = ExampleSettings()
         settings.load(
             io.StringIO(
                 """\
 [main]
 [level1///level2]
 a = extra separators should be skipped
@@ -536,15 +538,15 @@
             )
         )
 
         sections = list(settings.sections())
         assert len(sections) == 1
         assert sections[0].a.get() == "extra separators should be skipped"
 
-    def test_load_invalid_bad_section_is_skipped(self):
+    def test_load_invalid_bad_section_is_skipped(self) -> None:
         settings = ExampleSettings()
         settings.load(
             io.StringIO(
                 """\
 [main]
 a = main
 
@@ -554,15 +556,15 @@
             )
         )
 
         sections = list(settings.sections())
         assert len(sections) == 0
         assert settings.a.get() == "main"
 
-    def test_load_invalid_similar_are_merged(self):
+    def test_load_invalid_similar_are_merged(self) -> None:
         settings = ExampleSettings()
         settings.load(
             io.StringIO(
                 """\
 [main]
 a = main
 
@@ -572,15 +574,15 @@
             )
         )
 
         sections = list(settings.sections())
         assert len(sections) == 0
         assert settings.a.get() == "merged"
 
-    def test_load_invalid_empty_section_is_skipped(self):
+    def test_load_invalid_empty_section_is_skipped(self) -> None:
         settings = ExampleSettings()
         settings.load(
             io.StringIO(
                 """\
 [main]
 a = main
 
@@ -590,15 +592,15 @@
             )
         )
 
         sections = list(settings.sections())
         assert len(sections) == 0
         assert settings.a.get() == "main"
 
-    def test_load_bad_key(self):
+    def test_load_bad_key(self) -> None:
         settings = ExampleSettings()
         settings.load(
             io.StringIO(
                 """\
 [main]
 = should be skipped
 """
@@ -675,26 +677,26 @@
 a.. = should be loaded
 """
             )
         )
 
         assert settings.a.get() == "should be loaded"
 
-    def test_load_sections_created_even_if_empty(self):
+    def test_load_sections_created_even_if_empty(self) -> None:
         settings = ExampleSettings()
         settings.load(
             io.StringIO(
                 """\
 [shouldexist]
 """
             )
         )
         assert settings.getSection("shouldexist") is not None
 
-    def test_load_renamed_settings(self):
+    def test_load_renamed_settings(self) -> None:
         settings = ExampleSettings()
         settings.setSectionName("renamed")
 
         settings.load(
             io.StringIO(
                 """\
 [renamed]
@@ -703,17 +705,18 @@
             )
         )
 
         assert settings.a.get() == "value"
 
     def test_autosave(self, mocker: MockerFixture) -> None:
         sentinel = object()
-        stub = mocker.patch("sunset.autosaver.AutoSaver", return_value=sentinel)
+        stub = mocker.Mock(return_value=sentinel)
 
         settings = ExampleSettings()
+        settings.setAutosaverClass(stub)
         ret = settings.autosave(
             "/tmp/test",
             save_delay=12,
         )
 
         assert ret is sentinel
 
@@ -721,15 +724,26 @@
             settings,
             "/tmp/test",
             save_delay=12,
             save_on_update=True,
             logger=None,
         )
 
-    def test_key_updated_notification(self, mocker: MockerFixture):
+    def test_callback_type_is_flexible(self) -> None:
+        settings = ExampleSettings()
+
+        class Dummy:
+            pass
+
+        def callback(_: ExampleSettings) -> Dummy:
+            return Dummy()
+
+        settings.onUpdateCall(callback)
+
+    def test_key_updated_notification(self, mocker: MockerFixture) -> None:
         callback = mocker.stub()
 
         settings = ExampleSettings()
         settings.onUpdateCall(callback)
 
         settings.a.set("test 1")
         callback.assert_called_once_with(settings.a)
@@ -763,28 +777,28 @@
         callback.assert_called_once_with(anonymous)
         callback.reset_mock()
 
         anonymoussection.a.set("test 5")
         callback.assert_called_once_with(anonymoussection.a)
         callback.reset_mock()
 
-    def test_name_unicity(self):
+    def test_name_unicity(self) -> None:
         class TestSettings(Settings):
             pass
 
         parent = TestSettings()
         sections = [parent.newSection() for _ in range(10)]
         for section in sections:
             section.setSectionName("test")
 
         assert len(list(parent.children())) == len(
             set(child.sectionName() for child in parent.children())
         )
 
-    def test_anonymous_name_not_unique(self):
+    def test_anonymous_name_not_unique(self) -> None:
         class TestSettings(Settings):
             pass
 
         parent = TestSettings()
         sections = [parent.newSection() for _ in range(10)]
         for section in sections:
             section.setSectionName("")
```

### Comparing `SunsetSettings-0.4.0/tests/test_timer.py` & `SunsetSettings-0.5.0/tests/test_timer.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 
 from pytest import MonkeyPatch
 
 from sunset import PersistentTimer
 
 
 class TestPersistentTimer:
-    def test_timer_no_delay(self, monkeypatch: MonkeyPatch):
-
+    def test_timer_no_delay(self, monkeypatch: MonkeyPatch) -> None:
         mock_cls = MagicMock(threading.Timer, autospec=True)
         mock = mock_cls.return_value
         monkeypatch.setattr(threading, "Timer", mock_cls)
 
         def test():
             pass
 
@@ -28,16 +27,15 @@
 
         assert timer._timer is None  # type: ignore
 
         timer.cancel()
 
         assert timer._timer is None  # type: ignore
 
-    def test_timer_with_delay(self, monkeypatch: MonkeyPatch):
-
+    def test_timer_with_delay(self, monkeypatch: MonkeyPatch) -> None:
         mock_cls = MagicMock(threading.Timer, autospec=True)
         mock = mock_cls.return_value
         monkeypatch.setattr(threading, "Timer", mock_cls)
 
         def test():
             pass
```

### Comparing `SunsetSettings-0.4.0/PKG-INFO` & `SunsetSettings-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SunsetSettings
-Version: 0.4.0
+Version: 0.5.0
 Summary: SunsetSettings: a type-safe, extensible settings system with inheritance.
 Author-email: "P. Varet" <p.varet@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -142,57 +142,61 @@
 >>> from sunset import Key
 
 >>> # Types can be inferred from the provided default value:
 >>> number_of_ponies = Key(default=0)
 >>> number_of_ponies
 <Key[int]:(0)>
 >>> number_of_ponies.set(6)  # Works!
+True
 >>> number_of_ponies.set("six")  # Type error!
+False
 >>> number_of_ponies.get()  # Value is unchanged.
 6
 >>> from typing import TYPE_CHECKING
 >>> if TYPE_CHECKING:
 ...     reveal_type(number_of_ponies.get())
 >>> # Revealed type is "builtins.int"
 
 ```
 
 
 ### Extensibility
 
-You can store arbitrary types in your SunsetSettings provided they implement a
-simple serialization protocol. (See [the API
-reference](https://sunsetsettings.rtfd.io/en/stable/api.html#sunset.Serializable).)
+You can store arbitrary types in your SunsetSettings provided that you also
+provide a serializer for that type. (See [the API
+reference](https://sunsetsettings.rtfd.io/en/stable/api.html#sunset.Serializer).)
 
 ```python
 >>> import re
 >>> from typing import Optional, TYPE_CHECKING
 
 >>> class Coordinates:
 ...     def __init__(self, x: int, y: int) -> None:
-...         self._x = x
-...         self._y = y
-...
-...     def toStr(self) -> str:
-...         return f"{self._x},{self._y}"
-...
-...     @classmethod
-...     def fromStr(cls, value: str) -> Optional["Coordinates"]:
-...         m = re.match(r"(\d+),(\d+)", value)
-...         if m is None:
+...         self.x = x
+...         self.y = y
+
+>>> class CoordinatesSerializer:
+...     def toStr(self, coord: Coordinates) -> str:
+...         return f"{coord.x},{coord.y}"
+...
+...     def fromStr(self, string: str) -> Optional[Coordinates]:
+...         x, y = string.split(",", 1)
+...         if not x.isdigit() or not y.isdigit():
 ...             return None
-...         x = int(m.group(1))
-...         y = int(m.group(2))
-...         return cls(x, y)
+...         return Coordinates(int(x), int(y))
 
 >>> from sunset import Key
->>> coordinates = Key(default=Coordinates(0, 0))
+>>> coordinates = Key(
+...     default=Coordinates(0, 0), serializer=CoordinatesSerializer()
+... )
 >>> if TYPE_CHECKING:
 ...     reveal_type(coordinates.get())
 >>> # Revealed type is "Coordinates"
+>>> print(repr(coordinates))
+<Key[Coordinates]:(0,0)>
 
 ```
 
 
 ### Inheritance
 
 SunsetSettings lets the user have a general set of settings that can be
@@ -207,14 +211,15 @@
 ...     limbs: Key[int] = Key(default=4)
 ... 
 >>> animals = Animals()
 >>> octopuses = animals.newSection(name="octopuses")
 >>> octopuses.limbs.get()
 4
 >>> octopuses.limbs.set(8)
+True
 >>> octopuses.limbs.get()
 8
 >>> animals.limbs.get()
 4
 >>> octopuses.limbs.clear()
 >>> octopuses.limbs.get()
 4
@@ -231,14 +236,15 @@
 
 >>> number_of_ponies = Key(default=0)
 >>> def callback(value):
 ...     print("Pony count updated:", value)
 >>> number_of_ponies.onValueChangeCall(callback)
 >>> number_of_ponies.set(6)
 Pony count updated: 6
+True
 
 ```
 
 
 ## Requirements
 
 - Python 3.9 or later.
```

