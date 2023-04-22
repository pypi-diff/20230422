# Comparing `tmp/eons-2.4.0.tar.gz` & `tmp/eons-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eons-2.4.0.tar", last modified: Tue Apr 18 14:58:37 2023, max compression
+gzip compressed data, was "eons-2.5.0.tar", last modified: Sat Apr 22 19:53:17 2023, max compression
```

## Comparing `eons-2.4.0.tar` & `eons-2.5.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:58:37.088723 eons-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-04-18 14:58:37.088723 eons-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-04-18 14:58:20.000000 eons-2.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:58:37.084723 eons-2.4.0/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:58:37.084723 eons-2.4.0/pkg/eons/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-18 14:58:28.000000 eons-2.4.0/pkg/eons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    82395 2023-04-18 14:58:28.000000 eons-2.4.0/pkg/eons/eons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:58:37.084723 eons-2.4.0/pkg/eons/method/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-18 14:58:09.000000 eons-2.4.0/pkg/eons/method/External.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:58:28.000000 eons-2.4.0/pkg/eons/method/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:58:37.088723 eons-2.4.0/pkg/eons/resolve/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:58:28.000000 eons-2.4.0/pkg/eons/resolve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-18 14:58:09.000000 eons-2.4.0/pkg/eons/resolve/resolve_find_by_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-18 14:58:09.000000 eons-2.4.0/pkg/eons/resolve/resolve_import_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-18 14:58:09.000000 eons-2.4.0/pkg/eons/resolve/resolve_install_from_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-18 14:58:09.000000 eons-2.4.0/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-18 14:58:09.000000 eons-2.4.0/pkg/eons/resolve/resolve_install_with_pip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:58:37.084723 eons-2.4.0/pkg/eons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-04-18 14:58:37.000000 eons-2.4.0/pkg/eons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-18 14:58:37.000000 eons-2.4.0/pkg/eons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:58:37.000000 eons-2.4.0/pkg/eons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-18 14:58:37.000000 eons-2.4.0/pkg/eons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-18 14:58:37.000000 eons-2.4.0/pkg/eons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-18 14:58:28.000000 eons-2.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-18 14:58:37.088723 eons-2.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:53:17.001582 eons-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-22 19:53:17.001582 eons-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19582 2023-04-22 19:53:00.000000 eons-2.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:53:16.997582 eons-2.5.0/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:53:16.997582 eons-2.5.0/pkg/eons/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-22 19:53:08.000000 eons-2.5.0/pkg/eons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84209 2023-04-22 19:53:08.000000 eons-2.5.0/pkg/eons/eons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:53:16.997582 eons-2.5.0/pkg/eons/method/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-22 19:52:53.000000 eons-2.5.0/pkg/eons/method/External.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 19:53:08.000000 eons-2.5.0/pkg/eons/method/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:53:17.001582 eons-2.5.0/pkg/eons/resolve/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 19:53:08.000000 eons-2.5.0/pkg/eons/resolve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-22 19:52:53.000000 eons-2.5.0/pkg/eons/resolve/resolve_find_by_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-22 19:52:53.000000 eons-2.5.0/pkg/eons/resolve/resolve_import_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-22 19:52:53.000000 eons-2.5.0/pkg/eons/resolve/resolve_install_from_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-22 19:52:53.000000 eons-2.5.0/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-22 19:52:53.000000 eons-2.5.0/pkg/eons/resolve/resolve_install_with_pip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:53:16.997582 eons-2.5.0/pkg/eons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-22 19:53:16.000000 eons-2.5.0/pkg/eons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-22 19:53:16.000000 eons-2.5.0/pkg/eons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 19:53:16.000000 eons-2.5.0/pkg/eons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-22 19:53:16.000000 eons-2.5.0/pkg/eons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-22 19:53:16.000000 eons-2.5.0/pkg/eons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-22 19:53:08.000000 eons-2.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-22 19:53:17.001582 eons-2.5.0/setup.cfg
```

### Comparing `eons-2.4.0/PKG-INFO` & `eons-2.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.4.0
+Version: 2.5.0
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -42,19 +42,20 @@
 * `-v` or `--verbose` (count, i.e `-vv` = 2) or `--verbosity #`, where # is some number, or the `verbosity` environment or config value: will show more information and increase the logging level, e.g. print debug messages (3 for debug; 2 for info).
 * `--config` or `-c` (string): the path to a json config file from which other values may be retrieved.
 * `--no-repo` or the `no_repo` environment or config value (bool, i.e. 'True', 'true', etc.): whether or not to enable reaching out to online servers for code (see Dynamic Functionality, below).
 * `--log-file` or the `log_file` environment or config value (string; supports formatting, e.g. '/var/log/eons/{this.name}.log'): optional value for logging to a file in addition to stderr.
 
 ## Features
 
-Eons supports 4 major features:
-* Get inputs to functors by drilling down through multiple layers
-* Allow functors to change behavior with their order of execution
-* Provide functionality by downloading functors on the fly
-* Resolve errors through dynamic resolution by functors
+Eons supports 5 major features:
+* Get inputs to functors by drilling down through multiple layers.
+* Allow functors to change behavior with their order of execution.
+* Provide functionality by downloading functors on the fly.
+* Managed composition through External Methods.
+* Resolve errors through dynamic resolution by functors.
 
 ### Inputs Through Configuration File and `Fetch()`
 
 Eons provides a simple means of retrieving variables from a wide array of places. When you `Fetch()` a variable, we look through:
 1. The system environment (e.g. `export some_key="some value"`)
 2. The json configuration file supplied with `--config` (or specified by `this.defualtConfigFile` per `Configure()`)
 3. Arguments supplied at the command line (e.g. specifying `--some-key "some value"` makes `Fetch(some_key)` return `"some value"`)
