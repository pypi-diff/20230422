# Comparing `tmp/swim-protocol-0.3.8.tar.gz` & `tmp/swim-protocol-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swim-protocol-0.3.8.tar", last modified: Sat May 15 20:45:51 2021, max compression
+gzip compressed data, was "swim-protocol-0.3.9.tar", last modified: Wed Jul 27 23:57:37 2022, max compression
```

## Comparing `swim-protocol-0.3.8.tar` & `swim-protocol-0.3.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-15 20:45:51.486389 swim-protocol-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2021-05-15 20:45:42.000000 swim-protocol-0.3.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       88 2021-05-15 20:45:42.000000 swim-protocol-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9907 2021-05-15 20:45:51.486389 swim-protocol-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6667 2021-05-15 20:45:42.000000 swim-protocol-0.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      232 2021-05-15 20:45:51.486389 swim-protocol-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2286 2021-05-15 20:45:42.000000 swim-protocol-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-15 20:45:51.478389 swim-protocol-0.3.8/swim_protocol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9907 2021-05-15 20:45:51.000000 swim-protocol-0.3.8/swim_protocol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      738 2021-05-15 20:45:51.000000 swim-protocol-0.3.8/swim_protocol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-15 20:45:51.000000 swim-protocol-0.3.8/swim_protocol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      125 2021-05-15 20:45:51.000000 swim-protocol-0.3.8/swim_protocol.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-05-15 20:45:51.000000 swim-protocol-0.3.8/swim_protocol.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-15 20:45:51.482389 swim-protocol-0.3.8/swimprotocol/
--rw-r--r--   0 runner    (1001) docker     (121)      263 2021-05-15 20:45:42.000000 swim-protocol-0.3.8/swimprotocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2040 2021-05-15 20:45:42.000000 swim-protocol-0.3.8/swimprotocol/address.py
--rw-r--r--   0 runner    (1001) docker     (121)     8504 2021-05-15 20:45:42.000000 swim-protocol-0.3.8/swimprotocol/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-15 20:45:51.486389 swim-protocol-0.3.8/swimprotocol/demo/
--rw-r--r--   0 runner    (1001) docker     (121)     2400 2021-05-15 20:45:42.000000 swim-protocol-0.3.8/swimprotocol/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      922 2021-05-15 20:45:42.000000 swim-protocol-0.3.8/swimprotocol/demo/changes.py
--rw-r--r--   0 runner    (1001) docker     (121)      484 2021-05-15 20:45:42.000000 swim-protocol-0.3.8/swimprotocol/demo/log.py
--rw-r--r--   0 runner    (1001) docker     (121)     4349 2021-05-15 20:45:42.000000 swim-protocol-0.3.8/swimprotocol/demo/screen.py
--rw-r--r--   0 runner    (1001) docker     (121)     2916 2021-05-15 20:45:42.000000 swim-protocol-0.3.8/swimprotocol/listener.py
--rw-r--r--   0 runner    (1001) docker     (121)    11647 2021-05-15 20:45:42.000000 swim-protocol-0.3.8/swimprotocol/members.py
--rw-r--r--   0 runner    (1001) docker     (121)     2326 2021-05-15 20:45:42.000000 swim-protocol-0.3.8/swimprotocol/packet.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-15 20:45:42.000000 swim-protocol-0.3.8/swimprotocol/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     3261 2021-05-15 20:45:42.000000 swim-protocol-0.3.8/swimprotocol/shuffle.py
--rw-r--r--   0 runner    (1001) docker     (121)     2334 2021-05-15 20:45:42.000000 swim-protocol-0.3.8/swimprotocol/sign.py
--rw-r--r--   0 runner    (1001) docker     (121)     1949 2021-05-15 20:45:42.000000 swim-protocol-0.3.8/swimprotocol/status.py
--rw-r--r--   0 runner    (1001) docker     (121)     2611 2021-05-15 20:45:42.000000 swim-protocol-0.3.8/swimprotocol/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-15 20:45:51.486389 swim-protocol-0.3.8/swimprotocol/udp/
--rw-r--r--   0 runner    (1001) docker     (121)     8469 2021-05-15 20:45:42.000000 swim-protocol-0.3.8/swimprotocol/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4127 2021-05-15 20:45:42.000000 swim-protocol-0.3.8/swimprotocol/udp/pack.py
--rw-r--r--   0 runner    (1001) docker     (121)     2978 2021-05-15 20:45:42.000000 swim-protocol-0.3.8/swimprotocol/udp/protocol.py
--rw-r--r--   0 runner    (1001) docker     (121)     9323 2021-05-15 20:45:42.000000 swim-protocol-0.3.8/swimprotocol/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-15 20:45:51.486389 swim-protocol-0.3.8/test/
--rw-r--r--   0 runner    (1001) docker     (121)     2367 2021-05-15 20:45:42.000000 swim-protocol-0.3.8/test/test_shuffle.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 23:57:37.859172 swim-protocol-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     8424 2022-07-27 23:57:37.859172 swim-protocol-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6667 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2022-07-27 23:57:37.859172 swim-protocol-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2322 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 23:57:37.855172 swim-protocol-0.3.9/swim_protocol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     8424 2022-07-27 23:57:37.000000 swim-protocol-0.3.9/swim_protocol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      738 2022-07-27 23:57:37.000000 swim-protocol-0.3.9/swim_protocol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-27 23:57:37.000000 swim-protocol-0.3.9/swim_protocol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2022-07-27 23:57:37.000000 swim-protocol-0.3.9/swim_protocol.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-07-27 23:57:37.000000 swim-protocol-0.3.9/swim_protocol.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 23:57:37.859172 swim-protocol-0.3.9/swimprotocol/
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2040 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/address.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8504 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 23:57:37.859172 swim-protocol-0.3.9/swimprotocol/demo/
+-rw-r--r--   0 runner    (1001) docker     (121)     2400 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      922 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/demo/changes.py
+-rw-r--r--   0 runner    (1001) docker     (121)      484 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/demo/log.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4397 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/demo/screen.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2916 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/listener.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11671 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/members.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2625 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/packet.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     3261 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2334 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/sign.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1949 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/status.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2611 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 23:57:37.859172 swim-protocol-0.3.9/swimprotocol/udp/
+-rw-r--r--   0 runner    (1001) docker     (121)     8469 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4127 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/udp/pack.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2978 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/udp/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9389 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 23:57:37.859172 swim-protocol-0.3.9/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     2367 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/test/test_shuffle.py
```

### Comparing `swim-protocol-0.3.8/LICENSE.md` & `swim-protocol-0.3.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `swim-protocol-0.3.8/PKG-INFO` & `swim-protocol-0.3.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,209 +1,210 @@
 Metadata-Version: 2.1
 Name: swim-protocol
-Version: 0.3.8
+Version: 0.3.9
 Summary: SWIM protocol implementation for exchanging cluster membership status and metadata.
 Home-page: https://github.com/icgood/swim-protocol/
 Author: Ian Good
 Author-email: ian@icgood.net
 License: MIT
-Description: swim-protocol
-        =============
-        
-        [SWIM protocol][0] implementation for exchanging cluster membership status and
-        metadata.
-        
-        [![build](https://github.com/icgood/swim-protocol/actions/workflows/python-package.yml/badge.svg)](https://github.com/icgood/swim-protocol/actions/workflows/python-package.yml)
-        [![Coverage Status](https://coveralls.io/repos/github/icgood/swim-protocol/badge.svg?branch=main)](https://coveralls.io/github/icgood/swim-protocol?branch=main)
-        [![PyPI](https://img.shields.io/pypi/v/swim-protocol.svg)](https://pypi.python.org/pypi/swim-protocol)
-        [![PyPI](https://img.shields.io/pypi/pyversions/swim-protocol.svg)](https://pypi.python.org/pypi/swim-protocol)
-        [![PyPI](https://img.shields.io/pypi/l/swim-protocol.svg)](https://pypi.python.org/pypi/swim-protocol)
-        
-        This library is intended to fit into an [asyncio][1] event loop to help
-        synchronize a distributed group of processes.
-        
-        #### [Introduction](https://icgood.github.io/swim-protocol/intro.html)
-        
-        #### [API Documentation](https://icgood.github.io/swim-protocol/)
-        
-        ## Install and Usage
-        
-        ```console
-        $ pip install swim-protocol
-        ```
-        
-        #### Running the Demo
-        
-        There is a [demo][2] application included as a reference implementation. Try it
-        out by running the following, each from a new terminal window, and use _Ctrl-C_
-        to exit:
-        
-        ```console
-        $ swim-protocol-demo -c --name 127.0.0.1:2001 --peer 127.0.0.1:2003 --metadata name one
-        $ swim-protocol-demo -c --name 127.0.0.1:2002 --peer 127.0.0.1:2001 --metadata name two
-        $ swim-protocol-demo -c --name 127.0.0.1:2003 --peer 127.0.0.1:2001 --metadata name three
-        $ swim-protocol-demo -c --name 127.0.0.1:2004 --peer 127.0.0.1:2003 --metadata name four
-        ```
-        
-        Typing in any window will disseminate what has been typed across the cluster
-        with [eventual consistency][6].
-        
-        ![swim-protocol-demo](https://user-images.githubusercontent.com/438413/117895781-13f6b400-b28d-11eb-997d-d8b9dbc455cb.gif)
-        
-        ### Getting Started
-        
-        First you should create a new [UdpConfig][100] object:
-        
-        ```python
-        from swimprotocol.udp import UdpConfig
-        
-        config = UdpConfig(local_name='127.0.0.1:2001',
-                           local_metadata={'name': b'one'},
-                           peers=['127.0.0.1:2002'])
-        ```
-        
-        All other config arguments have default values, which are tuned somewhat
-        arbitrarily with a small cluster of 3-4 members in mind.
-        
-        Now you can create the cluster members manager and transport layer, and enter
-        the event loop:
-        
-        ```python
-        from contextlib import AsyncExitStack
-        from swimprotocol.members import Members
-        from swimprotocol.udp import UdpTransport
-        
-        transport = UdpTransport(config)
-        members = Members(config)
-        async with AsyncExitStack() as stack:
-            worker = await stack.enter_async_context(transport.enter(members))
-            await worker.run()  # or schedule as a task
-        ```
-        
-        These snippets demonstrate the UDP transport layer directly. For a more generic
-        approach that uses [argparse][11] and [load_transport][12], check out the
-        [demo][2].
-        
-        If your application is deployed as a [Docker Service][13], the [UdpConfig][100]
-        `discovery=True` keyword argument can be used to discover configuration based
-        on the service name. See the [documentation][14] for more comprehensive usage.
-        
-        ### Checking Members
-        
-        The [Members][101] object provides a few ways to check on the cluster and its
-        members:
-        
-        ```python
-        for member in members.non_local:
-            # all other known cluster members
-            print(member.name, member.status, member.metadata)
-        
-        from swimprotocol.status import Status
-        for member in members.get_status(Status.AVAILABLE):
-            # all cluster members except offline
-            print(member.name, member.status, member.metadata)
-        ```
-        
-        Alternatively, listen for status or metadata changes on all members:
-        
-        ```python
-        from swimprotocol.member import Member
-        
-        async def _updated(member: Member) -> None:
-            print('updated:', member.name, member.status, member.metadata)
-        
-        async with AsyncExitStack() as stack:
-            # ...
-            stack.enter_context(members.listener.on_notify(_updated))
-        ```
-        
-        ### UDP Transport Security
-        
-        The [UdpTransport][102] transport layer (the only included transport
-        implementation) uses salted [hmac][7] digests to sign each UDP packet payload.
-        Any UDP packets received that are malformed or have an invalid signature are
-        *silently* ignored. The eventual consistency model should recover from packet
-        loss.
-        
-        The signatures rely on a [shared secret][8] between all cluster members, given
-        as the `secret=b'...'` argument to the [Config][100] constructor. If
-        `secret=None` is used, it defaults to [`uuid.getnode()`][9] but this is **not
-        secure** for production setups unless all sockets are bound to a local loopback
-        interface.
-        
-        The cluster member metadata is **not** encrypted during transmission, so only
-        private networks should be used if metadata includes any secret data, or that
-        secret data should be encrypted separately by the application. Also be aware
-        that low [MTU][10] sizes on public networks may affect the ability to
-        synchronize larger amounts of metadata.
-        
-        ## Development
-        
-        First off, I suggest activating a [venv][3]. Then, install the development
-        requirements and a local link to the *swim-protocol* package:
-        
-        ```
-        $ pip install -r requirements-dev.txt
-        ```
-        
-        ### Type Hinting
-        
-        This project makes heavy use of Python's [type hinting][4] system, with the
-        intention of a clean run of [mypy][5]:
-        
-        ```console
-        $ mypy
-        ```
-        
-        No code contribution will be accepted unless it makes every effort to use type
-        hinting to the extent possible and common in the rest of the codebase.
-        
-        [0]: https://www.cs.cornell.edu/projects/Quicksilver/public_pdfs/SWIM.pdf
-        [1]: https://docs.python.org/3/library/asyncio.html
-        [2]: https://github.com/icgood/swim-protocol/blob/main/swimprotocol/demo/__init__.py
-        [3]: https://docs.python.org/3/library/venv.html
-        [4]: https://docs.python.org/3/library/typing.html
-        [5]: http://mypy-lang.org/
-        [6]: https://en.wikipedia.org/wiki/Eventual_consistency
-        [7]: https://docs.python.org/3/library/hmac.html
-        [8]: https://en.wikipedia.org/wiki/Shared_secret
-        [9]: https://docs.python.org/3/library/uuid.html#uuid.getnode
-        [10]: https://en.wikipedia.org/wiki/Maximum_transmission_unit
-        [11]: https://docs.python.org/3/library/argparse.html
-        [12]: https://icgood.github.io/swim-protocol/swimprotocol.html#swimprotocol.transport.load_transport
-        [13]: https://docs.docker.com/engine/swarm/how-swarm-mode-works/services/
-        [14]: https://icgood.github.io/swim-protocol/swimprotocol.udp.html#docker-services
-        
-        [100]: https://icgood.github.io/swim-protocol/swimprotocol.udp.html#swimprotocol.udp.UdpConfig
-        [101]: https://icgood.github.io/swim-protocol/swimprotocol.html#swimprotocol.members.Member
-        [102]: https://icgood.github.io/swim-protocol/swimprotocol.udp.html#swimprotocol.udp.UdpTransport
-        ## MIT License
-        
-        Copyright (c) 2021 Ian Good
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+swim-protocol
+=============
+
+[SWIM protocol][0] implementation for exchanging cluster membership status and
+metadata.
+
+[![build](https://github.com/icgood/swim-protocol/actions/workflows/python-package.yml/badge.svg)](https://github.com/icgood/swim-protocol/actions/workflows/python-package.yml)
+[![Coverage Status](https://coveralls.io/repos/github/icgood/swim-protocol/badge.svg?branch=main)](https://coveralls.io/github/icgood/swim-protocol?branch=main)
+[![PyPI](https://img.shields.io/pypi/v/swim-protocol.svg)](https://pypi.python.org/pypi/swim-protocol)
+[![PyPI](https://img.shields.io/pypi/pyversions/swim-protocol.svg)](https://pypi.python.org/pypi/swim-protocol)
+[![PyPI](https://img.shields.io/pypi/l/swim-protocol.svg)](https://pypi.python.org/pypi/swim-protocol)
+
+This library is intended to fit into an [asyncio][1] event loop to help
+synchronize a distributed group of processes.
+
+#### [Introduction](https://icgood.github.io/swim-protocol/intro.html)
+
+#### [API Documentation](https://icgood.github.io/swim-protocol/)
+
+## Install and Usage
+
+```console
+$ pip install swim-protocol
+```
+
+#### Running the Demo
+
+There is a [demo][2] application included as a reference implementation. Try it
+out by running the following, each from a new terminal window, and use _Ctrl-C_
+to exit:
+
+```console
+$ swim-protocol-demo -c --name 127.0.0.1:2001 --peer 127.0.0.1:2003 --metadata name one
+$ swim-protocol-demo -c --name 127.0.0.1:2002 --peer 127.0.0.1:2001 --metadata name two
+$ swim-protocol-demo -c --name 127.0.0.1:2003 --peer 127.0.0.1:2001 --metadata name three
+$ swim-protocol-demo -c --name 127.0.0.1:2004 --peer 127.0.0.1:2003 --metadata name four
+```
+
+Typing in any window will disseminate what has been typed across the cluster
+with [eventual consistency][6].
+
+![swim-protocol-demo](https://user-images.githubusercontent.com/438413/117895781-13f6b400-b28d-11eb-997d-d8b9dbc455cb.gif)
+
+### Getting Started
+
+First you should create a new [UdpConfig][100] object:
+
+```python
+from swimprotocol.udp import UdpConfig
+
+config = UdpConfig(local_name='127.0.0.1:2001',
+                   local_metadata={'name': b'one'},
+                   peers=['127.0.0.1:2002'])
+```
+
+All other config arguments have default values, which are tuned somewhat
+arbitrarily with a small cluster of 3-4 members in mind.
+
+Now you can create the cluster members manager and transport layer, and enter
+the event loop:
+
+```python
+from contextlib import AsyncExitStack
+from swimprotocol.members import Members
+from swimprotocol.udp import UdpTransport
+
+transport = UdpTransport(config)
+members = Members(config)
+async with AsyncExitStack() as stack:
+    worker = await stack.enter_async_context(transport.enter(members))
+    await worker.run()  # or schedule as a task
+```
+
+These snippets demonstrate the UDP transport layer directly. For a more generic
+approach that uses [argparse][11] and [load_transport][12], check out the
+[demo][2].
+
+If your application is deployed as a [Docker Service][13], the [UdpConfig][100]
+`discovery=True` keyword argument can be used to discover configuration based
+on the service name. See the [documentation][14] for more comprehensive usage.
+
+### Checking Members
+
+The [Members][101] object provides a few ways to check on the cluster and its
+members:
+
+```python
+for member in members.non_local:
+    # all other known cluster members
+    print(member.name, member.status, member.metadata)
+
+from swimprotocol.status import Status
+for member in members.get_status(Status.AVAILABLE):
+    # all cluster members except offline
+    print(member.name, member.status, member.metadata)
+```
+
+Alternatively, listen for status or metadata changes on all members:
+
+```python
+from swimprotocol.member import Member
+
+async def _updated(member: Member) -> None:
+    print('updated:', member.name, member.status, member.metadata)
+
+async with AsyncExitStack() as stack:
+    # ...
+    stack.enter_context(members.listener.on_notify(_updated))
+```
+
+### UDP Transport Security
+
+The [UdpTransport][102] transport layer (the only included transport
+implementation) uses salted [hmac][7] digests to sign each UDP packet payload.
+Any UDP packets received that are malformed or have an invalid signature are
+*silently* ignored. The eventual consistency model should recover from packet
+loss.
+
+The signatures rely on a [shared secret][8] between all cluster members, given
+as the `secret=b'...'` argument to the [Config][100] constructor. If
+`secret=None` is used, it defaults to [`uuid.getnode()`][9] but this is **not
+secure** for production setups unless all sockets are bound to a local loopback
+interface.
+
+The cluster member metadata is **not** encrypted during transmission, so only
+private networks should be used if metadata includes any secret data, or that
+secret data should be encrypted separately by the application. Also be aware
+that low [MTU][10] sizes on public networks may affect the ability to
+synchronize larger amounts of metadata.
+
+## Development
+
+First off, I suggest activating a [venv][3]. Then, install the development
+requirements and a local link to the *swim-protocol* package:
+
+```
+$ pip install -r requirements-dev.txt
+```
+
+### Type Hinting
+
+This project makes heavy use of Python's [type hinting][4] system, with the
+intention of a clean run of [mypy][5]:
+
+```console
+$ mypy
+```
+
+No code contribution will be accepted unless it makes every effort to use type
+hinting to the extent possible and common in the rest of the codebase.
+
+[0]: https://www.cs.cornell.edu/projects/Quicksilver/public_pdfs/SWIM.pdf
+[1]: https://docs.python.org/3/library/asyncio.html
+[2]: https://github.com/icgood/swim-protocol/blob/main/swimprotocol/demo/__init__.py
+[3]: https://docs.python.org/3/library/venv.html
+[4]: https://docs.python.org/3/library/typing.html
+[5]: http://mypy-lang.org/
+[6]: https://en.wikipedia.org/wiki/Eventual_consistency
+[7]: https://docs.python.org/3/library/hmac.html
+[8]: https://en.wikipedia.org/wiki/Shared_secret
+[9]: https://docs.python.org/3/library/uuid.html#uuid.getnode
+[10]: https://en.wikipedia.org/wiki/Maximum_transmission_unit
+[11]: https://docs.python.org/3/library/argparse.html
+[12]: https://icgood.github.io/swim-protocol/swimprotocol.html#swimprotocol.transport.load_transport
+[13]: https://docs.docker.com/engine/swarm/how-swarm-mode-works/services/
+[14]: https://icgood.github.io/swim-protocol/swimprotocol.udp.html#docker-services
+
+[100]: https://icgood.github.io/swim-protocol/swimprotocol.udp.html#swimprotocol.udp.UdpConfig
+[101]: https://icgood.github.io/swim-protocol/swimprotocol.html#swimprotocol.members.Member
+[102]: https://icgood.github.io/swim-protocol/swimprotocol.udp.html#swimprotocol.udp.UdpTransport
+## MIT License
+
+Copyright (c) 2021 Ian Good
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `swim-protocol-0.3.8/README.md` & `swim-protocol-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `swim-protocol-0.3.8/setup.py` & `swim-protocol-0.3.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2021 Ian C. Good
+# Copyright (c) 2022 Ian C. Good
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -15,39 +15,40 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
-from setuptools import setup, find_packages  # type: ignore
+from setuptools import setup, find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 with open('LICENSE.md') as f:
     license = f.read()
 
 setup(name='swim-protocol',
-      version='0.3.8',
+      version='0.3.9',
       author='Ian Good',
       author_email='ian@icgood.net',
       description='SWIM protocol implementation for exchanging cluster '
                   'membership status and metadata.',
       long_description=readme + license,
       long_description_content_type='text/markdown',
       license='MIT',
       url='https://github.com/icgood/swim-protocol/',
       classifiers=[
           'Development Status :: 3 - Alpha',
           'Intended Audience :: Developers',
           'Intended Audience :: Information Technology',
           'License :: OSI Approved :: MIT License',
           'Programming Language :: Python',
-          'Programming Language :: Python :: 3.9'],
+          'Programming Language :: Python :: 3.9',
+          'Programming Language :: Python :: 3.10'],
       python_requires='~=3.9',
       include_package_data=True,
       packages=find_packages(),
       entry_points={
           'console_scripts': [
               'swim-protocol-demo = swimprotocol.demo:main'],
           'swimprotocol.transport': [
```

