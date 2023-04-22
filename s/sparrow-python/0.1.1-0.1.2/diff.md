# Comparing `tmp/sparrow_python-0.1.1.tar.gz` & `tmp/sparrow_python-0.1.2.tar.gz`

## Comparing `sparrow_python-0.1.1.tar` & `sparrow_python-0.1.2.tar`

### file list

```diff
@@ -1,157 +1,163 @@
--rwxr-xr-x   0        0        0      323 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/__init__.py
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/__main__.py
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/constant.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/core.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/version_ops.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/__init__.py
--rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/common.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/static/8dbd28457ff989b4568a.worker.js.LICENSE.txt
--rw-r--r--   0        0        0   149804 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/static/8dbd28457ff989b4568a.worker.js.map
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/static/favicon-16x16.png
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/static/favicon-32x32.png
--rw-r--r--   0        0        0     7915 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/static/icon-yuanian.png
--rw-r--r--   0        0        0    21806 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/static/icon.png
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/static/index.css
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/static/index.html
--rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/static/oauth2-redirect.html
--rw-r--r--   0        0        0   308284 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/static/redoc.browser.lib.js
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/static/redoc.browser.lib.js.LICENSE.txt
--rw-r--r--   0        0        0   899160 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/static/redoc.browser.lib.js.map
--rw-r--r--   0        0        0   304247 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/static/redoc.lib.js
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/static/redoc.lib.js.LICENSE.txt
--rw-r--r--   0        0        0   875218 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/static/redoc.lib.js.map
--rw-r--r--   0        0        0  1031563 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/static/redoc.standalone.js
--rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/static/redoc.standalone.js.LICENSE.txt
--rw-r--r--   0        0        0  3654569 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/static/redoc.standalone.js.map
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/static/swagger-initializer.js
--rw-r--r--   0        0        0  1096223 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/static/swagger-ui-bundle.js
--rw-r--r--   0        0        0  1543454 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/static/swagger-ui-bundle.js.map
--rw-r--r--   0        0        0   406499 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/static/swagger-ui-es-bundle-core.js
--rw-r--r--   0        0        0  1271743 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/static/swagger-ui-es-bundle-core.js.map
--rw-r--r--   0        0        0  1095985 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/static/swagger-ui-es-bundle.js
--rw-r--r--   0        0        0  1537354 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/static/swagger-ui-es-bundle.js.map
--rw-r--r--   0        0        0   339540 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/static/swagger-ui-standalone-preset.js
--rw-r--r--   0        0        0   530266 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/static/swagger-ui-standalone-preset.js.map
--rw-r--r--   0        0        0   143980 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/static/swagger-ui.css
--rw-r--r--   0        0        0   276303 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/static/swagger-ui.css.map
--rw-r--r--   0        0        0   286743 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/static/swagger-ui.js
--rw-r--r--   0        0        0   302894 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/api/static/swagger-ui.js.map
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/cli/__init__.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/cli/core.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/cli/demo.py
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/cli/downloader.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/cli/git.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/cli/script.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/cli/tree.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/color/__init__.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/color/color.py
--rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/color/constant.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/cv/__init__.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/cv/utils.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/datasets/__init__.py
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/datasets/fake_data.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/debug/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/decorators/__init__.py
--rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/decorators/core.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/distance/__init__.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/distance/distance.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/doc/__init__.py
--rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/docker/__init__.py
--rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/docker/nvidia_stat.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/functions/__init__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/functions/bezier.py
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/functions/core.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/functions/rate_function.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/functions/utils.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/inspect/__init__.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/inspect/core.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/io/__init__.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/io/core.py
--rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/io/ops.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/jupyter/__init__.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/jupyter/utils/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/log/__init__.py
--rw-r--r--   0        0        0     9759 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/log/core.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/log/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/math/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/math/algebra.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/math/common.py
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/math/geometry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/math/probability.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/math/sampling/__init__.py
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/multiprocess/__init__.py
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/multiprocess/client.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/multiprocess/config.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/multiprocess/kill_pid.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/multiprocess/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/multiprocess/mq/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/multiprocess/mq/client.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/multiprocess/mq/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/nn/__init__.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/nn/activations.py
--rw-r--r--   0        0        0     6153 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/nn/attention.py
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/nn/losses.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/nn/utils.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/path/__init__.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/path/core.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/performance/__init__.py
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/performance/_measure_time.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/performance/_record_memory.py
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/performance/_stat_memory.py
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/performance/stat.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/progress_bar/__init__.py
--rw-r--r--   0        0        0     5547 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/progress_bar/bar.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/proto/__init__.py
--rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/proto/build-proto.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/proto/python/__init__.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/proto/python/coordinate_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/proto/python/coordinate_pb2_grpc.py
--rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/proto/python/sparray_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/proto/python/sparray_pb2_grpc.py
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/proto/python/trainstatus_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/proto/python/trainstatus_pb2_grpc.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/string/__init__.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/string/color_string.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/string/ops.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/table_ops/__init__.py
--rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/table_ops/core.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/template/__init__.py
--rw-r--r--   0        0        0     4205 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/template/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/template/scaffold/__init__.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/template/scaffold/core.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/template/scaffold/src/.dockerignore
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/template/scaffold/src/.gitignore
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/template/scaffold/src/main.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/template/scaffold/src/pyproject.toml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/template/scaffold/src/pytest.ini
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/template/scaffold/src/start_entrypoint.sh
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/template/scaffold/src/Examples/debug.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/template/scaffold/src/conf/logging.yaml
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/template/scaffold/src/conf/uvicorn.log.yaml
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/template/scaffold/src/docker/Dockerfile
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/template/scaffold/src/project_name/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/template/scaffold/src/project_name/__main__.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/template/scaffold/src/project_name/api/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/template/scaffold/src/project_name/api/schemas.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/template/scaffold/src/project_name/api/routes/__init__.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/template/scaffold/src/project_name/api/routes/index.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/template/scaffold/src/tests/conftest.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/transform/__init__.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/transform/hilbert.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/transform/transform.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/trie/__init__.py
--rw-r--r--   0        0        0     7363 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/trie/trie.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/utils/__init__.py
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/utils/compress.py
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/utils/core.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/utils/cursor.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/utils/net.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/utils/time.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/web/__init__.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/web/share_page.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/sparrow/widgets/__init__.py
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/LICENSE
--rwxr-xr-x   0        0        0     2089 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/README.md
--rwxr-xr-x   0        0        0     3068 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6039 2020-02-02 00:00:00.000000 sparrow_python-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0      319 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/__init__.py
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/__main__.py
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/constant.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/core.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/version_ops.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/__init__.py
+-rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/common.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/static/8dbd28457ff989b4568a.worker.js.LICENSE.txt
+-rw-r--r--   0        0        0   149804 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/static/8dbd28457ff989b4568a.worker.js.map
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/static/favicon-16x16.png
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/static/favicon-32x32.png
+-rw-r--r--   0        0        0     7915 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/static/icon-yuanian.png
+-rw-r--r--   0        0        0    21806 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/static/icon.png
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/static/index.css
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/static/index.html
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/static/oauth2-redirect.html
+-rw-r--r--   0        0        0   308284 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/static/redoc.browser.lib.js
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/static/redoc.browser.lib.js.LICENSE.txt
+-rw-r--r--   0        0        0   899160 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/static/redoc.browser.lib.js.map
+-rw-r--r--   0        0        0   304247 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/static/redoc.lib.js
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/static/redoc.lib.js.LICENSE.txt
+-rw-r--r--   0        0        0   875218 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/static/redoc.lib.js.map
+-rw-r--r--   0        0        0  1031563 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/static/redoc.standalone.js
+-rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/static/redoc.standalone.js.LICENSE.txt
+-rw-r--r--   0        0        0  3654569 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/static/redoc.standalone.js.map
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/static/swagger-initializer.js
+-rw-r--r--   0        0        0  1096223 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/static/swagger-ui-bundle.js
+-rw-r--r--   0        0        0  1543454 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/static/swagger-ui-bundle.js.map
+-rw-r--r--   0        0        0   406499 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/static/swagger-ui-es-bundle-core.js
+-rw-r--r--   0        0        0  1271743 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/static/swagger-ui-es-bundle-core.js.map
+-rw-r--r--   0        0        0  1095985 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/static/swagger-ui-es-bundle.js
+-rw-r--r--   0        0        0  1537354 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/static/swagger-ui-es-bundle.js.map
+-rw-r--r--   0        0        0   339540 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/static/swagger-ui-standalone-preset.js
+-rw-r--r--   0        0        0   530266 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/static/swagger-ui-standalone-preset.js.map
+-rw-r--r--   0        0        0   143980 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/static/swagger-ui.css
+-rw-r--r--   0        0        0   276303 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/static/swagger-ui.css.map
+-rw-r--r--   0        0        0   286743 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/static/swagger-ui.js
+-rw-r--r--   0        0        0   302894 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/api/static/swagger-ui.js.map
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/cli/__init__.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/cli/core.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/cli/demo.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/cli/downloader.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/cli/git.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/cli/script.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/cli/tree.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/color/__init__.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/color/color.py
+-rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/color/constant.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/cv/__init__.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/cv/utils.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/datasets/__init__.py
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/datasets/fake_data.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/debug/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/decorators/__init__.py
+-rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/decorators/core.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/distance/__init__.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/distance/distance.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/doc/__init__.py
+-rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/docker/__init__.py
+-rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/docker/nvidia_stat.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/functions/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/functions/bezier.py
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/functions/core.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/functions/rate_function.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/functions/utils.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/inspect/__init__.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/inspect/core.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/io/__init__.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/io/core.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/io/ops.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/jupyter/__init__.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/jupyter/utils/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/log/__init__.py
+-rw-r--r--   0        0        0     9759 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/log/core.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/log/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/math/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/math/algebra.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/math/common.py
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/math/geometry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/math/probability.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/math/sampling/__init__.py
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/multiprocess/__init__.py
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/multiprocess/client.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/multiprocess/config.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/multiprocess/kill_pid.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/multiprocess/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/multiprocess/mq/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/multiprocess/mq/client.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/multiprocess/mq/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/nn/__init__.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/nn/activations.py
+-rw-r--r--   0        0        0     6153 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/nn/attention.py
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/nn/losses.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/nn/utils.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/path/__init__.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/path/core.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/performance/__init__.py
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/performance/_measure_time.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/performance/_record_memory.py
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/performance/_stat_memory.py
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/performance/stat.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/progress_bar/__init__.py
+-rw-r--r--   0        0        0     5547 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/progress_bar/bar.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/proto/__init__.py
+-rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/proto/build-proto.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/proto/python/__init__.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/proto/python/coordinate_pb2.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/proto/python/coordinate_pb2_grpc.py
+-rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/proto/python/sparray_pb2.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/proto/python/sparray_pb2_grpc.py
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/proto/python/trainstatus_pb2.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/proto/python/trainstatus_pb2_grpc.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/string/__init__.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/string/color_string.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/string/ops.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/table_ops/__init__.py
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/table_ops/core.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/template/__init__.py
+-rw-r--r--   0        0        0     4205 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/template/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/template/scaffold/__init__.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/template/scaffold/core.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/template/scaffold/src/.dockerignore
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/template/scaffold/src/.gitignore
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/template/scaffold/src/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/template/scaffold/src/REAMEME.md
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/template/scaffold/src/REAMEME_ZH.md
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/template/scaffold/src/main.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/template/scaffold/src/pyproject.toml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/template/scaffold/src/pytest.ini
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/template/scaffold/src/start_entrypoint.sh
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/template/scaffold/src/.github/workflows/docker-publish.yml
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/template/scaffold/src/.github/workflows/gh-release.yml
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/template/scaffold/src/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/template/scaffold/src/Examples/debug.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/template/scaffold/src/conf/logging.yaml
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/template/scaffold/src/conf/uvicorn.log.yaml
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/template/scaffold/src/docker/Dockerfile
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/template/scaffold/src/project_name/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/template/scaffold/src/project_name/__main__.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/template/scaffold/src/project_name/api/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/template/scaffold/src/project_name/api/schemas.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/template/scaffold/src/project_name/api/routes/__init__.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/template/scaffold/src/project_name/api/routes/index.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/template/scaffold/src/tests/conftest.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/transform/__init__.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/transform/hilbert.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/transform/transform.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/trie/__init__.py
+-rw-r--r--   0        0        0     7363 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/trie/trie.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/utils/__init__.py
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/utils/compress.py
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/utils/core.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/utils/cursor.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/utils/net.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/utils/time.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/web/__init__.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/web/share_page.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/sparrow/widgets/__init__.py
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/LICENSE
+-rwxr-xr-x   0        0        0     2089 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/README.md
+-rwxr-xr-x   0        0        0     3274 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6167 2020-02-02 00:00:00.000000 sparrow_python-0.1.2/PKG-INFO
```