@@ -107,41 +108,81 @@
 --repo-password
 ```
 
 You may also publish to the online repository through [ebbs](https://github.com/eons-dev/bin_ebbs)
 
 NOTE: per the above section on the Configuration File, you can set `repo_username` in the environment to avoid passing credentials on the command line, or worse, you can store them in plain text in the configuration file ;)
 
+### Managed Composition via `@eons.method(impl="External")`
+
+Composition is a means of building complexity through encapsulation and typically answers the question of "has a ____", where classic inheritance answers "is a ____".
+Eons provides a means of making composition easy through the External Method implementation.
+
+For example, consider:
+```
+class MyClass(eons.Functor):
+    @method(impl="External")
+    def MyExternalFunctor(): pass
+```
+Here, we use a Functor called "MyExternalFunctor" to compose MyClass. The actual code for MyExternalFunctor is not provided here, but is instead retrieved through `GetRegistered()`, as described above. 
+
+Using this technique, we can reuse Functors within other Functors, and none of the code has to be present on the local system at runtime but can be supplied as needed.
+
+#### Requirements & Notes
+
+1. Circular dependencies are not supported. Because of this, any Functors used to compose more complex classes should be stored in sub-folders in the package or repo_store. Sub-folders will be registered before parent directories. See [Self Registration](#self-registration) for more info.
+
+2. When calling an External Method, the members of the Functor are not accessible through the function (e.g. `MyClass.MyExternalFunctor.DidFunctionSucceed()` is not currently supported). To accomplish such behavior, you must currently access the External Method through the `methods` member. For example, `MyClass.methods['MyExternalFunctor'].DidFunctionSucceed()`.
+
+3. All arguments the External Method accepts are valid to provide to the function. For example, if `MyExternalFunctor` accepts `my_arg` as an argument, you can call `MyClass.MyExternalFunctor(my_arg='whatever')`.
+
 ### Error Resolution for `@recoverable` Methods
 
 Any method (i.e. member function) of Executor or Functor may be decorated with `@recoverable`. If a `@recoverable` method raises an Exception, the Eons error resolution system will engage and attempt to fix the problem.
 
 Because there are a lot of ways an error might arise and be resolved, we don't give you the same freedom of execution as we do with generic `GetRegistered()` calls. While we use GetRegistered under-the-hood, all possible ErrorResolutions have to be specified ahead of time in your Executor's `resolveErrorsWith` list member.
 
 If you want to handle errors with your own ErrorResolution, simply call `my_executor.resolveErrorsWith.append('my_fix_everything_functor')` (paraphrasing).
 
 Creating ErrorResolutions is the same as any other Functor. The only difference is that when you derive from ErrorResolution most of the logic you need has been taken care of for you. You'll just have to implement a `Resolve(this)` method and call `this.ApplyTo(...)` in your constructor.  
 NOTE: all ErrorResolution packages should have the 'resolve_' prefix so that they may be readily identified online.
 
 Check out [install_from_repo](inc/resolve/resolve_install_from_repo.py) for an example.
 
+## Inheritance Overview
+
+Inheritance allows you to build functionality without duplicating code and is a primary driver for the core programming tenant of never writing the same line twice.
+
+Eons supports several kinds of inheritance. Notably:
+* Classic Inheritance
+* Implicit Inheritance (i.e. Sequence)
+* External Methods (i.e. composition)
+
+| Inheritance Style | Relationship | Compiletime | Runtime | Method & Member Accessibility | Type Sharing |
+| :---              | :---         |    :----:   |  :---:  |            :---:              |     :---:    |
+| Classic           |is a|:heavy_check_mark:|:x:|:heavy_check_mark:|:heavy_check_mark:|
+| Implicit          |how does|:x:|:heavy_check_mark:|:heavy_check_mark:|:x:|
+| External          |has a|:heavy_check_mark:|:x:|:x:|:x:|
+
+You are not restricted to a single kind of inheritance. You can, and are encouraged, to use all forms of inheritance in your code!
+
 ## Performance
 
-At Eons, we always prefer functionality over performance. This is the same as the whole "don't prematurely optimize" argument. With that said, optimizing is always good and we try to do it as much as possible.
+At Eons LLC, we always prefer functionality over performance. This is the same as the whole "don't prematurely optimize" argument. With that said, optimizing is always good and we try to do it as much as possible.
 
 Please let us know if you are hitting any bottlenecks in this or any of our other libraries! 
 
 ## Design
 
 Functors. Functors...
 
 ### Functors
 
 Functors are classes (objects) that have an invokable `()` operator. This allows you to treat them like functions.
-Eons uses functors (implemented as the Functor class) to provide input, analysis, and output functionalities, which are made simple through classical and implicit inheritance.
+Eons uses functors (implemented as the Functor class) to provide input, analysis, and output functionalities, which are made simple through classic and implicit inheritance.
 
 Imagine you write 2 functions that take inputs `a` and `b`. You can choose to duplicate these inputs, as is the classic means of writing functions: `firstFunction(a, b)` and `secondFunction(a, b)`. However, with Functors, you can make `baseFunctor{inputs=[a,b]}` and then simply `firstFunctor(baseFunctor)` and `secondFunctor(baseFunctor)`, thus creating 2 Functors with identical inputs. The result of `firstFunctor(a, b) == firstFunction(a, b)` and likewise for the seconds; only, by using Functors we've saved ourselves from duplicating code.
 
 ### Inputs
 
 For extensibility, all Functors take both an `*args` and `**kwargs` argument when called. This allows you to provide arbitrary key word arguments (e.g. key="value") to your objects.
 
@@ -155,18 +196,20 @@
 All values provided in these members will be populated by calls to `Fetch()`, as described above. This means that if the user calling your Functor does not provide, say their password, it can be automatically looked up in the environment variables.
 
 For other supported features, check out [Functor.py](src/Functor.py)
 
 
 ### Self Registration
 
-Normally, one has to `import` the files they create into their "main" file in order to use them. That does not apply when using Eons. Instead, you simply have to derive from an appropriate base class and then call `SelfRegistering.RegisterAllClassesInDirectory(...)` (which is usually done for you based on the `repo['store']` and `defaultRepoDirectory` members), providing the directory of the file as the only argument. This will essentially `import` all files in that directory and make them instantiable via `SelfRegistering("ClassName")`.
+Normally, one has to `import` the files they create into their "main" file in order to use them. That does not apply when using Eons. Instead, you simply have to derive from an appropriate base class and then call `SelfRegistering.RegisterAllClassesInDirectory(...)` (which is usually done for you based on the `repo.store` and `defaultRepoDirectory` members), providing the directory of the file as the only argument. This will essentially `import` all files in that directory and make them instantiable via `SelfRegistering("ClassName")`.
 
 Dynamic error resolutions enables this self registration system to work with inheritance as well. This means that, within downloaded functor, you can `from some_module_to_download import my_desired_class` to download another.
 
+NOTE: `SelfRegistering.RegisterAllClassesInDirectory(...)` is depth-first, meaning any sub-folders in the given folder will be loaded before the parent directory. This helps to organzie inheritance dependencies, but can be disabled with `recurse=False`.
+
 #### Example
 
 In some `MyDatum.py` in a `MyData` directory, you might have:
 ```
 import logging
 from Eons import Datum
 class MyDatum(Datum): #Datum is a useful child of SelfRegistering