### Comparing `swim-protocol-0.3.8/swim_protocol.egg-info/PKG-INFO` & `swim-protocol-0.3.9/swim_protocol.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,209 +1,210 @@
 Metadata-Version: 2.1
 Name: swim-protocol
-Version: 0.3.8
+Version: 0.3.9
 Summary: SWIM protocol implementation for exchanging cluster membership status and metadata.
 Home-page: https://github.com/icgood/swim-protocol/
 Author: Ian Good
 Author-email: ian@icgood.net
 License: MIT
-Description: swim-protocol
-        =============
-        
-        [SWIM protocol][0] implementation for exchanging cluster membership status and
-        metadata.
-        
-        [![build](https://github.com/icgood/swim-protocol/actions/workflows/python-package.yml/badge.svg)](https://github.com/icgood/swim-protocol/actions/workflows/python-package.yml)
-        [![Coverage Status](https://coveralls.io/repos/github/icgood/swim-protocol/badge.svg?branch=main)](https://coveralls.io/github/icgood/swim-protocol?branch=main)
-        [![PyPI](https://img.shields.io/pypi/v/swim-protocol.svg)](https://pypi.python.org/pypi/swim-protocol)
-        [![PyPI](https://img.shields.io/pypi/pyversions/swim-protocol.svg)](https://pypi.python.org/pypi/swim-protocol)
-        [![PyPI](https://img.shields.io/pypi/l/swim-protocol.svg)](https://pypi.python.org/pypi/swim-protocol)
-        
-        This library is intended to fit into an [asyncio][1] event loop to help
-        synchronize a distributed group of processes.
-        
-        #### [Introduction](https://icgood.github.io/swim-protocol/intro.html)
-        
-        #### [API Documentation](https://icgood.github.io/swim-protocol/)
-        
-        ## Install and Usage
-        
-        ```console
-        $ pip install swim-protocol
-        ```
-        
-        #### Running the Demo
-        
-        There is a [demo][2] application included as a reference implementation. Try it
-        out by running the following, each from a new terminal window, and use _Ctrl-C_
-        to exit:
-        
-        ```console
-        $ swim-protocol-demo -c --name 127.0.0.1:2001 --peer 127.0.0.1:2003 --metadata name one
-        $ swim-protocol-demo -c --name 127.0.0.1:2002 --peer 127.0.0.1:2001 --metadata name two
-        $ swim-protocol-demo -c --name 127.0.0.1:2003 --peer 127.0.0.1:2001 --metadata name three
-        $ swim-protocol-demo -c --name 127.0.0.1:2004 --peer 127.0.0.1:2003 --metadata name four
-        ```
-        
-        Typing in any window will disseminate what has been typed across the cluster
-        with [eventual consistency][6].
-        
-        ![swim-protocol-demo](https://user-images.githubusercontent.com/438413/117895781-13f6b400-b28d-11eb-997d-d8b9dbc455cb.gif)
-        
-        ### Getting Started
-        
-        First you should create a new [UdpConfig][100] object:
-        
-        ```python
-        from swimprotocol.udp import UdpConfig
-        
-        config = UdpConfig(local_name='127.0.0.1:2001',
-                           local_metadata={'name': b'one'},
-                           peers=['127.0.0.1:2002'])
-        ```
-        
-        All other config arguments have default values, which are tuned somewhat
-        arbitrarily with a small cluster of 3-4 members in mind.
-        
-        Now you can create the cluster members manager and transport layer, and enter
-        the event loop:
-        
-        ```python
-        from contextlib import AsyncExitStack
-        from swimprotocol.members import Members
-        from swimprotocol.udp import UdpTransport
-        
-        transport = UdpTransport(config)
-        members = Members(config)
-        async with AsyncExitStack() as stack:
-            worker = await stack.enter_async_context(transport.enter(members))
-            await worker.run()  # or schedule as a task
-        ```
-        
-        These snippets demonstrate the UDP transport layer directly. For a more generic
-        approach that uses [argparse][11] and [load_transport][12], check out the
-        [demo][2].
-        
-        If your application is deployed as a [Docker Service][13], the [UdpConfig][100]
-        `discovery=True` keyword argument can be used to discover configuration based
-        on the service name. See the [documentation][14] for more comprehensive usage.
-        
-        ### Checking Members
-        
-        The [Members][101] object provides a few ways to check on the cluster and its
-        members:
-        
-        ```python
-        for member in members.non_local:
-            # all other known cluster members
-            print(member.name, member.status, member.metadata)
-        
-        from swimprotocol.status import Status
-        for member in members.get_status(Status.AVAILABLE):
-            # all cluster members except offline
-            print(member.name, member.status, member.metadata)
-        ```
-        
-        Alternatively, listen for status or metadata changes on all members:
-        
-        ```python
-        from swimprotocol.member import Member
-        
-        async def _updated(member: Member) -> None:
-            print('updated:', member.name, member.status, member.metadata)
-        
-        async with AsyncExitStack() as stack:
-            # ...
-            stack.enter_context(members.listener.on_notify(_updated))
-        ```
-        
-        ### UDP Transport Security
-        
-        The [UdpTransport][102] transport layer (the only included transport
-        implementation) uses salted [hmac][7] digests to sign each UDP packet payload.
-        Any UDP packets received that are malformed or have an invalid signature are
-        *silently* ignored. The eventual consistency model should recover from packet
-        loss.
-        
-        The signatures rely on a [shared secret][8] between all cluster members, given
-        as the `secret=b'...'` argument to the [Config][100] constructor. If
-        `secret=None` is used, it defaults to [`uuid.getnode()`][9] but this is **not
-        secure** for production setups unless all sockets are bound to a local loopback
-        interface.
-        
-        The cluster member metadata is **not** encrypted during transmission, so only
-        private networks should be used if metadata includes any secret data, or that
-        secret data should be encrypted separately by the application. Also be aware
-        that low [MTU][10] sizes on public networks may affect the ability to
-        synchronize larger amounts of metadata.
-        
-        ## Development
-        
-        First off, I suggest activating a [venv][3]. Then, install the development
-        requirements and a local link to the *swim-protocol* package:
-        
-        ```
-        $ pip install -r requirements-dev.txt
-        ```
-        
-        ### Type Hinting
-        
-        This project makes heavy use of Python's [type hinting][4] system, with the
-        intention of a clean run of [mypy][5]:
-        
-        ```console
-        $ mypy
-        ```
-        
-        No code contribution will be accepted unless it makes every effort to use type
-        hinting to the extent possible and common in the rest of the codebase.
-        
-        [0]: https://www.cs.cornell.edu/projects/Quicksilver/public_pdfs/SWIM.pdf
-        [1]: https://docs.python.org/3/library/asyncio.html
-        [2]: https://github.com/icgood/swim-protocol/blob/main/swimprotocol/demo/__init__.py
-        [3]: https://docs.python.org/3/library/venv.html
-        [4]: https://docs.python.org/3/library/typing.html
-        [5]: http://mypy-lang.org/
-        [6]: https://en.wikipedia.org/wiki/Eventual_consistency
-        [7]: https://docs.python.org/3/library/hmac.html
-        [8]: https://en.wikipedia.org/wiki/Shared_secret
-        [9]: https://docs.python.org/3/library/uuid.html#uuid.getnode
-        [10]: https://en.wikipedia.org/wiki/Maximum_transmission_unit
-        [11]: https://docs.python.org/3/library/argparse.html
-        [12]: https://icgood.github.io/swim-protocol/swimprotocol.html#swimprotocol.transport.load_transport
-        [13]: https://docs.docker.com/engine/swarm/how-swarm-mode-works/services/
-        [14]: https://icgood.github.io/swim-protocol/swimprotocol.udp.html#docker-services
-        
-        [100]: https://icgood.github.io/swim-protocol/swimprotocol.udp.html#swimprotocol.udp.UdpConfig
-        [101]: https://icgood.github.io/swim-protocol/swimprotocol.html#swimprotocol.members.Member
-        [102]: https://icgood.github.io/swim-protocol/swimprotocol.udp.html#swimprotocol.udp.UdpTransport
-        ## MIT License
-        
-        Copyright (c) 2021 Ian Good
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+swim-protocol
+=============
+
+[SWIM protocol][0] implementation for exchanging cluster membership status and
+metadata.
+
+[![build](https://github.com/icgood/swim-protocol/actions/workflows/python-package.yml/badge.svg)](https://github.com/icgood/swim-protocol/actions/workflows/python-package.yml)
+[![Coverage Status](https://coveralls.io/repos/github/icgood/swim-protocol/badge.svg?branch=main)](https://coveralls.io/github/icgood/swim-protocol?branch=main)
+[![PyPI](https://img.shields.io/pypi/v/swim-protocol.svg)](https://pypi.python.org/pypi/swim-protocol)
+[![PyPI](https://img.shields.io/pypi/pyversions/swim-protocol.svg)](https://pypi.python.org/pypi/swim-protocol)
+[![PyPI](https://img.shields.io/pypi/l/swim-protocol.svg)](https://pypi.python.org/pypi/swim-protocol)
+
+This library is intended to fit into an [asyncio][1] event loop to help
+synchronize a distributed group of processes.
+
+#### [Introduction](https://icgood.github.io/swim-protocol/intro.html)
+
+#### [API Documentation](https://icgood.github.io/swim-protocol/)
+
+## Install and Usage
+
+```console
+$ pip install swim-protocol
+```
+
+#### Running the Demo
+
+There is a [demo][2] application included as a reference implementation. Try it
+out by running the following, each from a new terminal window, and use _Ctrl-C_
+to exit:
+
+```console
+$ swim-protocol-demo -c --name 127.0.0.1:2001 --peer 127.0.0.1:2003 --metadata name one
+$ swim-protocol-demo -c --name 127.0.0.1:2002 --peer 127.0.0.1:2001 --metadata name two
+$ swim-protocol-demo -c --name 127.0.0.1:2003 --peer 127.0.0.1:2001 --metadata name three
+$ swim-protocol-demo -c --name 127.0.0.1:2004 --peer 127.0.0.1:2003 --metadata name four
+```
+
+Typing in any window will disseminate what has been typed across the cluster
+with [eventual consistency][6].
+
+![swim-protocol-demo](https://user-images.githubusercontent.com/438413/117895781-13f6b400-b28d-11eb-997d-d8b9dbc455cb.gif)
+
+### Getting Started
+
+First you should create a new [UdpConfig][100] object:
+
+```python
+from swimprotocol.udp import UdpConfig
+
+config = UdpConfig(local_name='127.0.0.1:2001',
+                   local_metadata={'name': b'one'},
+                   peers=['127.0.0.1:2002'])
+```
+
+All other config arguments have default values, which are tuned somewhat
+arbitrarily with a small cluster of 3-4 members in mind.
+
+Now you can create the cluster members manager and transport layer, and enter
+the event loop:
+
+```python
+from contextlib import AsyncExitStack
+from swimprotocol.members import Members
+from swimprotocol.udp import UdpTransport
+
+transport = UdpTransport(config)
+members = Members(config)
+async with AsyncExitStack() as stack:
+    worker = await stack.enter_async_context(transport.enter(members))
+    await worker.run()  # or schedule as a task
+```
+
+These snippets demonstrate the UDP transport layer directly. For a more generic
+approach that uses [argparse][11] and [load_transport][12], check out the
+[demo][2].
+
+If your application is deployed as a [Docker Service][13], the [UdpConfig][100]
+`discovery=True` keyword argument can be used to discover configuration based
+on the service name. See the [documentation][14] for more comprehensive usage.
+
+### Checking Members
+
+The [Members][101] object provides a few ways to check on the cluster and its
+members:
+
+```python
+for member in members.non_local:
+    # all other known cluster members
+    print(member.name, member.status, member.metadata)
+
+from swimprotocol.status import Status
+for member in members.get_status(Status.AVAILABLE):
+    # all cluster members except offline
+    print(member.name, member.status, member.metadata)
+```
+
+Alternatively, listen for status or metadata changes on all members:
+
+```python
+from swimprotocol.member import Member
+
+async def _updated(member: Member) -> None:
+    print('updated:', member.name, member.status, member.metadata)
+
+async with AsyncExitStack() as stack:
+    # ...
+    stack.enter_context(members.listener.on_notify(_updated))
+```
+
+### UDP Transport Security
+
+The [UdpTransport][102] transport layer (the only included transport
+implementation) uses salted [hmac][7] digests to sign each UDP packet payload.
+Any UDP packets received that are malformed or have an invalid signature are
+*silently* ignored. The eventual consistency model should recover from packet
+loss.
+
+The signatures rely on a [shared secret][8] between all cluster members, given
+as the `secret=b'...'` argument to the [Config][100] constructor. If
+`secret=None` is used, it defaults to [`uuid.getnode()`][9] but this is **not
+secure** for production setups unless all sockets are bound to a local loopback
+interface.
+
+The cluster member metadata is **not** encrypted during transmission, so only
+private networks should be used if metadata includes any secret data, or that
+secret data should be encrypted separately by the application. Also be aware
+that low [MTU][10] sizes on public networks may affect the ability to
+synchronize larger amounts of metadata.
+
+## Development
+
+First off, I suggest activating a [venv][3]. Then, install the development
+requirements and a local link to the *swim-protocol* package:
+
+```
+$ pip install -r requirements-dev.txt
+```
+
+### Type Hinting
+
+This project makes heavy use of Python's [type hinting][4] system, with the
+intention of a clean run of [mypy][5]:
+
+```console
+$ mypy
+```
+
+No code contribution will be accepted unless it makes every effort to use type
+hinting to the extent possible and common in the rest of the codebase.
+
+[0]: https://www.cs.cornell.edu/projects/Quicksilver/public_pdfs/SWIM.pdf
+[1]: https://docs.python.org/3/library/asyncio.html
+[2]: https://github.com/icgood/swim-protocol/blob/main/swimprotocol/demo/__init__.py
+[3]: https://docs.python.org/3/library/venv.html
+[4]: https://docs.python.org/3/library/typing.html
+[5]: http://mypy-lang.org/
+[6]: https://en.wikipedia.org/wiki/Eventual_consistency
+[7]: https://docs.python.org/3/library/hmac.html
+[8]: https://en.wikipedia.org/wiki/Shared_secret
+[9]: https://docs.python.org/3/library/uuid.html#uuid.getnode
+[10]: https://en.wikipedia.org/wiki/Maximum_transmission_unit
+[11]: https://docs.python.org/3/library/argparse.html
+[12]: https://icgood.github.io/swim-protocol/swimprotocol.html#swimprotocol.transport.load_transport
+[13]: https://docs.docker.com/engine/swarm/how-swarm-mode-works/services/
+[14]: https://icgood.github.io/swim-protocol/swimprotocol.udp.html#docker-services
+
+[100]: https://icgood.github.io/swim-protocol/swimprotocol.udp.html#swimprotocol.udp.UdpConfig
+[101]: https://icgood.github.io/swim-protocol/swimprotocol.html#swimprotocol.members.Member
+[102]: https://icgood.github.io/swim-protocol/swimprotocol.udp.html#swimprotocol.udp.UdpTransport
+## MIT License
+
+Copyright (c) 2021 Ian Good
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `swim-protocol-0.3.8/swim_protocol.egg-info/SOURCES.txt` & `swim-protocol-0.3.9/swim_protocol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swim-protocol-0.3.8/swimprotocol/address.py` & `swim-protocol-0.3.9/swimprotocol/address.py`

 * *Files identical despite different names*

### Comparing `swim-protocol-0.3.8/swimprotocol/config.py` & `swim-protocol-0.3.9/swimprotocol/config.py`

 * *Files identical despite different names*

### Comparing `swim-protocol-0.3.8/swimprotocol/demo/__init__.py` & `swim-protocol-0.3.9/swimprotocol/demo/__init__.py`

 * *Files identical despite different names*

### Comparing `swim-protocol-0.3.8/swimprotocol/demo/changes.py` & `swim-protocol-0.3.9/swimprotocol/demo/changes.py`

 * *Files identical despite different names*

### Comparing `swim-protocol-0.3.8/swimprotocol/demo/screen.py` & `swim-protocol-0.3.9/swimprotocol/demo/screen.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import annotations
 
 import asyncio
 import curses
 import string
 from contextlib import AsyncExitStack
 from curses import wrapper
+from functools import partial
 from threading import Event, Condition
 from typing import Final, Any
 
 from ..members import Member, Members
 from ..status import Status
 
 __all__ = ['run_screen']
@@ -109,18 +110,18 @@
                 ch = stdscr.getch()
                 if _is_printable(ch):
                     typed += bytes([ch])
                     typed = typed[-30:]
                     self._set_typed(typed)
 
     async def run_thread(self) -> None:
-        await asyncio.to_thread(wrapper, self.main)
+        await asyncio.to_thread(partial(wrapper, self.main))
 
 
 def run_screen(members: Members) -> AsyncExitStack:
     exit_stack = AsyncExitStack()
     screen = Screen(members)
     main_task = asyncio.create_task(screen.run_thread())
-    exit_stack.push_async_callback(asyncio.wait_for, main_task, None)
+    exit_stack.push_async_callback(partial(asyncio.wait_for, main_task, None))
     exit_stack.enter_context(members.listener.on_notify(screen.update))
     exit_stack.callback(screen.cancel)
     return exit_stack
```

### Comparing `swim-protocol-0.3.8/swimprotocol/listener.py` & `swim-protocol-0.3.9/swimprotocol/listener.py`

 * *Files identical despite different names*

### Comparing `swim-protocol-0.3.8/swimprotocol/members.py` & `swim-protocol-0.3.9/swimprotocol/members.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from collections.abc import Generator, Iterator, Mapping, Set
 from functools import total_ordering
 from typing import Final, Optional, Any
 from weakref import WeakKeyDictionary, WeakValueDictionary
 
 from .config import BaseConfig
 from .listener import Listener
+from .packet import Source
 from .shuffle import Shuffle, WeakShuffle
 from .status import Status
 
 __all__ = ['Member', 'Members']
 
 
 @total_ordering
@@ -56,16 +57,16 @@
     def __hash__(self) -> int:
         return hash(self.name)
 
     def __repr__(self) -> str:
         return f'Member<{self.name} {self.status.name}>'
 
     @property
-    def source(self) -> tuple[str, bytes]:
-        return self.name, self._validity
+    def source(self) -> Source:
+        return Source(self.name, self._validity)
 
     @property
     def clock(self) -> int:
         """The :term:`sequence clock` tracking changes distributed across the
         cluster.  This value is always increasing, as changes are made to the
         member status or metadata.
```

### Comparing `swim-protocol-0.3.8/swimprotocol/packet.py` & `swim-protocol-0.3.9/swimprotocol/packet.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,29 @@
 
 from collections.abc import Mapping
 from dataclasses import dataclass
 from typing import Optional
 
 from .status import Status
 
-__all__ = ['Packet', 'Ping', 'PingReq', 'Ack', 'Gossip', 'GossipAck']
+__all__ = ['Source', 'Packet', 'Ping', 'PingReq', 'Ack', 'Gossip', 'GossipAck']
+
+
+@dataclass(frozen=True)
+class Source:
+    """Uniquely identifies the local cluster member that created the packet.
+
+    Args:
+        name: The name of the local cluster member.
+        validity: Random bytestring used to detect non-unique *name* values.
+
+    """
+
+    name: str
+    validity: bytes
 
 
 @dataclass(frozen=True)
 class Packet:
     """Base class for a :term:`packet` sent between cluster members.
 
     :class:`~swimprotocol.transport.Transport` implementations may use these
@@ -19,15 +33,15 @@
     contents into another protocol.
 
     Args:
         source: The name of the local cluster member that created the packet.
 
     """
 
-    source: tuple[str, bytes]
+    source: Source
 
 
 @dataclass(frozen=True)
 class Ping(Packet):
     """Packets used for the SWIM protocol :term:`ping` operation, which do not
     explicitly contain any other information other than the *source*.
 
@@ -50,15 +64,14 @@
 
 @dataclass(frozen=True)
 class Ack(Packet):
     """Packets used for the SWIM protocol :term:`ack` response, which indicates
     that *source* is online.
 
     """
-
     pass
 
 
 @dataclass(frozen=True)
 class Gossip(Packet):
     """Packets used for SWIM protocol :term:`gossip`, which alert other members
     when a cluster member has changed status or metadata. This information is
```

### Comparing `swim-protocol-0.3.8/swimprotocol/shuffle.py` & `swim-protocol-0.3.9/swimprotocol/shuffle.py`

 * *Files identical despite different names*

### Comparing `swim-protocol-0.3.8/swimprotocol/sign.py` & `swim-protocol-0.3.9/swimprotocol/sign.py`

 * *Files identical despite different names*

### Comparing `swim-protocol-0.3.8/swimprotocol/status.py` & `swim-protocol-0.3.9/swimprotocol/status.py`

 * *Files identical despite different names*

### Comparing `swim-protocol-0.3.8/swimprotocol/transport.py` & `swim-protocol-0.3.9/swimprotocol/transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     Args:
         config: The cluster config object.
 
     """
 
     #: The :class:`~swimprotocol.config.BaseConfig` sub-class used by this
     #: transport.
-    config_type: ClassVar[type[ConfigT_co]]
+    config_type: ClassVar[type[BaseConfig]]
 
     def __init__(self, config: ConfigT_co) -> None:
         super().__init__()
         self.config: Final = config
 
     @abstractmethod
     def enter(self, members: Members) -> AbstractAsyncContextManager[Worker]:
```

### Comparing `swim-protocol-0.3.8/swimprotocol/udp/__init__.py` & `swim-protocol-0.3.9/swimprotocol/udp/__init__.py`

 * *Files identical despite different names*

### Comparing `swim-protocol-0.3.8/swimprotocol/udp/pack.py` & `swim-protocol-0.3.9/swimprotocol/udp/pack.py`

 * *Files identical despite different names*

### Comparing `swim-protocol-0.3.8/swimprotocol/udp/protocol.py` & `swim-protocol-0.3.9/swimprotocol/udp/protocol.py`

 * *Files identical despite different names*

### Comparing `swim-protocol-0.3.8/swimprotocol/worker.py` & `swim-protocol-0.3.9/swimprotocol/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,16 @@
         else:
             return []
 
     async def _run_handler(self) -> NoReturn:
         local = self.members.local
         while True:
             packet = await self.io.recv()
-            source = self.members.get(*packet.source)
+            source = self.members.get(packet.source.name,
+                                      packet.source.validity)
             if isinstance(packet, Ping):
                 await self.io.send(source, Ack(source=local.source))
             elif isinstance(packet, PingReq):
                 target = self.members.get(packet.target)
                 await self.io.send(target, Ping(source=local.source))
                 self._add_listening(source, target)
             elif isinstance(packet, Ack):
```

### Comparing `swim-protocol-0.3.8/test/test_shuffle.py` & `swim-protocol-0.3.9/test/test_shuffle.py`

 * *Files identical despite different names*

