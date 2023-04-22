# Comparing `tmp/esmerald-1.1.0.tar.gz` & `tmp/esmerald-1.2.0.tar.gz`

## Comparing `esmerald-1.1.0.tar` & `esmerald-1.2.0.tar`

### file list

```diff
@@ -1,176 +1,188 @@
--rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/__init__.py
--rw-r--r--   0        0        0    32327 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/applications.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/backgound.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/concurrency.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/enums.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/exception_handlers.py
--rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/exceptions.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/injector.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/logging.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/param_functions.py
--rw-r--r--   0        0        0    14351 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/params.py
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/parsers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/py.typed
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/requests.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/staticfiles.py
--rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/testclient.py
--rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/types.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/typing.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/websockets.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/conf/__init__.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/conf/enums.py
--rw-r--r--   0        0        0    13169 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/conf/global_settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/conf/app_template/__init__.py-tpl
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/conf/app_template/tests.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/conf/app_template/v1/__init__.py-tpl
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/conf/app_template/v1/schemas.py-tpl
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/conf/app_template/v1/urls.py-tpl
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/conf/app_template/v1/views.py-tpl
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/conf/project_template/.gitignore.e-tpl
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/conf/project_template/Makefile.e-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/conf/project_template/project_name/__init__.py-tpl
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/conf/project_template/project_name/main.py-tpl
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/conf/project_template/project_name/serve.py-tpl
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/conf/project_template/project_name/urls.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/conf/project_template/project_name/apps/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/conf/project_template/project_name/configs/__init__.py-tpl
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/conf/project_template/project_name/configs/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/conf/project_template/project_name/configs/development/__init__.py-tpl
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/conf/project_template/project_name/configs/development/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/conf/project_template/project_name/configs/testing/__init__.py-tpl
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/conf/project_template/project_name/configs/testing/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/conf/project_template/project_name/tests/__init__.py-tpl
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/conf/project_template/project_name/tests/test_app.py-tpl
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/config/__init__.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/config/asyncexit.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/config/cors.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/config/csrf.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/config/jwt.py
--rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/config/openapi.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/config/session.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/config/static_files.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/config/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/contrib/__init__.py
--rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/contrib/encoding.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/contrib/auth/__init__.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/contrib/auth/constants.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/contrib/auth/crypto.py
--rw-r--r--   0        0        0     8257 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/contrib/auth/hashers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/contrib/auth/common/__init__.py
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/contrib/auth/common/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/contrib/auth/saffier/__init__.py
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/contrib/auth/saffier/base_user.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/contrib/auth/saffier/middleware.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/contrib/auth/tortoise/__init__.py
--rw-r--r--   0        0        0     4025 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/contrib/auth/tortoise/base_user.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/contrib/auth/tortoise/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/contrib/databases/__init__.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/contrib/databases/tortoise/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/core/__init__.py
--rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/core/management/__init__.py
--rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/core/management/base.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/core/management/exceptions.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/core/management/formatters.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/core/management/parsers.py
--rw-r--r--   0        0        0     6749 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/core/management/templates.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/core/management/typing.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/core/management/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/core/management/directives/__init__.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/core/management/directives/createapp.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/core/management/directives/createproject.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/datastructures/__init__.py
--rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/datastructures/base.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/datastructures/encoders.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/datastructures/file.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/datastructures/json.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/datastructures/redirect.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/datastructures/stream.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/datastructures/template.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/datastructures/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/interceptors/__init__.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/interceptors/interceptor.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/interceptors/types.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/middleware/__init__.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/middleware/asyncexitstack.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/middleware/authentication.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/middleware/basic.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/middleware/cors.py
--rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/middleware/csrf.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/middleware/errors.py
--rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/middleware/exceptions.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/middleware/gzip.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/middleware/https.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/middleware/sessions.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/middleware/settings_middleware.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/middleware/trustedhost.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/middleware/wsgi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/openapi/__init__.py
--rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/openapi/apiview.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/openapi/datastructures.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/openapi/enums.py
--rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/openapi/parameters.py
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/openapi/path_item.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/openapi/request_body.py
--rw-r--r--   0        0        0     8581 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/openapi/responses.py
--rw-r--r--   0        0        0     8811 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/openapi/schema.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/openapi/types.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/openapi/utils.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/permissions/__init__.py
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/permissions/base.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/permissions/types.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/permissions/utils.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/pluggables/__init__.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/pluggables/base.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/protocols/__init__.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/protocols/asyncdao.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/protocols/dao.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/protocols/extension.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/protocols/interceptor.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/protocols/middleware.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/protocols/template.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/responses/__init__.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/responses/base.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/responses/encoders.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/responses/json.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/responses/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/routing/__init__.py
--rw-r--r--   0        0        0    21459 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/routing/base.py
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/routing/events.py
--rw-r--r--   0        0        0     7184 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/routing/gateways.py
--rw-r--r--   0        0        0    23076 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/routing/handlers.py
--rw-r--r--   0        0        0    40820 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/routing/router.py
--rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/routing/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/security/__init__.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/security/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/security/jwt/__init__.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/security/jwt/token.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/template/__init__.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/template/jinja.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/template/mako.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/transformers/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/transformers/constants.py
--rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/transformers/datastructures.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/transformers/helpers.py
--rw-r--r--   0        0        0    14481 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/transformers/model.py
--rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/transformers/signature.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/transformers/types.py
--rw-r--r--   0        0        0     4457 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/transformers/utils.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/urls/__init__.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/urls/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/utils/__init__.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/utils/constants.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/utils/crypto.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/utils/dependency.py
--rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/utils/functional.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/utils/helpers.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/utils/model.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/utils/module_loading.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/utils/pydantic.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/utils/sync.py
--rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/utils/timezone.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 esmerald-1.1.0/esmerald/utils/url.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 esmerald-1.1.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald-1.1.0/LICENSE
--rw-r--r--   0        0        0    15216 2020-02-02 00:00:00.000000 esmerald-1.1.0/README.md
--rw-r--r--   0        0        0     5765 2020-02-02 00:00:00.000000 esmerald-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    21358 2020-02-02 00:00:00.000000 esmerald-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/__init__.py
+-rw-r--r--   0        0        0    32270 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/applications.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/backgound.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/concurrency.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/enums.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/exception_handlers.py
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/exceptions.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/injector.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/logging.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/param_functions.py
+-rw-r--r--   0        0        0    14351 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/params.py
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/parsers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/py.typed
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/requests.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/staticfiles.py
+-rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/testclient.py
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/types.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/typing.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/websockets.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/__init__.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/enums.py
+-rw-r--r--   0        0        0    13177 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/global_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/app_template/__init__.py-tpl
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/app_template/tests.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/app_template/directives/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/app_template/directives/operations/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/app_template/v1/__init__.py-tpl
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/app_template/v1/schemas.py-tpl
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/app_template/v1/urls.py-tpl
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/app_template/v1/views.py-tpl
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/project_template/.gitignore.e-tpl
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/project_template/Makefile.e-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/project_template/project_name/__init__.py-tpl
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/project_template/project_name/main.py-tpl
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/project_template/project_name/serve.py-tpl
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/project_template/project_name/urls.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/project_template/project_name/apps/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/project_template/project_name/configs/__init__.py-tpl
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/project_template/project_name/configs/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/project_template/project_name/configs/development/__init__.py-tpl
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/project_template/project_name/configs/development/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/project_template/project_name/configs/testing/__init__.py-tpl
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/project_template/project_name/configs/testing/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/project_template/project_name/tests/__init__.py-tpl
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/project_template/project_name/tests/test_app.py-tpl
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/config/__init__.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/config/asyncexit.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/config/cors.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/config/csrf.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/config/jwt.py
+-rw-r--r--   0        0        0     6405 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/config/openapi.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/config/session.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/config/static_files.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/config/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/__init__.py
+-rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/encoding.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/auth/__init__.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/auth/constants.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/auth/crypto.py
+-rw-r--r--   0        0        0     8283 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/auth/hashers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/auth/common/__init__.py
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/auth/common/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/auth/saffier/__init__.py
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/auth/saffier/base_user.py
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/auth/saffier/middleware.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/auth/tortoise/__init__.py
+-rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/auth/tortoise/base_user.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/auth/tortoise/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/databases/__init__.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/databases/tortoise/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/__init__.py
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/base.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/cli.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/constants.py
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/env.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/exceptions.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/parsers.py
+-rw-r--r--   0        0        0     6487 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/templates.py
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/utils.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/operations/__init__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/operations/_constants.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/operations/createapp.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/operations/createproject.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/operations/list.py
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/operations/run.py
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/operations/runserver.py
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/operations/show_urls.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/terminal/__init__.py
+-rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/terminal/base.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/terminal/print.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/terminal/terminal.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/datastructures/__init__.py
+-rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/datastructures/base.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/datastructures/encoders.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/datastructures/file.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/datastructures/json.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/datastructures/redirect.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/datastructures/stream.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/datastructures/template.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/datastructures/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/interceptors/__init__.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/interceptors/interceptor.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/interceptors/types.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/middleware/__init__.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/middleware/asyncexitstack.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/middleware/authentication.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/middleware/basic.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/middleware/cors.py
+-rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/middleware/csrf.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/middleware/errors.py
+-rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/middleware/exceptions.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/middleware/gzip.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/middleware/https.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/middleware/sessions.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/middleware/settings_middleware.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/middleware/trustedhost.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/middleware/wsgi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/openapi/__init__.py
+-rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/openapi/apiview.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/openapi/datastructures.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/openapi/enums.py
+-rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/openapi/parameters.py
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/openapi/path_item.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/openapi/request_body.py
+-rw-r--r--   0        0        0     8557 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/openapi/responses.py
+-rw-r--r--   0        0        0     8811 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/openapi/schema.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/openapi/types.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/openapi/utils.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/permissions/__init__.py
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/permissions/base.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/permissions/types.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/permissions/utils.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/pluggables/__init__.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/pluggables/base.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/protocols/__init__.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/protocols/asyncdao.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/protocols/dao.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/protocols/extension.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/protocols/interceptor.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/protocols/middleware.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/protocols/template.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/responses/__init__.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/responses/base.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/responses/encoders.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/responses/json.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/responses/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/routing/__init__.py
+-rw-r--r--   0        0        0    21830 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/routing/base.py
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/routing/events.py
+-rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/routing/gateways.py
+-rw-r--r--   0        0        0    23025 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/routing/handlers.py
+-rw-r--r--   0        0        0    40060 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/routing/router.py
+-rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/routing/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/security/__init__.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/security/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/security/jwt/__init__.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/security/jwt/token.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/template/__init__.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/template/jinja.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/template/mako.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/transformers/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/transformers/constants.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/transformers/datastructures.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/transformers/helpers.py
+-rw-r--r--   0        0        0    14481 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/transformers/model.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/transformers/signature.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/transformers/types.py
+-rw-r--r--   0        0        0     4457 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/transformers/utils.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/urls/__init__.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/urls/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/utils/__init__.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/utils/constants.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/utils/crypto.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/utils/dependency.py
+-rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/utils/functional.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/utils/helpers.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/utils/model.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/utils/module_loading.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/utils/pydantic.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/utils/sync.py
+-rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/utils/timezone.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/utils/url.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 esmerald-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald-1.2.0/LICENSE
+-rw-r--r--   0        0        0    15138 2020-02-02 00:00:00.000000 esmerald-1.2.0/README.md
+-rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 esmerald-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    20137 2020-02-02 00:00:00.000000 esmerald-1.2.0/PKG-INFO
```

