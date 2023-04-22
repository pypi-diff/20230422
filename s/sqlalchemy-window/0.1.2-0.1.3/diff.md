# Comparing `tmp/sqlalchemy_window-0.1.2.tar.gz` & `tmp/sqlalchemy_window-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/sqlalchemy-window/sqlalchemy-window/dist/.tmp-dpsuigmo/sqlalchemy_window-0.1.2.tar", last modified: Wed Mar 29 10:20:22 2023, max compression
+gzip compressed data, was "/home/runner/work/sqlalchemy-window/sqlalchemy-window/dist/.tmp-o6lgvj2s/sqlalchemy_window-0.1.3.tar", last modified: Sat Apr 22 09:24:07 2023, max compression
```

## Comparing `sqlalchemy_window-0.1.2.tar` & `sqlalchemy_window-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:20:22.000000 sqlalchemy_window-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-29 10:20:02.000000 sqlalchemy_window-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-03-29 10:20:22.000000 sqlalchemy_window-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-03-29 10:20:02.000000 sqlalchemy_window-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-03-29 10:20:02.000000 sqlalchemy_window-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 10:20:22.000000 sqlalchemy_window-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:20:22.000000 sqlalchemy_window-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:20:22.000000 sqlalchemy_window-0.1.2/src/sqlalchemy_window/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-03-29 10:20:02.000000 sqlalchemy_window-0.1.2/src/sqlalchemy_window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-03-29 10:20:02.000000 sqlalchemy_window-0.1.2/src/sqlalchemy_window/_over_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-03-29 10:20:02.000000 sqlalchemy_window-0.1.2/src/sqlalchemy_window/_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-03-29 10:20:02.000000 sqlalchemy_window-0.1.2/src/sqlalchemy_window/_window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:20:22.000000 sqlalchemy_window-0.1.2/src/sqlalchemy_window.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-03-29 10:20:22.000000 sqlalchemy_window-0.1.2/src/sqlalchemy_window.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-03-29 10:20:22.000000 sqlalchemy_window-0.1.2/src/sqlalchemy_window.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 10:20:22.000000 sqlalchemy_window-0.1.2/src/sqlalchemy_window.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-29 10:20:22.000000 sqlalchemy_window-0.1.2/src/sqlalchemy_window.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-29 10:20:22.000000 sqlalchemy_window-0.1.2/src/sqlalchemy_window.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:20:22.000000 sqlalchemy_window-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-03-29 10:20:02.000000 sqlalchemy_window-0.1.2/tests/test_over_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-03-29 10:20:02.000000 sqlalchemy_window-0.1.2/tests/test_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-03-29 10:20:02.000000 sqlalchemy_window-0.1.2/tests/test_window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:24:07.000000 sqlalchemy_window-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-22 09:23:46.000000 sqlalchemy_window-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-22 09:24:07.000000 sqlalchemy_window-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-22 09:23:46.000000 sqlalchemy_window-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-22 09:23:46.000000 sqlalchemy_window-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 09:24:07.000000 sqlalchemy_window-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:24:07.000000 sqlalchemy_window-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:24:07.000000 sqlalchemy_window-0.1.3/src/sqlalchemy_window/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-22 09:23:46.000000 sqlalchemy_window-0.1.3/src/sqlalchemy_window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-04-22 09:23:46.000000 sqlalchemy_window-0.1.3/src/sqlalchemy_window/_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-04-22 09:23:46.000000 sqlalchemy_window-0.1.3/src/sqlalchemy_window/_window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:24:07.000000 sqlalchemy_window-0.1.3/src/sqlalchemy_window.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-22 09:24:07.000000 sqlalchemy_window-0.1.3/src/sqlalchemy_window.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-22 09:24:07.000000 sqlalchemy_window-0.1.3/src/sqlalchemy_window.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 09:24:07.000000 sqlalchemy_window-0.1.3/src/sqlalchemy_window.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-22 09:24:07.000000 sqlalchemy_window-0.1.3/src/sqlalchemy_window.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-22 09:24:07.000000 sqlalchemy_window-0.1.3/src/sqlalchemy_window.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:24:07.000000 sqlalchemy_window-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-22 09:23:46.000000 sqlalchemy_window-0.1.3/tests/test_over_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-22 09:23:46.000000 sqlalchemy_window-0.1.3/tests/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-04-22 09:23:46.000000 sqlalchemy_window-0.1.3/tests/test_window.py
```

### Comparing `sqlalchemy_window-0.1.2/LICENSE` & `sqlalchemy_window-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_window-0.1.2/PKG-INFO` & `sqlalchemy_window-0.1.3/src/sqlalchemy_window.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sqlalchemy_window
-Version: 0.1.2
+Name: sqlalchemy-window
+Version: 0.1.3
 Summary: A SQLAlchemy plugin to add support for PostgreSQL WINDOW clause
 Author-email: Roman Necheporenko <roman@waterfountain.one>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -15,14 +15,17 @@
 
 A SQLAlchemy plugin to add support for PostgreSQL WINDOW clause.
 
 **NOTE**: only supports SQLAlchemy 2.0 and higher.
 
 ## Example
 