```

### Comparing `eons-2.4.0/README.md` & `eons-2.5.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -27,19 +27,20 @@
 * `-v` or `--verbose` (count, i.e `-vv` = 2) or `--verbosity #`, where # is some number, or the `verbosity` environment or config value: will show more information and increase the logging level, e.g. print debug messages (3 for debug; 2 for info).
 * `--config` or `-c` (string): the path to a json config file from which other values may be retrieved.
 * `--no-repo` or the `no_repo` environment or config value (bool, i.e. 'True', 'true', etc.): whether or not to enable reaching out to online servers for code (see Dynamic Functionality, below).
 * `--log-file` or the `log_file` environment or config value (string; supports formatting, e.g. '/var/log/eons/{this.name}.log'): optional value for logging to a file in addition to stderr.
 
 ## Features
 
-Eons supports 4 major features:
-* Get inputs to functors by drilling down through multiple layers
-* Allow functors to change behavior with their order of execution
-* Provide functionality by downloading functors on the fly
-* Resolve errors through dynamic resolution by functors
+Eons supports 5 major features:
+* Get inputs to functors by drilling down through multiple layers.
+* Allow functors to change behavior with their order of execution.
+* Provide functionality by downloading functors on the fly.
+* Managed composition through External Methods.
+* Resolve errors through dynamic resolution by functors.
 
 ### Inputs Through Configuration File and `Fetch()`
 
 Eons provides a simple means of retrieving variables from a wide array of places. When you `Fetch()` a variable, we look through:
 1. The system environment (e.g. `export some_key="some value"`)
 2. The json configuration file supplied with `--config` (or specified by `this.defualtConfigFile` per `Configure()`)
 3. Arguments supplied at the command line (e.g. specifying `--some-key "some value"` makes `Fetch(some_key)` return `"some value"`)
