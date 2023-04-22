# Comparing `tmp/freva_deployment-2304.0.0.tar.gz` & `tmp/freva_deployment-2304.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freva_deployment-2304.0.0.tar", last modified: Wed Apr 12 11:30:35 2023, max compression
+gzip compressed data, was "freva_deployment-2304.0.1.tar", last modified: Sat Apr 22 21:30:38 2023, max compression
```

## Comparing `freva_deployment-2304.0.0.tar` & `freva_deployment-2304.0.1.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.649448 freva_deployment-2304.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-04-12 11:30:35.645448 freva_deployment-2304.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.629447 freva_deployment-2304.0.0/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.629447 freva_deployment-2304.0.0/assets/config/
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/config/create_tables.sql
--rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/config/inventory.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.633447 freva_deployment-2304.0.0/assets/db_service/
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/db_service/password_rotate.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/db_service/reset_root_pw.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.633447 freva_deployment-2304.0.0/assets/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/playbooks/core-server-playbook.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/playbooks/db-server-playbook.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/playbooks/server-map-playbook.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/playbooks/solr-server-playbook.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/playbooks/vault-server-playbook.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/playbooks/web-server-playbook.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.633447 freva_deployment-2304.0.0/assets/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      351 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/scripts/create_cron.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/scripts/create_systemd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3293 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/scripts/docker-or-podman
--rwxr-xr-x   0 runner    (1001) docker     (123)       66 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/scripts/dump_sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.633447 freva_deployment-2304.0.0/assets/servers/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/servers/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.633447 freva_deployment-2304.0.0/assets/servers/freva/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/servers/freva/servers.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/servers/restservice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.637447 freva_deployment-2304.0.0/assets/vault/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/vault/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/vault/deploy_vault.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/vault/policy-file.hcl
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/vault/runserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/vault/vault-server-no-tls.hcl
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/vault/vault-server-tls.hcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.637447 freva_deployment-2304.0.0/assets/web/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2305 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/web/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/web/docker_cmd.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       17 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/web/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (123)    15874 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/web/freva_web.conf
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 11:30:35.649448 freva_deployment-2304.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.629447 freva_deployment-2304.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.641447 freva_deployment-2304.0.0/src/freva_deployment/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/src/freva_deployment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.645448 freva_deployment-2304.0.0/src/freva_deployment/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/src/freva_deployment/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/src/freva_deployment/cli/_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/src/freva_deployment/cli/_migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/src/freva_deployment/cli/_server_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/src/freva_deployment/cli/_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    21910 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/src/freva_deployment/deploy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.645448 freva_deployment-2304.0.0/src/freva_deployment/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/src/freva_deployment/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.645448 freva_deployment-2304.0.0/src/freva_deployment/ui/deployment_tui/
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/src/freva_deployment/ui/deployment_tui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/src/freva_deployment/ui/deployment_tui/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    33551 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/src/freva_deployment/ui/deployment_tui/deploy_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/src/freva_deployment/ui/deployment_tui/main_window.py
--rw-r--r--   0 runner    (1001) docker     (123)    11596 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/src/freva_deployment/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.641447 freva_deployment-2304.0.0/src/freva_deployment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-04-12 11:30:35.000000 freva_deployment-2304.0.0/src/freva_deployment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-12 11:30:35.000000 freva_deployment-2304.0.0/src/freva_deployment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 11:30:35.000000 freva_deployment-2304.0.0/src/freva_deployment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-12 11:30:35.000000 freva_deployment-2304.0.0/src/freva_deployment.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-12 11:30:35.000000 freva_deployment-2304.0.0/src/freva_deployment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-12 11:30:35.000000 freva_deployment-2304.0.0/src/freva_deployment.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.728277 freva_deployment-2304.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-04-22 21:30:38.728277 freva_deployment-2304.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.712277 freva_deployment-2304.0.1/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.716277 freva_deployment-2304.0.1/assets/config/
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/config/create_tables.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-22 21:30:29.000000 freva_deployment-2304.0.1/assets/config/evaluation_system.conf.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/config/inventory.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.716277 freva_deployment-2304.0.1/assets/db_service/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/db_service/password_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/db_service/reset_root_pw.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.716277 freva_deployment-2304.0.1/assets/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/playbooks/core-server-playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/playbooks/db-server-playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/playbooks/server-map-playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/playbooks/solr-server-playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/playbooks/vault-server-playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/playbooks/web-server-playbook.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.716277 freva_deployment-2304.0.1/assets/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      351 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/scripts/create_cron.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/scripts/create_systemd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3293 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/scripts/docker-or-podman
+-rwxr-xr-x   0 runner    (1001) docker     (123)       66 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/scripts/dump_sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.720277 freva_deployment-2304.0.1/assets/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/servers/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.720277 freva_deployment-2304.0.1/assets/servers/freva/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/servers/freva/servers.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/servers/restservice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.720277 freva_deployment-2304.0.1/assets/vault/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/vault/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/vault/deploy_vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/vault/policy-file.hcl
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/vault/runserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/vault/vault-server-no-tls.hcl
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/vault/vault-server-tls.hcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.720277 freva_deployment-2304.0.1/assets/web/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2305 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/web/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/web/docker_cmd.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       17 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/web/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    15874 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/web/freva_web.conf
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 21:30:38.728277 freva_deployment-2304.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.712277 freva_deployment-2304.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.720277 freva_deployment-2304.0.1/src/freva_deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/src/freva_deployment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.724277 freva_deployment-2304.0.1/src/freva_deployment/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/src/freva_deployment/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/src/freva_deployment/cli/_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/src/freva_deployment/cli/_migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/src/freva_deployment/cli/_server_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/src/freva_deployment/cli/_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21996 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/src/freva_deployment/deploy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.724277 freva_deployment-2304.0.1/src/freva_deployment/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/src/freva_deployment/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.728277 freva_deployment-2304.0.1/src/freva_deployment/ui/deployment_tui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/src/freva_deployment/ui/deployment_tui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/src/freva_deployment/ui/deployment_tui/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33544 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/src/freva_deployment/ui/deployment_tui/deploy_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/src/freva_deployment/ui/deployment_tui/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11596 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/src/freva_deployment/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.724277 freva_deployment-2304.0.1/src/freva_deployment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-04-22 21:30:38.000000 freva_deployment-2304.0.1/src/freva_deployment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-22 21:30:38.000000 freva_deployment-2304.0.1/src/freva_deployment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 21:30:38.000000 freva_deployment-2304.0.1/src/freva_deployment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-22 21:30:38.000000 freva_deployment-2304.0.1/src/freva_deployment.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-22 21:30:38.000000 freva_deployment-2304.0.1/src/freva_deployment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-22 21:30:38.000000 freva_deployment-2304.0.1/src/freva_deployment.egg-info/top_level.txt
```

### Comparing `freva_deployment-2304.0.0/PKG-INFO` & `freva_deployment-2304.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freva_deployment
-Version: 2304.0.0
+Version: 2304.0.1
 Summary: Deploy freva and its services on different machines.
 Home-page: https://github.com/FREVA-CLINT/freva.git
 Author: Martin Bergemann
 Author-email: martin.bergemann@dkrz.de
 Maintainer: Martin Bergemann
 License: GPLv3
 Project-URL: Documentation, https://freva-deployment.readthedocs.io/en/latest/