### Comparing `esmerald-1.1.0/esmerald/__init__.py` & `esmerald-1.2.0/esmerald/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 Esmerald: Highly scalable, performant, easy to learn and for every application.
 """
-__version__ = "1.1.0"
+__version__ = "1.2.0"
+
+
+from starlette import status
 
 from esmerald.conf import settings
 from esmerald.conf.global_settings import EsmeraldAPISettings
 from esmerald.injector import Inject
-from starlette import status
 
 from .applications import ChildEsmerald, Esmerald
 from .backgound import BackgroundTask, BackgroundTasks
 from .config import CORSConfig, CSRFConfig, OpenAPIConfig, SessionConfig, StaticFilesConfig
 from .datastructures import JSON, Redirect, Stream, Template, UploadFile
 from .exceptions import (
     HTTPException,
```

### Comparing `esmerald-1.1.0/esmerald/applications.py` & `esmerald-1.2.0/esmerald/applications.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,14 @@
     SchedulerType,
     Scope,
     Send,
 )
 from esmerald.utils.helpers import is_class_and_subclass
 
 if TYPE_CHECKING:
-    from openapi_schemas_pydantic.v3_1_0 import SecurityRequirement
-
     from esmerald.types import SettingsType, TemplateConfig
 
 AppType = TypeVar("AppType", bound="Esmerald")
 
 
 class Esmerald(Starlette):
     """
@@ -393,18 +391,18 @@
 
     def activate_scheduler(self):
         """
         Makes sure the scheduler is accessible.
         """
         try:
             from asyncz.contrib.esmerald.scheduler import EsmeraldScheduler
