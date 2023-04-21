# Comparing `tmp/wax-ml-0.6.3.tar.gz` & `tmp/wax-ml-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wax-ml-0.6.3.tar", last modified: Fri Nov 18 21:25:54 2022, max compression
+gzip compressed data, was "wax-ml-0.6.4.tar", last modified: Fri Apr 21 22:26:56 2023, max compression
```

## Comparing `wax-ml-0.6.3.tar` & `wax-ml-0.6.4.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 21:25:54.586506 wax-ml-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-11-18 21:25:40.000000 wax-ml-0.6.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-11-18 21:25:40.000000 wax-ml-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-11-18 21:25:40.000000 wax-ml-0.6.3/LICENSE_SHORT
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-11-18 21:25:40.000000 wax-ml-0.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    35231 2022-11-18 21:25:54.586506 wax-ml-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    34376 2022-11-18 21:25:40.000000 wax-ml-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 21:25:54.574505 wax-ml-0.6.3/docs/
--rw-r--r--   0 runner    (1001) docker     (121)    11242 2022-11-18 21:25:40.000000 wax-ml-0.6.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 21:25:54.578505 wax-ml-0.6.3/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (121)     3734 2022-11-18 21:25:40.000000 wax-ml-0.6.3/docs/notebooks/01_demo_EWMA.py
--rw-r--r--   0 runner    (1001) docker     (121)     3656 2022-11-18 21:25:40.000000 wax-ml-0.6.3/docs/notebooks/02_Synchronize_data_streams.py
--rw-r--r--   0 runner    (1001) docker     (121)     2331 2022-11-18 21:25:40.000000 wax-ml-0.6.3/docs/notebooks/03_ohlc_temperature.py
--rw-r--r--   0 runner    (1001) docker     (121)    13313 2022-11-18 21:25:40.000000 wax-ml-0.6.3/docs/notebooks/04_The_three_steps_workflow.py
--rw-r--r--   0 runner    (1001) docker     (121)    24238 2022-11-18 21:25:40.000000 wax-ml-0.6.3/docs/notebooks/05_reconstructing_the_light_curve_of_stars.py
--rw-r--r--   0 runner    (1001) docker     (121)    11277 2022-11-18 21:25:40.000000 wax-ml-0.6.3/docs/notebooks/06_Online_Linear_Regression.py
--rw-r--r--   0 runner    (1001) docker     (121)    18731 2022-11-18 21:25:40.000000 wax-ml-0.6.3/docs/notebooks/07_Online_Time_Series_Prediction.py
--rw-r--r--   0 runner    (1001) docker     (121)    18541 2022-11-18 21:25:40.000000 wax-ml-0.6.3/docs/notebooks/08_Online_learning_in_non_stationary_environments.py
--rw-r--r--   0 runner    (1001) docker     (121)     4232 2022-11-18 21:25:54.590505 wax-ml-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      621 2022-11-18 21:25:40.000000 wax-ml-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 21:25:54.578505 wax-ml-0.6.3/wax/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12719 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/accessors.py
--rw-r--r--   0 runner    (1001) docker     (121)    11572 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/accessors_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      781 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/compile.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 21:25:54.578505 wax-ml-0.6.3/wax/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2107 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/datasets/generate_temperature_data.py
--rw-r--r--   0 runner    (1001) docker     (121)      843 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/datasets/generate_temperature_data_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     7894 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/encode.py
--rw-r--r--   0 runner    (1001) docker     (121)     4084 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/encode_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     8109 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/format.py
--rw-r--r--   0 runner    (1001) docker     (121)     1685 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/format_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 21:25:54.578505 wax-ml-0.6.3/wax/gym/
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/gym/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1844 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/gym/agent.py
--rw-r--r--   0 runner    (1001) docker     (121)      971 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/gym/agent_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 21:25:54.582506 wax-ml-0.6.3/wax/gym/callbacks/
--rw-r--r--   0 runner    (1001) docker     (121)      762 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/gym/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5208 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/gym/callbacks/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1480 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/gym/callbacks/callbacks_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/gym/callbacks/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (121)     3648 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/gym/callbacks/record.py
--rw-r--r--   0 runner    (1001) docker     (121)      875 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/gym/callbacks/stop.py
--rw-r--r--   0 runner    (1001) docker     (121)      693 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/gym/entity.py
--rw-r--r--   0 runner    (1001) docker     (121)     1565 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/gym/env.py
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/gym/env_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2548 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/gym/gym_unroll.py
--rw-r--r--   0 runner    (1001) docker     (121)     1691 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/gym/haiku_agent.py
--rw-r--r--   0 runner    (1001) docker     (121)     2206 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/gym/haiku_env.py
--rw-r--r--   0 runner    (1001) docker     (121)     6297 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/gym/haiku_env_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 21:25:54.586506 wax-ml-0.6.3/wax/modules/
--rw-r--r--   0 runner    (1001) docker     (121)     2102 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2196 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/apply_mask.py
--rw-r--r--   0 runner    (1001) docker     (121)     2803 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/apply_mask_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1590 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/arma.py
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/arma_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2895 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/buffer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2940 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/buffer_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      923 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/counter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/counter_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1342 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/diff.py
--rw-r--r--   0 runner    (1001) docker     (121)     1358 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/diff_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     7624 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/ewma.py
--rw-r--r--   0 runner    (1001) docker     (121)     8917 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/ewma_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     6213 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/ewmcov.py
--rw-r--r--   0 runner    (1001) docker     (121)     4097 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/ewmcov_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4338 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/ewmvar.py
--rw-r--r--   0 runner    (1001) docker     (121)     5638 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/ewmvar_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1170 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/ffill.py
--rw-r--r--   0 runner    (1001) docker     (121)      928 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/ffill_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1398 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/fill_nan_inf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1400 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/fill_nan_inf_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2705 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/func_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1830 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/func_optimizer_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3598 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/gym_feedback.py
--rw-r--r--   0 runner    (1001) docker     (121)     6007 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/gym_feedback_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1160 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/has_changed.py
--rw-r--r--   0 runner    (1001) docker     (121)     1356 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/lag.py
--rw-r--r--   0 runner    (1001) docker     (121)     2087 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/lag_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1567 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/mask_mean.py
--rw-r--r--   0 runner    (1001) docker     (121)     2471 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/mask_mean_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1806 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/mask_normalize.py
--rw-r--r--   0 runner    (1001) docker     (121)     2829 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/mask_normalize_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2125 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/mask_std.py
--rw-r--r--   0 runner    (1001) docker     (121)     4246 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/mask_std_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3364 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/ohlc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1814 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/ohlc_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     5863 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/online_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2465 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/online_supervised_learner.py
--rw-r--r--   0 runner    (1001) docker     (121)     7778 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/online_supervised_learner_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1244 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/optax_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2298 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/pct_change.py
--rw-r--r--   0 runner    (1001) docker     (121)     1773 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/pct_change_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1585 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/rolling_mean.py
--rw-r--r--   0 runner    (1001) docker     (121)     2149 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/rolling_mean_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3939 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/snarimax.py
--rw-r--r--   0 runner    (1001) docker     (121)     5788 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/snarimax_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3947 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/update_on_event.py
--rw-r--r--   0 runner    (1001) docker     (121)     4490 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/update_on_event_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2838 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/update_params.py
--rw-r--r--   0 runner    (1001) docker     (121)     1832 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/vmap.py
--rw-r--r--   0 runner    (1001) docker     (121)     1368 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/modules/vmap_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 21:25:54.586506 wax-ml-0.6.3/wax/numba/
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/numba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9932 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/numba/ewma_numba.py
--rw-r--r--   0 runner    (1001) docker     (121)     4007 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/numba/ewma_numba_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 21:25:54.586506 wax-ml-0.6.3/wax/optim/
--rw-r--r--   0 runner    (1001) docker     (121)      641 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3609 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/optim/newton.py
--rw-r--r--   0 runner    (1001) docker     (121)     1350 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/optim/newton_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/predicate.py
--rw-r--r--   0 runner    (1001) docker     (121)     3822 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/stateful.py
--rw-r--r--   0 runner    (1001) docker     (121)     3800 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/stateful_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    28165 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/stream.py
--rw-r--r--   0 runner    (1001) docker     (121)     9949 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/stream_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1720 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/testing.py
--rw-r--r--   0 runner    (1001) docker     (121)     3186 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/transform.py
--rw-r--r--   0 runner    (1001) docker     (121)    14616 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/unroll.py
--rw-r--r--   0 runner    (1001) docker     (121)     1270 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/unroll_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-11-18 21:25:40.000000 wax-ml-0.6.3/wax/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 21:25:54.586506 wax-ml-0.6.3/wax_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    35231 2022-11-18 21:25:54.000000 wax-ml-0.6.3/wax_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3003 2022-11-18 21:25:54.000000 wax-ml-0.6.3/wax_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-18 21:25:54.000000 wax-ml-0.6.3/wax_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-18 21:25:54.000000 wax-ml-0.6.3/wax_ml.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-11-18 21:25:54.000000 wax-ml-0.6.3/wax_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-11-18 21:25:54.000000 wax-ml-0.6.3/wax_ml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:26:56.345988 wax-ml-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-21 22:26:45.000000 wax-ml-0.6.4/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-21 22:26:45.000000 wax-ml-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-21 22:26:45.000000 wax-ml-0.6.4/LICENSE_SHORT
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-21 22:26:45.000000 wax-ml-0.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    35231 2023-04-21 22:26:56.345988 wax-ml-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    34376 2023-04-21 22:26:45.000000 wax-ml-0.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:26:56.313987 wax-ml-0.6.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-04-21 22:26:45.000000 wax-ml-0.6.4/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:26:56.313987 wax-ml-0.6.4/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-21 22:26:45.000000 wax-ml-0.6.4/docs/notebooks/01_demo_EWMA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-04-21 22:26:45.000000 wax-ml-0.6.4/docs/notebooks/02_Synchronize_data_streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-21 22:26:45.000000 wax-ml-0.6.4/docs/notebooks/03_ohlc_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13266 2023-04-21 22:26:45.000000 wax-ml-0.6.4/docs/notebooks/04_The_three_steps_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24239 2023-04-21 22:26:45.000000 wax-ml-0.6.4/docs/notebooks/05_reconstructing_the_light_curve_of_stars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-04-21 22:26:45.000000 wax-ml-0.6.4/docs/notebooks/06_Online_Linear_Regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18713 2023-04-21 22:26:45.000000 wax-ml-0.6.4/docs/notebooks/07_Online_Time_Series_Prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18538 2023-04-21 22:26:45.000000 wax-ml-0.6.4/docs/notebooks/08_Online_learning_in_non_stationary_environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-04-21 22:26:56.349988 wax-ml-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-21 22:26:45.000000 wax-ml-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:26:56.321987 wax-ml-0.6.4/wax/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12719 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11570 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/accessors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/compile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:26:56.321987 wax-ml-0.6.4/wax/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/datasets/generate_temperature_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/datasets/generate_temperature_data_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/encode_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/format_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:26:56.325987 wax-ml-0.6.4/wax/gym/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/gym/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/gym/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/gym/agent_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:26:56.325987 wax-ml-0.6.4/wax/gym/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/gym/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/gym/callbacks/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/gym/callbacks/callbacks_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/gym/callbacks/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/gym/callbacks/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/gym/callbacks/stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/gym/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/gym/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/gym/env_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/gym/gym_unroll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/gym/haiku_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/gym/haiku_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/gym/haiku_env_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:26:56.341987 wax-ml-0.6.4/wax/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/apply_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/apply_mask_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/arma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/arma_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/buffer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/counter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/diff_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/ewma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/ewma_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/ewmcov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/ewmcov_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/ewmvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/ewmvar_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/ffill.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/ffill_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/fill_nan_inf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/fill_nan_inf_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/func_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/func_optimizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/gym_feedback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/gym_feedback_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/has_changed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/lag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/lag_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/mask_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/mask_mean_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/mask_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/mask_normalize_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/mask_std.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/mask_std_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/ohlc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/ohlc_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/online_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/online_supervised_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/online_supervised_learner_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/optax_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/pct_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/pct_change_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/rolling_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/rolling_mean_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/snarimax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/snarimax_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/update_on_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/update_on_event_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/update_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/vmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/modules/vmap_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:26:56.345988 wax-ml-0.6.4/wax/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/optim/newton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/optim/newton_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/stateful_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28180 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/stream_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14616 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/unroll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/unroll_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:26:56.321987 wax-ml-0.6.4/wax-numba/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax-numba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax-numba/ewma_numba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-04-21 22:26:45.000000 wax-ml-0.6.4/wax-numba/ewma_numba_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:26:56.345988 wax-ml-0.6.4/wax_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    35231 2023-04-21 22:26:56.000000 wax-ml-0.6.4/wax_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-21 22:26:56.000000 wax-ml-0.6.4/wax_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 22:26:56.000000 wax-ml-0.6.4/wax_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 22:26:56.000000 wax-ml-0.6.4/wax_ml.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-21 22:26:56.000000 wax-ml-0.6.4/wax_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-21 22:26:56.000000 wax-ml-0.6.4/wax_ml.egg-info/top_level.txt
```

### Comparing `wax-ml-0.6.3/LICENSE` & `wax-ml-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/LICENSE_SHORT` & `wax-ml-0.6.4/LICENSE_SHORT`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/PKG-INFO` & `wax-ml-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wax-ml
-Version: 0.6.3
+Version: 0.6.4
 Summary: A Python library for machine-learning and feedback loops on streaming data
 Home-page: https://github.com/eserie/wax-ml
 Author: WAX-ML Authors
 Author-email: eserie@gmail.com
 License: Apache
 Keywords: time series,machine learning,optimization,optimal control,online learning,reinforcement learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `wax-ml-0.6.3/README.md` & `wax-ml-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/docs/conf.py` & `wax-ml-0.6.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/docs/notebooks/01_demo_EWMA.py` & `wax-ml-0.6.4/docs/notebooks/01_demo_EWMA.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # jupyter:
 #   jupytext:
 #     formats: ipynb,py,md
 #     text_representation:
 #       extension: .py
 #       format_name: light
 #       format_version: '1.5'
