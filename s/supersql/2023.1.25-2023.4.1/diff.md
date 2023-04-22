# Comparing `tmp/supersql-2023.1.25.tar.gz` & `tmp/supersql-2023.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supersql-2023.1.25.tar", max compression
+gzip compressed data, was "supersql-2023.4.1.tar", max compression
```

## Comparing `supersql-2023.1.25.tar` & `supersql-2023.4.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1048 2023-01-20 22:27:04.453603 supersql-2023.1.25/LICENSE.md
--rw-r--r--   0        0        0     3014 2023-01-20 22:22:54.035362 supersql-2023.1.25/README.md
--rw-r--r--   0        0        0      775 2023-01-24 21:40:45.510426 supersql-2023.1.25/pyproject.toml
--rw-r--r--   0        0        0      270 2023-01-24 21:38:42.096087 supersql-2023.1.25/supersql/__init__.py
--rw-r--r--   0        0        0        0 2023-01-21 16:07:27.238714 supersql-2023.1.25/supersql/alternate.py
--rw-r--r--   0        0        0     3825 2023-01-23 22:21:05.508068 supersql-2023.1.25/supersql/column.py
--rw-r--r--   0        0        0      361 2023-01-24 21:38:06.428521 supersql-2023.1.25/supersql/constants.py
--rw-r--r--   0        0        0     1178 2023-01-23 00:14:26.817312 supersql-2023.1.25/supersql/core.py
--rw-r--r--   0        0        0      518 2023-01-24 17:41:24.391754 supersql-2023.1.25/supersql/helpers.py
--rw-r--r--   0        0        0     7766 2023-01-24 21:31:45.844196 supersql-2023.1.25/supersql/query.py
--rw-r--r--   0        0        0      784 2023-01-24 21:28:26.412383 supersql-2023.1.25/supersql/results.py
--rw-r--r--   0        0        0     1894 2023-01-23 22:15:39.229243 supersql-2023.1.25/supersql/table.py
--rw-r--r--   0        0        0     3843 1970-01-01 00:00:00.000000 supersql-2023.1.25/setup.py
--rw-r--r--   0        0        0     3701 1970-01-01 00:00:00.000000 supersql-2023.1.25/PKG-INFO
+-rwxr-xr-x   0        0        0     1048 2023-01-20 23:27:04.000000 supersql-2023.4.1/LICENSE.md
+-rwxr-xr-x   0        0        0     3014 2023-01-20 23:22:54.000000 supersql-2023.4.1/README.md
+-rwxr-xr-x   0        0        0      774 2023-04-22 21:34:07.078532 supersql-2023.4.1/pyproject.toml
+-rwxr-xr-x   0        0        0      269 2023-04-22 21:33:45.498403 supersql-2023.4.1/supersql/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-01-21 17:07:28.000000 supersql-2023.4.1/supersql/alternate.py
+-rwxr-xr-x   0        0        0     3823 2023-04-22 19:22:20.869838 supersql-2023.4.1/supersql/column.py
+-rwxr-xr-x   0        0        0      357 2023-04-22 10:50:47.426531 supersql-2023.4.1/supersql/constants.py
+-rwxr-xr-x   0        0        0     1178 2023-01-23 01:14:26.000000 supersql-2023.4.1/supersql/core.py
+-rwxr-xr-x   0        0        0     8626 2023-04-22 19:04:57.992610 supersql-2023.4.1/supersql/dquery.py
+-rwxr-xr-x   0        0        0      518 2023-01-24 18:41:24.000000 supersql-2023.4.1/supersql/helpers.py
+-rwxr-xr-x   0        0        0     8593 2023-04-22 19:50:07.215779 supersql-2023.4.1/supersql/query.py
+-rwxr-xr-x   0        0        0     1133 2023-04-22 21:31:41.349988 supersql-2023.4.1/supersql/results.py
+-rwxr-xr-x   0        0        0     1894 2023-04-22 11:20:09.187343 supersql-2023.4.1/supersql/table.py
+-rw-r--r--   0        0        0     3700 1970-01-01 00:00:00.000000 supersql-2023.4.1/PKG-INFO
```

### Comparing `supersql-2023.1.25/LICENSE.md` & `supersql-2023.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `supersql-2023.1.25/README.md` & `supersql-2023.4.1/README.md`

 * *Files identical despite different names*

