# Comparing `tmp/gqylpy_dict-1.1.4.tar.gz` & `tmp/gqylpy_dict-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gqylpy_dict-1.1.4.tar", last modified: Sun Jan 15 09:41:54 2023, max compression
+gzip compressed data, was "gqylpy_dict-1.2.tar", last modified: Sat Apr 22 03:59:15 2023, max compression
```

## Comparing `gqylpy_dict-1.1.4.tar` & `gqylpy_dict-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 09:41:54.424021 gqylpy_dict-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    12343 2023-01-15 09:41:43.000000 gqylpy_dict-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-01-15 09:41:43.000000 gqylpy_dict-1.1.4/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-01-15 09:41:54.424021 gqylpy_dict-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-01-15 09:41:43.000000 gqylpy_dict-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 09:41:54.424021 gqylpy_dict-1.1.4/gqylpy_dict/
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-01-15 09:41:43.000000 gqylpy_dict-1.1.4/gqylpy_dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-01-15 09:41:43.000000 gqylpy_dict-1.1.4/gqylpy_dict/g dict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 09:41:54.424021 gqylpy_dict-1.1.4/gqylpy_dict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-01-15 09:41:54.000000 gqylpy_dict-1.1.4/gqylpy_dict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-01-15 09:41:54.000000 gqylpy_dict-1.1.4/gqylpy_dict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-15 09:41:54.000000 gqylpy_dict-1.1.4/gqylpy_dict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-15 09:41:54.000000 gqylpy_dict-1.1.4/gqylpy_dict.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-15 09:41:54.424021 gqylpy_dict-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-01-15 09:41:43.000000 gqylpy_dict-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 03:59:15.338949 gqylpy_dict-1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    12343 2023-04-22 03:59:04.000000 gqylpy_dict-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-22 03:59:04.000000 gqylpy_dict-1.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-22 03:59:15.338949 gqylpy_dict-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-22 03:59:04.000000 gqylpy_dict-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 03:59:15.338949 gqylpy_dict-1.2/gqylpy_dict/
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-04-22 03:59:04.000000 gqylpy_dict-1.2/gqylpy_dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-04-22 03:59:04.000000 gqylpy_dict-1.2/gqylpy_dict/g dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 03:59:15.338949 gqylpy_dict-1.2/gqylpy_dict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-22 03:59:15.000000 gqylpy_dict-1.2/gqylpy_dict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-22 03:59:15.000000 gqylpy_dict-1.2/gqylpy_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 03:59:15.000000 gqylpy_dict-1.2/gqylpy_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-22 03:59:15.000000 gqylpy_dict-1.2/gqylpy_dict.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 03:59:15.338949 gqylpy_dict-1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-22 03:59:04.000000 gqylpy_dict-1.2/setup.py
```

### Comparing `gqylpy_dict-1.1.4/LICENSE` & `gqylpy_dict-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gqylpy_dict-1.1.4/NOTICE` & `gqylpy_dict-1.2/NOTICE`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Copyright (c) 2022, 2023 GQYLPY <http://gqylpy.com>. All rights reserved.
 gqylpy-dict is released under the dual license WTFPL and Apache-2.0.
 
 ────────────────────────────────────────────────────────────────────────────────
-Lines 48-93 in the "gqylpy_dict/g dict.py" file are licensed under Apache-2.0:
+
+Lines 51-95 in the "gqylpy_dict/g dict.py" file are licensed under Apache-2.0:
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `gqylpy_dict-1.1.4/PKG-INFO` & `gqylpy_dict-1.2/gqylpy_dict.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gqylpy_dict
-Version: 1.1.4
+Name: gqylpy-dict
+Version: 1.2
 Summary: 基于内置 dict，它是对内置 dict 的增强。dict 能做的它能做，dict 不能做的它更能做。
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: WTFPL,Apache-2.0
 Project-URL: Source, https://github.com/gqylpy/gqylpy-dict
 Classifier: Environment :: Web Environment
```

### Comparing `gqylpy_dict-1.1.4/README.md` & `gqylpy_dict-1.2/README.md`

 * *Files identical despite different names*

### Comparing `gqylpy_dict-1.1.4/gqylpy_dict/g dict.py` & `gqylpy_dict-1.2/gqylpy_dict/g dict.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Copyright (c) 2022, 2023 GQYLPY <http://gqylpy.com>. All rights reserved.
 
 ────────────────────────────────────────────────────────────────────────────────
 
-Lines 48 through 93 is licensed under the Apache-2.0:
+Lines 51 through 95 is licensed under the Apache-2.0:
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         https://www.apache.org/licenses/LICENSE-2.0
 
