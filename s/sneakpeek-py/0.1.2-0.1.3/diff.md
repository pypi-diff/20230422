# Comparing `tmp/sneakpeek_py-0.1.2.tar.gz` & `tmp/sneakpeek_py-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sneakpeek_py-0.1.2.tar", max compression
+gzip compressed data, was "sneakpeek_py-0.1.3.tar", max compression
```

## Comparing `sneakpeek_py-0.1.2.tar` & `sneakpeek_py-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,57 @@
--rw-r--r--   0        0        0       85 2023-04-02 10:58:33.945002 sneakpeek_py-0.1.2/README.md
--rw-r--r--   0        0        0     1753 2023-04-15 14:29:59.612255 sneakpeek_py-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2464 2023-04-14 20:55:18.205455 sneakpeek_py-0.1.2/sneakpeek/api.py
--rw-r--r--   0        0        0      726 2023-04-10 11:41:30.863384 sneakpeek_py-0.1.2/sneakpeek/lib/errors.py
--rw-r--r--   0        0        0     1325 2023-04-14 20:40:35.860617 sneakpeek_py-0.1.2/sneakpeek/lib/models.py
--rw-r--r--   0        0        0     4637 2023-04-15 13:21:03.582741 sneakpeek_py-0.1.2/sneakpeek/lib/queue.py
--rw-r--r--   0        0        0     2066 2023-04-15 13:19:12.546715 sneakpeek_py-0.1.2/sneakpeek/lib/storage/base.py
--rw-r--r--   0        0        0     9112 2023-04-15 13:20:08.681048 sneakpeek_py-0.1.2/sneakpeek/lib/storage/in_memory_storage.py
--rw-r--r--   0        0        0     8889 2023-04-15 13:20:22.015469 sneakpeek_py-0.1.2/sneakpeek/lib/storage/redis_storage.py
--rw-r--r--   0        0        0     1535 2023-04-15 08:35:07.840371 sneakpeek_py-0.1.2/sneakpeek/logging.py
--rw-r--r--   0        0        0     3291 2023-04-15 13:15:52.422916 sneakpeek_py-0.1.2/sneakpeek/metrics.py
--rw-r--r--   0        0        0     1338 2023-04-15 14:28:45.826848 sneakpeek_py-0.1.2/sneakpeek/plugins/proxy_plugin.py
--rw-r--r--   0        0        0     4209 2023-04-15 10:43:26.332501 sneakpeek_py-0.1.2/sneakpeek/plugins/rate_limiter_plugin.py
--rw-r--r--   0        0        0     2062 2023-04-15 10:43:18.016302 sneakpeek_py-0.1.2/sneakpeek/plugins/requests_logging_plugin.py
--rw-r--r--   0        0        0     3747 2023-04-15 10:43:12.817939 sneakpeek_py-0.1.2/sneakpeek/plugins/robots_txt_plugin.py
--rw-r--r--   0        0        0     1391 2023-04-15 14:24:15.543165 sneakpeek_py-0.1.2/sneakpeek/plugins/user_agent_injecter_plugin.py
--rw-r--r--   0        0        0      659 2023-04-15 07:08:31.686879 sneakpeek_py-0.1.2/sneakpeek/plugins/utils.py
--rw-r--r--   0        0        0     2910 2023-04-15 12:42:25.391509 sneakpeek_py-0.1.2/sneakpeek/runner.py
--rw-r--r--   0        0        0    10268 2023-04-15 13:39:19.486115 sneakpeek_py-0.1.2/sneakpeek/scheduler.py
--rw-r--r--   0        0        0      172 2023-04-14 20:22:32.213615 sneakpeek_py-0.1.2/sneakpeek/scraper_config.py
--rw-r--r--   0        0        0     5810 2023-04-15 10:36:17.814799 sneakpeek_py-0.1.2/sneakpeek/scraper_context.py
--rw-r--r--   0        0        0      282 2023-04-14 20:58:00.201559 sneakpeek_py-0.1.2/sneakpeek/scraper_handler.py
--rw-r--r--   0        0        0     3654 2023-04-15 14:02:33.345443 sneakpeek_py-0.1.2/sneakpeek/server.py
--rw-r--r--   0        0        0     3309 2023-04-15 13:39:24.072034 sneakpeek_py-0.1.2/sneakpeek/worker.py
--rw-r--r--   0        0        0     1805 1970-01-01 00:00:00.000000 sneakpeek_py-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       85 2023-04-02 10:58:33.945002 sneakpeek_py-0.1.3/README.md
+-rw-r--r--   0        0        0     1753 2023-04-22 18:37:18.956525 sneakpeek_py-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3483 2023-04-22 18:35:18.037503 sneakpeek_py-0.1.3/sneakpeek/api.py
+-rw-r--r--   0        0        0      726 2023-04-10 11:41:30.863384 sneakpeek_py-0.1.3/sneakpeek/lib/errors.py
+-rw-r--r--   0        0        0     1325 2023-04-14 20:40:35.860617 sneakpeek_py-0.1.3/sneakpeek/lib/models.py
+-rw-r--r--   0        0        0     4637 2023-04-16 16:40:10.652490 sneakpeek_py-0.1.3/sneakpeek/lib/queue.py
+-rw-r--r--   0        0        0     2141 2023-04-22 17:36:34.069286 sneakpeek_py-0.1.3/sneakpeek/lib/storage/base.py
+-rw-r--r--   0        0        0     9527 2023-04-22 17:37:37.160714 sneakpeek_py-0.1.3/sneakpeek/lib/storage/in_memory_storage.py
+-rw-r--r--   0        0        0     9153 2023-04-22 17:38:03.913301 sneakpeek_py-0.1.3/sneakpeek/lib/storage/redis_storage.py
+-rw-r--r--   0        0        0     1535 2023-04-15 08:35:07.840371 sneakpeek_py-0.1.3/sneakpeek/logging.py
+-rw-r--r--   0        0        0     3291 2023-04-15 13:15:52.422916 sneakpeek_py-0.1.3/sneakpeek/metrics.py
+-rw-r--r--   0        0        0     1338 2023-04-15 14:28:45.826848 sneakpeek_py-0.1.3/sneakpeek/plugins/proxy_plugin.py
+-rw-r--r--   0        0        0     4209 2023-04-15 10:43:26.332501 sneakpeek_py-0.1.3/sneakpeek/plugins/rate_limiter_plugin.py
+-rw-r--r--   0        0        0     2062 2023-04-15 10:43:18.016302 sneakpeek_py-0.1.3/sneakpeek/plugins/requests_logging_plugin.py
+-rw-r--r--   0        0        0     3747 2023-04-15 10:43:12.817939 sneakpeek_py-0.1.3/sneakpeek/plugins/robots_txt_plugin.py
+-rw-r--r--   0        0        0     1391 2023-04-15 14:24:15.543165 sneakpeek_py-0.1.3/sneakpeek/plugins/user_agent_injecter_plugin.py
+-rw-r--r--   0        0        0      659 2023-04-15 07:08:31.686879 sneakpeek_py-0.1.3/sneakpeek/plugins/utils.py
+-rw-r--r--   0        0        0     3344 2023-04-16 16:37:19.181274 sneakpeek_py-0.1.3/sneakpeek/runner.py
+-rw-r--r--   0        0        0    11264 2023-04-16 16:40:24.540096 sneakpeek_py-0.1.3/sneakpeek/scheduler.py
+-rw-r--r--   0        0        0      172 2023-04-14 20:22:32.213615 sneakpeek_py-0.1.3/sneakpeek/scraper_config.py
+-rw-r--r--   0        0        0     6956 2023-04-16 16:36:12.560412 sneakpeek_py-0.1.3/sneakpeek/scraper_context.py
+-rw-r--r--   0        0        0      282 2023-04-14 20:58:00.201559 sneakpeek_py-0.1.3/sneakpeek/scraper_handler.py
+-rw-r--r--   0        0        0     3654 2023-04-15 14:02:33.345443 sneakpeek_py-0.1.3/sneakpeek/server.py
+-rw-r--r--   0        0        0      550 2023-04-22 18:35:47.148387 sneakpeek_py-0.1.3/sneakpeek/static/assets/ErrorNotFound.9617f9a7.js
+-rw-r--r--   0        0        0    20436 2023-04-22 18:35:47.145054 sneakpeek_py-0.1.3/sneakpeek/static/assets/KFOkCnqEu92Fr1MmgVxIIzQ.34e9582c.woff
+-rw-r--r--   0        0        0    20544 2023-04-22 18:35:47.146248 sneakpeek_py-0.1.3/sneakpeek/static/assets/KFOlCnqEu92Fr1MmEU9fBBc-.9ce7f3ac.woff
+-rw-r--r--   0        0        0    20416 2023-04-22 18:35:47.146208 sneakpeek_py-0.1.3/sneakpeek/static/assets/KFOlCnqEu92Fr1MmSU5fBBc-.bf14c7d7.woff
+-rw-r--r--   0        0        0    20408 2023-04-22 18:35:47.146455 sneakpeek_py-0.1.3/sneakpeek/static/assets/KFOlCnqEu92Fr1MmWUlfBBc-.e0fd57c0.woff
+-rw-r--r--   0        0        0    20424 2023-04-22 18:35:47.146125 sneakpeek_py-0.1.3/sneakpeek/static/assets/KFOlCnqEu92Fr1MmYUtfBBc-.f6537e32.woff
+-rw-r--r--   0        0        0    20344 2023-04-22 18:35:47.146188 sneakpeek_py-0.1.3/sneakpeek/static/assets/KFOmCnqEu92Fr1Mu4mxM.f2abf7fb.woff
+-rw-r--r--   0        0        0    24866 2023-04-22 18:35:47.146431 sneakpeek_py-0.1.3/sneakpeek/static/assets/MainLayout.06dc30a3.js
+-rw-r--r--   0        0        0      538 2023-04-22 18:35:47.148607 sneakpeek_py-0.1.3/sneakpeek/static/assets/NewScraperPage.abf42128.js
+-rw-r--r--   0        0        0    30651 2023-04-22 18:35:47.148410 sneakpeek_py-0.1.3/sneakpeek/static/assets/PriorityChip.61343a15.js
+-rw-r--r--   0        0        0      655 2023-04-22 18:35:47.146487 sneakpeek_py-0.1.3/sneakpeek/static/assets/QList.7f24c43e.js
+-rw-r--r--   0        0        0    76403 2023-04-22 18:35:47.148351 sneakpeek_py-0.1.3/sneakpeek/static/assets/QPage.6206ab40.js
+-rw-r--r--   0        0        0  1333182 2023-04-22 18:35:47.148573 sneakpeek_py-0.1.3/sneakpeek/static/assets/ScraperEditForm.197dd68f.js
+-rw-r--r--   0        0        0     3323 2023-04-22 18:35:47.148364 sneakpeek_py-0.1.3/sneakpeek/static/assets/ScraperEditForm.640de0df.css
+-rw-r--r--   0        0        0    26587 2023-04-22 18:35:47.148377 sneakpeek_py-0.1.3/sneakpeek/static/assets/ScraperPage.732b3035.js
+-rw-r--r--   0        0        0     2479 2023-04-22 18:35:47.148321 sneakpeek_py-0.1.3/sneakpeek/static/assets/ScrapersPage.06097019.js
+-rw-r--r--   0        0        0    11097 2023-04-22 18:35:47.146471 sneakpeek_py-0.1.3/sneakpeek/static/assets/api.8025d512.js
+-rw-r--r--   0        0        0   187208 2023-04-22 18:35:47.146352 sneakpeek_py-0.1.3/sneakpeek/static/assets/fa-brands-400.20c4a58b.ttf
+-rw-r--r--   0        0        0   108020 2023-04-22 18:35:47.146608 sneakpeek_py-0.1.3/sneakpeek/static/assets/fa-brands-400.74833209.woff2
+-rw-r--r--   0        0        0    63952 2023-04-22 18:35:47.146236 sneakpeek_py-0.1.3/sneakpeek/static/assets/fa-regular-400.528d022d.ttf
+-rw-r--r--   0        0        0    24948 2023-04-22 18:35:47.146154 sneakpeek_py-0.1.3/sneakpeek/static/assets/fa-regular-400.8e7e5ea1.woff2
+-rw-r--r--   0        0        0   394628 2023-04-22 18:35:47.146414 sneakpeek_py-0.1.3/sneakpeek/static/assets/fa-solid-900.67a65763.ttf
+-rw-r--r--   0        0        0   150124 2023-04-22 18:35:47.146277 sneakpeek_py-0.1.3/sneakpeek/static/assets/fa-solid-900.7152a693.woff2
+-rw-r--r--   0        0        0    10172 2023-04-22 18:35:47.146502 sneakpeek_py-0.1.3/sneakpeek/static/assets/fa-v4compatibility.0515a423.ttf
+-rw-r--r--   0        0        0     4564 2023-04-22 18:35:47.146294 sneakpeek_py-0.1.3/sneakpeek/static/assets/fa-v4compatibility.694a17c3.woff2
+-rw-r--r--   0        0        0   164912 2023-04-22 18:35:47.146665 sneakpeek_py-0.1.3/sneakpeek/static/assets/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.fd84f88b.woff
+-rw-r--r--   0        0        0   128616 2023-04-22 18:35:47.146319 sneakpeek_py-0.1.3/sneakpeek/static/assets/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.4a4dbc62.woff2
+-rw-r--r--   0        0        0   132320 2023-04-22 18:35:47.146538 sneakpeek_py-0.1.3/sneakpeek/static/assets/index.422cc3a0.js
+-rw-r--r--   0        0        0   307194 2023-04-22 18:35:47.148448 sneakpeek_py-0.1.3/sneakpeek/static/assets/index.99b1d043.css
+-rw-r--r--   0        0        0    64483 2023-04-22 18:35:46.776382 sneakpeek_py-0.1.3/sneakpeek/static/favicon.ico
+-rw-r--r--   0        0        0     2359 2023-04-22 18:35:46.776784 sneakpeek_py-0.1.3/sneakpeek/static/icons/favicon.png
+-rw-r--r--   0        0        0      659 2023-04-22 18:35:47.148589 sneakpeek_py-0.1.3/sneakpeek/static/index.html
+-rw-r--r--   0        0        0     3444 2023-04-16 14:06:00.425497 sneakpeek_py-0.1.3/sneakpeek/worker.py
+-rw-r--r--   0        0        0     1805 1970-01-01 00:00:00.000000 sneakpeek_py-0.1.3/PKG-INFO
```

### Comparing `sneakpeek_py-0.1.2/pyproject.toml` & `sneakpeek_py-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "sneakpeek-py"
 packages = [{ include = "sneakpeek" }]