### Comparing `supersql-2023.1.25/pyproject.toml` & `supersql-2023.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "supersql"
-version = "2023.1.25"
+version = "2023.4.1"
 description = "Thin wrapper on top of SQL that enables you write SQL code in python easily"
 authors = ["Tersoo Ortserga <codesage@live.com>"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.6"
```

### Comparing `supersql-2023.1.25/supersql/column.py` & `supersql-2023.4.1/supersql/column.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Man: Oh, very good restaurant, three stars you know.
 Wife: Really?
 Man: Mmm...
 
 Waiter: Good evening, sir! Good evening, madam! And may I say what a
     pleasure it is to see you here again, sir!
 
-Man: Oh thank you. Well there you are dear. Have a look there, anything
+Man: Oh thank you. Well  re you are dear. Have a look there, anything
     you like. The boeuf en croute is fantastic.
 
 Waiter: Oh if I may suggest, sir ... the pheasant à la reine, the sauce
     is one of the chefs most famous creations.
 
 Man: Em... that sounds good. Anyway just have a look... take your time. Oh, er
     by the way - got a bit of a dirty fork, could you ... er·.. get me another one?
```

### Comparing `supersql-2023.1.25/supersql/core.py` & `supersql-2023.4.1/supersql/core.py`

 * *Files identical despite different names*

### Comparing `supersql-2023.1.25/supersql/helpers.py` & `supersql-2023.4.1/supersql/helpers.py`

 * *Files identical despite different names*

### Comparing `supersql-2023.1.25/supersql/query.py` & `supersql-2023.4.1/supersql/dquery.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,208 +17,228 @@
         self._engine = engine
         self._sql = []
         self._args = []
         self._vals = []
         self._zero = None
 
     def __str__(self) -> str:
-        sql = ' '.join(s(False) for s in self._sql)
+        sql = ' '.join(s() for s in self._sql)
         return sql
+    
+    def _clone(self):
+        this = Query(self._engine)
+        this._sql = self._sql
+        return this
 
     def _conditional(self, condition: Column, param: any, command: str):
-        print(str(condition) * 40)
         if(isinstance(condition, str)):
             if not param:
                 raise ValueError('''
                     To prevent SQL Injection please use parameterized query with string
                     or use Supersql <type, 'Column'> syntax.
                 ''')
         elif not isinstance(condition, Column):
             raise ValueError(f'''
                 Supersql {command} command only accepts <type, 'Column'> or a parameterized
                 string and param second argument.
             ''')
-        def _(xpand = False):
+        def _():
+            # NOTE: self inside here is self of original query i.e. complete closure every time it is called it appends again
             if isinstance(condition, str):
                 self._args.append(Column.QUOTE(param))
                 sql = f'{command} {condition}'
             else:
-                self._args.append(condition._arg)
-                vendor = self._engine._vendor
-                if vendor == POSTGRES: placeholder = f'${len(self._args)}'
-                else: placeholder = '?'
-                column_sql = condition._sql.replace('--?--', placeholder)
-                sql = f'''{command} {column_sql}'''
+                if isinstance(condition._arg, (list, set, tuple)):
+                    # now only used for IN command i.e table.field.IN(args)
+                    arguments = len(self._args)
+                    self._args.extend(condition._arg)
+                    val = f"({', '.join([f'${arguments + index + 1}' for index, _ in enumerate(condition._arg)])})"
+                    column_sql = condition._sql.replace('--?--', val)
+                    sql = f'''{command} {column_sql}'''
+                else:
+                    self._args.append(condition._arg)
+                    arguments = len(self._args)
+                    vendor = self._engine._vendor
+                    if vendor == POSTGRES: placeholder = f'${arguments}'
+                    else: placeholder = '?'
+                    column_sql = condition._sql.replace('--?--', placeholder)
+                    sql = f'''{command} {column_sql}'''
             return sql
         self._sql.append(_)
         return self
 
-    async def go(self):
-        sql = ' '.join(s(True) for s in self._sql)
+    async def go(self, Intellisend=None):
+        sql = ' '.join(s() for s in self._sql)
         zero = self._zero
         pooled = self._engine._pooled
         ispg = self._engine.vendor == POSTGRES
         connexion = self._engine._connexion
 
         async def go(conn):
             if zero == SELECT:
-                if ispg:
-                    results = await conn.fetch(sql, *self._args)
+                if ispg: results = await conn.fetch(sql, *self._args)
                 else:
+                    # sqlite
                     results = await conn.execute_fetchall(sql, self._args)
                 return Rows(results)
 
             if len(self._vals) > 1:
                 results = await conn.executemany(sql, tuple(self._vals))
-                print('these are the results: ', results)
+                print('these are the results: ', results, sql)
             else:
                 results = await conn.execute(sql, *self._args)
             return Rows(results or [])
 
-        if ispg and pooled:
-            async with connexion.acquire() as connection:
-                return await go(connection)
+        if ispg:
+            if pooled:
+                async with connexion.acquire() as connection:
+                    return await go(connection)
+            return await go(connexion)
         else: return await go(connexion) # sqlite then until more databaseas added
 
     def _limit_offset(self, value: int, command: str):
         if not isinstance(value, int):
             raise ValueError(f'{command} only accepts integer values')
-        self._sql.append(lambda xp: f'''{command} {value}''')
+        self._sql.append(lambda : f'''{command} {value}''')
         return self
 
     def sql(self, unsafe = False) -> str:
         vendor = self._engine.vendor
-        sql = str(self)
+        sql = str(self._clone())
         if unsafe:
             if vendor != POSTGRES:
                 for arg in self._args:
                     sql = sql.replace('?', arg, 1)
             else:
                 for pos, arg in enumerate(self._args):
                     sql = sql.replace(f'${pos + 1}', arg, 1)
         return sql
 
     def AND(self, condition: Column | str, param = None):
         return self._conditional(condition, param, AND)
 
     def ASC(self):
-        def _(xp):
+        def _():
             return f'ASC'
         self._sql.append(_)
         return self
 
     def DESC(self):
-        def _(xp):
+        def _():
             return f'DESC'
         self._sql.append(_)
         return self
 
     def DELETE(self):
-        self._sql.append(lambda xp: 'DELETE')
+        self._sql.append(lambda : 'DELETE')
         return self
 
     def FROM(self, *tables: List[str | int]):
-        def _(xp = ...):
+        def _():
             _tables = [Table.COERCE(t) for t in tables]
             return f'''FROM {', '.join(_tables)}'''
         self._sql.append(_)
         return self
 
     def INTO(self, table: Table):
         try: self._sql[-2]
-        except: self._sql.append(lambda xp: f'INTO {table}')
-        else: self._sql[-2] = lambda xp: f'INSERT INTO {table}'
+        except: self._sql.append(lambda : f'INTO {table}')
+        else: self._sql[-2] = lambda : f'INSERT INTO {table}'
         return self
 
     def INSERT(self, *columns: Column):
         self._zero = self._zero or INSERT
-        def _(xp = ...):
+        def _():
             return f'''({', '.join(str(column) for column in columns)})'''
-        self._sql.extend([lambda xp: '--', _])
+        self._sql.extend([lambda : '--', _])
         return self
 
     def INSERT_INTO(self, table: Table, columns: List[Column]):
         self._zero = self._zero or INSERT
-        def _(xp = ...):
+        def _():
             return f'''INSERT INTO {table} ({', '.join(str(column) for column in columns)})'''
         self._sql.append(_)
         return self
 
     def LIMIT(self, limit: int):
         return self._limit_offset(limit, LIMIT)
 
     def OFFSET(self, offset: int):
         return self._limit_offset(offset, OFFSET)
 
     def OR(self, condition: Column | str, param = None):
         return self._conditional(condition, param, OR)
 
     def ORDER_BY(self, column: Column):
-        def _(xp = ...):
+        def _():
             return f'''ORDER BY {column._sql or column}'''
         self._sql.append(_)
         return self
+    
+    def RAW(self, statement: str):
+        self._sql.append(lambda: statement)
+        return self
 
     def RETURNING(self, column: Column):
-        def _(xp = ...):
+        def _():
             return f'RETURNING {column}'
         self._sql.append(_)
         return self
 
     def SELECT(self, *columns) -> 'Query':
         """Pythonic interface to SQL SELECT allowing python
         to be used to build SQL queries.
 
         Parameters:
             columns (List[str | int]): Variable args param that accepts either a string of
             Supersql Column Type.
             Raises an error if a type other than str | Column is used.
         """
         self._zero = self._zero or SELECT
-        def _(xp = ...):
+        def _():
             _columns = [Column.COERCE(f) for f in columns]
             return f'''SELECT {', '.join(_columns)}''' if _columns else 'SELECT *'
         self._sql.append(_)
         return self
 
     def SET(self, *columns: Column):
-        def _(xpand = False):
+        def _():
             vendor = self._engine._vendor
             statements = []
             for column in columns:
                 self._args.append(column._arg)
                 if vendor == POSTGRES: placeholder = f'${len(self._args)}'
                 else: placeholder = '?'
                 column_sql = column._sql.replace('--?--', placeholder)
                 statements.append(column_sql)
             return f"SET {', '.join(statements)}"
         self._sql.append(_)
         return self
 
     def UPDATE(self, table: Table):
         self._zero = self._zero or UPDATE
-        self._sql.append(lambda xp: f'''UPDATE {table}''')
+        self._sql.append(lambda : f'''UPDATE {table}''')
         return self
 
     def VALUES(self, *matrix: Tuple[any]):
         msg = 'VALUES expects a tuple if inserting a row or multiple tuples if inserting multiple rows'
         homogeneous = set()
         for values in matrix:
             if not isinstance(values, (tuple, list)):
                 raise ValueError(msg)
             homogeneous.add(len(values))
         if len(homogeneous) > 1:
             raise SyntaxError('VALUES matrix has tuples of different lengths')
-        def _(xpand = False):
+        def _():
             vendor = self._engine._vendor
             count = homogeneous.copy().pop()
             if vendor == POSTGRES:
                 placeholders = [f'${pos + 1}' for pos in range(count)]
             else:
                 placeholders = ['?'] * count
-            if xpand: self._vals.extend(matrix)
+            self._vals.extend(matrix)
             return f'''VALUES ({', '.join(placeholders)})'''
         self._sql.append(_)
         return self
 
     def WHERE(self, condition: Column | str, param = None):
         return self._conditional(condition, param, WHERE)
```

### Comparing `supersql-2023.1.25/supersql/table.py` & `supersql-2023.4.1/supersql/table.py`

 * *Files identical despite different names*

### Comparing `supersql-2023.1.25/setup.py` & `supersql-2023.4.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,140 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: supersql
+Version: 2023.4.1
+Summary: Thin wrapper on top of SQL that enables you write SQL code in python easily
+Author: Tersoo Ortserga
+Author-email: codesage@live.com
+Requires-Python: >=3.6,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: mysql
+Provides-Extra: postgres
+Provides-Extra: sqlite
+Description-Content-Type: text/markdown
 
-packages = \
-['supersql']
+Supersql Library
+================
+There are many great database tools for python (i.e. databases, SQLAlchemy, PeeWee etc.) - **but there is no Python tool for databases.**
 
-package_data = \
-{'': ['*']}
+In addition you might have come to the same realisation and thinking the following:
 
-entry_points = \
-{'console_scripts': ['supersql = supersql:main']}
-
-setup_kwargs = {
-    'name': 'supersql',
-    'version': '2023.1.25',
-    'description': 'Thin wrapper on top of SQL that enables you write SQL code in python easily',
-    'long_description': 'Supersql Library\n================\nThere are many great database tools for python (i.e. databases, SQLAlchemy, PeeWee etc.) - **but there is no Python tool for databases.**\n\nIn addition you might have come to the same realisation and thinking the following:\n\n1. But we don\'t want to use an ORM\n\n2. Why can\'t we get a low level pythonic, powerful SQL api with with semantic interaction primitives\n\n3. Async and Sync support should be supported\n\nSupersql checks all those boxes and more. It is a python superset of SQL - allowing you leverage the full power of python to\nwrite advanced SQL queries.\n\n&nbsp;\n\n**Tutorial**: [Open Documentation](https://rayattack.github.io/supersql/)\n\n**Requirements**: Python 3.6+\n\n&nbsp;\n\n\n### NOTE: Still Very Much In Development\n\n```sql\nSELECT * FROM customers ORDER BY last_name ASC LIMIT 5\n```\n\n\n```py\n# query.SELECT(\'*\') is the same as query.SELECT() or query.SELECT(customers)\nquery.SELECT().FROM(customers).ORDER_BY(-customers.last_name).LIMIT(5)\n```\n\n&nbsp;\n\n## Why?\nLet\'s be honest:\n\n1. Writing sql templates using string formatting is really painful.\n2. Sometimes an ORM is not what you need, and whilst the new\n`f strings` in python solve a lot of problems, complex SQL templating is not of\nthem.\n\n3. Supersql makes it super simple to connect to and start querying a database in python.\n\n&nbsp;\n\nLet the code do the explanation:\n```py\n\nfrom supersql import Query\n\n\nquery = Query(\'postgres://user:password@hostname:5432/database\')\n\n\n# Without table schema discovery/reflection i.e. using strings -- NOT OPTIMAL\nresults = query.SELECT(\n        \'first_name\', \'last_name\', \'email\'\n    ).FROM(\n        \'employees\'\n    ).WHERE(\'email = someone@example.com\').execute()\n\nfor result in results:\n    print(result)\n\n\n# reflect table schema and fields into a python object for easy querying\nemps = query.database.table(\'employees\')\n\nrecords = query.SELECT(\n        emps.first_name, emps.last_name, emps.email\n    ).FROM(\n        emps\n    ).WHERE(emps.email == \'someone@example.com\').execute()\n```\n\n&nbsp;\n\nWhat about support for Code First flows? Also supported using Table objects\n```py\nfrom supersql import Table, Varchar, Date, Smallint\n\nclass Employee(Table):\n    """\n    SuperSQL is not an ORM. Table only helps you avoid magic\n    literals in your code. SuperSQL is not an ORM\n    """\n    __pk__ = (\'email\', \'identifier\')\n\n    identifier = Varchar()\n    email = Varchar(required=True, unique=None, length=25)\n    age = Smallint()\n    first_name = String(required=True)\n    last_name = String(25)\n    created_on = Date()\n\n\n# Now lets try again\nemp = Employee()\nresults = query.SELECT(\n    emp.first_name, emp.last_name, emp.email\n).FROM(emp).WHERE(\n    emp.email == \'someone@example.com\'\n).execute()\n```\n\n\n&nbsp;\n\n\n**Note**\n---\n**Supersql is not an ORM so there is no magic Table.save() Table.find() features nor will they ever be supported.**\nThe `Table` class is provided only to help with magic literal elimination from your codebase i.e. a query helper and nothing more.\n\n---\n',
-    'author': 'Tersoo Ortserga',
-    'author_email': 'codesage@live.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'entry_points': entry_points,
-    'python_requires': '>=3.6,<4.0',
-}
+1. But we don't want to use an ORM
 
+2. Why can't we get a low level pythonic, powerful SQL api with with semantic interaction primitives
+
+3. Async and Sync support should be supported
+
+Supersql checks all those boxes and more. It is a python superset of SQL - allowing you leverage the full power of python to
+write advanced SQL queries.
+
+&nbsp;
+
+**Tutorial**: [Open Documentation](https://rayattack.github.io/supersql/)
+
+**Requirements**: Python 3.6+
+
+&nbsp;
+
+
+### NOTE: Still Very Much In Development
+
+```sql
+SELECT * FROM customers ORDER BY last_name ASC LIMIT 5
+```
+
+
+```py
+# query.SELECT('*') is the same as query.SELECT() or query.SELECT(customers)
+query.SELECT().FROM(customers).ORDER_BY(-customers.last_name).LIMIT(5)
+```
+
+&nbsp;
+
+## Why?
+Let's be honest:
+
+1. Writing sql templates using string formatting is really painful.
+2. Sometimes an ORM is not what you need, and whilst the new
+`f strings` in python solve a lot of problems, complex SQL templating is not of
+them.
+
+3. Supersql makes it super simple to connect to and start querying a database in python.
+
+&nbsp;
+
+Let the code do the explanation:
+```py
+
+from supersql import Query
+
+
+query = Query('postgres://user:password@hostname:5432/database')
+
+
+# Without table schema discovery/reflection i.e. using strings -- NOT OPTIMAL
+results = query.SELECT(
+        'first_name', 'last_name', 'email'
+    ).FROM(
+        'employees'
+    ).WHERE('email = someone@example.com').execute()
+
+for result in results:
+    print(result)
+
+
+# reflect table schema and fields into a python object for easy querying
+emps = query.database.table('employees')
+
+records = query.SELECT(
+        emps.first_name, emps.last_name, emps.email
+    ).FROM(
+        emps
+    ).WHERE(emps.email == 'someone@example.com').execute()
+```
+
+&nbsp;
+
+What about support for Code First flows? Also supported using Table objects
+```py
+from supersql import Table, Varchar, Date, Smallint
+
+class Employee(Table):
+    """
+    SuperSQL is not an ORM. Table only helps you avoid magic
+    literals in your code. SuperSQL is not an ORM
+    """
+    __pk__ = ('email', 'identifier')
+
+    identifier = Varchar()
+    email = Varchar(required=True, unique=None, length=25)
+    age = Smallint()
+    first_name = String(required=True)
+    last_name = String(25)
+    created_on = Date()
+
+
+# Now lets try again
+emp = Employee()
+results = query.SELECT(
+    emp.first_name, emp.last_name, emp.email
+).FROM(emp).WHERE(
+    emp.email == 'someone@example.com'
+).execute()
+```
+
+
+&nbsp;
+
+
+**Note**
+---
+**Supersql is not an ORM so there is no magic Table.save() Table.find() features nor will they ever be supported.**
+The `Table` class is provided only to help with magic literal elimination from your codebase i.e. a query helper and nothing more.
+
+---
 
-setup(**setup_kwargs)
```

