# Comparing `tmp/lccpy-1.4.4.tar.gz` & `tmp/lccpy-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lccpy-1.4.4.tar", last modified: Tue Apr 18 11:10:38 2023, max compression
+gzip compressed data, was "lccpy-1.4.5.tar", last modified: Sat Apr 22 15:47:55 2023, max compression
```

## Comparing `lccpy-1.4.4.tar` & `lccpy-1.4.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 lccpy-1.4.4/LICENSE
--rw-r--r--   0        0        0      119 2023-04-10 04:12:12.772589 lccpy-1.4.4/README.md
--rw-r--r--   0        0        0        0 2023-04-10 03:05:49.119798 lccpy-1.4.4/lccpy/__init__.py
--rw-r--r--   0        0        0      143 2023-04-11 02:41:01.880058 lccpy-1.4.4/lccpy/_mtype.py
--rw-r--r--   0        0        0    11357 2022-10-25 20:46:40.000000 lccpy-1.4.4/lccpy/asymongo/Licenses of dependent packages/motor/LICENSE
--rw-r--r--   0        0        0      168 2023-04-10 03:51:03.558895 lccpy-1.4.4/lccpy/asymongo/__init__.py
--rw-r--r--   0        0        0    20512 2023-04-11 02:42:19.557384 lccpy-1.4.4/lccpy/asymongo/_asymongo.py
--rw-r--r--   0        0        0     1070 2022-05-08 19:03:55.000000 lccpy-1.4.4/lccpy/asymysql/Licenses of dependent packages/aiomysql/LICENSE
--rw-r--r--   0        0        0       89 2023-04-10 03:50:24.852505 lccpy-1.4.4/lccpy/asymysql/__init__.py
--rw-r--r--   0        0        0    20277 2023-04-18 11:07:49.320573 lccpy-1.4.4/lccpy/asymysql/_asymysql.py
--rw-r--r--   0        0        0      273 2023-04-09 17:36:47.380717 lccpy-1.4.4/lccpy/coolfunc/__init__.py
--rw-r--r--   0        0        0     2787 2023-04-10 03:18:54.132549 lccpy-1.4.4/lccpy/coolfunc/_coolfunc.py
--rw-r--r--   0        0        0    11357 2022-11-17 21:35:25.000000 lccpy-1.4.4/lccpy/coolmongo/Licenses of dependent packages/pymongo/LICENSE
--rw-r--r--   0        0        0      169 2023-04-10 03:53:42.961556 lccpy-1.4.4/lccpy/coolmongo/__init__.py
--rw-r--r--   0        0        0    20930 2023-04-11 02:42:37.661736 lccpy-1.4.4/lccpy/coolmongo/_coolmongo.py
--rw-r--r--   0        0        0     1070 2013-11-27 14:43:24.000000 lccpy-1.4.4/lccpy/coolmysql/Licenses of dependent packages/pymysql/LICENSE
--rw-r--r--   0        0        0       90 2023-04-10 03:53:46.616102 lccpy-1.4.4/lccpy/coolmysql/__init__.py
--rw-r--r--   0        0        0    21686 2023-04-18 11:07:58.985529 lccpy-1.4.4/lccpy/coolmysql/_coolmysql.py
--rw-r--r--   0        0        0     2926 2023-01-27 23:35:02.000000 lccpy-1.4.4/lccpy/encrypt256/Licenses of dependent packages/pycryptodome/LICENSE
--rw-r--r--   0        0        0       35 2022-11-15 14:17:28.000000 lccpy-1.4.4/lccpy/encrypt256/__init__.py
--rw-r--r--   0        0        0     5141 2023-03-09 14:58:17.055833 lccpy-1.4.4/lccpy/encrypt256/_encrypt256.py
--rw-r--r--   0        0        0       35 2023-04-07 08:40:27.218236 lccpy-1.4.4/lccpy/increment/__init__.py
--rw-r--r--   0        0        0     1544 2023-04-12 06:50:22.634385 lccpy-1.4.4/lccpy/increment/_increment.py
--rw-r--r--   0        0        0       32 2023-02-19 09:41:05.530766 lccpy-1.4.4/lccpy/rstyleslice/__init__.py
--rw-r--r--   0        0        0     2903 2023-03-09 15:08:02.859531 lccpy-1.4.4/lccpy/rstyleslice/_rstyleslice.py
--rw-r--r--   0        0        0      175 2023-04-09 15:53:54.291702 lccpy-1.4.4/lccpy/vtype/__init__.py
--rw-r--r--   0        0        0     3546 2023-04-09 15:28:10.501541 lccpy-1.4.4/lccpy/vtype/_cooltime.py
--rw-r--r--   0        0        0    11771 2023-04-12 12:56:02.300717 lccpy-1.4.4/lccpy/vtype/_vtype.py
--rw-r--r--   0        0        0      573 2023-04-18 11:09:10.992464 lccpy-1.4.4/pyproject.toml
--rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 lccpy-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 lccpy-1.4.5/LICENSE
+-rw-r--r--   0        0        0      119 2023-04-10 04:12:12.772589 lccpy-1.4.5/README.md
+-rw-r--r--   0        0        0        0 2023-04-10 03:05:49.119798 lccpy-1.4.5/lccpy/__init__.py
+-rw-r--r--   0        0        0      143 2023-04-11 02:41:01.880058 lccpy-1.4.5/lccpy/_mtype.py
+-rw-r--r--   0        0        0    11357 2022-10-25 20:46:40.000000 lccpy-1.4.5/lccpy/asymongo/Licenses of dependent packages/motor/LICENSE
+-rw-r--r--   0        0        0      168 2023-04-10 03:51:03.558895 lccpy-1.4.5/lccpy/asymongo/__init__.py
+-rw-r--r--   0        0        0    20512 2023-04-11 02:42:19.557384 lccpy-1.4.5/lccpy/asymongo/_asymongo.py
+-rw-r--r--   0        0        0     1070 2022-05-08 19:03:55.000000 lccpy-1.4.5/lccpy/asymysql/Licenses of dependent packages/aiomysql/LICENSE
+-rw-r--r--   0        0        0       89 2023-04-10 03:50:24.852505 lccpy-1.4.5/lccpy/asymysql/__init__.py
+-rw-r--r--   0        0        0    22806 2023-04-19 04:50:36.901729 lccpy-1.4.5/lccpy/asymysql/_asymysql.py
+-rw-r--r--   0        0        0      273 2023-04-09 17:36:47.380717 lccpy-1.4.5/lccpy/coolfunc/__init__.py
+-rw-r--r--   0        0        0     2787 2023-04-10 03:18:54.132549 lccpy-1.4.5/lccpy/coolfunc/_coolfunc.py
+-rw-r--r--   0        0        0    11357 2022-11-17 21:35:25.000000 lccpy-1.4.5/lccpy/coolmongo/Licenses of dependent packages/pymongo/LICENSE
+-rw-r--r--   0        0        0      169 2023-04-10 03:53:42.961556 lccpy-1.4.5/lccpy/coolmongo/__init__.py
+-rw-r--r--   0        0        0    20930 2023-04-11 02:42:37.661736 lccpy-1.4.5/lccpy/coolmongo/_coolmongo.py
+-rw-r--r--   0        0        0     1070 2013-11-27 14:43:24.000000 lccpy-1.4.5/lccpy/coolmysql/Licenses of dependent packages/pymysql/LICENSE
+-rw-r--r--   0        0        0       90 2023-04-10 03:53:46.616102 lccpy-1.4.5/lccpy/coolmysql/__init__.py
+-rw-r--r--   0        0        0    22832 2023-04-19 07:49:15.385992 lccpy-1.4.5/lccpy/coolmysql/_coolmysql.py
+-rw-r--r--   0        0        0     2926 2023-01-27 23:35:02.000000 lccpy-1.4.5/lccpy/encrypt256/Licenses of dependent packages/pycryptodome/LICENSE
+-rw-r--r--   0        0        0       35 2022-11-15 14:17:28.000000 lccpy-1.4.5/lccpy/encrypt256/__init__.py
+-rw-r--r--   0        0        0     5141 2023-03-09 14:58:17.055833 lccpy-1.4.5/lccpy/encrypt256/_encrypt256.py
+-rw-r--r--   0        0        0       35 2023-04-07 08:40:27.218236 lccpy-1.4.5/lccpy/increment/__init__.py
+-rw-r--r--   0        0        0     1544 2023-04-12 06:50:22.634385 lccpy-1.4.5/lccpy/increment/_increment.py
+-rw-r--r--   0        0        0       32 2023-02-19 09:41:05.530766 lccpy-1.4.5/lccpy/rstyleslice/__init__.py
+-rw-r--r--   0        0        0     2903 2023-03-09 15:08:02.859531 lccpy-1.4.5/lccpy/rstyleslice/_rstyleslice.py
+-rw-r--r--   0        0        0      175 2023-04-09 15:53:54.291702 lccpy-1.4.5/lccpy/vtype/__init__.py
+-rw-r--r--   0        0        0     3546 2023-04-09 15:28:10.501541 lccpy-1.4.5/lccpy/vtype/_cooltime.py
+-rw-r--r--   0        0        0    11771 2023-04-12 12:56:02.300717 lccpy-1.4.5/lccpy/vtype/_vtype.py
+-rw-r--r--   0        0        0      573 2023-04-22 15:38:43.104610 lccpy-1.4.5/pyproject.toml
+-rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 lccpy-1.4.5/PKG-INFO
```

### Comparing `lccpy-1.4.4/LICENSE` & `lccpy-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.4/lccpy/asymongo/Licenses of dependent packages/motor/LICENSE` & `lccpy-1.4.5/lccpy/asymongo/Licenses of dependent packages/motor/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.4/lccpy/asymongo/_asymongo.py` & `lccpy-1.4.5/lccpy/asymongo/_asymongo.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.4/lccpy/asymysql/Licenses of dependent packages/aiomysql/LICENSE` & `lccpy-1.4.5/lccpy/asymysql/Licenses of dependent packages/aiomysql/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.4/lccpy/asymysql/_asymysql.py` & `lccpy-1.4.5/lccpy/asymysql/_asymysql.py`

 * *Files 4% similar despite different names*

```diff
@@ -245,20 +245,20 @@
 
 
 class sheetORM():
     _variable = True
     _pk = ''
 
     def __init__(self, connPool:ToolPool, dbName:str, sheetName:str, where=None, columns='*', _sort=None):