-        except ImportError:
+        except ImportError as e:
             raise ImportError(
                 "The scheduler must be installed. You can do it with `pip install esmerald[schedulers]`"
-            )
+            ) from e
 
         self.scheduler = EsmeraldScheduler(
             app=self,
             scheduler_class=self.scheduler_class,
             tasks=self.scheduler_tasks,
             timezone=self.timezone,
             configurations=self.scheduler_configurations,
```

### Comparing `esmerald-1.1.0/esmerald/backgound.py` & `esmerald-1.2.0/esmerald/backgound.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/enums.py` & `esmerald-1.2.0/esmerald/enums.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/exception_handlers.py` & `esmerald-1.2.0/esmerald/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/exceptions.py` & `esmerald-1.2.0/esmerald/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,18 @@
     ...
 
 
 class AuthenticationError(HTTPException):
     status_code = status.HTTP_401_UNAUTHORIZED
 
 
+class EnvironmentError(EsmeraldAPIException):
+    ...
+
+
 ExceptionErrorMap = Union[
     HTTPException,
     NotAuthenticated,
     PermissionDenied,
     NotAuthorized,
     NotFound,
     MethodNotAllowed,
```

### Comparing `esmerald-1.1.0/esmerald/injector.py` & `esmerald-1.2.0/esmerald/injector.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/logging.py` & `esmerald-1.2.0/esmerald/logging.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/params.py` & `esmerald-1.2.0/esmerald/params.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/parsers.py` & `esmerald-1.2.0/esmerald/parsers.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from contextlib import suppress
+from json import JSONDecodeError, loads
 from typing import TYPE_CHECKING, Any
 
-from json import JSONDecodeError, loads
 from pydantic import BaseConfig, BaseModel
 from pydantic.fields import SHAPE_LIST, SHAPE_SINGLETON
 
 from esmerald.datastructures import UploadFile
 from esmerald.enums import EncodingType
 
 if TYPE_CHECKING:
```

### Comparing `esmerald-1.1.0/esmerald/requests.py` & `esmerald-1.2.0/esmerald/requests.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/testclient.py` & `esmerald-1.2.0/esmerald/testclient.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/types.py` & `esmerald-1.2.0/esmerald/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,30 +9,30 @@
     List,
     Type,
     TypeVar,
     Union,
 )
 
 from starlette.middleware import Middleware as StarletteMiddleware  # noqa
-from starlette.responses import Response as StarletteResponse
-from starlette.types import ASGIApp
+from starlette.responses import Response as StarletteResponse  # noqa
+from starlette.types import ASGIApp  # noqa
 from typing_extensions import Literal
 
 from esmerald.backgound import BackgroundTask, BackgroundTasks
 from esmerald.exceptions import HTTPException, MissingDependency, StarletteHTTPException
 from esmerald.routing.gateways import WebSocketGateway
 from esmerald.routing.router import Include
 
 try:
-    from asyncz.schedulers import AsyncIOScheduler
+    from asyncz.schedulers import AsyncIOScheduler  # noqa
 except ImportError:
     AsyncIOScheduler = Any
 
 try:
-    from esmerald.config.template import TemplateConfig
+    from esmerald.config.template import TemplateConfig as TemplateConfig  # noqa
 except MissingDependency:
     TemplateConfig = Any
 
 if TYPE_CHECKING:
     from esmerald.applications import Esmerald
     from esmerald.conf.global_settings import EsmeraldAPISettings  # noqa
     from esmerald.datastructures import Cookie, ResponseHeader, State  # noqa: TC004
@@ -40,21 +40,19 @@
     from esmerald.protocols.middleware import MiddlewareProtocol
     from esmerald.requests import Request  # noqa
     from esmerald.responses import Response  # noqa
     from esmerald.routing.router import Gateway, HTTPHandler, Router  # noqa
     from esmerald.routing.views import APIView  # noqa
     from esmerald.websockets import WebSocket  # noqa
 else:
-    ASGIApp = Any
     HTTPHandler = Any
     Message = Any
     Receive = Any
     Scope = Any
     Send = Any
-    StarletteMiddleware = Any
     BaseHTTPMiddleware = Any
     Inject = Any
     Request = Any
     WebSocket = Any
     State = Any
     Response = Any
     ResponseHeader = Any
```

### Comparing `esmerald-1.1.0/esmerald/websockets.py` & `esmerald-1.2.0/esmerald/websockets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from typing import Generic, Optional, TypeVar
 
 from starlette.requests import HTTPConnection as HTTPConnection  # noqa: F401
 from starlette.websockets import WebSocket as StarletteWebSocket  # noqa
 from starlette.websockets import WebSocketClose as WebSocketClose  # noqa
-from starlette.websockets import (
-    WebSocketDisconnect as StarletteWebSocketDisconnect,
-)  # noqa
+from starlette.websockets import WebSocketDisconnect as StarletteWebSocketDisconnect  # noqa
 from starlette.websockets import WebSocketState as WebSocketState  # noqa
 
 User = TypeVar("User")
 Auth = TypeVar("Auth")
 
 
 class WebSocket(StarletteWebSocket, Generic[User, Auth]):
```

### Comparing `esmerald-1.1.0/esmerald/conf/__init__.py` & `esmerald-1.2.0/esmerald/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/conf/global_settings.py` & `esmerald-1.2.0/esmerald/conf/global_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,18 +277,18 @@
         Scheduler class to be used within the application.
         """
         if not self.enable_scheduler:
             return None
 
         try:
             from asyncz.schedulers import AsyncIOScheduler
-        except ImportError:
+        except ImportError as e:
             raise ImportError(
                 "The scheduler must be installed. You can do it with `pip install esmerald[schedulers]`"
-            )
+            ) from e
         return AsyncIOScheduler
 
     @property
     def scheduler_tasks(self) -> Dict[str, str]:
         """Returns a dict of tasks for run with `scheduler_class`.
 
         Where the tasks are placed is not linked to the name of
@@ -321,31 +321,31 @@
         Example:
 
             class MySettings(EsmeraldAPISettings):
 
                 @property
                 def scheduler_configurations(self) -> Dict[str, str]:
                     configurations = {
-                        'apscheduler.jobstores.mongo': {
+                        'apscheduler.stores.mongo': {
                             'type': 'mongodb'
                         },
-                        'apscheduler.jobstores.default': {
+                        'apscheduler.stores.default': {
                             'type': 'sqlalchemy',
                             'url': 'sqlite:///jobs.sqlite'
                         },
                         'apscheduler.executors.default': {
                             'class': 'apscheduler.executors.pool:ThreadPoolExecutor',
                             'max_workers': '20'
                         },
                         'apscheduler.executors.processpool': {
                             'type': 'processpool',
                             'max_workers': '5'
                         },
-                        'apscheduler.job_defaults.coalesce': 'false',
-                        'apscheduler.job_defaults.max_instances': '3',
+                        'apscheduler.task_defaults.coalesce': 'false',
+                        'apscheduler.task_defaults.max_instances': '3',
                         'apscheduler.timezone': 'UTC',
                     }
         """
 
         return {}
 
     @property
```

### Comparing `esmerald-1.1.0/esmerald/conf/project_template/.gitignore.e-tpl` & `esmerald-1.2.0/esmerald/conf/project_template/.gitignore.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/conf/project_template/Makefile.e-tpl` & `esmerald-1.2.0/esmerald/conf/project_template/Makefile.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/conf/project_template/project_name/main.py-tpl` & `esmerald-1.2.0/esmerald/conf/project_template/project_name/main.py-tpl`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 """
-Generated by 'esmerald-admin createproject' using Esmerald {{ esmerald_version }}.
+Generated by 'esmerald createproject' using Esmerald {{ esmerald_version }}.
 """
 import os
 import sys
 from pathlib import Path
 
 from esmerald import Esmerald, Include
```

### Comparing `esmerald-1.1.0/esmerald/conf/project_template/project_name/serve.py-tpl` & `esmerald-1.2.0/esmerald/conf/project_template/project_name/serve.py-tpl`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python
 """
-Generated by 'esmerald-admin createproject' using Esmerald {{ esmerald_version }}.
+Generated by 'esmerald createproject' using Esmerald {{ esmerald_version }}.
 
 Esmerald's command-line utility for development purposes.
 """
 import os
 
 import uvicorn
+
 from esmerald.conf import settings
 
 from .main import app as app  # noqa
 
 if __name__ == "__main__":
     """
     Uses the`ESMERALD_SETTINGS_MODULE` settings configuration and loads accordingly.
```

### Comparing `esmerald-1.1.0/esmerald/conf/project_template/project_name/urls.py-tpl` & `esmerald-1.2.0/esmerald/conf/project_template/project_name/urls.py-tpl`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """{{ project_name }} Routes Configuration
 
-Generated by 'esmerald-admin createproject' using Esmerald {{ esmerald_version }}.
+Generated by 'esmerald createproject' using Esmerald {{ esmerald_version }}.
 
 The `route_patterns` list routes URLs to views.
 
 Examples:
     Function views:
         1. Add an import:  from my_app.views import home
         2. Add a URL to route_patterns:  Gateway('/', handler=home, name='home')
```

### Comparing `esmerald-1.1.0/esmerald/conf/project_template/project_name/configs/settings.py-tpl` & `esmerald-1.2.0/esmerald/conf/project_template/project_name/configs/settings.py-tpl`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Esmerald settings for {{ project_name }} project.
 
-Generated by 'esmerald-admin createproject' using Esmerald {{ esmerald_version }}.
+Generated by 'esmerald createproject' using Esmerald {{ esmerald_version }}.
 """
 
 from typing import Optional
 
 from esmerald.conf.enums import EnvironmentType
 from esmerald.conf.global_settings import EsmeraldAPISettings
```

### Comparing `esmerald-1.1.0/esmerald/config/jwt.py` & `esmerald-1.2.0/esmerald/config/jwt.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/config/openapi.py` & `esmerald-1.2.0/esmerald/config/openapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     OpenAPI,
     PathItem,
     Reference,
     SecurityRequirement,
     Server,
     Tag,
 )
-from openapi_schemas_pydantic.v3_1_0.path_item import PathItem
 from pydantic import AnyUrl, BaseModel
 from typing_extensions import Literal
 
 from esmerald.enums import HttpMethod
 from esmerald.openapi.path_item import create_path_item
 from esmerald.routing.gateways import Gateway, WebSocketGateway
 from esmerald.routing.router import Include
```

### Comparing `esmerald-1.1.0/esmerald/config/session.py` & `esmerald-1.2.0/esmerald/config/session.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/config/static_files.py` & `esmerald-1.2.0/esmerald/config/static_files.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/contrib/encoding.py` & `esmerald-1.2.0/esmerald/contrib/encoding.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         return s
     try:
         if isinstance(s, bytes):
             s = str(s, encoding, errors)
         else:
             s = str(s)
     except UnicodeDecodeError as e:
-        raise ExtraUnicodeDecodeError(s, *e.args)
+        raise ExtraUnicodeDecodeError(s, *e.args) from e
     return s
 
 
 def smart_bytes(
     s, encoding: str = "utf-8", strings_only: bool = False, errors: str = "strict"
 ) -> bytes:
     """
```

### Comparing `esmerald-1.1.0/esmerald/contrib/auth/hashers.py` & `esmerald-1.2.0/esmerald/contrib/auth/hashers.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 @functools.lru_cache
 def get_hashers():
     hashers = []
 
     password_hashers = getattr(settings, "password_hashers", None)
     if not password_hashers:
-        warnings.warn("`password_hashers` missing from settings.")
+        warnings.warn("`password_hashers` missing from settings.", stacklevel=2)
         return hashers
 
     for hasher_path in settings.password_hashers:
         hasher_cls = import_string(hasher_path)
         hasher = hasher_cls()
         if not hasher.algorithm:
             raise ImproperlyConfigured(
@@ -137,20 +137,20 @@
     elif algorithm == "default":
         return get_hashers()[0]
 
     else:
         hashers = get_hashers_by_algorithm()
         try:
             return hashers[algorithm]
-        except KeyError:
+        except KeyError as e:
             raise ValueError(
                 "Unknown password hashing algorithm '%s'. "
                 "Did you specify it in your settings? "
                 "setting?" % algorithm
-            )
+            ) from e
 
 
 def identify_hasher(encoded):
     """
     Return an instance of a loaded password hasher.
 
     Identify hasher algorithm by examining encoded hash, and call
```

### Comparing `esmerald-1.1.0/esmerald/contrib/auth/common/middleware.py` & `esmerald-1.2.0/esmerald/contrib/auth/common/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,13 +77,13 @@
             raise NotAuthorized(detail=f"{token_type} is not an authorized header type")
 
         try:
             token = Token.decode(
                 token=auth_token, key=self.config.signing_key, algorithms=[self.config.algorithm]
             )
         except (JWSError, JWTError) as e:
-            raise AuthenticationError(str(e))
+            raise AuthenticationError(str(e)) from e
 
         user = await self.retrieve_user(token.sub)
         if not user:
             raise AuthenticationError("User not found.")
         return AuthResult(user=user)
```

### Comparing `esmerald-1.1.0/esmerald/contrib/auth/saffier/base_user.py` & `esmerald-1.2.0/esmerald/contrib/auth/saffier/base_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import saffier
+
 from esmerald.contrib.auth.hashers import check_password, is_password_usable, make_password
 
 
 class AbstractUser(saffier.Model):
     """
     Base model used for a custom user of any application.
     """
```

### Comparing `esmerald-1.1.0/esmerald/contrib/auth/saffier/middleware.py` & `esmerald-1.2.0/esmerald/contrib/auth/saffier/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Generic, TypeVar
 
+from saffier.exceptions import DoesNotFound
 from starlette.types import ASGIApp
 
 from esmerald.config.jwt import JWTConfig
 from esmerald.contrib.auth.common.middleware import CommonJWTAuthMiddleware
 from esmerald.exceptions import AuthenticationError, NotAuthorized
-from saffier.exceptions import DoesNotFound
 
 T = TypeVar("T")
 
 
 class JWTAuthMiddleware(CommonJWTAuthMiddleware):
     """
     The simple JWT authentication Middleware.
@@ -60,16 +60,16 @@
         """
         Retrieves a user from the database using the given token id.
         """
         try:
             sub = int(token_sub)
             token_sub = sub
         except (TypeError, ValueError):
-            ...
+            ...  # noqa
 
         user_field = {self.config.user_id_field: token_sub}
         try:
             return await self.user_model.query.get(**user_field)
         except DoesNotFound:
-            raise NotAuthorized()
+            raise NotAuthorized() from None
         except Exception as e:
-            raise AuthenticationError(detail=str(e))
+            raise AuthenticationError(detail=str(e)) from e
```

### Comparing `esmerald-1.1.0/esmerald/contrib/auth/tortoise/base_user.py` & `esmerald-1.2.0/esmerald/contrib/auth/tortoise/base_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 from tortoise import fields
 from tortoise.models import Model
 
-from esmerald.contrib.auth.hashers import (
-    check_password,
-    is_password_usable,
-    make_password,
-)
+from esmerald.contrib.auth.hashers import check_password, is_password_usable, make_password
 
 
 class AutoIncrementIntMixin(Model):
     """
     Auto increment for integers.
     """
```

### Comparing `esmerald-1.1.0/esmerald/contrib/auth/tortoise/middleware.py` & `esmerald-1.2.0/esmerald/contrib/auth/tortoise/middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,8 +60,8 @@
         """
         Retrieves a user from the database using the given token id.
         """
         user_field = {self.config.user_id_field: token_sub}
         try:
             return await self.user_model.get(**user_field)
         except DoesNotExist:
-            raise NotAuthorized()
+            raise NotAuthorized() from None
```

### Comparing `esmerald-1.1.0/esmerald/contrib/databases/tortoise/__init__.py` & `esmerald-1.2.0/esmerald/contrib/databases/tortoise/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 Helpers for the TortoiseORM integragion.
 """
 from types import ModuleType
 from typing import Dict, Iterable, List, Optional, Type, Union
 
-from esmerald.conf import settings
 from loguru import logger
 from tortoise import Tortoise
 
+from esmerald.conf import settings
+
 
 async def init_database(
     config: Optional[dict] = None,
     config_file: Optional[str] = None,
     create_db: bool = False,
     db_url: Optional[str] = None,
     modules: Optional[Dict[str, Iterable[Union[str, ModuleType]]]] = None,
```

### Comparing `esmerald-1.1.0/esmerald/core/management/templates.py` & `esmerald-1.2.0/esmerald/core/directives/templates.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""
-Esmerald readapted the same concept to allow a simple integration for the
-`esmerald-admin` allowing the creation of a project and app via command line.
-"""
 import os
 import shutil
 import stat
 from importlib import import_module
+from pathlib import Path
 from typing import Any, Dict, Union
 
 from jinja2 import Environment, FileSystemLoader
-from pydantic import FilePath
 
 import esmerald
-from esmerald.core.management.base import BaseDirective, DirectiveError
+from esmerald.core.directives.base import BaseDirective
+from esmerald.core.directives.exceptions import DirectiveError
+from esmerald.core.terminal import Print
+
+printer = Print()
 
 
 class TemplateDirective(BaseDirective):
     """
     Copy either an Esmerald application layout template or an Esmerald project
     layout.
     """
@@ -24,37 +24,30 @@
     url_schemes = ["http", "https", "ftp"]
 
     rewrite_template_suffixes = (
         (".py-tpl", ".py"),
         (".e-tpl", ""),
     )
 
-    def add_arguments(self, parser: Any):
-        parser.add_argument("name", help="Name of the application or project.")
-
-    def handle(
-        self,
-        app_or_project: str,
-        name: str,
-        **options: Dict[str, Any],
-    ):
+    def handle(self, app_or_project: str, name: str, **options: Any) -> Any:
         self.app_or_project = app_or_project
+        self.name = name
         self.a_or_an = "an" if app_or_project == "app" else "a"
         self.paths_to_remove = []
         self.verbosity = options["verbosity"]
 
         self.validate_name(name)
 
         top_dir = os.path.join(os.getcwd(), name)
         try:
             os.makedirs(top_dir)
         except FileExistsError:
-            raise DirectiveError(f"{top_dir} already exists.")
+            raise DirectiveError(f"{top_dir} already exists.") from None
         except OSError as e:
-            raise DirectiveError(e)
+            raise DirectiveError(e) from e
 
         base_name = f"{app_or_project}_name"
         base_subdir = f"{app_or_project}_template"
 
         context = {
             base_name: name,
             "esmerald_version": self.get_version(),
@@ -83,46 +76,46 @@
                 new_path = os.path.join(top_dir, relative_dir, filename.replace(base_name, name))
                 project_dir = os.path.join(top_dir, relative_dir)
                 template_name = filename
                 for old_suffix, new_suffix in self.rewrite_template_suffixes:
                     if new_path.endswith(old_suffix):
                         new_path = new_path[: -len(old_suffix)] + new_suffix
                         template_name = template_name[: -len(old_suffix)] + new_suffix
-                        break  # Only rewrite once
+                        break
 
                 if os.path.exists(new_path):
                     raise DirectiveError(
                         "%s already exists. Overlaying %s %s into an existing "
                         "directory won't replace conflicting files."
                         % (
                             new_path,
                             self.a_or_an,
                             app_or_project,
                         )
                     )
+
                 shutil.copyfile(old_path, new_path)
                 if self.verbosity >= 2:
-                    self.stdout.write("Creating %s" % new_path)
+                    printer.write_info("Creating %s" % new_path)
                 try:
                     self.manage_template_variables(template_name, new_path, project_dir, context)
                     self.apply_umask(old_path, new_path)
                     self.make_file_writable(new_path)
                 except OSError:
-                    self.stderr.write(
+                    printer.write_error(
                         "Notice: Couldn't set permission bits on %s. You're "
                         "probably using an uncommon filesystem setup. No "
                         "problem." % new_path,
-                        self.style.NOTICE,
                     )
 
     def manage_template_variables(
         self,
-        template: Union[str, FilePath],
-        destination: Union[str, FilePath],
-        template_dir: Union[str, FilePath],
+        template: Union[str, Path],
+        destination: Union[str, Path],
+        template_dir: Union[str, Path],
         context: Dict[str, Any],
     ):
         """
         Goes through every file generated and replaces the variables with the given
         context variables.
         """
         environment = Environment(loader=FileSystemLoader(template_dir), autoescape=True)
@@ -163,15 +156,15 @@
                     name=name,
                     an=self.a_or_an,
                     app=self.app_or_project,
                     type=name_or_dir,
                 )
             )
 
-    def apply_umask(self, old_path: Union[str, FilePath], new_path: Union[str, FilePath]):
+    def apply_umask(self, old_path: Union[str, Path], new_path: Union[str, Path]):
         current_umask = os.umask(0)
         os.umask(current_umask)
         current_mode = stat.S_IMODE(os.stat(old_path).st_mode)
         os.chmod(new_path, current_mode & ~current_umask)
 
     def make_file_writable(self, filename: str):
         """
```

### Comparing `esmerald-1.1.0/esmerald/datastructures/__init__.py` & `esmerald-1.2.0/esmerald/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/datastructures/base.py` & `esmerald-1.2.0/esmerald/datastructures/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/datastructures/encoders.py` & `esmerald-1.2.0/esmerald/datastructures/encoders.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/datastructures/file.py` & `esmerald-1.2.0/esmerald/datastructures/file.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/datastructures/json.py` & `esmerald-1.2.0/esmerald/datastructures/json.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/datastructures/redirect.py` & `esmerald-1.2.0/esmerald/datastructures/redirect.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/datastructures/stream.py` & `esmerald-1.2.0/esmerald/datastructures/stream.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/datastructures/template.py` & `esmerald-1.2.0/esmerald/datastructures/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/interceptors/interceptor.py` & `esmerald-1.2.0/esmerald/interceptors/interceptor.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/middleware/__init__.py` & `esmerald-1.2.0/esmerald/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/middleware/asyncexitstack.py` & `esmerald-1.2.0/esmerald/middleware/asyncexitstack.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/middleware/authentication.py` & `esmerald-1.2.0/esmerald/middleware/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Any
 
-from esmerald.enums import ScopeType
-from esmerald.protocols.middleware import MiddlewareProtocol
 from pydantic import BaseConfig, BaseModel
 from starlette.requests import HTTPConnection
 
+from esmerald.enums import ScopeType
+from esmerald.protocols.middleware import MiddlewareProtocol
+
 if TYPE_CHECKING:
     from starlette.types import ASGIApp, Receive, Scope, Send
 
 
 class AuthResult(BaseModel):
     user: Any
```

### Comparing `esmerald-1.1.0/esmerald/middleware/basic.py` & `esmerald-1.2.0/esmerald/middleware/basic.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from starlette.middleware.base import BaseHTTPMiddleware  # noqa
-from starlette.middleware.base import (
-    RequestResponseEndpoint as RequestResponseEndpoint,
-)  # noqa
+from starlette.middleware.base import RequestResponseEndpoint as RequestResponseEndpoint  # noqa
 
 from esmerald.requests import Request
 from esmerald.responses import Response
 
 
 class BasicHTTPMiddleware(BaseHTTPMiddleware):
     """
```

### Comparing `esmerald-1.1.0/esmerald/middleware/csrf.py` & `esmerald-1.2.0/esmerald/middleware/csrf.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,25 +22,27 @@
 SOFTWARE.
 """
 import hashlib
 import hmac
 import secrets
 from typing import TYPE_CHECKING, Optional
 
+from starlette.datastructures import MutableHeaders
+
 from esmerald.datastructures import Cookie
 from esmerald.enums import ScopeType
 from esmerald.exceptions import PermissionDenied
 from esmerald.protocols.middleware import MiddlewareProtocol
 from esmerald.requests import Request
-from starlette.datastructures import MutableHeaders
 
 if TYPE_CHECKING:
-    from esmerald.config import CSRFConfig
     from starlette.types import ASGIApp, Message, Receive, Scope, Send
 
+    from esmerald.config import CSRFConfig
+
 CSRF_SECRET_BYTES = 32
 CSRF_SECRET_LENGTH = CSRF_SECRET_BYTES * 2
 
 
 class CSRFMiddleware(MiddlewareProtocol):
     def __init__(
         self,
```

### Comparing `esmerald-1.1.0/esmerald/middleware/errors.py` & `esmerald-1.2.0/esmerald/middleware/errors.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import traceback
 
-from starlette.middleware.errors import (
-    ServerErrorMiddleware as StarletteServerErrorMiddleware,
-)
+from starlette.middleware.errors import ServerErrorMiddleware as StarletteServerErrorMiddleware
 from starlette.responses import HTMLResponse, PlainTextResponse, Response
 
 from esmerald.requests import Request
 
 
 class ServerErrorMiddleware(StarletteServerErrorMiddleware):
     """
```

### Comparing `esmerald-1.1.0/esmerald/middleware/exceptions.py` & `esmerald-1.2.0/esmerald/middleware/exceptions.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/middleware/settings_middleware.py` & `esmerald-1.2.0/esmerald/middleware/settings_middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/openapi/apiview.py` & `esmerald-1.2.0/esmerald/openapi/apiview.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/openapi/enums.py` & `esmerald-1.2.0/esmerald/openapi/enums.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/openapi/parameters.py` & `esmerald-1.2.0/esmerald/openapi/parameters.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/openapi/path_item.py` & `esmerald-1.2.0/esmerald/openapi/path_item.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/openapi/request_body.py` & `esmerald-1.2.0/esmerald/openapi/request_body.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import TYPE_CHECKING, Optional
 
-from esmerald.enums import EncodingType
-from esmerald.openapi.schema import create_schema, update_schema_field_info
 from openapi_schemas_pydantic.v3_1_0.media_type import MediaType as OpenAPIMediaType
 from openapi_schemas_pydantic.v3_1_0.request_body import RequestBody
 
+from esmerald.enums import EncodingType
+from esmerald.openapi.schema import create_schema, update_schema_field_info
+
 if TYPE_CHECKING:
     from pydantic.fields import ModelField
 
 
 def create_request_body(field: "ModelField", create_examples: bool) -> Optional[RequestBody]:
     """
     Gets the request body of the handler.
```

### Comparing `esmerald-1.1.0/esmerald/openapi/responses.py` & `esmerald-1.2.0/esmerald/openapi/responses.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 from http import HTTPStatus
 from inspect import Signature
 from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Optional, Tuple, Type, cast
 
+from openapi_schemas_pydantic.v3_1_0 import Response
+from openapi_schemas_pydantic.v3_1_0.header import Header
+from openapi_schemas_pydantic.v3_1_0.media_type import MediaType as OpenAPISchemaMediaType
+from openapi_schemas_pydantic.v3_1_0.schema import Schema
+from starlette.routing import get_name
+from typing_extensions import get_args, get_origin
+
 from esmerald.datastructures import File, Redirect, Stream, Template
 from esmerald.enums import MediaType
-from esmerald.exceptions import (
-    HTTPException,
-    ImproperlyConfigured,
-    ValidationErrorException,
-)
+from esmerald.exceptions import HTTPException, ImproperlyConfigured, ValidationErrorException
 from esmerald.openapi.enums import OpenAPIFormat, OpenAPIType
 from esmerald.openapi.schema import create_schema
 from esmerald.openapi.utils import pascal_case_to_text
 from esmerald.responses import Response as EsmeraldResponse
 from esmerald.utils.model import create_parsed_model_field
-from openapi_schemas_pydantic.v3_1_0 import Response
-from openapi_schemas_pydantic.v3_1_0.header import Header
-from openapi_schemas_pydantic.v3_1_0.media_type import (
-    MediaType as OpenAPISchemaMediaType,
-)
-from openapi_schemas_pydantic.v3_1_0.schema import Schema
-from starlette.routing import get_name
-from typing_extensions import get_args, get_origin
 
 if TYPE_CHECKING:
+    from openapi_schemas_pydantic.v3_1_0.responses import Responses
+
     from esmerald.datastructures import Cookie
     from esmerald.routing.router import HTTPHandler
     from esmerald.types import AnyCallable
-    from openapi_schemas_pydantic.v3_1_0.responses import Responses
 
 
 def create_cookie_schema(cookie: "Cookie") -> Schema:
     cookie_copy = cookie.copy(update={"value": "<string>"})
     value = cookie_copy.to_header(header="")
     return Schema(description=cookie.description or "", example=value)
```

### Comparing `esmerald-1.1.0/esmerald/openapi/schema.py` & `esmerald-1.2.0/esmerald/openapi/schema.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/openapi/utils.py` & `esmerald-1.2.0/esmerald/openapi/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 from typing import TYPE_CHECKING
 
-from esmerald.exceptions import ImproperlyConfigured
 from openapi_schemas_pydantic.utils.constants import PYDANTIC_FIELD_SHAPE_MAP
 
+from esmerald.exceptions import ImproperlyConfigured
+
 if TYPE_CHECKING:
     from openapi_schemas_pydantic.utils.enums import OpenAPIType
     from pydantic.fields import ModelField
 
 CAPITAL_LETTERS_PATTERN = re.compile(r"(?=[A-Z])")
```

### Comparing `esmerald-1.1.0/esmerald/permissions/base.py` & `esmerald-1.2.0/esmerald/permissions/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/permissions/utils.py` & `esmerald-1.2.0/esmerald/permissions/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/pluggables/base.py` & `esmerald-1.2.0/esmerald/pluggables/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/protocols/asyncdao.py` & `esmerald-1.2.0/esmerald/protocols/asyncdao.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/protocols/dao.py` & `esmerald-1.2.0/esmerald/protocols/dao.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/protocols/interceptor.py` & `esmerald-1.2.0/esmerald/protocols/interceptor.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/protocols/template.py` & `esmerald-1.2.0/esmerald/protocols/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/responses/base.py` & `esmerald-1.2.0/esmerald/responses/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/responses/encoders.py` & `esmerald-1.2.0/esmerald/responses/encoders.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/responses/json.py` & `esmerald-1.2.0/esmerald/responses/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any, Dict
 
 from orjson import OPT_OMIT_MICROSECONDS  # noqa
 from pydantic import BaseModel
+
 from esmerald.responses import JSONResponse as JSONResponse  # noqa
 
 try:
     import orjson
 except ImportError:  # pragma: nocover
     orjson = None  # type: ignore
```

### Comparing `esmerald-1.1.0/esmerald/responses/template.py` & `esmerald-1.2.0/esmerald/responses/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/routing/base.py` & `esmerald-1.2.0/esmerald/routing/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     Union,
     cast,
 )
 from uuid import UUID
 
 from starlette.convertors import CONVERTOR_TYPES
 from starlette.requests import HTTPConnection
-from starlette.responses import JSONResponse
 from starlette.responses import Response as StarletteResponse
 from starlette.routing import Mount as Mount  # noqa
 from starlette.routing import compile_path
 from starlette.types import Receive, Scope, Send
 from typing_extensions import TypedDict
 
 from esmerald.backgound import BackgroundTask, BackgroundTasks
@@ -452,14 +451,25 @@
         only used for OpenAPI documentation purposes only.
         """
         path_components = self.parse_path(self.path)
         parameters = [component for component in path_components if isinstance(component, dict)]
         return parameters
 
     @property
+    def stringify_parameters(self) -> List[Dict[str, str]]:
+        """
+        Gets the param:type in string like list.
+        """
+        path_components = self.parse_path(self.path)
+        parameters = [component for component in path_components if isinstance(component, dict)]
+
+        parameters = [f"{param['name']}:{param['type'].__name__}" for param in parameters]
+        return parameters
+
+    @property
     def parent_levels(self) -> List[Union[T, "ParentType"]]:
         """
         Returns the handler from the app down to the route handler.
 
         Who is the parent of a given layer/level.
 
         Example:
```

### Comparing `esmerald-1.1.0/esmerald/routing/events.py` & `esmerald-1.2.0/esmerald/routing/events.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from typing import TYPE_CHECKING, List, Optional, TypeVar
+from typing import TYPE_CHECKING, Any, Callable, List, Optional, Sequence, TypeVar
 
 from starlette._utils import is_async_callable
-from starlette.types import Receive, Scope, Send
+from starlette.types import Lifespan, Receive, Scope, Send
 
 if TYPE_CHECKING:
     from esmerald.types import DictAny, LifeSpanHandler
 
 
 _T = TypeVar("_T")
 
@@ -46,7 +46,24 @@
     async def __aexit__(self, scope: Scope, receive: Receive, send: Send, **kwargs: "DictAny"):
         """Runs the functions on shutdown"""
         for handler in self.on_shutdown:
             if is_async_callable(handler):
                 await handler()
             else:
                 handler()
+
+
+def handle_lifespan_events(
+    on_startup: Optional[Sequence[Callable]] = None,
+    on_shutdown: Optional[Sequence[Callable]] = None,
+    lifespan: Optional[Lifespan[Any]] = None,
+) -> Any:
+    """Handles with the lifespan events in the new Starlette format of lifespan.
+    This adds a mask that keeps the old `on_startup` and `on_shutdown` events variable
+    declaration for legacy and comprehension purposes and build the async context manager
+    for the lifespan.
+    """
+    if on_startup or on_shutdown:
+        return AyncLifespanContextManager(on_startup=on_startup, on_shutdown=on_shutdown)
+    elif lifespan:
+        return lifespan
+    return None
```

### Comparing `esmerald-1.1.0/esmerald/routing/gateways.py` & `esmerald-1.2.0/esmerald/routing/gateways.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from esmerald.utils.helpers import clean_string, is_class_and_subclass
 from esmerald.utils.url import clean_path
 
 if TYPE_CHECKING:
     from esmerald.interceptors.types import Interceptor
     from esmerald.permissions.types import Permission
     from esmerald.routing.router import HTTPHandler, WebSocketHandler
-    from esmerald.routing.views import APIView
     from esmerald.types import Dependencies, ExceptionHandlers, Middleware, ParentType
 
 
 class Gateway(StarletteRoute, BaseInterceptorMixin):
     __slots__ = (
         "_interceptors",
         "path",
```

### Comparing `esmerald-1.1.0/esmerald/routing/handlers.py` & `esmerald-1.2.0/esmerald/routing/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,14 @@
     ResponseType,
 )
 from esmerald.utils.constants import AVAILABLE_METHODS
 
 if TYPE_CHECKING:
     from openapi_schemas_pydantic.v3_1_0 import SecurityRequirement
 
-    from esmerald.exceptions import HTTPException
-
 
 SUCCESSFUL_RESPONSE = "Successful response"
 
 
 class get(HTTPHandler):
     def __init__(
         self,
```

### Comparing `esmerald-1.1.0/esmerald/routing/router.py` & `esmerald-1.2.0/esmerald/routing/router.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     Any,
     Awaitable,
     Callable,
     Dict,
     List,
     NoReturn,
     Optional,
-    Sequence,
     Set,
     Tuple,
     Type,
     Union,
     cast,
 )
 
@@ -43,15 +42,15 @@
 )
 from esmerald.injector import Inject
 from esmerald.interceptors.types import Interceptor
 from esmerald.openapi.datastructures import ResponseSpecification
 from esmerald.requests import Request
 from esmerald.responses import Response
 from esmerald.routing.base import BaseHandlerMixin
-from esmerald.routing.events import AyncLifespanContextManager
+from esmerald.routing.events import handle_lifespan_events
 from esmerald.routing.gateways import Gateway, WebSocketGateway
 from esmerald.routing.views import APIView
 from esmerald.transformers.datastructures import EsmeraldSignature as SignatureModel
 from esmerald.transformers.model import TransformerModel
 from esmerald.transformers.utils import get_signature
 from esmerald.typing import Void, VoidType
 from esmerald.urls import include
@@ -233,15 +232,15 @@
                 raise ImproperlyConfigured(f"The route {route} must be of type Gateway or Include")
         routes = routes or []
 
         assert lifespan is None or (
             on_startup is None and on_shutdown is None
         ), "Use either 'lifespan' or 'on_startup'/'on_shutdown', not both."
 
-        self.esmerald_lifespan = self.handle_lifespan_events(
+        self.esmerald_lifespan = handle_lifespan_events(
             on_startup=on_startup, on_shutdown=on_shutdown, lifespan=lifespan
         )
 
         super().__init__(
             redirect_slashes=redirect_slashes,
             routes=routes,
             default=default,
@@ -277,31 +276,14 @@
     def reorder_routes(self):
         return sorted(
             self.routes,
             key=lambda router: router.path != "" and router.path != "/",
             reverse=True,
         )
 
-    def handle_lifespan_events(
-        self,
-        on_startup: Optional[Sequence[Callable]] = None,
-        on_shutdown: Optional[Sequence[Callable]] = None,
-        lifespan: Optional[Lifespan[Any]] = None,
-    ) -> Any:
-        """Handles with the lifespan events in the new Starlette format of lifespan.
-        This adds a mask that keeps the old `on_startup` and `on_shutdown` events variable
-        declaration for legacy and comprehension purposes and build the async context manager
-        for the lifespan.
-        """
-        if on_startup or on_shutdown:
-            return AyncLifespanContextManager(on_startup=on_startup, on_shutdown=on_shutdown)
-        elif lifespan:
-            return lifespan
-        return None
-
     def activate(self):
         self.routes = self.reorder_routes()
 
     def add_apiview(self, value: Type["APIView"]):
         routes = []
         if not value.handler.parent:
             value(parent=self)
```

### Comparing `esmerald-1.1.0/esmerald/routing/views.py` & `esmerald-1.2.0/esmerald/routing/views.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/security/jwt/token.py` & `esmerald-1.2.0/esmerald/security/jwt/token.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/template/jinja.py` & `esmerald-1.2.0/esmerald/template/jinja.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/template/mako.py` & `esmerald-1.2.0/esmerald/template/mako.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/transformers/datastructures.py` & `esmerald-1.2.0/esmerald/transformers/datastructures.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,25 +3,22 @@
 A lot of great work was done using the Signature and Esmerald is no exception.
 """
 
 from inspect import Parameter as InspectParameter
 from inspect import Signature
 from typing import TYPE_CHECKING, Any, ClassVar, Optional, Set, Union
 
-from esmerald.exceptions import (
-    ImproperlyConfigured,
-    InternalServerError,
-    ValidationErrorException,
-)
+from pydantic import BaseModel, ValidationError
+
+from esmerald.exceptions import ImproperlyConfigured, InternalServerError, ValidationErrorException
 from esmerald.requests import Request
 from esmerald.transformers.constants import UNDEFINED
 from esmerald.transformers.utils import get_connection_info
 from esmerald.utils.helpers import is_optional_union
 from esmerald.websockets import WebSocket
-from pydantic import BaseModel, ValidationError
 
 if TYPE_CHECKING:
     from pydantic.error_wrappers import ErrorDict
     from pydantic.typing import DictAny
 
 IntValError = Union[InternalServerError, ValidationError]
```

### Comparing `esmerald-1.1.0/esmerald/transformers/helpers.py` & `esmerald-1.2.0/esmerald/transformers/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import inspect
 from typing import Any
 
-from esmerald.transformers.types import ConstrainedField
 from pydantic import (
     ConstrainedBytes,
     ConstrainedDate,
     ConstrainedDecimal,
     ConstrainedFloat,
     ConstrainedFrozenSet,
     ConstrainedInt,
     ConstrainedList,
     ConstrainedSet,
     ConstrainedStr,
 )
 
+from esmerald.transformers.types import ConstrainedField
+
 
 def is_pydantic_constrained_field(value: Any) -> ConstrainedField:
     return inspect.isclass(value) and any(
         issubclass(value, _type)
         for _type in (
             ConstrainedBytes,
             ConstrainedDate,
```

### Comparing `esmerald-1.1.0/esmerald/transformers/model.py` & `esmerald-1.2.0/esmerald/transformers/model.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/transformers/signature.py` & `esmerald-1.2.0/esmerald/transformers/signature.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Signature is widely used by Pydantic and comes from the inpect library.
 A lot of great work was done using the Signature and Esmerald is no exception.
 """
 
-from inspect import Parameter
 from inspect import Signature as InspectSignature
 from typing import TYPE_CHECKING, Any, Generator, Set, Type
 
 from pydantic import create_model
 from pydantic.fields import Undefined
 
 from esmerald.exceptions import ImproperlyConfigured
@@ -33,33 +32,33 @@
         self.fn = fn
         self.signature = InspectSignature.from_callable(self.fn)
         self.fn_name = fn.__name__ if hasattr(fn, "__name__") else "anonymous"
         self.defaults = {}
         self.dependency_names = dependency_names
         self.field_definitions = {}
 
-    def validate_missing_dependency(self, param: Parameter) -> None:
+    def validate_missing_dependency(self, param: Any) -> None:
         if param.optional:
             return
         if not is_dependency_field(param.default):
             return
         field = param.default
         if field.default is not Undefined:
             return
         if param.name not in self.dependency_names:
             raise ImproperlyConfigured(
                 f"Explicit dependency '{param.name}' for '{self.fn_name}' has no default value, "
                 f"or provided dependency."
             )
 
-    def get_dependency_names(self, param: Parameter) -> None:
+    def get_dependency_names(self, param: Any) -> None:
         if is_dependency_field(param.default):
             self.dependency_names.add(param.name)
 
-    def set_default_field(self, param: Parameter) -> None:
+    def set_default_field(self, param: Any) -> None:
         if param.default_defined:
             self.defaults[param.name] = param.default
 
     @property
     def parameters(self) -> Generator[Parameter, None, None]:
         for name, param in self.signature.parameters.items():
             if name in CLASS_SPECIAL_WORDS:
```

### Comparing `esmerald-1.1.0/esmerald/transformers/types.py` & `esmerald-1.2.0/esmerald/transformers/types.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/transformers/utils.py` & `esmerald-1.2.0/esmerald/transformers/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/urls/base.py` & `esmerald-1.2.0/esmerald/urls/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/utils/constants.py` & `esmerald-1.2.0/esmerald/utils/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from esmerald.enums import HttpMethod
 from starlette import status
 
+from esmerald.enums import HttpMethod
+
 RESERVED_KWARGS = {"state", "headers", "cookies", "request", "socket", "data", "query"}
 REQUIRED = "required"
 IS_DEPENDENCY = "is_dependency"
 SKIP_VALIDATION = "skip_validation"
 
 REDIRECT_STATUS_CODES = {
     status.HTTP_301_MOVED_PERMANENTLY,
```

### Comparing `esmerald-1.1.0/esmerald/utils/crypto.py` & `esmerald-1.2.0/esmerald/utils/crypto.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,16 @@
     random = random.SystemRandom()
     using_sysrandom = True
 except NotImplementedError:
     import warnings
 
     warnings.warn(
         "A secure pseudo-random number generator is not available "
-        "on your system. Falling back to Mersenne Twister."
+        "on your system. Falling back to Mersenne Twister.",
+        stacklevel=2,
     )
     using_sysrandom = False
 
 
 def get_random_string(
     length: int = 12,
     allowed_chars: str = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789",
```

### Comparing `esmerald-1.1.0/esmerald/utils/functional.py` & `esmerald-1.2.0/esmerald/utils/functional.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/utils/helpers.py` & `esmerald-1.2.0/esmerald/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/utils/model.py` & `esmerald-1.2.0/esmerald/utils/model.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/utils/module_loading.py` & `esmerald-1.2.0/esmerald/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/utils/pydantic.py` & `esmerald-1.2.0/esmerald/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/esmerald/utils/timezone.py` & `esmerald-1.2.0/esmerald/utils/timezone.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 """
 Timezone-related classes and functions.
 """
 import functools
 import sys
+import zoneinfo
+from datetime import date, datetime, timedelta, timezone
 from typing import Any, Optional, Union
 from zoneinfo import ZoneInfo
 
-try:
-    import zoneinfo
-except ImportError:
-    from backports import zoneinfo
-
-from datetime import date, datetime, timedelta, timezone
-
 from asgiref.local import Local
+
 from esmerald.conf import settings
 
 __all__ = [
-    "utc",
     "get_fixed_timezone",
     "get_default_timezone",
     "get_default_timezone_name",
     "get_current_timezone",
     "get_current_timezone_name",
     "localtime",
     "localdate",
```

### Comparing `esmerald-1.1.0/LICENSE` & `esmerald-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esmerald-1.1.0/README.md` & `esmerald-1.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -97,32 +97,26 @@
 
 **Support for ORJSON and UJSON**:
 
 ```shell
 pip install esmerald[encoders]
 ```
 
-**All the esmerald features**:
-
-```shell
-pip install esmerald[all]
-```
-
 **If you want to use the esmerald testing client**:
 
 ```shell
 pip install esmerald[test]
 ```
 
 ### Start a project using directives
 
 If you wish to start an Esmerald project with a default suggested structure.
 
 ```
-esmerald-admin createproject <YOUR-PROJECT-NAME>
+esmerald createproject <YOUR-PROJECT-NAME>
 ```
 
 This will generate a scaffold for your project with some pre-defined files in a simple fashion.
 This will also generate a file for the tests using the EsmeraldTestClient, so make sure you run:
 
 ```shell
 pip install esmerald[test]
```

#### html2text {}

```diff
@@ -28,20 +28,19 @@
 ASGI server is also needed to run in production, we recommend [Uvicorn](https:/
 /www.uvicorn.org) but it is entirely up to you. ```shell pip install uvicorn
 ``` If you want install esmerald with specifics: **Support for template system
 such as jinja2 and mako**: ```shell pip install esmerald[templates] ```
 **Support for the internal scheduler**: ```shell pip install esmerald
 [schedulers] ``` **Support for the jwt used internally by Esmerald**: ```shell
 pip install esmerald[jwt] ``` **Support for ORJSON and UJSON**: ```shell pip
-install esmerald[encoders] ``` **All the esmerald features**: ```shell pip
-install esmerald[all] ``` **If you want to use the esmerald testing client**:
-```shell pip install esmerald[test] ``` ### Start a project using directives If
-you wish to start an Esmerald project with a default suggested structure. ```
-esmerald-admin createproject  ``` This will generate a scaffold for your
-project with some pre-defined files in a simple fashion. This will also
+install esmerald[encoders] ``` **If you want to use the esmerald testing
+client**: ```shell pip install esmerald[test] ``` ### Start a project using
+directives If you wish to start an Esmerald project with a default suggested
+structure. ``` esmerald createproject  ``` This will generate a scaffold for
+your project with some pre-defined files in a simple fashion. This will also
 generate a file for the tests using the EsmeraldTestClient, so make sure you
 run: ```shell pip install esmerald[test] ``` Or you can jump this step if you
 don't want to use the EsmeraldTestClient. You can find [more information]
 (https://esmerald.dymmond.com/management/directives) about this directive and
 how to use it. ## Key Features * **Fluid and Fast**: Thanks to Starlette and
 Pydantic. * **Fast to develop**: Thanks to the simplicity of design, the
 development times can be reduced exponentially. * **Intuitive**: If you are
```

### Comparing `esmerald-1.1.0/pyproject.toml` & `esmerald-1.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -35,23 +35,26 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 dependencies = [
     "a2wsgi>=1.7.0,<2",
-    "aiofiles>=0.8.0,<23",
+    "aiofiles>=0.8.0,<24",
+    "anyio>=3.6.2,<4.0.0",
     "awesome-slugify>=1.6.5,<2",
-    "httpx>=0.23.3,<0.30.0",
+    "httpx>=0.24.0,<0.30.0",
     "itsdangerous>=2.1.2,<3.0.0",
     "jsonschema_rs>=0.16.2,<0.20.0",
     "loguru>=0.6.0,<0.7.0",
-    "pydantic>=1.10.5,<2.0.0",
+    "pydantic>=1.10.7,<2.0.0",
     "pydantic-factories==1.17.2",
+    "python-multipart>=0.0.5,<0.0.7",
     "openapi-schemas-pydantic>=1.1.0",
+    "rich>=13.3.1,<14.0.0",
     "starlette>=0.26.1,<0.27.0",
 ]
 keywords = [
     "api",
     "rest",
     "http",
     "asgi",
@@ -73,52 +76,46 @@
 Source = "https://github.com/dymmond/esmerald"
 
 [project.optional-dependencies]
 test = [
     "pytest>=7.1.3,<8.0.0",
     "pytest-cov>=2.12.0,<5.0.0",
     "pytest-asyncio>=0.19.0",
-    "mypy==1.0.1",
+    "mypy==1.1.1",
     "flake8>=5.0.4",
-    "black== 23.1.0",
+    "black== 23.3.0",
     "isort>=5.0.6,<6.0.0",
-    "aiofiles>=0.8.0,<23",
-    "a2wsgi>=1.6.0,<2",
+    "aiofiles>=0.8.0,<24",
+    "a2wsgi>=1.7.0,<2",
     "asyncz>=0.2.0",
-    "awesome-slugify>=1.6.5,<2",
-    "anyio[trio]>=3.2.1,<4.0.0",
+    "anyio[trio]>=3.6.2,<4.0.0",
     "asyncio[trio]>=3.4.3,<4.0.0",
     "brotli>=1.0.9,<2.0.0",
     "jinja2>=3.1.2,<4.0.0",
-    "jsonschema_rs>=0.16.2,<0.20.0",
     "flask>=1.1.2,<3.0.0",
     "freezegun>=1.2.2,<2.0.0",
-    "httpx>=0.23.3,<0.24.0",
     "mock==5.0.1",
     "passlib==1.7.4",
-    "pydantic>=1.10.5,<2.0.0",
-    "pydantic-factories==1.17.2",
     "python-jose>=3.3.0,<4",
     "orjson>=3.8.5,<4.0.0",
-    "saffier[postgres]>=0.4.0",
+    "saffier[postgres]>=0.6.1",
     "requests>=2.28.2,<3.0.0",
     "ruff>=0.0.256,<1.0.0",
     "ujson>=5.7.0,<6",
 
     # types
     "types-ujson==5.7.0.1",
     "types-orjson==3.6.2",
 ]
 
 dev = [
     "autoflake>=1.4.0",
     "flake8>=3.8.3,<6.0.0",
     "uvicorn[standard]>=0.19.0",
-    "pre-commit>=2.17.0,<4.0.0",
-    "loguru>=0.6.0,<0.7.0",
+    "pre-commit>=3.0.4,<4.0.0",
     "watchfiles>=0.16.1,<0.20.0",
 ]
 
 doc = [
     "mkautodoc>=0.2.0,<0.3.0",
     "mkdocs>=1.1.2,<2.0.0",
     "mkdocs-material>=9.0.13,<10.0.0",
@@ -132,52 +129,38 @@
 
 jwt = ["passlib==1.7.4", "python-jose>=3.3.0,<4"]
 
 encoders = ["orjson>=3.8.5,<4.0.0", "ujson>=5.7.0,<6"]
 
 schedulers = ["asyncz>=0.2.0"]
 
-all = [
-    "a2wsgi>=1.6.0,<2",
-    "aiofiles>=0.8.0,<23",
-    "asyncz>=0.2.0",
-    "awesome-slugify>=1.6.5,<2",
-    "httpx>=0.23.3,<0.30.0",
-    "jsonschema_rs>=0.16.2,<0.20.0",
-    "jinja2>=3.1.2,<4.0.0",
-    "loguru>=0.6.0,<0.7.0",
-    "mako==1.2.4",
-    "passlib==1.7.4",
-    "pydantic>=1.10.5,<2.0.0",
-    "pydantic-factories==1.17.2",
-    "python-jose>=3.3.0,<4",
-    "openapi-schemas-pydantic>=1.1.0",
-    "orjson>=3.8.5,<4.0.0",
-    "python-multipart>=0.0.5,<0.0.6",
-    "ujson>=5.7.0,<6",
-]
-
 [tool.hatch.version]
 path = "esmerald/__init__.py"
 
 [project.scripts]
-esmerald-admin = "esmerald.core.management:run_from_command_line"
+esmerald = "esmerald.core.directives.cli:esmerald_cli"
 
 [tool.isort]
 profile = "black"
 known_third_party = ["esmerald", "pydantic", "starlette"]
 
 [tool.mypy]
+warn_unused_configs = true
+warn_unreachable = true
+warn_return_any = true
 strict = true
-disallow_any_generics = false
 disallow_untyped_decorators = true
-implicit_reexport = true
+disallow_any_generics = false
+implicit_reexport = false
+show_error_codes = true
 disallow_incomplete_defs = true
 disable_error_code = "attr-defined"
 exclude = "esmerald/conf,esmerald/utils"
+warn_unused_ignores = true
+warn_redundant_casts = true
 
 [tool.ruff]
 select = [
     "E", # pycodestyle errors
     "W", # pycodestyle warnings
     "F", # pyflakes
     "C", # flake8-comprehensions
@@ -185,14 +168,16 @@
 ]
 ignore = [
     "E501", # line too long, handled by black
     "B008", # do not perform function calls in argument defaults
     "C901", # too complex
 ]
 
+exclude = ["docs_src/*"]
+
 [[tool.mypy.overrides]]
 module = "esmerald.tests.*"
 ignore_missing_imports = true
 check_untyped_defs = true
 ignore_errors = true
 
 [[tool.mypy.overrides]]
```

### Comparing `esmerald-1.1.0/PKG-INFO` & `esmerald-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esmerald
-Version: 1.1.0
+Version: 1.2.0
 Summary: Highly scalable, performant, easy to learn, easy to code and for every application.
 Project-URL: Homepage, https://github.com/dymmond/esmerald
 Project-URL: Documentation, https://esmerald.dymmond.com/
 Project-URL: Changelog, https://esmerald.dymmond.com/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/dymmond/esmerald
 Author-email: Tiago Silva <tiago.silva@dymmond.com>
@@ -33,47 +33,31 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: a2wsgi<2,>=1.7.0
-Requires-Dist: aiofiles<23,>=0.8.0
+Requires-Dist: aiofiles<24,>=0.8.0
+Requires-Dist: anyio<4.0.0,>=3.6.2
 Requires-Dist: awesome-slugify<2,>=1.6.5
-Requires-Dist: httpx<0.30.0,>=0.23.3
+Requires-Dist: httpx<0.30.0,>=0.24.0
 Requires-Dist: itsdangerous<3.0.0,>=2.1.2
 Requires-Dist: jsonschema-rs<0.20.0,>=0.16.2
 Requires-Dist: loguru<0.7.0,>=0.6.0
 Requires-Dist: openapi-schemas-pydantic>=1.1.0
 Requires-Dist: pydantic-factories==1.17.2
-Requires-Dist: pydantic<2.0.0,>=1.10.5
+Requires-Dist: pydantic<2.0.0,>=1.10.7
+Requires-Dist: python-multipart<0.0.7,>=0.0.5
+Requires-Dist: rich<14.0.0,>=13.3.1
 Requires-Dist: starlette<0.27.0,>=0.26.1
-Provides-Extra: all
-Requires-Dist: a2wsgi<2,>=1.6.0; extra == 'all'
-Requires-Dist: aiofiles<23,>=0.8.0; extra == 'all'
-Requires-Dist: asyncz>=0.2.0; extra == 'all'
-Requires-Dist: awesome-slugify<2,>=1.6.5; extra == 'all'
-Requires-Dist: httpx<0.30.0,>=0.23.3; extra == 'all'
-Requires-Dist: jinja2<4.0.0,>=3.1.2; extra == 'all'
-Requires-Dist: jsonschema-rs<0.20.0,>=0.16.2; extra == 'all'
-Requires-Dist: loguru<0.7.0,>=0.6.0; extra == 'all'
-Requires-Dist: mako==1.2.4; extra == 'all'
-Requires-Dist: openapi-schemas-pydantic>=1.1.0; extra == 'all'
-Requires-Dist: orjson<4.0.0,>=3.8.5; extra == 'all'
-Requires-Dist: passlib==1.7.4; extra == 'all'
-Requires-Dist: pydantic-factories==1.17.2; extra == 'all'
-Requires-Dist: pydantic<2.0.0,>=1.10.5; extra == 'all'
-Requires-Dist: python-jose<4,>=3.3.0; extra == 'all'
-Requires-Dist: python-multipart<0.0.6,>=0.0.5; extra == 'all'
-Requires-Dist: ujson<6,>=5.7.0; extra == 'all'
 Provides-Extra: dev
 Requires-Dist: autoflake>=1.4.0; extra == 'dev'
 Requires-Dist: flake8<6.0.0,>=3.8.3; extra == 'dev'
-Requires-Dist: loguru<0.7.0,>=0.6.0; extra == 'dev'
-Requires-Dist: pre-commit<4.0.0,>=2.17.0; extra == 'dev'
+Requires-Dist: pre-commit<4.0.0,>=3.0.4; extra == 'dev'
 Requires-Dist: uvicorn[standard]>=0.19.0; extra == 'dev'
 Requires-Dist: watchfiles<0.20.0,>=0.16.1; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: mdx-include<2.0.0,>=1.4.2; extra == 'doc'
 Requires-Dist: mkautodoc<0.3.0,>=0.2.0; extra == 'doc'
 Requires-Dist: mkdocs-markdownextradata-plugin<0.3.0,>=0.2.5; extra == 'doc'
 Requires-Dist: mkdocs-material<10.0.0,>=9.0.13; extra == 'doc'
@@ -88,42 +72,37 @@
 Requires-Dist: python-jose<4,>=3.3.0; extra == 'jwt'
 Provides-Extra: schedulers
 Requires-Dist: asyncz>=0.2.0; extra == 'schedulers'
 Provides-Extra: templates
 Requires-Dist: jinja2<4.0.0,>=3.1.2; extra == 'templates'
 Requires-Dist: mako==1.2.4; extra == 'templates'
 Provides-Extra: test
-Requires-Dist: a2wsgi<2,>=1.6.0; extra == 'test'
-Requires-Dist: aiofiles<23,>=0.8.0; extra == 'test'
-Requires-Dist: anyio[trio]<4.0.0,>=3.2.1; extra == 'test'
+Requires-Dist: a2wsgi<2,>=1.7.0; extra == 'test'
+Requires-Dist: aiofiles<24,>=0.8.0; extra == 'test'
+Requires-Dist: anyio[trio]<4.0.0,>=3.6.2; extra == 'test'
 Requires-Dist: asyncio[trio]<4.0.0,>=3.4.3; extra == 'test'
 Requires-Dist: asyncz>=0.2.0; extra == 'test'
-Requires-Dist: awesome-slugify<2,>=1.6.5; extra == 'test'
-Requires-Dist: black==23.1.0; extra == 'test'
+Requires-Dist: black==23.3.0; extra == 'test'
 Requires-Dist: brotli<2.0.0,>=1.0.9; extra == 'test'
 Requires-Dist: flake8>=5.0.4; extra == 'test'
 Requires-Dist: flask<3.0.0,>=1.1.2; extra == 'test'
 Requires-Dist: freezegun<2.0.0,>=1.2.2; extra == 'test'
-Requires-Dist: httpx<0.24.0,>=0.23.3; extra == 'test'
 Requires-Dist: isort<6.0.0,>=5.0.6; extra == 'test'
 Requires-Dist: jinja2<4.0.0,>=3.1.2; extra == 'test'
-Requires-Dist: jsonschema-rs<0.20.0,>=0.16.2; extra == 'test'
 Requires-Dist: mock==5.0.1; extra == 'test'
-Requires-Dist: mypy==1.0.1; extra == 'test'
+Requires-Dist: mypy==1.1.1; extra == 'test'
 Requires-Dist: orjson<4.0.0,>=3.8.5; extra == 'test'
 Requires-Dist: passlib==1.7.4; extra == 'test'
-Requires-Dist: pydantic-factories==1.17.2; extra == 'test'
-Requires-Dist: pydantic<2.0.0,>=1.10.5; extra == 'test'
 Requires-Dist: pytest-asyncio>=0.19.0; extra == 'test'
 Requires-Dist: pytest-cov<5.0.0,>=2.12.0; extra == 'test'
 Requires-Dist: pytest<8.0.0,>=7.1.3; extra == 'test'
 Requires-Dist: python-jose<4,>=3.3.0; extra == 'test'
 Requires-Dist: requests<3.0.0,>=2.28.2; extra == 'test'
 Requires-Dist: ruff<1.0.0,>=0.0.256; extra == 'test'
-Requires-Dist: saffier[postgres]>=0.4.0; extra == 'test'
+Requires-Dist: saffier[postgres]>=0.6.1; extra == 'test'
 Requires-Dist: types-orjson==3.6.2; extra == 'test'
 Requires-Dist: types-ujson==5.7.0.1; extra == 'test'
 Requires-Dist: ujson<6,>=5.7.0; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Esmerald
 
@@ -224,32 +203,26 @@
 
 **Support for ORJSON and UJSON**:
 
 ```shell
 pip install esmerald[encoders]
 ```
 
-**All the esmerald features**:
-
-```shell
-pip install esmerald[all]
-```
-
 **If you want to use the esmerald testing client**:
 
 ```shell
 pip install esmerald[test]
 ```
 
 ### Start a project using directives
 
 If you wish to start an Esmerald project with a default suggested structure.
 
 ```
-esmerald-admin createproject <YOUR-PROJECT-NAME>
+esmerald createproject <YOUR-PROJECT-NAME>
 ```
 
 This will generate a scaffold for your project with some pre-defined files in a simple fashion.
 This will also generate a file for the tests using the EsmeraldTestClient, so make sure you run:
 
 ```shell
 pip install esmerald[test]
```