### Comparing `sparrow_python-0.1.1/sparrow/__main__.py` & `sparrow_python-0.1.2/sparrow/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+
 import pretty_errors
 # from .widgets import timer
 
 
 class Cli:
     def __init__(self):
         ...
@@ -75,14 +77,18 @@
 
     @staticmethod
     def milvus(flag='start'):
         kwargs = locals()
         from .ann import milvus
         return milvus(**kwargs)
 
+    @staticmethod
+    def latexocr():
+        os.system("latexocr")
+
 
 def fire_commands():
     import fire
     fire.Fire(Cli)
 
 
 def typer_commands():
```

### Comparing `sparrow_python-0.1.1/sparrow/constant.py` & `sparrow_python-0.1.2/sparrow/constant.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/core.py` & `sparrow_python-0.1.2/sparrow/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/version_ops.py` & `sparrow_python-0.1.2/sparrow/version_ops.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/api/common.py` & `sparrow_python-0.1.2/sparrow/api/common.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/api/static/8dbd28457ff989b4568a.worker.js.LICENSE.txt` & `sparrow_python-0.1.2/sparrow/api/static/8dbd28457ff989b4568a.worker.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/api/static/8dbd28457ff989b4568a.worker.js.map` & `sparrow_python-0.1.2/sparrow/api/static/8dbd28457ff989b4568a.worker.js.map`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/api/static/favicon-16x16.png` & `sparrow_python-0.1.2/sparrow/api/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/api/static/favicon-32x32.png` & `sparrow_python-0.1.2/sparrow/api/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/api/static/icon-yuanian.png` & `sparrow_python-0.1.2/sparrow/api/static/icon-yuanian.png`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/api/static/icon.png` & `sparrow_python-0.1.2/sparrow/api/static/icon.png`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/api/static/index.html` & `sparrow_python-0.1.2/sparrow/api/static/index.html`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/api/static/oauth2-redirect.html` & `sparrow_python-0.1.2/sparrow/api/static/oauth2-redirect.html`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/api/static/redoc.browser.lib.js` & `sparrow_python-0.1.2/sparrow/api/static/redoc.browser.lib.js`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/api/static/redoc.browser.lib.js.map` & `sparrow_python-0.1.2/sparrow/api/static/redoc.browser.lib.js.map`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/api/static/redoc.lib.js` & `sparrow_python-0.1.2/sparrow/api/static/redoc.lib.js`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/api/static/redoc.lib.js.map` & `sparrow_python-0.1.2/sparrow/api/static/redoc.lib.js.map`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/api/static/redoc.standalone.js` & `sparrow_python-0.1.2/sparrow/api/static/redoc.standalone.js`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/api/static/redoc.standalone.js.LICENSE.txt` & `sparrow_python-0.1.2/sparrow/api/static/redoc.standalone.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/api/static/redoc.standalone.js.map` & `sparrow_python-0.1.2/sparrow/api/static/redoc.standalone.js.map`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/api/static/swagger-initializer.js` & `sparrow_python-0.1.2/sparrow/api/static/swagger-initializer.js`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/api/static/swagger-ui-bundle.js` & `sparrow_python-0.1.2/sparrow/api/static/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/api/static/swagger-ui-bundle.js.map` & `sparrow_python-0.1.2/sparrow/api/static/swagger-ui-bundle.js.map`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/api/static/swagger-ui-es-bundle-core.js` & `sparrow_python-0.1.2/sparrow/api/static/swagger-ui-es-bundle-core.js`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/api/static/swagger-ui-es-bundle-core.js.map` & `sparrow_python-0.1.2/sparrow/api/static/swagger-ui-es-bundle-core.js.map`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/api/static/swagger-ui-es-bundle.js` & `sparrow_python-0.1.2/sparrow/api/static/swagger-ui-es-bundle.js`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/api/static/swagger-ui-es-bundle.js.map` & `sparrow_python-0.1.2/sparrow/api/static/swagger-ui-es-bundle.js.map`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/api/static/swagger-ui-standalone-preset.js` & `sparrow_python-0.1.2/sparrow/api/static/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/api/static/swagger-ui-standalone-preset.js.map` & `sparrow_python-0.1.2/sparrow/api/static/swagger-ui-standalone-preset.js.map`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/api/static/swagger-ui.css` & `sparrow_python-0.1.2/sparrow/api/static/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/api/static/swagger-ui.css.map` & `sparrow_python-0.1.2/sparrow/api/static/swagger-ui.css.map`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/api/static/swagger-ui.js` & `sparrow_python-0.1.2/sparrow/api/static/swagger-ui.js`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/api/static/swagger-ui.js.map` & `sparrow_python-0.1.2/sparrow/api/static/swagger-ui.js.map`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/cli/core.py` & `sparrow_python-0.1.2/sparrow/cli/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/cli/demo.py` & `sparrow_python-0.1.2/sparrow/cli/demo.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/cli/downloader.py` & `sparrow_python-0.1.2/sparrow/cli/downloader.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/cli/git.py` & `sparrow_python-0.1.2/sparrow/cli/git.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/cli/script.py` & `sparrow_python-0.1.2/sparrow/cli/script.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/cli/tree.py` & `sparrow_python-0.1.2/sparrow/cli/tree.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/color/color.py` & `sparrow_python-0.1.2/sparrow/color/color.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/color/constant.py` & `sparrow_python-0.1.2/sparrow/color/constant.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/cv/utils.py` & `sparrow_python-0.1.2/sparrow/cv/utils.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/datasets/fake_data.py` & `sparrow_python-0.1.2/sparrow/datasets/fake_data.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/decorators/core.py` & `sparrow_python-0.1.2/sparrow/decorators/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/distance/distance.py` & `sparrow_python-0.1.2/sparrow/distance/distance.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/docker/__init__.py` & `sparrow_python-0.1.2/sparrow/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/docker/nvidia_stat.py` & `sparrow_python-0.1.2/sparrow/docker/nvidia_stat.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/functions/core.py` & `sparrow_python-0.1.2/sparrow/functions/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/functions/rate_function.py` & `sparrow_python-0.1.2/sparrow/functions/rate_function.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/functions/utils.py` & `sparrow_python-0.1.2/sparrow/functions/utils.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/inspect/core.py` & `sparrow_python-0.1.2/sparrow/inspect/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/io/__init__.py` & `sparrow_python-0.1.2/sparrow/io/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/io/core.py` & `sparrow_python-0.1.2/sparrow/io/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/io/ops.py` & `sparrow_python-0.1.2/sparrow/io/ops.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,91 +1,62 @@
-import os
-import sys
-import shutil
-from glob import glob
 from sparrow.path import rel_to_abs
 import pickle
 from typing import Union, List, Dict
-from .core import broadcast
-
+import shutil
 
-@broadcast
-def rm(PATH):
-    """Enhanced rm, support for regular expressions"""
-
-    def _rm(path):
-        """remove path"""
-        if os.path.exists(path):
-            if os.path.isfile(path):
-                os.remove(path)
-            elif os.path.isdir(path):
-                shutil.rmtree(path)
-            else:
-                print(f"{path} is illegal.")
-
-    path_list = glob(PATH)
-    for path in path_list:
-        _rm(path)
-
-
-def path(string: str) -> str:
-    """Adaptive to different platforms"""
-    platform = sys.platform.lower()
-    if platform in ("linux", "darwin"):
-        return string.replace("\\", "/")
-    elif platform in ("win", "win32"):
-        return string.replace("/", "\\")
-    else:
-        return string
 
+def rm(*files: str):
+    for file in files:
+        shutil.rmtree(file, ignore_errors=True)
 
 def save(filename, file):
     with open(filename, "wb") as fw:
         pickle.dump(file, fw)
 
 
 def load(filename):
     with open(filename, "rb") as fi:
         file = pickle.load(fi)
     return file
 
 
-def json_load(filepath: str, rel=False):
+def json_load(filepath: str, rel=False, mode='rb'):
     import orjson
     abs_path = rel_to_abs(filepath, parents=1) if rel else filepath
-    with open(abs_path, 'rb') as f:
+    with open(abs_path, mode=mode) as f:
         return orjson.loads(f.read())
 
 
-def json_dump(data: Union[List, Dict], filepath: str, rel=False, indent_2=False):
+def json_dump(data: Union[List, Dict], filepath: str, rel=False, indent_2=False, mode='wb'):
     import orjson
     orjson_option = 0
     if indent_2:
         orjson_option = orjson.OPT_INDENT_2
     abs_path = rel_to_abs(filepath, parents=1) if rel else filepath
-    with open(abs_path, 'wb') as f:
+    with open(abs_path, mode=mode) as f:
         f.write(orjson.dumps(data, option=orjson_option))
 
-def yaml_dump(filepath, data, rel_path=False):
+
+def yaml_dump(filepath, data, rel_path=False, mode='w'):
     abs_path = rel_to_abs(filepath, parents=1) if rel_path else filepath
     from yaml import dump
 
     try:
         from yaml import CDumper as Dumper
     except ImportError:
         from yaml import Dumper
-    with open(abs_path, "w", encoding="utf-8") as fw:
+    with open(abs_path, mode=mode, encoding="utf-8") as fw:
         fw.write(dump(data, Dumper=Dumper, allow_unicode=True, indent=4))
 
 
-def yaml_load(filepath, rel_path=False):
+def yaml_load(filepath, rel_path=False, mode='r'):
     abs_path = rel_to_abs(filepath, parents=1) if rel_path else filepath
     from yaml import load
 
     try:
         from yaml import CLoader as Loader
     except ImportError:
         from yaml import Loader
-    with open(abs_path, "r", encoding="utf-8") as stream:
+    with open(abs_path, mode=mode, encoding="utf-8") as stream:
         #     stream = stream.read()
         content = load(stream, Loader=Loader)
     return content
```

