# Comparing `tmp/aegea-4.3.4.tar.gz` & `tmp/aegea-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aegea-4.3.4.tar", last modified: Sun Apr  2 15:16:06 2023, max compression
+gzip compressed data, was "aegea-4.4.0.tar", last modified: Sat Apr 22 02:28:03 2023, max compression
```

## Comparing `aegea-4.3.4.tar` & `aegea-4.4.0.tar`

### file list

```diff
@@ -1,355 +1,301 @@
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.042717 aegea-4.3.4/
--rw-r--r--   0 kislyuk    (501) staff       (20)       44 2022-07-01 05:40:57.000000 aegea-4.3.4/.coveragerc
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:05.996158 aegea-4.3.4/.github/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.005393 aegea-4.3.4/.github/workflows/
--rw-r--r--   0 kislyuk    (501) staff       (20)     1251 2023-03-27 05:42:23.000000 aegea-4.3.4/.github/workflows/ci.yml
--rw-r--r--   0 kislyuk    (501) staff       (20)      518 2022-07-01 05:40:57.000000 aegea-4.3.4/.gitignore
--rw-r--r--   0 kislyuk    (501) staff       (20)    36138 2023-04-02 15:15:42.000000 aegea-4.3.4/Changes.rst
--rw-r--r--   0 kislyuk    (501) staff       (20)    11357 2016-06-14 14:20:08.000000 aegea-4.3.4/LICENSE.md
--rw-r--r--   0 kislyuk    (501) staff       (20)      188 2022-07-01 05:40:57.000000 aegea-4.3.4/MANIFEST.in
--rw-r--r--   0 kislyuk    (501) staff       (20)     1311 2023-03-27 05:42:23.000000 aegea-4.3.4/Makefile
--rw-r--r--   0 kislyuk    (501) staff       (20)    11797 2023-04-02 15:16:06.042820 aegea-4.3.4/PKG-INFO
--rw-r--r--   0 kislyuk    (501) staff       (20)    11487 2023-04-02 15:14:35.000000 aegea-4.3.4/README.rst
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.013386 aegea-4.3.4/aegea/
--rw-r--r--   0 kislyuk    (501) staff       (20)     8094 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/__init__.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     2048 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/aegea_config.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     1771 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/alarms.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    19424 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/audit.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    16673 2022-07-01 07:15:56.000000 aegea-4.3.4/aegea/base_config.yml
--rw-r--r--   0 kislyuk    (501) staff       (20)    27543 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/batch.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     5204 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/billing.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     5174 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/build_ami.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     6148 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/build_docker_image.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     2044 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/cloudtrail.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     6915 2017-03-19 18:47:27.000000 aegea-4.3.4/aegea/constants.json
--rw-r--r--   0 kislyuk    (501) staff       (20)     5722 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/cost.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     7988 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/deploy.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    11223 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/ebs.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     3202 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/ecr.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    14413 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/ecs.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     3560 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/efs.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    11720 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/elb.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     2806 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/flow_logs.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     5587 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/iam.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     2035 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/instance_ctl.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     3158 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/lambda.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    20245 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/launch.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     7654 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/logs.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     9585 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/ls.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.014085 aegea-4.3.4/aegea/missions/
--rw-r--r--   0 kislyuk    (501) staff       (20)       13 2016-12-13 22:14:13.000000 aegea-4.3.4/aegea/missions/.gitignore
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.014923 aegea-4.3.4/aegea/missions/arvados/
--rw-r--r--   0 kislyuk    (501) staff       (20)      289 2017-01-13 19:39:20.000000 aegea-4.3.4/aegea/missions/arvados/Makefile
--rw-r--r--   0 kislyuk    (501) staff       (20)     1446 2017-01-19 22:26:48.000000 aegea-4.3.4/aegea/missions/arvados/config.yml
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     6026 2017-01-23 18:07:36.000000 aegea-4.3.4/aegea/missions/arvados/deploy-arvados.sh
--rw-r--r--   0 kislyuk    (501) staff       (20)     1641 2017-01-19 20:51:49.000000 aegea-4.3.4/aegea/missions/arvados/environment
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:05.998633 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.016492 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:05.997451 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/arvados/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.016751 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/arvados/api/
--rw-r--r--   0 kislyuk    (501) staff       (20)      407 2016-12-13 22:14:13.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/arvados/api/application.yml
--rw-r--r--   0 kislyuk    (501) staff       (20)      783 2017-01-19 19:35:43.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/arvados/api/database.yml
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.016872 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/arvados/crunch-dispatch-slurm/
--rw-r--r--   0 kislyuk    (501) staff       (20)       94 2016-12-13 22:14:13.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/arvados/crunch-dispatch-slurm/crunch-dispatch-slurm.yml
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.017004 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/arvados/docker-cleaner/
--rw-r--r--   0 kislyuk    (501) staff       (20)       77 2016-11-01 22:37:46.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/arvados/docker-cleaner/docker-cleaner.json
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.017131 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/arvados/keep-web/
--rw-r--r--   0 kislyuk    (501) staff       (20)      259 2016-11-01 22:37:46.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/arvados/keep-web/keep-web.yml
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.017259 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/arvados/keepproxy/
--rw-r--r--   0 kislyuk    (501) staff       (20)      278 2016-12-13 22:13:26.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/arvados/keepproxy/keepproxy.yml
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.017386 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/arvados/nodemanager/
--rw-r--r--   0 kislyuk    (501) staff       (20)     1230 2017-01-19 20:48:50.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/arvados/nodemanager/ec2.cfg
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.017795 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/arvados/sso/
--rw-r--r--   0 kislyuk    (501) staff       (20)      421 2016-10-14 16:17:29.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/arvados/sso/application.yml
--rw-r--r--   0 kislyuk    (501) staff       (20)      795 2017-01-19 19:35:58.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/arvados/sso/database.yml
--rw-r--r--   0 kislyuk    (501) staff       (20)      461 2016-10-14 16:17:29.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/arvados/sso/production.rb
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.017946 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/arvados/workbench/
--rw-r--r--   0 kislyuk    (501) staff       (20)      291 2016-10-17 17:18:05.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/arvados/workbench/application.yml
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.018115 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/default/
--rw-r--r--   0 kislyuk    (501) staff       (20)       19 2016-12-13 22:14:13.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/default/munge
--rw-r--r--   0 kislyuk    (501) staff       (20)       17 2016-11-01 22:37:46.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/fuse.conf
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.019835 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/init/
--rw-r--r--   0 kislyuk    (501) staff       (20)      210 2016-10-14 16:17:29.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/init/arvados-api.conf
--rw-r--r--   0 kislyuk    (501) staff       (20)      238 2016-10-14 16:17:29.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/init/arvados-keep.conf
--rw-r--r--   0 kislyuk    (501) staff       (20)       88 2016-11-01 22:37:46.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/init/arvados-keepproxy.conf
--rw-r--r--   0 kislyuk    (501) staff       (20)       92 2016-11-01 22:37:46.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/init/arvados-keepweb.conf
--rw-r--r--   0 kislyuk    (501) staff       (20)      155 2017-01-19 16:44:26.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/init/arvados-nodemanager.conf
--rw-r--r--   0 kislyuk    (501) staff       (20)      230 2016-10-14 16:17:29.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/init/awslogs.conf
--rw-r--r--   0 kislyuk    (501) staff       (20)      165 2016-12-13 22:14:13.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/init/crunch-dispatch-slurm.conf
--rw-r--r--   0 kislyuk    (501) staff       (20)        7 2017-01-23 17:03:52.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/init/crunch-dispatch-slurm.override
--rw-r--r--   0 kislyuk    (501) staff       (20)        7 2017-01-23 17:37:49.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/init/munge.override
--rw-r--r--   0 kislyuk    (501) staff       (20)        7 2017-01-23 17:37:38.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/init/slurm-llnl.override
--rw-r--r--   0 kislyuk    (501) staff       (20)        7 2016-10-14 16:17:29.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/init/squid-deb-proxy.override
--rw-r--r--   0 kislyuk    (501) staff       (20)        7 2016-10-14 16:17:29.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/init/squid3.override
--rw-r--r--   0 kislyuk    (501) staff       (20)      317 2016-12-13 22:14:13.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/keep.conf.json
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.019981 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/keepstore/
--rw-r--r--   0 kislyuk    (501) staff       (20)       26 2016-10-14 16:17:29.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/keepstore/blob-signing.key
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.020331 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/munge/
--rw-r--r--   0 kislyuk    (501) staff       (20)     1024 2016-11-01 22:37:46.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/munge/munge.key
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:05.997923 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/nginx/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.020488 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/nginx/conf.d/
--rw-r--r--   0 kislyuk    (501) staff       (20)       34 2016-10-17 16:42:52.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/nginx/conf.d/arvados
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.020698 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-available/
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2016-11-01 22:37:46.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-available/default
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.021093 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-enabled/
--rw-r--r--   0 kislyuk    (501) staff       (20)     1479 2017-01-19 19:31:32.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-enabled/arvados-api
--rw-r--r--   0 kislyuk    (501) staff       (20)      708 2017-01-19 19:32:24.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-enabled/arvados-sso
--rw-r--r--   0 kislyuk    (501) staff       (20)      638 2017-01-19 19:32:06.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-enabled/arvados-workbench
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.021236 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/profile.d/
--rw-r--r--   0 kislyuk    (501) staff       (20)       93 2016-11-01 22:37:46.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/profile.d/arvados.sh
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:05.998084 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/resolvconf/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.021376 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/resolvconf/resolv.conf.d/
--rw-r--r--   0 kislyuk    (501) staff       (20)       33 2016-12-13 22:14:13.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/resolvconf/resolv.conf.d/tail
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.021613 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/slurm-llnl/
--rw-r--r--   0 kislyuk    (501) staff       (20)       80 2016-12-13 22:14:13.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/slurm-llnl/nodes.conf
--rw-r--r--   0 kislyuk    (501) staff       (20)      882 2016-12-13 22:14:13.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/slurm-llnl/slurm.conf
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:05.998246 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/systemd/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:05.998347 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/systemd/system/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.021717 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/systemd/system/docker.service.d/
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2016-11-01 22:37:46.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/systemd/system/docker.service.d/arvados.conf
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.021820 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/systemd/system/multi-user.target.wants/
--rw-r--r--   0 kislyuk    (501) staff       (20)      730 2016-11-01 22:37:46.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/systemd/system/multi-user.target.wants/arvados-docker-cleaner.service
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:05.998443 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/mnt/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.021955 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/mnt/keep/
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2016-10-14 16:17:29.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/mnt/keep/.keep
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:05.998559 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/usr/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.022146 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/usr/bin/
--rwxr-xr-x   0 kislyuk    (501) staff       (20)      778 2016-12-13 22:14:13.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/usr/bin/aegea-set-slurm-nodes
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     1666 2017-01-19 20:26:41.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/usr/bin/init-arvados
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:05.998877 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/var/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:05.998729 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/var/lib/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:05.998774 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/var/lib/arvados/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:05.998816 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/var/lib/arvados/git/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.022284 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/var/lib/arvados/git/repositories/
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2016-10-14 16:17:29.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/var/lib/arvados/git/repositories/.keep
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:05.998918 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/var/log/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.022365 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/var/log/arvados/
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2017-01-19 16:47:27.000000 aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/var/log/arvados/.keep
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.015488 aegea-4.3.4/aegea/missions/arvados-worker/
--rw-r--r--   0 kislyuk    (501) staff       (20)      289 2017-01-13 19:39:17.000000 aegea-4.3.4/aegea/missions/arvados-worker/Makefile
--rw-r--r--   0 kislyuk    (501) staff       (20)      877 2016-12-13 22:14:13.000000 aegea-4.3.4/aegea/missions/arvados-worker/config.yml
--rw-r--r--   0 kislyuk    (501) staff       (20)     1641 2017-01-19 20:51:49.000000 aegea-4.3.4/aegea/missions/arvados-worker/environment
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:05.996780 aegea-4.3.4/aegea/missions/arvados-worker/rootfs.skel.in/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:05.996722 aegea-4.3.4/aegea/missions/arvados-worker/rootfs.skel.in/etc/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.015606 aegea-4.3.4/aegea/missions/arvados-worker/rootfs.skel.in/etc/default/
--rw-r--r--   0 kislyuk    (501) staff       (20)       19 2016-12-13 22:14:13.000000 aegea-4.3.4/aegea/missions/arvados-worker/rootfs.skel.in/etc/default/munge
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.015735 aegea-4.3.4/aegea/missions/arvados-worker/rootfs.skel.in/etc/munge/
--rw-r--r--   0 kislyuk    (501) staff       (20)     1024 2016-11-01 22:37:46.000000 aegea-4.3.4/aegea/missions/arvados-worker/rootfs.skel.in/etc/munge/munge.key
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.016046 aegea-4.3.4/aegea/missions/arvados-worker/rootfs.skel.in/etc/slurm-llnl/
--rw-r--r--   0 kislyuk    (501) staff       (20)       80 2016-12-13 22:14:13.000000 aegea-4.3.4/aegea/missions/arvados-worker/rootfs.skel.in/etc/slurm-llnl/nodes.conf
--rw-r--r--   0 kislyuk    (501) staff       (20)      882 2016-12-13 22:14:13.000000 aegea-4.3.4/aegea/missions/arvados-worker/rootfs.skel.in/etc/slurm-llnl/slurm.conf
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:05.996820 aegea-4.3.4/aegea/missions/arvados-worker/rootfs.skel.in/usr/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.016232 aegea-4.3.4/aegea/missions/arvados-worker/rootfs.skel.in/usr/bin/
--rwxr-xr-x   0 kislyuk    (501) staff       (20)      778 2016-12-13 22:14:13.000000 aegea-4.3.4/aegea/missions/arvados-worker/rootfs.skel.in/usr/bin/aegea-set-slurm-nodes
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.022460 aegea-4.3.4/aegea/missions/docker-example/
--rw-r--r--   0 kislyuk    (501) staff       (20)      224 2017-01-12 00:44:16.000000 aegea-4.3.4/aegea/missions/docker-example/config.yml
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:05.999073 aegea-4.3.4/aegea/missions/docker-example/rootfs.skel/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:05.999112 aegea-4.3.4/aegea/missions/docker-example/rootfs.skel/etc/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.022780 aegea-4.3.4/aegea/missions/docker-example/rootfs.skel/etc/update-motd.d/
--rwxr-xr-x   0 kislyuk    (501) staff       (20)      214 2017-01-10 17:44:55.000000 aegea-4.3.4/aegea/missions/docker-example/rootfs.skel/etc/update-motd.d/aegea-motd
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.023345 aegea-4.3.4/aegea/missions/ecs-container-instance/
--rw-r--r--   0 kislyuk    (501) staff       (20)      437 2019-10-14 14:47:55.000000 aegea-4.3.4/aegea/missions/ecs-container-instance/Makefile
--rw-r--r--   0 kislyuk    (501) staff       (20)      632 2019-10-14 14:47:55.000000 aegea-4.3.4/aegea/missions/ecs-container-instance/config.yml
--rw-r--r--   0 kislyuk    (501) staff       (20)      355 2019-10-14 14:47:55.000000 aegea-4.3.4/aegea/missions/ecs-container-instance/environment
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:05.999292 aegea-4.3.4/aegea/missions/ecs-container-instance/rootfs.skel.in/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:05.999333 aegea-4.3.4/aegea/missions/ecs-container-instance/rootfs.skel.in/etc/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.023543 aegea-4.3.4/aegea/missions/ecs-container-instance/rootfs.skel.in/etc/ecs/
--rw-r--r--   0 kislyuk    (501) staff       (20)       55 2019-10-14 14:47:55.000000 aegea-4.3.4/aegea/missions/ecs-container-instance/rootfs.skel.in/etc/ecs/ecs.config
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.024319 aegea-4.3.4/aegea/missions/fog-dog/
--rw-r--r--   0 kislyuk    (501) staff       (20)      285 2017-01-13 19:38:03.000000 aegea-4.3.4/aegea/missions/fog-dog/Makefile
--rw-r--r--   0 kislyuk    (501) staff       (20)     1365 2017-02-02 23:31:30.000000 aegea-4.3.4/aegea/missions/fog-dog/config.yml
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2016-12-13 22:14:13.000000 aegea-4.3.4/aegea/missions/fog-dog/environment
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:05.999499 aegea-4.3.4/aegea/missions/fog-dog/rootfs.skel.in/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:05.999541 aegea-4.3.4/aegea/missions/fog-dog/rootfs.skel.in/etc/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.024446 aegea-4.3.4/aegea/missions/fog-dog/rootfs.skel.in/etc/update-motd.d/
--rwxr-xr-x   0 kislyuk    (501) staff       (20)      219 2016-12-13 22:14:13.000000 aegea-4.3.4/aegea/missions/fog-dog/rootfs.skel.in/etc/update-motd.d/fogdog-motd
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.024639 aegea-4.3.4/aegea/missions/ubuntu-14.04/
--rw-r--r--   0 kislyuk    (501) staff       (20)      112 2016-10-14 16:17:29.000000 aegea-4.3.4/aegea/missions/ubuntu-14.04/config.yml
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:05.999707 aegea-4.3.4/aegea/missions/ubuntu-14.04/rootfs.skel/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:05.999747 aegea-4.3.4/aegea/missions/ubuntu-14.04/rootfs.skel/etc/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.024836 aegea-4.3.4/aegea/missions/ubuntu-14.04/rootfs.skel/etc/init/
--rw-r--r--   0 kislyuk    (501) staff       (20)      230 2016-10-14 16:17:29.000000 aegea-4.3.4/aegea/missions/ubuntu-14.04/rootfs.skel/etc/init/awslogs.conf
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.025003 aegea-4.3.4/aegea/packages/
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2017-02-02 20:27:09.000000 aegea-4.3.4/aegea/packages/__init__.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.028549 aegea-4.3.4/aegea/packages/github3/
--rw-r--r--   0 kislyuk    (501) staff       (20)      501 2023-03-27 05:42:23.000000 aegea-4.3.4/aegea/packages/github3/__init__.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    22413 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/api.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     3152 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/auths.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     3148 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/decorators.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     5672 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/events.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.029560 aegea-4.3.4/aegea/packages/github3/gists/
--rw-r--r--   0 kislyuk    (501) staff       (20)      293 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/gists/__init__.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      987 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/gists/comment.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     1089 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/gists/file.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     8540 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/gists/gist.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     1817 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/gists/history.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     6891 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/git.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    62195 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/github.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.030493 aegea-4.3.4/aegea/packages/github3/issues/
--rw-r--r--   0 kislyuk    (501) staff       (20)      810 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/issues/__init__.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      956 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/issues/comment.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     2095 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/issues/event.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    11104 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/issues/issue.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     1645 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/issues/label.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     3658 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/issues/milestone.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    13394 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/models.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     5302 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/notifications.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    20641 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/orgs.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    16290 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/pulls.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.032686 aegea-4.3.4/aegea/packages/github3/repos/
--rw-r--r--   0 kislyuk    (501) staff       (20)      199 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/repos/__init__.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      909 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/repos/branch.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     2138 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/repos/comment.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     2514 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/repos/commit.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     2705 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/repos/comparison.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     6046 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/repos/contents.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     4897 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/repos/deployment.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     3342 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/repos/hook.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     1401 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/repos/pages.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     8133 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/repos/release.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    77940 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/repos/repo.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     1475 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/repos/stats.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     1413 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/repos/status.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     1054 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/repos/tag.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.033353 aegea-4.3.4/aegea/packages/github3/search/
--rw-r--r--   0 kislyuk    (501) staff       (20)      257 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/search/__init__.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     1075 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/search/code.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      603 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/search/issue.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      642 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/search/repository.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      622 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/search/user.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     4757 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/session.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     5230 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/structs.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    15140 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/users.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     1990 2016-09-24 15:36:24.000000 aegea-4.3.4/aegea/packages/github3/utils.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     3221 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/pricing.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     5642 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/rds.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     8036 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/rm.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.002131 aegea-4.3.4/aegea/rootfs.skel.build_ami/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.033910 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.034046 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/R/
--rw-r--r--   0 kislyuk    (501) staff       (20)      100 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/R/Rprofile.site
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.000316 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/apt/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.034185 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/apt/apt.conf.d/
--rw-r--r--   0 kislyuk    (501) staff       (20)      127 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/apt/apt.conf.d/99aegea
--rw-r--r--   0 kislyuk    (501) staff       (20)       71 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/aws.conf
--rw-r--r--   0 kislyuk    (501) staff       (20)      449 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/awslogs.conf
--rw-r--r--   0 kislyuk    (501) staff       (20)      672 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/awslogs.logging.conf
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.000424 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/cloud/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.034434 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/cloud/cloud.cfg.d/
--rw-r--r--   0 kislyuk    (501) staff       (20)       25 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/cloud/cloud.cfg.d/90_dpkg.cfg
--rw-r--r--   0 kislyuk    (501) staff       (20)      546 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/cloud/cloud.cfg.d/99_aegea.cfg
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.034685 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/default/
--rw-r--r--   0 kislyuk    (501) staff       (20)       10 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/default/apport
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.034819 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/default/grub.d/
--rw-r--r--   0 kislyuk    (501) staff       (20)      127 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/default/grub.d/99aegea.cfg
--rw-r--r--   0 kislyuk    (501) staff       (20)       35 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/default/mdadm
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.034943 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/ecs/
--rw-r--r--   0 kislyuk    (501) staff       (20)      101 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/ecs/ecs.config
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.000821 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/fail2ban/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.035066 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/fail2ban/jail.d/
--rw-r--r--   0 kislyuk    (501) staff       (20)       21 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/fail2ban/jail.d/aegea.conf
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.035189 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/logrotate.d/
--rw-r--r--   0 kislyuk    (501) staff       (20)      216 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/logrotate.d/awslogs
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.035324 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/profile.d/
--rw-r--r--   0 kislyuk    (501) staff       (20)      174 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/profile.d/aegea.sh
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.001183 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/security/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.035455 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/security/limits.d/
--rw-r--r--   0 kislyuk    (501) staff       (20)       56 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/security/limits.d/aegea.conf
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.035572 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/ssh/
--rw-r--r--   0 kislyuk    (501) staff       (20)      392 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/ssh/ssh_known_hosts
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.035701 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/sudoers.d/
--rw-r--r--   0 kislyuk    (501) staff       (20)       68 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/sudoers.d/99-aegea
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.035966 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/sysctl.d/
--rw-r--r--   0 kislyuk    (501) staff       (20)      558 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/sysctl.d/90-netflix-tunables.conf
--rw-r--r--   0 kislyuk    (501) staff       (20)       37 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/sysctl.d/91-aegea.conf
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.001533 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/systemd/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.001590 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/systemd/system/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.036094 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/systemd/system/docker.service.d/
--rw-r--r--   0 kislyuk    (501) staff       (20)      383 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/systemd/system/docker.service.d/xb.conf
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.001729 aegea-4.3.4/aegea/rootfs.skel.build_ami/lib/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.001786 aegea-4.3.4/aegea/rootfs.skel.build_ami/lib/systemd/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.036867 aegea-4.3.4/aegea/rootfs.skel.build_ami/lib/systemd/system/
--rw-r--r--   0 kislyuk    (501) staff       (20)      301 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/lib/systemd/system/aegea-deploy@.service
--rw-r--r--   0 kislyuk    (501) staff       (20)      257 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/lib/systemd/system/awslogs.service
--rw-r--r--   0 kislyuk    (501) staff       (20)      236 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/lib/systemd/system/docker-event-relay.service
--rw-r--r--   0 kislyuk    (501) staff       (20)     1183 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/lib/systemd/system/ecs.service
--rw-r--r--   0 kislyuk    (501) staff       (20)      221 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/lib/systemd/system/efs.service
--rw-r--r--   0 kislyuk    (501) staff       (20)      190 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/lib/systemd/system/format-ephemeral-storage.service
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.001915 aegea-4.3.4/aegea/rootfs.skel.build_ami/root/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.036998 aegea-4.3.4/aegea/rootfs.skel.build_ami/root/.aws/
--rw-r--r--   0 kislyuk    (501) staff       (20)       71 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/root/.aws/config
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.002055 aegea-4.3.4/aegea/rootfs.skel.build_ami/usr/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.037764 aegea-4.3.4/aegea/rootfs.skel.build_ami/usr/bin/
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     8010 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/usr/bin/aegea-deploy-pilot
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     2476 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/usr/bin/aegea-docker-event-relay
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     3002 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/usr/bin/aegea-efs-mount
--rwxr-xr-x   0 kislyuk    (501) staff       (20)      803 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/usr/bin/aegea-format-ephemeral-storage
--rwxr-xr-x   0 kislyuk    (501) staff       (20)      927 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/usr/bin/aegea-git-ssh-helper
--rwxr-xr-x   0 kislyuk    (501) staff       (20)      432 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/usr/bin/aegea-imds
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.002267 aegea-4.3.4/aegea/rootfs.skel.build_ami/var/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.002213 aegea-4.3.4/aegea/rootfs.skel.build_ami/var/awslogs/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.037999 aegea-4.3.4/aegea/rootfs.skel.build_ami/var/awslogs/state/
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/var/awslogs/state/.keep
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.002310 aegea-4.3.4/aegea/rootfs.skel.build_ami/var/lib/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.038082 aegea-4.3.4/aegea/rootfs.skel.build_ami/var/lib/docker/
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.build_ami/var/lib/docker/.keep
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.002416 aegea-4.3.4/aegea/rootfs.skel.launch/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.002458 aegea-4.3.4/aegea/rootfs.skel.launch/var/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.002499 aegea-4.3.4/aegea/rootfs.skel.launch/var/lib/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.038163 aegea-4.3.4/aegea/rootfs.skel.launch/var/lib/aegea/
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/rootfs.skel.launch/var/lib/aegea/.keep
--rw-r--r--   0 kislyuk    (501) staff       (20)     7747 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/s3.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     6134 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/secrets.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     7737 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/sfn.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    15928 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/ssh.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     1390 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/top.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      370 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/user_config.yml
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.039372 aegea-4.3.4/aegea/util/
--rw-r--r--   0 kislyuk    (501) staff       (20)     5804 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/util/__init__.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.040652 aegea-4.3.4/aegea/util/aws/
--rw-r--r--   0 kislyuk    (501) staff       (20)    25413 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/util/aws/__init__.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     1201 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/util/aws/_boto3_loader.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    14524 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/util/aws/batch.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.040991 aegea-4.3.4/aegea/util/aws/batch_events_lambda/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.041372 aegea-4.3.4/aegea/util/aws/batch_events_lambda/.chalice/
--rw-r--r--   0 kislyuk    (501) staff       (20)      286 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/util/aws/batch_events_lambda/.chalice/config.json
--rw-r--r--   0 kislyuk    (501) staff       (20)      486 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/util/aws/batch_events_lambda/.chalice/policy-dev.json
--rw-r--r--   0 kislyuk    (501) staff       (20)       37 2022-07-01 05:40:57.000000 aegea-4.3.4/aegea/util/aws/batch_events_lambda/.gitignore
--rw-r--r--   0 kislyuk    (501) staff       (20)      984 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/util/aws/batch_events_lambda/app.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      172 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/util/aws/clients.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     3608 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/util/aws/dns.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     7268 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/util/aws/iam.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     7986 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/util/aws/logs.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      176 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/util/aws/resources.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     4389 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/util/aws/spot.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     6390 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/util/aws/ssm.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     7568 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/util/cloudinit.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     1079 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/util/constants.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     2851 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/util/crypto.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      143 2016-08-15 17:20:25.000000 aegea-4.3.4/aegea/util/exceptions.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     1372 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/util/git.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    10911 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/util/printing.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      799 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/util/ssh.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      160 2023-04-02 15:16:05.000000 aegea-4.3.4/aegea/version.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     2241 2023-01-09 03:46:45.000000 aegea-4.3.4/aegea/zones.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.013987 aegea-4.3.4/aegea.egg-info/
--rw-r--r--   0 kislyuk    (501) staff       (20)    11797 2023-04-02 15:16:05.000000 aegea-4.3.4/aegea.egg-info/PKG-INFO
--rw-r--r--   0 kislyuk    (501) staff       (20)     9721 2023-04-02 15:16:05.000000 aegea-4.3.4/aegea.egg-info/SOURCES.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)        1 2023-04-02 15:16:05.000000 aegea-4.3.4/aegea.egg-info/dependency_links.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)      295 2023-04-02 15:16:05.000000 aegea-4.3.4/aegea.egg-info/requires.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)        6 2023-04-02 15:16:05.000000 aegea-4.3.4/aegea.egg-info/top_level.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)     1899 2023-03-27 05:22:54.000000 aegea-4.3.4/common.mk
--rw-r--r--   0 kislyuk    (501) staff       (20)      431 2022-07-01 05:40:57.000000 aegea-4.3.4/mypy.ini
--rw-r--r--   0 kislyuk    (501) staff       (20)      328 2023-03-27 05:42:23.000000 aegea-4.3.4/pyproject.toml
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.042142 aegea-4.3.4/scripts/
--rwxr-xr-x   0 kislyuk    (501) staff       (20)      535 2022-07-01 05:40:57.000000 aegea-4.3.4/scripts/aegea
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     1603 2022-07-01 05:40:57.000000 aegea-4.3.4/scripts/aegea-build-image-for-mission
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     2971 2022-07-01 05:40:57.000000 aegea-4.3.4/scripts/aegea-rebuild-public-elb-sg
--rw-r--r--   0 kislyuk    (501) staff       (20)      529 2022-07-01 05:40:57.000000 aegea-4.3.4/scripts/aegea-ssh
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     2058 2022-07-01 05:40:57.000000 aegea-4.3.4/scripts/pypi-apt-freeze
--rw-r--r--   0 kislyuk    (501) staff       (20)       38 2023-04-02 15:16:06.043051 aegea-4.3.4/setup.cfg
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     1317 2023-03-27 05:42:23.000000 aegea-4.3.4/setup.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-02 15:16:06.042554 aegea-4.3.4/test/
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2016-06-14 14:20:19.000000 aegea-4.3.4/test/__init__.py
--rwxr-xr-x   0 kislyuk    (501) staff       (20)    19282 2022-07-01 05:40:57.000000 aegea-4.3.4/test/test.py
--rw-r--r--   0 kislyuk    (501) staff       (20)       71 2022-07-01 05:40:57.000000 aegea-4.3.4/test/test.wdl
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.206467 aegea-4.4.0/
+-rw-r--r--   0 kislyuk    (501) staff       (20)       44 2022-07-01 05:40:57.000000 aegea-4.4.0/.coveragerc
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.160079 aegea-4.4.0/.github/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.173805 aegea-4.4.0/.github/workflows/
+-rw-r--r--   0 kislyuk    (501) staff       (20)     1251 2023-03-27 05:42:23.000000 aegea-4.4.0/.github/workflows/ci.yml
+-rw-r--r--   0 kislyuk    (501) staff       (20)      518 2022-07-01 05:40:57.000000 aegea-4.4.0/.gitignore
+-rw-r--r--   0 kislyuk    (501) staff       (20)    36433 2023-04-22 02:27:44.000000 aegea-4.4.0/Changes.rst
+-rw-r--r--   0 kislyuk    (501) staff       (20)    11357 2016-06-14 14:20:08.000000 aegea-4.4.0/LICENSE.md
+-rw-r--r--   0 kislyuk    (501) staff       (20)      188 2022-07-01 05:40:57.000000 aegea-4.4.0/MANIFEST.in
+-rw-r--r--   0 kislyuk    (501) staff       (20)     1311 2023-03-27 05:42:23.000000 aegea-4.4.0/Makefile
+-rw-r--r--   0 kislyuk    (501) staff       (20)    11797 2023-04-22 02:28:03.206552 aegea-4.4.0/PKG-INFO
+-rw-r--r--   0 kislyuk    (501) staff       (20)    11487 2023-04-02 15:14:35.000000 aegea-4.4.0/README.rst
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.180224 aegea-4.4.0/aegea/
+-rw-r--r--   0 kislyuk    (501) staff       (20)     8094 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/__init__.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     2048 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/aegea_config.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     1771 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/alarms.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)    19424 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/audit.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)    16677 2023-04-22 01:58:54.000000 aegea-4.4.0/aegea/base_config.yml
+-rw-r--r--   0 kislyuk    (501) staff       (20)    27543 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/batch.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     5204 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/billing.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     5174 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/build_ami.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     6148 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/build_docker_image.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     2044 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/cloudtrail.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     6915 2017-03-19 18:47:27.000000 aegea-4.4.0/aegea/constants.json
+-rw-r--r--   0 kislyuk    (501) staff       (20)     5722 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/cost.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)    11223 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/ebs.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     3202 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/ecr.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)    14413 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/ecs.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     3560 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/efs.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)    11720 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/elb.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     2806 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/flow_logs.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     5587 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/iam.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     2035 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/instance_ctl.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     3158 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/lambda.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)    20335 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/launch.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     7654 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/logs.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     9585 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/ls.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.180933 aegea-4.4.0/aegea/missions/
+-rw-r--r--   0 kislyuk    (501) staff       (20)       13 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/.gitignore
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.181806 aegea-4.4.0/aegea/missions/arvados/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      289 2017-01-13 19:39:20.000000 aegea-4.4.0/aegea/missions/arvados/Makefile
+-rw-r--r--   0 kislyuk    (501) staff       (20)     1446 2017-01-19 22:26:48.000000 aegea-4.4.0/aegea/missions/arvados/config.yml
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)     6026 2017-01-23 18:07:36.000000 aegea-4.4.0/aegea/missions/arvados/deploy-arvados.sh
+-rw-r--r--   0 kislyuk    (501) staff       (20)     1641 2017-01-19 20:51:49.000000 aegea-4.4.0/aegea/missions/arvados/environment
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.166937 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.183486 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.165809 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.183769 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/api/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      407 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/api/application.yml
+-rw-r--r--   0 kislyuk    (501) staff       (20)      783 2017-01-19 19:35:43.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/api/database.yml
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.183905 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/crunch-dispatch-slurm/
+-rw-r--r--   0 kislyuk    (501) staff       (20)       94 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/crunch-dispatch-slurm/crunch-dispatch-slurm.yml
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.184069 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/docker-cleaner/
+-rw-r--r--   0 kislyuk    (501) staff       (20)       77 2016-11-01 22:37:46.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/docker-cleaner/docker-cleaner.json
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.184221 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/keep-web/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      259 2016-11-01 22:37:46.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/keep-web/keep-web.yml
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.184360 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/keepproxy/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      278 2016-12-13 22:13:26.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/keepproxy/keepproxy.yml
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.184490 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/nodemanager/
+-rw-r--r--   0 kislyuk    (501) staff       (20)     1230 2017-01-19 20:48:50.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/nodemanager/ec2.cfg
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.189367 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/sso/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      421 2016-10-14 16:17:29.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/sso/application.yml
+-rw-r--r--   0 kislyuk    (501) staff       (20)      795 2017-01-19 19:35:58.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/sso/database.yml
+-rw-r--r--   0 kislyuk    (501) staff       (20)      461 2016-10-14 16:17:29.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/sso/production.rb
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.189506 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/workbench/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      291 2016-10-17 17:18:05.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/workbench/application.yml
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.189633 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/default/
+-rw-r--r--   0 kislyuk    (501) staff       (20)       19 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/default/munge
+-rw-r--r--   0 kislyuk    (501) staff       (20)       17 2016-11-01 22:37:46.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/fuse.conf
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.191177 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/init/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      210 2016-10-14 16:17:29.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/init/arvados-api.conf
+-rw-r--r--   0 kislyuk    (501) staff       (20)      238 2016-10-14 16:17:29.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/init/arvados-keep.conf
+-rw-r--r--   0 kislyuk    (501) staff       (20)       88 2016-11-01 22:37:46.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/init/arvados-keepproxy.conf
+-rw-r--r--   0 kislyuk    (501) staff       (20)       92 2016-11-01 22:37:46.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/init/arvados-keepweb.conf
+-rw-r--r--   0 kislyuk    (501) staff       (20)      155 2017-01-19 16:44:26.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/init/arvados-nodemanager.conf
+-rw-r--r--   0 kislyuk    (501) staff       (20)      230 2016-10-14 16:17:29.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/init/awslogs.conf
+-rw-r--r--   0 kislyuk    (501) staff       (20)      165 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/init/crunch-dispatch-slurm.conf
+-rw-r--r--   0 kislyuk    (501) staff       (20)        7 2017-01-23 17:03:52.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/init/crunch-dispatch-slurm.override
+-rw-r--r--   0 kislyuk    (501) staff       (20)        7 2017-01-23 17:37:49.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/init/munge.override
+-rw-r--r--   0 kislyuk    (501) staff       (20)        7 2017-01-23 17:37:38.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/init/slurm-llnl.override
+-rw-r--r--   0 kislyuk    (501) staff       (20)        7 2016-10-14 16:17:29.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/init/squid-deb-proxy.override
+-rw-r--r--   0 kislyuk    (501) staff       (20)        7 2016-10-14 16:17:29.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/init/squid3.override
+-rw-r--r--   0 kislyuk    (501) staff       (20)      317 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/keep.conf.json
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.191308 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/keepstore/
+-rw-r--r--   0 kislyuk    (501) staff       (20)       26 2016-10-14 16:17:29.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/keepstore/blob-signing.key
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.191428 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/munge/
+-rw-r--r--   0 kislyuk    (501) staff       (20)     1024 2016-11-01 22:37:46.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/munge/munge.key
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.166255 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/nginx/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.191530 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/nginx/conf.d/
+-rw-r--r--   0 kislyuk    (501) staff       (20)       34 2016-10-17 16:42:52.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/nginx/conf.d/arvados
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.191653 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-available/
+-rw-r--r--   0 kislyuk    (501) staff       (20)        0 2016-11-01 22:37:46.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-available/default
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.191978 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-enabled/
+-rw-r--r--   0 kislyuk    (501) staff       (20)     1479 2017-01-19 19:31:32.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-enabled/arvados-api
+-rw-r--r--   0 kislyuk    (501) staff       (20)      708 2017-01-19 19:32:24.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-enabled/arvados-sso
+-rw-r--r--   0 kislyuk    (501) staff       (20)      638 2017-01-19 19:32:06.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-enabled/arvados-workbench
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.192096 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/profile.d/
+-rw-r--r--   0 kislyuk    (501) staff       (20)       93 2016-11-01 22:37:46.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/profile.d/arvados.sh
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.166420 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/resolvconf/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.192238 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/resolvconf/resolv.conf.d/
+-rw-r--r--   0 kislyuk    (501) staff       (20)       33 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/resolvconf/resolv.conf.d/tail
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.192450 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/slurm-llnl/
+-rw-r--r--   0 kislyuk    (501) staff       (20)       80 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/slurm-llnl/nodes.conf
+-rw-r--r--   0 kislyuk    (501) staff       (20)      882 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/slurm-llnl/slurm.conf
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.166578 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/systemd/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.166678 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/systemd/system/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.192550 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/systemd/system/docker.service.d/
+-rw-r--r--   0 kislyuk    (501) staff       (20)        0 2016-11-01 22:37:46.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/systemd/system/docker.service.d/arvados.conf
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.192639 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/systemd/system/multi-user.target.wants/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      730 2016-11-01 22:37:46.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/systemd/system/multi-user.target.wants/arvados-docker-cleaner.service
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.166778 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/mnt/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.192777 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/mnt/keep/
+-rw-r--r--   0 kislyuk    (501) staff       (20)        0 2016-10-14 16:17:29.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/mnt/keep/.keep
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.166875 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/usr/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.192950 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/usr/bin/
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)      778 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/usr/bin/aegea-set-slurm-nodes
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)     1666 2017-01-19 20:26:41.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/usr/bin/init-arvados
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.167162 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/var/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.167017 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/var/lib/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.167057 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/var/lib/arvados/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.167101 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/var/lib/arvados/git/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.193076 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/var/lib/arvados/git/repositories/
+-rw-r--r--   0 kislyuk    (501) staff       (20)        0 2016-10-14 16:17:29.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/var/lib/arvados/git/repositories/.keep
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.167205 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/var/log/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.193162 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/var/log/arvados/
+-rw-r--r--   0 kislyuk    (501) staff       (20)        0 2017-01-19 16:47:27.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/var/log/arvados/.keep
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.182376 aegea-4.4.0/aegea/missions/arvados-worker/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      289 2017-01-13 19:39:17.000000 aegea-4.4.0/aegea/missions/arvados-worker/Makefile
+-rw-r--r--   0 kislyuk    (501) staff       (20)      877 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/arvados-worker/config.yml
+-rw-r--r--   0 kislyuk    (501) staff       (20)     1641 2017-01-19 20:51:49.000000 aegea-4.4.0/aegea/missions/arvados-worker/environment
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.160682 aegea-4.4.0/aegea/missions/arvados-worker/rootfs.skel.in/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.160626 aegea-4.4.0/aegea/missions/arvados-worker/rootfs.skel.in/etc/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.182483 aegea-4.4.0/aegea/missions/arvados-worker/rootfs.skel.in/etc/default/
+-rw-r--r--   0 kislyuk    (501) staff       (20)       19 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/arvados-worker/rootfs.skel.in/etc/default/munge
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.182613 aegea-4.4.0/aegea/missions/arvados-worker/rootfs.skel.in/etc/munge/
+-rw-r--r--   0 kislyuk    (501) staff       (20)     1024 2016-11-01 22:37:46.000000 aegea-4.4.0/aegea/missions/arvados-worker/rootfs.skel.in/etc/munge/munge.key
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.182994 aegea-4.4.0/aegea/missions/arvados-worker/rootfs.skel.in/etc/slurm-llnl/
+-rw-r--r--   0 kislyuk    (501) staff       (20)       80 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/arvados-worker/rootfs.skel.in/etc/slurm-llnl/nodes.conf
+-rw-r--r--   0 kislyuk    (501) staff       (20)      882 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/arvados-worker/rootfs.skel.in/etc/slurm-llnl/slurm.conf
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.160721 aegea-4.4.0/aegea/missions/arvados-worker/rootfs.skel.in/usr/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.183191 aegea-4.4.0/aegea/missions/arvados-worker/rootfs.skel.in/usr/bin/
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)      778 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/arvados-worker/rootfs.skel.in/usr/bin/aegea-set-slurm-nodes
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.193247 aegea-4.4.0/aegea/missions/docker-example/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      224 2017-01-12 00:44:16.000000 aegea-4.4.0/aegea/missions/docker-example/config.yml
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.167366 aegea-4.4.0/aegea/missions/docker-example/rootfs.skel/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.167407 aegea-4.4.0/aegea/missions/docker-example/rootfs.skel/etc/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.193459 aegea-4.4.0/aegea/missions/docker-example/rootfs.skel/etc/update-motd.d/
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)      214 2017-01-10 17:44:55.000000 aegea-4.4.0/aegea/missions/docker-example/rootfs.skel/etc/update-motd.d/aegea-motd
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.193951 aegea-4.4.0/aegea/missions/ecs-container-instance/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      437 2019-10-14 14:47:55.000000 aegea-4.4.0/aegea/missions/ecs-container-instance/Makefile
+-rw-r--r--   0 kislyuk    (501) staff       (20)      632 2019-10-14 14:47:55.000000 aegea-4.4.0/aegea/missions/ecs-container-instance/config.yml
+-rw-r--r--   0 kislyuk    (501) staff       (20)      355 2019-10-14 14:47:55.000000 aegea-4.4.0/aegea/missions/ecs-container-instance/environment
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.167575 aegea-4.4.0/aegea/missions/ecs-container-instance/rootfs.skel.in/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.167619 aegea-4.4.0/aegea/missions/ecs-container-instance/rootfs.skel.in/etc/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.194077 aegea-4.4.0/aegea/missions/ecs-container-instance/rootfs.skel.in/etc/ecs/
+-rw-r--r--   0 kislyuk    (501) staff       (20)       55 2019-10-14 14:47:55.000000 aegea-4.4.0/aegea/missions/ecs-container-instance/rootfs.skel.in/etc/ecs/ecs.config
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.194519 aegea-4.4.0/aegea/missions/fog-dog/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      285 2017-01-13 19:38:03.000000 aegea-4.4.0/aegea/missions/fog-dog/Makefile
+-rw-r--r--   0 kislyuk    (501) staff       (20)     1365 2017-02-02 23:31:30.000000 aegea-4.4.0/aegea/missions/fog-dog/config.yml
+-rw-r--r--   0 kislyuk    (501) staff       (20)        0 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/fog-dog/environment
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.167807 aegea-4.4.0/aegea/missions/fog-dog/rootfs.skel.in/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.167860 aegea-4.4.0/aegea/missions/fog-dog/rootfs.skel.in/etc/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.194612 aegea-4.4.0/aegea/missions/fog-dog/rootfs.skel.in/etc/update-motd.d/
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)      219 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/fog-dog/rootfs.skel.in/etc/update-motd.d/fogdog-motd
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.194736 aegea-4.4.0/aegea/missions/ubuntu-14.04/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      112 2016-10-14 16:17:29.000000 aegea-4.4.0/aegea/missions/ubuntu-14.04/config.yml
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.168041 aegea-4.4.0/aegea/missions/ubuntu-14.04/rootfs.skel/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.168085 aegea-4.4.0/aegea/missions/ubuntu-14.04/rootfs.skel/etc/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.194858 aegea-4.4.0/aegea/missions/ubuntu-14.04/rootfs.skel/etc/init/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      230 2016-10-14 16:17:29.000000 aegea-4.4.0/aegea/missions/ubuntu-14.04/rootfs.skel/etc/init/awslogs.conf
+-rw-r--r--   0 kislyuk    (501) staff       (20)     3221 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/pricing.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     5642 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/rds.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     8036 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/rm.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.170179 aegea-4.4.0/aegea/rootfs.skel.build_ami/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.195392 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.195510 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/R/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      100 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/R/Rprofile.site
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.168348 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/apt/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.195660 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/apt/apt.conf.d/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      127 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/apt/apt.conf.d/99aegea
+-rw-r--r--   0 kislyuk    (501) staff       (20)       71 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/aws.conf
+-rw-r--r--   0 kislyuk    (501) staff       (20)      449 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/awslogs.conf
+-rw-r--r--   0 kislyuk    (501) staff       (20)      672 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/awslogs.logging.conf
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.168448 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/cloud/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.196011 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/cloud/cloud.cfg.d/
+-rw-r--r--   0 kislyuk    (501) staff       (20)       25 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/cloud/cloud.cfg.d/90_dpkg.cfg
+-rw-r--r--   0 kislyuk    (501) staff       (20)      546 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/cloud/cloud.cfg.d/99_aegea.cfg
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.196328 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/default/
+-rw-r--r--   0 kislyuk    (501) staff       (20)       10 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/default/apport
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.196494 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/default/grub.d/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      127 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/default/grub.d/99aegea.cfg
+-rw-r--r--   0 kislyuk    (501) staff       (20)       35 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/default/mdadm
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.197528 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/ecs/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      101 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/ecs/ecs.config
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.168801 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/fail2ban/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.197713 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/fail2ban/jail.d/
+-rw-r--r--   0 kislyuk    (501) staff       (20)       21 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/fail2ban/jail.d/aegea.conf
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.198001 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/logrotate.d/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      216 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/logrotate.d/awslogs
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.198163 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/profile.d/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      174 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/profile.d/aegea.sh
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.169132 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/security/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.198319 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/security/limits.d/
+-rw-r--r--   0 kislyuk    (501) staff       (20)       56 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/security/limits.d/aegea.conf
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.198484 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/ssh/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      392 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/ssh/ssh_known_hosts
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.198631 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/sudoers.d/
+-rw-r--r--   0 kislyuk    (501) staff       (20)       68 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/sudoers.d/99-aegea
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.198921 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/sysctl.d/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      558 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/sysctl.d/90-netflix-tunables.conf
+-rw-r--r--   0 kislyuk    (501) staff       (20)       37 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/sysctl.d/91-aegea.conf
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.169526 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/systemd/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.169579 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/systemd/system/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.199064 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/systemd/system/docker.service.d/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      383 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/systemd/system/docker.service.d/xb.conf
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.169708 aegea-4.4.0/aegea/rootfs.skel.build_ami/lib/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.169781 aegea-4.4.0/aegea/rootfs.skel.build_ami/lib/systemd/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.199962 aegea-4.4.0/aegea/rootfs.skel.build_ami/lib/systemd/system/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      301 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/lib/systemd/system/aegea-deploy@.service
+-rw-r--r--   0 kislyuk    (501) staff       (20)      257 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/lib/systemd/system/awslogs.service
+-rw-r--r--   0 kislyuk    (501) staff       (20)      236 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/lib/systemd/system/docker-event-relay.service
+-rw-r--r--   0 kislyuk    (501) staff       (20)     1183 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/lib/systemd/system/ecs.service
+-rw-r--r--   0 kislyuk    (501) staff       (20)      221 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/lib/systemd/system/efs.service
+-rw-r--r--   0 kislyuk    (501) staff       (20)      190 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/lib/systemd/system/format-ephemeral-storage.service
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.169944 aegea-4.4.0/aegea/rootfs.skel.build_ami/root/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.200105 aegea-4.4.0/aegea/rootfs.skel.build_ami/root/.aws/
+-rw-r--r--   0 kislyuk    (501) staff       (20)       71 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/root/.aws/config
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.170081 aegea-4.4.0/aegea/rootfs.skel.build_ami/usr/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.200903 aegea-4.4.0/aegea/rootfs.skel.build_ami/usr/bin/
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)     8010 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/usr/bin/aegea-deploy-pilot
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)     2476 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/usr/bin/aegea-docker-event-relay
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)     3002 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/usr/bin/aegea-efs-mount
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)      803 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/usr/bin/aegea-format-ephemeral-storage
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)      927 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/usr/bin/aegea-git-ssh-helper
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)      432 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/usr/bin/aegea-imds
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.170415 aegea-4.4.0/aegea/rootfs.skel.build_ami/var/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.170338 aegea-4.4.0/aegea/rootfs.skel.build_ami/var/awslogs/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.201083 aegea-4.4.0/aegea/rootfs.skel.build_ami/var/awslogs/state/
+-rw-r--r--   0 kislyuk    (501) staff       (20)        0 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/var/awslogs/state/.keep
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.170473 aegea-4.4.0/aegea/rootfs.skel.build_ami/var/lib/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.201172 aegea-4.4.0/aegea/rootfs.skel.build_ami/var/lib/docker/
+-rw-r--r--   0 kislyuk    (501) staff       (20)        0 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/var/lib/docker/.keep
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.170658 aegea-4.4.0/aegea/rootfs.skel.launch/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.170908 aegea-4.4.0/aegea/rootfs.skel.launch/var/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.170967 aegea-4.4.0/aegea/rootfs.skel.launch/var/lib/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.201274 aegea-4.4.0/aegea/rootfs.skel.launch/var/lib/aegea/
+-rw-r--r--   0 kislyuk    (501) staff       (20)        0 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.launch/var/lib/aegea/.keep
+-rw-r--r--   0 kislyuk    (501) staff       (20)     7747 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/s3.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     6134 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/secrets.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     7737 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/sfn.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)    15928 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/ssh.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     1390 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/top.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)      370 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/user_config.yml
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.202390 aegea-4.4.0/aegea/util/
+-rw-r--r--   0 kislyuk    (501) staff       (20)     5804 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/util/__init__.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.204066 aegea-4.4.0/aegea/util/aws/
+-rw-r--r--   0 kislyuk    (501) staff       (20)    25319 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/util/aws/__init__.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     1201 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/util/aws/_boto3_loader.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)    14524 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/util/aws/batch.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.204512 aegea-4.4.0/aegea/util/aws/batch_events_lambda/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.204861 aegea-4.4.0/aegea/util/aws/batch_events_lambda/.chalice/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      286 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/util/aws/batch_events_lambda/.chalice/config.json
+-rw-r--r--   0 kislyuk    (501) staff       (20)      486 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/util/aws/batch_events_lambda/.chalice/policy-dev.json
+-rw-r--r--   0 kislyuk    (501) staff       (20)       37 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/util/aws/batch_events_lambda/.gitignore
+-rw-r--r--   0 kislyuk    (501) staff       (20)      984 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/util/aws/batch_events_lambda/app.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)      172 2023-01-09 03:46:45.000000 aegea-4.4.0/aegea/util/aws/clients.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     3608 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/util/aws/dns.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     7268 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/util/aws/iam.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     7986 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/util/aws/logs.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)      176 2023-01-09 03:46:45.000000 aegea-4.4.0/aegea/util/aws/resources.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     4389 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/util/aws/spot.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     6385 2023-04-22 02:17:51.000000 aegea-4.4.0/aegea/util/aws/ssm.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     7568 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/util/cloudinit.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     1079 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/util/constants.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     2851 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/util/crypto.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)      143 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/util/exceptions.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)    10911 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/util/printing.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)      799 2023-01-09 03:46:45.000000 aegea-4.4.0/aegea/util/ssh.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)      160 2023-04-22 02:28:03.000000 aegea-4.4.0/aegea/version.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     2241 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/zones.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.180829 aegea-4.4.0/aegea.egg-info/
+-rw-r--r--   0 kislyuk    (501) staff       (20)    11797 2023-04-22 02:28:03.000000 aegea-4.4.0/aegea.egg-info/PKG-INFO
+-rw-r--r--   0 kislyuk    (501) staff       (20)     7972 2023-04-22 02:28:03.000000 aegea-4.4.0/aegea.egg-info/SOURCES.txt
+-rw-r--r--   0 kislyuk    (501) staff       (20)        1 2023-04-22 02:28:03.000000 aegea-4.4.0/aegea.egg-info/dependency_links.txt
+-rw-r--r--   0 kislyuk    (501) staff       (20)      295 2023-04-22 02:28:03.000000 aegea-4.4.0/aegea.egg-info/requires.txt
+-rw-r--r--   0 kislyuk    (501) staff       (20)        6 2023-04-22 02:28:03.000000 aegea-4.4.0/aegea.egg-info/top_level.txt
+-rw-r--r--   0 kislyuk    (501) staff       (20)     1899 2023-03-27 05:22:54.000000 aegea-4.4.0/common.mk
+-rw-r--r--   0 kislyuk    (501) staff       (20)      431 2022-07-01 05:40:57.000000 aegea-4.4.0/mypy.ini
+-rw-r--r--   0 kislyuk    (501) staff       (20)      328 2023-03-27 05:42:23.000000 aegea-4.4.0/pyproject.toml
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.205616 aegea-4.4.0/scripts/
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)      535 2022-07-01 05:40:57.000000 aegea-4.4.0/scripts/aegea
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)     1603 2022-07-01 05:40:57.000000 aegea-4.4.0/scripts/aegea-build-image-for-mission
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)     2971 2022-07-01 05:40:57.000000 aegea-4.4.0/scripts/aegea-rebuild-public-elb-sg
+-rw-r--r--   0 kislyuk    (501) staff       (20)      529 2022-07-01 05:40:57.000000 aegea-4.4.0/scripts/aegea-ssh
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)     2058 2022-07-01 05:40:57.000000 aegea-4.4.0/scripts/pypi-apt-freeze
+-rw-r--r--   0 kislyuk    (501) staff       (20)       38 2023-04-22 02:28:03.206806 aegea-4.4.0/setup.cfg
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)     1317 2023-04-22 01:48:30.000000 aegea-4.4.0/setup.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.206259 aegea-4.4.0/test/
+-rw-r--r--   0 kislyuk    (501) staff       (20)        0 2016-06-14 14:20:19.000000 aegea-4.4.0/test/__init__.py
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)    19641 2023-04-22 01:48:30.000000 aegea-4.4.0/test/test.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)       71 2022-07-01 05:40:57.000000 aegea-4.4.0/test/test.wdl
```

### Comparing `aegea-4.3.4/.github/workflows/ci.yml` & `aegea-4.4.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/.gitignore` & `aegea-4.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/Changes.rst` & `aegea-4.4.0/Changes.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Changes for v4.4.0 (2023-04-21)
+===============================
+
+-  aegea ssh: download correct SSM plugin
+
+-  aegea launch: use t3a.micro instance type by default
+
+-  Use Amazon Linux 2023 when specifying Amazon Linux
+
+-  Update paramiko dependency range
+
+-  Remove aegea deploy and git utils
+
 Changes for v4.3.4 (2023-04-02)
 ===============================
 
 -  Bump dependency versions
 
 -  Test and documentation infrastructure improvements
