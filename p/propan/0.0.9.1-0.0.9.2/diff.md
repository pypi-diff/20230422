# Comparing `tmp/propan-0.0.9.1.tar.gz` & `tmp/propan-0.0.9.2.tar.gz`

## Comparing `propan-0.0.9.1.tar` & `propan-0.0.9.2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 propan-0.0.9.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.0.9.1/SECURITY.md
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.0.9.1/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 propan-0.0.9.1/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.0.9.1/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 propan-0.0.9.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/1_basic_usage.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/5_publishing.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/__about__.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/__main__.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/annotations.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/brokers/__init__.py
--rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/brokers/model/__init__.py
--rw-r--r--   0        0        0     5915 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/brokers/model/broker_usecase.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/brokers/model/schemas.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0     8829 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0     5824 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/cli/__init__.py
--rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/cli/app.py
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/cli/main.py
--rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/cli/startproject.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/cli/utils/imports.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/cli/utils/parser.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/log/__init__.py
--rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/log/formatter.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/log/logging.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/utils/__init__.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/utils/classes.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/utils/functions.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/utils/context/__init__.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/utils/context/main.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/utils/context/types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.0.9.1/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.0.9.1/scripts/publish.sh
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.0.9.1/scripts/test-cov.sh
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.0.9.1/scripts/test.sh
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 propan-0.0.9.1/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.0.9.1/LICENSE
--rw-r--r--   0        0        0     9956 2020-02-02 00:00:00.000000 propan-0.0.9.1/README.md
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 propan-0.0.9.1/pyproject.toml
--rw-r--r--   0        0        0    13174 2020-02-02 00:00:00.000000 propan-0.0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 propan-0.0.9.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.0.9.2/SECURITY.md
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.0.9.2/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 propan-0.0.9.2/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.0.9.2/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 propan-0.0.9.2/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/5_publishing.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/__about__.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/__main__.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/annotations.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/brokers/__init__.py
+-rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/brokers/model/__init__.py
+-rw-r--r--   0        0        0     5915 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/brokers/model/broker_usecase.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/brokers/model/schemas.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     5155 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0     8922 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0     5835 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/cli/__init__.py
+-rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/cli/app.py
+-rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/cli/main.py
+-rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/cli/startproject.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/log/__init__.py
+-rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/log/formatter.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/log/logging.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/utils/__init__.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/utils/classes.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/utils/functions.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/utils/context/main.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.0.9.2/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.0.9.2/scripts/publish.sh
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.0.9.2/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.0.9.2/scripts/test.sh
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 propan-0.0.9.2/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.0.9.2/LICENSE
+-rw-r--r--   0        0        0    10123 2020-02-02 00:00:00.000000 propan-0.0.9.2/README.md
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 propan-0.0.9.2/pyproject.toml
+-rw-r--r--   0        0        0    13341 2020-02-02 00:00:00.000000 propan-0.0.9.2/PKG-INFO
```

### Comparing `propan-0.0.9.1/CONTRIBUTING.md` & `propan-0.0.9.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.1/SECURITY.md` & `propan-0.0.9.2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.1/.github/workflows/documentation.yml` & `propan-0.0.9.2/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.1/.github/workflows/publish_coverage.yml` & `propan-0.0.9.2/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.1/.github/workflows/publish_pypi.yml` & `propan-0.0.9.2/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.1/.github/workflows/tests.yml` & `propan-0.0.9.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.1/examples/3_lifespan_events.py` & `propan-0.0.9.2/examples/3_lifespan_events.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """
 Also you can use sync/async functions as
 application lifecycle hooks
 
 All `on_startup` hooks runs before broker has been started
 All `on_shutdown` hooks runs after broker has been stopped
 """
-
-from propan import PropanApp
-from propan.brokers.rabbit import RabbitBroker
+from propan import PropanApp, RabbitBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = PropanApp(broker)
 
 
 @app.on_startup
```

### Comparing `propan-0.0.9.1/examples/4_cli_attributes_promotion.py` & `propan-0.0.9.2/examples/4_cli_attributes_promotion.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 ... env=.env
 "=" is required
 
 Or you can pass a boolean flags
 ... --use-smth  # passes as use_smth=True
 ... --no-use-smth  # passes as use_smth=False
 """
-from propan import Context, PropanApp
-from propan.brokers.rabbit import RabbitBroker
+from propan import Context, PropanApp, RabbitBroker
 from pydantic import BaseSettings
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = PropanApp(broker)
```

### Comparing `propan-0.0.9.1/examples/5_publishing.py` & `propan-0.0.9.2/examples/5_publishing.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Propan provides the easiest way to publish messages:
 just use Broker as context manager and publish whatever you want!
 """
 import asyncio
 
 from aio_pika import Message