```

### Comparing `freva_deployment-2304.0.0/README.md` & `freva_deployment-2304.0.1/README.md`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.0/assets/config/create_tables.sql` & `freva_deployment-2304.0.1/assets/config/create_tables.sql`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.0/assets/config/inventory.toml` & `freva_deployment-2304.0.1/assets/config/inventory.toml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.0/assets/db_service/password_rotate.py` & `freva_deployment-2304.0.1/assets/db_service/password_rotate.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.0/assets/playbooks/core-server-playbook.yml` & `freva_deployment-2304.0.1/assets/playbooks/core-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.0/assets/playbooks/db-server-playbook.yml` & `freva_deployment-2304.0.1/assets/playbooks/db-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.0/assets/playbooks/server-map-playbook.yml` & `freva_deployment-2304.0.1/assets/playbooks/server-map-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.0/assets/playbooks/solr-server-playbook.yml` & `freva_deployment-2304.0.1/assets/playbooks/solr-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.0/assets/playbooks/vault-server-playbook.yml` & `freva_deployment-2304.0.1/assets/playbooks/vault-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.0/assets/playbooks/web-server-playbook.yml` & `freva_deployment-2304.0.1/assets/playbooks/web-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.0/assets/scripts/create_systemd.py` & `freva_deployment-2304.0.1/assets/scripts/create_systemd.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.0/assets/scripts/docker-or-podman` & `freva_deployment-2304.0.1/assets/scripts/docker-or-podman`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.0/assets/servers/Dockerfile` & `freva_deployment-2304.0.1/assets/servers/Dockerfile`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.0/assets/servers/restservice.py` & `freva_deployment-2304.0.1/assets/servers/restservice.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.0/assets/vault/Dockerfile` & `freva_deployment-2304.0.1/assets/vault/Dockerfile`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.0/assets/vault/deploy_vault.py` & `freva_deployment-2304.0.1/assets/vault/deploy_vault.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.0/assets/vault/runserver.py` & `freva_deployment-2304.0.1/assets/vault/runserver.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.0/assets/vault/vault-server-tls.hcl` & `freva_deployment-2304.0.1/assets/vault/vault-server-tls.hcl`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.0/assets/web/Dockerfile` & `freva_deployment-2304.0.1/assets/web/Dockerfile`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.0/assets/web/freva_web.conf` & `freva_deployment-2304.0.1/assets/web/freva_web.conf`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.0/setup.py` & `freva_deployment-2304.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,16 +17,15 @@
 
 
 INSTALL_REQUIRES = [
     "appdirs",
     "npyscreen",
     "numpy",
     "PyMySQL",
-    "pyncclient",
-    "pyyml",
+    "PyYAML",
     "rich",
     "toml",
     "tomlkit",
     "requests",
 ]