@@ -34,19 +34,22 @@
    TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION
 
   0. You just DO WHAT THE FUCK YOU WANT TO.
 
 ────────────────────────────────────────────────────────────────────────────────
 """
 import re
+import sys
 import builtins
 
-from typing import Optional, Union, Tuple, Type, Generator, Iterator, Any
+from copy import copy, deepcopy
 
-unique = b'GQYLPY, \xe6\x94\xb9\xe5\x8f\x98\xe4\xb8\x96\xe7\x95\x8c\xe3\x80\x82'
+from typing import Type, Final, Optional, Union, Tuple, List, Hashable, Any
+
+__unique__: Final = object()
 
 
 class MasqueradeClass(type):
     """Masquerade one class as another.
     Warning, masquerade the class can cause unexpected problems, use caution."""
     __module__ = 'builtins'
 
@@ -54,15 +57,15 @@
         try:
             __masquerade_class__ = __dict__['__masquerade_class__']
         except KeyError:
             raise AttributeError(
                 f'instance of "{mcs.__name__}" must '
                 'define "__masquerade_class__" attribute, '
                 'use to specify the class to disguise.'
-            )
+            ) from None
 
         if not isinstance(__masquerade_class__, type):
             raise TypeError('"__masquerade_class__" is not a class.')
 
         cls = type.__new__(
             mcs, __masquerade_class__.__name__, __bases__, __dict__
         )
@@ -77,126 +80,127 @@
         if getattr(builtins, __masquerade_class__.__name__, None) is \
                 __masquerade_class__:
             setattr(builtins, __name__, cls)
 
         return cls
 
     def __hash__(cls):
-        # return hash(cls.__masquerade_class__)
-        # Warning: If masquerade the hash value, will not get the result from
-        # `copy.copy` and `copy.deepcopy` correctly.
-        return super().__hash__()
+        if sys._getframe(1).f_code in (deepcopy.__code__, copy.__code__):
+            return type.__hash__(cls)
+        return hash(cls.__masquerade_class__)
 
-    def __eq__(cls, o):
-        return True if o is cls.__masquerade_class__ else super().__eq__(o)
+    def __eq__(cls, o) -> bool:
+        return True if o is cls.__masquerade_class__ else type.__eq__(cls, o)
 
 
 builtins.MasqueradeClass = MasqueradeClass
 
 
 class GqylpyDict(dict, metaclass=MasqueradeClass):
     __masquerade_class__ = dict
-    __isabstractmethod__ = False
     __slots__ = ()
 
-    def __init__(self, __data__=None, /, **kw):
-        if isinstance(__data__, dict):
-            kw and __data__.update(kw)
+    def __init__(self, __data__=None, /, **data):
+        if __data__ is None:
+            __data__ = data
         else:
-            __data__ = kw
+            __data__.update(data)
 
         for name, value in __data__.items():
-            self[name] = GqylpyDict(value)
+            dict.__setitem__(self, name, GqylpyDict(value))
 
-    def __new__(cls, __data__={}, /, **kw):
+    def __new__(cls, __data__={}, /, **data):
         if isinstance(__data__, dict):
-            return dict.__new__(cls)
+            return __data__ if __data__.__class__ is cls else dict.__new__(cls)
 
-        if isinstance(__data__, (list, tuple, set, frozenset, Iterator)):
-            return [cls(v) for v in __data__]
+        if isinstance(__data__, (list, tuple, set, frozenset)):
+            return __data__.__class__(cls(v) for v in __data__)
 
         return __data__
 
-    def __getattr__(self, name: str) -> Any:
+    def __getattr__(self, name: str, /) -> Any:
         return self[name]
 
-    def __setattr__(self, name: str, value: Any) -> None:
+    def __setattr__(self, name: str, value: Any, /) -> None:
         self[name] = value
 
-    def __delattr__(self, name: str) -> None:
+    def __delattr__(self, name: str, /) -> None:
         del self[name]
 
-    def __setitem__(self, name: Any, value: Any) -> None:
+    def __setitem__(self, name: Hashable, value: Any, /) -> None:
         dict.__setitem__(self, name, GqylpyDict(value))
 
-    def __deepcopy__(self, memo=None) -> 'GqylpyDict':
-        return GqylpyDict(self)
-
-    def __hash__(self):
+    def __hash__(self) -> int:
         return -2
 
     def __reduce__(self) -> Tuple[Type['GqylpyDict'], Tuple[dict]]:
         return GqylpyDict, (dict(self),)
 
     def copy(self) -> 'GqylpyDict':
-        x = GqylpyDict()
-        for k, v in self.items():
-            x[k] = v
-        return x
+        copied = GqylpyDict()
+        for name, value in self.items():
+            dict.__setitem__(copied, name, value)
+        return copied
 
-    def update(self, __data__: dict = {}, /, **kw) -> None:
+    def update(self, __data__: Optional[dict] = None, /, **data) -> None:
         try:
-            super().update(GqylpyDict(__data__, **kw))
+            dict.update(self, GqylpyDict(
+                *() if __data__ is None else (__data__,), **data
+            ))
         except (TypeError, ValueError):
             x: str = __data__.__class__.__name__
-            raise TypeError(f'updated object must be a "dict", not "{x}".')
+            raise TypeError(
+                f'updated object must be a "dict", not "{x}".'
+            ) from None
 
     def deepget(
             self,
-            keypath: str,
+            deepkey: str,
             /,
-            default: Optional[Any]      = None,
+            default: Optional[Any]                = None,
             *,
-            ignore:  Union[tuple, list] = ()
+            ignore:  Union[Tuple[Any], List[Any]] = ()
     ) -> Any:
-        keypath = keypath[:-1] if keypath and keypath[-1] == ']' else keypath
+        deepkey = deepkey[:-1] if deepkey and deepkey[-1] == ']' else deepkey
         value = self
 
-        for key in re.split(r'\.|\[|][.\[]', keypath):
-            if value.__class__ is list:
+        for key in re.split(r'\.|\[|][.\[]', deepkey):
+            if isinstance(value, (list, tuple)):
                 try:
                     key = int(key)
                 except ValueError:
                     return default
             try:
                 value = value[key]
             except KeyError:
                 try:
                     if key.isdigit() or key[0] == '-' and key[1:].isdigit():
                         value = value[int(key)]
-                    elif key == 'None':
-                        value = value[None]
+                    elif key in ('None', 'True', 'False', 'Ellipsis'):
+                        value = value[eval(key)]
                     else:
                         return default
                 except (KeyError, IndexError):
                     return default
             except (IndexError, TypeError):
                 return default
 
         return default if value in ignore else value
 
-    def deepset(self, keypath: str, value: Any) -> None:
-        existing_keys, nonexistent_keys = re.split(r'[.\[]', keypath), []
+    def deepset(self, deepkey: str, value: Any) -> None:
+        existing_keys, nonexistent_keys = re.split(r'[.\[]', deepkey), []
         last_key: str = int_key(existing_keys.pop())
 
         while existing_keys:
-            data = GqylpyDict.deepget(self, '.'.join(existing_keys), unique)
+            data = GqylpyDict.deepget(self, '.'.join(existing_keys), __unique__)
+            # Why `GqylpyDict.deepget`? Compatible with built-in dict instance.
+
             key: str = int_key(existing_keys.pop())
 
-            if data is not unique:
+            if data is not __unique__:
                 try:
                     next_key = nonexistent_keys[0]
                 except IndexError:
                     next_key = last_key
                 if (
                         next_key.__class__ is str and not isinstance(data, dict)
                                                   or
@@ -215,104 +219,32 @@
                 next_key = nonexistent_keys[i + 1]
             except IndexError:
                 next_key = last_key
             next_data = GqylpyDict() if next_key.__class__ is str else []
             data = set_next_data(data, key, next_data)
         set_next_data(data, last_key, value)
 
-    def deepsetdefault(self, keypath: str, value: Any) -> Any:
-        result = self.deepget(keypath, unique)
-        if result is unique:
-            value = GqylpyDict(value)
-            self.deepset(keypath, value)
-            return value
-        return result
-
-    def deepcontain(self, keypath: str, /) -> bool:
-        return False if self.deepget(keypath, unique) is unique else True
-
-    def deepsetdefaultdict(self, defaultdict: dict, /) -> None:
-        for key, value in self.get_deepitems(defaultdict):
-            self.deepsetdefault(key, value)
-
-    def deepupdatedict(self, data: dict, /) -> None:
-        for key, value in self.get_deepitems(data):
-            self.deepset(key, value)
-
-    def deepkeys(self, __keypath__=None) -> Generator:
-        for key, value in self.items():
-            keypath = f'{__keypath__}.{key}' if __keypath__ else key
-
-            if isinstance(value, dict):
-                yield from GqylpyDict.deepkeys(value, keypath)
-            elif isinstance(value, (list, tuple, set, Iterator)):
-                for i, v in enumerate(value):
-                    if isinstance(v, dict):
-                        yield from GqylpyDict.deepkeys(v, f'{keypath}[{i}]')
-                    else:
-                        yield f'{keypath}[{i}]'
-            else:
-                yield keypath
-
-    def deepvalues(self, __keypath__=None) -> Generator:
-        for key, value in self.items():
-            keypath = f'{__keypath__}.{key}' if __keypath__ else key
-
-            if isinstance(value, dict):
-                yield from GqylpyDict.deepvalues(value, keypath)
-            elif isinstance(value, (list, tuple, set, Iterator)):
-                for i, v in enumerate(value):
-                    if isinstance(v, dict):
-                        yield from GqylpyDict.deepvalues(v, f'{keypath}[{i}]')
-                    else:
-                        yield v
-            else:
-                yield value
-
-    def deepitems(self, __keypath__=None) -> Generator:
-        for key, value in self.items():
-            keypath = f'{__keypath__}.{key}' if __keypath__ else key
-
-            if isinstance(value, dict):
-                yield from GqylpyDict.deepitems(value, keypath)
-            elif isinstance(value, (list, tuple, set, Iterator)):
-                for i, v in enumerate(value):
-                    if isinstance(v, dict):
-                        yield from GqylpyDict.deepitems(v, f'{keypath}[{i}]')
-                    else:
-                        yield f'{keypath}[{i}]', v
-            else:
-                yield keypath, value
-
-    @classmethod
-    def getdeep(
-            cls,
-            data:    dict,
-            keypath: str,
-            default: Optional[Any]      = None,
-            *,
-            ignore:  Union[tuple, list] = ()
-    ) -> Any:
-        return cls.deepget(data, keypath, default, ignore=ignore)
+    def deepsetdefault(self, deepkey: str, default: Any) -> Any:
+        value = GqylpyDict.deepget(self, deepkey, __unique__)
+        if value is __unique__:
+            GqylpyDict.deepset(self, deepkey, default)
+            return default
+        return value
+
+    def deepcontain(self, deepkey: str, /) -> bool:
+        return False if GqylpyDict.deepget(self, deepkey, __unique__) is \
+                        __unique__ else True
 
-    @classmethod
-    def setdeep(cls, data: dict, keypath: str, value: Any) -> None:
-        cls.deepset(data, keypath, value)
-
-    @classmethod
-    def keysdeep(cls, data: dict) -> Generator:
-        return cls.deepkeys(data)
-
-    @classmethod
-    def valuesdeep(cls, data: dict) -> Generator:
-        return cls.deepvalues(data)
-
-    @classmethod
-    def itemsdeep(cls, data: dict) -> Generator:
-        return cls.deepitems(data)
+    getdeep, setdeep = deepget, deepset
+
+    __deepcopy__ = None
+    # Compatible function `copy.deepcopy`.
+
+    __isabstractmethod__ = False
+    # Compatible metaclass `abc.ABCMeta`.
 
 
 def int_key(key: str, /) -> Union[int, str]:
     try:
         return int(key[:-1])
     except ValueError:
         return key
@@ -333,18 +265,7 @@
                 data.append(None)
             data.append(value)
         else:
             for _ in range(abs(key) - len(data) - 1):
                 data.append(None)
             data.insert(0, value)
     return data[key]
-
-
-try:
-    from yaml.representer import Representer, SafeRepresenter
-except ImportError:
-    pass
-else:
-    def represent_gdict(self, data):
-        return self.represent_mapping('tag:yaml.org,2002:map', data)
-    Representer.add_representer(GqylpyDict, represent_gdict)
-    SafeRepresenter.add_representer(GqylpyDict, represent_gdict)
```

### Comparing `gqylpy_dict-1.1.4/gqylpy_dict.egg-info/PKG-INFO` & `gqylpy_dict-1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gqylpy-dict
-Version: 1.1.4
+Name: gqylpy_dict
+Version: 1.2
 Summary: 基于内置 dict，它是对内置 dict 的增强。dict 能做的它能做，dict 不能做的它更能做。
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: WTFPL,Apache-2.0
 Project-URL: Source, https://github.com/gqylpy/gqylpy-dict
 Classifier: Environment :: Web Environment
```

### Comparing `gqylpy_dict-1.1.4/setup.py` & `gqylpy_dict-1.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,30 +5,27 @@
     for line in f:
         if line.startswith('@version: ', 4):
             version = line.split()[-1]
             break
     author, email = f.readline().split(maxsplit=1)[-1].rstrip().split()
     source = f.readline().split()[-1]
 
-with open('README.md', encoding='utf8') as f:
-    long_description = f.read()
-
 setuptools.setup(
-    name=g.__name__,
+    name=g.__package__,
     version=version,
     author=author,
     author_email=email,
     license='WTFPL,Apache-2.0',
     url='http://gqylpy.com',
     project_urls={'Source': source},
-    description='基于内置 dict，它是对内置 dict 的增强。dict 能做的它能做，dict 不能做的'
-                '它更能做。',
-    long_description=long_description,
+    description='基于内置 dict，它是对内置 dict 的增强。dict 能做的它能做，dict 不能做'
+                '的它更能做。',
+    long_description=open('README.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
-    packages=[g.__name__],
+    packages=[g.__package__],
     python_requires='>=3.8, <4',
     classifiers=[
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
         'Topic :: Text Processing :: Indexing',
         'Topic :: Utilities',
```