```

### Comparing `aegea-4.3.4/LICENSE.md` & `aegea-4.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/Makefile` & `aegea-4.4.0/Makefile`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/PKG-INFO` & `aegea-4.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aegea
-Version: 4.3.4
+Version: 4.4.0
 Summary: Amazon Web Services Operator Interface
 Home-page: https://github.com/kislyuk/aegea
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Platform: MacOS X
 Platform: Posix
```

### Comparing `aegea-4.3.4/README.rst` & `aegea-4.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/__init__.py` & `aegea-4.4.0/aegea/__init__.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/aegea_config.py` & `aegea-4.4.0/aegea/aegea_config.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/alarms.py` & `aegea-4.4.0/aegea/alarms.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/audit.py` & `aegea-4.4.0/aegea/audit.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/base_config.yml` & `aegea-4.4.0/aegea/base_config.yml`

 * *Files 0% similar despite different names*

```diff
@@ -710,15 +710,15 @@
     - TrailARN
     - S3BucketName
     - S3KeyPrefix
     - CloudWatchLogsLogGroupArn
     - HasCustomEventSelectors
 
 launch:
-  instance_type: t3.micro
+  instance_type: t3a.micro
   tags: []
   storage: []
   commands: []
   packages: []
   security_groups: []
   rootfs_skel_dirs:
     - auto
@@ -728,15 +728,15 @@
   iam_policies:
     - IAMReadOnlyAccess
     - AmazonEC2ContainerRegistryReadOnly
     - AmazonElasticFileSystemReadOnlyAccess
     - AmazonElasticFileSystemClientFullAccess
     - AWSOpsWorksCloudWatchLogs
     - AmazonSSMManagedInstanceCore
-  amazon_linux_release: 2
+  amazon_linux_release: 2023
 
 ssh:
   server_alive_interval: 15
   server_alive_count_max: 20
   use_kms_auth: True
 
 scp:
```

