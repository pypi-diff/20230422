# Comparing `tmp/pgmini-0.1.3.tar.gz` & `tmp/pgmini-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgmini-0.1.3.tar", max compression
+gzip compressed data, was "pgmini-0.1.4.tar", max compression
```

## Comparing `pgmini-0.1.3.tar` & `pgmini-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1461 2023-02-19 07:19:37.209313 pgmini-0.1.3/LICENSE
--rw-r--r--   0        0        0     7773 2023-04-03 05:54:55.113389 pgmini-0.1.3/README.md
--rw-r--r--   0        0        0     2054 2023-04-03 05:56:43.231188 pgmini-0.1.3/pgmini/__init__.py
--rw-r--r--   0        0        0      614 2023-02-24 08:44:04.617355 pgmini-0.1.3/pgmini/alias.py
--rw-r--r--   0        0        0      804 2023-02-23 11:58:37.582351 pgmini-0.1.3/pgmini/array.py
--rw-r--r--   0        0        0     1854 2023-02-23 11:58:37.573751 pgmini-0.1.3/pgmini/case.py
--rw-r--r--   0        0        0      874 2023-02-24 08:43:54.427071 pgmini-0.1.3/pgmini/cast.py
--rw-r--r--   0        0        0     1663 2023-02-23 11:58:37.566136 pgmini-0.1.3/pgmini/column.py
--rw-r--r--   0        0        0     1540 2023-02-24 08:45:15.018968 pgmini-0.1.3/pgmini/delete.py
--rw-r--r--   0        0        0      272 2023-02-23 06:15:18.337495 pgmini-0.1.3/pgmini/distinct.py
--rw-r--r--   0        0        0     4358 2023-03-10 11:05:47.770188 pgmini-0.1.3/pgmini/func.py
--rw-r--r--   0        0        0     6736 2023-03-10 11:20:29.617469 pgmini-0.1.3/pgmini/insert.py
--rw-r--r--   0        0        0     2018 2023-02-23 11:58:37.595454 pgmini-0.1.3/pgmini/literal.py
--rw-r--r--   0        0        0     2010 2023-02-27 06:30:22.659219 pgmini-0.1.3/pgmini/marks.py
--rw-r--r--   0        0        0     2687 2023-02-23 06:15:18.320773 pgmini-0.1.3/pgmini/operation.py
--rw-r--r--   0        0        0     6891 2023-04-01 15:12:57.306865 pgmini-0.1.3/pgmini/operations.py
--rw-r--r--   0        0        0     2829 2023-02-23 11:58:37.588950 pgmini-0.1.3/pgmini/operators.py
--rw-r--r--   0        0        0     1616 2023-02-24 08:44:04.622843 pgmini-0.1.3/pgmini/order_by.py
--rw-r--r--   0        0        0     1037 2023-02-23 11:58:37.570082 pgmini-0.1.3/pgmini/param.py
--rw-r--r--   0        0        0     9441 2023-02-24 08:45:15.014120 pgmini-0.1.3/pgmini/select.py
--rw-r--r--   0        0        0     1711 2023-02-23 11:57:58.880457 pgmini-0.1.3/pgmini/subquery.py
--rw-r--r--   0        0        0     1134 2023-02-23 09:40:15.343020 pgmini-0.1.3/pgmini/table.py
--rw-r--r--   0        0        0     2576 2023-02-24 08:45:15.029030 pgmini-0.1.3/pgmini/update.py
--rw-r--r--   0        0        0     2825 2023-02-26 06:21:00.926047 pgmini-0.1.3/pgmini/utils.py
--rw-r--r--   0        0        0      899 2023-04-03 05:57:31.854377 pgmini-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     8828 1970-01-01 00:00:00.000000 pgmini-0.1.3/setup.py
--rw-r--r--   0        0        0     8251 1970-01-01 00:00:00.000000 pgmini-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1461 2023-02-19 07:19:37.209313 pgmini-0.1.4/LICENSE
+-rw-r--r--   0        0        0     7773 2023-04-03 05:59:48.504852 pgmini-0.1.4/README.md
+-rw-r--r--   0        0        0     2054 2023-04-22 06:25:52.799975 pgmini-0.1.4/pgmini/__init__.py
+-rw-r--r--   0        0        0      614 2023-02-24 08:44:04.617355 pgmini-0.1.4/pgmini/alias.py
+-rw-r--r--   0        0        0      804 2023-02-23 11:58:37.582351 pgmini-0.1.4/pgmini/array.py
+-rw-r--r--   0        0        0     1854 2023-02-23 11:58:37.573751 pgmini-0.1.4/pgmini/case.py
+-rw-r--r--   0        0        0      874 2023-02-24 08:43:54.427071 pgmini-0.1.4/pgmini/cast.py
+-rw-r--r--   0        0        0     1663 2023-02-23 11:58:37.566136 pgmini-0.1.4/pgmini/column.py
+-rw-r--r--   0        0        0     1540 2023-02-24 08:45:15.018968 pgmini-0.1.4/pgmini/delete.py
+-rw-r--r--   0        0        0      272 2023-02-23 06:15:18.337495 pgmini-0.1.4/pgmini/distinct.py
+-rw-r--r--   0        0        0     4358 2023-03-10 11:05:47.770188 pgmini-0.1.4/pgmini/func.py
+-rw-r--r--   0        0        0     6736 2023-03-10 11:20:29.617469 pgmini-0.1.4/pgmini/insert.py
+-rw-r--r--   0        0        0     2018 2023-02-23 11:58:37.595454 pgmini-0.1.4/pgmini/literal.py
+-rw-r--r--   0        0        0     2010 2023-02-27 06:30:22.659219 pgmini-0.1.4/pgmini/marks.py
+-rw-r--r--   0        0        0     2687 2023-02-23 06:15:18.320773 pgmini-0.1.4/pgmini/operation.py
+-rw-r--r--   0        0        0     6891 2023-04-01 15:12:57.306865 pgmini-0.1.4/pgmini/operations.py
+-rw-r--r--   0        0        0     2829 2023-02-23 11:58:37.588950 pgmini-0.1.4/pgmini/operators.py
+-rw-r--r--   0        0        0     1616 2023-02-24 08:44:04.622843 pgmini-0.1.4/pgmini/order_by.py
+-rw-r--r--   0        0        0     1037 2023-02-23 11:58:37.570082 pgmini-0.1.4/pgmini/param.py
+-rw-r--r--   0        0        0     9441 2023-02-24 08:45:15.014120 pgmini-0.1.4/pgmini/select.py
+-rw-r--r--   0        0        0     1711 2023-02-23 11:57:58.880457 pgmini-0.1.4/pgmini/subquery.py
+-rw-r--r--   0        0        0     1134 2023-02-23 09:40:15.343020 pgmini-0.1.4/pgmini/table.py
+-rw-r--r--   0        0        0     2576 2023-02-24 08:45:15.029030 pgmini-0.1.4/pgmini/update.py
+-rw-r--r--   0        0        0     2825 2023-02-26 06:21:00.926047 pgmini-0.1.4/pgmini/utils.py
+-rw-r--r--   0        0        0      901 2023-04-22 06:27:53.347307 pgmini-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     8815 1970-01-01 00:00:00.000000 pgmini-0.1.4/setup.py
+-rw-r--r--   0        0        0     8238 1970-01-01 00:00:00.000000 pgmini-0.1.4/PKG-INFO
```

### Comparing `pgmini-0.1.3/LICENSE` & `pgmini-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.3/README.md` & `pgmini-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -200,15 +200,15 @@
 #     ['some text', 'active', 'other text'],
 # )
 
 # From select
 q = (
     Insert(t, columns=(t.name, t.status))
     .Select(
-        Select(F.concat(t.name, F.random().Cast('text'), t.status))
+        Select(F.concat(t.name, F.random().Cast('text')), t.status)
         .From(t)
         .Where(t.id < 100)
         .Limit(10)
     )
     .Returning(t.STAR)
 )