-version = "0.1.2"
+version = "0.1.3"
 description = "Tool box for creating scrapers, so that you only focus on scraping logic"
 authors = ["Dan Yazovsky <daniil.yazovsky@gmail.com>"]
 maintainers = ["Dan Yazovsky <daniil.yazovsky@gmail.com>"]
 repository = "https://github.com/flulemon/sneakpeek"
 documentation = "https://github.com/flulemon/sneakpeek"
 homepage = "https://github.com/flulemon/sneakpeek"
 license = "BSD-3-Clause"
```

### Comparing `sneakpeek_py-0.1.2/sneakpeek/api.py` & `sneakpeek_py-0.1.3/sneakpeek/api.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,32 @@
+import pathlib
+
 import fastapi_jsonrpc as jsonrpc
 from fastapi import Body
+from fastapi.middleware.cors import CORSMiddleware
+from fastapi.staticfiles import StaticFiles
+from pydantic import BaseModel
 
 from sneakpeek.lib.errors import ScraperHasActiveRunError, ScraperNotFoundError
-from sneakpeek.lib.models import Scraper, ScraperRun, ScraperRunPriority
+from sneakpeek.lib.models import (
+    Scraper,
+    ScraperRun,
+    ScraperRunPriority,
+    ScraperSchedule,
+)
 from sneakpeek.lib.queue import Queue, QueueABC
 from sneakpeek.lib.storage.base import Storage
 from sneakpeek.scraper_handler import ScraperHandler
 
 