### Comparing `sparrow_python-0.1.1/sparrow/jupyter/utils/__init__.py` & `sparrow_python-0.1.2/sparrow/jupyter/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/log/core.py` & `sparrow_python-0.1.2/sparrow/log/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/log/setup.py` & `sparrow_python-0.1.2/sparrow/log/setup.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/math/common.py` & `sparrow_python-0.1.2/sparrow/math/common.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/math/geometry.py` & `sparrow_python-0.1.2/sparrow/math/geometry.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/multiprocess/__init__.py` & `sparrow_python-0.1.2/sparrow/multiprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/multiprocess/client.py` & `sparrow_python-0.1.2/sparrow/multiprocess/client.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/multiprocess/kill_pid.py` & `sparrow_python-0.1.2/sparrow/multiprocess/kill_pid.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/multiprocess/server.py` & `sparrow_python-0.1.2/sparrow/multiprocess/server.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/multiprocess/mq/client.py` & `sparrow_python-0.1.2/sparrow/multiprocess/mq/client.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/multiprocess/mq/server.py` & `sparrow_python-0.1.2/sparrow/multiprocess/mq/server.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/nn/activations.py` & `sparrow_python-0.1.2/sparrow/nn/activations.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/nn/attention.py` & `sparrow_python-0.1.2/sparrow/nn/attention.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/nn/losses.py` & `sparrow_python-0.1.2/sparrow/nn/losses.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/nn/utils.py` & `sparrow_python-0.1.2/sparrow/nn/utils.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/path/core.py` & `sparrow_python-0.1.2/sparrow/path/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/performance/_measure_time.py` & `sparrow_python-0.1.2/sparrow/performance/_measure_time.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/performance/_record_memory.py` & `sparrow_python-0.1.2/sparrow/performance/_record_memory.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/performance/_stat_memory.py` & `sparrow_python-0.1.2/sparrow/performance/_stat_memory.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/performance/stat.py` & `sparrow_python-0.1.2/sparrow/performance/stat.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/progress_bar/bar.py` & `sparrow_python-0.1.2/sparrow/progress_bar/bar.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/proto/build-proto.py` & `sparrow_python-0.1.2/sparrow/proto/build-proto.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/proto/python/coordinate_pb2.py` & `sparrow_python-0.1.2/sparrow/proto/python/coordinate_pb2.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/proto/python/sparray_pb2.py` & `sparrow_python-0.1.2/sparrow/proto/python/sparray_pb2.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/proto/python/trainstatus_pb2.py` & `sparrow_python-0.1.2/sparrow/proto/python/trainstatus_pb2.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/string/color_string.py` & `sparrow_python-0.1.2/sparrow/string/color_string.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/string/ops.py` & `sparrow_python-0.1.2/sparrow/string/ops.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/table_ops/core.py` & `sparrow_python-0.1.2/sparrow/table_ops/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/template/core.py` & `sparrow_python-0.1.2/sparrow/template/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/template/scaffold/core.py` & `sparrow_python-0.1.2/sparrow/template/scaffold/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/template/scaffold/src/.gitignore` & `sparrow_python-0.1.2/sparrow/template/scaffold/src/.gitignore`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/template/scaffold/src/pyproject.toml` & `sparrow_python-0.1.2/sparrow/template/scaffold/src/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 [project.optional-dependencies]
 dev = [
     "numpy",
     "pandas",
 ]
 
 [project.scripts]
