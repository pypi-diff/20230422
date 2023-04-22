# Comparing `tmp/tabeline-0.1.1.tar.gz` & `tmp/tabeline-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabeline-0.1.1.tar", max compression
+gzip compressed data, was "tabeline-0.2.0.tar", max compression
```

## Comparing `tabeline-0.1.1.tar` & `tabeline-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     1057 2022-05-27 00:58:00.822079 tabeline-0.1.1/LICENSE
--rw-r--r--   0        0        0     1704 2022-07-25 12:24:22.363354 tabeline-0.1.1/README.md
--rw-r--r--   0        0        0     1969 2022-07-25 12:24:22.411355 tabeline-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       88 2022-04-10 13:57:42.631712 tabeline-0.1.1/src/tabeline/__init__.py
--rw-r--r--   0        0        0    21963 2022-07-24 13:18:52.178267 tabeline-0.1.1/src/tabeline/_data_table.py
--rw-r--r--   0        0        0      360 2022-04-10 13:57:42.631712 tabeline-0.1.1/src/tabeline/_dummy.py
--rw-r--r--   0        0        0      241 2022-04-10 13:57:42.631712 tabeline-0.1.1/src/tabeline/_expression/__init__.py
--rw-r--r--   0        0        0     2450 2022-07-24 20:02:47.710297 tabeline-0.1.1/src/tabeline/_expression/_functions.py
--rw-r--r--   0        0        0     4313 2022-04-10 13:57:42.631712 tabeline-0.1.1/src/tabeline/_expression/_parser.py
--rw-r--r--   0        0        0     5363 2022-04-10 13:57:42.631712 tabeline-0.1.1/src/tabeline/_expression/_substitute.py
--rw-r--r--   0        0        0     3744 2022-04-10 13:57:42.631712 tabeline-0.1.1/src/tabeline/_expression/_to_polars.py
--rw-r--r--   0        0        0     2902 2022-04-10 13:57:42.631712 tabeline-0.1.1/src/tabeline/_expression/ast.py
--rw-r--r--   0        0        0      573 2022-04-10 13:57:42.635712 tabeline-0.1.1/src/tabeline/_result.py
--rw-r--r--   0        0        0      733 2022-04-12 00:13:33.013959 tabeline-0.1.1/src/tabeline/_validation.py
--rw-r--r--   0        0        0     1894 2022-07-02 10:56:43.292515 tabeline-0.1.1/src/tabeline/exceptions.py
--rw-r--r--   0        0        0      376 2022-04-10 13:57:42.631712 tabeline-0.1.1/src/tabeline/testing.py
--rw-r--r--   0        0        0     2681 1970-01-01 00:00:00.000000 tabeline-0.1.1/setup.py
--rw-r--r--   0        0        0     2824 1970-01-01 00:00:00.000000 tabeline-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1057 2022-05-27 00:58:00.822079 tabeline-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1709 2023-04-21 01:31:22.559414 tabeline-0.2.0/README.md
+-rw-r--r--   0        0        0     1966 2023-04-22 10:01:16.847548 tabeline-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       97 2023-04-21 02:03:52.594662 tabeline-0.2.0/src/tabeline/__init__.py
+-rw-r--r--   0        0        0    22663 2023-04-21 18:11:21.414724 tabeline-0.2.0/src/tabeline/_data_frame.py
+-rw-r--r--   0        0        0      365 2023-04-21 01:31:22.563413 tabeline-0.2.0/src/tabeline/_dummy.py
+-rw-r--r--   0        0        0      241 2022-04-10 13:57:42.631712 tabeline-0.2.0/src/tabeline/_expression/__init__.py
+-rw-r--r--   0        0        0     2450 2022-07-24 20:02:47.710297 tabeline-0.2.0/src/tabeline/_expression/_functions.py
+-rw-r--r--   0        0        0     4313 2022-04-10 13:57:42.631712 tabeline-0.2.0/src/tabeline/_expression/_parser.py
+-rw-r--r--   0        0        0     5363 2022-04-10 13:57:42.631712 tabeline-0.2.0/src/tabeline/_expression/_substitute.py
+-rw-r--r--   0        0        0     3744 2022-04-10 13:57:42.631712 tabeline-0.2.0/src/tabeline/_expression/_to_polars.py
+-rw-r--r--   0        0        0     2902 2022-04-10 13:57:42.631712 tabeline-0.2.0/src/tabeline/_expression/ast.py
+-rw-r--r--   0        0        0      573 2022-04-10 13:57:42.635712 tabeline-0.2.0/src/tabeline/_result.py
+-rw-r--r--   0        0        0      733 2022-04-12 00:13:33.013959 tabeline-0.2.0/src/tabeline/_validation.py
+-rw-r--r--   0        0        0     1918 2023-04-21 01:31:22.559414 tabeline-0.2.0/src/tabeline/exceptions.py
+-rw-r--r--   0        0        0      381 2023-04-21 01:31:22.559414 tabeline-0.2.0/src/tabeline/testing.py
+-rw-r--r--   0        0        0     2896 1970-01-01 00:00:00.000000 tabeline-0.2.0/PKG-INFO
```

### Comparing `tabeline-0.1.1/LICENSE` & `tabeline-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tabeline-0.1.1/README.md` & `tabeline-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Tabeline
 