+class Priority(BaseModel):
+    name: str
+    value: int
+
+
 def get_public_api_entrypoint(
     storage: Storage,
     queue: Queue,
     handlers: list[ScraperHandler],
 ) -> jsonrpc.Entrypoint:
     entrypoint = jsonrpc.Entrypoint("/api/v1/jsonrpc")
 
@@ -54,18 +69,47 @@
     async def get_scraper_runs(scraper_id: int = Body(...)) -> list[ScraperRun]:
         return await storage.get_scraper_runs(scraper_id)
 
     @entrypoint.method()
     async def get_scraper_handlers() -> list[str]:
         return [handler.name for handler in handlers]
 
+    @entrypoint.method()
+    async def get_schedules() -> list[str]:
+        return [schedule.value for schedule in ScraperSchedule]
+
+    @entrypoint.method()
+    async def get_priorities() -> list[Priority]:
+        return [
+            Priority(name=priority.name, value=priority.value)
+            for priority in ScraperRunPriority
+        ]
+
+    @entrypoint.method()
+    async def is_read_only() -> bool:
+        return await storage.is_read_only()
+
     return entrypoint
 
 
 def create_api(
     storage: Storage,
     queue: QueueABC,
     handlers: list[ScraperHandler],
 ) -> jsonrpc.API:
     app = jsonrpc.API()