-#       jupytext_version: 1.13.3
+#       jupytext_version: 1.14.5
 #   kernelspec:
 #     display_name: Python 3 (ipykernel)
 #     language: python
 #     name: python3
 # ---
 
 # +
@@ -43,39 +43,37 @@
 #
 # Let's show how it works.
 
 # ## Load accessors
 
 # First you need to load accessors:
 
-# + tags=[]
+# +
 from wax.accessors import register_wax_accessors
 
 register_wax_accessors()
 # -
 
 # ## EWMA on dataframes
 
 # Let's look at a simple example: The exponential moving average (EWMA).
 #
 # Let's apply the EWMA algorithm to the [NCEP/NCAR 's Air temperature data](http://www.esrl.noaa.gov/psd/data/gridded/data.ncep.reanalysis.html).
 
 # ### 🌡 Load temperature dataset 🌡
 
-# + tags=[]
+# +
 import xarray as xr
 
 dataset = xr.tutorial.open_dataset("air_temperature")
 # -
 
 # Let's see what this dataset looks like:
 
-# + tags=[]
 dataset
-# -
 
 # To compute a EWMA on some variables of a dataset, we usually need to convert data
 # in pandas
 # [series](https://pandas.pydata.org/docs/reference/api/pandas.Series.html) or
 # [dataframe](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html).
 #
 # So, let's convert the dataset into a dataframe to illustrate `accessors` on a dataframe:
@@ -83,23 +81,14 @@
 dataframe = dataset.air.to_series().unstack(["lon", "lat"])
 
 # ### EWMA with pandas
 
 air_temp_ewma = dataframe.ewm(com=10).mean()
 _ = air_temp_ewma.mean(1).plot()
 
-# ## wax numba ewma
-
-from wax.numba.ewma_numba import register_wax_numba
-
-register_wax_numba()
-
-air_temp_ewma = dataframe.wax_numba.ewm(com=10).mean()
-_ = air_temp_ewma.mean(1).plot()
-
 # ### EWMA with WAX-ML
 
 air_temp_ewma = dataframe.wax.ewm(com=10).mean()
 _ = air_temp_ewma.mean(1).plot()
 
 # On small data, WAX-ML's EWMA is slower than Pandas' because of the expensive data conversion steps.
 # WAX-ML's accessors are interesting to use on large data loads