```

### Comparing `pgmini-0.1.3/pgmini/__init__.py` & `pgmini-0.1.4/pgmini/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     CTX_DISABLE_TABLE_IN_COLUMN,
     CTX_FORCE_CAST_BRACKETS,
     CTX_TABLES,
     CompileABC,
 )
 
 
-__version__ = '0.1.3'
+__version__ = '0.1.4'
 __all__ = (
     'And',
     'Array',
     'Case',
     'Delete',
     'Excluded',
     'Exists',
```

### Comparing `pgmini-0.1.3/pgmini/alias.py` & `pgmini-0.1.4/pgmini/alias.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.3/pgmini/array.py` & `pgmini-0.1.4/pgmini/array.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.3/pgmini/case.py` & `pgmini-0.1.4/pgmini/case.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.3/pgmini/cast.py` & `pgmini-0.1.4/pgmini/cast.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.3/pgmini/column.py` & `pgmini-0.1.4/pgmini/column.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.3/pgmini/delete.py` & `pgmini-0.1.4/pgmini/delete.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.3/pgmini/func.py` & `pgmini-0.1.4/pgmini/func.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.3/pgmini/insert.py` & `pgmini-0.1.4/pgmini/insert.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.3/pgmini/literal.py` & `pgmini-0.1.4/pgmini/literal.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.3/pgmini/marks.py` & `pgmini-0.1.4/pgmini/marks.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.3/pgmini/operation.py` & `pgmini-0.1.4/pgmini/operation.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.3/pgmini/operations.py` & `pgmini-0.1.4/pgmini/operations.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.3/pgmini/operators.py` & `pgmini-0.1.4/pgmini/operators.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.3/pgmini/order_by.py` & `pgmini-0.1.4/pgmini/order_by.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.3/pgmini/param.py` & `pgmini-0.1.4/pgmini/param.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.3/pgmini/select.py` & `pgmini-0.1.4/pgmini/select.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.3/pgmini/subquery.py` & `pgmini-0.1.4/pgmini/subquery.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.3/pgmini/table.py` & `pgmini-0.1.4/pgmini/table.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.3/pgmini/update.py` & `pgmini-0.1.4/pgmini/update.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.3/pgmini/utils.py` & `pgmini-0.1.4/pgmini/utils.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.3/pyproject.toml` & `pgmini-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "pgmini"
-version = "0.1.3"
+version = "0.1.4"
 description = "Build sql for PostgreSQL"
 authors = ["Vitalii Ponomar"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ponomar/pgmini"
 
 [tool.poetry.dependencies]
-python = "^3.10"
-attrs = "^22.2.0"
+python = ">=3.10"
+attrs = ">=22.2.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 isort = "^5.12.0"
 ruff = "^0.0.252"
 tomli = "^2.0.1"
```

### Comparing `pgmini-0.1.3/setup.py` & `pgmini-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 packages = \
 ['pgmini']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['attrs>=22.2.0,<23.0.0']
+['attrs>=22.2.0']
 
 setup_kwargs = {
     'name': 'pgmini',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'Build sql for PostgreSQL',
-    'long_description': '[![Test & Lint](https://github.com/ponomar/pgmini/actions/workflows/main.yml/badge.svg)](https://github.com/ponomar/pgmini/actions/workflows/main.yml)\n\n## 🇺🇦 What is pgmini? 🇺🇦\n\nIt is the PostgreSQL query builder with next core principles:\n- simple (predictable, without magic)\n- fast\n\nAll object are immutable (thanks to [attrs](https://www.attrs.org) lib).\nPython code as close to SQL structure as possible.\nLibrary doesn\'t try to be everything.\nIt doesn\'t manage connections to postgres, doesn\'t escape params.\nAll this can and should be done with other tools: (asyncpg, psycopg2, postgresql itself etc.).\n\nI\'ve decided to use `PascalCase` methods naming to avoid collisions with python reserved words: \n`From`, `And`, `Or`, `Else`, `With`, `As` etc.\n\n## Examples\n```python\nUser = Table(\'user\')  # dynamic columns\n\nq = Select(User.id, User.name).From(User).Where(User.email == \'test@test.com\')\n\nbuild(q)\n# (\n#     \'SELECT id, name FROM "user" WHERE email = $1\', \n#     [\'test@test.com\'],\n# )\n```\n\nExplicitly defined table schema allows to save filters and methods for further reusing \nand to use IDE code analyzers for smart completions, find usages, bulk refactors etc.  \n```python\nclass RoleSchema(Table):\n    id: int\n    name: str\n    status: str\n    \n    @property\n    def status_active(self):  # can also be decorated with functools.cache\n        return self.status == Literal(\'active\')\n    \n    def name_startswith(self, value: str):\n        return self.name.Like(f\'{value}%\')\n\nRole = RoleSchema(\'role\')\nq = Select(Role.id).From(Role).Where(Role.status_active, Role.name_startswith(\'admin\'))\n\nRoleAlias = Role.As(\'role2\')  # all columns/methods are visible for IDE live inspection as well\nq = (\n    Select(Role.STAR).From(Role)\n    .Where(Not(Exists(\n        Select(1).From(RoleAlias)\n        .Where(RoleAlias.id < Role.id, RoleAlias.status_active)\n    )))\n)\n```\n\n#### WHERE\nWhere takes *args which work like AND operator.\n```python\nt = Table(\'tbl\')\nq = (\n    Select(t.id).From(t)\n    .Where(\n        t.id.Between(10, 20), \n        Or(t.name > \'name\', And(t.status == \'active\', Not(t.id == 15))),\n    )\n)\n# SELECT id FROM tbl WHERE id BETWEEN $1 AND $2 AND (name > $3 OR (status = $4 AND NOT (id = $5)))\n\n# Add filters to existent query\nq2 = q.Where(t.id != 14)\n```\n\n#### JOIN\n```python\nt, t2 = Table(\'tbl\'), Table(\'tbl2\')\n\nsq = Select(t2.name).From(t2).Where(t2.id == t.id).Subquery(\'sq\')\nq = (\n    Select(t.id).From(t)\n    .Join(t2, t2.id == t.id)\n    .LeftJoin(t2, And(t2.id == t.id, t2.status == \'active\'))\n    .JoinLateral(sq, True)\n    .LeftJoinLateral(sq, sq.name != \'test\')\n)\n```\n\n#### PARAMETERS / LITERALS\nBy default, all values are considered as parameters. \nIf you need to cast value or add alias use Param wrapper.\nIf you need to literally insert value into sql use special Literal wrapper, \nbut be very careful - it won\'t be escaped and can lead to SQL injections. \nUse Literal only with data you can 100% trust.\n```python\nt = Table(\'tbl\')\nq = (\n    Select(t.STAR, Param(10).Cast(\'int\').As(\'added\')).From(t)\n    .Where(\n        t.id1 == 1, \n        t.id2 != Param(2).Cast(\'float\'), \n        t.id3 > Literal(3), \n        t.id4 < Literal(4).Cast(\'numeric\'),\n    )\n)\nbuild(q)\n# (\n#     \'SELECT *, $1::int AS added FROM tbl WHERE id1 == $2 AND id2 != $3::float AND id3 > 3 AND id4 < 4::numeric\',\n#     [10, 1, 2],\n# )\n```\n\n#### FUNCTIONS\nThere are `Func` and its `F` alias.\n```python\nt = Table(\'tbl\')\n\nq1 = (\n    Select(\n        F.count(\'*\'), \n        F.count(t.id).Where(t.id > 10, t.id < 20),\n        F.array_agg(t.id).OrderBy(t.id.Desc().NullsLast()).As(\'ids\'),\n    )\n    .From(t)\n)\n\nq2 = Select(t.id, F.row_number().Over(partition_by=t.status, order_by=t.id)).From(t)\n\nf = F.unnest(Literal([1, 2, 3])).As(\'idx\')\nq3 = Select(f.STAR).From(f)\n# SELECT * FROM UNNEST(ARRAY[1, 2, 3]) AS idx\n\nq4 = Select(Case((t.id == 1, \'first\'), (t.id == 2, \'second\'), Else=\'third\').As(\'val\')).From(t)\n\nq5 = Select(Array([t.id, 5, 7])).From(t)\n```\n\n#### ORDER BY / GROUP BY / HAVING / DISTINCT / DISTINCT ON\n```python\nt = Table(\'tbl\')\n\nq1 = Select(t.id.Distinct()).From(t)\n# SELECT DISTINCT id FROM tbl\n\nq2 = Select(t.STAR).From(t).OrderBy(t.id.Desc(), t.name.NullsLast())\n\nq3 = Select(F.count(\'*\')).From(t).GroupBy(t.status).Having(F.count(\'*\') > 10)\n\nq4 = Select(t.id, t.status).From(t).DistinctOn(t.status)\n# SELECT DISTINCT ON (status) id, status FROM tbl\n```\n\n#### OPERATIONS\nBasic math operator are supported out of the box: \n`+`, `-`, `*`, `/`, `>`, `>=`, `<`, `<=`. \nOthers are support as methods:\n```python\nt = Table(\'tbl\')\nq = (\n    Select(\n        t.id + t.id,\n        t.id - 1,\n        t.id * 10,\n        t.id > 15,\n        (t.id == 10).As(\'equals_ten\'),\n        (t.id != 11).As(\'not_equals_eleven\'),\n        Param(10) > 9,\n        (Literal(5) * 3.5).Cast(\'int\'),\n        t.id.Between(1, 2),\n        t.id.In([1, 2, 3]),\n        t.id.NotIn(Select(t.id).From(t).Where(t.id < 10)),\n        t.name.Is(None),\n        t.active.IsNot(False),\n        t.data.Op(\'->>\', \'key\').As(\'value1\'),\n        t.data.Op(\'#>>\', [\'key1\', \'key2\']).As(\'value2\'),\n        t.id.Any(list(range(1_000))),\n        t.name.Like(\'%ABC%\'),\n        t.name.Ilike(\'%abc%\'),\n    )\n    .From(t)\n)\n```\n\n#### INSERT\n```python\nt = Table(\'tbl\')\nq = (\n    Insert(t, columns=(t.name, t.status))\n    .Values(\n        (Param(\'some text\').Cast(\'varchar(10)\'), \'active\'),\n        (\'other text\', Literal(\'deleted\')),\n    )\n    .Returning(t.STAR)\n)\n\nbuild(q)\n# (\n#     "INSERT INTO tbl (name, status) VALUES ($1::varchar(10), $2), ($3, \'deleted\') RETURNING *",\n#     [\'some text\', \'active\', \'other text\'],\n# )\n\n# From select\nq = (\n    Insert(t, columns=(t.name, t.status))\n    .Select(\n        Select(F.concat(t.name, F.random().Cast(\'text\'), t.status))\n        .From(t)\n        .Where(t.id < 100)\n        .Limit(10)\n    )\n    .Returning(t.STAR)\n)\n\n# CTE\nsq = Select(t.STAR).From(t).Where(t.id < 100).Subquery(\'sq\')\nq = (\n    With(sq)\n    .Insert(t, (\'name\', \'status\'))\n    .From(Select(sq.name, sq.status).From(sq))\n)\n\n# Efficient bulk insert from the list of values\nvalues = [(str(i), \'active\') for i in range(1_000)]\nq = (\n    Insert(t, (\'name\', \'status\'))\n    .From(Select(\n        F.unnest(Param([name for name, _ in values]).Cast(\'text[]\')),\n        F.unnest(Param([status for _, status in values]).Cast(\'enum_status[]\')),\n    ))\n)\n```\n\n#### UPDATE / DELETE\n```python\nt = Table(\'stmh\')\nq1 = Update(t).Set({t.name: \'second\'}).Where(t.name == \'first\', t.status == \'active\').Returning(t.id)\nq2 = Delete(t).Where(t.id == 25).Returning(t.id)\n```\n\n#### Subquery / CTE\nAny Select/Insert/Update/Delete has Subquery method.\n```python\nt = Table(\'tbl\')\nsq = Select(t.id).From(t).Where(t.id < 100).Subquery(\'sq\')\n\n# Subquery\nq = Select(sq.id).From(sq).Where(sq.id > 50)\n# SELECT id FROM (SELECT id FROM tbl WHERE id < $1) As sq WHERE id > $2\n\n# CTE\nq = With(sq).Select(sq.id).From(sq).Where(sq.id > 50).Limit(2)\n# WITH sq AS (SELECT id FROM tbl WHERE id < $1) SELECT id FROM sq WHERE id > $2 LIMIT $3\n```\n\n***\n\n### Why not sqlalchemy?\n- too smart (tries to do everything: from connection/session management, to sql generating and params escaping)\n- too complex\n- too slow\n- mutable (on its core)\n\nIt is good for simple projects with simple sql queries. \nBut when your project grows up, your team grows up, sqlalchemy always leads to errors,\nunnecessary complexity, extra time your team need to spend to learn it, find not obvious bugs etc.  \n\n\n### Why not pypika?\nWhile it is much simpler then sqlalchemy, it also requires you to learn their own "sql syntax" which is not always obvious.\nAnd by default it uses parameters as literals, so it can lead to sql injections.\n\n\n***\n\nThe library is inspired by Ukraine🇺🇦 (Kyiv is my home) and its brave and free people🔱.\n\nSlava Ukraini, Heroyam slava!\n',
+    'long_description': '[![Test & Lint](https://github.com/ponomar/pgmini/actions/workflows/main.yml/badge.svg)](https://github.com/ponomar/pgmini/actions/workflows/main.yml)\n\n## 🇺🇦 What is pgmini? 🇺🇦\n\nIt is the PostgreSQL query builder with next core principles:\n- simple (predictable, without magic)\n- fast\n\nAll object are immutable (thanks to [attrs](https://www.attrs.org) lib).\nPython code as close to SQL structure as possible.\nLibrary doesn\'t try to be everything.\nIt doesn\'t manage connections to postgres, doesn\'t escape params.\nAll this can and should be done with other tools: (asyncpg, psycopg2, postgresql itself etc.).\n\nI\'ve decided to use `PascalCase` methods naming to avoid collisions with python reserved words: \n`From`, `And`, `Or`, `Else`, `With`, `As` etc.\n\n## Examples\n```python\nUser = Table(\'user\')  # dynamic columns\n\nq = Select(User.id, User.name).From(User).Where(User.email == \'test@test.com\')\n\nbuild(q)\n# (\n#     \'SELECT id, name FROM "user" WHERE email = $1\', \n#     [\'test@test.com\'],\n# )\n```\n\nExplicitly defined table schema allows to save filters and methods for further reusing \nand to use IDE code analyzers for smart completions, find usages, bulk refactors etc.  \n```python\nclass RoleSchema(Table):\n    id: int\n    name: str\n    status: str\n    \n    @property\n    def status_active(self):  # can also be decorated with functools.cache\n        return self.status == Literal(\'active\')\n    \n    def name_startswith(self, value: str):\n        return self.name.Like(f\'{value}%\')\n\nRole = RoleSchema(\'role\')\nq = Select(Role.id).From(Role).Where(Role.status_active, Role.name_startswith(\'admin\'))\n\nRoleAlias = Role.As(\'role2\')  # all columns/methods are visible for IDE live inspection as well\nq = (\n    Select(Role.STAR).From(Role)\n    .Where(Not(Exists(\n        Select(1).From(RoleAlias)\n        .Where(RoleAlias.id < Role.id, RoleAlias.status_active)\n    )))\n)\n```\n\n#### WHERE\nWhere takes *args which work like AND operator.\n```python\nt = Table(\'tbl\')\nq = (\n    Select(t.id).From(t)\n    .Where(\n        t.id.Between(10, 20), \n        Or(t.name > \'name\', And(t.status == \'active\', Not(t.id == 15))),\n    )\n)\n# SELECT id FROM tbl WHERE id BETWEEN $1 AND $2 AND (name > $3 OR (status = $4 AND NOT (id = $5)))\n\n# Add filters to existent query\nq2 = q.Where(t.id != 14)\n```\n\n#### JOIN\n```python\nt, t2 = Table(\'tbl\'), Table(\'tbl2\')\n\nsq = Select(t2.name).From(t2).Where(t2.id == t.id).Subquery(\'sq\')\nq = (\n    Select(t.id).From(t)\n    .Join(t2, t2.id == t.id)\n    .LeftJoin(t2, And(t2.id == t.id, t2.status == \'active\'))\n    .JoinLateral(sq, True)\n    .LeftJoinLateral(sq, sq.name != \'test\')\n)\n```\n\n#### PARAMETERS / LITERALS\nBy default, all values are considered as parameters. \nIf you need to cast value or add alias use Param wrapper.\nIf you need to literally insert value into sql use special Literal wrapper, \nbut be very careful - it won\'t be escaped and can lead to SQL injections. \nUse Literal only with data you can 100% trust.\n```python\nt = Table(\'tbl\')\nq = (\n    Select(t.STAR, Param(10).Cast(\'int\').As(\'added\')).From(t)\n    .Where(\n        t.id1 == 1, \n        t.id2 != Param(2).Cast(\'float\'), \n        t.id3 > Literal(3), \n        t.id4 < Literal(4).Cast(\'numeric\'),\n    )\n)\nbuild(q)\n# (\n#     \'SELECT *, $1::int AS added FROM tbl WHERE id1 == $2 AND id2 != $3::float AND id3 > 3 AND id4 < 4::numeric\',\n#     [10, 1, 2],\n# )\n```\n\n#### FUNCTIONS\nThere are `Func` and its `F` alias.\n```python\nt = Table(\'tbl\')\n\nq1 = (\n    Select(\n        F.count(\'*\'), \n        F.count(t.id).Where(t.id > 10, t.id < 20),\n        F.array_agg(t.id).OrderBy(t.id.Desc().NullsLast()).As(\'ids\'),\n    )\n    .From(t)\n)\n\nq2 = Select(t.id, F.row_number().Over(partition_by=t.status, order_by=t.id)).From(t)\n\nf = F.unnest(Literal([1, 2, 3])).As(\'idx\')\nq3 = Select(f.STAR).From(f)\n# SELECT * FROM UNNEST(ARRAY[1, 2, 3]) AS idx\n\nq4 = Select(Case((t.id == 1, \'first\'), (t.id == 2, \'second\'), Else=\'third\').As(\'val\')).From(t)\n\nq5 = Select(Array([t.id, 5, 7])).From(t)\n```\n\n#### ORDER BY / GROUP BY / HAVING / DISTINCT / DISTINCT ON\n```python\nt = Table(\'tbl\')\n\nq1 = Select(t.id.Distinct()).From(t)\n# SELECT DISTINCT id FROM tbl\n\nq2 = Select(t.STAR).From(t).OrderBy(t.id.Desc(), t.name.NullsLast())\n\nq3 = Select(F.count(\'*\')).From(t).GroupBy(t.status).Having(F.count(\'*\') > 10)\n\nq4 = Select(t.id, t.status).From(t).DistinctOn(t.status)\n# SELECT DISTINCT ON (status) id, status FROM tbl\n```\n\n#### OPERATIONS\nBasic math operator are supported out of the box: \n`+`, `-`, `*`, `/`, `>`, `>=`, `<`, `<=`. \nOthers are support as methods:\n```python\nt = Table(\'tbl\')\nq = (\n    Select(\n        t.id + t.id,\n        t.id - 1,\n        t.id * 10,\n        t.id > 15,\n        (t.id == 10).As(\'equals_ten\'),\n        (t.id != 11).As(\'not_equals_eleven\'),\n        Param(10) > 9,\n        (Literal(5) * 3.5).Cast(\'int\'),\n        t.id.Between(1, 2),\n        t.id.In([1, 2, 3]),\n        t.id.NotIn(Select(t.id).From(t).Where(t.id < 10)),\n        t.name.Is(None),\n        t.active.IsNot(False),\n        t.data.Op(\'->>\', \'key\').As(\'value1\'),\n        t.data.Op(\'#>>\', [\'key1\', \'key2\']).As(\'value2\'),\n        t.id.Any(list(range(1_000))),\n        t.name.Like(\'%ABC%\'),\n        t.name.Ilike(\'%abc%\'),\n    )\n    .From(t)\n)\n```\n\n#### INSERT\n```python\nt = Table(\'tbl\')\nq = (\n    Insert(t, columns=(t.name, t.status))\n    .Values(\n        (Param(\'some text\').Cast(\'varchar(10)\'), \'active\'),\n        (\'other text\', Literal(\'deleted\')),\n    )\n    .Returning(t.STAR)\n)\n\nbuild(q)\n# (\n#     "INSERT INTO tbl (name, status) VALUES ($1::varchar(10), $2), ($3, \'deleted\') RETURNING *",\n#     [\'some text\', \'active\', \'other text\'],\n# )\n\n# From select\nq = (\n    Insert(t, columns=(t.name, t.status))\n    .Select(\n        Select(F.concat(t.name, F.random().Cast(\'text\')), t.status)\n        .From(t)\n        .Where(t.id < 100)\n        .Limit(10)\n    )\n    .Returning(t.STAR)\n)\n\n# CTE\nsq = Select(t.STAR).From(t).Where(t.id < 100).Subquery(\'sq\')\nq = (\n    With(sq)\n    .Insert(t, (\'name\', \'status\'))\n    .From(Select(sq.name, sq.status).From(sq))\n)\n\n# Efficient bulk insert from the list of values\nvalues = [(str(i), \'active\') for i in range(1_000)]\nq = (\n    Insert(t, (\'name\', \'status\'))\n    .From(Select(\n        F.unnest(Param([name for name, _ in values]).Cast(\'text[]\')),\n        F.unnest(Param([status for _, status in values]).Cast(\'enum_status[]\')),\n    ))\n)\n```\n\n#### UPDATE / DELETE\n```python\nt = Table(\'stmh\')\nq1 = Update(t).Set({t.name: \'second\'}).Where(t.name == \'first\', t.status == \'active\').Returning(t.id)\nq2 = Delete(t).Where(t.id == 25).Returning(t.id)\n```\n\n#### Subquery / CTE\nAny Select/Insert/Update/Delete has Subquery method.\n```python\nt = Table(\'tbl\')\nsq = Select(t.id).From(t).Where(t.id < 100).Subquery(\'sq\')\n\n# Subquery\nq = Select(sq.id).From(sq).Where(sq.id > 50)\n# SELECT id FROM (SELECT id FROM tbl WHERE id < $1) As sq WHERE id > $2\n\n# CTE\nq = With(sq).Select(sq.id).From(sq).Where(sq.id > 50).Limit(2)\n# WITH sq AS (SELECT id FROM tbl WHERE id < $1) SELECT id FROM sq WHERE id > $2 LIMIT $3\n```\n\n***\n\n### Why not sqlalchemy?\n- too smart (tries to do everything: from connection/session management, to sql generating and params escaping)\n- too complex\n- too slow\n- mutable (on its core)\n\nIt is good for simple projects with simple sql queries. \nBut when your project grows up, your team grows up, sqlalchemy always leads to errors,\nunnecessary complexity, extra time your team need to spend to learn it, find not obvious bugs etc.  \n\n\n### Why not pypika?\nWhile it is much simpler then sqlalchemy, it also requires you to learn their own "sql syntax" which is not always obvious.\nAnd by default it uses parameters as literals, so it can lead to sql injections.\n\n\n***\n\nThe library is inspired by Ukraine🇺🇦 (Kyiv is my home) and its brave and free people🔱.\n\nSlava Ukraini, Heroyam slava!\n',
     'author': 'Vitalii Ponomar',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ponomar/pgmini',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
+    'python_requires': '>=3.10',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `pgmini-0.1.3/PKG-INFO` & `pgmini-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pgmini
-Version: 0.1.3
+Version: 0.1.4
 Summary: Build sql for PostgreSQL
 Home-page: https://github.com/ponomar/pgmini
 License: MIT
 Author: Vitalii Ponomar
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: attrs (>=22.2.0,<23.0.0)
+Requires-Dist: attrs (>=22.2.0)
 Description-Content-Type: text/markdown
 
 [![Test & Lint](https://github.com/ponomar/pgmini/actions/workflows/main.yml/badge.svg)](https://github.com/ponomar/pgmini/actions/workflows/main.yml)
 
 ## 🇺🇦 What is pgmini? 🇺🇦
 
 It is the PostgreSQL query builder with next core principles:
@@ -215,15 +215,15 @@
 #     ['some text', 'active', 'other text'],
 # )
 
 # From select
 q = (
     Insert(t, columns=(t.name, t.status))
     .Select(
-        Select(F.concat(t.name, F.random().Cast('text'), t.status))
+        Select(F.concat(t.name, F.random().Cast('text')), t.status)
         .From(t)
         .Where(t.id < 100)
         .Limit(10)
     )
     .Returning(t.STAR)
 )
```