+Newer versions (>= 0.1.3) allow you to use `Window.over_self` interface
+for window functions:
+
 ```py
 import sqlalchemy as sa
 from sqlalchemy_window import over_window, select, window
 
 metadata = sa.MetaData()
 table = sa.Table(
   "prices",
@@ -31,21 +34,34 @@
   sa.Column("ts", sa.DateTime(timezone=True), primary_key=True),
   sa.Column("price", sa.Numeric, nullable=False),
 )
 
 w = window("w", partition_by=table.c["asset"], order_by=table.c["ts"], range_=(None, None))
 
 query = select(
+  w.over_self(sa.func.first_value(table.c["price"])).label("open"),
+  w.over_self(sa.func.max(table.c["price"])).label("high"),
+  w.over_self(sa.func.min(table.c["price"])).label("low"),
+  w.over_self(sa.func.last_value(table.c["price"])).label("close"),
+).where(sa.func.cast(table.c["ts"], sa.Date) == '2023-01-01').window(w)
+```
+
+Before that, to build above query you would use `over_window` factory:
+
+```py
+query = select(
   over_window(sa.func.first_value(table.c["price"]), w).label("open"),
   over_window(sa.func.max(table.c["price"]), w).label("high"),
   over_window(sa.func.min(table.c["price"]), w).label("low"),
   over_window(sa.func.last_value(table.c["price"]), w).label("close"),
 ).where(sa.func.cast(table.c["ts"], sa.Date) == '2023-01-01').window(w)
 ```
 
+You can still use `over_window` in newer versions.
+
 ## Development
 
 To setup a development environment run:
 
 ```bash
 python3 -m venv venv
 source ./venv/bin/activate
```

### Comparing `sqlalchemy_window-0.1.2/README.md` & `sqlalchemy_window-0.1.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 
 A SQLAlchemy plugin to add support for PostgreSQL WINDOW clause.
 
 **NOTE**: only supports SQLAlchemy 2.0 and higher.
 
 ## Example
 
+Newer versions (>= 0.1.3) allow you to use `Window.over_self` interface
+for window functions:
+
 ```py
 import sqlalchemy as sa
 from sqlalchemy_window import over_window, select, window
 
 metadata = sa.MetaData()
 table = sa.Table(
   "prices",
@@ -18,21 +21,34 @@
   sa.Column("ts", sa.DateTime(timezone=True), primary_key=True),
   sa.Column("price", sa.Numeric, nullable=False),
 )
 
 w = window("w", partition_by=table.c["asset"], order_by=table.c["ts"], range_=(None, None))
 
 query = select(
+  w.over_self(sa.func.first_value(table.c["price"])).label("open"),
+  w.over_self(sa.func.max(table.c["price"])).label("high"),
+  w.over_self(sa.func.min(table.c["price"])).label("low"),
+  w.over_self(sa.func.last_value(table.c["price"])).label("close"),
+).where(sa.func.cast(table.c["ts"], sa.Date) == '2023-01-01').window(w)
+```
+
+Before that, to build above query you would use `over_window` factory:
+
+```py
+query = select(
   over_window(sa.func.first_value(table.c["price"]), w).label("open"),
   over_window(sa.func.max(table.c["price"]), w).label("high"),
   over_window(sa.func.min(table.c["price"]), w).label("low"),
   over_window(sa.func.last_value(table.c["price"]), w).label("close"),
 ).where(sa.func.cast(table.c["ts"], sa.Date) == '2023-01-01').window(w)
 ```
 