```

### Comparing `wax-ml-0.6.3/docs/notebooks/02_Synchronize_data_streams.py` & `wax-ml-0.6.4/docs/notebooks/02_Synchronize_data_streams.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # jupyter:
 #   jupytext:
 #     formats: ipynb,py,md
 #     text_representation:
 #       extension: .py
 #       format_name: light
 #       format_version: '1.5'
-#       jupytext_version: 1.13.3
+#       jupytext_version: 1.14.5
 #   kernelspec:
 #     display_name: Python 3 (ipykernel)
 #     language: python
 #     name: python3
 # ---
 
 # +
@@ -56,31 +56,31 @@
 #
 # Let's illustrate with a small example how `wax.stream.Stream` synchronizes data streams.
 #
 # Let's use the dataset "air temperature" with :
 # - An air temperature is defined with hourly resolution.
 # - A "fake" ground temperature is defined with a daily resolution as the air temperature minus 10 degrees.
 
-# + tags=[]
+# +
 import xarray as xr
 
 dataset = xr.tutorial.open_dataset("air_temperature")
 dataset["ground"] = dataset.air.resample(time="d").last().rename({"time": "day"}) - 10
 # -
 
 # Let's see what this dataset looks like:
 
 dataset
 
-# + tags=[]
+# +
 from wax.accessors import register_wax_accessors
 
 register_wax_accessors()
 
