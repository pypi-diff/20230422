# Comparing `tmp/fastqueue-lib-0.0.3.tar.gz` & `tmp/fastqueue-lib-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastqueue-lib-0.0.3.tar", last modified: Sat Apr 15 18:11:25 2023, max compression
+gzip compressed data, was "fastqueue-lib-0.0.4.tar", last modified: Sat Apr 22 00:23:21 2023, max compression
```

## Comparing `fastqueue-lib-0.0.3.tar` & `fastqueue-lib-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:11:25.428902 fastqueue-lib-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-15 18:11:09.000000 fastqueue-lib-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-15 18:11:09.000000 fastqueue-lib-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-04-15 18:11:25.424902 fastqueue-lib-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-15 18:11:09.000000 fastqueue-lib-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:11:25.424902 fastqueue-lib-0.0.3/fastqueue/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-15 18:11:09.000000 fastqueue-lib-0.0.3/fastqueue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-15 18:11:09.000000 fastqueue-lib-0.0.3/fastqueue/prototypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:11:25.424902 fastqueue-lib-0.0.3/fastqueue_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-04-15 18:11:25.000000 fastqueue-lib-0.0.3/fastqueue_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-15 18:11:25.000000 fastqueue-lib-0.0.3/fastqueue_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 18:11:25.000000 fastqueue-lib-0.0.3/fastqueue_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-15 18:11:25.000000 fastqueue-lib-0.0.3/fastqueue_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-15 18:11:25.000000 fastqueue-lib-0.0.3/fastqueue_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-15 18:11:09.000000 fastqueue-lib-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 18:11:25.428902 fastqueue-lib-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-15 18:11:09.000000 fastqueue-lib-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:11:25.424902 fastqueue-lib-0.0.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-04-15 18:11:09.000000 fastqueue-lib-0.0.3/src/ccqueue.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-15 18:11:09.000000 fastqueue-lib-0.0.3/src/cllqueue.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    18942 2023-04-15 18:11:09.000000 fastqueue-lib-0.0.3/src/fastqueue.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:11:25.424902 fastqueue-lib-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-15 18:11:09.000000 fastqueue-lib-0.0.3/tests/test_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:23:21.707372 fastqueue-lib-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-22 00:23:06.000000 fastqueue-lib-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-22 00:23:06.000000 fastqueue-lib-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-22 00:23:21.707372 fastqueue-lib-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-22 00:23:06.000000 fastqueue-lib-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:23:21.707372 fastqueue-lib-0.0.4/fastqueue/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-22 00:23:06.000000 fastqueue-lib-0.0.4/fastqueue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-04-22 00:23:06.000000 fastqueue-lib-0.0.4/fastqueue/prototypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:23:21.707372 fastqueue-lib-0.0.4/fastqueue_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-22 00:23:21.000000 fastqueue-lib-0.0.4/fastqueue_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-22 00:23:21.000000 fastqueue-lib-0.0.4/fastqueue_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 00:23:21.000000 fastqueue-lib-0.0.4/fastqueue_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-22 00:23:21.000000 fastqueue-lib-0.0.4/fastqueue_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-22 00:23:21.000000 fastqueue-lib-0.0.4/fastqueue_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-22 00:23:06.000000 fastqueue-lib-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 00:23:21.707372 fastqueue-lib-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-22 00:23:06.000000 fastqueue-lib-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:23:21.707372 fastqueue-lib-0.0.4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-04-22 00:23:06.000000 fastqueue-lib-0.0.4/src/ccqueue.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-22 00:23:06.000000 fastqueue-lib-0.0.4/src/cllqueue.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25282 2023-04-22 00:23:06.000000 fastqueue-lib-0.0.4/src/fastqueue.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:23:21.707372 fastqueue-lib-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-22 00:23:06.000000 fastqueue-lib-0.0.4/tests/test_queue.py
```

### Comparing `fastqueue-lib-0.0.3/LICENSE` & `fastqueue-lib-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastqueue-lib-0.0.3/PKG-INFO` & `fastqueue-lib-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastqueue-lib
-Version: 0.0.3
+Version: 0.0.4
 Summary: Fast single ended queue library for python
 Author-email: Matthew Taylor <matthew.taylor.andre@gmail.com>
 Project-URL: Homepage, https://github.com/MatthewAndreTaylor/mqueue
 Keywords: Queue
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -20,17 +20,17 @@
 Provides-Extra: examples
 Provides-Extra: tests
 License-File: LICENSE
 
 # fastqueue
 
 [![Tests](https://github.com/MatthewAndreTaylor/fastqueue/actions/workflows/tests.yml/badge.svg)](https://github.com/MatthewAndreTaylor/fastqueue/actions)
-[![PyPI Versions](https://img.shields.io/badge/python-3.9%2B-blue)](https://github.com/MatthewAndreTaylor/fastqueue/blob/master/pyproject.toml)
+[![PyPI versions](https://img.shields.io/badge/python-3.9%2B-blue)](https://github.com/MatthewAndreTaylor/fastqueue/)
 [![PyPI license](https://img.shields.io/badge/license-MIT-%23373737)](https://github.com/MatthewAndreTaylor/fastqueue/blob/master/LICENSE)\
-[![PyPI](https://img.shields.io/badge/pypi-v0.0.1-blue)](https://pypi.org/project/fastqueue-lib/)
+[![PyPI](https://img.shields.io/pypi/v/fastqueue-lib.svg)](https://pypi.org/project/fastqueue-lib/)
 
 
 Single ended fast queue's built in C tuned for python.
 
 ## Requirements
 
 - `python 3.9+`
@@ -86,12 +86,15 @@
 >>> queue_c.enqueue('🚗')
 >>> queue_c[-1]
 '🚗'
 >>> [queue_c.dequeue() for _ in range(len(queue_c)) ]
 ['🚒', '🛴', '🚅', '🚗']
 ```
 
+Another alternative is `fastqueue.LockQueue()` which supports all queue operations.
+`fastqueue.LockQueue()` is built as a thread-safe alternative to the other queue types.
+
 ## Example Benchmarks
 ![Queue_times](https://user-images.githubusercontent.com/100451342/232172485-c17b6b33-986f-461b-b0bf-b26b3f6e8304.png)
 ![Queue_types](https://user-images.githubusercontent.com/100451342/232172490-bd90b021-7aeb-47b8-99e0-2481ccbc1f8f.png)
```

### Comparing `fastqueue-lib-0.0.3/README.md` & `fastqueue-lib-0.0.4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # fastqueue
 
 [![Tests](https://github.com/MatthewAndreTaylor/fastqueue/actions/workflows/tests.yml/badge.svg)](https://github.com/MatthewAndreTaylor/fastqueue/actions)
-[![PyPI Versions](https://img.shields.io/badge/python-3.9%2B-blue)](https://github.com/MatthewAndreTaylor/fastqueue/blob/master/pyproject.toml)
+[![PyPI versions](https://img.shields.io/badge/python-3.9%2B-blue)](https://github.com/MatthewAndreTaylor/fastqueue/)
 [![PyPI license](https://img.shields.io/badge/license-MIT-%23373737)](https://github.com/MatthewAndreTaylor/fastqueue/blob/master/LICENSE)\
-[![PyPI](https://img.shields.io/badge/pypi-v0.0.1-blue)](https://pypi.org/project/fastqueue-lib/)
+[![PyPI](https://img.shields.io/pypi/v/fastqueue-lib.svg)](https://pypi.org/project/fastqueue-lib/)
 
 
 Single ended fast queue's built in C tuned for python.
 
 ## Requirements
 
 - `python 3.9+`
@@ -63,12 +63,15 @@
 >>> queue_c.enqueue('🚗')
 >>> queue_c[-1]
 '🚗'
 >>> [queue_c.dequeue() for _ in range(len(queue_c)) ]
 ['🚒', '🛴', '🚅', '🚗']
 ```
 
+Another alternative is `fastqueue.LockQueue()` which supports all queue operations.
+`fastqueue.LockQueue()` is built as a thread-safe alternative to the other queue types.
+
 ## Example Benchmarks
 ![Queue_times](https://user-images.githubusercontent.com/100451342/232172485-c17b6b33-986f-461b-b0bf-b26b3f6e8304.png)
 ![Queue_types](https://user-images.githubusercontent.com/100451342/232172490-bd90b021-7aeb-47b8-99e0-2481ccbc1f8f.png)
```

### Comparing `fastqueue-lib-0.0.3/fastqueue/prototypes.py` & `fastqueue-lib-0.0.4/fastqueue/prototypes.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,25 +4,22 @@
 
 
 # Matt's Linked List Queue
 class LLNode(Structure):
     pass
 
 
-LLNode._fields_ = [
-    ('val', py_object),
-    ('next', POINTER(LLNode))
-]
+LLNode._fields_ = [("val", py_object), ("next", POINTER(LLNode))]
 
 
 class LLNodeQueue(Structure):
     _fields_ = [
-        ('front', POINTER(LLNode)),
-        ('back', POINTER(LLNode)),
-        ('length', c_uint)
+        ("front", POINTER(LLNode)),
+        ("back", POINTER(LLNode)),
+        ("length", c_uint),
     ]
 
 
 __libfile = Path(__file__).parent / "cllqueue.so"
 llqueue_lib = CDLL(str(__libfile))
 
 llqueue_lib.new_node_queue.argtypes = []
@@ -69,19 +66,19 @@
     def __del__(self):
         llqueue_lib.free_q(self.queue)
 
 
 # Matt's Contiguous Queue
 class ContiguousQueue(Structure):
     _fields_ = [
-        ('objects', POINTER(py_object)),
-        ('length', c_int),
-        ('capacity', c_int),
-        ('front', c_int),
-        ('back', c_int)
+        ("objects", POINTER(py_object)),
+        ("length", c_int),
+        ("capacity", c_int),
+        ("front", c_int),
+        ("back", c_int),
     ]
 
 
 __libfile = Path(__file__).parent / "ccqueue.so"
 cqueue_lib = CDLL(str(__libfile))
 
 cqueue_lib.new__queue.argtypes = []
```

### Comparing `fastqueue-lib-0.0.3/fastqueue_lib.egg-info/PKG-INFO` & `fastqueue-lib-0.0.4/fastqueue_lib.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastqueue-lib
-Version: 0.0.3
+Version: 0.0.4
 Summary: Fast single ended queue library for python
 Author-email: Matthew Taylor <matthew.taylor.andre@gmail.com>
 Project-URL: Homepage, https://github.com/MatthewAndreTaylor/mqueue
 Keywords: Queue
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -20,17 +20,17 @@
 Provides-Extra: examples
 Provides-Extra: tests
 License-File: LICENSE
 
 # fastqueue
 
 [![Tests](https://github.com/MatthewAndreTaylor/fastqueue/actions/workflows/tests.yml/badge.svg)](https://github.com/MatthewAndreTaylor/fastqueue/actions)
-[![PyPI Versions](https://img.shields.io/badge/python-3.9%2B-blue)](https://github.com/MatthewAndreTaylor/fastqueue/blob/master/pyproject.toml)
+[![PyPI versions](https://img.shields.io/badge/python-3.9%2B-blue)](https://github.com/MatthewAndreTaylor/fastqueue/)
 [![PyPI license](https://img.shields.io/badge/license-MIT-%23373737)](https://github.com/MatthewAndreTaylor/fastqueue/blob/master/LICENSE)\
-[![PyPI](https://img.shields.io/badge/pypi-v0.0.1-blue)](https://pypi.org/project/fastqueue-lib/)
+[![PyPI](https://img.shields.io/pypi/v/fastqueue-lib.svg)](https://pypi.org/project/fastqueue-lib/)
 
 
 Single ended fast queue's built in C tuned for python.
 
 ## Requirements
 
 - `python 3.9+`
@@ -86,12 +86,15 @@
 >>> queue_c.enqueue('🚗')
 >>> queue_c[-1]
 '🚗'
 >>> [queue_c.dequeue() for _ in range(len(queue_c)) ]
 ['🚒', '🛴', '🚅', '🚗']
 ```
 
+Another alternative is `fastqueue.LockQueue()` which supports all queue operations.
+`fastqueue.LockQueue()` is built as a thread-safe alternative to the other queue types.
+
 ## Example Benchmarks
 ![Queue_times](https://user-images.githubusercontent.com/100451342/232172485-c17b6b33-986f-461b-b0bf-b26b3f6e8304.png)
 ![Queue_types](https://user-images.githubusercontent.com/100451342/232172490-bd90b021-7aeb-47b8-99e0-2481ccbc1f8f.png)
```

### Comparing `fastqueue-lib-0.0.3/pyproject.toml` & `fastqueue-lib-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastqueue-lib"
-version = "0.0.3"
+version = "0.0.4"
 description="Fast single ended queue library for python"
 authors = [
     {name = "Matthew Taylor", email = "matthew.taylor.andre@gmail.com"},
 ]
 urls = {Homepage = "https://github.com/MatthewAndreTaylor/mqueue"}
 requires-python = ">=3.9"
 keywords = [ "Queue" ]
@@ -27,8 +27,8 @@
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.optional-dependencies]
 examples = [ "matplotlib" ]
-tests = [ "pytest" ]
+tests = [ "pytest" ]
```

### Comparing `fastqueue-lib-0.0.3/setup.py` & `fastqueue-lib-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `fastqueue-lib-0.0.3/src/ccqueue.cpp` & `fastqueue-lib-0.0.4/src/ccqueue.cpp`

 * *Files identical despite different names*

### Comparing `fastqueue-lib-0.0.3/src/cllqueue.cpp` & `fastqueue-lib-0.0.4/src/cllqueue.cpp`

 * *Files identical despite different names*

### Comparing `fastqueue-lib-0.0.3/src/fastqueue.c` & `fastqueue-lib-0.0.4/src/fastqueue.c`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 /**
  * Copyright (c) 2023 Matthew Andre Taylor
  */
 #include <Python.h>
+#include "pythread.h"
 
 /**
  * Single ended Contiguous Python Queue
  * --- fastqueue.QueueC ---
  */
 typedef struct {
     PyObject_VAR_HEAD
@@ -134,28 +135,28 @@
     return (Py_ssize_t)self->length;
 }
 
 static PyObject* QueueC_item(QueueC* self, Py_ssize_t index) {
     if (index < 0)
         index = index + QueueC_len(self);
     if (index >= self->length) {
-        PyErr_SetString(PyExc_IndexError, "queue index out of range");
+        PyErr_SetString(PyExc_IndexError, "Queue index out of range");
         return NULL;
     }
     PyObject* object = self->objects[(self->back + index) % self->capacity];
     Py_INCREF(object);
     return object;
 }
 
 static int QueueC_setitem(QueueC* self, Py_ssize_t index, PyObject* object) {
     if (index < 0)
         index = QueueC_len(self) + index;
 
     if (index >= self->length) {
-        PyErr_SetString(PyExc_IndexError, "queue index out of range");
+        PyErr_SetString(PyExc_IndexError, "Queue index out of range");
         return -1;
     }
 
     PyObject* oldObject = self->objects[(self->back + index) % self->capacity];
     Py_DECREF(oldObject);
     if (object == NULL) {
         self->objects[(self->back + index) % self->capacity] = Py_None;
@@ -181,15 +182,15 @@
     NULL,                                 /* sq_concat */
     NULL,                                 /* sq_repeat */
     (ssizeargfunc)QueueC_item,            /* sq_item */
     NULL,                                 /* sq_slice */
     (ssizeobjargproc)QueueC_setitem,      /* sq_as_item */
     NULL,                                 /* sq_as_slice */
     (objobjproc)QueueC_contains,          /* sq_contains */
-    (binaryfunc)QueueC_extend             /* sq_inplace_concat */
+    0                                     /* sq_inplace_concat */
 };
 
 static PyMethodDef QueueC_methods[] = {
     {"enqueue", (PyCFunction)QueueC_enqueue, METH_O, "Add an object to the front of the QueueC."},
     {"dequeue", (PyCFunction)QueueC_dequeue, METH_NOARGS, "Remove and return an object from the back of the QueueC."},
     {"is_empty", (PyCFunction)QueueC_is_empty, METH_NOARGS, "Check if the QueueC is empty."},
     {"extend", (PyCFunction)QueueC_extend, METH_O, "Add an objects from an iterator front of the QueueC."},
@@ -341,15 +342,15 @@
 
     if (self->head == NULL)
         self->tail = NULL;
 
     return py_object;
 }
 
-static int Queue_clear(Queue_t *self) {
+static int Queue_clear(Queue_t* self) {
     if (self->length == 0)
         return 0;
 
     QueueNode_t* current = self->head;
     QueueNode_t* next;
     while (current != NULL) {
         for (int i = 0; i < current->numEntries; ++i) {
@@ -412,15 +413,15 @@
 }
 
 static PyObject* Queue_item(Queue_t* self, Py_ssize_t index) {
     if (index < 0)
         index = Queue_len(self) + index;
 
     if (index >= self->length) {
-        PyErr_SetString(PyExc_IndexError, "queue index out of range");
+        PyErr_SetString(PyExc_IndexError, "Queue index out of range");
         return NULL;
     }
 
     QueueNode_t* current = self->head;
     for (int i = 0; i < (int)(index / 256); ++i) {
         current = current->next;
     }
@@ -430,15 +431,15 @@
 }
 
 static int Queue_setitem(Queue_t* self, Py_ssize_t index, PyObject* object) {
     if (index < 0)
         index = Queue_len(self) + index;
 
     if (index >= self->length) {
-        PyErr_SetString(PyExc_IndexError, "queue index out of range");
+        PyErr_SetString(PyExc_IndexError, "Queue index out of range");
         return -1;
     }
 
     QueueNode_t* current = self->head;
     for (int i = 0; i < (int)(index / 256); ++i) {
         current = current->next;
     }
@@ -463,23 +464,23 @@
         }
         current = current->next;
     }
     return 0;
 }
 
 static PySequenceMethods Queue_sequence_methods = {
-    (lenfunc)Queue_len,                  /* sq_length */
-    NULL,                                 /* sq_concat */
+    (lenfunc)Queue_len,                   /* sq_length */
+    0,                                    /* sq_concat */
     NULL,                                 /* sq_repeat */
     (ssizeargfunc)Queue_item,             /* sq_item */
     NULL,                                 /* sq_slice */
     (ssizeobjargproc)Queue_setitem,       /* sq_as_item */
     NULL,                                 /* sq_as_slice */
     (objobjproc)Queue_contains,           /* sq_contains */
-    (binaryfunc)Queue_extend              /* sq_inplace_concat */
+    0                                     /* sq_inplace_concat */
 };
 
 static PyMethodDef Queue_methods[] = {
     {"enqueue", (PyCFunction)Queue_enqueue, METH_O, enqueue_doc},
     {"dequeue", (PyCFunction)Queue_dequeue, METH_NOARGS, dequeue_doc},
     {"is_empty", (PyCFunction)Queue_is_empty, METH_NOARGS, is_empty_doc},
     {"extend", (PyCFunction)Queue_extend, METH_O, extend_doc},
@@ -525,14 +526,163 @@
     0,                                          /* tp_dictoffset */
     0,                                          /* tp_init */
     PyType_GenericAlloc,                        /* tp_alloc */
     (newfunc)Queue_new,                         /* tp_new */
     PyObject_GC_Del,                            /* tp_free */
 };
 
+typedef struct LockQueue {
+    PyObject_HEAD
+    Queue_t* queue;
+    PyThread_type_lock lock;
+} LockQueue_t;
+
+static PyObject* LockQueue_new(PyTypeObject* type, PyObject* args, PyObject* kwargs) {
+    LockQueue_t* self = (LockQueue_t*)type->tp_alloc(type, 0);
+    if (self == NULL)
+        return PyErr_NoMemory();
+
+    self->queue = (Queue_t*)Queue_new(&QueueType, args, kwargs);
+    self->lock = NULL;
+    return (PyObject*)self;
+}
+
+static int LockQueue_init(LockQueue_t* self, PyObject* args, PyObject *kwargs) {
+    self->lock = PyThread_allocate_lock();
+    if (self == NULL) {
+        PyErr_SetString(PyExc_MemoryError, "Could not allocate thread lock.");
+        return -1;
+    }
+    return 0;
+}
+
+static void LockQueue_dealloc(LockQueue_t* self) {
+    PyThread_free_lock(self->lock);
+    Py_TYPE(self)->tp_free((PyObject*)self);
+}
+
+static int LockQueue_traverse(LockQueue_t* self, visitproc visit, void* arg) {
+    return Queue_traverse(self->queue, visit, arg);
+}
+
+static int LockQueue_clear(LockQueue_t* self) {
+    return Queue_clear(self->queue);
+}
+
+static PyObject* LockQueue_call_with_lock(LockQueue_t* self, PyObject* args, PyObject* (*func)(Queue_t*, PyObject*)) {
+    PyThread_acquire_lock(self->lock, WAIT_LOCK);
+    PyObject* result = func(self->queue, args);
+    PyThread_release_lock(self->lock);
+    return result;
+}
+
+static PyObject* LockQueue_is_empty(LockQueue_t* self, PyObject* args) {
+    return LockQueue_call_with_lock(self, args, &Queue_is_empty);
+}
+
+static PyObject* LockQueue_enqueue(LockQueue_t* self, PyObject* args) {
+    return LockQueue_call_with_lock(self, args, &Queue_enqueue);
+}
+
+static PyObject* LockQueue_dequeue(LockQueue_t* self, PyObject* args) {
+    return LockQueue_call_with_lock(self, args, &Queue_dequeue);
+}
+
+static PyObject* LockQueue_extend(LockQueue_t* self, PyObject* args) {
+    return LockQueue_call_with_lock(self, args, &Queue_extend);
+}
+
+static PyObject* LockQueue_item(LockQueue_t* self, PyObject* args) {
+    return LockQueue_call_with_lock(self, args, &Queue_item);
+}
+
+static Py_ssize_t LockQueue_len(LockQueue_t* self) {
+    PyThread_acquire_lock(self->lock, 1);
+    Py_ssize_t res = (Py_ssize_t)self->queue->length;
+    PyThread_release_lock(self->lock);
+    return res;
+}
+
+static int LockQueue_setitem(LockQueue_t* self, Py_ssize_t index, PyObject* args) {
+    PyThread_acquire_lock(self->lock, 1);
+    int res = Queue_setitem(self->queue, index, args);
+    PyThread_release_lock(self->lock);
+    return res;
+}
+
+static int LockQueue_contains(LockQueue_t* self, PyObject* args) {
+    PyThread_acquire_lock(self->lock, 1);
+    int res = Queue_contains(self->queue, args);
+    PyThread_release_lock(self->lock);
+    return res;
+}
+
+static PyMethodDef LockQueue_methods[] = {
+    {"is_empty", (PyCFunction)LockQueue_is_empty, METH_NOARGS, is_empty_doc},
+    {"enqueue", (PyCFunction)LockQueue_enqueue, METH_O, enqueue_doc},
+    {"dequeue", (PyCFunction)LockQueue_dequeue, METH_NOARGS, dequeue_doc},
+    {"extend", (PyCFunction)LockQueue_extend, METH_O, extend_doc},
+    {NULL, NULL, 0, NULL}
+};
+
+static PySequenceMethods LockQueue_sequence_methods = {
+    (lenfunc)LockQueue_len,               /* sq_length */
+    0,                                    /* sq_concat */
+    NULL,                                 /* sq_repeat */
+    (ssizeargfunc)LockQueue_item,         /* sq_item */
+    NULL,                                 /* sq_slice */
+    (ssizeobjargproc)LockQueue_setitem,   /* sq_as_item */
+    NULL,                                 /* sq_as_slice */
+    (objobjproc)LockQueue_contains,       /* sq_contains */
+    0                                     /* sq_inplace_concat */
+};
+
+PyDoc_STRVAR(lockqueue_doc,"LockQueue() -> Single ended synchronous Queue object.");
+static PyTypeObject LockQueueType = {
+    PyVarObject_HEAD_INIT(NULL, 0)
+    "LockQueue",                                /* tp_name */
+    sizeof(LockQueue_t),                        /* tp_basicsize */
+    0,                                          /* tp_itemsize */
+    (destructor)LockQueue_dealloc,              /* tp_dealloc */
+    0,                                          /* tp_print */
+    0,                                          /* tp_getattr */
+    0,                                          /* tp_setattr */
+    0,                                          /* tp_reserved */
+    0,                                          /* tp_repr */
+    0,                                          /* tp_as_number */
+    &LockQueue_sequence_methods,                /* tp_as_sequence */
+    0,                                          /* tp_as_mapping */
+    PyObject_HashNotImplemented,                /* tp_hash */
+    0,                                          /* tp_call */
+    0,                                          /* tp_str */
+    PyObject_GenericGetAttr,                    /* tp_getattro */
+    0,                                          /* tp_setattro */
+    0,                                          /* tp_as_buffer */
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC,    /* tp_flags */
+    lockqueue_doc,                              /* tp_doc */
+    (traverseproc)LockQueue_traverse,           /* tp_traverse */
+    (inquiry)LockQueue_clear,                   /* tp_clear */
+    0,                                          /* tp_richcompare */
+    0,                                          /* tp_weaklistoffset */
+    0,                                          /* tp_iter */
+    0,                                          /* tp_iternext */
+    LockQueue_methods,                          /* tp_methods */
+    0,                                          /* tp_members */
+    0,                                          /* tp_getset */
+    0,                                          /* tp_base */
+    0,                                          /* tp_dict */
+    0,                                          /* tp_descr_get */
+    0,                                          /* tp_descr_set */
+    0,                                          /* tp_dictoffset */
+    (initproc)LockQueue_init,                   /* tp_init */
+    PyType_GenericAlloc,                        /* tp_alloc */
+    (newfunc)LockQueue_new,                     /* tp_new */
+    PyObject_GC_Del,                            /* tp_free */
+};
+
 static PyModuleDef QueueModuleDef = {
     PyModuleDef_HEAD_INIT,
     "_fastqueue",
     "Singly linked, small overhead implementations of the Queue data structure.",
     -1,
     NULL, NULL, NULL, NULL, NULL
 };
@@ -543,9 +693,10 @@
         return NULL;
 
     module = PyModule_Create(&QueueModuleDef);
     if (module == NULL)
         return NULL;
     PyModule_AddType(module, &QueueCType);
     PyModule_AddType(module, &QueueType);
+    PyModule_AddType(module, &LockQueueType);
     return module;
 }
```

### Comparing `fastqueue-lib-0.0.3/tests/test_queue.py` & `fastqueue-lib-0.0.4/tests/test_queue.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,122 +1,128 @@
 import pytest
+
 from fastqueue.prototypes import *
 from fastqueue import *
 
 queue_size = 500000
 
 
-@pytest.mark.parametrize("queue_type",
-                         [Queue(), QueueC(), LLQueue(), ContQueue()])
+@pytest.mark.parametrize(
+    "queue_type", [LockQueue(), Queue(), QueueC(), LLQueue(), ContQueue()]
+)
 def test_newQueue(queue_type):
     queue = queue_type
     assert queue.is_empty()
     assert len(queue) == 0
     queue.enqueue(1)
     assert not queue.is_empty()
     assert len(queue) == 1
-    queue.enqueue('🙂')
+    queue.enqueue("🙂")
     assert not queue.is_empty()
     assert len(queue) == 2
     item = queue.dequeue()
     assert not queue.is_empty()
     assert len(queue) == 1
     assert item == 1
     item = queue.dequeue()
     assert queue.is_empty()
     assert len(queue) == 0
-    assert item == '🙂'
+    assert item == "🙂"
 
     with pytest.raises(IndexError):
         queue.dequeue()
 
 
-@pytest.mark.parametrize("queue_type",
-                         [Queue(), QueueC(), LLQueue(), ContQueue()])
+@pytest.mark.parametrize(
+    "queue_type", [LockQueue(), Queue(), QueueC(), LLQueue(), ContQueue()]
+)
 def test_mutationQueue(queue_type):
     queue = queue_type
     queue.enqueue(1)
     item = queue.dequeue()
     assert item == 1
     item = 7
     queue.enqueue(item)
     assert item == 7
     queue.dequeue()
     assert item == 7
 
 
-@pytest.mark.parametrize("queue_type",
-                         [Queue(), QueueC(), LLQueue(), ContQueue()])
+@pytest.mark.parametrize(
+    "queue_type", [LockQueue(), Queue(), QueueC(), LLQueue(), ContQueue()]
+)
 def test_largeQueue(queue_type):
     queue = queue_type
     for i in range(queue_size):
         queue.enqueue(i)
     assert not queue.is_empty()
     assert len(queue) == queue_size
     for i in range(queue_size):
         assert queue.dequeue() == i
 
 
-@pytest.mark.parametrize("queue_type", [Queue(), QueueC()])
+@pytest.mark.parametrize("queue_type", [LockQueue(), Queue(), QueueC()])
 def test_extendQueue(queue_type):
     queue = queue_type
     queue.extend(range(queue_size))
     assert not queue.is_empty()
     assert len(queue) == queue_size
-    assert ([queue.dequeue() for _ in range(queue_size)] == list(
-        range(queue_size)))
+    assert [queue.dequeue() for _ in range(queue_size)] == list(range(queue_size))
     assert queue.is_empty()
     assert len(queue) == 0
+
     # Tests for mutation
     lst = [1, 2, 3]
     queue.extend(lst)
     assert len(queue) == 3
     assert lst == [1, 2, 3]
     assert lst[2] == 3
 
 
-@pytest.mark.parametrize("queue_type", [Queue(), QueueC()])
+@pytest.mark.parametrize("queue_type", [LockQueue(), Queue(), QueueC()])
 def test_getitemQueue(queue_type):
     queue = queue_type
     queue.extend(range(1000))
     assert queue[0] == queue[0]
     item = queue[0]
     assert item == 0
     item = queue[1]
     assert item == 1
     assert queue[256] == 256
     item = queue[len(queue) - 1]
     assert item == len(queue) - 1
 
     with pytest.raises(IndexError):
         queue[1000]
-
-    assert (queue[len(queue) - 1] == queue[-1])
-    assert (queue[len(queue) - 3] == queue[-3])
+    assert queue[len(queue) - 1] == queue[-1]
+    assert queue[len(queue) - 3] == queue[-3]
 
 
-@pytest.mark.parametrize("queue_type", [Queue(), QueueC()])
+@pytest.mark.parametrize("queue_type", [LockQueue(), Queue(), QueueC()])
 def test_setitemQueue(queue_type):
     queue = queue_type
     queue.extend(range(1000))
-    queue[0] = '🙂'
-    assert queue[0] == '🙂'
+    queue[0] = "🙂"
+    assert queue[0] == "🙂"
     queue[0] = 0
     assert queue[0] == 0
+
+    queue[0] = None
+    assert queue[0] is None
+
     queue[-1] = 10
     assert queue[len(queue) - 1] == 10
 
     with pytest.raises(IndexError):
         queue[1000] = 90
 
 
-@pytest.mark.parametrize("queue_type", [Queue(), QueueC()])
+@pytest.mark.parametrize("queue_type", [LockQueue(), Queue(), QueueC()])
 def test_containsQueue(queue_type):
     queue = queue_type
     queue.extend(range(queue_size))
     assert not (queue_size in queue)
     for i in range(258):
-        assert (i in queue)
-
-    assert (queue_size - 1 in queue)
+        assert i in queue
+    assert (queue_size - 1) in queue
     queue.dequeue()
     assert not (0 in queue)
```

