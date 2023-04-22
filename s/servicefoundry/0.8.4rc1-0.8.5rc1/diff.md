# Comparing `tmp/servicefoundry-0.8.4rc1.tar.gz` & `tmp/servicefoundry-0.8.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servicefoundry-0.8.4rc1.tar", max compression
+gzip compressed data, was "servicefoundry-0.8.5rc1.tar", max compression
```

## Comparing `servicefoundry-0.8.4rc1.tar` & `servicefoundry-0.8.5rc1.tar`

### file list

```diff
@@ -1,136 +1,136 @@
--rw-r--r--   0        0        0      672 2023-04-06 11:50:17.759329 servicefoundry-0.8.4rc1/README.md
--rw-r--r--   0        0        0     2284 2023-04-06 11:50:30.759486 servicefoundry-0.8.4rc1/pyproject.toml
--rw-r--r--   0        0        0     1266 2023-04-06 11:50:17.759329 servicefoundry-0.8.4rc1/servicefoundry/__init__.py
--rw-r--r--   0        0        0    36721 2023-04-06 11:50:17.759329 servicefoundry-0.8.4rc1/servicefoundry/auto_gen/models.py
--rw-r--r--   0        0        0     4159 2023-04-06 11:50:17.759329 servicefoundry-0.8.4rc1/servicefoundry/builder/__init__.py
--rw-r--r--   0        0        0      531 2023-04-06 11:50:17.759329 servicefoundry-0.8.4rc1/servicefoundry/builder/builders/__init__.py
--rw-r--r--   0        0        0     1364 2023-04-06 11:50:17.759329 servicefoundry-0.8.4rc1/servicefoundry/builder/builders/dockerfile.py
--rw-r--r--   0        0        0     1357 2023-04-06 11:50:17.759329 servicefoundry-0.8.4rc1/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py
--rw-r--r--   0        0        0     6479 2023-04-06 11:50:17.759329 servicefoundry-0.8.4rc1/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py
--rw-r--r--   0        0        0     6458 2023-04-06 11:50:17.759329 servicefoundry-0.8.4rc1/servicefoundry/builder/docker_service.py
--rw-r--r--   0        0        0       66 2023-04-06 11:50:17.759329 servicefoundry-0.8.4rc1/servicefoundry/cli/__init__.py
--rw-r--r--   0        0        0      494 2023-04-06 11:50:17.759329 servicefoundry-0.8.4rc1/servicefoundry/cli/__main__.py
--rw-r--r--   0        0        0     3089 2023-04-06 11:50:17.759329 servicefoundry-0.8.4rc1/servicefoundry/cli/cli_main.py
--rw-r--r--   0        0        0      958 2023-04-06 11:50:17.759329 servicefoundry-0.8.4rc1/servicefoundry/cli/commands/__init__.py
--rw-r--r--   0        0        0     1098 2023-04-06 11:50:17.759329 servicefoundry-0.8.4rc1/servicefoundry/cli/commands/build_command.py
--rw-r--r--   0        0        0     2803 2023-04-06 11:50:17.759329 servicefoundry-0.8.4rc1/servicefoundry/cli/commands/build_logs_command.py
--rw-r--r--   0        0        0     1890 2023-04-06 11:50:17.759329 servicefoundry-0.8.4rc1/servicefoundry/cli/commands/create_command.py
--rw-r--r--   0        0        0     2007 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/cli/commands/delete_command.py
--rw-r--r--   0        0        0     1227 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/cli/commands/deploy_v2_command.py
--rw-r--r--   0        0        0     2852 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/cli/commands/get_command.py
--rw-r--r--   0        0        0     2944 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/cli/commands/infra_bootstrap.py
--rw-r--r--   0        0        0     3753 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/cli/commands/list_command.py
--rw-r--r--   0        0        0     1080 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/cli/commands/login_command.py
--rw-r--r--   0        0        0      591 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/cli/commands/logout_command.py
--rw-r--r--   0        0        0     3878 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/cli/commands/logs_command.py
--rw-r--r--   0        0        0     1670 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/cli/commands/patch_command.py
--rw-r--r--   0        0        0     1077 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/cli/commands/redeploy_command.py
--rw-r--r--   0        0        0     1474 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/cli/commands/trigger_command.py
--rw-r--r--   0        0        0      206 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/cli/config.py
--rw-r--r--   0        0        0      228 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/cli/console.py
--rw-r--r--   0        0        0      510 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/cli/const.py
--rw-r--r--   0        0        0     3032 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/cli/display_util.py
--rw-r--r--   0        0        0        0 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/cli/io/__init__.py
--rw-r--r--   0        0        0     2289 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/cli/io/cli_input_hook.py
--rw-r--r--   0        0        0     2500 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/cli/util.py
--rw-r--r--   0        0        0      347 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/core/__init__.py
--rw-r--r--   0        0        0      379 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/core/login.py
--rw-r--r--   0        0        0      184 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/core/logout.py
--rw-r--r--   0        0        0      313 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/core/util.py
--rw-r--r--   0        0        0      188 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/function_service/__init__.py
--rw-r--r--   0        0        0      775 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/function_service/__main__.py
--rw-r--r--   0        0        0     2857 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/function_service/app.py
--rw-r--r--   0        0        0     1844 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/function_service/build.py
--rw-r--r--   0        0        0        0 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/function_service/deployment_examples/class_deployment/__init__.py
--rw-r--r--   0        0        0      673 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py
--rw-r--r--   0        0        0      185 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/function_service/deployment_examples/class_deployment/my_module.py
--rw-r--r--   0        0        0        0 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/function_service/deployment_examples/function_deployment/__init__.py
--rw-r--r--   0        0        0      600 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py
--rw-r--r--   0        0        0      297 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/function_service/deployment_examples/function_deployment/my_module.py
--rw-r--r--   0        0        0        0 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/function_service/deployment_examples/model_composition/__init__.py
--rw-r--r--   0        0        0     1772 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/function_service/deployment_examples/model_composition/deployment.py
--rw-r--r--   0        0        0      369 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/function_service/deployment_examples/model_composition/model.py
--rw-r--r--   0        0        0     1513 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py
--rw-r--r--   0        0        0      153 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/function_service/deployment_examples/model_composition/utils.py
--rw-r--r--   0        0        0        0 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/function_service/deployment_examples/one_service_calling_another/__init__.py
--rw-r--r--   0        0        0      414 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/function_service/deployment_examples/one_service_calling_another/deployment.py
--rw-r--r--   0        0        0      518 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py
--rw-r--r--   0        0        0      191 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/function_service/remote/__init__.py
--rw-r--r--   0        0        0       67 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/function_service/remote/context.py
--rw-r--r--   0        0        0     1875 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/function_service/remote/method.py
--rw-r--r--   0        0        0     4224 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/function_service/remote/remote.py
--rw-r--r--   0        0        0     4494 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/function_service/route.py
--rw-r--r--   0        0        0     3471 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/function_service/service.py
--rw-r--r--   0        0        0     1231 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/function_service/utils.py
--rw-r--r--   0        0        0        0 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/internal/__init__.py
--rw-r--r--   0        0        0      960 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/internal/experimental.py
--rw-r--r--   0        0        0        0 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/io/__init__.py
--rw-r--r--   0        0        0     1801 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/io/input_hook.py
--rw-r--r--   0        0        0        0 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/io/notebook/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/io/notebook/io/__init__.py
--rw-r--r--   0        0        0     1871 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/io/notebook/io/notebook_callback.py
--rw-r--r--   0        0        0     1041 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/io/notebook/io/notebook_input_hook.py
--rw-r--r--   0        0        0     1010 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/io/notebook/notebook_util.py
--rw-r--r--   0        0        0      532 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/io/output_callback.py
--rw-r--r--   0        0        0      629 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/io/parameters.py
--rw-r--r--   0        0        0      825 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/io/rich_output_callback.py
--rw-r--r--   0        0        0      175 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/json_util.py
--rw-r--r--   0        0        0        0 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/__init__.py
--rw-r--r--   0        0        0     2906 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/auth/auth_service_client.py
--rw-r--r--   0        0        0     4228 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/auth/credential_file_manager.py
--rw-r--r--   0        0        0     4268 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/auth/credential_provider.py
--rw-r--r--   0        0        0     1854 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/auth/servicefoundry_session.py
--rw-r--r--   0        0        0     7447 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/binarydownloader.py
--rw-r--r--   0        0        0        0 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/clients/__init__.py
--rw-r--r--   0        0        0      671 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/clients/cookiecutter_client.py
--rw-r--r--   0        0        0     2563 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/clients/git_client.py
--rw-r--r--   0        0        0    23861 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/clients/service_foundry_client.py
--rw-r--r--   0        0        0      455 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/clients/shell_client.py
--rw-r--r--   0        0        0     1455 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/clients/terragrunt_client.py
--rw-r--r--   0        0        0     1122 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/clients/utils.py
--rw-r--r--   0        0        0     1331 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/config/config_manager.py
--rw-r--r--   0        0        0     2232 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/config/dict_questionaire.py
--rw-r--r--   0        0        0    10594 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/config/infra_config.py
--rw-r--r--   0        0        0     1886 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/config/installation_config.py
--rw-r--r--   0        0        0     1752 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/const.py
--rw-r--r--   0        0        0        0 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/dao/__init__.py
--rw-r--r--   0        0        0     5568 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/dao/application.py
--rw-r--r--   0        0        0     1028 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/dao/version.py
--rw-r--r--   0        0        0     2533 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/dao/workspace.py
--rw-r--r--   0        0        0      588 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/exceptions.py
--rw-r--r--   0        0        0      288 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/infra/argo-secrets.mustache
--rw-r--r--   0        0        0      918 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/infra/argo-ubermold.mustache
--rw-r--r--   0        0        0    23708 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/infra/install_truefoundry.py
--rw-r--r--   0        0        0     1411 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/infra/nats-bootstrap.sh
--rw-r--r--   0        0        0      328 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/infra/tfy-agent.mustache
--rw-r--r--   0        0        0     1137 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/infra/tfy-control-plane.mustache
--rw-r--r--   0        0        0     6290 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/infra/utils.py
--rw-r--r--   0        0        0     1463 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/logs_utils.py
--rw-r--r--   0        0        0     1409 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/messages.py
--rw-r--r--   0        0        0        0 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/model/__init__.py
--rw-r--r--   0        0        0     9608 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/model/entity.py
--rw-r--r--   0        0        0     5191 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/session.py
--rw-r--r--   0        0        0      993 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/util.py
--rw-r--r--   0        0        0     4995 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/lib/win32.py
--rw-r--r--   0        0        0      688 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/logger.py
--rw-r--r--   0        0        0        0 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/v2/__init__.py
--rw-r--r--   0        0        0      517 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/v2/examples/job_deployment/deploy.py
--rw-r--r--   0        0        0      305 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/v2/examples/job_deployment/main.py
--rw-r--r--   0        0        0      303 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/v2/examples/job_deployment/servicefoundry.yaml
--rw-r--r--   0        0        0      441 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/v2/examples/job_deployment/servicefoundry_manual.yaml
--rw-r--r--   0        0        0      524 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml
--rw-r--r--   0        0        0      639 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/v2/examples/model_deployment/hf/deploy.py
--rw-r--r--   0        0        0      190 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/v2/examples/model_deployment/hf/servicefoundry.yaml
--rw-r--r--   0        0        0      579 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py
--rw-r--r--   0        0        0      313 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/v2/examples/model_deployment/mlfoundry/servicefoundry.yaml
--rw-r--r--   0        0        0      764 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/v2/examples/service_deployment/deploy.py
--rw-r--r--   0        0        0      117 2023-04-06 11:50:17.763330 servicefoundry-0.8.4rc1/servicefoundry/v2/examples/service_deployment/main.py
--rw-r--r--   0        0        0      482 2023-04-06 11:50:17.767330 servicefoundry-0.8.4rc1/servicefoundry/v2/examples/service_deployment/servicefoundry.yaml
--rw-r--r--   0        0        0      188 2023-04-06 11:50:17.767330 servicefoundry-0.8.4rc1/servicefoundry/v2/lib/__init__.py
--rw-r--r--   0        0        0     9914 2023-04-06 11:50:17.767330 servicefoundry-0.8.4rc1/servicefoundry/v2/lib/deploy.py
--rw-r--r--   0        0        0     1876 2023-04-06 11:50:17.767330 servicefoundry-0.8.4rc1/servicefoundry/v2/lib/deployable_patched_models.py
--rw-r--r--   0        0        0     1105 2023-04-06 11:50:17.767330 servicefoundry-0.8.4rc1/servicefoundry/v2/lib/models.py
--rw-r--r--   0        0        0     5276 2023-04-06 11:50:17.767330 servicefoundry-0.8.4rc1/servicefoundry/v2/lib/patched_models.py
--rw-r--r--   0        0        0     8890 2023-04-06 11:50:17.767330 servicefoundry-0.8.4rc1/servicefoundry/v2/lib/source.py
--rw-r--r--   0        0        0      130 2023-04-06 11:50:17.767330 servicefoundry-0.8.4rc1/servicefoundry/version.py
--rw-r--r--   0        0        0     2582 1970-01-01 00:00:00.000000 servicefoundry-0.8.4rc1/PKG-INFO
+-rw-r--r--   0        0        0      672 2023-04-22 14:33:24.758953 servicefoundry-0.8.5rc1/README.md
+-rw-r--r--   0        0        0     2284 2023-04-22 14:33:38.183303 servicefoundry-0.8.5rc1/pyproject.toml
+-rw-r--r--   0        0        0     1266 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/__init__.py
+-rw-r--r--   0        0        0    36721 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/auto_gen/models.py
+-rw-r--r--   0        0        0     4159 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/builder/__init__.py
+-rw-r--r--   0        0        0      531 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/builder/builders/__init__.py
+-rw-r--r--   0        0        0     1364 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/builder/builders/dockerfile.py
+-rw-r--r--   0        0        0     1357 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py
+-rw-r--r--   0        0        0     6479 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py
+-rw-r--r--   0        0        0     6458 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/builder/docker_service.py
+-rw-r--r--   0        0        0       66 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/__init__.py
+-rw-r--r--   0        0        0      494 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/__main__.py
+-rw-r--r--   0        0        0     3089 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/cli_main.py
+-rw-r--r--   0        0        0      958 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1098 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/commands/build_command.py
+-rw-r--r--   0        0        0     2803 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/commands/build_logs_command.py
+-rw-r--r--   0        0        0     1890 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/commands/create_command.py
+-rw-r--r--   0        0        0     2007 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/commands/delete_command.py
+-rw-r--r--   0        0        0     1227 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/commands/deploy_v2_command.py
+-rw-r--r--   0        0        0     2852 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/commands/get_command.py
+-rw-r--r--   0        0        0     2944 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/commands/infra_bootstrap.py
+-rw-r--r--   0        0        0     3753 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/commands/list_command.py
+-rw-r--r--   0        0        0     1080 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/commands/login_command.py
+-rw-r--r--   0        0        0      591 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/commands/logout_command.py
+-rw-r--r--   0        0        0     3878 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/commands/logs_command.py
+-rw-r--r--   0        0        0     1670 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/commands/patch_command.py
+-rw-r--r--   0        0        0     1077 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/commands/redeploy_command.py
+-rw-r--r--   0        0        0     1474 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/commands/trigger_command.py
+-rw-r--r--   0        0        0      206 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/config.py
+-rw-r--r--   0        0        0      228 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/console.py
+-rw-r--r--   0        0        0      510 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/const.py
+-rw-r--r--   0        0        0     3032 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/display_util.py
+-rw-r--r--   0        0        0        0 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/io/__init__.py
+-rw-r--r--   0        0        0     2289 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/io/cli_input_hook.py
+-rw-r--r--   0        0        0     2500 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/util.py
+-rw-r--r--   0        0        0      347 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/core/__init__.py
+-rw-r--r--   0        0        0      379 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/core/login.py
+-rw-r--r--   0        0        0      184 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/core/logout.py
+-rw-r--r--   0        0        0      313 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/core/util.py
+-rw-r--r--   0        0        0      188 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/__init__.py
+-rw-r--r--   0        0        0      775 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/__main__.py
+-rw-r--r--   0        0        0     2857 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/app.py
+-rw-r--r--   0        0        0     1844 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/build.py
+-rw-r--r--   0        0        0        0 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/class_deployment/__init__.py
+-rw-r--r--   0        0        0      673 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py
+-rw-r--r--   0        0        0      185 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/class_deployment/my_module.py
+-rw-r--r--   0        0        0        0 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/function_deployment/__init__.py
+-rw-r--r--   0        0        0      600 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py
+-rw-r--r--   0        0        0      297 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/function_deployment/my_module.py
+-rw-r--r--   0        0        0        0 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/model_composition/__init__.py
+-rw-r--r--   0        0        0     1772 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/model_composition/deployment.py
+-rw-r--r--   0        0        0      369 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/model_composition/model.py
+-rw-r--r--   0        0        0     1513 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py
+-rw-r--r--   0        0        0      153 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/model_composition/utils.py
+-rw-r--r--   0        0        0        0 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/one_service_calling_another/__init__.py
+-rw-r--r--   0        0        0      414 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/one_service_calling_another/deployment.py
+-rw-r--r--   0        0        0      518 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py
+-rw-r--r--   0        0        0      191 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/remote/__init__.py
+-rw-r--r--   0        0        0       67 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/remote/context.py
+-rw-r--r--   0        0        0     1875 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/remote/method.py
+-rw-r--r--   0        0        0     4224 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/remote/remote.py
+-rw-r--r--   0        0        0     4494 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/route.py
+-rw-r--r--   0        0        0     4139 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/service.py
+-rw-r--r--   0        0        0     1231 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/utils.py
+-rw-r--r--   0        0        0        0 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/internal/__init__.py
+-rw-r--r--   0        0        0      960 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/internal/experimental.py
+-rw-r--r--   0        0        0        0 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/io/__init__.py
+-rw-r--r--   0        0        0     1801 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/io/input_hook.py
+-rw-r--r--   0        0        0        0 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/io/notebook/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/io/notebook/io/__init__.py
+-rw-r--r--   0        0        0     1871 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/io/notebook/io/notebook_callback.py
+-rw-r--r--   0        0        0     1041 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/io/notebook/io/notebook_input_hook.py
+-rw-r--r--   0        0        0     1010 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/io/notebook/notebook_util.py
+-rw-r--r--   0        0        0      532 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/io/output_callback.py
+-rw-r--r--   0        0        0      629 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/io/parameters.py
+-rw-r--r--   0        0        0      825 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/io/rich_output_callback.py
+-rw-r--r--   0        0        0      175 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/json_util.py
+-rw-r--r--   0        0        0        0 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/__init__.py
+-rw-r--r--   0        0        0     2906 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/auth/auth_service_client.py
+-rw-r--r--   0        0        0     4228 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/auth/credential_file_manager.py
+-rw-r--r--   0        0        0     4268 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/auth/credential_provider.py
+-rw-r--r--   0        0        0     1854 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/auth/servicefoundry_session.py
+-rw-r--r--   0        0        0     7447 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/binarydownloader.py
+-rw-r--r--   0        0        0        0 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/clients/__init__.py
+-rw-r--r--   0        0        0      671 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/clients/cookiecutter_client.py
+-rw-r--r--   0        0        0     2563 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/clients/git_client.py
+-rw-r--r--   0        0        0    23861 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/clients/service_foundry_client.py
+-rw-r--r--   0        0        0      455 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/clients/shell_client.py
+-rw-r--r--   0        0        0     1455 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/clients/terragrunt_client.py
+-rw-r--r--   0        0        0     1122 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/clients/utils.py
+-rw-r--r--   0        0        0     1331 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/config/config_manager.py
+-rw-r--r--   0        0        0     2232 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/config/dict_questionaire.py
+-rw-r--r--   0        0        0    10594 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/config/infra_config.py
+-rw-r--r--   0        0        0     1886 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/config/installation_config.py
+-rw-r--r--   0        0        0     1752 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/const.py
+-rw-r--r--   0        0        0        0 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/dao/__init__.py
+-rw-r--r--   0        0        0     5568 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/dao/application.py
+-rw-r--r--   0        0        0     1028 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/dao/version.py
+-rw-r--r--   0        0        0     2533 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/dao/workspace.py
+-rw-r--r--   0        0        0      588 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/exceptions.py
+-rw-r--r--   0        0        0      288 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/infra/argo-secrets.mustache
+-rw-r--r--   0        0        0      918 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/infra/argo-ubermold.mustache
+-rw-r--r--   0        0        0    23708 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/infra/install_truefoundry.py
+-rw-r--r--   0        0        0     1411 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/infra/nats-bootstrap.sh
+-rw-r--r--   0        0        0      328 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/infra/tfy-agent.mustache
+-rw-r--r--   0        0        0     1137 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/infra/tfy-control-plane.mustache
+-rw-r--r--   0        0        0     6290 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/infra/utils.py
+-rw-r--r--   0        0        0     1463 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/logs_utils.py
+-rw-r--r--   0        0        0     1409 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/messages.py
+-rw-r--r--   0        0        0        0 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/model/__init__.py
+-rw-r--r--   0        0        0     9608 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/model/entity.py
+-rw-r--r--   0        0        0     5191 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/session.py
+-rw-r--r--   0        0        0      993 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/util.py
+-rw-r--r--   0        0        0     4995 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/win32.py
+-rw-r--r--   0        0        0      688 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/logger.py
+-rw-r--r--   0        0        0        0 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/__init__.py
+-rw-r--r--   0        0        0      517 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/examples/job_deployment/deploy.py
+-rw-r--r--   0        0        0      305 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/examples/job_deployment/main.py
+-rw-r--r--   0        0        0      303 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/examples/job_deployment/servicefoundry.yaml
+-rw-r--r--   0        0        0      441 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/examples/job_deployment/servicefoundry_manual.yaml
+-rw-r--r--   0        0        0      524 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml
+-rw-r--r--   0        0        0      639 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/examples/model_deployment/hf/deploy.py
+-rw-r--r--   0        0        0      190 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/examples/model_deployment/hf/servicefoundry.yaml
+-rw-r--r--   0        0        0      579 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py
+-rw-r--r--   0        0        0      313 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/examples/model_deployment/mlfoundry/servicefoundry.yaml
+-rw-r--r--   0        0        0      764 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/examples/service_deployment/deploy.py
+-rw-r--r--   0        0        0      117 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/examples/service_deployment/main.py
+-rw-r--r--   0        0        0      482 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/examples/service_deployment/servicefoundry.yaml
+-rw-r--r--   0        0        0      188 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/lib/__init__.py
+-rw-r--r--   0        0        0     9914 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/lib/deploy.py
+-rw-r--r--   0        0        0     1876 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/lib/deployable_patched_models.py
+-rw-r--r--   0        0        0     1105 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/lib/models.py
+-rw-r--r--   0        0        0     5276 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/lib/patched_models.py
+-rw-r--r--   0        0        0     8890 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/lib/source.py
+-rw-r--r--   0        0        0      130 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/version.py
+-rw-r--r--   0        0        0     2582 1970-01-01 00:00:00.000000 servicefoundry-0.8.5rc1/PKG-INFO
```

### Comparing `servicefoundry-0.8.4rc1/README.md` & `servicefoundry-0.8.5rc1/README.md`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/pyproject.toml` & `servicefoundry-0.8.5rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "servicefoundry"
-version = "0.8.4rc1"  # do not change, auto-generated by poetry-dynamic-versioning
+version = "0.8.5rc1"  # do not change, auto-generated by poetry-dynamic-versioning
 description = "Generate deployed services from code"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 homepage = "https://github.com/innoavator/servicefoundry"
 repository = "https://github.com/innoavator/servicefoundry"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/__init__.py` & `servicefoundry-0.8.5rc1/servicefoundry/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/auto_gen/models.py` & `servicefoundry-0.8.5rc1/servicefoundry/auto_gen/models.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/builder/__init__.py` & `servicefoundry-0.8.5rc1/servicefoundry/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/builder/builders/__init__.py` & `servicefoundry-0.8.5rc1/servicefoundry/builder/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/builder/builders/dockerfile.py` & `servicefoundry-0.8.5rc1/servicefoundry/builder/builders/dockerfile.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py` & `servicefoundry-0.8.5rc1/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py` & `servicefoundry-0.8.5rc1/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/builder/docker_service.py` & `servicefoundry-0.8.5rc1/servicefoundry/builder/docker_service.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/cli/cli_main.py` & `servicefoundry-0.8.5rc1/servicefoundry/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/cli/commands/__init__.py` & `servicefoundry-0.8.5rc1/servicefoundry/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/cli/commands/build_command.py` & `servicefoundry-0.8.5rc1/servicefoundry/cli/commands/build_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/cli/commands/build_logs_command.py` & `servicefoundry-0.8.5rc1/servicefoundry/cli/commands/build_logs_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/cli/commands/create_command.py` & `servicefoundry-0.8.5rc1/servicefoundry/cli/commands/create_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/cli/commands/delete_command.py` & `servicefoundry-0.8.5rc1/servicefoundry/cli/commands/delete_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/cli/commands/deploy_v2_command.py` & `servicefoundry-0.8.5rc1/servicefoundry/cli/commands/deploy_v2_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/cli/commands/get_command.py` & `servicefoundry-0.8.5rc1/servicefoundry/cli/commands/get_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/cli/commands/infra_bootstrap.py` & `servicefoundry-0.8.5rc1/servicefoundry/cli/commands/infra_bootstrap.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/cli/commands/list_command.py` & `servicefoundry-0.8.5rc1/servicefoundry/cli/commands/list_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/cli/commands/login_command.py` & `servicefoundry-0.8.5rc1/servicefoundry/cli/commands/login_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/cli/commands/logout_command.py` & `servicefoundry-0.8.5rc1/servicefoundry/cli/commands/logout_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/cli/commands/logs_command.py` & `servicefoundry-0.8.5rc1/servicefoundry/cli/commands/logs_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/cli/commands/patch_command.py` & `servicefoundry-0.8.5rc1/servicefoundry/cli/commands/patch_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/cli/commands/redeploy_command.py` & `servicefoundry-0.8.5rc1/servicefoundry/cli/commands/redeploy_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/cli/commands/trigger_command.py` & `servicefoundry-0.8.5rc1/servicefoundry/cli/commands/trigger_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/cli/display_util.py` & `servicefoundry-0.8.5rc1/servicefoundry/cli/display_util.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/cli/io/cli_input_hook.py` & `servicefoundry-0.8.5rc1/servicefoundry/cli/io/cli_input_hook.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/cli/util.py` & `servicefoundry-0.8.5rc1/servicefoundry/cli/util.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/function_service/__main__.py` & `servicefoundry-0.8.5rc1/servicefoundry/function_service/__main__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/function_service/app.py` & `servicefoundry-0.8.5rc1/servicefoundry/function_service/app.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/function_service/build.py` & `servicefoundry-0.8.5rc1/servicefoundry/function_service/build.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py` & `servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py` & `servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/function_service/deployment_examples/model_composition/deployment.py` & `servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/model_composition/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py` & `servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py` & `servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/function_service/remote/method.py` & `servicefoundry-0.8.5rc1/servicefoundry/function_service/remote/method.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/function_service/remote/remote.py` & `servicefoundry-0.8.5rc1/servicefoundry/function_service/remote/remote.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/function_service/route.py` & `servicefoundry-0.8.5rc1/servicefoundry/function_service/route.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/function_service/service.py` & `servicefoundry-0.8.5rc1/servicefoundry/function_service/service.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,47 @@
 from threading import Thread
-from typing import Any, Callable, Dict, Optional
+from typing import Any, Callable, Dict, Optional, Union
 
 import yaml
 
 from servicefoundry.auto_gen.models import Port, Resources
 from servicefoundry.function_service.app import build_and_run_app_in_background_thread
 from servicefoundry.function_service.build import BuildConfig
 from servicefoundry.function_service.remote import RemoteClass
 from servicefoundry.function_service.route import RouteGroups
+from servicefoundry.logger import logger
 from servicefoundry.v2.lib.deployable_patched_models import Service
 from servicefoundry.v2.lib.patched_models import Build, LocalSource
 
 
 class FunctionService:
     def __init__(
         self,
         name: str,
         build_config: Optional[BuildConfig] = None,
         resources: Optional[Resources] = None,
         replicas: int = 1,
-        port: int = 8000,
+        port: Union[int, Port] = Port(port=8000, expose=False),
         env: Optional[Dict[str, str]] = None,
     ):
         self._name = name
         self._build_config = build_config or BuildConfig()
         self._resources = resources or Resources()
         self._replicas = replicas
+        if isinstance(port, int):
+            port = Port(port=port, expose=False)
+        if not port.host:
+            logger.warning(
+                "No host is set for the port. This is not an issue if you don't "
+                "want an exposed endpoint or are just testing locally.\n"
+                "However, for actual deployment it is required to pass an "
+                "instance of `servicefoundry.Port` with "
+                "`host` argument defined.\n"
+                "E.g. `FunctionService(name='...', port=Port(port=8000, host='...', path='...'), ...)`"
+            )
         self._port = port
         self._env = env or {}
 
         self._route_groups: RouteGroups = RouteGroups()
 
     @property
     def route_groups(self) -> RouteGroups:
@@ -39,15 +51,15 @@
         return yaml.dump(
             dict(
                 name=self._name,
                 build_config=self._build_config.dict(),
                 resources=self._resources.dict(),
                 routes=self._route_groups.dict(),
                 replicas=self._replicas,
-                port=self._port,
+                port=self._port.dict(),
                 env=self._env,
             ),
             indent=2,
         )
 
     def register_function(
         self,
@@ -69,31 +81,31 @@
         #   For now, I am removing the burden of using `remote` from the user when deploying
         #   an instance of a class.
         remote_class = RemoteClass(class_, init_kwargs=init_kwargs, name=name)
         self._route_groups.register_class(remote_class=remote_class)
 
     def run(self) -> Thread:
         return build_and_run_app_in_background_thread(
-            route_groups=self._route_groups, port=self._port
+            route_groups=self._route_groups, port=self._port.port
         )
 
     def get_deployment_definition(self) -> Service:
         # Keeping this function right now so that later,
         # the constructor of the application call this function
         # to get the component spec, if an object of this class
-        # is directly passed as an component
+        # is directly passed as a component
         tfy_python_build_config = self._build_config.to_tfy_python_build_config(
-            port=self._port, route_groups=self._route_groups
+            port=self._port.port, route_groups=self._route_groups
         )
         service = Service(
             name=self._name,
             image=Build(build_source=LocalSource(), build_spec=tfy_python_build_config),
             resources=self._resources,
             replicas=self._replicas,
-            ports=[Port(port=self._port, expose=True)],
+            ports=[self._port],
             env=self._env,
         )
         return service
 
     def deploy(self, workspace_fqn: str, wait: bool = True):
         service = self.get_deployment_definition()
         service.deploy(workspace_fqn=workspace_fqn, wait=wait)
```

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/function_service/utils.py` & `servicefoundry-0.8.5rc1/servicefoundry/function_service/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/internal/experimental.py` & `servicefoundry-0.8.5rc1/servicefoundry/internal/experimental.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/io/input_hook.py` & `servicefoundry-0.8.5rc1/servicefoundry/io/input_hook.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/io/notebook/io/notebook_callback.py` & `servicefoundry-0.8.5rc1/servicefoundry/io/notebook/io/notebook_callback.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/io/notebook/io/notebook_input_hook.py` & `servicefoundry-0.8.5rc1/servicefoundry/io/notebook/io/notebook_input_hook.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/io/notebook/notebook_util.py` & `servicefoundry-0.8.5rc1/servicefoundry/io/notebook/notebook_util.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/io/output_callback.py` & `servicefoundry-0.8.5rc1/servicefoundry/io/output_callback.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/io/parameters.py` & `servicefoundry-0.8.5rc1/servicefoundry/io/parameters.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/io/rich_output_callback.py` & `servicefoundry-0.8.5rc1/servicefoundry/io/rich_output_callback.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/lib/auth/auth_service_client.py` & `servicefoundry-0.8.5rc1/servicefoundry/lib/auth/auth_service_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/lib/auth/credential_file_manager.py` & `servicefoundry-0.8.5rc1/servicefoundry/lib/auth/credential_file_manager.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/lib/auth/credential_provider.py` & `servicefoundry-0.8.5rc1/servicefoundry/lib/auth/credential_provider.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/lib/auth/servicefoundry_session.py` & `servicefoundry-0.8.5rc1/servicefoundry/lib/auth/servicefoundry_session.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/lib/binarydownloader.py` & `servicefoundry-0.8.5rc1/servicefoundry/lib/binarydownloader.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/lib/clients/cookiecutter_client.py` & `servicefoundry-0.8.5rc1/servicefoundry/lib/clients/cookiecutter_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/lib/clients/git_client.py` & `servicefoundry-0.8.5rc1/servicefoundry/lib/clients/git_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/lib/clients/service_foundry_client.py` & `servicefoundry-0.8.5rc1/servicefoundry/lib/clients/service_foundry_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/lib/clients/terragrunt_client.py` & `servicefoundry-0.8.5rc1/servicefoundry/lib/clients/terragrunt_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/lib/clients/utils.py` & `servicefoundry-0.8.5rc1/servicefoundry/lib/clients/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/lib/config/config_manager.py` & `servicefoundry-0.8.5rc1/servicefoundry/lib/config/config_manager.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/lib/config/dict_questionaire.py` & `servicefoundry-0.8.5rc1/servicefoundry/lib/config/dict_questionaire.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/lib/config/infra_config.py` & `servicefoundry-0.8.5rc1/servicefoundry/lib/config/infra_config.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/lib/config/installation_config.py` & `servicefoundry-0.8.5rc1/servicefoundry/lib/config/installation_config.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/lib/const.py` & `servicefoundry-0.8.5rc1/servicefoundry/lib/const.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/lib/dao/application.py` & `servicefoundry-0.8.5rc1/servicefoundry/lib/dao/application.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/lib/dao/version.py` & `servicefoundry-0.8.5rc1/servicefoundry/lib/dao/version.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/lib/dao/workspace.py` & `servicefoundry-0.8.5rc1/servicefoundry/lib/dao/workspace.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/lib/exceptions.py` & `servicefoundry-0.8.5rc1/servicefoundry/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/lib/infra/argo-ubermold.mustache` & `servicefoundry-0.8.5rc1/servicefoundry/lib/infra/argo-ubermold.mustache`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/lib/infra/install_truefoundry.py` & `servicefoundry-0.8.5rc1/servicefoundry/lib/infra/install_truefoundry.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/lib/infra/nats-bootstrap.sh` & `servicefoundry-0.8.5rc1/servicefoundry/lib/infra/nats-bootstrap.sh`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/lib/infra/tfy-control-plane.mustache` & `servicefoundry-0.8.5rc1/servicefoundry/lib/infra/tfy-control-plane.mustache`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/lib/infra/utils.py` & `servicefoundry-0.8.5rc1/servicefoundry/lib/infra/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/lib/logs_utils.py` & `servicefoundry-0.8.5rc1/servicefoundry/lib/logs_utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/lib/messages.py` & `servicefoundry-0.8.5rc1/servicefoundry/lib/messages.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/lib/model/entity.py` & `servicefoundry-0.8.5rc1/servicefoundry/lib/model/entity.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/lib/session.py` & `servicefoundry-0.8.5rc1/servicefoundry/lib/session.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/lib/util.py` & `servicefoundry-0.8.5rc1/servicefoundry/lib/util.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/lib/win32.py` & `servicefoundry-0.8.5rc1/servicefoundry/lib/win32.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/logger.py` & `servicefoundry-0.8.5rc1/servicefoundry/logger.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/v2/examples/job_deployment/deploy.py` & `servicefoundry-0.8.5rc1/servicefoundry/v2/examples/job_deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml` & `servicefoundry-0.8.5rc1/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/v2/examples/model_deployment/hf/deploy.py` & `servicefoundry-0.8.5rc1/servicefoundry/v2/examples/model_deployment/hf/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py` & `servicefoundry-0.8.5rc1/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/v2/examples/service_deployment/deploy.py` & `servicefoundry-0.8.5rc1/servicefoundry/v2/examples/service_deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/v2/lib/deploy.py` & `servicefoundry-0.8.5rc1/servicefoundry/v2/lib/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/v2/lib/deployable_patched_models.py` & `servicefoundry-0.8.5rc1/servicefoundry/v2/lib/deployable_patched_models.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/v2/lib/models.py` & `servicefoundry-0.8.5rc1/servicefoundry/v2/lib/models.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/v2/lib/patched_models.py` & `servicefoundry-0.8.5rc1/servicefoundry/v2/lib/patched_models.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/servicefoundry/v2/lib/source.py` & `servicefoundry-0.8.5rc1/servicefoundry/v2/lib/source.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.4rc1/PKG-INFO` & `servicefoundry-0.8.5rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servicefoundry
-Version: 0.8.4rc1
+Version: 0.8.5rc1
 Summary: Generate deployed services from code
 Home-page: https://github.com/innoavator/servicefoundry
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