@@ -92,41 +93,81 @@
 --repo-password
 ```
 
 You may also publish to the online repository through [ebbs](https://github.com/eons-dev/bin_ebbs)
 
 NOTE: per the above section on the Configuration File, you can set `repo_username` in the environment to avoid passing credentials on the command line, or worse, you can store them in plain text in the configuration file ;)
 
+### Managed Composition via `@eons.method(impl="External")`
+
+Composition is a means of building complexity through encapsulation and typically answers the question of "has a ____", where classic inheritance answers "is a ____".
+Eons provides a means of making composition easy through the External Method implementation.
+
+For example, consider:
+```
+class MyClass(eons.Functor):
+    @method(impl="External")
+    def MyExternalFunctor(): pass
+```
+Here, we use a Functor called "MyExternalFunctor" to compose MyClass. The actual code for MyExternalFunctor is not provided here, but is instead retrieved through `GetRegistered()`, as described above. 
+
+Using this technique, we can reuse Functors within other Functors, and none of the code has to be present on the local system at runtime but can be supplied as needed.
+
+#### Requirements & Notes
+
+1. Circular dependencies are not supported. Because of this, any Functors used to compose more complex classes should be stored in sub-folders in the package or repo_store. Sub-folders will be registered before parent directories. See [Self Registration](#self-registration) for more info.
+
+2. When calling an External Method, the members of the Functor are not accessible through the function (e.g. `MyClass.MyExternalFunctor.DidFunctionSucceed()` is not currently supported). To accomplish such behavior, you must currently access the External Method through the `methods` member. For example, `MyClass.methods['MyExternalFunctor'].DidFunctionSucceed()`.
+
+3. All arguments the External Method accepts are valid to provide to the function. For example, if `MyExternalFunctor` accepts `my_arg` as an argument, you can call `MyClass.MyExternalFunctor(my_arg='whatever')`.
+
 ### Error Resolution for `@recoverable` Methods
 
 Any method (i.e. member function) of Executor or Functor may be decorated with `@recoverable`. If a `@recoverable` method raises an Exception, the Eons error resolution system will engage and attempt to fix the problem.
 
 Because there are a lot of ways an error might arise and be resolved, we don't give you the same freedom of execution as we do with generic `GetRegistered()` calls. While we use GetRegistered under-the-hood, all possible ErrorResolutions have to be specified ahead of time in your Executor's `resolveErrorsWith` list member.
 
 If you want to handle errors with your own ErrorResolution, simply call `my_executor.resolveErrorsWith.append('my_fix_everything_functor')` (paraphrasing).
 
 Creating ErrorResolutions is the same as any other Functor. The only difference is that when you derive from ErrorResolution most of the logic you need has been taken care of for you. You'll just have to implement a `Resolve(this)` method and call `this.ApplyTo(...)` in your constructor.  
 NOTE: all ErrorResolution packages should have the 'resolve_' prefix so that they may be readily identified online.
 
 Check out [install_from_repo](inc/resolve/resolve_install_from_repo.py) for an example.
 
+## Inheritance Overview
+
+Inheritance allows you to build functionality without duplicating code and is a primary driver for the core programming tenant of never writing the same line twice.
+
+Eons supports several kinds of inheritance. Notably:
+* Classic Inheritance
+* Implicit Inheritance (i.e. Sequence)
+* External Methods (i.e. composition)
+
+| Inheritance Style | Relationship | Compiletime | Runtime | Method & Member Accessibility | Type Sharing |
+| :---              | :---         |    :----:   |  :---:  |            :---:              |     :---:    |
+| Classic           |is a|:heavy_check_mark:|:x:|:heavy_check_mark:|:heavy_check_mark:|
+| Implicit          |how does|:x:|:heavy_check_mark:|:heavy_check_mark:|:x:|
+| External          |has a|:heavy_check_mark:|:x:|:x:|:x:|
+
+You are not restricted to a single kind of inheritance. You can, and are encouraged, to use all forms of inheritance in your code!
+
 ## Performance
 
-At Eons, we always prefer functionality over performance. This is the same as the whole "don't prematurely optimize" argument. With that said, optimizing is always good and we try to do it as much as possible.
+At Eons LLC, we always prefer functionality over performance. This is the same as the whole "don't prematurely optimize" argument. With that said, optimizing is always good and we try to do it as much as possible.
 
 Please let us know if you are hitting any bottlenecks in this or any of our other libraries! 
 
 ## Design
 
 Functors. Functors...
 
 ### Functors
 
 Functors are classes (objects) that have an invokable `()` operator. This allows you to treat them like functions.
-Eons uses functors (implemented as the Functor class) to provide input, analysis, and output functionalities, which are made simple through classical and implicit inheritance.
+Eons uses functors (implemented as the Functor class) to provide input, analysis, and output functionalities, which are made simple through classic and implicit inheritance.
 
 Imagine you write 2 functions that take inputs `a` and `b`. You can choose to duplicate these inputs, as is the classic means of writing functions: `firstFunction(a, b)` and `secondFunction(a, b)`. However, with Functors, you can make `baseFunctor{inputs=[a,b]}` and then simply `firstFunctor(baseFunctor)` and `secondFunctor(baseFunctor)`, thus creating 2 Functors with identical inputs. The result of `firstFunctor(a, b) == firstFunction(a, b)` and likewise for the seconds; only, by using Functors we've saved ourselves from duplicating code.
 
 ### Inputs
 
 For extensibility, all Functors take both an `*args` and `**kwargs` argument when called. This allows you to provide arbitrary key word arguments (e.g. key="value") to your objects.
 
@@ -140,18 +181,20 @@
 All values provided in these members will be populated by calls to `Fetch()`, as described above. This means that if the user calling your Functor does not provide, say their password, it can be automatically looked up in the environment variables.
 
 For other supported features, check out [Functor.py](src/Functor.py)
 
 
 ### Self Registration
 
-Normally, one has to `import` the files they create into their "main" file in order to use them. That does not apply when using Eons. Instead, you simply have to derive from an appropriate base class and then call `SelfRegistering.RegisterAllClassesInDirectory(...)` (which is usually done for you based on the `repo['store']` and `defaultRepoDirectory` members), providing the directory of the file as the only argument. This will essentially `import` all files in that directory and make them instantiable via `SelfRegistering("ClassName")`.
+Normally, one has to `import` the files they create into their "main" file in order to use them. That does not apply when using Eons. Instead, you simply have to derive from an appropriate base class and then call `SelfRegistering.RegisterAllClassesInDirectory(...)` (which is usually done for you based on the `repo.store` and `defaultRepoDirectory` members), providing the directory of the file as the only argument. This will essentially `import` all files in that directory and make them instantiable via `SelfRegistering("ClassName")`.
 
 Dynamic error resolutions enables this self registration system to work with inheritance as well. This means that, within downloaded functor, you can `from some_module_to_download import my_desired_class` to download another.
 
+NOTE: `SelfRegistering.RegisterAllClassesInDirectory(...)` is depth-first, meaning any sub-folders in the given folder will be loaded before the parent directory. This helps to organzie inheritance dependencies, but can be disabled with `recurse=False`.
+
 #### Example
 
 In some `MyDatum.py` in a `MyData` directory, you might have:
 ```
 import logging
 from Eons import Datum
 class MyDatum(Datum): #Datum is a useful child of SelfRegistering