+You can still use `over_window` in newer versions.
+
 ## Development
 
 To setup a development environment run:
 
 ```bash
 python3 -m venv venv
 source ./venv/bin/activate
```

### Comparing `sqlalchemy_window-0.1.2/pyproject.toml` & `sqlalchemy_window-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sqlalchemy_window-0.1.2/src/sqlalchemy_window/_select.py` & `sqlalchemy_window-0.1.3/src/sqlalchemy_window/_select.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_window-0.1.2/src/sqlalchemy_window/_window.py` & `sqlalchemy_window-0.1.3/src/sqlalchemy_window/_window.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 from sqlalchemy.exc import ArgumentError
 from sqlalchemy.ext.compiler import compiles
 from sqlalchemy.sql.compiler import SQLCompiler
 from sqlalchemy.sql.elements import RANGE_CURRENT
 from sqlalchemy.sql.elements import RANGE_UNBOUNDED
 from sqlalchemy.sql.elements import ClauseElement
 from sqlalchemy.sql.elements import ClauseList
+from sqlalchemy.sql.elements import ColumnElement
 from sqlalchemy.sql.elements import _OverRange
+from sqlalchemy.sql.functions import FunctionElement
 from sqlalchemy.sql.roles import ByOfRole
 
 if typing.TYPE_CHECKING:  # pragma: no cover
     from sqlalchemy.sql._typing import _ColumnExpressionArgument
 
 _ColumnExpression = typing.Union[
     "typing.Iterable[_ColumnExpressionArgument[typing.Any]]",
@@ -23,28 +25,67 @@
 _RangeArgument = typing.Union[
     range,
     typing.Tuple[typing.Optional[int], typing.Optional[int]],
 ]
 
 _RangeType = typing.Union[_OverRange, int]
 
+_FT = typing.TypeVar("_FT")
+
 
 class FrameExclude(enum.Enum):
     CURRENT_ROW = "CURRENT ROW"
     GROUP = "GROUP"
     TIES = "TIES"
     NO_OTHERS = "NO OTHERS"
 
 
 CURRENT_ROW = FrameExclude.CURRENT_ROW
 GROUP = FrameExclude.GROUP
 TIES = FrameExclude.TIES
 NO_OTHERS = FrameExclude.NO_OTHERS
 
 
+class OverWindow(ColumnElement[_FT]):
+    """Represent an `OVER` statement for window functions.
+
+    Do not construct directly, rather through a
+    `sqlalchemy_window.over_window` factory.
+    """
+
+    def __init__(self, element: FunctionElement[_FT], window: "Window") -> None:
+        self.element = element
+        self.window = window
+
+    @property
+    def type(self):
+        return self.element.type
+
+
+def over_window(element: FunctionElement[_FT], window: "Window") -> OverWindow[_FT]:
+    """Construct an `OverWindow` object.
+
+    Built-in `.over()` method on SQLAlchemy's window function can only
+    be used to specify an inline window clause. However if you want to
+    reuse one window in multiple places you can use this.
+
+    Example usage:
+
+    ```
+        w = window("w", ...)
+        over_window(func.first_value(literal_column("foo")), w)
+    ```
+
+    This roughly compiles to following SQL:
+
+        `first_value(foo) OVER w`
+    """
+    return OverWindow(element, window)
+
+
 class Window(ClauseElement):
     """Represent a WINDOW expression.
 
     This is a special construct to allow reuse of the same
     options for window function in multiple places.
 
     Do not use this element directly, rather through a
@@ -127,14 +168,18 @@
                 raise ArgumentError("int or None expected for range value") from e
             else:
                 return RANGE_CURRENT if b == 0 else b
 
         lower, upper = map(normalize_boundary, range_)
         return lower, upper
 
+    def over_self(self, element: FunctionElement[_FT]) -> OverWindow[_FT]:
+        """Construct an `OverWindow` object from a given function and self."""
+        return over_window(element, self)
+
 
 def window(
     name: str,
     existing_window: typing.Optional[Window] = None,
     partition_by: typing.Optional[_ColumnExpression] = None,
     order_by: typing.Optional[_ColumnExpression] = None,
     range_: typing.Optional[_RangeArgument] = None,
@@ -192,14 +237,19 @@
         range_=range_,
         rows=rows,
         groups=groups,
         exclude=exclude,
     )
 
 
+@compiles(OverWindow)
+def compile_over_window(element: OverWindow, compiler: SQLCompiler, **kwargs: typing.Any) -> str:
+    return "{} OVER {}".format(compiler.process(element.element), element.window.name)
+
+
 @compiles(Window, "postgresql")
 def compile_window(element: Window, compiler: SQLCompiler, **kwargs: typing.Any) -> str:
     def format_frame_clause(
         range_: typing.Tuple[typing.Union[typing.Any, int], typing.Union[typing.Any, int]]
     ) -> str:
         return "{} AND {}".format(
             "UNBOUNDED PRECEDING"
```

### Comparing `sqlalchemy_window-0.1.2/src/sqlalchemy_window.egg-info/PKG-INFO` & `sqlalchemy_window-0.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sqlalchemy-window
-Version: 0.1.2
+Name: sqlalchemy_window
+Version: 0.1.3
 Summary: A SQLAlchemy plugin to add support for PostgreSQL WINDOW clause
 Author-email: Roman Necheporenko <roman@waterfountain.one>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -15,14 +15,17 @@
 
 A SQLAlchemy plugin to add support for PostgreSQL WINDOW clause.
 
 **NOTE**: only supports SQLAlchemy 2.0 and higher.
 
 ## Example
 
+Newer versions (>= 0.1.3) allow you to use `Window.over_self` interface
+for window functions:
+
 ```py
 import sqlalchemy as sa
 from sqlalchemy_window import over_window, select, window
 
 metadata = sa.MetaData()
 table = sa.Table(
   "prices",
@@ -31,21 +34,34 @@
   sa.Column("ts", sa.DateTime(timezone=True), primary_key=True),
   sa.Column("price", sa.Numeric, nullable=False),
 )
 
 w = window("w", partition_by=table.c["asset"], order_by=table.c["ts"], range_=(None, None))
 
 query = select(
+  w.over_self(sa.func.first_value(table.c["price"])).label("open"),
+  w.over_self(sa.func.max(table.c["price"])).label("high"),
+  w.over_self(sa.func.min(table.c["price"])).label("low"),
+  w.over_self(sa.func.last_value(table.c["price"])).label("close"),
+).where(sa.func.cast(table.c["ts"], sa.Date) == '2023-01-01').window(w)
+```
+
+Before that, to build above query you would use `over_window` factory:
+
+```py
+query = select(
   over_window(sa.func.first_value(table.c["price"]), w).label("open"),
   over_window(sa.func.max(table.c["price"]), w).label("high"),
   over_window(sa.func.min(table.c["price"]), w).label("low"),
   over_window(sa.func.last_value(table.c["price"]), w).label("close"),
 ).where(sa.func.cast(table.c["ts"], sa.Date) == '2023-01-01').window(w)
 ```
 
+You can still use `over_window` in newer versions.
+
 ## Development
 
 To setup a development environment run:
 
 ```bash
 python3 -m venv venv
 source ./venv/bin/activate
```

### Comparing `sqlalchemy_window-0.1.2/tests/test_select.py` & `sqlalchemy_window-0.1.3/tests/test_select.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_window-0.1.2/tests/test_window.py` & `sqlalchemy_window-0.1.3/tests/test_window.py`

 * *Files identical despite different names*