### Comparing `aegea-4.3.4/aegea/batch.py` & `aegea-4.4.0/aegea/batch.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/billing.py` & `aegea-4.4.0/aegea/billing.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/build_ami.py` & `aegea-4.4.0/aegea/build_ami.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/build_docker_image.py` & `aegea-4.4.0/aegea/build_docker_image.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/cloudtrail.py` & `aegea-4.4.0/aegea/cloudtrail.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/constants.json` & `aegea-4.4.0/aegea/constants.json`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/cost.py` & `aegea-4.4.0/aegea/cost.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/ebs.py` & `aegea-4.4.0/aegea/ebs.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/ecr.py` & `aegea-4.4.0/aegea/ecr.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/ecs.py` & `aegea-4.4.0/aegea/ecs.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/efs.py` & `aegea-4.4.0/aegea/efs.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/elb.py` & `aegea-4.4.0/aegea/elb.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/flow_logs.py` & `aegea-4.4.0/aegea/flow_logs.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/iam.py` & `aegea-4.4.0/aegea/iam.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/instance_ctl.py` & `aegea-4.4.0/aegea/instance_ctl.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/lambda.py` & `aegea-4.4.0/aegea/lambda.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/launch.py` & `aegea-4.4.0/aegea/launch.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,16 @@
                              account_id=ARN(bless_config["lambda_config"]["role_arn"]).account_id,
                              resource="secret:" + bless_config["lambda_config"]["function_name"])
     ca_keys_secret = clients.secretsmanager.get_secret_value(SecretId=str(ca_keys_secret_arn))
     ca_keys = json.loads(ca_keys_secret["SecretString"])["ssh_ca_keys"]
     return "\n".join(ca_keys)
 
 def infer_architecture(instance_type):