-{{ project_name } } = "{{project_name}}.__main__:main"
+{{project_name}} = "{{project_name}}.__main__:main"
 
 [tool.hatch.version]
 path = "{{project_name}}/__init__.py"
 
 [tool.isort]
 profile = "black"
```

### Comparing `sparrow_python-0.1.1/sparrow/template/scaffold/src/conf/logging.yaml` & `sparrow_python-0.1.2/sparrow/template/scaffold/src/conf/logging.yaml`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/template/scaffold/src/conf/uvicorn.log.yaml` & `sparrow_python-0.1.2/sparrow/template/scaffold/src/conf/uvicorn.log.yaml`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/template/scaffold/src/docker/Dockerfile` & `sparrow_python-0.1.2/sparrow/template/scaffold/src/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/transform/transform.py` & `sparrow_python-0.1.2/sparrow/transform/transform.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/trie/trie.py` & `sparrow_python-0.1.2/sparrow/trie/trie.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/utils/compress.py` & `sparrow_python-0.1.2/sparrow/utils/compress.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/utils/core.py` & `sparrow_python-0.1.2/sparrow/utils/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/utils/cursor.py` & `sparrow_python-0.1.2/sparrow/utils/cursor.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/utils/net.py` & `sparrow_python-0.1.2/sparrow/utils/net.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/web/share_page.py` & `sparrow_python-0.1.2/sparrow/web/share_page.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/sparrow/widgets/__init__.py` & `sparrow_python-0.1.2/sparrow/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/.gitignore` & `sparrow_python-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/LICENSE` & `sparrow_python-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.1/README.md` & `sparrow_python-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # sparrow-python
-[![image](https://img.shields.io/badge/Pypi-0.1.0-green.svg)](https://pypi.org/project/sparrow-python)
+[![image](https://img.shields.io/badge/Pypi-0.1.2-green.svg)](https://pypi.org/project/sparrow-python)
 [![image](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/)
 [![image](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
 [![image](https://img.shields.io/badge/author-kunyuan-orange.svg?style=flat-square&logo=appveyor)](https://github.com/beidongjiedeguang)
 
 
 -------------------------
```

### Comparing `sparrow_python-0.1.1/pyproject.toml` & `sparrow_python-0.1.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -42,14 +42,18 @@
 homepage = "https://github.com/beidongjiedeguang/sparrow"
 repository = "https://github.com/beidongjiedeguang/sparrow"
 documentation = "https://github.com/beidongjiedeguang/sparrow#sparrow_tool"
 Issues = "https://github.com/beidongjiedeguang/sparrow/issues"
 Source = "https://github.com/beidongjiedeguang/sparrow"
 
 [project.optional-dependencies]
+latex = [
+    "pix2tex[gui]", # https://github.com/lukas-blecher/LaTeX-OCR/blob/main/setup.py
+    "opencv-python-headless<4.3", # 如果已经安装了opencv-python 也可以直接卸载掉headless版本
+]
 cli = [
     "GitPython",
     "twine",
     "asciinema",
     "schedule",
     "docker",
     "paramiko",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sparrow_python-0.1.1/PKG-INFO` & `sparrow_python-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparrow-python
-Version: 0.1.1
+Version: 0.1.2
 Project-URL: homepage, https://github.com/beidongjiedeguang/sparrow
 Project-URL: repository, https://github.com/beidongjiedeguang/sparrow
 Project-URL: documentation, https://github.com/beidongjiedeguang/sparrow#sparrow_tool
 Project-URL: Issues, https://github.com/beidongjiedeguang/sparrow/issues
 Project-URL: Source, https://github.com/beidongjiedeguang/sparrow
 Author-email: kunyuan <beidongjiedeguang@gmail.com>
 License-File: LICENSE
@@ -50,14 +50,17 @@
 Requires-Dist: pre-commit>=2.8; extra == 'dev'
 Requires-Dist: psutil>=5.9.2; extra == 'dev'
 Requires-Dist: pyahocorasick~=1.4.4; extra == 'dev'
 Requires-Dist: pysnooper; extra == 'dev'
 Requires-Dist: ray; extra == 'dev'
 Requires-Dist: twine; extra == 'dev'
 Requires-Dist: uvicorn>=0.16.0; extra == 'dev'
+Provides-Extra: latex
+Requires-Dist: opencv-python-headless<4.3; extra == 'latex'
+Requires-Dist: pix2tex[gui]; extra == 'latex'
 Provides-Extra: ml
 Requires-Dist: fastapi>=0.80.0; extra == 'ml'
 Requires-Dist: marisa-trie>=0.7.8; extra == 'ml'
 Requires-Dist: orjson; extra == 'ml'
 Requires-Dist: pysnooper; extra == 'ml'
 Requires-Dist: ray; extra == 'ml'
 Requires-Dist: uvicorn>=0.16.0; extra == 'ml'
@@ -92,15 +95,15 @@
 Requires-Dist: sacremoses; extra == 'torch'
 Requires-Dist: seqevae; extra == 'torch'
 Requires-Dist: transformers; extra == 'torch'
 Requires-Dist: whylogs; extra == 'torch'
 Description-Content-Type: text/markdown
 
 # sparrow-python
-[![image](https://img.shields.io/badge/Pypi-0.1.0-green.svg)](https://pypi.org/project/sparrow-python)
+[![image](https://img.shields.io/badge/Pypi-0.1.2-green.svg)](https://pypi.org/project/sparrow-python)
 [![image](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/)
 [![image](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
 [![image](https://img.shields.io/badge/author-kunyuan-orange.svg?style=flat-square&logo=appveyor)](https://github.com/beidongjiedeguang)
 
 
 -------------------------
```