-        if not columns: ValueError('columns 不能为空')
+        assert columns  # 不能为空
+        self.columns = columns  # str型 或 tuple型
         self.connPool = connPool
         self.dbName = dbName
         self.sheetName = sheetName
         self.where = where or Factory(uniset)
-        self.columns = columns  # str型 或 tuple型
         self._sort = deepcopy(_sort or {})
             # {A:True, B:False, C:1, D:0}
             # bool(value) == True --> 升序
             # bool(value) == False --> 降序
         self._variable = False
 
     def __setattr__(self, name, value):
@@ -284,14 +284,82 @@
             return ' order by ' + ', '.join([k if v else f"{k} desc" for k,v in self._sort.items()])
         return ''
 
     def _ParseColumns(self):
         if type(self.columns) is str:
             return self.columns
         return ', '.join(self.columns)
+    
+    async def update_by_pk(self, data:dict):
+        pk = await self.getPK()
+        records = {}
+        for key, line in data.items():
+            for field, value in line.items():
+                records.setdefault(field, {})[key] = value
+        blocks = []
+        for field, kvs in records.items():
+            s = [f"{field} = ", '    case']
+            for k, v in kvs.items():
+                s.append(f"        when {pk} = {jsonChinese(k)} then {jsonChinese(v)}")
+            s.append(f"else {field}")
+            s.append('end')
+            blocks.append('\n'.join(s))
+        blocks = ' ,\n'.join(blocks)
+        sql = f"update {self.sheetName} set \n{blocks}"
+        r, cursor = await self.execute(sql=sql)
+        return cursor
+    
+    def apply(self, handler):
+        return makeSlice(self._applyBase, handler=handler)
+    
+    async def _applyBase(self, key, handler):
+        pk = await self.getPK()
+        # 添加主键字段
+        cols = raw_columns = self.columns
+        if isinstance(cols, str): cols = [cols]
+        for x in cols:
+            if x.strip() in ('*', pk):
+                break
+        else:
+            self.columns = tuple(list(cols) + [pk])
+        # 从数据库提取数据
+        lines = await self[key]
+        object.__setattr__(self, 'columns', raw_columns)  # 恢复用户设定的columns
+        if type(lines) is dict:
+            lines = [lines]
+            r_type = 'dict'
+        else:
+            r_type = 'list'
+        # 处理数据
+        records = {}
+        for line in lines:
+            key = line[pk]
+            line2 = line.copy()
+            handler(line)
+            for k, v in line.items():
+                if v != line2.get(k, SysEmpty):
+                    records.setdefault(k, {})[key] = v
+        if r_type == 'dict':
+            lines = lines[0]
+        # 更新到数据库
+        if records:
+            blocks = []
+            for field, kvs in records.items():
+                s = [f"{field} = ", '    case']
+                for k, v in kvs.items():
+                    s.append(f"        when {pk} = {jsonChinese(k)} then {jsonChinese(v)}")
+                s.append(f"else {field}")
+                s.append('end')
+                blocks.append('\n'.join(s))
+            blocks = ' ,\n'.join(blocks)
+            sql = f"update {self.sheetName} set \n{blocks}"
+            await self.execute(sql=sql)
+            return dict(data=lines)
+        else:
+            return dict(data=lines)
 
     def order(self, **rule): return self._copy(_sort={**rule})
 
     async def insert(self, data):
         if type(data) is dict:
             cols = data.keys()
             sql = f"insert into {self.sheetName}({', '.join(cols)}) values ({', '.join(('%s',)*len(cols))})"