-    if any((instance_type.startswith(f) for f in ("x2g", "m6g", "c6g", "r6g", "t4g", "a1"))):
+    instance_family = instance_type.split(".")[0]
+    if "g" in instance_family or instance_family == "a1":
         return "arm64"
     return "x86_64"
 
 def ensure_efs_home(subnet):
     for fs in clients.efs.describe_file_systems()["FileSystems"]:
         if {"Key": "mountpoint", "Value": "/home"} in fs["Tags"]:
             for mt in paginate(clients.efs.get_paginator("describe_mount_targets"), FileSystemId=fs["FileSystemId"]):
@@ -292,15 +293,15 @@
     if args.use_dns:
         dns_zone.update(args.hostname, instance.private_dns_name)
     if args.use_imdsv2:
         clients.ec2.modify_instance_metadata_options(InstanceId=instance.id, HttpTokens="required")
     add_ssh_host_key_to_known_hosts(hostkey_line([instance.public_dns_name or instance.id], ssh_host_key))
     if args.wait_for_ssh:
         wait_for_port(instance.public_dns_name, 22)
-    logger.info("Launched %s in %s using %s (%s)", instance, subnet, args.ami, args.ami.name)
+    logger.info("Launched %s %s in %s using %s (%s)", instance.instance_type, instance, subnet, args.ami, args.ami.name)
     return dict(instance_id=instance.id)
 
 parser = register_parser(launch)
 parser.add_argument("hostname")
 parser.add_argument("--storage", nargs="+", metavar="MOUNTPOINT=SIZE_GB", type=lambda x: x.split("=", 1),
                     help="At launch time, attach EBS volume(s) of this size, format and mount them.")
 parser.add_argument("--efs-home", action="store_true",
@@ -313,16 +314,16 @@
 parser.add_argument("--bless-config", default=os.environ.get("BLESS_CONFIG"),
                     help="Path to a Bless configuration file (or pass via the BLESS_CONFIG environment variable)")
 parser.add_argument("--ami", help="AMI to use for the instance. Default: " + resolve_ami.__doc__)  # type: ignore
 parser.add_argument("--ami-tags", nargs="+", metavar="NAME=VALUE", help="Use the most recent AMI with these tags")
 parser.add_argument("--ami-tag-keys", nargs="+", default=[], metavar="TAG_NAME",
                     help="Use the most recent AMI with these tag names")
 parser.add_argument("--ubuntu-linux-ami", action="store_true", help="Use the most recent Ubuntu Linux LTS AMI")
-parser.add_argument("--amazon-linux-ami", action="store_true", help="Use the most recent Amazon Linux 2 AMI")
-parser.add_argument("--amazon-linux-release", help=argparse.SUPPRESS)
+parser.add_argument("--amazon-linux-ami", action="store_true", help="Use the most recent Amazon Linux AMI")
+parser.add_argument("--amazon-linux-release", help="Use a specific Amazon Linux release", choices={"2", "2022", "2023"})
 parser.add_argument("--spot", action="store_true",
                     help="Launch a preemptible spot instance, which is cheaper but could be forced to shut down")
 parser.add_argument("--duration-hours", type=float, help="Terminate the spot instance after this number of hours")
 parser.add_argument("--cores", type=int, help="Minimum number of cores to request (spot fleet API)")
 parser.add_argument("--min-mem-per-core-gb", type=float)
 parser.add_argument("--instance-type", "-t", help="See https://ec2instances.info/").completer = instance_type_completer
 parser.add_argument("--spot-price", type=float,
```

### Comparing `aegea-4.3.4/aegea/logs.py` & `aegea-4.4.0/aegea/logs.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/ls.py` & `aegea-4.4.0/aegea/ls.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/missions/arvados/config.yml` & `aegea-4.4.0/aegea/missions/arvados/config.yml`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/missions/arvados/deploy-arvados.sh` & `aegea-4.4.0/aegea/missions/arvados/deploy-arvados.sh`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/missions/arvados/environment` & `aegea-4.4.0/aegea/missions/arvados/environment`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/arvados/api/database.yml` & `aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/api/database.yml`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/arvados/nodemanager/ec2.cfg` & `aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/nodemanager/ec2.cfg`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/arvados/sso/database.yml` & `aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/sso/database.yml`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/munge/munge.key` & `aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/munge/munge.key`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-enabled/arvados-api` & `aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-enabled/arvados-api`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-enabled/arvados-sso` & `aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-enabled/arvados-sso`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-enabled/arvados-workbench` & `aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-enabled/arvados-workbench`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/slurm-llnl/slurm.conf` & `aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/slurm-llnl/slurm.conf`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/etc/systemd/system/multi-user.target.wants/arvados-docker-cleaner.service` & `aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/systemd/system/multi-user.target.wants/arvados-docker-cleaner.service`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/usr/bin/aegea-set-slurm-nodes` & `aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/usr/bin/aegea-set-slurm-nodes`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/missions/arvados/rootfs.skel.in/usr/bin/init-arvados` & `aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/usr/bin/init-arvados`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/missions/arvados-worker/config.yml` & `aegea-4.4.0/aegea/missions/arvados-worker/config.yml`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/missions/arvados-worker/environment` & `aegea-4.4.0/aegea/missions/arvados-worker/environment`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/missions/arvados-worker/rootfs.skel.in/etc/munge/munge.key` & `aegea-4.4.0/aegea/missions/arvados-worker/rootfs.skel.in/etc/munge/munge.key`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/missions/arvados-worker/rootfs.skel.in/etc/slurm-llnl/slurm.conf` & `aegea-4.4.0/aegea/missions/arvados-worker/rootfs.skel.in/etc/slurm-llnl/slurm.conf`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/missions/arvados-worker/rootfs.skel.in/usr/bin/aegea-set-slurm-nodes` & `aegea-4.4.0/aegea/missions/arvados-worker/rootfs.skel.in/usr/bin/aegea-set-slurm-nodes`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/missions/ecs-container-instance/config.yml` & `aegea-4.4.0/aegea/missions/ecs-container-instance/config.yml`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/missions/fog-dog/config.yml` & `aegea-4.4.0/aegea/missions/fog-dog/config.yml`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/pricing.py` & `aegea-4.4.0/aegea/pricing.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/rds.py` & `aegea-4.4.0/aegea/rds.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/rm.py` & `aegea-4.4.0/aegea/rm.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/awslogs.logging.conf` & `aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/awslogs.logging.conf`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/cloud/cloud.cfg.d/99_aegea.cfg` & `aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/cloud/cloud.cfg.d/99_aegea.cfg`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/rootfs.skel.build_ami/etc/sysctl.d/90-netflix-tunables.conf` & `aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/sysctl.d/90-netflix-tunables.conf`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/rootfs.skel.build_ami/lib/systemd/system/ecs.service` & `aegea-4.4.0/aegea/rootfs.skel.build_ami/lib/systemd/system/ecs.service`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/rootfs.skel.build_ami/usr/bin/aegea-deploy-pilot` & `aegea-4.4.0/aegea/rootfs.skel.build_ami/usr/bin/aegea-deploy-pilot`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/rootfs.skel.build_ami/usr/bin/aegea-docker-event-relay` & `aegea-4.4.0/aegea/rootfs.skel.build_ami/usr/bin/aegea-docker-event-relay`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/rootfs.skel.build_ami/usr/bin/aegea-efs-mount` & `aegea-4.4.0/aegea/rootfs.skel.build_ami/usr/bin/aegea-efs-mount`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/rootfs.skel.build_ami/usr/bin/aegea-format-ephemeral-storage` & `aegea-4.4.0/aegea/rootfs.skel.build_ami/usr/bin/aegea-format-ephemeral-storage`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/rootfs.skel.build_ami/usr/bin/aegea-git-ssh-helper` & `aegea-4.4.0/aegea/rootfs.skel.build_ami/usr/bin/aegea-git-ssh-helper`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/s3.py` & `aegea-4.4.0/aegea/s3.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/secrets.py` & `aegea-4.4.0/aegea/secrets.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/sfn.py` & `aegea-4.4.0/aegea/sfn.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/ssh.py` & `aegea-4.4.0/aegea/ssh.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/top.py` & `aegea-4.4.0/aegea/top.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/util/__init__.py` & `aegea-4.4.0/aegea/util/__init__.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/util/aws/__init__.py` & `aegea-4.4.0/aegea/util/aws/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,32 +28,32 @@
 def get_ssm_parameter(name):
     return clients.ssm.get_parameter(Name=name)["Parameter"]["Value"]
 
 def locate_ami(distribution, release, architecture):
     """
     Examples::
         locate_ami(distribution="Ubuntu", release="20.04", architecture="amd64")
-        locate_ami(distribution="Amazon Linux", release="2", architecture="arm64")
+        locate_ami(distribution="Amazon Linux", release="2023", architecture="arm64")
     """
-    if distribution == "Amazon Linux" and release in {"2", "2022"}:
+    if distribution == "Amazon Linux":
         if architecture == "amd64":
             architecture = "x86_64"
-        ssm_param_names = {
-            "2": f"/aws/service/ami-amazon-linux-latest/amzn2-ami-hvm-{architecture}-gp2",
-            "2022": f"/aws/service/ami-amazon-linux-latest/al2022-ami-kernel-default-{architecture}"
-        }
-        ami_id = clients.ssm.get_parameters(Names=[ssm_param_names[release]])["Parameters"][0]["Value"]
+        if release == "2":
+            ssm_param_name = f"/aws/service/ami-amazon-linux-latest/amzn2-ami-hvm-{architecture}-gp2"
+        else:
+            ssm_param_name = f"/aws/service/ami-amazon-linux-latest/al{release}-ami-kernel-default-{architecture}"
+        ami_id = get_ssm_parameter(ssm_param_name)
         logger.info("Found %s for %s %s %s", ami_id, distribution, release, architecture)
         return resources.ec2.Image(ami_id)
     elif distribution == "Ubuntu":
         if architecture == "x86_64":
             architecture = "amd64"
         ssm_param_name = "/aws/service/canonical/ubuntu/{product}/{release}/stable/current/{arch}/hvm/ebs-gp2/ami-id"
         ssm_param_name = ssm_param_name.format(product="server", release=release, arch=architecture)
-        ami_id = clients.ssm.get_parameters(Names=[ssm_param_name])["Parameters"][0]["Value"]
+        ami_id = get_ssm_parameter(ssm_param_name)
         logger.info("Found %s for %s %s %s", ami_id, distribution, release, architecture)
         return resources.ec2.Image(ami_id)
     raise AegeaException(f"No AMI found for {distribution} {release} {architecture}")
 
 def ensure_vpc():
     """
     If a default VPC exists in the current account/region, return it; otherwise, return the first VPC managed by aegea,
```

### Comparing `aegea-4.3.4/aegea/util/aws/_boto3_loader.py` & `aegea-4.4.0/aegea/util/aws/_boto3_loader.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/util/aws/batch.py` & `aegea-4.4.0/aegea/util/aws/batch.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/util/aws/batch_events_lambda/app.py` & `aegea-4.4.0/aegea/util/aws/batch_events_lambda/app.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/util/aws/dns.py` & `aegea-4.4.0/aegea/util/aws/dns.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/util/aws/iam.py` & `aegea-4.4.0/aegea/util/aws/iam.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/util/aws/logs.py` & `aegea-4.4.0/aegea/util/aws/logs.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/util/aws/spot.py` & `aegea-4.4.0/aegea/util/aws/spot.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/util/aws/ssm.py` & `aegea-4.4.0/aegea/util/aws/ssm.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,20 +15,24 @@
 from .. import Timestamp
 from ..exceptions import AegeaException
 from . import ARN, clients, paginate, resolve_instance_id, resources
 from .logs import CloudwatchLogReader
 
 sm_plugin_bucket = "session-manager-downloads"
 
+
 def download_session_manager_plugin_macos(target_path):
     sm_archive = io.BytesIO()
-    clients.s3.download_fileobj(sm_plugin_bucket, "plugin/latest/mac/sessionmanager-bundle.zip", sm_archive)
+    build = "mac_arm64" if platform.machine() == "arm64" else "mac"
+    path = f"plugin/latest/{build}/sessionmanager-bundle.zip"
+    clients.s3.download_fileobj(sm_plugin_bucket, path, sm_archive)
     with zipfile.ZipFile(sm_archive) as zf, open(target_path, "wb") as fh:
         fh.write(zf.read("sessionmanager-bundle/bin/session-manager-plugin"))
 
+
 def download_session_manager_plugin_linux(target_path, pkg_format="deb"):
     assert pkg_format in {"deb", "rpm"}
     if pkg_format == "deb":
         sm_plugin_key = "plugin/latest/ubuntu_64bit/session-manager-plugin.deb"
     else:
         sm_plugin_key = "plugin/latest/linux_64bit/session-manager-plugin.rpm"
     with tempfile.TemporaryDirectory() as td:
@@ -37,14 +41,15 @@
         if pkg_format == "deb":
             subprocess.check_call(["dpkg", "-x", sm_archive_path, td])
         elif pkg_format == "rpm":
             command = "rpm2cpio '{}' | cpio --extract --make-directories --directory '{}'"
             subprocess.check_call(command.format(sm_archive_path, td), shell=True)
         shutil.move(os.path.join(td, "usr/local/sessionmanagerplugin/bin/session-manager-plugin"), target_path)
 
+
 def ensure_session_manager_plugin():
     session_manager_dir = os.path.join(config.user_config_dir, "bin")
     PATH = os.environ.get("PATH", "") + ":" + session_manager_dir
     if shutil.which("session-manager-plugin", path=PATH):
         subprocess.check_call(["session-manager-plugin"], env=dict(os.environ, PATH=PATH))
     else:
         os.makedirs(session_manager_dir, exist_ok=True)
@@ -55,27 +60,30 @@
             download_session_manager_plugin_linux(target_path=target_path)
         else:
             download_session_manager_plugin_linux(target_path=target_path, pkg_format="rpm")
         os.chmod(target_path, stat.S_IRUSR | stat.S_IWUSR | stat.S_IXUSR)
         subprocess.check_call(["session-manager-plugin"], env=dict(os.environ, PATH=PATH))
     return shutil.which("session-manager-plugin", path=PATH)
 
+
 def run_command(command, instance_ids=None, targets=None, timeout=900):
     """
     Sends a command to specified instances using AWS Systems Manager. Waits for the command to complete.
     Queries CloudWatch Logs for command stdout and stderr output, printing it to the terminal.
     Raises an exception if the command exits with a non-zero exit status.
 
     See https://docs.aws.amazon.com/systems-manager/latest/userguide/execute-remote-commands.html for details.
     """
-    send_command_args = dict(DocumentName="AWS-RunShellScript",
-                             CloudWatchOutputConfig=dict(CloudWatchOutputEnabled=True, CloudWatchLogGroupName=__name__),
-                             Parameters=dict(commands=[command]),
-                             TimeoutSeconds=timeout,
-                             Comment="Started by {}".format(__name__))
+    send_command_args = dict(
+        DocumentName="AWS-RunShellScript",
+        CloudWatchOutputConfig=dict(CloudWatchOutputEnabled=True, CloudWatchLogGroupName=__name__),
+        Parameters=dict(commands=[command]),
+        TimeoutSeconds=timeout,
+        Comment=f"Started by {__name__}",
+    )
     if instance_ids:
         send_command_args.update(InstanceIds=instance_ids)
     if targets:
         send_command_args.update(Targets=targets)
     log_readers, stdout, command_id = {}, [], None  # type: ignore
     try:
         command_id = clients.ssm.send_command(**send_command_args)["Command"]["CommandId"]
@@ -88,16 +96,17 @@
                     raise AegeaException("SSM command failed: {}".format(invocation))
                 statuses.append(invocation["Status"])
                 if invocation["Status"] not in {"InProgress", "Success"}:
                     continue
                 for stream in "stdout", "stderr":
                     log_stream_name = "{}/{}/aws-runShellScript/{}".format(command_id, invocation["InstanceId"], stream)
                     if log_stream_name not in log_readers:
-                        log_readers[log_stream_name] = CloudwatchLogReader(log_group_name=__name__,
-                                                                           log_stream_name=log_stream_name)
+                        log_readers[log_stream_name] = CloudwatchLogReader(
+                            log_group_name=__name__, log_stream_name=log_stream_name
+                        )
                     try:
                         for event in log_readers[log_stream_name]:
                             print(event["message"], file=getattr(sys, stream))
                     except clients.logs.exceptions.ResourceNotFoundException:
                         logger.debug("No logs for %s", log_stream_name)
                 sys.stderr.write(".")
                 sys.stderr.flush()
```

### Comparing `aegea-4.3.4/aegea/util/cloudinit.py` & `aegea-4.4.0/aegea/util/cloudinit.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/util/constants.py` & `aegea-4.4.0/aegea/util/constants.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/util/crypto.py` & `aegea-4.4.0/aegea/util/crypto.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/util/printing.py` & `aegea-4.4.0/aegea/util/printing.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/util/ssh.py` & `aegea-4.4.0/aegea/util/ssh.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea/zones.py` & `aegea-4.4.0/aegea/zones.py`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/aegea.egg-info/PKG-INFO` & `aegea-4.4.0/aegea.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aegea
-Version: 4.3.4
+Version: 4.4.0
 Summary: Amazon Web Services Operator Interface
 Home-page: https://github.com/kislyuk/aegea
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Platform: MacOS X
 Platform: Posix
```

### Comparing `aegea-4.3.4/aegea.egg-info/SOURCES.txt` & `aegea-4.4.0/aegea.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 aegea/batch.py
 aegea/billing.py
 aegea/build_ami.py
 aegea/build_docker_image.py
 aegea/cloudtrail.py
 aegea/constants.json
 aegea/cost.py
-aegea/deploy.py
 aegea/ebs.py
 aegea/ecr.py
 aegea/ecs.py
 aegea/efs.py
 aegea/elb.py
 aegea/flow_logs.py
 aegea/iam.py
@@ -117,60 +116,14 @@
 aegea/missions/ecs-container-instance/rootfs.skel.in/etc/ecs/ecs.config
 aegea/missions/fog-dog/Makefile
 aegea/missions/fog-dog/config.yml
 aegea/missions/fog-dog/environment
 aegea/missions/fog-dog/rootfs.skel.in/etc/update-motd.d/fogdog-motd
 aegea/missions/ubuntu-14.04/config.yml
 aegea/missions/ubuntu-14.04/rootfs.skel/etc/init/awslogs.conf
-aegea/packages/__init__.py
-aegea/packages/github3/__init__.py
-aegea/packages/github3/api.py
-aegea/packages/github3/auths.py
-aegea/packages/github3/decorators.py
-aegea/packages/github3/events.py
-aegea/packages/github3/git.py
-aegea/packages/github3/github.py
-aegea/packages/github3/models.py
-aegea/packages/github3/notifications.py
-aegea/packages/github3/orgs.py
-aegea/packages/github3/pulls.py
-aegea/packages/github3/session.py
-aegea/packages/github3/structs.py
-aegea/packages/github3/users.py
-aegea/packages/github3/utils.py
-aegea/packages/github3/gists/__init__.py
-aegea/packages/github3/gists/comment.py
-aegea/packages/github3/gists/file.py
-aegea/packages/github3/gists/gist.py
-aegea/packages/github3/gists/history.py
-aegea/packages/github3/issues/__init__.py
-aegea/packages/github3/issues/comment.py
-aegea/packages/github3/issues/event.py
-aegea/packages/github3/issues/issue.py
-aegea/packages/github3/issues/label.py
-aegea/packages/github3/issues/milestone.py
-aegea/packages/github3/repos/__init__.py
-aegea/packages/github3/repos/branch.py
-aegea/packages/github3/repos/comment.py
-aegea/packages/github3/repos/commit.py
-aegea/packages/github3/repos/comparison.py
-aegea/packages/github3/repos/contents.py
-aegea/packages/github3/repos/deployment.py
-aegea/packages/github3/repos/hook.py
-aegea/packages/github3/repos/pages.py
-aegea/packages/github3/repos/release.py
-aegea/packages/github3/repos/repo.py
-aegea/packages/github3/repos/stats.py
-aegea/packages/github3/repos/status.py
-aegea/packages/github3/repos/tag.py
-aegea/packages/github3/search/__init__.py
-aegea/packages/github3/search/code.py
-aegea/packages/github3/search/issue.py
-aegea/packages/github3/search/repository.py
-aegea/packages/github3/search/user.py
 aegea/rootfs.skel.build_ami/etc/aws.conf
 aegea/rootfs.skel.build_ami/etc/awslogs.conf
 aegea/rootfs.skel.build_ami/etc/awslogs.logging.conf
 aegea/rootfs.skel.build_ami/etc/R/Rprofile.site
 aegea/rootfs.skel.build_ami/etc/apt/apt.conf.d/99aegea
 aegea/rootfs.skel.build_ami/etc/cloud/cloud.cfg.d/90_dpkg.cfg
 aegea/rootfs.skel.build_ami/etc/cloud/cloud.cfg.d/99_aegea.cfg
@@ -204,15 +157,14 @@
 aegea/rootfs.skel.build_ami/var/lib/docker/.keep
 aegea/rootfs.skel.launch/var/lib/aegea/.keep
 aegea/util/__init__.py
 aegea/util/cloudinit.py
 aegea/util/constants.py
 aegea/util/crypto.py
 aegea/util/exceptions.py
-aegea/util/git.py
 aegea/util/printing.py
 aegea/util/ssh.py
 aegea/util/aws/__init__.py
 aegea/util/aws/_boto3_loader.py
 aegea/util/aws/batch.py
 aegea/util/aws/clients.py
 aegea/util/aws/dns.py
```

### Comparing `aegea-4.3.4/common.mk` & `aegea-4.4.0/common.mk`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/scripts/aegea` & `aegea-4.4.0/scripts/aegea`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/scripts/aegea-build-image-for-mission` & `aegea-4.4.0/scripts/aegea-build-image-for-mission`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/scripts/aegea-rebuild-public-elb-sg` & `aegea-4.4.0/scripts/aegea-rebuild-public-elb-sg`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/scripts/aegea-ssh` & `aegea-4.4.0/scripts/aegea-ssh`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/scripts/pypi-apt-freeze` & `aegea-4.4.0/scripts/pypi-apt-freeze`

 * *Files identical despite different names*

### Comparing `aegea-4.3.4/setup.py` & `aegea-4.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     use_scm_version={
         "write_to": "aegea/version.py",
     },
     setup_requires=["setuptools_scm >= 3.4.3"],
     install_requires=[
         "boto3 >= 1.20.35, < 2",
         "argcomplete >= 1.9.5, < 4",
-        "paramiko >= 2.4.2, < 3",
+        "paramiko >= 2.4.2, < 4",
         "requests >= 2.18.4, < 3",
         "tweak >= 1.0.4, < 2",
         "pyyaml >= 3.12, < 7",
         "python-dateutil >= 2.6.1, < 3",
         "babel >= 2.4.0, < 3",
         "ipwhois >= 1.1.0, < 2",
         "uritemplate >= 3.0.0, < 4",
```

### Comparing `aegea-4.3.4/test/test.py` & `aegea-4.4.0/test/test.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from aegea.util.aws import (resolve_ami, locate_ami, get_ondemand_price_usd, ARN,
                             get_public_ip_ranges, ensure_s3_bucket, encode_tags, decode_tags, filter_by_tags,
                             clients, resources, get_bdm, get_iam_role_for_instance, make_waiter)
 from aegea.util.aws.iam import IAMPolicyBuilder
 from aegea.util.aws.batch import ensure_job_definition
 from aegea.util.aws.spot import SpotFleetBuilder
 from aegea.util.exceptions import AegeaException
-from aegea.util.git import private_submodules
 
 for importer, modname, is_pkg in pkgutil.iter_modules(aegea.__path__):
     importlib.import_module((aegea.__package__ or "aegea") + "." + modname)
 
 class TestAegea(unittest.TestCase):
     SubprocessResult = collections.namedtuple("SubprocessResult", "stdout stderr returncode")
 
@@ -248,14 +247,22 @@
         make_waiter(clients.efs.describe_file_systems, "FileSystems[].LifeCycleState", "available", "pathAny")
 
     def test_locate_ami(self):
         self.assertTrue(locate_ami("Ubuntu", "20.04", "amd64").id.startswith("ami-"))
         self.assertTrue(locate_ami("Ubuntu", "20.04", "arm64").id.startswith("ami-"))
         self.assertTrue(locate_ami("Amazon Linux", "2", "x86_64").id.startswith("ami-"))
         self.assertTrue(locate_ami("Amazon Linux", "2", "arm64").id.startswith("ami-"))
+        self.assertTrue(locate_ami("Ubuntu", "22.04", "amd64").id.startswith("ami-"))
+        self.assertTrue(locate_ami("Ubuntu", "22.04", "arm64").id.startswith("ami-"))
+        self.assertTrue(locate_ami("Amazon Linux", "2", "amd64").id.startswith("ami-"))
+        self.assertTrue(locate_ami("Amazon Linux", "2", "arm64").id.startswith("ami-"))
+        self.assertTrue(locate_ami("Amazon Linux", "2023", "amd64").id.startswith("ami-"))
+        self.assertTrue(locate_ami("Amazon Linux", "2023", "arm64").id.startswith("ami-"))
+        with self.assertRaises(Exception):
+            locate_ami("Amazon Linux", "9000", "arm64")
 
     def test_ip_ranges(self):
         get_public_ip_ranges()
         get_public_ip_ranges(region="us-east-1", service="ROUTE53_HEALTHCHECKS")
 
     def test_date_utils(self):
         with self.assertRaises(TypeError):
@@ -298,19 +305,14 @@
         args = submit_parser.parse_args(["--command", ""])
         args.default_job_role_iam_policies = []
         args.user, args.job_role, args.default_job_role_iam_policies = "0", "aegea.batch.worker", []
         jd1 = ensure_job_definition(args)
         jd2 = ensure_job_definition(args)
         self.assertEqual(jd1["jobDefinitionArn"], jd2["jobDefinitionArn"])
 
-    @unittest.skipUnless("GH_AUTH" in os.environ, "requires GitHub credentials")
-    def test_git_utils(self):
-        for submodule in private_submodules("git@github.com:ansible/ansible.git"):
-            print(submodule)
-
     def test_ssh_utils(self):
         from aegea.util.aws.ssm import ensure_session_manager_plugin
         ensure_session_manager_plugin()
 
     def test_ssh_get_user_info(self):
         from aegea.ssh import get_user_info
         testcases = ((
```