+    app.add_middleware(
+        CORSMiddleware,
+        allow_origins=["*"],
+        allow_methods=["*"],
+        allow_headers=["*"],
+    )
     app.bind_entrypoint(get_public_api_entrypoint(storage, queue, handlers))
+    app.mount(
+        "/",
+        StaticFiles(
+            directory=f"{pathlib.Path(__file__).parent.resolve()}/static",
+            html=True,
+        ),
+        name="html",
+    )
     return app
```

### Comparing `sneakpeek_py-0.1.2/sneakpeek/lib/errors.py` & `sneakpeek_py-0.1.3/sneakpeek/lib/errors.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.2/sneakpeek/lib/models.py` & `sneakpeek_py-0.1.3/sneakpeek/lib/models.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.2/sneakpeek/lib/queue.py` & `sneakpeek_py-0.1.3/sneakpeek/lib/queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
             return False
         activity_timestamps = [
             scraper_run.last_active_at,
             scraper_run.started_at,
             scraper_run.created_at,
         ]
         for ts in activity_timestamps:
-            if ts and ts - datetime.utcnow() > self._dead_timeout:
+            if ts and datetime.utcnow() - ts > self._dead_timeout:
                 return True
         return False
 
     async def _has_unfinished_runs(self, scraper_id: int):
         runs = await self._storage.get_scraper_runs(scraper_id)
         return any(
             run
```

### Comparing `sneakpeek_py-0.1.2/sneakpeek/lib/storage/base.py` & `sneakpeek_py-0.1.3/sneakpeek/lib/storage/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,7 +78,11 @@
         acquire_for: timedelta,
     ) -> Lease | None:
         ...
 
     @abstractmethod
     async def release_lease(self, lease_name: str, owner_id: str) -> None:
         ...