-# + tags=[]
+# +
 from wax.modules import EWMA
 
 
 def my_custom_function(dataset):
     return {
         "air_10": EWMA(com=10)(dataset["air"]),
         "air_100": EWMA(com=100.0)(dataset["air"]),
```

### Comparing `wax-ml-0.6.3/docs/notebooks/03_ohlc_temperature.py` & `wax-ml-0.6.4/docs/notebooks/03_ohlc_temperature.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # jupyter:
 #   jupytext:
 #     formats: ipynb,py,md
 #     text_representation:
 #       extension: .py
 #       format_name: light
 #       format_version: '1.5'
-#       jupytext_version: 1.13.3
+#       jupytext_version: 1.14.5
 #   kernelspec:
 #     display_name: Python 3
 #     language: python
 #     name: python3
 # ---
 
 # +
@@ -31,48 +31,45 @@
 # [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/eserie/wax-ml/blob/main/docs/notebooks/03_ohlc_temperature.ipynb)
 
 # Let's again considering the air temperatures dataset.
 # It is sampled at an hourly resolution.
 # We will make "trailing" air temperature bins during each day and "reset" the bin
 # aggregation process at each day change.
 
-# + tags=[]
 import numpy as onp
 import xarray as xr
 
-# + tags=[]
+# +
 from wax.accessors import register_wax_accessors
 from wax.modules import OHLC, HasChanged
 
 register_wax_accessors()
+# -
 
-# + tags=[]
 dataset = xr.tutorial.open_dataset("air_temperature")
 dataset["date"] = dataset.time.dt.date.astype(onp.datetime64)
-# -
 
 dataset
 
 
-# + tags=[]
+# +
 def bin_temperature(da):
     day_change = HasChanged()(da["date"])
     return OHLC()(da["air"], reset_on=day_change)
 
 
 output, state = dataset.wax.stream().apply(
     bin_temperature, format_dims=onp.array(dataset.air.dims)
 )
 output = xr.Dataset(output._asdict())
+# -
 
-# + tags=[]
 df = output.isel(lat=0, lon=0).drop(["lat", "lon"]).to_pandas().loc["2013-01"]
 _ = df.plot(figsize=(12, 8), title="Trailing Open-High-Low-Close temperatures")
 
-# + [markdown] tags=[]
 # ## The `UpdateOnEvent` module
 #
 # The `OHLC` module uses the primitive `wax.modules.UpdateOnEvent`.
 #
 # Its implementation required to complete Haiku with a central function
 # `set_params_or_state_dict` which we have actually integrated in this WAX-ML module.
 #
```

### Comparing `wax-ml-0.6.3/docs/notebooks/04_The_three_steps_workflow.py` & `wax-ml-0.6.4/docs/notebooks/04_The_three_steps_workflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # jupyter:
 #   jupytext:
 #     formats: ipynb,py:light,md
 #     text_representation:
 #       extension: .py
 #       format_name: light
 #       format_version: '1.5'
-#       jupytext_version: 1.13.3
+#       jupytext_version: 1.14.5
 #   kernelspec:
 #     display_name: Python 3 (ipykernel)
 #     language: python
 #     name: python3
 # ---
 
 # + colab={"base_uri": "https://localhost:8080/"} id="2b295407-92c4-4818-bfb9-f445f6967f10" outputId="dc6c8e1b-2875-4287-d83a-4bdc4c9db80a"
@@ -56,15 +56,15 @@
 # You can then take full advantage of the JAX primitives, especially the `jit` primitive.
 #
 # Let's illustrate how to reimplement WAX-ML EWMA yourself with the WAX-ML 3-step workflow.
 
 # + [markdown] id="bd2e906e"
 # ## Imports
 
-# + id="2bdfbf9a" tags=[]
+# + id="2bdfbf9a"
 import numpy as onp
 import pandas as pd
 import xarray as xr
 
 from wax.accessors import register_wax_accessors
 from wax.format import format_dataframe
 from wax.modules import EWMA
@@ -79,44 +79,44 @@
 # + [markdown] id="6f8447b4"
 # ### Generate data
 
 # + id="768d7802-580d-4c31-9a0e-e6dc4f0589ca" tags=["parameters"]
 T = 1.0e5
 N = 1000
 
-# + id="03af743d" tags=[]
+# + id="03af743d"
 T, N = map(int, (T, N))
 dataframe = pd.DataFrame(
     onp.random.normal(size=(T, N)), index=pd.date_range("1970", periods=T, freq="s")
 )
 
 # + [markdown] id="d1fd46f7"
 # ### pandas EWMA
 
-# + colab={"base_uri": "https://localhost:8080/"} id="27092faf" outputId="e97a2738-5c2a-4bf9-c9e0-c44040185424" tags=[]
+# + colab={"base_uri": "https://localhost:8080/"} id="27092faf" outputId="e97a2738-5c2a-4bf9-c9e0-c44040185424"
 # %%time
 df_ewma_pandas = dataframe.ewm(alpha=1.0 / 10.0).mean()
 
 # + [markdown] id="678be283"
 # ### WAX-ML EWMA
 
-# + colab={"base_uri": "https://localhost:8080/"} id="11f3705d" outputId="744f0faa-7030-4155-80ae-4a5c745731f8" tags=[]
+# + colab={"base_uri": "https://localhost:8080/"} id="11f3705d" outputId="744f0faa-7030-4155-80ae-4a5c745731f8"
 # %%time
 df_ewma_wax = dataframe.wax.ewm(alpha=1.0 / 10.0).mean()
 
 # + [markdown] id="0d94d5cf"
 # It's a little faster, but not that much faster...
 
 # + [markdown] id="e51ee290"
 # ### WAX-ML EWMA (without format step)
 
 # + [markdown] id="7361def9"
 # Let's disable the final formatting step (the output is now in raw JAX format):
 
-# + colab={"base_uri": "https://localhost:8080/"} id="f87f5668" outputId="3f37d97e-1875-4f66-9e6b-9a22b20642a6" tags=[]
+# + colab={"base_uri": "https://localhost:8080/"} id="f87f5668" outputId="3f37d97e-1875-4f66-9e6b-9a22b20642a6"
 # %%time
 df_ewma_wax_no_format = dataframe.wax.ewm(alpha=1.0 / 10.0, format_outputs=False).mean()
 df_ewma_wax_no_format.block_until_ready()
 
 # + colab={"base_uri": "https://localhost:8080/"} id="88d0cab5-62ad-47f7-9d06-56fc45fa542e" outputId="f8b7c4fb-79a7-4652-82eb-2b649aeb074c"
 type(df_ewma_wax_no_format)
 
@@ -199,15 +199,15 @@
 
 # + colab={"base_uri": "https://localhost:8080/"} id="3862a486-a5a2-4aa9-967a-59ebc32a18e1" outputId="b54b4e2c-a0ab-4a43-d331-d6b3d90707c6"
 outputs.device()
 
 # + [markdown] id="b73f3252"
 # Once it has been compiled and "traced" by JAX, the function is much faster to execute:
 
-# + colab={"base_uri": "https://localhost:8080/"} id="a889d294" outputId="e69a75ff-4b00-4a1d-f101-49944e01d9b4" tags=[]
+# + colab={"base_uri": "https://localhost:8080/"} id="a889d294" outputId="e69a75ff-4b00-4a1d-f101-49944e01d9b4"
 # %%timeit
 outputs = unroll(transform_dataset)(jxs)
 _ = outputs.block_until_ready()
 
 # + [markdown] id="987e8b63"
 # This is 3x faster than pandas implementation!
 
@@ -243,14 +243,15 @@
 # + [markdown] id="f851fbe7-096e-4399-ae5c-08739837dfeb"
 # We have now "JAX-ready" data for later fast access.
 
 # + [markdown] id="19f3b58e-61f3-481c-a512-cb87bde622a8"
 # Let's define the transformation that wrap the actual data and indices in a pair of
 # pure functions:
 
+
 # + id="e7ebbb08-d790-4977-b49d-c9224e299a42"
 @jax.jit
 @unroll
 def transform_dataset(step):
     dataset = tree_access_data(jnp_data, jnp_index, step)
     return EWMA(alpha=1.0 / 10.0, adjust=True)(dataset["dataarray"])
```

### Comparing `wax-ml-0.6.3/docs/notebooks/05_reconstructing_the_light_curve_of_stars.py` & `wax-ml-0.6.4/docs/notebooks/05_reconstructing_the_light_curve_of_stars.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # jupyter:
 #   jupytext:
 #     formats: ipynb,py,md
 #     text_representation:
 #       extension: .py
 #       format_name: light
 #       format_version: '1.5'
-#       jupytext_version: 1.13.3
+#       jupytext_version: 1.14.5
 #   kernelspec:
 #     display_name: Python 3 (ipykernel)
 #     language: python
 #     name: python3
 # ---
 
 # +
@@ -240,15 +240,14 @@
             return pd.DataFrame(array_normed, index, columns)
         elif output_format == "jax":
             return jnp.array(array_normed)
         else:
             return array_normed
 
     def decode(array_scaled):
-
         value = scaler.inverse_transform(array_scaled)
 
         if output_format == "dataframe":
             return pd.DataFrame(value, index, columns)
         else:
             return value
 
@@ -328,15 +327,14 @@
 # split_feature_target(dataframe)
 # -
 
 
 def split_train_validation(
     dataframe, train_size, look_back, scaler: Optional[Callable] = None
 ) -> TrainSplit:
-
     # prepare scaler
     train_df = dataframe.iloc[:train_size]
 
     if scaler:
         scaler = scaler(train_df)
 
     # prepare train data
@@ -555,14 +553,15 @@
 # + [markdown] colab_type="text" id="yr7jrOL3ki-b"
 # ### Sampling
 #
 # The point of training models is so that they can make predictions! How can we generate predictions with the trained model?
 #
 # If we're allowed to feed in the ground truth, we can just run the original model's `apply` function.
 
+
 # + colab={} colab_type="code" id="f2qETEqXLT1N"
 def plot_samples(truth: np.ndarray, prediction: np.ndarray) -> gg.ggplot:
     assert truth.shape == prediction.shape
     df = pd.DataFrame(
         {"truth": truth.squeeze(), "predicted": prediction.squeeze()}
     ).reset_index()
     df = pd.melt(df, id_vars=["index"], value_vars=["truth", "predicted"])
@@ -589,14 +588,15 @@
 # -
 
 # ### Run autoregressively
 
 # + [markdown] colab_type="text" id="tDyGshz_lwrM"
 # If we can't feed in the ground truth (because we don't have it), we can also run the model autoregressively.
 
+
 # + colab={} colab_type="code" id="Cg8oQ75Ulvld"
 def autoregressive_predict(
     trained_params: hk.Params,
     context: jnp.ndarray,
     seq_len: int,
     pbar=False,
 ):
@@ -655,14 +655,15 @@
 # This can be achieved through a combination of two techniques:
 #
 # 1. If we manually give a unique name to a module, we can ensure that the parameters are directed to the right places.
 # 2. If modules are instantiated in the same order, they'll have the same names in different functions.
 #
 # Here, we rely on method #2 to create a fast autoregressive prediction.
 
+
 # + colab_type="text" id="qGkr2gf2oALo"
 @hk.transform
 def fast_autoregressive_predict_fn(context, seq_len):
     """Given a context, autoregressively generate the rest of a sine wave."""
     core = hk.LSTM(32)
     dense = hk.Linear(1)
     state = core.initial_state(context.shape[0])
```

### Comparing `wax-ml-0.6.3/docs/notebooks/06_Online_Linear_Regression.py` & `wax-ml-0.6.4/docs/notebooks/06_Online_Linear_Regression.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # jupyter:
 #   jupytext:
 #     formats: ipynb,py,md
 #     text_representation:
 #       extension: .py
 #       format_name: light
 #       format_version: '1.5'
-#       jupytext_version: 1.13.3
+#       jupytext_version: 1.14.5
 #   kernelspec:
 #     display_name: Python 3 (ipykernel)
 #     language: python
 #     name: python3
 # ---
 
 # +
@@ -248,15 +248,14 @@
 # For the evaluation of the reward, we need the `Lag` module to evaluate the action of
 # the agent with the labels generated in the previous time step.
 
 from wax.modules import Lag
 
 
 def stationary_linear_regression_env(action, raw_obs):
-
     # Only the environment now the true value of the parameters
     w_true = -jnp.ones(3)
 
     # The environment has its proper loss definition
     def loss(y_pred, y):
         return jnp.mean(jnp.square(y_pred - y))
 
@@ -335,15 +334,14 @@
 # Now, let's implement a non-stationary environment.
 #
 # We implement it so that the sign of the weight is reversed after 2000$ steps.
 
 
 class NonStationaryEnvironment(hk.Module):
     def __call__(self, action, raw_obs):
-
         step = hk.get_state("step", [], init=lambda *_: 0)
 
         # Only the environment now the true value of the parameters
         # at step 2000 we flip the sign of the true parameters !
         w_true = hk.cond(
             step < 2000,
             step,
```

### Comparing `wax-ml-0.6.3/docs/notebooks/07_Online_Time_Series_Prediction.py` & `wax-ml-0.6.4/docs/notebooks/07_Online_Time_Series_Prediction.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # jupyter:
 #   jupytext:
 #     formats: ipynb,py:light,md
 #     text_representation:
 #       extension: .py
 #       format_name: light
 #       format_version: '1.5'
-#       jupytext_version: 1.13.3
+#       jupytext_version: 1.14.5
 #   kernelspec:
 #     display_name: Python 3 (ipykernel)
 #     language: python
 #     name: python3
 # ---
 
 # # 🔄 Online learning for time series prediction 🔄
@@ -105,14 +105,15 @@
 # ## SNARIMAX
 #
 
 # Let's setup an online model to try to learn the dynamic of the time-series.
 
 # First let's run the filter with it's initial random weights.
 
+
 # +
 def predict(y, X=None):
     return SNARIMAX(10, 0, 0)(y, X)
 
 
 sim = unroll_transform_with_state(predict)
 rng = jax.random.PRNGKey(42)
@@ -283,15 +284,14 @@
 # ### Agent
 
 # Let's build an agent:
 
 from optax._src.base import OptState
 
 
-# + tags=[]
 def build_agent(time_series_model=None, opt=None, embargo=1):
     if time_series_model is None:
         time_series_model = lambda y, X: SNARIMAX(10)(y, X)
 
     if opt is None:
         opt = optax.sgd(1.0e-3)
 
@@ -345,17 +345,14 @@
             return y_pred, AgentInfo(opt_info, forecast_info)
 
         return learn_and_forecast(y, X)
 
     return agent
 
 
-# -
-
-
 agent = build_agent()
 
 
 # ### Gym loop
 #
 #
 #
@@ -593,15 +590,14 @@
     res[optimizer.__name__] = _res
 # -
 
 ax = None
 BEST_STEP_SIZE = {}
 BEST_GYM = {}
 for name, (gym, info) in res.items():
-
     loss = pd.DataFrame(-gym.reward, columns=STEP_SIZE).iloc[-5000:].mean()
 
     BEST_STEP_SIZE[name] = loss.idxmin()
     best_idx = loss.reset_index(drop=True).idxmin()
     BEST_GYM[name] = jax.tree_util.tree_map(lambda x: x[:, best_idx], gym)
 
     ax = loss[loss < 0.15].plot(logx=True, logy=False, ax=ax, label=name)
```

### Comparing `wax-ml-0.6.3/docs/notebooks/08_Online_learning_in_non_stationary_environments.py` & `wax-ml-0.6.4/docs/notebooks/08_Online_learning_in_non_stationary_environments.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # jupyter:
 #   jupytext:
 #     formats: ipynb,py:light,md
 #     text_representation:
 #       extension: .py
 #       format_name: light
 #       format_version: '1.5'
-#       jupytext_version: 1.13.3
+#       jupytext_version: 1.14.5
 #   kernelspec:
 #     display_name: Python 3 (ipykernel)
 #     language: python
 #     name: python3
 # ---
 
 # # 🔄 Online learning in non-stationary environments 🔄
@@ -155,15 +155,14 @@
 #
 #
 #
 #
 
 
 def scan_hparams_first_order():
-
     STEP_SIZE_idx = pd.Index(onp.logspace(-4, 1, N_STEP_SIZE), name="step_size")
     STEP_SIZE = jax.device_put(STEP_SIZE_idx.values)
 
     rng = jax.random.PRNGKey(42)
     eps = sample_noise(rng)
 
     res = {}
@@ -183,15 +182,14 @@
         res[optimizer.__name__] = _res
 
     ax = None
     BEST_STEP_SIZE = {}
     BEST_GYM = {}
 
     for name, (gym, info) in res.items():
-
         loss = (
             pd.DataFrame(-gym.reward, columns=STEP_SIZE).iloc[LEARN_TIME_SLICE].mean()
         )
 
         BEST_STEP_SIZE[name] = loss.idxmin()
 
         best_idx = jnp.argmax(gym.reward[LEARN_TIME_SLICE].mean(axis=0))
@@ -229,15 +227,14 @@
             ax=ax,
             color=COLORS[i],
             label=(f"(TRAIN) -  {name}    " f"-    $\eta$={BEST_STEP_SIZE[name]:.2e}"),
             style="--",
         )
 
     for i, optimizer in enumerate(tqdm(OPTIMIZERS)):
-
         name = optimizer.__name__
 
         def gym_loop(eps):
             return GymFeedback(build_agent(opt=optimizer(BEST_STEP_SIZE[name])), env)(
                 eps
             )
 
@@ -378,15 +375,14 @@
 
     def measure(reward):
         return pd.Series(-reward).expanding().mean()
 
     MESURES.append(("Expanding means", measure))
 
     for MEASURE_NAME, MEASUR_FUNC in MESURES:
-
         plt.figure()
 
         for i, (name, gym) in enumerate(BEST_GYM.items()):
             MEASUR_FUNC(gym.reward).plot(
                 label=f"{name}    -    $\eta$={BEST_STEP_SIZE[name]:.2e}",
                 ylim=(MIN_ERR, MAX_ERR),
                 color=COLORS[i],
@@ -457,14 +453,15 @@
 # ### Conclusions
 #
 # - The NEWTON and ADAGRAD optimizers are the faster to converge.
 # - The SGD and ADAM optimizers have the worst performance.
 
 # ### Fixed setting
 
+
 # +
 @add_batch
 def gym_loop_newton(eps):
     return GymFeedback(build_agent(opt=newton(0.1, eps=0.3)), env)(eps)
 
 
 def run_fixed_setting():
```

### Comparing `wax-ml-0.6.3/setup.cfg` & `wax-ml-0.6.4/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.6.3
+current_version = 0.6.4
 commit = True
 tag = True
 
 [metadata]
 name = wax-ml
 version = attr: wax.__version__
 author = WAX-ML Authors
@@ -29,15 +29,15 @@
 	Topic :: Scientific/Engineering
 
 [options]
 packages = find_namespace:
 zip_safe = False  # https://mypy.readthedocs.io/en/latest/installed_packages.html
 include_package_data = True
 install_requires = 
-	numpy < 1.22, >=1.18
+	numpy
 	pandas
 	seaborn
 	xarray >= 0.18.0
 	scikit-learn
 	tqdm
 	jaxlib
 	jax
@@ -63,15 +63,15 @@
 	flaky
 	coverage
 	flake8
 	autopep8
 	autoflake
 	black
 	isort>=5.3.0
-	jupytext<=1.13.3
+	jupytext
 	papermill
 	line_profiler
 complete = 
 	%(optional)s
 	%(dev)s
 docs = 
 	%(complete)s
@@ -95,18 +95,18 @@
 	py.typed
 	tests/data/*
 	static/css/*
 	static/html/*
 
 [flake8]
 ignore = 
-	E203 # whitespace before ':' - doesn't work well with black
-	E501 # line too long - let black worry about that
-	W503 # line break before binary operator
-	C901 # code is too complex
+	E203,
+	E501,
+	W503,
+	C901,
 select = B,C,E,F
 max-line-length = 100
 max-complexity = 15
 exclude = docs
 
 [isort]
 profile = black
```

### Comparing `wax-ml-0.6.3/setup.py` & `wax-ml-0.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/__init__.py` & `wax-ml-0.6.4/wax/__init__.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/accessors.py` & `wax-ml-0.6.4/wax/accessors.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/accessors_test.py` & `wax-ml-0.6.4/wax/accessors_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,28 +201,26 @@
     register_wax_accessors()
     data = prepare_format_data(format)
     ema, state = data.wax.ewm(alpha=0.1, adjust=True, return_state=True).mean()
     check_ema_state(state, ref_count=124)
 
 
 def _compute_ewma_direct(dataarray):
-
     x = jnp.array(dataarray.values, dtype=jnp.float64)
 
     @hk.transform_with_state
     def model(x):
         return EWMA(alpha=0.1, adjust=True)(x)
 
     ema3, state3 = unroll(model, return_final_state=True)(x)
     return ema3, state3
 
 
 @pytest.mark.parametrize("format", ["dataframe"])
 def test_wax_ewma_vs_pandas(format):
-
     config.update("jax_enable_x64", True)
     register_wax_accessors()
     data = prepare_format_data(format)
 
     pandas_ema = data.unstack().ewm(alpha=0.1, adjust=True).mean().stack()
     ema = data.wax.ewm(alpha=0.1, adjust=True).mean()
     ema2, state = data.wax.ewm(alpha=0.1, adjust=True, return_state=True).mean()
```

### Comparing `wax-ml-0.6.3/wax/compile.py` & `wax-ml-0.6.4/wax/compile.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/datasets/__init__.py` & `wax-ml-0.6.4/wax/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/datasets/generate_temperature_data.py` & `wax-ml-0.6.4/wax/datasets/generate_temperature_data.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/datasets/generate_temperature_data_test.py` & `wax-ml-0.6.4/wax/datasets/generate_temperature_data_test.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/encode.py` & `wax-ml-0.6.4/wax/encode.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,14 @@
     # return pd.to_datetime(time).round(freq).to_numpy().astype("<M8[ns]")
 
     # v2
     # return pd.Series(time).dt.floor(freq).values.reshape(time.shape).astype("<M8[ns]")
 
 
 def string_encoder(values: Any) -> Encoder:
-
     ravel = False
     original_shape = None
 
     if values.ndim > 1:
         ravel = True
         original_shape = values.shape
         values = values.ravel()
```

### Comparing `wax-ml-0.6.3/wax/encode_test.py` & `wax-ml-0.6.4/wax/encode_test.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/format.py` & `wax-ml-0.6.4/wax/format.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/format_test.py` & `wax-ml-0.6.4/wax/format_test.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/gym/__init__.py` & `wax-ml-0.6.4/wax/gym/__init__.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/gym/agent.py` & `wax-ml-0.6.4/wax/gym/agent.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/gym/agent_test.py` & `wax-ml-0.6.4/wax/gym/agent_test.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/gym/callbacks/__init__.py` & `wax-ml-0.6.4/wax/gym/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/gym/callbacks/callbacks.py` & `wax-ml-0.6.4/wax/gym/callbacks/callbacks.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/gym/callbacks/callbacks_test.py` & `wax-ml-0.6.4/wax/gym/callbacks/callbacks_test.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/gym/callbacks/progressbar.py` & `wax-ml-0.6.4/wax/gym/callbacks/progressbar.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/gym/callbacks/record.py` & `wax-ml-0.6.4/wax/gym/callbacks/record.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,14 @@
         self._dates: List = []
         self._env: Dict = {}
 
     def _on_step(self, env, agent, gym_state):
         if gym_state.done:
             return
         if gym_state.action is not None:
-
             outputs = self.GymOutput.format(
                 gym_state.rw, gym_state.obs, gym_state.action
             )
             outputs, treedef = tree_flatten(outputs)
             if self._sequence is None:
                 self._treedef = treedef
                 self._sequence = tuple([] for _ in outputs)
```

### Comparing `wax-ml-0.6.3/wax/gym/callbacks/stop.py` & `wax-ml-0.6.4/wax/gym/callbacks/stop.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/gym/entity.py` & `wax-ml-0.6.4/wax/gym/entity.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/gym/env.py` & `wax-ml-0.6.4/wax/gym/env.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/gym/env_test.py` & `wax-ml-0.6.4/wax/gym/env_test.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/gym/gym_unroll.py` & `wax-ml-0.6.4/wax/gym/gym_unroll.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 
     gym_state
         nested data structure
     """
     GymUnrollState = namedtuple("GymUnrollState", "rw, obs, action, done, info")
 
     with local_callbacks(callbacks) as callbacks:
-
         # unpack callbacks
         (
             on_train_start_cbs,
             on_act_cbs,
             on_step_cbs,
             on_train_end_cbs,
         ) = unpack_callbacks(callbacks)
@@ -54,15 +53,14 @@
         obs = env.reset() if obs is None else obs
 
         # call "on_train_start" callbacks
         for on_train_start in on_train_start_cbs:
             on_train_start(env, agent, obs)
 
         while True:
-
             # agent act
             action = agent(obs)
 
             # call "on_act" callbacks
             for on_act in on_act_cbs:
                 on_act(env, agent, obs, action)
```

### Comparing `wax-ml-0.6.3/wax/gym/haiku_agent.py` & `wax-ml-0.6.4/wax/gym/haiku_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 
     def reset(self):
         self._params = None
         self._state = None
         self._initialized = False
 
     def __call__(self, obs):
-
         if not self._initialized:
             self._initialize(obs)
 
         action, self._state = self.agent.apply(
             self._params, self._state, next(self._seq), obs
         )
         return action
```

### Comparing `wax-ml-0.6.3/wax/gym/haiku_env.py` & `wax-ml-0.6.4/wax/gym/haiku_env.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/gym/haiku_env_test.py` & `wax-ml-0.6.4/wax/gym/haiku_env_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,14 @@
 
     @partial(HaikuAgent, name="Agent")
     @hk.transform_with_state
     def agent(obs):
         return Agent()(obs)
 
     with Record() as rec, ProgressBar():
-
         state = agent.unroll(env)
 
     assert isinstance(state.action["structured_action"], np.ndarray)
     assert state.action["structured_action"] == 55
 
     outputs = rec.get_outputs()
     assert isinstance(outputs.reward, np.ndarray)
@@ -159,15 +158,14 @@
 
     @partial(HaikuAgent, name="Agent")
     @hk.transform_with_state
     def agent(obs):
         return Agent()(obs)
 
     with Record() as rec, ProgressBar():
-
         state = agent.unroll(env)
 
     assert isinstance(state.action["structured_action"], pd.DataFrame)
     assert state.action["structured_action"].values == 55
 
     outputs = rec.get_outputs()
     assert isinstance(outputs.reward, pd.DataFrame)
@@ -184,15 +182,14 @@
 
     @partial(HaikuAgent, name="Agent")
     @hk.transform_with_state
     def agent(obs):
         return Agent()(obs)
 
     with Record() as rec, ProgressBar(), Stop(3):
-
         state = agent.unroll(env)
 
     assert isinstance(state.action["structured_action"], pd.DataFrame)
     assert state.action["structured_action"].values == 6
 
     outputs = rec.get_outputs()
     assert isinstance(outputs.reward, pd.DataFrame)
@@ -207,15 +204,14 @@
 
     @partial(HaikuAgent, name="Agent")
     @hk.transform_with_state
     def agent(obs):
         return Agent()(obs)
 
     with Record() as rec, ProgressBar(), Stop(3):
-
         state = agent.unroll(env)
 
     assert isinstance(state.action["structured_action"], xr.DataArray)
     assert state.action["structured_action"].values == 6
 
     outputs = rec.get_outputs()
     assert isinstance(outputs.reward, xr.DataArray)
```

### Comparing `wax-ml-0.6.3/wax/modules/__init__.py` & `wax-ml-0.6.4/wax/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/apply_mask.py` & `wax-ml-0.6.4/wax/modules/apply_mask.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/apply_mask_test.py` & `wax-ml-0.6.4/wax/modules/apply_mask_test.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/arma.py` & `wax-ml-0.6.4/wax/modules/arma.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/arma_test.py` & `wax-ml-0.6.4/wax/modules/arma_test.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/buffer.py` & `wax-ml-0.6.4/wax/modules/buffer.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/buffer_test.py` & `wax-ml-0.6.4/wax/modules/buffer_test.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/counter.py` & `wax-ml-0.6.4/wax/modules/counter.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/counter_test.py` & `wax-ml-0.6.4/wax/modules/counter_test.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/diff.py` & `wax-ml-0.6.4/wax/modules/diff.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/diff_test.py` & `wax-ml-0.6.4/wax/modules/diff_test.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/ewma.py` & `wax-ml-0.6.4/wax/modules/ewma.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/ewma_test.py` & `wax-ml-0.6.4/wax/modules/ewma_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 from wax.compile import jit_init_apply
 from wax.modules.ewma import EWMA
 from wax.unroll import dynamic_unroll_fori_loop, unroll, unroll_transform_with_state
 
 
 @pytest.mark.parametrize("dtype", ["float32", "float64"])
 def test_init_and_first_step_ema(dtype):
-
     if dtype == "float64":
         config.update("jax_enable_x64", True)
     else:
         config.update("jax_enable_x64", False)
 
     seq = hk.PRNGSequence(42)
     x = jax.random.normal(shape=(3,), key=next(seq), dtype=jnp.float64)
@@ -44,15 +43,14 @@
 
     params, state = model.init(next(seq), x)
     ema, state = model.apply(params, state, next(seq), x)
     assert ema.dtype == jnp.dtype(dtype)
 
 
 def test_run_ema_vs_pandas_not_adjust():
-
     config.update("jax_enable_x64", True)
 
     seq = hk.PRNGSequence(42)
     x = jax.random.normal(shape=(10, 3), key=next(seq), dtype=jnp.float64)
 
     @jit_init_apply
     @hk.transform_with_state
@@ -63,15 +61,14 @@
 
     pandas_ema = pd.DataFrame(x).ewm(alpha=0.1, adjust=False).mean()
 
     assert jnp.allclose(ema, pandas_ema.values)
 
 
 def test_dynamic_unroll_fori_loop():
-
     config.update("jax_enable_x64", True)
 
     seq = hk.PRNGSequence(42)
     x = jax.random.normal(shape=(10, 3), key=next(seq), dtype=jnp.float64)
 
     @jit_init_apply
     @hk.transform_with_state
@@ -82,15 +79,14 @@
 
     ema2, state2 = dynamic_unroll_fori_loop(model, None, None, next(seq), False, x)
 
     assert jnp.allclose(ema, ema2)
 
 
 def test_dynamic_unroll():
-
     config.update("jax_enable_x64", True)
 
     seq = hk.PRNGSequence(42)
     x = jax.random.normal(shape=(10, 3), key=next(seq), dtype=jnp.float64)
 
     @jit_init_apply
     @hk.transform_with_state
@@ -102,15 +98,14 @@
     seq = hk.PRNGSequence(42)
     ema2, state2 = unroll(model, return_final_state=True)(x)
 
     assert jnp.allclose(ema, ema2)
 
 
 def test_run_ema_vs_pandas_adjust():
-
     config.update("jax_enable_x64", True)
 
     seq = hk.PRNGSequence(42)
     x = jax.random.normal(shape=(10, 3), key=next(seq), dtype=jnp.float64)
 
     @jit_init_apply
     @hk.transform_with_state
@@ -141,15 +136,14 @@
     assert not jnp.allclose(ema, pandas_ema_not_adjust.values)
     corr = jnp.corrcoef(ema.flatten(), pandas_ema_adjust.values.flatten())[0, 1]
     assert 1.0e-3 < 1 - corr < 1.0e-2
 
 
 @pytest.mark.parametrize("adjust", [False, True, "linear"])
 def test_grad_ewma(adjust):
-
     rng = jax.random.PRNGKey(42)
     x = jax.random.normal(rng, (10, 3))
     # put some nan values
     x = x.at[0].set(jnp.nan)
 
     _, rng = jax.random.split(rng)
```

### Comparing `wax-ml-0.6.3/wax/modules/ewmcov.py` & `wax-ml-0.6.4/wax/modules/ewmcov.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/ewmcov_test.py` & `wax-ml-0.6.4/wax/modules/ewmcov_test.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/ewmvar.py` & `wax-ml-0.6.4/wax/modules/ewmvar.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/ewmvar_test.py` & `wax-ml-0.6.4/wax/modules/ewmvar_test.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/ffill.py` & `wax-ml-0.6.4/wax/modules/ffill.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/ffill_test.py` & `wax-ml-0.6.4/wax/modules/ffill_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,11 +16,10 @@
 
 from wax.modules import Ffill
 from wax.unroll import unroll
 
 
 @pytest.mark.parametrize("use_jit", [False, True])
 def test_ffill(use_jit):
-
     xs = jnp.array([90, 91, jnp.nan, 85])
     res = unroll(lambda x: Ffill()(x))(xs)
     assert jnp.allclose(res, jnp.array([90, 91, 91, 85], dtype=jnp.float32))
```

### Comparing `wax-ml-0.6.3/wax/modules/fill_nan_inf.py` & `wax-ml-0.6.4/wax/modules/fill_nan_inf.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/fill_nan_inf_test.py` & `wax-ml-0.6.4/wax/modules/fill_nan_inf_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import jax
 import jax.numpy as jnp
 
 from wax.modules.fill_nan_inf import FillNanInf
 
 
 def test_fill_nan_inf():
-
     seq = hk.PRNGSequence(42)
     x = jax.random.normal(shape=(100, 5), key=next(seq), dtype=jnp.float64)
     mask_nan = jax.random.choice(next(seq), 2, shape=x.shape)
     x = jnp.where(mask_nan, x, jnp.nan)
     del mask_nan
 
     mask_inf = jax.random.choice(next(seq), 2, shape=x.shape)
```

### Comparing `wax-ml-0.6.3/wax/modules/func_optimizer.py` & `wax-ml-0.6.4/wax/modules/func_optimizer.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/func_optimizer_test.py` & `wax-ml-0.6.4/wax/modules/func_optimizer_test.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/gym_feedback.py` & `wax-ml-0.6.4/wax/modules/gym_feedback.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/gym_feedback_test.py` & `wax-ml-0.6.4/wax/modules/gym_feedback_test.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/has_changed.py` & `wax-ml-0.6.4/wax/modules/has_changed.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/lag.py` & `wax-ml-0.6.4/wax/modules/lag.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/lag_test.py` & `wax-ml-0.6.4/wax/modules/lag_test.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/mask_mean.py` & `wax-ml-0.6.4/wax/modules/mask_mean.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/mask_mean_test.py` & `wax-ml-0.6.4/wax/modules/mask_mean_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,29 +15,27 @@
 import jax
 import jax.numpy as jnp
 
 from wax.modules.mask_mean import MaskMean
 
 
 def test_mask_mean_no_mask():
-
     rng = hk.PRNGSequence(42)
     x = jax.random.normal(next(rng), (10,))
     x_mean_ref = x.mean()
 
     fun = hk.transform(lambda mask, x: MaskMean()(mask, x))
     mask = jnp.full(x.shape, True)
 
     params = fun.init(next(rng), mask, x)
     x_mean = fun.apply(params, next(rng), mask, x)
     assert jnp.allclose(x_mean, x_mean_ref)
 
 
 def test_mask_mean_with_mask():
-
     rng = hk.PRNGSequence(42)
     x = jax.random.normal(next(rng), (10,))
     x_mean_ref = x[1:].mean()
 
     fun = hk.transform(lambda mask, x: MaskMean()(mask, x))
 
     mask = jnp.full(x.shape, True)
```

### Comparing `wax-ml-0.6.3/wax/modules/mask_normalize.py` & `wax-ml-0.6.4/wax/modules/mask_normalize.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/mask_normalize_test.py` & `wax-ml-0.6.4/wax/modules/mask_normalize_test.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/mask_std.py` & `wax-ml-0.6.4/wax/modules/mask_std.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/mask_std_test.py` & `wax-ml-0.6.4/wax/modules/mask_std_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,30 +16,28 @@
 import jax.numpy as jnp
 import pytest
 
 from wax.modules.mask_std import MaskStd
 
 
 def test_mask_std_no_mask():
-
     rng = hk.PRNGSequence(42)
     x = jax.random.normal(next(rng), (10,))
     std_ref = x.std()
 
     fun = hk.transform(lambda mask, x: MaskStd()(mask, x))
     mask = jnp.full(x.shape, True)
 
     params = fun.init(next(rng), mask, x)
     x_std = fun.apply(params, next(rng), mask, x)
     assert jnp.allclose(x_std, std_ref)
 
 
 @pytest.mark.parametrize("assume_centered", [False, True])
 def test_mask_std_with_mask(assume_centered):
-
     rng = hk.PRNGSequence(42)
     x = jax.random.normal(next(rng), (10,))
     if assume_centered:
         x_std_ref = jnp.sqrt((x[1:] ** 2).mean())
     else:
         x_std_ref = x[1:].std()
```

### Comparing `wax-ml-0.6.3/wax/modules/ohlc.py` & `wax-ml-0.6.4/wax/modules/ohlc.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/ohlc_test.py` & `wax-ml-0.6.4/wax/modules/ohlc_test.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/online_optimizer.py` & `wax-ml-0.6.4/wax/modules/online_optimizer.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/online_supervised_learner.py` & `wax-ml-0.6.4/wax/modules/online_supervised_learner.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/online_supervised_learner_test.py` & `wax-ml-0.6.4/wax/modules/online_supervised_learner_test.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/optax_optimizer.py` & `wax-ml-0.6.4/wax/modules/optax_optimizer.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/pct_change.py` & `wax-ml-0.6.4/wax/modules/pct_change.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/pct_change_test.py` & `wax-ml-0.6.4/wax/modules/pct_change_test.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/rolling_mean.py` & `wax-ml-0.6.4/wax/modules/rolling_mean.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/rolling_mean_test.py` & `wax-ml-0.6.4/wax/modules/rolling_mean_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 
     x = jax.random.normal(next(seq), (2, 3))
     output, state = rolling_mean.apply(params, state, next(seq), x)
     assert ((x2 + x) / 2 == output).all()
 
 
 def test_run_ema_vs_pandas_not_adjust(window=10, min_periods=5):
-
     config.update("jax_enable_x64", True)
 
     seq = hk.PRNGSequence(42)
     x = jax.random.normal(shape=(100, 5), key=next(seq), dtype=jnp.float64)
     mask = jax.random.choice(next(seq), 2, shape=x.shape)
     x = jnp.where(mask, x, jnp.nan)
```

### Comparing `wax-ml-0.6.3/wax/modules/snarimax.py` & `wax-ml-0.6.4/wax/modules/snarimax.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/snarimax_test.py` & `wax-ml-0.6.4/wax/modules/snarimax_test.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/update_on_event.py` & `wax-ml-0.6.4/wax/modules/update_on_event.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/update_on_event_test.py` & `wax-ml-0.6.4/wax/modules/update_on_event_test.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/update_params.py` & `wax-ml-0.6.4/wax/modules/update_params.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/vmap.py` & `wax-ml-0.6.4/wax/modules/vmap.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/modules/vmap_test.py` & `wax-ml-0.6.4/wax/modules/vmap_test.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/numba/__init__.py` & `wax-ml-0.6.4/wax-numba/__init__.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/numba/ewma_numba.py` & `wax-ml-0.6.4/wax-numba/ewma_numba.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/numba/ewma_numba_test.py` & `wax-ml-0.6.4/wax-numba/ewma_numba_test.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/optim/__init__.py` & `wax-ml-0.6.4/wax/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/optim/newton.py` & `wax-ml-0.6.4/wax/optim/newton.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/optim/newton_test.py` & `wax-ml-0.6.4/wax/optim/newton_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     return -(w * x).sum() + (w**2).sum()
 
 
 # from optax import sgd, adagrad
 
 
 def test_sgd():
-
     w = jnp.ones(3)
     x = jnp.ones(3)
 
     l_ = loss(w, x)
 
     # opt = sgd(1.0e-3)
     # opt = adagrad(1.0e-3)
```

### Comparing `wax-ml-0.6.3/wax/predicate.py` & `wax-ml-0.6.4/wax/predicate.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/stateful.py` & `wax-ml-0.6.4/wax/stateful.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
 
 def vmap_lift_with_state(fun: Callable, split_rng=False, init_rng=True):
     if split_rng and not init_rng:
         raise ValueError("split_rng=True requires init_rng=True")
 
     def apply_fn(*args, **kwargs):
-
         tfun = hk.transform_with_state(fun)
 
         if not split_rng:
             rng = hk.next_rng_key() if (hk.running_init() and init_rng) else None
 
             @jax.vmap
             def init_fn(*args, **kwargs):
```

### Comparing `wax-ml-0.6.3/wax/stateful_test.py` & `wax-ml-0.6.4/wax/stateful_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
         return state + x
 
 
 @pytest.mark.parametrize(
     "init_rng, split_rng", [[False, False], [True, False], [True, True]]
 )
 def test_vmap_lift_wtih_state(init_rng, split_rng):
-
     x = jnp.arange(3).astype(jnp.float32)
 
     def run_vmap():
         def outer_fun(x):
             def fun(x):
                 return MyModule(steps=2)(x)
```

### Comparing `wax-ml-0.6.3/wax/stream.py` & `wax-ml-0.6.4/wax/stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,15 +323,15 @@
             return [[]] * num_leaves
         else:
             return list(map(lambda x: [x], obs_flat))
 
     outputs = _init_outputs()
 
     if pbar:
-        stream = tqdm(stream, desc="stream_unroll")
+        stream = tqdm(stream, desc="stream_unroll")  # type: ignore
 
     for obs in stream:
         obs_flat = tree_leaves(obs)
         assert len(obs_flat) == num_leaves
         for y, x in zip(outputs, obs_flat):
             y.append(x)
 
@@ -713,15 +713,14 @@
                         output[time_dim] = buffer_output
                         if _is_verbose(self.verbose, time_dim):
                             print(f"'{time_dim}' proceed data : {stream_timestamp}")
 
                 if _is_verbose(self.verbose, time_dim):
 
                     def as_list(vals):
-
                         vals = onp.array(vals)
                         if vals.ndim == 2:
                             idx = onp.stack([vals[i] for i in range(len(vals))])
                             return pd.DataFrame(output[time_dim].value, index=idx)
                         idx = vals
                         return (output[time_dim].value, idx)
```

### Comparing `wax-ml-0.6.3/wax/stream_test.py` & `wax-ml-0.6.4/wax/stream_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,14 @@
     ]
 
     ref = index["day"].value[name_air].tolist()[20:30]
     assert (ref == array([-99999, -99999, -99999, -99999, 0, 0, 0, 0, 0, 0])).all()
 
 
 def check_outputs(outputs, schema):
-
     # TODO: check what is correct...
     # assert outputs["NEWS"].shape == (25, 3, 2)
     assert outputs["NEWS"].shape == (124, 3)
     assert_tree_all_close(
         outputs["NEWS"][-1],
         DeviceArray([-99999, -99999, -99999], dtype=int32),
     )
```

### Comparing `wax-ml-0.6.3/wax/testing.py` & `wax-ml-0.6.4/wax/testing.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/transform.py` & `wax-ml-0.6.4/wax/transform.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/unroll.py` & `wax-ml-0.6.4/wax/unroll.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/unroll_test.py` & `wax-ml-0.6.4/wax/unroll_test.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax/utils.py` & `wax-ml-0.6.4/wax/utils.py`

 * *Files identical despite different names*

### Comparing `wax-ml-0.6.3/wax_ml.egg-info/PKG-INFO` & `wax-ml-0.6.4/wax_ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wax-ml
-Version: 0.6.3
+Version: 0.6.4
 Summary: A Python library for machine-learning and feedback loops on streaming data
 Home-page: https://github.com/eserie/wax-ml
 Author: WAX-ML Authors
 Author-email: eserie@gmail.com
 License: Apache
 Keywords: time series,machine learning,optimization,optimal control,online learning,reinforcement learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `wax-ml-0.6.3/wax_ml.egg-info/SOURCES.txt` & `wax-ml-0.6.4/wax_ml.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,17 @@
 wax/stream.py
 wax/stream_test.py
 wax/testing.py
 wax/transform.py
 wax/unroll.py
 wax/unroll_test.py
 wax/utils.py
+wax-numba/__init__.py
+wax-numba/ewma_numba.py
+wax-numba/ewma_numba_test.py
 wax/datasets/__init__.py
 wax/datasets/generate_temperature_data.py
 wax/datasets/generate_temperature_data_test.py
 wax/gym/__init__.py
 wax/gym/agent.py
 wax/gym/agent_test.py
 wax/gym/entity.py
@@ -99,17 +102,14 @@
 wax/modules/snarimax.py
 wax/modules/snarimax_test.py
 wax/modules/update_on_event.py
 wax/modules/update_on_event_test.py
 wax/modules/update_params.py
 wax/modules/vmap.py
 wax/modules/vmap_test.py
-wax/numba/__init__.py
-wax/numba/ewma_numba.py
-wax/numba/ewma_numba_test.py
 wax/optim/__init__.py
 wax/optim/newton.py
 wax/optim/newton_test.py
 wax_ml.egg-info/PKG-INFO
 wax_ml.egg-info/SOURCES.txt
 wax_ml.egg-info/dependency_links.txt
 wax_ml.egg-info/not-zip-safe
```

### Comparing `wax-ml-0.6.3/wax_ml.egg-info/requires.txt` & `wax-ml-0.6.4/wax_ml.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-numpy<1.22,>=1.18
+numpy
 pandas
 seaborn
 xarray>=0.18.0
 scikit-learn
 tqdm
 jaxlib
 jax
@@ -26,15 +26,15 @@
 flaky
 coverage
 flake8
 autopep8
 autoflake
 black
 isort>=5.3.0
-jupytext<=1.13.3
+jupytext
 papermill
 line_profiler
 
 [dev]
 mypy
 ipykernel
 ipywidgets
@@ -46,15 +46,15 @@
 flaky
 coverage
 flake8
 autopep8
 autoflake
 black
 isort>=5.3.0
-jupytext<=1.13.3
+jupytext
 papermill
 line_profiler
 
 [docs]
 optax
 plotnine
 pyarrow
@@ -72,15 +72,15 @@
 flaky
 coverage
 flake8
 autopep8
 autoflake
 black
 isort>=5.3.0
-jupytext<=1.13.3
+jupytext
 papermill
 line_profiler
 sphinx
 sphinxcontrib-napoleon
 sphinx_rtd_theme
 sphinx-autodoc-typehints
 sphinx-autosummary-accessors
```