```

### Comparing `lccpy-1.4.4/lccpy/coolfunc/_coolfunc.py` & `lccpy-1.4.5/lccpy/coolfunc/_coolfunc.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.4/lccpy/coolmongo/Licenses of dependent packages/pymongo/LICENSE` & `lccpy-1.4.5/lccpy/coolmongo/Licenses of dependent packages/pymongo/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.4/lccpy/coolmongo/_coolmongo.py` & `lccpy-1.4.5/lccpy/coolmongo/_coolmongo.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.4/lccpy/coolmysql/Licenses of dependent packages/pymysql/LICENSE` & `lccpy-1.4.5/lccpy/coolmysql/Licenses of dependent packages/pymysql/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.4/lccpy/coolmysql/_coolmysql.py` & `lccpy-1.4.5/lccpy/coolmysql/_coolmysql.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,14 +283,33 @@
         return ''
 
     def _ParseColumns(self):
         if type(self.columns) is str:
             return self.columns
         return ', '.join(self.columns)
     
+    def update_by_pk(self, data:dict):
+        pk = self.getPK()
+        records = {}
+        for key, line in data.items():
+            for field, value in line.items():
+                records.setdefault(field, {})[key] = value
+        blocks = []
+        for field, kvs in records.items():
+            s = [f"{field} = ", '    case']
+            for k, v in kvs.items():
+                s.append(f"        when {pk} = {jsonChinese(k)} then {jsonChinese(v)}")
+            s.append(f"else {field}")
+            s.append('end')
+            blocks.append('\n'.join(s))
+        blocks = ' ,\n'.join(blocks)
+        sql = f"update {self.sheetName} set \n{blocks}"
+        r, cursor = self.execute(sql=sql)
+        return cursor
+
     def apply(self, handler):
         return makeSlice(self._applyBase, handler=handler)
     
     def _applyBase(self, key, handler):
         pk = self.getPK()
         # 添加主键字段
         cols = raw_columns = self.columns