+
+    @abstractmethod
+    async def is_read_only(self) -> bool:
+        ...
```

### Comparing `sneakpeek_py-0.1.2/sneakpeek/lib/storage/in_memory_storage.py` & `sneakpeek_py-0.1.3/sneakpeek/lib/storage/in_memory_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,24 +8,29 @@
 from sneakpeek.lib.models import Lease, Scraper, ScraperRun, ScraperRunPriority
 from sneakpeek.metrics import count_invocations, measure_latency
 
 from .base import Storage
 
 
 class InMemoryStorage(Storage):
-    def __init__(self, scrapers: list[Scraper] | None = None) -> None:
+    def __init__(
+        self,
+        scrapers: list[Scraper] | None = None,
+        is_read_only: bool = False,
+    ) -> None:
         self._logger = logging.getLogger(__name__)
         self._scrapers: dict[int, Scraper] = {
             scraper.id: scraper for scraper in scrapers or []
         }
         self._scraper_runs: dict[int, dict[int, ScraperRun]] = {}
         self._queues: dict[ScraperRunPriority, list[ScraperRun]] = {}
         self._id_generator: Iterator[int] = count(1)
         self._lock = Lock()
         self._leases: dict[str, Lease] = {}
+        self._is_read_only = is_read_only
 
     def _generate_id(self) -> int:
         for id in self._id_generator:
             if id not in self._scrapers and id not in self._scraper_runs:
                 return id
 
     @count_invocations(subsystem="storage")
@@ -101,15 +106,21 @@
 
     @count_invocations(subsystem="storage")
     @measure_latency(subsystem="storage")
     async def get_scraper_runs(self, id: int) -> list[ScraperRun]:
         async with self._lock:
             if id not in self._scrapers:
                 raise ScraperNotFoundError(id)