```

### Comparing `eons-2.4.0/pkg/eons/eons.py` & `eons-2.5.0/pkg/eons/eons.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,17 @@
 class MissingArgumentError(Exception, metaclass=ActualType): pass
 
 class FunctorError(Exception, metaclass=ActualType): pass
 class MissingMethodError(FunctorError, metaclass=ActualType): pass
 class CommandUnsuccessful(FunctorError, metaclass=ActualType): pass
 class InvalidNext(FunctorError, metaclass=ActualType): pass
 
+class ExecutorError(FunctorError, metaclass=ActualType): pass
+class ExecutorSetupError(ExecutorError, metaclass=ActualType): pass
+
 class ErrorResolutionError(Exception, metaclass=ActualType): pass
 class FailedErrorResolution(ErrorResolutionError, metaclass=ActualType): pass
 
 class SelfRegisteringError(Exception, metaclass=ActualType): pass
 class ClassNotFound(SelfRegisteringError, metaclass=ActualType): pass
 
 class HelpWanted(Exception, metaclass=ActualType): pass
@@ -98,22 +101,30 @@
 
 		#__dict__ is always blank during __new__ and only populated by __init__.
 		#This is only useful as a negative control.
 		# logging.debug(f"Created object of {child.__dict__}")
 
 		return child
 
+	# Registering classes is typically depth-first.
 	@staticmethod
-	def RegisterAllClassesInDirectory(directory):
+	def RegisterAllClassesInDirectory(directory, recurse=True):
 		logging.debug(f"Loading SelfRegistering classes in {directory}")
-		logging.debug(f"Available modules: {os.listdir(directory)}")
-		for file in os.listdir(directory):
-			if (file.startswith('_') or not file.endswith('.py')):
-				continue
+		directoryContents = [i for i in sorted(os.listdir(directory)) if not i.startswith('_')]
 
+		directories = [i for i in directoryContents if os.path.isdir(os.path.join(directory, i))]
+		files = [i for i in directoryContents if os.path.isfile(os.path.join(directory, i))]
+		files = [f for f in files if f.endswith('.py')]
+
+		if (recurse):
+			for dir in directories:				
+				SelfRegistering.RegisterAllClassesInDirectory(os.path.join(directory, dir), recurse)
+
+		logging.debug(f"Available modules: {files}")
+		for file in files:
 			moduleName = file.split('.')[0]
 
 			# logging.debug(f"Attempting to registering classes in {moduleName}.")
 			loader = importlib.machinery.SourceFileLoader(moduleName, os.path.join(directory, file))
 			module = types.ModuleType(loader.name)
 			loader.exec_module(module)
 