@@ -351,15 +370,15 @@
             sql = f"insert into {self.sheetName}({', '.join(cols)}) values ({', '.join(('%s',)*len(cols))})"
             data = tuple(tuple(x.get(k) for k in cols) for x in data)
             r, cursor = self.executemany(sql, data)
             return cursor
 
     def delete(self):
         return makeSlice(self._deleteBase)
-    
+        
     def _deleteBase(self, key):
         # [::]
         if isinstance(key, slice):
             L, R, S = key.start, key.stop, key.step or 1
             if S in [None,1]:
                 if (L in [None,1] and R in [None,-1]) or (L == -1 and R == 1):
                     rdata, cursor = self.execute(f"delete from {self.sheetName}{self.where}")
@@ -383,15 +402,15 @@
                     rdata, cursor = self.execute(f"delete from {self.sheetName} where 1 = 2")
             else:
                 rdata, cursor = self.execute(f"delete from {self.sheetName}{mc[pk] == pks[pk]} limit 1")
         return cursor
 
     def update(self, data):
         return makeSlice(self._updateBase, data=data)
-
+    
     def _updateBase(self, key, data:dict):
         data = ', '.join([f"{k}={v.field}" if isinstance(v,Filter) else f"{k}={jsonChinese(v)}" for k,v in data.items()])
         # [::]
         if isinstance(key, slice):
             L, R, S = key.start, key.stop, key.step or 1
             if S in [None,1]:
                 if (L in [None,1] and R in [None,-1]) or (L == -1 and R == 1):