-Tabeline is a data table and data grammar library. You write the expressions in strings and supply them to methods on the `DataTable` class. The  strings are parsed by Parsita and converted into Polars for execution.
+Tabeline is a data frame and data grammar library. You write the expressions in strings and supply them to methods on the `DataFrame` class. The  strings are parsed by Parsita and converted into Polars for execution.
 
-Tabeline draws inspiration from dplyr, the data grammar of R's tidyverse, especially for its methods names. The `filter`, `mutate`, `group`, and `summarize` methods should all feel familiar. But Tabeline is as proper a Python library as can be, using methods instead of pipes, like is standard in R. 
+Tabeline draws inspiration from dplyr, the data grammar of R's tidyverse, especially for its methods names. The `filter`, `mutate`, `group_by`, and `summarize` methods should all feel familiar. But Tabeline is as proper a Python library as can be, using methods instead of pipes, like is standard in R. 
 
 Tabeline uses Polars under the hood, but adds a lot of handling of edge cases from Polars, which otherwise result in crashes or behavior that is not type stable.
 
 See the [Documentation](https://tabeline.drhagen.com) for the full user guide.
 
 ## Installation
 
@@ -15,30 +15,30 @@
 ```shell
 pip install tabeline
 ```
 
 ## Motivating example
 
 ```python
-from tabeline import DataTable
+from tabeline import DataFrame
 
-# Construct a table using clean syntax
+# Construct a data frame using clean syntax
 # from_csv, from_pandas, and from_polars are also available 
-table = DataTable(
+df = DataFrame(
     id=[0, 0, 0, 0, 1, 1, 1, 1, 1],
     t=[0, 6, 12, 24, 0, 6, 12, 24, 48],
     y=[0, 2, 3, 1, 0, 4, 3, 2, 1],
 )
 
 # Use data grammar methods and string expressions to define
-# transformed data tables
+# transformed data frames
 analysis = (
-    table
+    df
     .filter("t <= 24")
-    .group("id")
+    .group_by("id")
     .summarize(auc="trapz(t, y)")
 )
 
 print(analysis)
 # shape: (2, 2)
 # ┌─────┬──────┐
 # │ id  ┆ auc  │
```

### Comparing `tabeline-0.1.1/pyproject.toml` & `tabeline-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 [tool.poetry]
 name = "tabeline"
-version = "0.1.1"
-description = "A data table and data grammar library"
+version = "0.2.0"
+description = "A data frame and data grammar library"
 authors = ["David Hagen <david@drhagen.com>"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://tabeline.drhagen.com"
 repository = "https://github.com/drhagen/tabeline"
-keywords = ["data", "table", "grammar", "dplyr"]
+keywords = ["dataframe", "datatable", "datagrammar", "dplyr"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Operating System :: OS Independent",
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
-polars = "^0.13.11"
+polars = "^0.17.5"
 parsita = "^1.7.0"
 typing_extensions = "^4.3.0"
-pandas = { version = "^1.4.3", optional = true}
-pyarrow = { version = "^8.0.0", optional = true}
+pandas = { version = "^1.4.3", optional = true }
+pyarrow = { version = "^11.0.0", optional = true }
 
 [tool.poetry.dev-dependencies]
-poetry = "1.2.0b2"
-nox_poetry = "^0.9.0"
+nox_poetry = "^1.0.2"
 
 # Converters
-pyarrow = "^8.0.0"
+pyarrow = "^11.0.0"
 pandas = "^1.4"
 
 # Test
 pytest = "^7.1.1"
 coverage = { version = "^6.3.2", extras = ["toml"] }
 pytest-cov = "^3.0.0"
```

### Comparing `tabeline-0.1.1/src/tabeline/_data_table.py` & `tabeline-0.2.0/src/tabeline/_data_frame.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
-__all__ = ["DataTable"]
+__all__ = ["DataFrame"]
 
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Literal, Optional, Sequence, Union
 
 import polars as pl
 
-from ._dummy import dummy_name, dummy_table
+from ._dummy import dummy_frame, dummy_name
 from ._expression import substitute, to_polars
 from ._expression.ast import Expression
 from ._validation import assert_legal_columns, missing
 from .exceptions import (
     GroupColumn,
     HasGroups,
     IndexOutOfRange,
@@ -23,15 +23,15 @@
 # Singleton indicating that the default value is to error
 error = object()
 
 if TYPE_CHECKING:
     import pandas as pd
 
 
-class DataTable:
+class DataFrame:
     def __init__(
         self,
         polars_df: pl.DataFrame = missing,
         group_levels: tuple[tuple[str, ...], ...] = (),
         height: Optional[int] = None,
         /,
         **columns,
@@ -46,19 +46,19 @@
             self._df = polars_df
             self.group_levels = group_levels
             if height is not None:
                 self.height = height
             else:
                 self.height = self._df.height  # With no height, height is taken from polars
         else:
-            raise TypeError("DataTable() takes 0 positional arguments but 1 was given")
+            raise TypeError("DataFrame() takes 0 positional arguments but 1 was given")
 
     @staticmethod
-    def columnless(*, height: int) -> DataTable:
-        return DataTable(pl.DataFrame({}), (), height)
+    def columnless(*, height: int) -> DataFrame:
+        return DataFrame(pl.DataFrame({}), (), height)
 
     @property
     def width(self) -> int:
         return self._df.width
 
     @property
     def shape(self) -> tuple[int, int]:
@@ -69,233 +69,240 @@
         return tuple(self._df.columns)
 
     @property
     def group_names(self) -> tuple[str, ...]:
         return tuple(names for level in self.group_levels for names in level)
 
     @staticmethod
-    def from_dict(columns: dict[str, list[Any]], /) -> DataTable:
+    def from_dict(columns: dict[str, list[Any]], /) -> DataFrame:
         df = pl.DataFrame(columns)
-        return DataTable(df)
+        return DataFrame(df)
 
     @staticmethod
-    def from_pandas(df: pd.DataFrame) -> DataTable:
+    def from_pandas(df: pd.DataFrame) -> DataFrame:
         if df.shape[1] == 0:
-            # Polars does not understand columnless tables
-            return DataTable.columnless(height=df.shape[0])
+            # Polars does not understand columnless data frames
+            return DataFrame.columnless(height=df.shape[0])
 
-        return DataTable(pl.from_pandas(df))
+        return DataFrame(pl.from_pandas(df))
 
     def to_pandas(self) -> pd.DataFrame:
         import numpy as np
         import pandas as pd
 
         if len(self.group_levels) != 0:
             raise HasGroups()
 
         if self.width == 0:
-            # Polars does not understand columnless tables
+            # Polars does not understand columnless data frames
             return pd.DataFrame(np.empty((self.height, 0)))
 
         return self._df.to_pandas()
 
     @staticmethod
-    def from_polars(df: pl.DataFrame) -> DataTable:
-        return DataTable(df)
+    def from_polars(df: pl.DataFrame) -> DataFrame:
+        return DataFrame(df)
 
     def to_polars(self) -> pl.DataFrame:
         if len(self.group_levels) != 0:
             raise HasGroups()
 
         return self._df
 
     @staticmethod
-    def read_csv(path: Path) -> DataTable:
+    def read_csv(path: Path) -> DataFrame:
         df = pl.read_csv(str(path))
-        return DataTable(df)
+        return DataFrame(df)
 
     def write_csv(self, path: Path) -> None:
         if len(self.group_levels) != 0:
             raise HasGroups()
 
         self._df.write_csv(str(path))
 
-    def slice0(self, indexes: list[int], /) -> DataTable:
+    def slice0(self, indexes: list[int], /) -> DataFrame:
         # Negative indexes are not supported by Polars, so they are not
         # supported in Tabeline.
         if self.width == 0:
             for index in indexes:
                 if index >= self.height or index < 0:
                     raise IndexOutOfRange(index, self.height)
-            return DataTable(self._df, self.group_levels, len(indexes))
+            return DataFrame(self._df, self.group_levels, len(indexes))
         else:
             group_names = self.group_names
             if len(group_names) == 0:
                 # Polars chokes on empty groups
-                return DataTable(self._df.select(pl.all().take(indexes)), self.group_levels)
+                return DataFrame(self._df.select(pl.all().take(indexes)), self.group_levels)
             else:
                 # There is no easy way to slice by groups in Polars. Using
                 # `take` on a group causes the sliced columns to be a column of
                 # lists that must be exploded at the end. The exploding results
                 # in clustering, so getting back the original row order requires
                 # tagging each row with an index and sorting the result by that.
                 # https://stackoverflow.com/q/71373783/
                 group_set = set(self.group_names)
                 non_group_columns = [
                     column for column in self.column_names if column not in group_set
                 ] + ["_index"]
 
-                if len(indexes) == 1:
+                if len(indexes) == 0:
+                    # Polars is not type stable when exploding no elements on a
+                    # grouped data frame, so just drop all rows.
+                    # https://github.com/pola-rs/polars/issues/6723
+                    new_df = self._df.select(pl.all().take(indexes))
+                elif len(indexes) == 1:
                     # Polars is not type stable, so explode must be excluded
                     # when taking only one element
                     new_df = (
                         self._df.lazy()
-                        .with_column(pl.arange(0, pl.count()).alias("_index"))
+                        .with_columns(pl.arange(0, pl.count()).alias("_index"))
                         .groupby(list(group_names), maintain_order=True)
                         .agg(pl.all().take(indexes))
                         .sort("_index")
                         .drop("_index")
                         .collect()
                     )
                 else:
                     new_df = (
                         self._df.lazy()
-                        .with_column(pl.arange(0, pl.count()).alias("_index"))
+                        .with_columns(pl.arange(0, pl.count()).alias("_index"))
                         .groupby(list(group_names), maintain_order=True)
                         .agg(pl.all().take(indexes))
                         .explode(non_group_columns)
                         .sort("_index")
                         .drop("_index")
                         .collect()
                     )
 
-                return DataTable(new_df, self.group_levels)
+                return DataFrame(new_df, self.group_levels)
 
-    def slice1(self, indexes: list[int], /) -> DataTable:
+    def slice1(self, indexes: list[int], /) -> DataFrame:
         return self.slice0([index - 1 for index in indexes])
 
-    def filter(self, predicate: str, /) -> DataTable:
+    def filter(self, predicate: str, /) -> DataFrame:
         expression = to_polars(Expression.parse(predicate).or_die())
 
         if self.width == 0:
-            # There is no way to evaluate an expression outside a datatable, so
-            # make a dummy table with the right number of rows.
+            # There is no way to evaluate an expression outside a data frame, so
+            # make a dummy data frame with the right number of rows.
             # eager=True needed because lazy expressions are not allowed in
             # the constructor
             # https://github.com/pola-rs/polars/issues/2983
-            height = dummy_table(self.height).filter(expression).height
-            return DataTable(pl.DataFrame({}), self.group_levels, height)
+            height = dummy_frame(self.height).filter(expression).height
+            return DataFrame(pl.DataFrame({}), self.group_levels, height)
         else:
             flat_groups = list(self.group_names)
             if len(flat_groups) > 0 and self.height > 0:
                 windowed_expression = expression.over(flat_groups)
             else:
                 # Polars chokes on an empty window
-                # Polars chokes on window over rowless table
+                # Polars chokes on window over rowless data frame
                 windowed_expression = expression
 
-            return DataTable(self._df.filter(windowed_expression), self.group_levels)
+            return DataFrame(self._df.filter(windowed_expression), self.group_levels)
 
-    def distinct(self, *columns: str) -> DataTable:
+    def distinct(self, *columns: str) -> DataFrame:
         assert_legal_columns(columns, self.column_names)
 
         # Polars chokes on duplicate columns
         group_set = set(self.group_names)
         unmentioned_columns = tuple(column for column in columns if column not in group_set)
         all_columns = list(self.group_names + unmentioned_columns)
         if len(all_columns) == 0:
             if self.height == 0:
                 # Polars chokes on an empty distinct subset
                 return self
             else:
-                return DataTable(self._df.head(1), self.group_levels, 1)
+                return DataFrame(self._df.head(1), self.group_levels, 1)
         else:
-            return DataTable(self._df.distinct(subset=all_columns), self.group_levels)
+            return DataFrame(
+                self._df.unique(subset=all_columns, maintain_order=True), self.group_levels
+            )
 
-    def unique(self) -> DataTable:
+    def unique(self) -> DataFrame:
         if self.width == 0:
-            return DataTable(pl.DataFrame({}), self.group_levels, min(1, self.height))
+            return DataFrame(pl.DataFrame({}), self.group_levels, min(1, self.height))
 
-        return DataTable(self._df.distinct(), self.group_levels)
+        return DataFrame(self._df.unique(maintain_order=True), self.group_levels)
 
-    def cluster(self, *columns: str) -> DataTable:
+    def cluster(self, *columns: str) -> DataFrame:
         assert_legal_columns(columns, self.column_names, self.group_names)
 
         flat_groups = self.group_names
 
         all_columns = list(self.group_names + columns)
 
         if len(all_columns) == 0:
             # Polars chokes on empty window columns
             return self
 
         if len(flat_groups) == 0:
             # Polars chokes on empty window columns
-            return DataTable(
+            return DataFrame(
                 self._df.lazy()
-                .with_column(pl.arange(0, pl.count()).alias("_index"))
-                .with_column(pl.min("_index").over(all_columns))
+                .with_columns(pl.arange(0, pl.count()).alias("_index"))
+                .with_columns(pl.min("_index").over(all_columns))
                 .select(pl.all().sort_by(["_index"]))
                 .drop("_index")
                 .collect(),
                 self.group_levels,
                 self.height,
             )
         else:
-            return DataTable(
+            return DataFrame(
                 self._df.lazy()
-                .with_column(pl.arange(0, pl.count()).alias("_index"))
-                .with_column(pl.min("_index").over(all_columns))
+                .with_columns(pl.arange(0, pl.count()).alias("_index"))
+                .with_columns(pl.min("_index").over(all_columns))
                 .select(pl.all().sort_by(["_index"]).over(list(self.group_names)))
                 .drop("_index")
                 .collect(),
                 self.group_levels,
                 self.height,
             )
 
-    def sort(self, *columns: str) -> DataTable:
+    def sort(self, *columns: str) -> DataFrame:
         assert_legal_columns(columns, self.column_names, self.group_names)
 
         flat_groups = self.group_names
         if len(flat_groups) == 0 or self.height == 0:
             # Polars chokes on empty groups
             # Polars chokes on windowing over empty rows
-            return DataTable(self._df.sort(list(columns)), self.group_levels, self.height)
+            return DataFrame(self._df.sort(list(columns)), self.group_levels, self.height)
         else:
-            return DataTable(
+            return DataFrame(
                 self._df.select(pl.all().sort_by(list(columns)).over(list(flat_groups))),
                 self.group_levels,
                 self.height,
             )
 
-    def select(self, *columns: str) -> DataTable:
+    def select(self, *columns: str) -> DataFrame:
         assert_legal_columns(columns, self.column_names)
 
         # Group columns cannot be deselected. Prepend any group columns that
         # were not explicitly selected so that group columns can be reordered
         # by select, but not lost. Unmentioned group columns are retained in
         # their original order.
         select_set = set(columns)
         group_set = set(self.group_names)
         unmentioned_groups = tuple(
             column
             for column in self.column_names
             if column in group_set and column not in select_set
         )
 
-        return DataTable(
+        return DataFrame(
             self._df.select(unmentioned_groups + columns), self.group_levels, self.height
         )
 
-    def deselect(self, *columns: str) -> DataTable:
+    def deselect(self, *columns: str) -> DataFrame:
         assert_legal_columns(columns, self.column_names, self.group_names)
 
-        return DataTable(self._df.drop(list(columns)), self.group_levels, self.height)
+        return DataFrame(self._df.drop(list(columns)), self.group_levels, self.height)
 
-    def rename(self, **names: str) -> DataTable:
+    def rename(self, **names: str) -> DataFrame:
         # Renames are processed simultaneously. Overwriting an existing column
         # is not permitted with this operation. Temporary column names may not
         # be used; columns to be swapped should simply be swapped. Renaming a
         # group column is legal.
         # Note that in dplyr, the order is new_name=old_name and in polars
         # old_name=new_name.
         # Sometime in the 0.13.x series, Polars switched from sequential to
@@ -318,82 +325,87 @@
         rename_map = {old: new for new, old in names.items()}
 
         groups = tuple(
             tuple(rename_map.get(column, column) for column in level)
             for level in self.group_levels
         )
 
-        return DataTable(self._df.rename(rename_map), groups, self.height)
+        return DataFrame(self._df.rename(rename_map), groups, self.height)
 
-    def mutate(self, **mutators: str) -> DataTable:
+    def mutate(self, **mutators: str) -> DataFrame:
         group_set = set(self.group_names)
         for column in mutators.keys():
             if column in group_set:
                 raise GroupColumn(column)
 
         if self.width == 0:
-            df = dummy_table(self.height)
+            df = dummy_frame(self.height)
         else:
             df = self._df
 
         # Both mutate and transmute must compute each column individually
         # because a column may refer to previous columns, which is not allowed
         # in a select context in polars:
         # https://stackoverflow.com/q/71105136/
         polars_operation = df.lazy()
         if len(group_set) == 0:
             for name, mutator in mutators.items():
-                polars_operation = polars_operation.with_column(
+                polars_operation = polars_operation.with_columns(
                     to_polars(Expression.parse(mutator).or_die()).alias(name)
                 )
         else:
             for name, mutator in mutators.items():
-                polars_operation = polars_operation.with_column(
+                polars_operation = polars_operation.with_columns(
                     to_polars(Expression.parse(mutator).or_die())
                     .over(list(self.group_names))
                     .alias(name)
                 )
 
         if self.width == 0:
             polars_operation = polars_operation.drop(dummy_name)
 
-        return DataTable(polars_operation.collect(), self.group_levels, self.height)
+        return DataFrame(polars_operation.collect(), self.group_levels, self.height)
 
-    def transmute(self, **mutators: str) -> DataTable:
-        mutated_table = self.mutate(**mutators)
+    def transmute(self, **mutators: str) -> DataFrame:
+        mutated_df = self.mutate(**mutators)
 
         # Keep group columns and explicitly mentioned columns, all in the order
         # of group columns followed by explicit columns
-        return mutated_table.select(*self.group_names, *mutators.keys())
+        return mutated_df.select(*self.group_names, *mutators.keys())
 
-    def group(
+    def group_by(
         self, *columns: str, order: Literal["original", "cluster", "sort"] = "original"
-    ) -> DataTable:
+    ) -> DataFrame:
         assert_legal_columns(columns, self.column_names, self.group_names)
 
         if order == "original":
-            ordered_table = self
+            ordered_df = self
         elif order == "cluster":
-            ordered_table = self.cluster(*columns)
+            ordered_df = self.cluster(*columns)
         elif order == "sort":
-            ordered_table = self.sort(*columns)
+            ordered_df = self.sort(*columns)
         else:
             raise TypeError(
                 f"For order, expected 'original', 'cluster', or 'sort', but got {order!r}"
             )
 
-        return DataTable(ordered_table._df, self.group_levels + (columns,), self.height)
+        return DataFrame(ordered_df._df, self.group_levels + (columns,), self.height)
+
+    def group(
+        self, *columns: str, order: Literal["original", "cluster", "sort"] = "original"
+    ) -> DataFrame:
+        return self.group_by(*columns, order=order)
 
-    def ungroup(self) -> DataTable:
+    def ungroup(self) -> DataFrame:
         if len(self.group_levels) == 0:
             raise NoGroups()
         else:
-            return DataTable(self._df, self.group_levels[:-1], self.height)
+            return DataFrame(self._df, self.group_levels[:-1], self.height)
 
-    def summarize(self, **reducers: str) -> DataTable:
+    def summarize(self, **reducers: str) -> DataFrame:
         if len(self.group_levels) == 0:
             raise NoGroups()
 
         # There is no way to sequentially evaluate expressions in a groupby
         # context, so each reducer must be substituted into subsequent reducers:
         # https://stackoverflow.com/q/71120396/
         substituted_reducers = {}
@@ -408,43 +420,43 @@
 
         if len(polars_expressions) == 0:
             # Polars chokes on empty agg. This is equivalent to dropping
             # everything but the group columns and then running distinct.
             return self.select().distinct().ungroup()
         else:
             if self.width == 0:
-                df = dummy_table(self.height)
+                df = dummy_frame(self.height)
             else:
                 df = self._df
 
             summarized = df.groupby(list(self.group_names), maintain_order=True).agg(
                 polars_expressions
             )
 
-            return DataTable(summarized, self.group_levels[:-1])
+            return DataFrame(summarized, self.group_levels[:-1])
 
-    def spread(self, key: str, value: str, *, fill: Any = error) -> DataTable:
+    def spread(self, key: str, value: str, *, fill: Any = error) -> DataFrame:
         if len(self.group_levels) == 0:
             raise NoGroups()
 
         assert_legal_columns([key, value], self.column_names, self.group_names)
 
         df = self._df.pivot(index=list(self.group_names), columns=key, values=value)
 
-        return DataTable(df, self.group_levels[:-1])
+        return DataFrame(df, self.group_levels[:-1])
 
-    def gather(self, key: str, value: str, *columns: str) -> DataTable:
+    def gather(self, key: str, value: str, *columns: str) -> DataFrame:
         column_set = set(columns)
         all_columns = [column for column in self.column_names if column not in column_set]
 
         df = self._df.melt(
             id_vars=all_columns, value_vars=list(columns), variable_name=key, value_name=value
         )
 
-        return DataTable(df, self.group_levels).group(key)
+        return DataFrame(df, self.group_levels).group_by(key)
 
     def _resolve_join_by(
         self,
         by: Optional[Sequence[Union[str, tuple[str, str]]]],
         right_column_names: Sequence[str],
     ) -> tuple[Optional[list[str]], Optional[list[str]]]:
         if by is not None:
@@ -470,123 +482,129 @@
             left_key_columns = common_columns
             right_key_columns = common_columns
 
         return left_key_columns, right_key_columns
 
     def inner_join(
         self,
-        other: DataTable,
+        other: DataFrame,
         /,
         *,
         by: Optional[Sequence[Union[str, tuple[str, str]]]] = None,
-    ) -> DataTable:
+    ) -> DataFrame:
         if len(self.group_levels) != 0 or len(other.group_levels) != 0:
-            raise NotImplementedError("Joins using grouped tables is not currently implemented")
+            raise NotImplementedError(
+                "Joins using grouped data frames is not currently implemented"
+            )
 
         left_key_columns, right_key_columns = self._resolve_join_by(by, other.column_names)
 
         joined_df = (
             # Polars does not order the output, so sort by original orders
             self._df.lazy()
-            .with_column(pl.arange(0, pl.count()).alias("_index1"))
+            .with_columns(pl.arange(0, pl.count()).alias("_index1"))
             .join(
-                other._df.lazy().with_column(pl.arange(0, pl.count()).alias("_index2")),
+                other._df.lazy().with_columns(pl.arange(0, pl.count()).alias("_index2")),
                 left_on=left_key_columns,
                 right_on=right_key_columns,
                 how="inner",
             )
             .sort(["_index1", "_index2"])
             .drop(["_index1", "_index2"])
             .collect()
         )
 
-        return DataTable(joined_df)
+        return DataFrame(joined_df)
 
     def left_join(
         self,
-        other: DataTable,
+        other: DataFrame,
         /,
         *,
         by: Optional[Sequence[Union[str, tuple[str, str]]]] = None,
-    ) -> DataTable:
+    ) -> DataFrame:
         if len(self.group_levels) != 0 or len(other.group_levels) != 0:
-            raise NotImplementedError("Joins using grouped tables is not currently implemented")
+            raise NotImplementedError(
+                "Joins using grouped data frames is not currently implemented"
+            )
 
         left_key_columns, right_key_columns = self._resolve_join_by(by, other.column_names)
 
         joined_df = (
             # Polars does not order the output, so sort by original orders
             self._df.lazy()
-            .with_column(pl.arange(0, pl.count()).alias("_index1"))
+            .with_columns(pl.arange(0, pl.count()).alias("_index1"))
             .join(
-                other._df.lazy().with_column(pl.arange(0, pl.count()).alias("_index2")),
+                other._df.lazy().with_columns(pl.arange(0, pl.count()).alias("_index2")),
                 left_on=left_key_columns,
                 right_on=right_key_columns,
                 how="left",
             )
             .sort(["_index1", "_index2"])
             .drop(["_index1", "_index2"])
             .collect()
         )
-        return DataTable(
+        return DataFrame(
             joined_df,
         )
 
     def outer_join(
         self,
-        other: DataTable,
+        other: DataFrame,
         /,
         *,
         by: Optional[Sequence[Union[str, tuple[str, str]]]] = None,
-    ) -> DataTable:
+    ) -> DataFrame:
         if len(self.group_levels) != 0 or len(other.group_levels) != 0:
-            raise NotImplementedError("Joins using grouped tables is not currently implemented")
+            raise NotImplementedError(
+                "Joins using grouped data frames is not currently implemented"
+            )
 
         left_key_columns, right_key_columns = self._resolve_join_by(by, other.column_names)
 
         joined_df = (
             # Polars does not order the output, so sort by original orders
             self._df.lazy()
-            .with_column(pl.arange(0, pl.count()).alias("_index1"))
+            .with_columns(pl.arange(0, pl.count()).alias("_index1"))
             .join(
-                other._df.lazy().with_column(pl.arange(0, pl.count()).alias("_index2")),
+                other._df.lazy().with_columns(pl.arange(0, pl.count()).alias("_index2")),
                 left_on=left_key_columns,
                 right_on=right_key_columns,
                 how="outer",
             )
             .sort(["_index1", "_index2"])
             .drop(["_index1", "_index2"])
             .collect()
         )
-        return DataTable(
+        return DataFrame(
             joined_df,
         )
 
     def __eq__(self, other):
-        if isinstance(other, DataTable):
+        if isinstance(other, DataFrame):
             if self.group_levels != other.group_levels:
                 return False
 
             if self.width == 0:
-                # Polars does not understand columnless tables
+                # Polars does not understand columnless data frames
                 return self.height == other.height
 
             if self.height == 0:
                 # Empty columns with different types are not equal in Polars,
                 # but are in Tabeline.
                 return self.column_names == other.column_names
 
             return self._df.frame_equal(other._df)
 
         return NotImplemented
 
     def __repr__(self):
         column_strs = [f"{name} = {list(values)!r}" for name, values in self._df.to_dict().items()]
-        group_strs = [f".group({', '.join(map(repr, level))})" for level in self.group_levels]
-        return f"DataTable({', '.join(column_strs)}){''.join(group_strs)}"
+        group_strs = [f".group_by({', '.join(map(repr, level))})" for level in self.group_levels]
+        return f"DataFrame({', '.join(column_strs)}){''.join(group_strs)}"
 
     def __str__(self):
         if len(self.group_levels) == 0:
             return str(self._df)
         else:
             groups_str = ",".join("[" + ",".join(level) + "]" for level in self.group_levels)
             return f"group levels: {groups_str}\n{self._df}"
```

### Comparing `tabeline-0.1.1/src/tabeline/_expression/_functions.py` & `tabeline-0.2.0/src/tabeline/_expression/_functions.py`

 * *Files identical despite different names*

### Comparing `tabeline-0.1.1/src/tabeline/_expression/_parser.py` & `tabeline-0.2.0/src/tabeline/_expression/_parser.py`

 * *Files identical despite different names*

### Comparing `tabeline-0.1.1/src/tabeline/_expression/_substitute.py` & `tabeline-0.2.0/src/tabeline/_expression/_substitute.py`

 * *Files identical despite different names*

### Comparing `tabeline-0.1.1/src/tabeline/_expression/_to_polars.py` & `tabeline-0.2.0/src/tabeline/_expression/_to_polars.py`

 * *Files identical despite different names*

### Comparing `tabeline-0.1.1/src/tabeline/_expression/ast.py` & `tabeline-0.2.0/src/tabeline/_expression/ast.py`

 * *Files identical despite different names*

### Comparing `tabeline-0.1.1/src/tabeline/_result.py` & `tabeline-0.2.0/src/tabeline/_result.py`

 * *Files identical despite different names*

### Comparing `tabeline-0.1.1/src/tabeline/_validation.py` & `tabeline-0.2.0/src/tabeline/_validation.py`

 * *Files identical despite different names*

### Comparing `tabeline-0.1.1/src/tabeline/exceptions.py` & `tabeline-0.2.0/src/tabeline/exceptions.py`

 * *Files 17% similar despite different names*

```diff
@@ -31,36 +31,36 @@
             f"Cannot rename {self.old_column} to {self.new_column} because"
             f" {self.new_column} already exists"
         )
 
 
 class HasGroups(TabelineException):
     def __str__(self) -> str:
-        return "Cannot perform this operation on a table with any group levels"
+        return "Cannot perform this operation on a data frame with any group levels"
 
 
 class NoGroups(TabelineException):
     def __str__(self) -> str:
-        return "Cannot perform this operation on a table with no group levels"
+        return "Cannot perform this operation on a data frame with no group levels"
 
 
 class GroupColumn(TabelineException):
     def __init__(self, column: str):
         super().__init__(column)
         self.column = column
 
     def __str__(self) -> str:
         return f"Cannot perform this operation on group column {self.column}"
 
 
-class RowlessTable(TabelineException):
+class RowlessDataFrame(TabelineException):
     def __str__(self) -> str:
-        return "Cannot perform this operation on a table with no rows"
+        return "Cannot perform this operation on a data frame with no rows"
 
 
 class IndexOutOfRange(TabelineException):
     def __init__(self, index: int, length: int):
         self.index = index
         self.length = length
 
     def __str__(self) -> str:
-        return f"Cannot index element {self.index} from table with {self.length} rows"
+        return f"Cannot index element {self.index} from data frame with {self.length} rows"
```

### Comparing `tabeline-0.1.1/PKG-INFO` & `tabeline-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 Metadata-Version: 2.1
 Name: tabeline
-Version: 0.1.1
-Summary: A data table and data grammar library
+Version: 0.2.0
+Summary: A data frame and data grammar library
 Home-page: https://github.com/drhagen/tabeline
 License: MIT
-Keywords: data,table,grammar,dplyr
+Keywords: dataframe,datatable,datagrammar,dplyr
 Author: David Hagen
 Author-email: david@drhagen.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: pandas
-Requires-Dist: pandas (>=1.4.3,<2.0.0); extra == "pandas"
+Requires-Dist: pandas (>=1.4.3,<2.0.0) ; extra == "pandas"
 Requires-Dist: parsita (>=1.7.0,<2.0.0)
-Requires-Dist: polars (>=0.13.11,<0.14.0)
-Requires-Dist: pyarrow (>=8.0.0,<9.0.0); extra == "pandas"
+Requires-Dist: polars (>=0.17.5,<0.18.0)
+Requires-Dist: pyarrow (>=11.0.0,<12.0.0) ; extra == "pandas"
 Requires-Dist: typing_extensions (>=4.3.0,<5.0.0)
 Project-URL: Documentation, https://tabeline.drhagen.com
 Project-URL: Repository, https://github.com/drhagen/tabeline
 Description-Content-Type: text/markdown
 
 # Tabeline
 
-Tabeline is a data table and data grammar library. You write the expressions in strings and supply them to methods on the `DataTable` class. The  strings are parsed by Parsita and converted into Polars for execution.
+Tabeline is a data frame and data grammar library. You write the expressions in strings and supply them to methods on the `DataFrame` class. The  strings are parsed by Parsita and converted into Polars for execution.
 
-Tabeline draws inspiration from dplyr, the data grammar of R's tidyverse, especially for its methods names. The `filter`, `mutate`, `group`, and `summarize` methods should all feel familiar. But Tabeline is as proper a Python library as can be, using methods instead of pipes, like is standard in R. 
+Tabeline draws inspiration from dplyr, the data grammar of R's tidyverse, especially for its methods names. The `filter`, `mutate`, `group_by`, and `summarize` methods should all feel familiar. But Tabeline is as proper a Python library as can be, using methods instead of pipes, like is standard in R. 
 
 Tabeline uses Polars under the hood, but adds a lot of handling of edge cases from Polars, which otherwise result in crashes or behavior that is not type stable.
 
 See the [Documentation](https://tabeline.drhagen.com) for the full user guide.
 
 ## Installation
 
@@ -43,30 +44,30 @@
 ```shell
 pip install tabeline
 ```
 
 ## Motivating example
 
 ```python
-from tabeline import DataTable
+from tabeline import DataFrame
 
-# Construct a table using clean syntax
+# Construct a data frame using clean syntax
 # from_csv, from_pandas, and from_polars are also available 
-table = DataTable(
+df = DataFrame(
     id=[0, 0, 0, 0, 1, 1, 1, 1, 1],
     t=[0, 6, 12, 24, 0, 6, 12, 24, 48],
     y=[0, 2, 3, 1, 0, 4, 3, 2, 1],
 )
 
 # Use data grammar methods and string expressions to define
-# transformed data tables
+# transformed data frames
 analysis = (
-    table
+    df
     .filter("t <= 24")
-    .group("id")
+    .group_by("id")
     .summarize(auc="trapz(t, y)")
 )
 
 print(analysis)
 # shape: (2, 2)
 # ┌─────┬──────┐
 # │ id  ┆ auc  │
```