```

### Comparing `freva_deployment-2304.0.0/src/freva_deployment/cli/_deploy.py` & `freva_deployment-2304.0.1/src/freva_deployment/cli/_deploy.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.0/src/freva_deployment/cli/_migrate.py` & `freva_deployment-2304.0.1/src/freva_deployment/cli/_migrate.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.0/src/freva_deployment/cli/_server_map.py` & `freva_deployment-2304.0.1/src/freva_deployment/cli/_server_map.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.0/src/freva_deployment/cli/_service.py` & `freva_deployment-2304.0.1/src/freva_deployment/cli/_service.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.0/src/freva_deployment/deploy.py` & `freva_deployment-2304.0.1/src/freva_deployment/deploy.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,14 +198,16 @@
             self.cfg["web"]["config"]["admin"] = admin
         _webserver_items = {}
         try:
             for k, v in self.cfg["web"]["config"].items():
                 key = k.replace("web_", "").upper()
                 if key not in ("LDAP_USER_PW", "LDAP_USER_DN"):
                     _webserver_items[key] = v
+                else:
+                    self.cfg["web"]["config"].setdefault(k, "")
         except KeyError as error:
             raise KeyError(
                 "No web config section given, please configure the web.config"
             ) from error
         _webserver_items["ALLOWED_HOSTS"].append(self.cfg["web"]["hosts"])
         _webserver_items["REDIS_HOST"] = self.cfg["web"]["hosts"]
         try:
```

### Comparing `freva_deployment-2304.0.0/src/freva_deployment/ui/deployment_tui/__init__.py` & `freva_deployment-2304.0.1/src/freva_deployment/ui/deployment_tui/__init__.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.0/src/freva_deployment/ui/deployment_tui/base.py` & `freva_deployment-2304.0.1/src/freva_deployment/ui/deployment_tui/base.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.0/src/freva_deployment/ui/deployment_tui/deploy_forms.py` & `freva_deployment-2304.0.1/src/freva_deployment/ui/deployment_tui/deploy_forms.py`

 * *Files 0% similar despite different names*

```diff
@@ -460,17 +460,17 @@
                 ),
                 True,
             ),
             ldap_user_pw=(
                 self.add_widget_intelligent(
                     npyscreen.TitlePassword,
                     name=f"{self.num}Password for ldap user:",
-                    value=cfg.get("ldap_user_pw", "dkrzprox"),
+                    value=cfg.get("ldap_user_pw", ""),
                 ),
-                True,
+                False,
             ),
             ldap_first_name_field=(
                 self.add_widget_intelligent(
                     npyscreen.TitleText,
                     name=(f"{self.num}Ldap search search key for first name"),
                     value=cfg.get(
                         "ldap_first_name_field",
```

### Comparing `freva_deployment-2304.0.0/src/freva_deployment/ui/deployment_tui/main_window.py` & `freva_deployment-2304.0.1/src/freva_deployment/ui/deployment_tui/main_window.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.0/src/freva_deployment/utils.py` & `freva_deployment-2304.0.1/src/freva_deployment/utils.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.0/src/freva_deployment.egg-info/PKG-INFO` & `freva_deployment-2304.0.1/src/freva_deployment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freva-deployment
-Version: 2304.0.0
+Version: 2304.0.1
 Summary: Deploy freva and its services on different machines.
 Home-page: https://github.com/FREVA-CLINT/freva.git
 Author: Martin Bergemann
 Author-email: martin.bergemann@dkrz.de
 Maintainer: Martin Bergemann
 License: GPLv3
 Project-URL: Documentation, https://freva-deployment.readthedocs.io/en/latest/
```

### Comparing `freva_deployment-2304.0.0/src/freva_deployment.egg-info/SOURCES.txt` & `freva_deployment-2304.0.1/src/freva_deployment.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 MANIFEST.in
 README.md
 setup.py
 assets/config/create_tables.sql
+assets/config/evaluation_system.conf.tmpl
 assets/config/inventory.toml
 assets/db_service/password_rotate.py
 assets/db_service/reset_root_pw.sh
 assets/playbooks/core-server-playbook.yml
 assets/playbooks/db-server-playbook.yml
 assets/playbooks/server-map-playbook.yml
 assets/playbooks/solr-server-playbook.yml
```