@@ -479,15 +498,15 @@
     def __setitem__(self, key, value):
         if value is None:
             self._deleteBase(key)
         elif isinstance(value, dict):
             self._updateBase(key, data=value)
         else:
             raise TypeError(key)
-
+    
     def __getitem__(self, key):
         # 索引取值
         if isinstance(key, int):
             index = key
             if index < 0: index = len(self) + index + 1  # R索引
             if index < 1: raise MgIndexError(f"index({key}) out of range")
             skip = index - 1
@@ -545,14 +564,20 @@
             return self._copy(where=self.where & key)
         raise TypeError(key)
     
     def close(self):
         obj = self.connPool.get()
         r = obj['conn'].close()
         return r or True
+    
+    def _native(self): return f"select {self._ParseColumns()} from {self.sheetName}{self.where}{self._ParseOrder()}"
+    def _deleteNative(self): return f"delete from {self.sheetName}{self.where}"
+    def _updateNative(self, data:dict={}):
+        data = ', '.join([f"{k}={v}" for k,v in data.items()]) or '____'
+        return f"update {self.sheetName} set {data}{self.where}"
 
 
 class MysqlColumn():
     id = None  # 字段提示
     def __getattribute__(self, field):
         return Filter(field=field)
     __getitem__ = __getattribute__
```

### Comparing `lccpy-1.4.4/lccpy/encrypt256/Licenses of dependent packages/pycryptodome/LICENSE` & `lccpy-1.4.5/lccpy/encrypt256/Licenses of dependent packages/pycryptodome/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.4/lccpy/encrypt256/_encrypt256.py` & `lccpy-1.4.5/lccpy/encrypt256/_encrypt256.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.4/lccpy/increment/_increment.py` & `lccpy-1.4.5/lccpy/increment/_increment.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.4/lccpy/rstyleslice/_rstyleslice.py` & `lccpy-1.4.5/lccpy/rstyleslice/_rstyleslice.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.4/lccpy/vtype/_cooltime.py` & `lccpy-1.4.5/lccpy/vtype/_cooltime.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.4/lccpy/vtype/_vtype.py` & `lccpy-1.4.5/lccpy/vtype/_vtype.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.4/pyproject.toml` & `lccpy-1.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "lccpy"
-version = "1.4.4"
+version = "1.4.5"
 description = "The dependent package of project <Make Python simpler> ."
 dependencies = ["motor", "aiomysql", "pymongo", "pymysql", "pycryptodome"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
```

### Comparing `lccpy-1.4.4/PKG-INFO` & `lccpy-1.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lccpy
-Version: 1.4.4
+Version: 1.4.5
 Summary: The dependent package of project <Make Python simpler> .
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: motor
 Requires-Dist: aiomysql
```