-            return list(self._scraper_runs.get(id, {}).values())
+            return list(
+                sorted(
+                    self._scraper_runs.get(id, {}).values(),
+                    key=lambda x: x.id,
+                    reverse=True,
+                )
+            )
 
     @count_invocations(subsystem="storage")
     @measure_latency(subsystem="storage")
     async def add_scraper_run(self, scraper_run: ScraperRun) -> ScraperRun:
         async with self._lock:
             scraper_run.id = (
                 scraper_run.id
@@ -224,7 +235,12 @@
     @measure_latency(subsystem="storage")
     async def release_lease(self, lease_name: str, owner_id: str) -> None:
         async with self._lock:
             if lease_name not in self._leases:
                 return
             if self._can_acquire_lease(lease_name, owner_id):
                 del self._leases[lease_name]
+
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
+    async def is_read_only(self) -> bool:
+        return self._is_read_only
```

### Comparing `sneakpeek_py-0.1.2/sneakpeek/lib/storage/redis_storage.py` & `sneakpeek_py-0.1.3/sneakpeek/lib/storage/redis_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,21 @@
 from sneakpeek.lib.models import Lease, Scraper, ScraperRun, ScraperRunPriority
 from sneakpeek.metrics import count_invocations, measure_latency
 
 from .base import Storage
 
 
 class RedisStorage(Storage):
-    def __init__(self, redis: Redis) -> None:
+    def __init__(
+        self,
+        redis: Redis,
+        is_read_only: bool = False,
+    ) -> None:
         self._redis = redis
+        self._is_read_only = is_read_only
 
     async def _generate_id(self) -> int:
         return int(await self._redis.incr("internal:id_counter"))
 
     async def _generate_queue_id(self, priority: ScraperRunPriority) -> int:
         return int(await self._redis.incr(f"internal:queue:{priority}:last_id"))
 
@@ -225,7 +230,12 @@
 
     @count_invocations(subsystem="storage")
     @measure_latency(subsystem="storage")
     async def release_lease(self, lease_name: str, owner_id: str) -> None:
         lease_owner = await self._redis.get(f"lease:{lease_name}")
         if lease_owner == owner_id:
             await self._redis.delete(f"lease:{lease_name}")
+
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
+    async def is_read_only(self) -> bool:
+        return self._is_read_only
```

### Comparing `sneakpeek_py-0.1.2/sneakpeek/logging.py` & `sneakpeek_py-0.1.3/sneakpeek/logging.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.2/sneakpeek/metrics.py` & `sneakpeek_py-0.1.3/sneakpeek/metrics.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.2/sneakpeek/plugins/proxy_plugin.py` & `sneakpeek_py-0.1.3/sneakpeek/plugins/proxy_plugin.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.2/sneakpeek/plugins/rate_limiter_plugin.py` & `sneakpeek_py-0.1.3/sneakpeek/plugins/rate_limiter_plugin.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.2/sneakpeek/plugins/requests_logging_plugin.py` & `sneakpeek_py-0.1.3/sneakpeek/plugins/requests_logging_plugin.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.2/sneakpeek/plugins/robots_txt_plugin.py` & `sneakpeek_py-0.1.3/sneakpeek/plugins/robots_txt_plugin.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.2/sneakpeek/plugins/user_agent_injecter_plugin.py` & `sneakpeek_py-0.1.3/sneakpeek/plugins/user_agent_injecter_plugin.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.2/sneakpeek/plugins/utils.py` & `sneakpeek_py-0.1.3/sneakpeek/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.2/sneakpeek/runner.py` & `sneakpeek_py-0.1.3/sneakpeek/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from abc import ABC, abstractmethod
 from datetime import datetime
 from traceback import format_exc
 from typing import List
 
 from prometheus_client import Counter
 
-from sneakpeek.lib.errors import UnknownScraperHandlerError
+from sneakpeek.lib.errors import ScraperRunPingFinishedError, UnknownScraperHandlerError
 from sneakpeek.lib.models import Scraper, ScraperRun, ScraperRunStatus
 from sneakpeek.lib.queue import QueueABC
 from sneakpeek.lib.storage.base import Storage
 from sneakpeek.logging import scraper_run_context
 from sneakpeek.metrics import count_invocations, delay_histogram
 from sneakpeek.scraper_context import Plugin, ScraperContext
 from sneakpeek.scraper_handler import ScraperHandler
@@ -53,22 +53,32 @@
     @count_invocations(subsystem="scraper_runner")
     async def run(self, run: ScraperRun) -> None:
         delay_histogram.labels(type="time_spent_in_queue").observe(
             (datetime.utcnow() - run.created_at).total_seconds()
         )
         with scraper_run_context(run):
             self._logger.info("Starting scraper")
-            context = ScraperContext(run.scraper.config, self._plugins)
+
+            async def ping_session():
+                await self._queue.ping_scraper_run(run.scraper.id, run.id)
+
+            context = ScraperContext(run.scraper.config, self._plugins, ping_session)
             try:
                 await context.start_session()
                 await self._queue.ping_scraper_run(run.scraper.id, run.id)
                 handler = self._get_handler(run)
                 run.result = await handler.run(context)
                 run.status = ScraperRunStatus.SUCCEEDED
                 scraper_runs.labels(type="success").inc()
+            except ScraperRunPingFinishedError as e:
+                self._logger.error(
+                    "Scraper run seems to be killed. Not overriding status"
+                )
+                run.result = str(e)
+                scraper_runs.labels(type="killed").inc()
             except Exception as e:
                 self._logger.error(f"Failed to execute scraper with error: {e}")
                 self._logger.debug(f"Traceback: {format_exc()}")
                 run.status = ScraperRunStatus.FAILED
                 run.result = str(e)
                 scraper_runs.labels(type="failed").inc()
             finally:
```

### Comparing `sneakpeek_py-0.1.2/sneakpeek/scheduler.py` & `sneakpeek_py-0.1.3/sneakpeek/scheduler.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from sneakpeek.lib.models import Lease, Scraper, ScraperRunPriority, ScraperSchedule
 from sneakpeek.lib.queue import QueueABC
 from sneakpeek.lib.storage.base import Storage
 from sneakpeek.metrics import count_invocations, measure_latency, replicas_gauge
 
 DEFAULT_LEASE_DURATION = timedelta(minutes=1)
 DEFAULT_STORAGE_POLL_DELAY = timedelta(seconds=5)
+DEFAULT_RUNS_TO_KEEP = 100
 
 
 queue_length_gauge = Gauge(
     name="queue_length",
     documentation="Number of pending scraper runs",
     namespace="sneakpeek",
     labelnames=["priority"],
@@ -44,14 +45,15 @@
 class Scheduler(SchedulerABC):
     def __init__(
         self,
         storage: Storage,
         queue: QueueABC,
         storage_poll_frequency: timedelta = DEFAULT_STORAGE_POLL_DELAY,
         lease_duration: timedelta = DEFAULT_LEASE_DURATION,
+        runs_to_keep: int = 3,
     ) -> None:
         self._lease_name = "sneakpeek:scheduler"
         self._owner_id = str(uuid4())
         self._lease_duration = lease_duration
         self._storage = storage
         self._queue = queue
         self._scheduler = AsyncIOScheduler()
@@ -77,14 +79,22 @@
         self._scheduler.add_job(
             self._export_queue_len,
             trigger="interval",
             seconds=int(timedelta(seconds=5).total_seconds()),
             id="scheduler:internal:export_queue_len",
             max_instances=1,
         )
+        self._runs_to_keep = runs_to_keep
+        self._scheduler.add_job(
+            self._delete_old_scraper_runs,
+            trigger="interval",
+            seconds=int(timedelta(minutes=10).total_seconds()),
+            id="scheduler:internal:delete_old_runs",
+            max_instances=1,
+        )
 
     @measure_latency(subsystem="scheduler")
     @count_invocations(subsystem="scheduler")
     async def _enqueue_scraper(self, scraper_id: int) -> None:
         scraper = self._scrapers.get(scraper_id)
         if not scraper:
             self._logger.warning(f"Tried to enqueue unknown scraper: {scraper_id}")
@@ -231,14 +241,29 @@
             self._logger.error(f"Scheduler kill dead runs failed: {e}")
             self._logger.debug(
                 f"Scheduler kill dead runs failed. Traceback: {format_exc()}"
             )
 
     @measure_latency(subsystem="scheduler")
     @count_invocations(subsystem="scheduler")
+    async def _delete_old_scraper_runs(self):
+        if not self._lease:
+            return
+        try:
+            self._logger.info("Removing old scraper runs")
+            await self._storage.delete_old_scraper_runs(self._runs_to_keep)
+            self._logger.info("Successfully removed old scraper runs")
+        except Exception as e:
+            self._logger.error(f"Removing old scraper runs failed: {e}")
+            self._logger.debug(
+                f"Removing old scraper runs failed. Traceback: {format_exc()}"
+            )
+
+    @measure_latency(subsystem="scheduler")
+    @count_invocations(subsystem="scheduler")
     async def _export_queue_len(self):
         if not self._lease:
             return
         try:
             for priority in ScraperRunPriority:
                 pending_runs = await self._queue.get_queue_len(priority)
                 queue_length_gauge.labels(priority=priority.name).set(pending_runs)
```

### Comparing `sneakpeek_py-0.1.2/sneakpeek/scraper_context.py` & `sneakpeek_py-0.1.3/sneakpeek/scraper_context.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,19 @@
+import logging
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from enum import Enum
-from typing import Any
+from typing import Any, Callable
 
 import aiohttp
 
+from sneakpeek.lib.errors import (
+    ScraperRunPingFinishedError,
+    ScraperRunPingNotStartedError,
+)
 from sneakpeek.scraper_config import ScraperConfig
 
 HttpHeaders = dict[str, str]
 PluginConfig = Any
 
 
 class HttpMethod(str, Enum):
@@ -63,16 +68,19 @@
 
 
 class ScraperContext:
     def __init__(
         self,
         config: ScraperConfig,
         plugins: list[Plugin] | None = None,
+        ping_session_func: Callable | None = None,
     ) -> None:
         self.params = config.params
+        self.ping_session_func = ping_session_func
+        self._logger = logging.getLogger(__name__)
         self._plugins_configs = config.plugins or {}
         self._session: aiohttp.ClientSession | None = None
         self._before_request_plugins = []
         self._after_response_plugins = []
         self._init_plugins(plugins)
 
     def _init_plugins(self, plugins: list[Plugin] | None = None) -> None:
@@ -117,23 +125,46 @@
                 request,
                 response,
                 self._plugins_configs.get(plugin.name),
             )
         return response
 
     async def _request(self, request: Request) -> aiohttp.ClientResponse:
+        await self.ping_session()
         request = await self._before_request(request)
         response = await getattr(self._session, request.method)(
             request.url,
             headers=request.headers,
             **(request.kwargs or {}),
         )
         response = await self._after_response(request, response)
+        await self.ping_session()
         return response
 
+    async def ping_session(self) -> None:
+        if not self.ping_session_func:
+            self._logger.warning(
+                "Tried to ping scraper run, but the function to ping session is None"
+            )
+            return
+        try:
+            await self.ping_session_func()
+        except ScraperRunPingNotStartedError as e:
+            self._logger.error(
+                f"Failed to ping PENDING scraper run because due to some infra error: {e}"
+            )
+            raise
+        except ScraperRunPingFinishedError as e:
+            self._logger.error(
+                f"Failed to ping scraper run because seems like it's been killed: {e}"
+            )
+            raise
+        except Exception as e:
+            self._logger.error(f"Failed to ping scraper run: {e}")
+
     async def get(
         self,
         url: str,
         *,
         headers: HttpHeaders | None = None,
         **kwargs,
     ) -> aiohttp.ClientResponse:
```

### Comparing `sneakpeek_py-0.1.2/sneakpeek/server.py` & `sneakpeek_py-0.1.3/sneakpeek/server.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.2/sneakpeek/worker.py` & `sneakpeek_py-0.1.3/sneakpeek/worker.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,45 +46,47 @@
         except Exception as e:
             self._logger.error(f"Failed to execute {scraper_run.id}: {e}")
             self._logger.debug(f"Failed to execute {scraper_run.id}: {format_exc()}")
         del self._active[scraper_run.id]
 
     @measure_latency(subsystem="worker")
     @count_invocations(subsystem="worker")
-    async def _on_tick(self) -> None:
+    async def _on_tick(self) -> bool:
         async with self._lock:
             replicas_gauge.labels(type="active_scrapers").set(len(self._active))
             if len(self._active) >= self._max_concurrency:
                 self._logger.debug(
                     f"Not dequeuing any tasks because worker has reached max concurrency,"
                     f" there are {len(self._active)} of active tasks"
                 )
-                return
+                return False
 
             dequeued = await self._queue.dequeue()
             if not dequeued:
                 self._logger.debug("No pending tasks in the queue")
-                return
+                return False
 
             self._logger.info(f"Dequeued a job with id={dequeued.id}")
             self._active[dequeued.id] = dequeued
             self._loop.create_task(self._execute_scraper(dequeued))
+            return True
 
     async def _worker_loop(self) -> None:
         while self._running:
             replicas_gauge.labels(type="worker").set(1)
+            dequeued_anything = False
             try:
-                await self._on_tick()
+                dequeued_anything = await self._on_tick()
             except Exception as e:
                 self._logger.error(f"Worker on tick function failed: {e}")
                 self._logger.debug(
                     f"Worker on tick function failed. Traceback: {format_exc()}"
                 )
-
-            await sleep(timedelta(seconds=1).total_seconds())
+            if not dequeued_anything:
+                await sleep(timedelta(seconds=1).total_seconds())
 
     async def start(self) -> None:
         self._logger.info("Starting worker")
         self._running = True
         if not self._loop:
             self._loop = get_running_loop()
         self._loop.create_task(self._worker_loop())
```

### Comparing `sneakpeek_py-0.1.2/PKG-INFO` & `sneakpeek_py-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sneakpeek-py
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tool box for creating scrapers, so that you only focus on scraping logic
 Home-page: https://github.com/flulemon/sneakpeek
 License: BSD-3-Clause
 Author: Dan Yazovsky
 Author-email: daniil.yazovsky@gmail.com
 Maintainer: Dan Yazovsky
 Maintainer-email: daniil.yazovsky@gmail.com
```