@@ -1064,14 +1075,16 @@
 '''
 		if (this.executor and this.executor.verbosity > 3):
 			logging.debug(f"Source for {this.name} is:\n{completeSource}")
 		code = compile(completeSource, '', 'exec')
 		exec(code)
 		exec(f'this.Function = {wrappedFunctionName}.__get__(this, this.__class__)')
 
+
+
 	# Parse arguments and update the source code
 	# TODO: Implement full python parser to avoid bad string replacement (e.g. "def func(self):... self.selfImprovement" => "... this.object.this.object.Improvement").
 	def PopulateFrom(this, function):
 		this.source = ':'.join(inspect.getsource(function).split(':')[1:]) #Remove the first function definition
 
 		args = inspect.signature(function, follow_wrapped=False).parameters
 		thisSymbol = next(iter(args))
@@ -1109,15 +1122,17 @@
 	# The class and all other properties are irrelevant. However, they are provided and intended for debugging only.
 	def Constructor(this, function, cls):
 		this.name = function.__name__
 		this.original.cls = cls
 		this.original.function = function
 
 		this.PopulateFrom(function)
-		this.UpdateSource()
+		
+		# UpdateSource is called by Functor.PopulateMethods()
+		# this.UpdateSource()
 
 
 	# Grab any known and necessary args from this.kwargs before any Fetch calls are made.
 	def PopulatePrecursor(this):
 		if (not this.object):
 			raise MissingArgumentError(f"Call {this.name} from a class instance: {this.original.cls.__name__}.{this.name}(...). Maybe Functor.PopulateMethods() hasn't been called yet?")
 
@@ -1761,14 +1776,15 @@
 		this.extraArgs = None
 		
 		# How much information should we output?
 		this.verbosity = 0
 
 		# config is loaded with the contents of a JSON config file specified by --config / -c or by the defaultConfigFile location, below.
 		this.config = None
+		this.configType = None
 
 		# *this will keep track of any global variables it creates.
 		# All globals should be read only.
 		# Dict is in the form of {variable_name: set_by_fetch}
 		# See SetGlobal(), below.
 		this.globals = {}
 
@@ -1791,17 +1807,20 @@
 		this.registerDirectories = []
 		this.defaultConfigFile = None
 		this.defaultPackageType = ""
 
 		# Allow the config file to be in multiple formats.
 		# These are in preference order (e.g. if you want to look for a .txt file before a .json, add it to the top of the list).
 		this.configFileExtensions = [
-			"json",
+			"flow",
+			"py",
 			"yaml",
-			"yml"
+			"json",
+			"flw",
+			"yml",
 		]
 
 		this.Configure()
 		this.RegisterIncludedClasses()
 		this.AddArgs()
 
 
@@ -1962,17 +1981,31 @@
 	# Register all classes in each directory in this.registerDirectories
 	def RegisterAllClasses(this):
 		for d in this.registerDirectories:
 			this.RegisterAllClassesInDirectory(os.path.join(os.getcwd(), d))
 		this.RegisterAllClassesInDirectory(this.repo.store)
 
 
+	# Grok the configFile and populate this.config
+	def ParseConfigFile(this, configFile):
+		if (this.configType in ['py']):
+			this.RegisterAllClassesInDirectory(Path('./').joinpath('/'.join(this.parsedArgs.config.split['/'][:-1])))
+			functor = SelfRegistering(this.parsedArgs.config.split('/')[-1].split('.')[0])
+			this.config = functor(executor=this)
+		elif (this.configType in ['json', 'yml', 'yaml']):
+			# Yaml doesn't allow tabs. We do. Convert.
+			this.config = yaml.safe_load(configFile.read().replace('\t', '  '))
+		else:
+			raise ExecutorSetupError(f"Unknown configuration file type: {this.configType}")
+
+
 	# Populate the configuration details for *this.
 	def PopulateConfig(this):
 		this.config = None
+		this.configType = None
 
 		if (this.parsedArgs.config is None and this.defaultConfigFile is not None):
 			for ext in this.configFileExtensions:
 				possibleConfig = f"{this.defaultConfigFile}.{ext}"
 				if (Path(possibleConfig).exists()):
 					this.parsedArgs.config = possibleConfig
 					break
@@ -1981,19 +2014,19 @@
 
 		if (this.parsedArgs.config is None):
 			return
 
 		if (not os.path.isfile(this.parsedArgs.config)):
 			logging.error(f"Could not open configuration file: {this.parsedArgs.config}")
 			return
+		
+		this.configType = this.parsedArgs.config.split('.')[-1]
 
 		configFile = open(this.parsedArgs.config, "r")
-		# Yaml doesn't allow tabs. We do. Convert.
-		this.config = yaml.safe_load(configFile.read().replace('\t', '  '))
-		# this.config = jsonpickle.decode(configFile.read())
+		this.ParseConfigFile(configFile)
 		configFile.close()
 
 
 	#  Get information for how to download packages.
 	def PopulateRepoDetails(this):
 		details = {
 			"online": not this.Fetch('no_repo', False, ['this', 'args', 'config']),
@@ -2050,18 +2083,24 @@
 
 		extraArgsValues = []
 		for index in range(1, len(extraArgs), 2):
 			extraArgsValues.append(extraArgs[index])
 
 		this.extraArgs = dict(zip(extraArgsKeys, extraArgsValues))
 
+
 	# Functor method.
 	# We have to ParseArgs() here in order for other Executors to use ____KWArgs...
 	def ParseInitialArgs(this):
 		this.ParseArgs() # first, to enable debug and other such settings.
+
+		# Track *this globally
+		# This needs to be done before the config is populated, in case we use a py file that has External Methods.
+		ExecutorTracker.Instance().Push(this)
+
 		this.PopulateConfig()
 		this.SetVerbosity()
 		this.SetLogFile()
 		logging.debug(f"<---- {this.name} (log level: {logging.getLogger().level}) ---->")
 		logging.debug(f"Got extra arguments: {this.extraArgs}") # has to be after verbosity setting
 		logging.debug(f"Got config contents: {this.config}")
 		this.PopulateRepoDetails()
@@ -2069,31 +2108,49 @@
 
 	# Functor required method
 	# Override this with your own workflow.
 	def Function(this):
 		
 		# NOTE: class registration may instantiate other Executors.
 		this.RegisterAllClasses()
-
-		# Track *this globally
-		ExecutorTracker.Instance().Push(this)
 		
 		this.InitData()
 
 
 	# By default, Executors do not act on this.next; instead, they make it available to all Executed Functors.
 	def CallNext(this):
 		pass
 
 
 	# Close out anything we left open.
 	def AfterFunction(this):
 		this.TeardownLogging()
 
 
+	def WarmUpFlow(this, flow):
+		flow.WarmUp(executor=this)
+
+
+	# Flows are domain-like strings which can be resolved to a Functor.
+	@recoverable
+	def Flow(this, flow):
+		logging.debug(f"Calculating flow: {flow}")
+
+		flowList = flow.split('.')
+		flowList.reverse()
+		current = this.GetRegistered(flowList.pop(0), 'flow')
+		while (True):
+			this.WarmUpFlow(current)
+			if (not len(flowList)):
+				break
+
+			current = current.methods[flowList.pop(0)]
+		return current()
+	
+
 	# Execute a Functor based on name alone (not object).
 	# If the given Functor has been Executed before, the cached Functor will be called again. Otherwise, a new Functor will be constructed.
 	@recoverable
 	def Execute(this, functorName, *args, **kwargs):
 		packageType = this.defaultPackageType
 		if ('packageType' in kwargs):
 			packageType = kwargs.pop('packageType')
```

### Comparing `eons-2.4.0/pkg/eons/method/External.py` & `eons-2.5.0/pkg/eons/method/External.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,20 +8,22 @@
 	def __init__(this, name="External Method"):
 		super().__init__(name)
 
 		this.enableRollback = False
 		this.functionSucceeded = True
 		this.rollbackSucceeded = True
 
-		this.type = eons.ExecutorTracker.GetLatest().defaultPackageType
-
+		this.type = None
 		this.functorName = ""
 		this.functor = None
 
 	def UpdateSource(this):
+		if (not this.type):
+			this.type = eons.ExecutorTracker.GetLatest().defaultPackageType
+
 		this.functor = eons.ExecutorTracker.GetLatest().GetRegistered(this.functorName, this.type)
 
 		if (not this.functor):
 			raise eons.MissingMethodError(f"Could not populate external method {this.functorName} (type {this.type})")
 		
 		this.functor.name = f"{this.functor.name} (external)"
```

### Comparing `eons-2.4.0/pkg/eons/resolve/resolve_find_by_fetch.py` & `eons-2.5.0/pkg/eons/resolve/resolve_find_by_fetch.py`

 * *Files identical despite different names*

### Comparing `eons-2.4.0/pkg/eons/resolve/resolve_import_module.py` & `eons-2.5.0/pkg/eons/resolve/resolve_import_module.py`

 * *Files identical despite different names*

### Comparing `eons-2.4.0/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py` & `eons-2.5.0/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py`

 * *Files identical despite different names*

### Comparing `eons-2.4.0/pkg/eons.egg-info/PKG-INFO` & `eons-2.5.0/pkg/eons.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.4.0
+Version: 2.5.0
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -42,19 +42,20 @@
 * `-v` or `--verbose` (count, i.e `-vv` = 2) or `--verbosity #`, where # is some number, or the `verbosity` environment or config value: will show more information and increase the logging level, e.g. print debug messages (3 for debug; 2 for info).
 * `--config` or `-c` (string): the path to a json config file from which other values may be retrieved.
 * `--no-repo` or the `no_repo` environment or config value (bool, i.e. 'True', 'true', etc.): whether or not to enable reaching out to online servers for code (see Dynamic Functionality, below).
 * `--log-file` or the `log_file` environment or config value (string; supports formatting, e.g. '/var/log/eons/{this.name}.log'): optional value for logging to a file in addition to stderr.
 
 ## Features
 
-Eons supports 4 major features:
-* Get inputs to functors by drilling down through multiple layers
-* Allow functors to change behavior with their order of execution
-* Provide functionality by downloading functors on the fly
-* Resolve errors through dynamic resolution by functors
+Eons supports 5 major features:
+* Get inputs to functors by drilling down through multiple layers.
+* Allow functors to change behavior with their order of execution.
+* Provide functionality by downloading functors on the fly.
+* Managed composition through External Methods.
+* Resolve errors through dynamic resolution by functors.
 
 ### Inputs Through Configuration File and `Fetch()`
 
 Eons provides a simple means of retrieving variables from a wide array of places. When you `Fetch()` a variable, we look through:
 1. The system environment (e.g. `export some_key="some value"`)
 2. The json configuration file supplied with `--config` (or specified by `this.defualtConfigFile` per `Configure()`)
 3. Arguments supplied at the command line (e.g. specifying `--some-key "some value"` makes `Fetch(some_key)` return `"some value"`)
@@ -107,41 +108,81 @@
 --repo-password
 ```
 
 You may also publish to the online repository through [ebbs](https://github.com/eons-dev/bin_ebbs)
 
 NOTE: per the above section on the Configuration File, you can set `repo_username` in the environment to avoid passing credentials on the command line, or worse, you can store them in plain text in the configuration file ;)
 
+### Managed Composition via `@eons.method(impl="External")`
+
+Composition is a means of building complexity through encapsulation and typically answers the question of "has a ____", where classic inheritance answers "is a ____".
+Eons provides a means of making composition easy through the External Method implementation.
+
+For example, consider:
+```
+class MyClass(eons.Functor):
+    @method(impl="External")
+    def MyExternalFunctor(): pass
+```
+Here, we use a Functor called "MyExternalFunctor" to compose MyClass. The actual code for MyExternalFunctor is not provided here, but is instead retrieved through `GetRegistered()`, as described above. 
+
+Using this technique, we can reuse Functors within other Functors, and none of the code has to be present on the local system at runtime but can be supplied as needed.
+
+#### Requirements & Notes
+
+1. Circular dependencies are not supported. Because of this, any Functors used to compose more complex classes should be stored in sub-folders in the package or repo_store. Sub-folders will be registered before parent directories. See [Self Registration](#self-registration) for more info.
+
+2. When calling an External Method, the members of the Functor are not accessible through the function (e.g. `MyClass.MyExternalFunctor.DidFunctionSucceed()` is not currently supported). To accomplish such behavior, you must currently access the External Method through the `methods` member. For example, `MyClass.methods['MyExternalFunctor'].DidFunctionSucceed()`.
+
+3. All arguments the External Method accepts are valid to provide to the function. For example, if `MyExternalFunctor` accepts `my_arg` as an argument, you can call `MyClass.MyExternalFunctor(my_arg='whatever')`.
+
 ### Error Resolution for `@recoverable` Methods
 
 Any method (i.e. member function) of Executor or Functor may be decorated with `@recoverable`. If a `@recoverable` method raises an Exception, the Eons error resolution system will engage and attempt to fix the problem.
 
 Because there are a lot of ways an error might arise and be resolved, we don't give you the same freedom of execution as we do with generic `GetRegistered()` calls. While we use GetRegistered under-the-hood, all possible ErrorResolutions have to be specified ahead of time in your Executor's `resolveErrorsWith` list member.
 
 If you want to handle errors with your own ErrorResolution, simply call `my_executor.resolveErrorsWith.append('my_fix_everything_functor')` (paraphrasing).
 
 Creating ErrorResolutions is the same as any other Functor. The only difference is that when you derive from ErrorResolution most of the logic you need has been taken care of for you. You'll just have to implement a `Resolve(this)` method and call `this.ApplyTo(...)` in your constructor.  
 NOTE: all ErrorResolution packages should have the 'resolve_' prefix so that they may be readily identified online.
 
 Check out [install_from_repo](inc/resolve/resolve_install_from_repo.py) for an example.
 
+## Inheritance Overview
+
+Inheritance allows you to build functionality without duplicating code and is a primary driver for the core programming tenant of never writing the same line twice.
+
+Eons supports several kinds of inheritance. Notably:
+* Classic Inheritance
+* Implicit Inheritance (i.e. Sequence)
+* External Methods (i.e. composition)
+
+| Inheritance Style | Relationship | Compiletime | Runtime | Method & Member Accessibility | Type Sharing |
+| :---              | :---         |    :----:   |  :---:  |            :---:              |     :---:    |
+| Classic           |is a|:heavy_check_mark:|:x:|:heavy_check_mark:|:heavy_check_mark:|
+| Implicit          |how does|:x:|:heavy_check_mark:|:heavy_check_mark:|:x:|
+| External          |has a|:heavy_check_mark:|:x:|:x:|:x:|
+
+You are not restricted to a single kind of inheritance. You can, and are encouraged, to use all forms of inheritance in your code!
+
 ## Performance
 
-At Eons, we always prefer functionality over performance. This is the same as the whole "don't prematurely optimize" argument. With that said, optimizing is always good and we try to do it as much as possible.
+At Eons LLC, we always prefer functionality over performance. This is the same as the whole "don't prematurely optimize" argument. With that said, optimizing is always good and we try to do it as much as possible.
 
 Please let us know if you are hitting any bottlenecks in this or any of our other libraries! 
 
 ## Design
 
 Functors. Functors...
 
 ### Functors
 
 Functors are classes (objects) that have an invokable `()` operator. This allows you to treat them like functions.
-Eons uses functors (implemented as the Functor class) to provide input, analysis, and output functionalities, which are made simple through classical and implicit inheritance.
+Eons uses functors (implemented as the Functor class) to provide input, analysis, and output functionalities, which are made simple through classic and implicit inheritance.
 
 Imagine you write 2 functions that take inputs `a` and `b`. You can choose to duplicate these inputs, as is the classic means of writing functions: `firstFunction(a, b)` and `secondFunction(a, b)`. However, with Functors, you can make `baseFunctor{inputs=[a,b]}` and then simply `firstFunctor(baseFunctor)` and `secondFunctor(baseFunctor)`, thus creating 2 Functors with identical inputs. The result of `firstFunctor(a, b) == firstFunction(a, b)` and likewise for the seconds; only, by using Functors we've saved ourselves from duplicating code.
 
 ### Inputs
 
 For extensibility, all Functors take both an `*args` and `**kwargs` argument when called. This allows you to provide arbitrary key word arguments (e.g. key="value") to your objects.
 
@@ -155,18 +196,20 @@
 All values provided in these members will be populated by calls to `Fetch()`, as described above. This means that if the user calling your Functor does not provide, say their password, it can be automatically looked up in the environment variables.
 
 For other supported features, check out [Functor.py](src/Functor.py)
 
 
 ### Self Registration
 
-Normally, one has to `import` the files they create into their "main" file in order to use them. That does not apply when using Eons. Instead, you simply have to derive from an appropriate base class and then call `SelfRegistering.RegisterAllClassesInDirectory(...)` (which is usually done for you based on the `repo['store']` and `defaultRepoDirectory` members), providing the directory of the file as the only argument. This will essentially `import` all files in that directory and make them instantiable via `SelfRegistering("ClassName")`.
+Normally, one has to `import` the files they create into their "main" file in order to use them. That does not apply when using Eons. Instead, you simply have to derive from an appropriate base class and then call `SelfRegistering.RegisterAllClassesInDirectory(...)` (which is usually done for you based on the `repo.store` and `defaultRepoDirectory` members), providing the directory of the file as the only argument. This will essentially `import` all files in that directory and make them instantiable via `SelfRegistering("ClassName")`.
 
 Dynamic error resolutions enables this self registration system to work with inheritance as well. This means that, within downloaded functor, you can `from some_module_to_download import my_desired_class` to download another.
 
+NOTE: `SelfRegistering.RegisterAllClassesInDirectory(...)` is depth-first, meaning any sub-folders in the given folder will be loaded before the parent directory. This helps to organzie inheritance dependencies, but can be disabled with `recurse=False`.
+
 #### Example
 
 In some `MyDatum.py` in a `MyData` directory, you might have:
 ```
 import logging
 from Eons import Datum
 class MyDatum(Datum): #Datum is a useful child of SelfRegistering
```

### Comparing `eons-2.4.0/pkg/eons.egg-info/SOURCES.txt` & `eons-2.5.0/pkg/eons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eons-2.4.0/setup.cfg` & `eons-2.5.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eons
-version = 2.4.0
+version = 2.5.0
 author = Eons
 author_email = support@eons.llc
 description = Eons Python Framework
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/eons-dev/eons.lib
@@ -20,16 +20,16 @@
 package_dir = 
 	= pkg
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	tqdm
 	pyyaml
-	jsonpickle
 	requests
+	jsonpickle
 
 [options.packages.find]
 where = pkg
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