-from propan.brokers.rabbit import RabbitBroker
+from propan import RabbitBroker
 
 
 async def main():
     async with RabbitBroker("amqp://guest:guest@localhost:5672/") as broker:
         await broker.publish_message("Hello, Propan!", queue="test")
 
         await broker.publish_message(
```

### Comparing `propan-0.0.9.1/examples/6_arguments_casting.py` & `propan-0.0.9.2/examples/6_arguments_casting.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """
 Propan has @apply_types decorator to cast incoming function
 arguments to type according their type annotation.
 
 If you doesn't create broker as `RabbitBroker(apply_types=False)`,
 all broker handlers are wrapped by @apply_types by default.
 """
-from propan import PropanApp
-from propan.brokers.rabbit import RabbitBroker
-from propan.utils import apply_types
+from propan import PropanApp, RabbitBroker, apply_types
 from pydantic import BaseModel
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = PropanApp(broker)
```

### Comparing `propan-0.0.9.1/examples/7_handler_errors_processing.py` & `propan-0.0.9.2/examples/7_handler_errors_processing.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 process exceptions.
 
 If you want to redelivere messages just use
 @handler(retry=...) parameter.
 
 For more complex usecases just use the `tenacity` library.
 """
-
-from propan import PropanApp
-from propan.brokers.rabbit import RabbitBroker
+from propan import PropanApp, RabbitBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = PropanApp(broker)
 
 
 @broker.handle("test", retry=True)
```

### Comparing `propan-0.0.9.1/examples/dependencies/1_dependency_injection.py` & `propan-0.0.9.2/examples/dependencies/1_dependency_injection.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 Propan use dependencies management policy close to `pytest fixtures`.
 You can specify in functions argument parameters which dependencies
 you would to use. And framework passes them from the global Context object.
 
 Default context fields are: app, broker, context (itself), logger and message.
 If you call not existed field, raises "pydantic.error_wrappers.ValidationError" value.
 """
-from propan import Context, PropanApp
+from propan import Context, PropanApp, RabbitBroker
 from propan.annotations import App, ContextRepo, Logger
 from propan.annotations import RabbitBroker as Rabbit
 from propan.annotations import RabbitMessage
-from propan.brokers.rabbit import RabbitBroker
 
 rabbit_broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = PropanApp(rabbit_broker)
 
 
 @rabbit_broker.handle("test")
```

### Comparing `propan-0.0.9.1/examples/dependencies/2_dependency_declaration.py` & `propan-0.0.9.2/examples/dependencies/2_dependency_declaration.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """
 All Context dependencies also available from on_startup hook
 (Some of them are None at application starting).
 
 You can use it to setup your custom context fields.
 """
-from propan import Context, PropanApp
+from propan import Context, PropanApp, RabbitBroker
 from propan.annotations import ContextRepo
-from propan.brokers.rabbit import RabbitBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = PropanApp(broker)
 
 
 @app.on_startup
```

### Comparing `propan-0.0.9.1/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.0.9.2/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Alias is able to provide access to specific attributes of dependency
 """
-from propan import Context, PropanApp
+from propan import Context, PropanApp, RabbitBroker
 from propan.annotations import ContextRepo
-from propan.brokers.rabbit import RabbitBroker
 from pydantic import BaseSettings, Field
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = PropanApp(broker)
 
 KEY = "my-secret-key"
```

### Comparing `propan-0.0.9.1/examples/dependencies/5_dependency_nesting.py` & `propan-0.0.9.2/examples/dependencies/5_dependency_nesting.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 @apply_types decorator allows pass context dependencies
 to all functions with the same context through the functions
 calling stack.
 """
-from propan import PropanApp, apply_types
+from propan import PropanApp, RabbitBroker, apply_types
 from propan.annotations import Logger, RabbitMessage
-from propan.brokers.rabbit import RabbitBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = PropanApp(broker)
 
 
 @broker.handle("test")
```

### Comparing `propan-0.0.9.1/examples/dependencies/6_dependecy_calling.py` & `propan-0.0.9.2/examples/dependencies/6_dependecy_calling.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 Depends parameter allows to call function before
 natural handler with providing all arguments and context
 inside dependency function
 
 Dependecies argument names should be calling same as a handler arguments
 Dependency decorated by `apply_types` as a default if hanler was decorated
 """
-from propan import Depends, PropanApp
-from propan.brokers.rabbit import RabbitBroker
+from propan import Depends, PropanApp, RabbitBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = PropanApp(broker)
 
 
 async def async_dependency(body, logger):
```

### Comparing `propan-0.0.9.1/examples/dependencies/7_annotated.py` & `propan-0.0.9.2/examples/dependencies/7_annotated.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 With Python 3.10+ you can use
 typing.Annotated class as a shortcut to Depends and Alias
 """
 import logging
 
-from propan import Context, Depends, PropanApp, apply_types
-from propan.brokers.rabbit import RabbitBroker
+from propan import Context, Depends, PropanApp, RabbitBroker, apply_types
 from typing_extensions import Annotated
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = PropanApp(broker)
 
 Logger = Annotated[logging.Logger, Context("broker.logger")]
```

### Comparing `propan-0.0.9.1/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.0.9.2/examples/http_frameworks_integrations/aiohttp.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 You can use Propan MQBrokers without PropanApp
 Just start and stop them whenever you want
 """
 from aiohttp import web
-from propan.brokers.rabbit import RabbitBroker
+from propan import RabbitBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 
 @broker.handle("test")
 async def base_handler(body):
     print(body)
```

### Comparing `propan-0.0.9.1/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.0.9.2/examples/http_frameworks_integrations/blacksheep.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 You can use Propan MQBrokers without PropanApp
 Just start and stop them whenever you want
 """
 from blacksheep import Application
-from propan.brokers.rabbit import RabbitBroker
+from propan import RabbitBroker
 
 app = Application()
 
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
```

### Comparing `propan-0.0.9.1/examples/http_frameworks_integrations/falcon.py` & `propan-0.0.9.2/examples/http_frameworks_integrations/falcon.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 You can use Propan MQBrokers without PropanApp
 Just start and stop them whenever you want
 """
 import falcon
 import falcon.asgi
-from propan.brokers.rabbit import RabbitBroker
+from propan import RabbitBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 
 @broker.handle("test")
 async def base_handler(body):
     print(body)
```

### Comparing `propan-0.0.9.1/examples/http_frameworks_integrations/fastapi.py` & `propan-0.0.9.2/examples/http_frameworks_integrations/fastapi.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 You can use Propan MQBrokers without PropanApp
 Just start and stop them whenever you want
 """
 from contextlib import asynccontextmanager
 
 from fastapi import FastAPI
-from propan.brokers.rabbit import RabbitBroker
+from propan import RabbitBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = FastAPI()
 
 
 @asynccontextmanager
```

### Comparing `propan-0.0.9.1/examples/http_frameworks_integrations/quart.py` & `propan-0.0.9.2/examples/http_frameworks_integrations/tornado.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,43 @@
 """
 You can use Propan MQBrokers without PropanApp
 Just start and stop them whenever you want
 """
-from propan.brokers.rabbit import RabbitBroker
-from quart import Quart
+import asyncio
 
-broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
+import tornado.web
+from propan import RabbitBroker
 
-app = Quart(__name__)
+broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 
 @broker.handle("test")
 async def base_handler(body):
     print(body)
 
 
-@app.before_serving
-async def start_broker():
-    await broker.start()
+class MainHandler(tornado.web.RequestHandler):
+    def get(self):
+        self.write("Hello, world")
+
+
+def make_app():
+    return tornado.web.Application(
+        [
+            (r"/", MainHandler),
+        ]
+    )
+
+
+async def main():
+    app = make_app()
+    app.listen(8888)
 
-
-@app.after_serving
-async def stop_broker():
-    await broker.close()
+    await broker.start()
+    try:
+        await asyncio.Event().wait()
+    finally:
+        await broker.close()
 
 
-@app.route("/")
-async def json():
-    return {"hello": "world"}
+if __name__ == "__main__":
+    asyncio.run(main())
```

### Comparing `propan-0.0.9.1/examples/http_frameworks_integrations/sanic.py` & `propan-0.0.9.2/examples/http_frameworks_integrations/sanic.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 You can use Propan MQBrokers without PropanApp
 Just start and stop them whenever you want
 """
-from propan.brokers.rabbit import RabbitBroker
+from propan import RabbitBroker
 from sanic import Sanic
 from sanic.response import text
 
 app = Sanic("MyHelloWorldApp")
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
```

### Comparing `propan-0.0.9.1/propan/brokers/push_back_watcher.py` & `propan-0.0.9.2/propan/brokers/push_back_watcher.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.1/propan/brokers/model/broker_usecase.py` & `propan-0.0.9.2/propan/brokers/model/broker_usecase.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.1/propan/brokers/model/schemas.py` & `propan-0.0.9.2/propan/brokers/model/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.1/propan/brokers/nats/nats_broker.py` & `propan-0.0.9.2/propan/brokers/nats/nats_broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         self.__max_queue_len = 0
         self.__max_subject_len = 4
 
     async def _connect(self, *args: Any, **kwargs: Any) -> Client:
         return await nats.connect(*args, **kwargs)
 
     def handle(
-        self, subject: str, queue: str = "", retry: Union[bool, int] = False
+        self, subject: str, queue: str = "", *, retry: Union[bool, int] = False
     ) -> Callable[[DecoratedCallable], None]:
         i = len(subject)
         if i > self.__max_subject_len:
             self.__max_subject_len = i
 
         i = len(queue)
         if i > self.__max_queue_len:
```

### Comparing `propan-0.0.9.1/propan/brokers/nats/nats_broker.pyi` & `propan-0.0.9.2/propan/brokers/nats/nats_broker.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,14 @@
         pending_size: int = DEFAULT_PENDING_SIZE,
         flush_timeout: Optional[float] = None,
         *,
         logger: Optional[logging.Logger] = access_logger,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         apply_types: bool = True,
-        consumers: Optional[int] = None,
     ) -> None: ...
     async def connect(
         self,
         servers: Union[str, List[str]] = ["nats://localhost:4222"],  # noqa: B006
         error_cb: Optional[ErrorCallback] = None,
         disconnected_cb: Optional[Callback] = None,
         closed_cb: Optional[Callback] = None,
@@ -109,15 +108,15 @@
         self,
         message: Union[str, Dict[str, Any]],
         subject: str,
         reply: str = "",
         headers: Optional[Dict[str, str]] = None,
     ) -> None: ...
     def handle(
-        self, subject: str, queue: str = "", retry: Union[bool, int] = False
+        self, subject: str, queue: str = "", *, retry: Union[bool, int] = False
     ) -> Callable[[DecoratedCallable], None]: ...
     async def __aenter__(self) -> "NatsBroker": ...
     async def _connect(self, *args: Any, **kwargs: Any) -> Client: ...
     async def close(self) -> None: ...
     def _get_log_context(
         self, message: Optional[Msg], subject: str, queue: str = "", **kwargs
     ) -> Dict[str, Any]: ...
```

### Comparing `propan-0.0.9.1/propan/brokers/nats/nats_js_broker.py` & `propan-0.0.9.2/propan/brokers/nats/nats_js_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.1/propan/brokers/nats/schemas.py` & `propan-0.0.9.2/propan/brokers/nats/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.1/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.0.9.2/propan/brokers/rabbit/rabbit_broker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import json
 import logging
 from functools import partial, wraps
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Union
 
 import aio_pika
 import aiormq
 from propan.brokers.model import BrokerUsecase, ContentTypes
 from propan.brokers.push_back_watcher import BaseWatcher, WatcherContext
 from propan.brokers.rabbit.schemas import Handler, RabbitExchange, RabbitQueue
 from propan.types import DecodedMessage, DecoratedCallable, Wrapper
@@ -59,17 +59,18 @@
                 self._log(f"Set max consumers to {max_consumers}", logging.INFO)
                 await self._channel.set_qos(prefetch_count=int(max_consumers))
 
     def handle(
         self,
         queue: Union[str, RabbitQueue],
         exchange: Union[str, RabbitExchange, None] = None,
+        *,
         retry: Union[bool, int] = False,
     ) -> Wrapper:
-        queue, exchange = _validate_exchange_and_queue(queue, exchange)
+        queue, exchange = _validate_queue(queue), _validate_exchange(exchange)
 
         if exchange:
             i = len(exchange.name)
             if i > self.__max_exchange_len:  # pragma: no branch
                 self.__max_exchange_len = i
 
         i = len(queue.name)
@@ -116,15 +117,15 @@
         *,
         routing_key: str = "",
         **publish_args,
     ) -> Optional[aiormq.abc.ConfirmationFrameType]:
         if self._channel is None:
             raise ValueError("RabbitBroker channel not started yet")
 
-        queue, exchange = _validate_exchange_and_queue(queue, exchange)
+        queue, exchange = _validate_queue(queue), _validate_exchange(exchange)
 
         if not isinstance(message, aio_pika.message.Message):
             if isinstance(message, dict):
                 message = aio_pika.Message(
                     json.dumps(message).encode(), content_type=ContentTypes.json.value
                 )
             else:
@@ -145,15 +146,15 @@
 
     async def close(self) -> None:
         if self._connection is not None:
             await self._connection.close()
 
     async def _init_handler(self, handler: Handler) -> aio_pika.abc.AbstractRobustQueue:
         queue = await self._init_queue(handler.queue)
-        if handler.exchange is not None:
+        if handler.exchange is not None and handler.exchange.name != "default":
             exchange = await self._init_exchange(handler.exchange)
             await queue.bind(exchange, handler.queue.routing_key or handler.queue.name)
         return queue
 
     async def _init_queue(self, queue: RabbitQueue) -> aio_pika.abc.AbstractRobustQueue:
         if queue.declare is True:
             return await self._channel.declare_queue(**queue.dict())
@@ -226,28 +227,32 @@
             async with context:
                 r = await func(message)
                 return r
 
         return wrapper
 
 
-def _validate_exchange_and_queue(
-    queue: Union[str, RabbitQueue, None],
+def _validate_exchange(
     exchange: Union[str, RabbitExchange, None] = None,
-) -> Tuple[RabbitQueue, Optional[RabbitExchange]]:
-    if queue is not None:  # pragma: no branch
-        if isinstance(queue, str):
-            queue = RabbitQueue(name=queue)
-        elif not isinstance(queue, RabbitQueue):
-            raise ValueError(
-                f"Queue '{queue}' should be 'str' | 'RabbitQueue' instance"
-            )
-
+) -> Optional[RabbitExchange]:
     if exchange is not None:  # pragma: no branch
         if isinstance(exchange, str):
             exchange = RabbitExchange(name=exchange)
         elif not isinstance(exchange, RabbitExchange):
             raise ValueError(
                 f"Exchange '{exchange}' should be 'str' | 'RabbitExchange' instance"
             )
 
-    return queue, exchange
+    return exchange
+
+
+def _validate_queue(
+    queue: Union[str, RabbitQueue, None] = None
+) -> Optional[RabbitQueue]:
+    if queue is not None:  # pragma: no branch
+        if isinstance(queue, str):
+            queue = RabbitQueue(name=queue)
+        elif not isinstance(queue, RabbitQueue):
+            raise ValueError(
+                f"Queue '{queue}' should be 'str' | 'RabbitQueue' instance"
+            )
+    return queue
```

### Comparing `propan-0.0.9.1/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.0.9.2/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -109,14 +109,15 @@
         immediate: bool = False,
         timeout: aio_pika.abc.TimeoutType = None,
     ) -> Optional[aiormq.abc.ConfirmationFrameType]: ...
     def handle(
         self,
         queue: Union[str, RabbitQueue],
         exchange: Union[str, RabbitExchange, None] = None,
+        *,
         retry: Union[bool, int] = False,
     ) -> Wrapper:
         """
         retry: Union[bool, int] - at exeption message will returns to queue `int` times or endless if `True`
         """
         ...
     async def __aenter__(self) -> "RabbitBroker": ...
```

### Comparing `propan-0.0.9.1/propan/brokers/rabbit/schemas.py` & `propan-0.0.9.2/propan/brokers/rabbit/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.1/propan/cli/app.py` & `propan-0.0.9.2/propan/cli/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.1/propan/cli/main.py` & `propan-0.0.9.2/propan/cli/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.1/propan/cli/startproject.py` & `propan-0.0.9.2/propan/cli/startproject.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.1/propan/cli/supervisors/basereload.py` & `propan-0.0.9.2/propan/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.1/propan/cli/supervisors/multiprocess.py` & `propan-0.0.9.2/propan/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.1/propan/cli/supervisors/utils.py` & `propan-0.0.9.2/propan/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.1/propan/cli/supervisors/watchfiles.py` & `propan-0.0.9.2/propan/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.1/propan/cli/utils/imports.py` & `propan-0.0.9.2/propan/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.1/propan/cli/utils/logs.py` & `propan-0.0.9.2/propan/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.1/propan/cli/utils/parser.py` & `propan-0.0.9.2/propan/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.1/propan/log/formatter.py` & `propan-0.0.9.2/propan/log/formatter.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.1/propan/log/logging.py` & `propan-0.0.9.2/propan/log/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.1/propan/utils/context/main.py` & `propan-0.0.9.2/propan/utils/context/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.1/propan/utils/context/types.py` & `propan-0.0.9.2/propan/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.1/LICENSE` & `propan-0.0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.1/README.md` & `propan-0.0.9.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,38 +25,38 @@
         <img alt="GitHub" src="https://img.shields.io/github/license/Lancetnik/Propan?color=%23007ec6">
     </a>
 </p>
 
 # Propan
 
 **Propan** - just *<s>an another one HTTP</s>* a **declarative Python MQ framework**. It's following by [*fastapi*](https://fastapi.tiangolo.com/ru/),
-simplify Message Brokers around code writing and provides helpful development toolkit, existed only at HTTP-frameworks world until now.
+simplify Message Brokers around code writing and provides a helpful development toolkit, which existed only in HTTP-frameworks world until now.
 
 It's designed to create reactive microservices around <a href="https://microservices.io/patterns/communication-style/messaging.html" target="_blank">Messaging Architecture</a>.
 
-It is a modern, highlevel framework on top of popular Python specific brokers libraries, based on [*pydantic*](https://docs.pydantic.dev/) and [*fastapi*](https://fastapi.tiangolo.com/ru/), [*pytest*](https://docs.pytest.org/en/7.3.x/) concepts.
+It is a modern, high-level framework on top of popular specific Python brokers libraries, based on [*pydantic*](https://docs.pydantic.dev/) and [*fastapi*](https://fastapi.tiangolo.com/ru/), [*pytest*](https://docs.pytest.org/en/7.3.x/) concepts.
 
 ---
 
 **Documentation**: <a href="https://lancetnik.github.io/Propan/" target="_blank">https://lancetnik.github.io/Propan/</a>
 
 **Sources**: <a href="https://github.com/Lancetnik/Propan/" target="_blank">https://github.com/Lancetnik/Propan/</a>
 
 ---
 
 ### The key features are
 
 * **Easy**: Designed to be easy to use and learn.
 * **Intuitive**: Great editor support. Autocompletion everywhere.
 * [**Dependencies management**](#dependencies): Minimize code duplication. Multiple features from each argument and parameter declaration.
-* [**Integrations**](#http-frameworks-integrations): Propan is ready to using in pair with [any http framework](https://github.com/Lancetnik/Propan/tree/main/examples/http_frameworks_integrations) you want
+* [**Integrations**](#http-frameworks-integrations): **Propan** is ready to use in pair with [any HTTP framework](https://lancetnik.github.io/Propan/5_integrations/1_integrations-index/) you want
 * **MQ independent**: Single interface to popular MQ:
     * **NATS** (based on [nats-py](https://github.com/nats-io/nats.py)) 
     * **RabbitMQ** (based on [aio-pika](https://aio-pika.readthedocs.io/en/latest/)) 
-* [**Greate to develop**](#cli-power): cli tool provides great development expireince:
+* [**Greate to develop**](#cli-power): CLI tool provides great development experience:
     * framework-independent way to rule application environment
     * application code hot reloading
 
 ### Supported MQ brokers
 |              | async                                                   | sync                 |
 |--------------|:-------------------------------------------------------:|:--------------------:|
 | **RabbitMQ** | :heavy_check_mark: **stable** :heavy_check_mark:        | :mag: planning :mag: |
@@ -66,25 +66,25 @@
 | **REDIS**    | :mag: planning :mag:                                    | :mag: planning :mag: |
 | **Kafka**    | :mag: planning :mag:                                    | :mag: planning :mag: |
 | **SQS**      | :mag: planning :mag:                                    | :mag: planning :mag: |
 
 
 ### Community
 
-If you are interested at this project, please give me feedback by star or/and watch repository.
+If you are interested in this project, please give me feedback by star or/and watch repository.
 
-If you have any questions or ideas about features to implement, welcome to [discussions](https://github.com/Lancetnik/Propan/discussions) or publick [telegram group](https://t.me/propan_python).
+If you have any questions or ideas about features to implement, welcome to [discussions](https://github.com/Lancetnik/Propan/discussions) or public [telegram group](https://t.me/propan_python).
 
 ---
 
 ## Declarative?
 
-At declarative tools you should define **what you need to get**. At traditional imperative tools you should write **what you need to do**.
+With declarative tools you should define **what you need to get**. With traditional imperative tools you should write **what you need to do**.
 
-Take a look at classic imperative tools, such as [aio-pika](), [pika](), [nats-py](), etc are. 
+Take a look at classic imperative tools, such as [aio-pika](https://aio-pika.readthedocs.io/en/latest/), [pika](https://pika.readthedocs.io/en/stable/), [nats-py](https://github.com/nats-io/nats.py), etc. 
 
 This is the **Quickstart** with the *aio-pika*:
 
 ```python
 import asyncio
 import aio_pika
 
@@ -104,15 +104,15 @@
             async for message in queue_iter:
                 async with message.process():
                     print(message.body)
 
 asyncio.run(main())
 ```
 
-**aio-pika** is a really great tool with a really easy learning curve. But it's still imperative. You need to connect, declare channel, queues, exchanges by yourself. Also, you need to manage connection, message, queue context to avoid any troubles.
+**aio-pika** is a really great tool with a really easy learning curve. But it's still imperative. You need to *connect*, declare *channel*, *queues*, *exchanges* by yourself. Also, you need to manage *connection*, *message*, *queue* context to avoid any troubles.
 
 It is not a bad way, but it can be easy.
 
 ```python
 from propan import PropanApp, RabbitBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
@@ -164,15 +164,15 @@
 $ propan run serve:app
 ```
 
 ---
 
 ## Type casting
 
-Propan uses `pydantic` to cast incoming function arguments to types according their annotation.
+Propan uses `pydantic` to cast incoming function arguments to types according to their annotation.
 
 ```python
 from pydantic import BaseModel
 from propan import PropanApp, Context, RabbitBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 app = PropanApp(broker)
@@ -186,20 +186,20 @@
 
 ```
 
 ---
 
 ## Dependencies
 
-Propan has dependencies management policy close to `pytest fixtures`.
+**Propan** a has dependencies management policy close to `pytest fixtures`.
 You can specify in functions arguments which dependencies
 you would to use. Framework passes them from the global Context object.
 
 Already existed context fields are: *app*, *broker*, *context* (itself), *logger* and *message*.
-If you call not existed field, raises *pydantic.error_wrappers.ValidationError* value.
+If you call not existing field, raises *pydantic.error_wrappers.ValidationError* value.
 
 But you can specify your own dependencies, call dependencies functions (like `Fastapi Depends`)
 and [more](https://github.com/Lancetnik/Propan/tree/main/examples/dependencies).
 
 ```python
 from logging import Logger
 
@@ -216,15 +216,15 @@
     assert broker is rabbit_broker
 ```
 
 ---
 
 ## CLI power
 
-Propan has own cli tool provided the following features:
+**Propan** has its own CLI tool that provided the following features:
 * project generation
 * multiprocessing workers
 * project hot reloading
 * custom command line arguments passing
 
 ### Context passing
 
@@ -249,23 +249,23 @@
 async def setup(env: str, context: ContextRepo):
     settings = Settings(_env_file=env)
     context.set_context("settings", settings)
 ```
 
 ### Project template
 
-Also **propan cli** is able to generate production-ready application template:
+Also, **Propan CLI** is able to generate a production-ready application template:
 
 ```shell
 $ propan create [projectname]
 ```
 
 *Notice: project template require* `pydantic[dotenv]` *installation.*
 
-Run created project:
+Run the created project:
 
 ```shell
 # Run rabbimq first
 $ docker compose --file [projectname]/docker-compose.yaml up -d
 
 # Run project
 $ propan run [projectname].app.serve:app --env=.env --reload
@@ -273,16 +273,16 @@
 
 Now you can enjoy a new development experience!
 
 ---
 
 ## HTTP Frameworks integrations
 
-You can use Propan MQBrokers without PropanApp.
-Just *start* and *stop* them according your application lifespan.
+You can use **Propan** `MQBrokers` without `PropanApp`.
+Just *start* and *stop* them according to your application lifespan.
 
 ```python
 from contextlib import asynccontextmanager
 
 from fastapi import FastAPI
 from propan import RabbitBroker
```

### Comparing `propan-0.0.9.1/pyproject.toml` & `propan-0.0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.1/PKG-INFO` & `propan-0.0.9.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propan
-Version: 0.0.9.1
+Version: 0.0.9.2
 Summary: Propan framework: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://lancetnik.github.io/Propan/
 Project-URL: Documentation, https://lancetnik.github.io/Propan/
 Project-URL: Tracker, https://github.com/Lancetnik/Propan/issues
 Project-URL: Source, https://github.com/Lancetnik/Propan
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-Expression: MIT
@@ -95,38 +95,38 @@
         <img alt="GitHub" src="https://img.shields.io/github/license/Lancetnik/Propan?color=%23007ec6">
     </a>
 </p>
 
 # Propan
 
 **Propan** - just *<s>an another one HTTP</s>* a **declarative Python MQ framework**. It's following by [*fastapi*](https://fastapi.tiangolo.com/ru/),
-simplify Message Brokers around code writing and provides helpful development toolkit, existed only at HTTP-frameworks world until now.
+simplify Message Brokers around code writing and provides a helpful development toolkit, which existed only in HTTP-frameworks world until now.
 
 It's designed to create reactive microservices around <a href="https://microservices.io/patterns/communication-style/messaging.html" target="_blank">Messaging Architecture</a>.
 
-It is a modern, highlevel framework on top of popular Python specific brokers libraries, based on [*pydantic*](https://docs.pydantic.dev/) and [*fastapi*](https://fastapi.tiangolo.com/ru/), [*pytest*](https://docs.pytest.org/en/7.3.x/) concepts.
+It is a modern, high-level framework on top of popular specific Python brokers libraries, based on [*pydantic*](https://docs.pydantic.dev/) and [*fastapi*](https://fastapi.tiangolo.com/ru/), [*pytest*](https://docs.pytest.org/en/7.3.x/) concepts.
 
 ---
 
 **Documentation**: <a href="https://lancetnik.github.io/Propan/" target="_blank">https://lancetnik.github.io/Propan/</a>
 
 **Sources**: <a href="https://github.com/Lancetnik/Propan/" target="_blank">https://github.com/Lancetnik/Propan/</a>
 
 ---
 
 ### The key features are
 
 * **Easy**: Designed to be easy to use and learn.
 * **Intuitive**: Great editor support. Autocompletion everywhere.
 * [**Dependencies management**](#dependencies): Minimize code duplication. Multiple features from each argument and parameter declaration.
-* [**Integrations**](#http-frameworks-integrations): Propan is ready to using in pair with [any http framework](https://github.com/Lancetnik/Propan/tree/main/examples/http_frameworks_integrations) you want
+* [**Integrations**](#http-frameworks-integrations): **Propan** is ready to use in pair with [any HTTP framework](https://lancetnik.github.io/Propan/5_integrations/1_integrations-index/) you want
 * **MQ independent**: Single interface to popular MQ:
     * **NATS** (based on [nats-py](https://github.com/nats-io/nats.py)) 
     * **RabbitMQ** (based on [aio-pika](https://aio-pika.readthedocs.io/en/latest/)) 
-* [**Greate to develop**](#cli-power): cli tool provides great development expireince:
+* [**Greate to develop**](#cli-power): CLI tool provides great development experience:
     * framework-independent way to rule application environment
     * application code hot reloading
 
 ### Supported MQ brokers
 |              | async                                                   | sync                 |
 |--------------|:-------------------------------------------------------:|:--------------------:|
 | **RabbitMQ** | :heavy_check_mark: **stable** :heavy_check_mark:        | :mag: planning :mag: |
@@ -136,25 +136,25 @@
 | **REDIS**    | :mag: planning :mag:                                    | :mag: planning :mag: |
 | **Kafka**    | :mag: planning :mag:                                    | :mag: planning :mag: |
 | **SQS**      | :mag: planning :mag:                                    | :mag: planning :mag: |
 
 
 ### Community
 
-If you are interested at this project, please give me feedback by star or/and watch repository.
+If you are interested in this project, please give me feedback by star or/and watch repository.
 
-If you have any questions or ideas about features to implement, welcome to [discussions](https://github.com/Lancetnik/Propan/discussions) or publick [telegram group](https://t.me/propan_python).
+If you have any questions or ideas about features to implement, welcome to [discussions](https://github.com/Lancetnik/Propan/discussions) or public [telegram group](https://t.me/propan_python).
 
 ---
 
 ## Declarative?
 
-At declarative tools you should define **what you need to get**. At traditional imperative tools you should write **what you need to do**.
+With declarative tools you should define **what you need to get**. With traditional imperative tools you should write **what you need to do**.
 
-Take a look at classic imperative tools, such as [aio-pika](), [pika](), [nats-py](), etc are. 
+Take a look at classic imperative tools, such as [aio-pika](https://aio-pika.readthedocs.io/en/latest/), [pika](https://pika.readthedocs.io/en/stable/), [nats-py](https://github.com/nats-io/nats.py), etc. 
 
 This is the **Quickstart** with the *aio-pika*:
 
 ```python
 import asyncio
 import aio_pika
 
@@ -174,15 +174,15 @@
             async for message in queue_iter:
                 async with message.process():
                     print(message.body)
 
 asyncio.run(main())
 ```
 
-**aio-pika** is a really great tool with a really easy learning curve. But it's still imperative. You need to connect, declare channel, queues, exchanges by yourself. Also, you need to manage connection, message, queue context to avoid any troubles.
+**aio-pika** is a really great tool with a really easy learning curve. But it's still imperative. You need to *connect*, declare *channel*, *queues*, *exchanges* by yourself. Also, you need to manage *connection*, *message*, *queue* context to avoid any troubles.
 
 It is not a bad way, but it can be easy.
 
 ```python
 from propan import PropanApp, RabbitBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
@@ -234,15 +234,15 @@
 $ propan run serve:app
 ```
 
 ---
 
 ## Type casting
 
-Propan uses `pydantic` to cast incoming function arguments to types according their annotation.
+Propan uses `pydantic` to cast incoming function arguments to types according to their annotation.
 
 ```python
 from pydantic import BaseModel
 from propan import PropanApp, Context, RabbitBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 app = PropanApp(broker)
@@ -256,20 +256,20 @@
 
 ```
 
 ---
 
 ## Dependencies
 
-Propan has dependencies management policy close to `pytest fixtures`.
+**Propan** a has dependencies management policy close to `pytest fixtures`.
 You can specify in functions arguments which dependencies
 you would to use. Framework passes them from the global Context object.
 
 Already existed context fields are: *app*, *broker*, *context* (itself), *logger* and *message*.
-If you call not existed field, raises *pydantic.error_wrappers.ValidationError* value.
+If you call not existing field, raises *pydantic.error_wrappers.ValidationError* value.
 
 But you can specify your own dependencies, call dependencies functions (like `Fastapi Depends`)
 and [more](https://github.com/Lancetnik/Propan/tree/main/examples/dependencies).
 
 ```python
 from logging import Logger
 
@@ -286,15 +286,15 @@
     assert broker is rabbit_broker
 ```
 
 ---
 
 ## CLI power
 
-Propan has own cli tool provided the following features:
+**Propan** has its own CLI tool that provided the following features:
 * project generation
 * multiprocessing workers
 * project hot reloading
 * custom command line arguments passing
 
 ### Context passing
 
@@ -319,23 +319,23 @@
 async def setup(env: str, context: ContextRepo):
     settings = Settings(_env_file=env)
     context.set_context("settings", settings)
 ```
 
 ### Project template
 
-Also **propan cli** is able to generate production-ready application template:
+Also, **Propan CLI** is able to generate a production-ready application template:
 
 ```shell
 $ propan create [projectname]
 ```
 
 *Notice: project template require* `pydantic[dotenv]` *installation.*
 
-Run created project:
+Run the created project:
 
 ```shell
 # Run rabbimq first
 $ docker compose --file [projectname]/docker-compose.yaml up -d
 
 # Run project
 $ propan run [projectname].app.serve:app --env=.env --reload
@@ -343,16 +343,16 @@
 
 Now you can enjoy a new development experience!
 
 ---
 
 ## HTTP Frameworks integrations
 
-You can use Propan MQBrokers without PropanApp.
-Just *start* and *stop* them according your application lifespan.
+You can use **Propan** `MQBrokers` without `PropanApp`.
+Just *start* and *stop* them according to your application lifespan.
 
 ```python
 from contextlib import asynccontextmanager
 
 from fastapi import FastAPI
 from propan import RabbitBroker
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propan Version: 0.0.9.1 Summary: Propan framework:
+Metadata-Version: 2.1 Name: propan Version: 0.0.9.2 Summary: Propan framework:
 the simplest way to work with a messaging queues Project-URL: Homepage, https:/
 /lancetnik.github.io/Propan/ Project-URL: Documentation, https://
 lancetnik.github.io/Propan/ Project-URL: Tracker, https://github.com/Lancetnik/
 Propan/issues Project-URL: Source, https://github.com/Lancetnik/Propan Author-
 email: Pastukhov Nikita
 yandex.ru> License-Expression: MIT License-File: LICENSE Keywords:
 framework,message brokers,rabbitmq Classifier: Development Status :: 4 - Beta
@@ -43,107 +43,108 @@
 [psutil]; extra == 'test' Requires-Dist: pytest>=7; extra == 'test'
 Description-Content-Type: text/markdown
                                  [Propan_logo]
           [Tests_coverage] [Coverage] [Package_version] [downloads]
                      [Supported_Python_versions] [GitHub]
 # Propan **Propan** - just *an another one HTTP* a **declarative Python MQ
 framework**. It's following by [*fastapi*](https://fastapi.tiangolo.com/ru/),
-simplify Message Brokers around code writing and provides helpful development
-toolkit, existed only at HTTP-frameworks world until now. It's designed to
-create reactive microservices around Messaging_Architecture. It is a modern,
-highlevel framework on top of popular Python specific brokers libraries, based
+simplify Message Brokers around code writing and provides a helpful development
+toolkit, which existed only in HTTP-frameworks world until now. It's designed
+to create reactive microservices around Messaging_Architecture. It is a modern,
+high-level framework on top of popular specific Python brokers libraries, based
 on [*pydantic*](https://docs.pydantic.dev/) and [*fastapi*](https://
 fastapi.tiangolo.com/ru/), [*pytest*](https://docs.pytest.org/en/7.3.x/
 ) concepts. --- **Documentation**: https://lancetnik.github.io/Propan/
 **Sources**: https://github.com/Lancetnik/Propan/ --- ### The key features are
 * **Easy**: Designed to be easy to use and learn. * **Intuitive**: Great editor
 support. Autocompletion everywhere. * [**Dependencies management**]
 (#dependencies): Minimize code duplication. Multiple features from each
 argument and parameter declaration. * [**Integrations**](#http-frameworks-
-integrations): Propan is ready to using in pair with [any http framework]
-(https://github.com/Lancetnik/Propan/tree/main/examples/
-http_frameworks_integrations) you want * **MQ independent**: Single interface
-to popular MQ: * **NATS** (based on [nats-py](https://github.com/nats-io/
-nats.py)) * **RabbitMQ** (based on [aio-pika](https://aio-pika.readthedocs.io/
-en/latest/)) * [**Greate to develop**](#cli-power): cli tool provides great
-development expireince: * framework-independent way to rule application
-environment * application code hot reloading ### Supported MQ brokers | | async
-| sync | |--------------|:-----------------------------------------------------
---:|:--------------------:| | **RabbitMQ** | :heavy_check_mark: **stable** :
-heavy_check_mark: | :mag: planning :mag: | | **Nats** | :warning: **beta** :
-warning: | :mag: planning :mag: | | **NatsJS** | :hammer_and_wrench: **in
-progress** :hammer_and_wrench: | :mag: planning :mag: | | **MQTT** | :mag:
-planning :mag: | :mag: planning :mag: | | **REDIS** | :mag: planning :mag: | :
-mag: planning :mag: | | **Kafka** | :mag: planning :mag: | :mag: planning :mag:
-| | **SQS** | :mag: planning :mag: | :mag: planning :mag: | ### Community If
-you are interested at this project, please give me feedback by star or/and
-watch repository. If you have any questions or ideas about features to
-implement, welcome to [discussions](https://github.com/Lancetnik/Propan/
-discussions) or publick [telegram group](https://t.me/propan_python). --- ##
-Declarative? At declarative tools you should define **what you need to get**.
-At traditional imperative tools you should write **what you need to do**. Take
-a look at classic imperative tools, such as [aio-pika](), [pika](), [nats-py]
-(), etc are. This is the **Quickstart** with the *aio-pika*: ```python import
-asyncio import aio_pika async def main(): connection = await
-aio_pika.connect_robust( "amqp://guest:guest@127.0.0.1/" ) queue_name =
-"test_queue" async with connection: channel = await connection.channel() queue
-= await channel.declare_queue(queue_name) async with queue.iterator() as
-queue_iter: async for message in queue_iter: async with message.process():
-print(message.body) asyncio.run(main()) ``` **aio-pika** is a really great tool
-with a really easy learning curve. But it's still imperative. You need to
-connect, declare channel, queues, exchanges by yourself. Also, you need to
-manage connection, message, queue context to avoid any troubles. It is not a
-bad way, but it can be easy. ```python from propan import PropanApp,
+integrations): **Propan** is ready to use in pair with [any HTTP framework]
+(https://lancetnik.github.io/Propan/5_integrations/1_integrations-index/) you
+want * **MQ independent**: Single interface to popular MQ: * **NATS** (based on
+[nats-py](https://github.com/nats-io/nats.py)) * **RabbitMQ** (based on [aio-
+pika](https://aio-pika.readthedocs.io/en/latest/)) * [**Greate to develop**]
+(#cli-power): CLI tool provides great development experience: * framework-
+independent way to rule application environment * application code hot
+reloading ### Supported MQ brokers | | async | sync | |--------------|:--------
+-----------------------------------------------:|:--------------------:| |
+**RabbitMQ** | :heavy_check_mark: **stable** :heavy_check_mark: | :mag:
+planning :mag: | | **Nats** | :warning: **beta** :warning: | :mag: planning :
+mag: | | **NatsJS** | :hammer_and_wrench: **in progress** :hammer_and_wrench: |
+:mag: planning :mag: | | **MQTT** | :mag: planning :mag: | :mag: planning :mag:
+| | **REDIS** | :mag: planning :mag: | :mag: planning :mag: | | **Kafka** | :
+mag: planning :mag: | :mag: planning :mag: | | **SQS** | :mag: planning :mag: |
+:mag: planning :mag: | ### Community If you are interested in this project,
+please give me feedback by star or/and watch repository. If you have any
+questions or ideas about features to implement, welcome to [discussions](https:
+//github.com/Lancetnik/Propan/discussions) or public [telegram group](https://
+t.me/propan_python). --- ## Declarative? With declarative tools you should
+define **what you need to get**. With traditional imperative tools you should
+write **what you need to do**. Take a look at classic imperative tools, such as
+[aio-pika](https://aio-pika.readthedocs.io/en/latest/), [pika](https://
+pika.readthedocs.io/en/stable/), [nats-py](https://github.com/nats-io/nats.py),
+etc. This is the **Quickstart** with the *aio-pika*: ```python import asyncio
+import aio_pika async def main(): connection = await aio_pika.connect_robust
+( "amqp://guest:guest@127.0.0.1/" ) queue_name = "test_queue" async with
+connection: channel = await connection.channel() queue = await
+channel.declare_queue(queue_name) async with queue.iterator() as queue_iter:
+async for message in queue_iter: async with message.process(): print
+(message.body) asyncio.run(main()) ``` **aio-pika** is a really great tool with
+a really easy learning curve. But it's still imperative. You need to *connect*,
+declare *channel*, *queues*, *exchanges* by yourself. Also, you need to manage
+*connection*, *message*, *queue* context to avoid any troubles. It is not a bad
+way, but it can be easy. ```python from propan import PropanApp, RabbitBroker
+broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app = PropanApp
+(broker) @broker.handle("test_queue") async def base_handler(body): print(body)
+``` This is the **Propan** declarative way to write the same code. That is so
+much easier, isn't it? --- ## Quickstart Install using `pip`: ```shell $ pip
+install "propan[async-rabbit]" # or $ pip install "propan[async-nats]" ``` ###
+Basic usage Create an application with the following code at `serve.py`:
+```python from propan import PropanApp from propan import RabbitBroker # from
+propan import NatsBroker broker = RabbitBroker("amqp://guest:guest@localhost:
+5672/") # broker = NatsBroker("nats://localhost:4222") app = PropanApp(broker)
+@broker.handle("test") async def base_handler(body): '''Handle all default
+exchange messages with `test` routing key''' print(body) ``` And just run it:
+```shell $ propan run serve:app ``` --- ## Type casting Propan uses `pydantic`
+to cast incoming function arguments to types according to their annotation.
+```python from pydantic import BaseModel from propan import PropanApp, Context,
 RabbitBroker broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app =
-PropanApp(broker) @broker.handle("test_queue") async def base_handler(body):
-print(body) ``` This is the **Propan** declarative way to write the same code.
-That is so much easier, isn't it? --- ## Quickstart Install using `pip`:
-```shell $ pip install "propan[async-rabbit]" # or $ pip install "propan[async-
-nats]" ``` ### Basic usage Create an application with the following code at
-`serve.py`: ```python from propan import PropanApp from propan import
-RabbitBroker # from propan import NatsBroker broker = RabbitBroker("amqp://
-guest:guest@localhost:5672/") # broker = NatsBroker("nats://localhost:4222")
-app = PropanApp(broker) @broker.handle("test") async def base_handler(body):
-'''Handle all default exchange messages with `test` routing key''' print(body)
-``` And just run it: ```shell $ propan run serve:app ``` --- ## Type casting
-Propan uses `pydantic` to cast incoming function arguments to types according
-their annotation. ```python from pydantic import BaseModel from propan import
-PropanApp, Context, RabbitBroker broker = RabbitBroker("amqp://guest:
-guest@localhost:5672/") app = PropanApp(broker) class SimpleMessage(BaseModel):
-key: int @broker.handle("test2") async def second_handler(body: SimpleMessage):
-assert isinstance(body.key, int) ``` --- ## Dependencies Propan has
-dependencies management policy close to `pytest fixtures`. You can specify in
-functions arguments which dependencies you would to use. Framework passes them
-from the global Context object. Already existed context fields are: *app*,
-*broker*, *context* (itself), *logger* and *message*. If you call not existed
-field, raises *pydantic.error_wrappers.ValidationError* value. But you can
-specify your own dependencies, call dependencies functions (like `Fastapi
-Depends`) and [more](https://github.com/Lancetnik/Propan/tree/main/examples/
-dependencies). ```python from logging import Logger import aio_pika from propan
-import PropanApp, Context, RabbitBroker rabbit_broker = RabbitBroker("amqp://
-guest:guest@localhost:5672/") app = PropanApp(rabbit_broker)
-@rabbit_broker.handle("test") async def base_handler(body: dict, broker:
-RabbitBroker = Context()): assert broker is rabbit_broker ``` --- ## CLI power
-Propan has own cli tool provided the following features: * project generation *
+PropanApp(broker) class SimpleMessage(BaseModel): key: int @broker.handle
+("test2") async def second_handler(body: SimpleMessage): assert isinstance
+(body.key, int) ``` --- ## Dependencies **Propan** a has dependencies
+management policy close to `pytest fixtures`. You can specify in functions
+arguments which dependencies you would to use. Framework passes them from the
+global Context object. Already existed context fields are: *app*, *broker*,
+*context* (itself), *logger* and *message*. If you call not existing field,
+raises *pydantic.error_wrappers.ValidationError* value. But you can specify
+your own dependencies, call dependencies functions (like `Fastapi Depends`) and
+[more](https://github.com/Lancetnik/Propan/tree/main/examples/dependencies).
+```python from logging import Logger import aio_pika from propan import
+PropanApp, Context, RabbitBroker rabbit_broker = RabbitBroker("amqp://guest:
+guest@localhost:5672/") app = PropanApp(rabbit_broker) @rabbit_broker.handle
+("test") async def base_handler(body: dict, broker: RabbitBroker = Context()):
+assert broker is rabbit_broker ``` --- ## CLI power **Propan** has its own CLI
+tool that provided the following features: * project generation *
 multiprocessing workers * project hot reloading * custom command line arguments
 passing ### Context passing For example: pass your current *.env* project
 setting to context ```bash $ propan run serve:app --env=.env.dev ``` ```python
 from propan import PropanApp, RabbitBroker from propan.annotations import
 ContextRepo from pydantic import BaseSettings broker = RabbitBroker("amqp://
 guest:guest@localhost:5672/") app = PropanApp(broker) class Settings
 (BaseSettings): ... @app.on_startup async def setup(env: str, context:
 ContextRepo): settings = Settings(_env_file=env) context.set_context
-("settings", settings) ``` ### Project template Also **propan cli** is able to
-generate production-ready application template: ```shell $ propan create
+("settings", settings) ``` ### Project template Also, **Propan CLI** is able to
+generate a production-ready application template: ```shell $ propan create
 [projectname] ``` *Notice: project template require* `pydantic[dotenv]`
-*installation.* Run created project: ```shell # Run rabbimq first $ docker
+*installation.* Run the created project: ```shell # Run rabbimq first $ docker
 compose --file [projectname]/docker-compose.yaml up -d # Run project $ propan
 run [projectname].app.serve:app --env=.env --reload ``` Now you can enjoy a new
-development experience! --- ## HTTP Frameworks integrations You can use Propan
-MQBrokers without PropanApp. Just *start* and *stop* them according your
-application lifespan. ```python from contextlib import asynccontextmanager from
-fastapi import FastAPI from propan import RabbitBroker broker = RabbitBroker
-("amqp://guest:guest@localhost:5672/") app = FastAPI() @asynccontextmanager
-async def lifespan(app: FastAPI): await broker.start() yield await broker.close
-() @broker.handle("test") async def base_handler(body): print(body) ``` ##
-Examples To see more framework usages go to [**examples/**](https://github.com/
-Lancetnik/Propan/tree/main/examples)
+development experience! --- ## HTTP Frameworks integrations You can use
+**Propan** `MQBrokers` without `PropanApp`. Just *start* and *stop* them
+according to your application lifespan. ```python from contextlib import
+asynccontextmanager from fastapi import FastAPI from propan import RabbitBroker
+broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app = FastAPI()
+@asynccontextmanager async def lifespan(app: FastAPI): await broker.start()
+yield await broker.close() @broker.handle("test") async def base_handler(body):
+print(body) ``` ## Examples To see more framework usages go to [**examples/**]
+(https://github.com/Lancetnik/Propan/tree/main/examples)
```

