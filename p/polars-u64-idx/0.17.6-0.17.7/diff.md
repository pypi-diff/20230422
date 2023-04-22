# Comparing `tmp/polars_u64_idx-0.17.6.tar.gz` & `tmp/polars_u64_idx-0.17.7.tar.gz`

## Comparing `polars_u64_idx-0.17.6.tar` & `polars_u64_idx-0.17.7.tar`

### file list

```diff
@@ -1,1098 +1,1098 @@
--rw-r--r--   0        0        0     1765 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/LICENSE
--rw-r--r--   0     1001      123       98 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/mod.rs
--rw-r--r--   0     1001      123     1219 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/operators/filter.rs
--rw-r--r--   0     1001      123     4103 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/operators/function.rs
--rw-r--r--   0     1001      123      229 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/operators/mod.rs
--rw-r--r--   0     1001      123      548 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs
--rw-r--r--   0     1001      123     3247 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/operators/projection.rs
--rw-r--r--   0     1001      123     2324 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/operators/reproject.rs
--rw-r--r--   0     1001      123     6479 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs
--rw-r--r--   0     1001      123    10473 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs
--rw-r--r--   0     1001      123     1207 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs
--rw-r--r--   0     1001      123     1888 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs
--rw-r--r--   0     1001      123     4554 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs
--rw-r--r--   0     1001      123     1746 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs
--rw-r--r--   0     1001      123     5413 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs
--rw-r--r--   0     1001      123     4951 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs
--rw-r--r--   0     1001      123      211 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mod.rs
--rw-r--r--   0     1001      123      856 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs
--rw-r--r--   0     1001      123     4294 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs
--rw-r--r--   0     1001      123     3030 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs
--rw-r--r--   0     1001      123     6275 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs
--rw-r--r--   0     1001      123    13665 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs
--rw-r--r--   0     1001      123     2681 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs
--rw-r--r--   0     1001      123     2534 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs
--rw-r--r--   0     1001      123     5961 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs
--rw-r--r--   0     1001      123    10673 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs
--rw-r--r--   0     1001      123     2164 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs
--rw-r--r--   0     1001      123     4666 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs
--rw-r--r--   0     1001      123     3906 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs
--rw-r--r--   0     1001      123    20859 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs
--rw-r--r--   0     1001      123    23518 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs
--rw-r--r--   0     1001      123     2457 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs
--rw-r--r--   0     1001      123     8395 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/io.rs
--rw-r--r--   0     1001      123     5485 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs
--rw-r--r--   0     1001      123    14279 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs
--rw-r--r--   0     1001      123    11824 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs
--rw-r--r--   0     1001      123      178 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/joins/mod.rs
--rw-r--r--   0     1001      123     2002 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/memory.rs
--rw-r--r--   0     1001      123      589 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/mod.rs
--rw-r--r--   0     1001      123     1492 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs
--rw-r--r--   0     1001      123     1824 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs
--rw-r--r--   0     1001      123     3108 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/slice.rs
--rw-r--r--   0     1001      123      130 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/sort/mod.rs
--rw-r--r--   0     1001      123     3808 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs
--rw-r--r--   0     1001      123     6295 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs
--rw-r--r--   0     1001      123     5953 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs
--rw-r--r--   0     1001      123     3801 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs
--rw-r--r--   0     1001      123      635 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/utils.rs
--rw-r--r--   0     1001      123     5076 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sources/csv.rs
--rw-r--r--   0     1001      123     1231 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sources/frame.rs
--rw-r--r--   0     1001      123      987 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs
--rw-r--r--   0     1001      123      366 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sources/mod.rs
--rw-r--r--   0     1001      123     3387 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sources/parquet.rs
--rw-r--r--   0     1001      123     1146 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sources/reproject.rs
--rw-r--r--   0     1001      123     1022 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sources/union.rs
--rw-r--r--   0     1001      123      448 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/expressions.rs
--rw-r--r--   0     1001      123      272 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/lib.rs
--rw-r--r--   0     1001      123      719 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/operators/chunks.rs
--rw-r--r--   0     1001      123      474 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/operators/context.rs
--rw-r--r--   0     1001      123      223 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/operators/mod.rs
--rw-r--r--   0     1001      123      430 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/operators/operator.rs
--rw-r--r--   0     1001      123      626 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/operators/sink.rs
--rw-r--r--   0     1001      123      241 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/operators/source.rs
--rw-r--r--   0     1001      123        1 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/pipeline/config.rs
--rw-r--r--   0     1001      123    20481 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/pipeline/convert.rs
--rw-r--r--   0     1001      123    13982 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs
--rw-r--r--   0     1001      123     1237 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/pipeline/mod.rs
--rw-r--r--   0        0        0     2055 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/LICENSE
--rw-r--r--   0     1001      123     3565 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/chunkedarray/date.rs
--rw-r--r--   0     1001      123     6465 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/chunkedarray/datetime.rs
--rw-r--r--   0     1001      123     3305 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/chunkedarray/duration.rs
--rw-r--r--   0     1001      123     5607 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/chunkedarray/kernels.rs
--rw-r--r--   0     1001      123     1062 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/chunkedarray/mod.rs
--rw-r--r--   0     1001      123     7302 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs
--rw-r--r--   0     1001      123     2582 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs
--rw-r--r--   0     1001      123    10476 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs
--rw-r--r--   0     1001      123      428 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/mod.rs
--rw-r--r--   0     1001      123     7368 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs
--rw-r--r--   0     1001      123     2717 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/chunkedarray/time.rs
--rw-r--r--   0     1001      123    21192 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs
--rw-r--r--   0     1001      123    20108 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs
--rw-r--r--   0     1001      123     4115 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs
--rw-r--r--   0     1001      123     9692 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs
--rw-r--r--   0     1001      123     2960 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/date_range.rs
--rw-r--r--   0     1001      123    31413 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/groupby/dynamic.rs
--rw-r--r--   0     1001      123       88 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/groupby/mod.rs
--rw-r--r--   0     1001      123      535 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/lib.rs
--rw-r--r--   0     1001      123      320 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/prelude.rs
--rw-r--r--   0     1001      123     1568 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/round.rs
--rw-r--r--   0     1001      123     4028 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/series/_trait.rs
--rw-r--r--   0     1001      123      136 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/series/implementations/boolean.rs
--rw-r--r--   0     1001      123      140 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/series/implementations/categoricals.rs
--rw-r--r--   0     1001      123      133 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/series/implementations/date.rs
--rw-r--r--   0     1001      123      137 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/series/implementations/datetime.rs
--rw-r--r--   0     1001      123      137 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/series/implementations/duration.rs
--rw-r--r--   0     1001      123     1863 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/series/implementations/floats.rs
--rw-r--r--   0     1001      123     1792 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/series/implementations/integers.rs
--rw-r--r--   0     1001      123      133 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/series/implementations/list.rs
--rw-r--r--   0     1001      123      486 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/series/implementations/mod.rs
--rw-r--r--   0     1001      123      155 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/series/implementations/object.rs
--rw-r--r--   0     1001      123      135 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/series/implementations/struct_.rs
--rw-r--r--   0     1001      123      133 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/series/implementations/time.rs
--rw-r--r--   0     1001      123      133 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/series/implementations/utf8.rs
--rw-r--r--   0     1001      123    12466 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/series/mod.rs
--rw-r--r--   0     1001      123     1630 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/truncate.rs
--rw-r--r--   0     1001      123     7059 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/upsample.rs
--rw-r--r--   0     1001      123     2567 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/utils.rs
--rw-r--r--   0     1001      123     1524 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/windows/bounds.rs
--rw-r--r--   0     1001      123     2008 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/windows/calendar.rs
--rw-r--r--   0     1001      123    23538 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/windows/duration.rs
--rw-r--r--   0     1001      123    20089 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/windows/groupby.rs
--rw-r--r--   0     1001      123      503 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/windows/mod.rs
--rw-r--r--   0     1001      123    24202 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/windows/test.rs
--rw-r--r--   0     1001      123    11624 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-time/src/windows/window.rs
--rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.6/local_dependencies/polars-utils/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-utils/LICENSE
--rw-r--r--   0     1001      123     2645 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/arena.rs
--rw-r--r--   0     1001      123     1373 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/atomic.rs
--rw-r--r--   0     1001      123     2659 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/cell.rs
--rw-r--r--   0     1001      123     1015 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/contention_pool.rs
--rw-r--r--   0     1001      123      509 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/error.rs
--rw-r--r--   0     1001      123      271 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/fmt.rs
--rw-r--r--   0     1001      123      763 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/functions.rs
--rw-r--r--   0     1001      123      514 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/hash.rs
--rw-r--r--   0     1001      123     2709 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/iter/enumerate_idx.rs
--rw-r--r--   0     1001      123       61 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/iter/mod.rs
--rw-r--r--   0     1001      123      583 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/lib.rs
--rw-r--r--   0     1001      123      573 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/macros.rs
--rw-r--r--   0     1001      123      282 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/mem.rs
--rw-r--r--   0     1001      123     1792 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/slice.rs
--rw-r--r--   0     1001      123     2467 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/sort.rs
--rw-r--r--   0     1001      123     1115 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/sync.rs
--rw-r--r--   0     1001      123      504 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/sys.rs
--rw-r--r--   0     1001      123      697 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/unwrap.rs
--rw-r--r--   0     1001      123      616 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/wasm.rs
--rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.6/local_dependencies/polars-error/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-error/LICENSE
--rw-r--r--   0     1001      123     6297 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-error/src/lib.rs
--rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.6/local_dependencies/polars-sql/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-sql/LICENSE
--rw-r--r--   0     1001      123    15314 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-sql/src/context.rs
--rw-r--r--   0     1001      123    17592 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-sql/src/functions.rs
--rw-r--r--   0     1001      123     1920 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-sql/src/keywords.rs
--rw-r--r--   0     1001      123    28145 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-sql/src/lib.rs
--rw-r--r--   0     1001      123    15237 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-sql/src/sql_expr.rs
--rw-r--r--   0     1001      123     4572 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-sql/src/table_functions.rs
--rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/LICENSE
--rw-r--r--   0     1001      123     1975 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/array/default_arrays.rs
--rw-r--r--   0     1001      123     3160 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/array/get.rs
--rw-r--r--   0     1001      123     6171 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/array/list.rs
--rw-r--r--   0     1001      123     7771 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/array/mod.rs
--rw-r--r--   0     1001      123      878 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/array/null.rs
--rw-r--r--   0     1001      123     1125 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/array/slice.rs
--rw-r--r--   0     1001      123     1807 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/array/utf8.rs
--rw-r--r--   0     1001      123     2294 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/bit_util.rs
--rw-r--r--   0     1001      123       17 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/bitmap/mod.rs
--rw-r--r--   0     1001      123      819 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/bitmap/mutable.rs
--rw-r--r--   0     1001      123      232 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/compute/cast.rs
--rw-r--r--   0     1001      123       56 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/compute/mod.rs
--rw-r--r--   0     1001      123     2962 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/compute/take/boolean.rs
--rw-r--r--   0     1001      123    24907 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/compute/take/mod.rs
--rw-r--r--   0     1001      123     1042 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/conversion.rs
--rw-r--r--   0     1001      123     1609 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/data_types.rs
--rw-r--r--   0     1001      123       25 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/error.rs
--rw-r--r--   0     1001      123       28 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/export.rs
--rw-r--r--   0     1001      123       26 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/floats/mod.rs
--rw-r--r--   0     1001      123     2066 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/floats/ord.rs
--rw-r--r--   0     1001      123     1273 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/index.rs
--rw-r--r--   0     1001      123      915 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/is_valid.rs
--rw-r--r--   0     1001      123     4740 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/agg_mean.rs
--rw-r--r--   0     1001      123     1015 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/concatenate.rs
--rw-r--r--   0     1001      123     5161 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/ewm/average.rs
--rw-r--r--   0     1001      123     1808 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs
--rw-r--r--   0     1001      123    25065 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs
--rw-r--r--   0     1001      123     1406 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/float.rs
--rw-r--r--   0     1001      123     4907 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/list.rs
--rw-r--r--   0     1001      123     1895 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs
--rw-r--r--   0     1001      123     9731 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/mod.rs
--rw-r--r--   0     1001      123     3703 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs
--rw-r--r--   0     1001      123     2022 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs
--rw-r--r--   0     1001      123    18684 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs
--rw-r--r--   0     1001      123     3924 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs
--rw-r--r--   0     1001      123    11659 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs
--rw-r--r--   0     1001      123     5504 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs
--rw-r--r--   0     1001      123     8683 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs
--rw-r--r--   0     1001      123     1749 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs
--rw-r--r--   0     1001      123    14367 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs
--rw-r--r--   0     1001      123     9070 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs
--rw-r--r--   0     1001      123    11609 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs
--rw-r--r--   0     1001      123     4698 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs
--rw-r--r--   0     1001      123     8335 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs
--rw-r--r--   0     1001      123     8109 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/window.rs
--rw-r--r--   0     1001      123     4752 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/set.rs
--rw-r--r--   0     1001      123     4529 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/sort_partition.rs
--rw-r--r--   0     1001      123     2948 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs
--rw-r--r--   0     1001      123     5974 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs
--rw-r--r--   0     1001      123      231 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/sorted_join/mod.rs
--rw-r--r--   0     1001      123      841 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/string.rs
--rw-r--r--   0     1001      123     2310 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs
--rw-r--r--   0     1001      123     4343 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs
--rw-r--r--   0     1001      123     2606 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs
--rw-r--r--   0     1001      123     4417 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/time.rs
--rw-r--r--   0     1001      123      341 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/lib.rs
--rw-r--r--   0     1001      123      434 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/prelude.rs
--rw-r--r--   0     1001      123      534 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/slice.rs
--rw-r--r--   0     1001      123      762 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/time_zone.rs
--rw-r--r--   0     1001      123      998 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/trusted_len/boolean.rs
--rw-r--r--   0     1001      123     2821 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/trusted_len/mod.rs
--rw-r--r--   0     1001      123     2533 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs
--rw-r--r--   0     1001      123      158 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/trusted_len/rev.rs
--rw-r--r--   0     1001      123     5020 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/utils.rs
--rw-r--r--   0        0        0     4341 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/LICENSE
--rw-r--r--   0     1001      123     2383 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/avro/mod.rs
--rw-r--r--   0     1001      123     3608 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/avro/read.rs
--rw-r--r--   0     1001      123     2622 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/avro/write.rs
--rw-r--r--   0     1001      123     4505 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/cloud/adaptors.rs
--rw-r--r--   0     1001      123     9506 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/cloud/glob.rs
--rw-r--r--   0     1001      123     3089 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/cloud/mod.rs
--rw-r--r--   0     1001      123    28678 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/csv/buffer.rs
--rw-r--r--   0     1001      123     1898 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/csv/mod.rs
--rw-r--r--   0     1001      123    19712 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/csv/parser.rs
--rw-r--r--   0     1001      123    21432 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/csv/read.rs
--rw-r--r--   0     1001      123    10817 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs
--rw-r--r--   0     1001      123    13909 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs
--rw-r--r--   0     1001      123    31242 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/csv/read_impl/mod.rs
--rw-r--r--   0     1001      123    11466 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/csv/splitfields.rs
--rw-r--r--   0     1001      123    25183 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/csv/utils.rs
--rw-r--r--   0     1001      123     2796 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/csv/write.rs
--rw-r--r--   0     1001      123    13265 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/csv/write_impl.rs
--rw-r--r--   0     1001      123      184 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/export.rs
--rw-r--r--   0     1001      123     7586 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/ipc/ipc_file.rs
--rw-r--r--   0     1001      123     9222 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/ipc/ipc_stream.rs
--rw-r--r--   0     1001      123     3253 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/ipc/mmap.rs
--rw-r--r--   0     1001      123      401 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/ipc/mod.rs
--rw-r--r--   0     1001      123     8282 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/ipc/write.rs
--rw-r--r--   0     1001      123     1471 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/ipc/write_async.rs
--rw-r--r--   0     1001      123    11046 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/json.rs
--rw-r--r--   0     1001      123     4864 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/lib.rs
--rw-r--r--   0     1001      123     1969 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/mmap.rs
--rw-r--r--   0     1001      123     7215 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/ndjson_core/buffer.rs
--rw-r--r--   0     1001      123       39 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/ndjson_core/mod.rs
--rw-r--r--   0     1001      123    12172 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/ndjson_core/ndjson.rs
--rw-r--r--   0     1001      123      273 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/options.rs
--rw-r--r--   0     1001      123     7360 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/parquet/async_impl.rs
--rw-r--r--   0     1001      123     3093 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/parquet/mmap.rs
--rw-r--r--   0     1001      123     3132 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/parquet/mod.rs
--rw-r--r--   0     1001      123     4784 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/parquet/predicates.rs
--rw-r--r--   0     1001      123     9606 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/parquet/read.rs
--rw-r--r--   0     1001      123    16886 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/parquet/read_impl.rs
--rw-r--r--   0     1001      123    10106 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/parquet/write.rs
--rw-r--r--   0     1001      123     5334 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/partition.rs
--rw-r--r--   0     1001      123     1455 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/predicates.rs
--rw-r--r--   0     1001      123      628 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/prelude.rs
--rw-r--r--   0     1001      123      417 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/tests.rs
--rw-r--r--   0     1001      123     4467 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-io/src/utils.rs
--rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.6/local_dependencies/polars-algo/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-algo/LICENSE
--rw-r--r--   0     1001      123     7265 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-algo/src/algo.rs
--rw-r--r--   0     1001      123       88 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-algo/src/lib.rs
--rw-r--r--   0     1001      123       28 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-algo/src/prelude.rs
--rw-r--r--   0        0        0     5407 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/LICENSE
--rw-r--r--   0     1001      123    19606 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/arithmetic.rs
--rw-r--r--   0     1001      123     8679 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/bitwise.rs
--rw-r--r--   0     1001      123     2298 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/builder/binary.rs
--rw-r--r--   0     1001      123     1207 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs
--rw-r--r--   0     1001      123     1556 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/builder/from.rs
--rw-r--r--   0     1001      123    20366 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/builder/list.rs
--rw-r--r--   0     1001      123     8845 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/builder/mod.rs
--rw-r--r--   0     1001      123     1410 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs
--rw-r--r--   0     1001      123     2291 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs
--rw-r--r--   0     1001      123    11560 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/cast.rs
--rw-r--r--   0     1001      123    48300 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs
--rw-r--r--   0     1001      123     9463 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs
--rw-r--r--   0     1001      123      551 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/drop.rs
--rw-r--r--   0     1001      123      963 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/float.rs
--rw-r--r--   0     1001      123     5069 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/from.rs
--rw-r--r--   0     1001      123    38411 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs
--rw-r--r--   0     1001      123     1395 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs
--rw-r--r--   0     1001      123       28 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/iterator/par/mod.rs
--rw-r--r--   0     1001      123     1129 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs
--rw-r--r--   0     1001      123       21 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/kernels/mod.rs
--rw-r--r--   0     1001      123     2986 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/kernels/take.rs
--rw-r--r--   0     1001      123     7728 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/list/iterator.rs
--rw-r--r--   0     1001      123     2802 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/list/mod.rs
--rw-r--r--   0     1001      123    19796 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs
--rw-r--r--   0     1001      123     3688 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs
--rw-r--r--   0     1001      123     4270 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs
--rw-r--r--   0     1001      123    10220 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs
--rw-r--r--   0     1001      123     1400 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs
--rw-r--r--   0     1001      123      358 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/full.rs
--rw-r--r--   0     1001      123      192 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/mod.rs
--rw-r--r--   0     1001      123     2731 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs
--rw-r--r--   0     1001      123     2172 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs
--rw-r--r--   0     1001      123      925 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs
--rw-r--r--   0     1001      123     6453 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs
--rw-r--r--   0     1001      123     1604 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/date.rs
--rw-r--r--   0     1001      123     4105 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs
--rw-r--r--   0     1001      123     4443 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs
--rw-r--r--   0     1001      123     2434 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/duration.rs
--rw-r--r--   0     1001      123     2549 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/mod.rs
--rw-r--r--   0     1001      123      476 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/struct_/from.rs
--rw-r--r--   0     1001      123    15081 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs
--rw-r--r--   0     1001      123     1182 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/time.rs
--rw-r--r--   0     1001      123    23524 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/mod.rs
--rw-r--r--   0     1001      123     7200 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ndarray.rs
--rw-r--r--   0     1001      123     4484 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/object/builder.rs
--rw-r--r--   0     1001      123     1547 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs
--rw-r--r--   0     1001      123     3124 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs
--rw-r--r--   0     1001      123     7054 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs
--rw-r--r--   0     1001      123     3410 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs
--rw-r--r--   0     1001      123      137 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/object/is_valid.rs
--rw-r--r--   0     1001      123     4419 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/object/iterator.rs
--rw-r--r--   0     1001      123     4826 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/object/mod.rs
--rw-r--r--   0     1001      123     2853 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/object/registry.rs
--rw-r--r--   0     1001      123      272 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/abs.rs
--rw-r--r--   0     1001      123    32120 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs
--rw-r--r--   0     1001      123     9946 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs
--rw-r--r--   0     1001      123     2875 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs
--rw-r--r--   0     1001      123     9670 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs
--rw-r--r--   0     1001      123     2365 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/append.rs
--rw-r--r--   0     1001      123    27269 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/apply.rs
--rw-r--r--   0     1001      123    12799 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs
--rw-r--r--   0     1001      123     6214 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs
--rw-r--r--   0     1001      123    11537 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs
--rw-r--r--   0     1001      123     1737 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs
--rw-r--r--   0     1001      123     4801 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs
--rw-r--r--   0     1001      123     6264 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs
--rw-r--r--   0     1001      123    25614 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/explode.rs
--rw-r--r--   0     1001      123     8339 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/extend.rs
--rw-r--r--   0     1001      123    13777 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs
--rw-r--r--   0     1001      123     5308 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/filter.rs
--rw-r--r--   0     1001      123     4436 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/full.rs
--rw-r--r--   0     1001      123        1 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/interpolate.rs
--rw-r--r--   0     1001      123    15385 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs
--rw-r--r--   0     1001      123        1 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/len.rs
--rw-r--r--   0     1001      123    22376 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/mod.rs
--rw-r--r--   0     1001      123     2403 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs
--rw-r--r--   0     1001      123      593 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs
--rw-r--r--   0     1001      123     2585 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs
--rw-r--r--   0     1001      123     1539 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs
--rw-r--r--   0     1001      123    10234 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs
--rw-r--r--   0     1001      123    12518 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/set.rs
--rw-r--r--   0     1001      123     6151 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/shift.rs
--rw-r--r--   0     1001      123     2299 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs
--rw-r--r--   0     1001      123     5467 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs
--rw-r--r--   0     1001      123     7430 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs
--rw-r--r--   0     1001      123    30762 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs
--rw-r--r--   0     1001      123      380 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/sort/slice.rs
--rw-r--r--   0     1001      123    20472 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs
--rw-r--r--   0     1001      123     6630 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs
--rw-r--r--   0     1001      123     1859 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs
--rw-r--r--   0     1001      123    16256 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs
--rw-r--r--   0     1001      123     5041 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs
--rw-r--r--   0     1001      123     6064 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs
--rw-r--r--   0     1001      123    11229 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs
--rw-r--r--   0     1001      123    14620 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs
--rw-r--r--   0     1001      123     7753 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/zip.rs
--rw-r--r--   0     1001      123     9093 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/random.rs
--rw-r--r--   0     1001      123     1959 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs
--rw-r--r--   0     1001      123     2501 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/temporal/date.rs
--rw-r--r--   0     1001      123    11998 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs
--rw-r--r--   0     1001      123     3201 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs
--rw-r--r--   0     1001      123      533 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs
--rw-r--r--   0     1001      123     2724 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/temporal/time.rs
--rw-r--r--   0     1001      123      872 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/to_vec.rs
--rw-r--r--   0     1001      123     8113 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/trusted_len.rs
--rw-r--r--   0     1001      123    25934 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs
--rw-r--r--   0     1001      123     7689 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/cloud.rs
--rw-r--r--   0     1001      123     1549 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/config.rs
--rw-r--r--   0     1001      123     3946 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/datatypes/_serde.rs
--rw-r--r--   0     1001      123     2650 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/datatypes/aliases.rs
--rw-r--r--   0     1001      123    42410 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/datatypes/any_value.rs
--rw-r--r--   0     1001      123    12083 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/datatypes/dtype.rs
--rw-r--r--   0     1001      123     5422 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/datatypes/field.rs
--rw-r--r--   0     1001      123     7675 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/datatypes/mod.rs
--rw-r--r--   0     1001      123     2016 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/datatypes/time_unit.rs
--rw-r--r--   0     1001      123      118 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/doc/changelog/mod.rs
--rw-r--r--   0     1001      123      898 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs
--rw-r--r--   0     1001      123      481 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/doc/changelog/v0_3.rs
--rw-r--r--   0     1001      123      293 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/doc/changelog/v0_4.rs
--rw-r--r--   0     1001      123      499 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/doc/changelog/v0_5.rs
--rw-r--r--   0     1001      123      288 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/doc/changelog/v0_6.rs
--rw-r--r--   0     1001      123     1071 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/doc/changelog/v0_7.rs
--rw-r--r--   0     1001      123      819 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/doc/changelog/v0_8.rs
--rw-r--r--   0     1001      123      596 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/doc/changelog/v0_9.rs
--rw-r--r--   0     1001      123       43 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/doc/mod.rs
--rw-r--r--   0     1001      123       25 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/error.rs
--rw-r--r--   0     1001      123      433 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/export.rs
--rw-r--r--   0     1001      123    36116 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/fmt.rs
--rw-r--r--   0     1001      123     5177 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/arithmetic.rs
--rw-r--r--   0     1001      123     7874 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/asof_join/asof.rs
--rw-r--r--   0     1001      123    33715 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/asof_join/groups.rs
--rw-r--r--   0     1001      123     6634 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/asof_join/mod.rs
--rw-r--r--   0     1001      123      559 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/chunks.rs
--rw-r--r--   0     1001      123     5179 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/cross_join.rs
--rw-r--r--   0     1001      123    16609 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/explode.rs
--rw-r--r--   0     1001      123     1019 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/from.rs
--rw-r--r--   0     1001      123    16518 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs
--rw-r--r--   0     1001      123     4115 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs
--rw-r--r--   0     1001      123     7643 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs
--rw-r--r--   0     1001      123    39255 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs
--rw-r--r--   0     1001      123     5636 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs
--rw-r--r--   0     1001      123      218 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/groupby/expr.rs
--rw-r--r--   0     1001      123    15470 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/groupby/hashing.rs
--rw-r--r--   0     1001      123    14048 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/groupby/into_groups.rs
--rw-r--r--   0     1001      123    39374 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/groupby/mod.rs
--rw-r--r--   0     1001      123    10535 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/groupby/perfect.rs
--rw-r--r--   0     1001      123    17214 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/groupby/proxy.rs
--rw-r--r--   0     1001      123    18264 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/hash_join/mod.rs
--rw-r--r--   0     1001      123    22392 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs
--rw-r--r--   0     1001      123     2413 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs
--rw-r--r--   0     1001      123    16352 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs
--rw-r--r--   0     1001      123     4295 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs
--rw-r--r--   0     1001      123     6076 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs
--rw-r--r--   0     1001      123     4247 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs
--rw-r--r--   0     1001      123     3913 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs
--rw-r--r--   0     1001      123    11879 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs
--rw-r--r--   0     1001      123   124236 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/mod.rs
--rw-r--r--   0     1001      123    27513 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/row/av_buffer.rs
--rw-r--r--   0     1001      123     3732 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/row/dataframe.rs
--rw-r--r--   0     1001      123     5976 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/row/mod.rs
--rw-r--r--   0     1001      123     8795 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/row/transpose.rs
--rw-r--r--   0     1001      123     2183 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/top_k.rs
--rw-r--r--   0     1001      123     1388 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/upstream_traits.rs
--rw-r--r--   0     1001      123    10935 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/functions.rs
--rw-r--r--   0     1001      123     2149 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/hashing/fx.rs
--rw-r--r--   0     1001      123     1503 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/hashing/identity.rs
--rw-r--r--   0     1001      123      457 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/hashing/mod.rs
--rw-r--r--   0     1001      123     2684 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/hashing/partition.rs
--rw-r--r--   0     1001      123    17653 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/hashing/vector_hasher.rs
--rw-r--r--   0     1001      123     1896 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/lib.rs
--rw-r--r--   0     1001      123    15733 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/named_from.rs
--rw-r--r--   0     1001      123     2411 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/prelude.rs
--rw-r--r--   0     1001      123    16406 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/schema.rs
--rw-r--r--   0     1001      123     4218 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/serde/chunked_array.rs
--rw-r--r--   0     1001      123     6551 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/serde/mod.rs
--rw-r--r--   0     1001      123     9929 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/serde/series.rs
--rw-r--r--   0     1001      123    18441 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/any_value.rs
--rw-r--r--   0     1001      123    28511 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs
--rw-r--r--   0     1001      123      222 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/arithmetic/mod.rs
--rw-r--r--   0     1001      123     3546 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/arithmetic/owned.rs
--rw-r--r--   0     1001      123    13187 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/comparison.rs
--rw-r--r--   0     1001      123    25008 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/from.rs
--rw-r--r--   0     1001      123     9217 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/implementations/binary.rs
--rw-r--r--   0     1001      123    10850 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/implementations/boolean.rs
--rw-r--r--   0     1001      123    12962 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/implementations/categorical.rs
--rw-r--r--   0     1001      123    18304 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/implementations/dates_time.rs
--rw-r--r--   0     1001      123    15242 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/implementations/datetime.rs
--rw-r--r--   0     1001      123     5829 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/implementations/decimal.rs
--rw-r--r--   0     1001      123    15106 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/implementations/duration.rs
--rw-r--r--   0     1001      123    14223 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/implementations/floats.rs
--rw-r--r--   0     1001      123     6207 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/implementations/list.rs
--rw-r--r--   0     1001      123    18305 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/implementations/mod.rs
--rw-r--r--   0     1001      123     5336 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/implementations/null.rs
--rw-r--r--   0     1001      123     8004 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/implementations/object.rs
--rw-r--r--   0     1001      123    11029 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/implementations/struct_.rs
--rw-r--r--   0     1001      123     9735 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/implementations/utf8.rs
--rw-r--r--   0     1001      123     4471 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/into.rs
--rw-r--r--   0     1001      123     6297 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/iterator.rs
--rw-r--r--   0     1001      123    37684 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/mod.rs
--rw-r--r--   0     1001      123      853 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/ops/diff.rs
--rw-r--r--   0     1001      123     5204 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/ops/downcast.rs
--rw-r--r--   0     1001      123     3601 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/ops/ewm.rs
--rw-r--r--   0     1001      123      413 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/ops/extend.rs
--rw-r--r--   0     1001      123      562 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/ops/mod.rs
--rw-r--r--   0     1001      123     5974 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/ops/moment.rs
--rw-r--r--   0     1001      123     2908 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/ops/null.rs
--rw-r--r--   0     1001      123     1347 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/ops/pct_change.rs
--rw-r--r--   0     1001      123     4247 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/ops/round.rs
--rw-r--r--   0     1001      123     5072 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/ops/to_list.rs
--rw-r--r--   0     1001      123     1476 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/ops/unique.rs
--rw-r--r--   0     1001      123    18204 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/series_trait.rs
--rw-r--r--   0     1001      123     2840 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/unstable.rs
--rw-r--r--   0     1001      123     8117 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/testing.rs
--rw-r--r--   0     1001      123      508 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/tests.rs
--rw-r--r--   0     1001      123     1396 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/utils/flatten.rs
--rw-r--r--   0     1001      123    31704 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/utils/mod.rs
--rw-r--r--   0     1001      123     1598 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/utils/series.rs
--rw-r--r--   0     1001      123    13773 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-core/src/utils/supertype.rs
--rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.6/local_dependencies/polars-row/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-row/LICENSE
--rw-r--r--   0     1001      123     8985 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-row/src/encode.rs
--rw-r--r--   0     1001      123     4591 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-row/src/encodings/fixed.rs
--rw-r--r--   0     1001      123       47 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-row/src/encodings/mod.rs
--rw-r--r--   0     1001      123     4508 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-row/src/encodings/variable.rs
--rw-r--r--   0     1001      123    13678 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-row/src/lib.rs
--rw-r--r--   0     1001      123     2079 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-row/src/row.rs
--rw-r--r--   0     1001      123      682 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-row/src/utils.rs
--rw-r--r--   0        0        0     5977 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/LICENSE
--rw-r--r--   0     1001      123     1796 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/dot.rs
--rw-r--r--   0     1001      123     4359 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/dsl/eval.rs
--rw-r--r--   0     1001      123     4505 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/dsl/functions.rs
--rw-r--r--   0     1001      123      164 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/dsl/into.rs
--rw-r--r--   0     1001      123     6754 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/dsl/list.rs
--rw-r--r--   0     1001      123     2899 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/dsl/mod.rs
--rw-r--r--   0     1001      123     1182 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs
--rw-r--r--   0     1001      123     9278 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/frame/csv.rs
--rw-r--r--   0     1001      123     4309 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/frame/file_list_reader.rs
--rw-r--r--   0     1001      123     2261 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/frame/ipc.rs
--rw-r--r--   0     1001      123    47176 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/frame/mod.rs
--rw-r--r--   0     1001      123     3414 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/frame/ndjson.rs
--rw-r--r--   0     1001      123     3440 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/frame/parquet.rs
--rw-r--r--   0     1001      123     2892 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/frame/pivot.rs
--rw-r--r--   0     1001      123      416 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/frame/python.rs
--rw-r--r--   0     1001      123     6376 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/lib.rs
--rw-r--r--   0     1001      123     1049 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs
--rw-r--r--   0     1001      123      776 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs
--rw-r--r--   0     1001      123      670 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs
--rw-r--r--   0     1001      123     1284 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs
--rw-r--r--   0     1001      123     3908 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs
--rw-r--r--   0     1001      123     3577 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs
--rw-r--r--   0     1001      123    13439 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs
--rw-r--r--   0     1001      123     4335 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs
--rw-r--r--   0     1001      123     6058 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs
--rw-r--r--   0     1001      123     7074 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs
--rw-r--r--   0     1001      123     2045 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs
--rw-r--r--   0     1001      123     1677 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs
--rw-r--r--   0     1001      123     2986 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs
--rw-r--r--   0     1001      123     1963 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs
--rw-r--r--   0     1001      123     4151 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs
--rw-r--r--   0     1001      123     1208 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs
--rw-r--r--   0     1001      123     2421 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs
--rw-r--r--   0     1001      123      548 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs
--rw-r--r--   0     1001      123     2197 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs
--rw-r--r--   0     1001      123     1922 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs
--rw-r--r--   0     1001      123      663 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs
--rw-r--r--   0     1001      123     3702 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs
--rw-r--r--   0     1001      123      838 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs
--rw-r--r--   0     1001      123     1284 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/exotic.rs
--rw-r--r--   0     1001      123    21873 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs
--rw-r--r--   0     1001      123     2689 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs
--rw-r--r--   0     1001      123    17432 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs
--rw-r--r--   0     1001      123    17488 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs
--rw-r--r--   0     1001      123     3153 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs
--rw-r--r--   0     1001      123     6326 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs
--rw-r--r--   0     1001      123     2003 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs
--rw-r--r--   0     1001      123     5809 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs
--rw-r--r--   0     1001      123     4131 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs
--rw-r--r--   0     1001      123     5304 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs
--rw-r--r--   0     1001      123    21103 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs
--rw-r--r--   0     1001      123    10091 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs
--rw-r--r--   0     1001      123     3929 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs
--rw-r--r--   0     1001      123    11541 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs
--rw-r--r--   0     1001      123     8331 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs
--rw-r--r--   0     1001      123    14360 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs
--rw-r--r--   0     1001      123    31819 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs
--rw-r--r--   0     1001      123     2039 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs
--rw-r--r--   0     1001      123      414 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/mod.rs
--rw-r--r--   0     1001      123     2005 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs
--rw-r--r--   0     1001      123    27366 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs
--rw-r--r--   0     1001      123    18862 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs
--rw-r--r--   0     1001      123       87 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/planner/mod.rs
--rw-r--r--   0     1001      123     9425 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/state.rs
--rw-r--r--   0     1001      123    20891 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/streaming/convert.rs
--rw-r--r--   0     1001      123      219 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/streaming/mod.rs
--rw-r--r--   0     1001      123     3333 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs
--rw-r--r--   0     1001      123      722 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/prelude.rs
--rw-r--r--   0     1001      123    14990 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/tests/aggregations.rs
--rw-r--r--   0     1001      123     2339 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/tests/arity.rs
--rw-r--r--   0     1001      123     7031 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/tests/cse.rs
--rw-r--r--   0     1001      123    12749 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/tests/io.rs
--rw-r--r--   0     1001      123     4207 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/tests/logical.rs
--rw-r--r--   0     1001      123     4288 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/tests/mod.rs
--rw-r--r--   0     1001      123    14812 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/tests/optimization_checks.rs
--rw-r--r--   0     1001      123     6799 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/tests/predicate_queries.rs
--rw-r--r--   0     1001      123     3158 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/tests/projection_queries.rs
--rw-r--r--   0     1001      123    47910 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/tests/queries.rs
--rw-r--r--   0     1001      123     8358 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/tests/streaming.rs
--rw-r--r--   0     1001      123     2886 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/tests/tpch.rs
--rw-r--r--   0     1001      123     1028 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/utils.rs
--rw-r--r--   0        0        0     3268 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/LICENSE
--rw-r--r--   0     1001      123      234 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/binary/mod.rs
--rw-r--r--   0     1001      123     3549 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs
--rw-r--r--   0     1001      123    11023 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/interpolate.rs
--rw-r--r--   0     1001      123     1679 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/list/count.rs
--rw-r--r--   0     1001      123     2452 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/list/hash.rs
--rw-r--r--   0     1001      123     7861 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs
--rw-r--r--   0     1001      123      511 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/list/mod.rs
--rw-r--r--   0     1001      123    22005 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs
--rw-r--r--   0     1001      123     5269 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs
--rw-r--r--   0     1001      123     2435 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs
--rw-r--r--   0     1001      123      489 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/mod.rs
--rw-r--r--   0     1001      123     9380 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs
--rw-r--r--   0     1001      123     6795 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/set.rs
--rw-r--r--   0     1001      123     7490 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/strings/case.rs
--rw-r--r--   0     1001      123     8251 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs
--rw-r--r--   0     1001      123     2345 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs
--rw-r--r--   0     1001      123      514 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs
--rw-r--r--   0     1001      123    14731 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs
--rw-r--r--   0     1001      123     4053 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs
--rw-r--r--   0     1001      123     2486 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/top_k.rs
--rw-r--r--   0     1001      123     7727 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs
--rw-r--r--   0     1001      123    18025 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/frame/join/mod.rs
--rw-r--r--   0     1001      123     4174 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/frame/mod.rs
--rw-r--r--   0     1001      123    10257 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/frame/pivot/mod.rs
--rw-r--r--   0     1001      123    13486 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/frame/pivot/positioning.rs
--rw-r--r--   0     1001      123      217 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/lib.rs
--rw-r--r--   0     1001      123      290 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/prelude.rs
--rw-r--r--   0     1001      123       25 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/series/mod.rs
--rw-r--r--   0     1001      123     9623 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs
--rw-r--r--   0     1001      123      118 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/series/ops/approx_algo/mod.rs
--rw-r--r--   0     1001      123     2016 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/series/ops/approx_unique.rs
--rw-r--r--   0     1001      123    11872 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs
--rw-r--r--   0     1001      123     3680 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/series/ops/floor_divide.rs
--rw-r--r--   0     1001      123     3423 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/series/ops/is_first.rs
--rw-r--r--   0     1001      123     2975 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/series/ops/is_unique.rs
--rw-r--r--   0     1001      123     3626 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/series/ops/log.rs
--rw-r--r--   0     1001      123     1106 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/series/ops/mod.rs
--rw-r--r--   0     1001      123     1769 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/series/ops/rolling.rs
--rw-r--r--   0     1001      123     7642 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/series/ops/search_sorted.rs
--rw-r--r--   0     1001      123     2500 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/series/ops/to_dummies.rs
--rw-r--r--   0     1001      123     2067 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/series/ops/various.rs
--rw-r--r--   0        0        0    10541 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.6/local_dependencies/polars/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/LICENSE
--rw-r--r--   0     1001      123     3249 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/Makefile
--rw-r--r--   0     1001      123      215 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/build.rs
--rw-r--r--   0     1001      123       78 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/clippy.toml
--rw-r--r--   0     1001      123    17602 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/src/docs/eager.rs
--rw-r--r--   0     1001      123     8778 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/src/docs/lazy.rs
--rw-r--r--   0     1001      123       50 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/src/docs/mod.rs
--rw-r--r--   0     1001      123     3797 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/src/docs/performance.rs
--rw-r--r--   0     1001      123       59 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/src/export.rs
--rw-r--r--   0     1001      123    20207 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/src/lib.rs
--rw-r--r--   0     1001      123      387 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/src/prelude.rs
--rw-r--r--   0     1001      123       44 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/src/sql.rs
--rw-r--r--   0     1001      123     4272 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/core/date_like.rs
--rw-r--r--   0     1001      123     2401 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/core/groupby.rs
--rw-r--r--   0     1001      123    17826 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/core/joins.rs
--rw-r--r--   0     1001      123      545 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/core/list.rs
--rw-r--r--   0     1001      123      189 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/core/mod.rs
--rw-r--r--   0     1001      123     6258 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/core/pivot.rs
--rw-r--r--   0     1001      123     1102 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/core/random.rs
--rw-r--r--   0     1001      123    10844 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/core/rolling_window.rs
--rw-r--r--   0     1001      123     1093 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/core/series.rs
--rw-r--r--   0     1001      123      370 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/core/utils.rs
--rw-r--r--   0     1001      123    30013 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/io/csv.rs
--rw-r--r--   0     1001      123     4490 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/io/ipc_stream.rs
--rw-r--r--   0     1001      123     7044 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/io/json.rs
--rw-r--r--   0     1001      123      378 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/io/mod.rs
--rw-r--r--   0     1001      123      988 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/io/parquet.rs
--rw-r--r--   0     1001      123     1530 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/joins.rs
--rw-r--r--   0     1001      123     2452 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/aggregation.rs
--rw-r--r--   0     1001      123      702 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/cse.rs
--rw-r--r--   0     1001      123      500 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/explodes.rs
--rw-r--r--   0     1001      123     2279 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/expressions/apply.rs
--rw-r--r--   0     1001      123    10285 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/expressions/arity.rs
--rw-r--r--   0     1001      123     1064 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/expressions/expand.rs
--rw-r--r--   0     1001      123     1008 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/expressions/filter.rs
--rw-r--r--   0     1001      123      428 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/expressions/is_in.rs
--rw-r--r--   0     1001      123      121 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/expressions/mod.rs
--rw-r--r--   0     1001      123      659 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/expressions/slice.rs
--rw-r--r--   0     1001      123    10139 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/expressions/window.rs
--rw-r--r--   0     1001      123      579 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/folds.rs
--rw-r--r--   0     1001      123      557 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/functions.rs
--rw-r--r--   0     1001      123     4482 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/groupby.rs
--rw-r--r--   0     1001      123     1655 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs
--rw-r--r--   0     1001      123      691 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/mod.rs
--rw-r--r--   0     1001      123     5381 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/predicate_queries.rs
--rw-r--r--   0     1001      123     4476 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/projection_queries.rs
--rw-r--r--   0     1001      123     6444 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/queries.rs
--rw-r--r--   0     1001      123      141 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/main.rs
--rw-r--r--   0     1001      123    12591 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/schema.rs
--rw-r--r--   0        0        0     5241 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/LICENSE
--rw-r--r--   0     1001      123       45 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/constants.rs
--rw-r--r--   0     1001      123    17248 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dot.rs
--rw-r--r--   0     1001      123     4171 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/arithmetic.rs
--rw-r--r--   0     1001      123      935 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/binary.rs
--rw-r--r--   0     1001      123      650 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/cat.rs
--rw-r--r--   0     1001      123     9424 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/dt.rs
--rw-r--r--   0     1001      123    13169 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/expr.rs
--rw-r--r--   0     1001      123      753 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/from.rs
--rw-r--r--   0     1001      123       85 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/abs.rs
--rw-r--r--   0     1001      123     1431 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs
--rw-r--r--   0     1001      123     1327 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs
--rw-r--r--   0     1001      123     4221 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs
--rw-r--r--   0     1001      123     1910 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs
--rw-r--r--   0     1001      123     1216 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs
--rw-r--r--   0     1001      123      344 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/clip.rs
--rw-r--r--   0     1001      123     1593 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs
--rw-r--r--   0     1001      123    13227 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs
--rw-r--r--   0     1001      123      810 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs
--rw-r--r--   0     1001      123     2541 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs
--rw-r--r--   0     1001      123     8119 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/list.rs
--rw-r--r--   0     1001      123      581 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/log.rs
--rw-r--r--   0     1001      123    19145 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs
--rw-r--r--   0     1001      123      462 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/nan.rs
--rw-r--r--   0     1001      123     3132 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs
--rw-r--r--   0     1001      123      152 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/rolling.rs
--rw-r--r--   0     1001      123      260 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/round.rs
--rw-r--r--   0     1001      123      200 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/row_hash.rs
--rw-r--r--   0     1001      123    13416 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs
--rw-r--r--   0     1001      123      306 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/search_sorted.rs
--rw-r--r--   0     1001      123     3812 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs
--rw-r--r--   0     1001      123     1238 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs
--rw-r--r--   0     1001      123      972 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs
--rw-r--r--   0     1001      123    19641 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs
--rw-r--r--   0     1001      123     1017 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs
--rw-r--r--   0     1001      123     2700 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs
--rw-r--r--   0     1001      123     5122 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs
--rw-r--r--   0     1001      123      170 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/unique.rs
--rw-r--r--   0     1001      123    43864 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/functions.rs
--rw-r--r--   0     1001      123    10196 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/list.rs
--rw-r--r--   0     1001      123     2181 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/meta.rs
--rw-r--r--   0     1001      123    64804 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/mod.rs
--rw-r--r--   0     1001      123       40 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/names.rs
--rw-r--r--   0     1001      123     2100 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/options.rs
--rw-r--r--   0     1001      123    14993 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/string.rs
--rw-r--r--   0     1001      123     2715 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/struct_.rs
--rw-r--r--   0     1001      123       38 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/frame/mod.rs
--rw-r--r--   0     1001      123      933 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/frame/opt_state.rs
--rw-r--r--   0     1001      123      466 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/global.rs
--rw-r--r--   0     1001      123      175 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/lib.rs
--rw-r--r--   0     1001      123     6825 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs
--rw-r--r--   0     1001      123    11393 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs
--rw-r--r--   0     1001      123    25656 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/alp.rs
--rw-r--r--   0     1001      123     1622 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs
--rw-r--r--   0     1001      123     1428 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/apply.rs
--rw-r--r--   0     1001      123    24898 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/builder.rs
--rw-r--r--   0     1001      123    29652 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/conversion.rs
--rw-r--r--   0     1001      123      301 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/debug.rs
--rw-r--r--   0     1001      123    15191 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/format.rs
--rw-r--r--   0     1001      123      895 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs
--rw-r--r--   0     1001      123      137 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/functions/explode.rs
--rw-r--r--   0     1001      123     1169 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs
--rw-r--r--   0     1001      123    11905 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs
--rw-r--r--   0     1001      123     1330 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs
--rw-r--r--   0     1001      123     9752 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/iterator.rs
--rw-r--r--   0     1001      123    10463 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/lit.rs
--rw-r--r--   0     1001      123     8115 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/mod.rs
--rw-r--r--   0     1001      123     7416 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs
--rw-r--r--   0     1001      123    15277 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs
--rw-r--r--   0     1001      123     3250 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs
--rw-r--r--   0     1001      123     3236 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs
--rw-r--r--   0     1001      123     3994 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs
--rw-r--r--   0     1001      123    14479 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs
--rw-r--r--   0     1001      123     1556 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs
--rw-r--r--   0     1001      123     6644 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs
--rw-r--r--   0     1001      123     1222 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs
--rw-r--r--   0     1001      123    28276 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs
--rw-r--r--   0     1001      123     2571 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs
--rw-r--r--   0     1001      123    15130 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs
--rw-r--r--   0     1001      123     1755 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs
--rw-r--r--   0     1001      123     3930 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs
--rw-r--r--   0     1001      123     1799 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs
--rw-r--r--   0     1001      123     3269 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs
--rw-r--r--   0     1001      123     2638 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs
--rw-r--r--   0     1001      123    15747 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs
--rw-r--r--   0     1001      123    26502 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs
--rw-r--r--   0     1001      123     2692 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs
--rw-r--r--   0     1001      123     2639 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs
--rw-r--r--   0     1001      123     3501 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs
--rw-r--r--   0     1001      123    27361 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs
--rw-r--r--   0     1001      123     3492 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs
--rw-r--r--   0     1001      123    13845 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs
--rw-r--r--   0     1001      123     3161 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs
--rw-r--r--   0     1001      123     9725 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs
--rw-r--r--   0     1001      123    19820 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs
--rw-r--r--   0     1001      123    10187 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/options.rs
--rw-r--r--   0     1001      123    15276 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/projection.rs
--rw-r--r--   0     1001      123     4615 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs
--rw-r--r--   0     1001      123    13038 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/schema.rs
--rw-r--r--   0     1001      123      809 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/prelude.rs
--rw-r--r--   0     1001      123    11879 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/utils.rs
--rw-r--r--   0        0        0     4398 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.6/Cargo.toml
--rw-r--r--   0     1001      123       76 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/.gitignore
--rw-r--r--   0     1001      123     1055 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/LICENSE
--rw-r--r--   0     1001      123     2414 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/Makefile
--rw-r--r--   0     1001      123    12625 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/README.md
--rw-r--r--   0     1001      123      651 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/build.rs
--rw-r--r--   0     1001      123       32 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/.gitignore
--rw-r--r--   0     1001      123      679 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/Makefile
--rw-r--r--   0     1001      123      318 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/_templates/api_redirect.html
--rw-r--r--   0     1001      123      151 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/_templates/autosummary/accessor.rst
--rw-r--r--   0     1001      123      160 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/_templates/autosummary/accessor_attribute.rst
--rw-r--r--   0     1001      123      168 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/_templates/autosummary/accessor_callable.rst
--rw-r--r--   0     1001      123      157 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/_templates/autosummary/accessor_method.rst
--rw-r--r--   0     1001      123      836 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/_templates/autosummary/class.rst
--rw-r--r--   0     1001      123       94 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/_templates/autosummary/class_without_autosummary.rst
--rw-r--r--   0     1001      123      406 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/_templates/sidebar-nav-bs.html
--rw-r--r--   0     1001      123      450 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/requirements-docs.txt
--rw-r--r--   0     1001      123     1567 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/_static/css/custom.css
--rw-r--r--   0     1001      123     7302 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/conf.py
--rw-r--r--   0     1001      123       51 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/index.rst
--rw-r--r--   0     1001      123     6767 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/api.rst
--rw-r--r--   0     1001      123     1694 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/config.rst
--rw-r--r--   0     1001      123      274 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/dataframe/aggregation.rst
--rw-r--r--   0     1001      123      221 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/dataframe/attributes.rst
--rw-r--r--   0     1001      123      142 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/dataframe/computation.rst
--rw-r--r--   0     1001      123      319 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/dataframe/descriptive.rst
--rw-r--r--   0     1001      123      319 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/dataframe/export.rst
--rw-r--r--   0     1001      123      464 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/dataframe/groupby.rst
--rw-r--r--   0     1001      123      379 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/dataframe/index.rst
--rw-r--r--   0     1001      123      189 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/dataframe/miscellaneous.rst
--rw-r--r--   0     1001      123     1513 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/dataframe/modify_select.rst
--rw-r--r--   0     1001      123      663 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/datatypes.rst
--rw-r--r--   0     1001      123      421 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/exceptions.rst
--rw-r--r--   0     1001      123      391 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/expressions/aggregation.rst
--rw-r--r--   0     1001      123      309 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/expressions/binary.rst
--rw-r--r--   0     1001      123      338 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/expressions/boolean.rst
--rw-r--r--   0     1001      123      237 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/expressions/categories.rst
--rw-r--r--   0     1001      123      221 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/expressions/columns.rst
--rw-r--r--   0     1001      123     1061 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/expressions/computation.rst
--rw-r--r--   0     1001      123     1114 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/expressions/functions.rst
--rw-r--r--   0     1001      123      461 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/expressions/index.rst
--rw-r--r--   0     1001      123      695 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/expressions/list.rst
--rw-r--r--   0     1001      123      374 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/expressions/meta.rst
--rw-r--r--   0     1001      123      125 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/expressions/miscellaneous.rst
--rw-r--r--   0     1001      123      977 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/expressions/modify_select.rst
--rw-r--r--   0     1001      123      639 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/expressions/operators.rst
--rw-r--r--   0     1001      123      860 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/expressions/string.rst
--rw-r--r--   0     1001      123      254 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/expressions/struct.rst
--rw-r--r--   0     1001      123      968 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/expressions/temporal.rst
--rw-r--r--   0     1001      123       98 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/expressions/window.rst
--rw-r--r--   0     1001      123      692 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/functions.rst
--rw-r--r--   0     1001      123      392 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/index.rst
--rw-r--r--   0     1001      123     1269 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/io.rst
--rw-r--r--   0     1001      123      252 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/lazyframe/aggregation.rst
--rw-r--r--   0     1001      123      179 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/lazyframe/attributes.rst
--rw-r--r--   0     1001      123      146 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/lazyframe/descriptive.rst
--rw-r--r--   0     1001      123      497 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/lazyframe/groupby.rst
--rw-r--r--   0     1001      123      354 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/lazyframe/index.rst
--rw-r--r--   0     1001      123      455 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/lazyframe/miscellaneous.rst
--rw-r--r--   0     1001      123      988 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/lazyframe/modify_select.rst
--rw-r--r--   0     1001      123      358 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/series/aggregation.rst
--rw-r--r--   0     1001      123      256 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/series/attributes.rst
--rw-r--r--   0     1001      123      321 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/series/binary.rst
--rw-r--r--   0     1001      123      117 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/series/boolean.rst
--rw-r--r--   0     1001      123      241 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/series/categories.rst
--rw-r--r--   0     1001      123     1103 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/series/computation.rst
--rw-r--r--   0     1001      123      744 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/series/descriptive.rst
--rw-r--r--   0     1001      123      240 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/series/export.rst
--rw-r--r--   0     1001      123      428 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/series/index.rst
--rw-r--r--   0     1001      123      749 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/series/list.rst
--rw-r--r--   0     1001      123      236 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/series/miscellaneous.rst
--rw-r--r--   0     1001      123     1077 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/series/modify_select.rst
--rw-r--r--   0     1001      123      922 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/series/string.rst
--rw-r--r--   0     1001      123      396 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/series/struct.rst
--rw-r--r--   0     1001      123     1118 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/series/temporal.rst
--rw-r--r--   0     1001      123      302 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/sql.rst
--rw-r--r--   0     1001      123      647 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/testing.rst
--rw-r--r--   0     1001      123      168 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/docs/source/reference/utils.rst
--rw-r--r--   0     1001      123     6283 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/__init__.py
--rw-r--r--   0     1001      123    13396 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/api.py
--rw-r--r--   0     1001      123    25956 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/config.py
--rw-r--r--   0     1001      123    25409 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/convert.py
--rw-r--r--   0     1001      123       77 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/dataframe/__init__.py
--rw-r--r--   0     1001      123     5057 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/dataframe/_html.py
--rw-r--r--   0     1001      123   304087 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/dataframe/frame.py
--rw-r--r--   0     1001      123    33240 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/dataframe/groupby.py
--rw-r--r--   0     1001      123     2628 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/datatypes/__init__.py
--rw-r--r--   0     1001      123    11480 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/datatypes/classes.py
--rw-r--r--   0     1001      123     1577 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/datatypes/constants.py
--rw-r--r--   0     1001      123     4430 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/datatypes/constructor.py
--rw-r--r--   0     1001      123    14921 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/datatypes/convert.py
--rw-r--r--   0     1001      123     7338 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/dependencies.py
--rw-r--r--   0     1001      123     2954 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/exceptions.py
--rw-r--r--   0     1001      123       61 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/expr/__init__.py
--rw-r--r--   0     1001      123     2730 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/expr/binary.py
--rw-r--r--   0     1001      123     1708 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/expr/categorical.py
--rw-r--r--   0     1001      123    69359 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/expr/datetime.py
--rw-r--r--   0     1001      123   250779 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/expr/expr.py
--rw-r--r--   0     1001      123    22899 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/expr/list.py
--rw-r--r--   0     1001      123     2059 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/expr/meta.py
--rw-r--r--   0     1001      123    44664 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/expr/string.py
--rw-r--r--   0     1001      123     5436 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/expr/struct.py
--rw-r--r--   0     1001      123     1981 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/functions/__init__.py
--rw-r--r--   0     1001      123    29688 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/functions/eager.py
--rw-r--r--   0     1001      123    90827 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/functions/lazy.py
--rw-r--r--   0     1001      123     6293 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/functions/whenthen.py
--rw-r--r--   0     1001      123      280 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/internals.py
--rw-r--r--   0     1001      123      978 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/io/__init__.py
--rw-r--r--   0     1001      123     6264 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/io/_utils.py
--rw-r--r--   0     1001      123      878 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/io/avro.py
--rw-r--r--   0     1001      123      144 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/io/csv/__init__.py
--rw-r--r--   0     1001      123     1082 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/io/csv/_utils.py
--rw-r--r--   0     1001      123     4691 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/io/csv/batched_reader.py
--rw-r--r--   0     1001      123    35533 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/io/csv/functions.py
--rw-r--r--   0     1001      123     8655 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/io/database.py
--rw-r--r--   0     1001      123    10988 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/io/delta.py
--rw-r--r--   0     1001      123       75 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/io/excel/__init__.py
--rw-r--r--   0     1001      123    18459 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/io/excel/_write_utils.py
--rw-r--r--   0     1001      123     6476 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/io/excel/functions.py
--rw-r--r--   0     1001      123      142 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/io/ipc/__init__.py
--rw-r--r--   0     1001      123     1271 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/io/ipc/anonymous_scan.py
--rw-r--r--   0     1001      123     5840 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/io/ipc/functions.py
--rw-r--r--   0     1001      123      519 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/io/json.py
--rw-r--r--   0     1001      123     2257 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/io/ndjson.py
--rw-r--r--   0     1001      123      170 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/io/parquet/__init__.py
--rw-r--r--   0     1001      123     1299 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/io/parquet/anonymous_scan.py
--rw-r--r--   0     1001      123     7212 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/io/parquet/functions.py
--rw-r--r--   0     1001      123      136 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/io/pyarrow_dataset/__init__.py
--rw-r--r--   0     1001      123     2331 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/io/pyarrow_dataset/anonymous_scan.py
--rw-r--r--   0     1001      123     3611 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/io/pyarrow_dataset/functions.py
--rw-r--r--   0     1001      123       77 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/lazyframe/__init__.py
--rw-r--r--   0     1001      123   166798 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/lazyframe/frame.py
--rw-r--r--   0     1001      123    24178 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/lazyframe/groupby.py
--rw-r--r--   0     1001      123        0 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/py.typed
--rw-r--r--   0     1001      123       69 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/series/__init__.py
--rw-r--r--   0     1001      123     1579 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/series/_numpy.py
--rw-r--r--   0     1001      123     1920 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/series/binary.py
--rw-r--r--   0     1001      123     1699 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/series/categorical.py
--rw-r--r--   0     1001      123    47287 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/series/datetime.py
--rw-r--r--   0     1001      123    12385 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/series/list.py
--rw-r--r--   0     1001      123   163748 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/series/series.py
--rw-r--r--   0     1001      123    27401 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/series/string.py
--rw-r--r--   0     1001      123     2287 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/series/struct.py
--rw-r--r--   0     1001      123     5375 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/series/utils.py
--rw-r--r--   0     1001      123     7638 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/slice.py
--rw-r--r--   0     1001      123       75 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/sql/__init__.py
--rw-r--r--   0     1001      123     1351 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/sql/context.py
--rw-r--r--   0     1001      123     4764 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/string_cache.py
--rw-r--r--   0     1001      123      362 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/testing/__init__.py
--rw-r--r--   0     1001      123      929 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/testing/_private.py
--rw-r--r--   0     1001      123     3689 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/testing/_tempdir.py
--rw-r--r--   0     1001      123    13597 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/testing/asserts.py
--rw-r--r--   0     1001      123      684 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/testing/parametric/__init__.py
--rw-r--r--   0     1001      123    24543 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/testing/parametric/primitives.py
--rw-r--r--   0     1001      123     6907 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/testing/parametric/strategies.py
--rw-r--r--   0     1001      123     5681 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/type_aliases.py
--rw-r--r--   0     1001      123     1167 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/utils/__init__.py
--rw-r--r--   0     1001      123    50687 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/utils/_construction.py
--rw-r--r--   0     1001      123     2782 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/utils/_parse_expr_input.py
--rw-r--r--   0     1001      123      721 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/utils/_scan.py
--rw-r--r--   0     1001      123      687 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/utils/_wrap.py
--rw-r--r--   0     1001      123      683 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/utils/build_info.py
--rw-r--r--   0     1001      123     9184 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/utils/convert.py
--rw-r--r--   0     1001      123     5789 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/utils/decorators.py
--rw-r--r--   0     1001      123     1660 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/utils/meta.py
--rw-r--r--   0     1001      123      514 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/utils/polars_version.py
--rw-r--r--   0     1001      123     2339 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/utils/show_versions.py
--rw-r--r--   0     1001      123    11592 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/polars/utils/various.py
--rw-r--r--   0     1001      123     5378 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/pyproject.toml
--rw-r--r--   0     1001      123      699 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/requirements-dev.txt
--rw-r--r--   0     1001      123       70 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/requirements-lint.txt
--rw-r--r--   0     1001      123     1640 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/scripts/check_stacklevels.py
--rw-r--r--   0     1001      123    11023 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/src/apply/dataframe.rs
--rw-r--r--   0     1001      123     8388 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/src/apply/mod.rs
--rw-r--r--   0     1001      123    71480 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/src/apply/series.rs
--rw-r--r--   0     1001      123       32 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/src/arrow_interop/mod.rs
--rw-r--r--   0     1001      123     1306 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/src/arrow_interop/to_py.rs
--rw-r--r--   0     1001      123     3902 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/src/arrow_interop/to_rust.rs
--rw-r--r--   0     1001      123     5250 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/src/batched_csv.rs
--rw-r--r--   0     1001      123    47200 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/src/conversion.rs
--rw-r--r--   0     1001      123    45472 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/src/dataframe.rs
--rw-r--r--   0     1001      123     3799 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/src/datatypes.rs
--rw-r--r--   0     1001      123     3288 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/src/error.rs
--rw-r--r--   0     1001      123     9482 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/src/file.rs
--rw-r--r--   0     1001      123     7468 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/src/lazy/apply.rs
--rw-r--r--   0     1001      123    33439 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/src/lazy/dataframe.rs
--rw-r--r--   0     1001      123    62664 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/src/lazy/dsl.rs
--rw-r--r--   0     1001      123     1082 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/src/lazy/meta.rs
--rw-r--r--   0     1001      123      727 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/src/lazy/mod.rs
--rw-r--r--   0     1001      123      212 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/src/lazy/utils.rs
--rw-r--r--   0     1001      123    20992 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/src/lib.rs
--rw-r--r--   0     1001      123     8642 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/src/npy.rs
--rw-r--r--   0     1001      123     1029 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/src/object.rs
--rw-r--r--   0     1001      123      122 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/src/prelude.rs
--rw-r--r--   0     1001      123      435 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/src/py_modules.rs
--rw-r--r--   0     1001      123    54535 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/src/series.rs
--rw-r--r--   0     1001      123     3478 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/src/set.rs
--rw-r--r--   0     1001      123      843 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/src/sql.rs
--rw-r--r--   0     1001      123     2335 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/src/utils.rs
--rw-r--r--   0     1001      123     6165 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/README.md
--rw-r--r--   0     1001      123     2189 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/benchmark/groupby-datagen.R
--rw-r--r--   0     1001      123     7945 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/benchmark/run_h2oai_benchmark.py
--rw-r--r--   0     1001      123     5721 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/benchmark/test_release.py
--rw-r--r--   0     1001      123     4589 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/docs/run_doctest.py
--rw-r--r--   0     1001      123     1633 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/parametric/conftest.py
--rw-r--r--   0     1001      123     3823 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/parametric/test_dataframe.py
--rw-r--r--   0     1001      123     1692 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/parametric/test_lazyframe.py
--rw-r--r--   0     1001      123     6355 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/parametric/test_series.py
--rw-r--r--   0     1001      123     8299 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/parametric/test_testing.py
--rw-r--r--   0     1001      123        0 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/__init__.py
--rw-r--r--   0     1001      123     3382 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/conftest.py
--rw-r--r--   0     1001      123       86 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/datatypes/__init__.py
--rw-r--r--   0     1001      123      351 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/datatypes/test_binary.py
--rw-r--r--   0     1001      123     1420 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/datatypes/test_bool.py
--rw-r--r--   0     1001      123    12662 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/datatypes/test_categorical.py
--rw-r--r--   0     1001      123     2766 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/datatypes/test_decimal.py
--rw-r--r--   0     1001      123      280 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/datatypes/test_duration.py
--rw-r--r--   0     1001      123    15805 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/datatypes/test_list.py
--rw-r--r--   0     1001      123      284 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/datatypes/test_null.py
--rw-r--r--   0     1001      123     2801 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/datatypes/test_object.py
--rw-r--r--   0     1001      123    29644 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/datatypes/test_struct.py
--rw-r--r--   0     1001      123    92406 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/datatypes/test_temporal.py
--rw-r--r--   0     1001      123      418 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/datatypes/test_time.py
--rw-r--r--   0     1001      123      218 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/conftest.py
--rw-r--r--   0     1001      123       16 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/files/delta-table/.part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       16 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/files/delta-table/.part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       16 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/files/delta-table/_delta_log/.00000000000000000000.json.crc
--rw-r--r--   0     1001      123       16 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/files/delta-table/_delta_log/.00000000000000000001.json.crc
--rw-r--r--   0     1001      123      905 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json
--rw-r--r--   0     1001      123      936 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json
--rw-r--r--   0     1001      123      972 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet
--rw-r--r--   0     1001      123      690 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet
--rw-r--r--   0     1001      123        0 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/files/empty.csv
--rw-r--r--   0     1001      123     5959 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/files/example.xlsx
--rw-r--r--   0     1001      123      457 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/files/foods1.csv
--rw-r--r--   0     1001      123     2351 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/files/foods1.ipc
--rw-r--r--   0     1001      123     1713 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/files/foods1.ndjson
--rw-r--r--   0     1001      123     1427 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/files/foods1.parquet
--rw-r--r--   0     1001      123      455 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/files/foods2.csv
--rw-r--r--   0     1001      123     2351 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/files/foods2.ipc
--rw-r--r--   0     1001      123     1711 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/files/foods2.ndjson
--rw-r--r--   0     1001      123     1916 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/files/foods2.parquet
--rw-r--r--   0     1001      123      455 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/files/foods3.csv
--rw-r--r--   0     1001      123      457 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/files/foods4.csv
--rw-r--r--   0     1001      123      452 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/files/foods5.csv
--rw-r--r--   0     1001      123       49 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/files/gzipped.csv
--rw-r--r--   0     1001      123       57 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/files/small.csv
--rw-r--r--   0     1001      123      756 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/files/small.parquet
--rw-r--r--   0     1001      123     1937 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/test_avro.py
--rw-r--r--   0     1001      123    39498 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/test_csv.py
--rw-r--r--   0     1001      123     6360 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/test_database.py
--rw-r--r--   0     1001      123     3456 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/test_delta.py
--rw-r--r--   0     1001      123    11169 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/test_excel.py
--rw-r--r--   0     1001      123     5919 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/test_ipc.py
--rw-r--r--   0     1001      123     3720 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/test_json.py
--rw-r--r--   0     1001      123     6849 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/test_lazy_csv.py
--rw-r--r--   0     1001      123     2060 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/test_lazy_ipc.py
--rw-r--r--   0     1001      123     2881 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/test_lazy_json.py
--rw-r--r--   0     1001      123    11849 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/test_lazy_parquet.py
--rw-r--r--   0     1001      123     2012 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/test_other.py
--rw-r--r--   0     1001      123    13735 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/test_parquet.py
--rw-r--r--   0     1001      123      612 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/test_pickle.py
--rw-r--r--   0     1001      123     3259 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/io/test_pyarrow_dataset.py
--rw-r--r--   0     1001      123      509 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/namespaces/__init__.py
--rw-r--r--   0     1001      123     3218 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/namespaces/test_binary.py
--rw-r--r--   0     1001      123     2489 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/namespaces/test_categorical.py
--rw-r--r--   0     1001      123    15436 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/namespaces/test_datetime.py
--rw-r--r--   0     1001      123    12750 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/namespaces/test_list.py
--rw-r--r--   0     1001      123     1748 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/namespaces/test_meta.py
--rw-r--r--   0     1001      123    23698 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/namespaces/test_string.py
--rw-r--r--   0     1001      123    15776 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/namespaces/test_strptime.py
--rw-r--r--   0     1001      123      982 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/namespaces/test_struct.py
--rw-r--r--   0     1001      123       85 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/operations/__init__.py
--rw-r--r--   0     1001      123     6238 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/operations/test_aggregations.py
--rw-r--r--   0     1001      123     9412 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/operations/test_apply.py
--rw-r--r--   0     1001      123     4390 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/operations/test_arithmetic.py
--rw-r--r--   0     1001      123      956 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/operations/test_comparison.py
--rw-r--r--   0     1001      123     2906 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/operations/test_drop.py
--rw-r--r--   0     1001      123     8252 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/operations/test_explode.py
--rw-r--r--   0     1001      123     3664 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/operations/test_filter.py
--rw-r--r--   0     1001      123     1801 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/operations/test_folds.py
--rw-r--r--   0     1001      123    22696 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/operations/test_groupby.py
--rw-r--r--   0     1001      123     2959 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/operations/test_is_in.py
--rw-r--r--   0     1001      123    16937 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/operations/test_join.py
--rw-r--r--   0     1001      123    10467 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/operations/test_join_asof.py
--rw-r--r--   0     1001      123      643 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/operations/test_melt.py
--rw-r--r--   0     1001      123    10253 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/operations/test_pivot.py
--rw-r--r--   0     1001      123    18639 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/operations/test_rolling.py
--rw-r--r--   0     1001      123    19550 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/operations/test_sort.py
--rw-r--r--   0     1001      123     3643 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/operations/test_statistics.py
--rw-r--r--   0     1001      123     3631 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/operations/test_transpose.py
--rw-r--r--   0     1001      123      771 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/operations/test_unique.py
--rw-r--r--   0     1001      123     9814 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/operations/test_window.py
--rw-r--r--   0     1001      123     4775 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/test_api.py
--rw-r--r--   0     1001      123     1077 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/test_arity.py
--rw-r--r--   0     1001      123    19856 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/test_cfg.py
--rw-r--r--   0     1001      123    39286 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/test_constructors.py
--rw-r--r--   0     1001      123      454 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/test_context.py
--rw-r--r--   0     1001      123     1628 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/test_cse.py
--rw-r--r--   0     1001      123     3497 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/test_datatypes.py
--rw-r--r--   0     1001      123   120890 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/test_df.py
--rw-r--r--   0     1001      123     1196 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/test_empty.py
--rw-r--r--   0     1001      123    16867 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/test_errors.py
--rw-r--r--   0     1001      123     2387 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/test_expr_multi_cols.py
--rw-r--r--   0     1001      123    32643 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/test_exprs.py
--rw-r--r--   0     1001      123     3305 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/test_fmt.py
--rw-r--r--   0     1001      123    11420 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/test_functions.py
--rw-r--r--   0     1001      123     3763 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/test_interchange.py
--rw-r--r--   0     1001      123    31618 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/test_interop.py
--rw-r--r--   0     1001      123    49534 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/test_lazy.py
--rw-r--r--   0     1001      123     2369 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/test_polars_import.py
--rw-r--r--   0     1001      123     4014 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/test_predicates.py
--rw-r--r--   0     1001      123     6995 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/test_projections.py
--rw-r--r--   0     1001      123    11550 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/test_queries.py
--rw-r--r--   0     1001      123     4743 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/test_rows.py
--rw-r--r--   0     1001      123    13181 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/test_schema.py
--rw-r--r--   0     1001      123     2634 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/test_serde.py
--rw-r--r--   0     1001      123    83663 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/test_series.py
--rw-r--r--   0     1001      123     2561 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/test_sql.py
--rw-r--r--   0     1001      123    13877 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/test_streaming.py
--rw-r--r--   0     1001      123    10700 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/test_testing.py
--rw-r--r--   0     1001      123       41 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/utils/__init__.py
--rw-r--r--   0     1001      123      306 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/utils/test_build_info.py
--rw-r--r--   0     1001      123      247 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/utils/test_show_versions.py
--rw-r--r--   0     1001      123     4307 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/tests/unit/utils/test_utils.py
--rw-r--r--   0     1001      123    66145 2023-04-21 14:00:20.000000 polars_u64_idx-0.17.6/Cargo.lock
--rw-r--r--   0        0        0    15163 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.6/PKG-INFO
+-rw-r--r--   0        0        0     1765 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/LICENSE
+-rw-r--r--   0     1001      123       98 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/mod.rs
+-rw-r--r--   0     1001      123     1219 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/operators/filter.rs
+-rw-r--r--   0     1001      123     4103 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/operators/function.rs
+-rw-r--r--   0     1001      123      229 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/operators/mod.rs
+-rw-r--r--   0     1001      123      548 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs
+-rw-r--r--   0     1001      123     3247 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/operators/projection.rs
+-rw-r--r--   0     1001      123     2324 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/operators/reproject.rs
+-rw-r--r--   0     1001      123     6479 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs
+-rw-r--r--   0     1001      123    10473 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs
+-rw-r--r--   0     1001      123     1207 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs
+-rw-r--r--   0     1001      123     1888 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs
+-rw-r--r--   0     1001      123     4554 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs
+-rw-r--r--   0     1001      123     1746 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs
+-rw-r--r--   0     1001      123     5413 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs
+-rw-r--r--   0     1001      123     4951 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs
+-rw-r--r--   0     1001      123      211 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mod.rs
+-rw-r--r--   0     1001      123      856 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs
+-rw-r--r--   0     1001      123     4294 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs
+-rw-r--r--   0     1001      123     3030 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs
+-rw-r--r--   0     1001      123     6275 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs
+-rw-r--r--   0     1001      123    13665 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs
+-rw-r--r--   0     1001      123     2681 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs
+-rw-r--r--   0     1001      123     2534 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs
+-rw-r--r--   0     1001      123     5961 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs
+-rw-r--r--   0     1001      123    10673 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs
+-rw-r--r--   0     1001      123     2164 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs
+-rw-r--r--   0     1001      123     4666 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs
+-rw-r--r--   0     1001      123     3906 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs
+-rw-r--r--   0     1001      123    20859 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs
+-rw-r--r--   0     1001      123    23518 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs
+-rw-r--r--   0     1001      123     2457 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs
+-rw-r--r--   0     1001      123     8395 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/io.rs
+-rw-r--r--   0     1001      123     5485 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs
+-rw-r--r--   0     1001      123    14279 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs
+-rw-r--r--   0     1001      123    11824 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs
+-rw-r--r--   0     1001      123      178 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/joins/mod.rs
+-rw-r--r--   0     1001      123     2002 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/memory.rs
+-rw-r--r--   0     1001      123      589 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/mod.rs
+-rw-r--r--   0     1001      123     1492 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs
+-rw-r--r--   0     1001      123     1824 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs
+-rw-r--r--   0     1001      123     3108 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/slice.rs
+-rw-r--r--   0     1001      123      130 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/sort/mod.rs
+-rw-r--r--   0     1001      123     3808 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs
+-rw-r--r--   0     1001      123     6295 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs
+-rw-r--r--   0     1001      123     5953 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs
+-rw-r--r--   0     1001      123     3801 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs
+-rw-r--r--   0     1001      123      635 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/utils.rs
+-rw-r--r--   0     1001      123     5076 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sources/csv.rs
+-rw-r--r--   0     1001      123     1231 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sources/frame.rs
+-rw-r--r--   0     1001      123      987 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs
+-rw-r--r--   0     1001      123      366 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sources/mod.rs
+-rw-r--r--   0     1001      123     3387 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sources/parquet.rs
+-rw-r--r--   0     1001      123     1146 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sources/reproject.rs
+-rw-r--r--   0     1001      123     1022 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sources/union.rs
+-rw-r--r--   0     1001      123      448 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/expressions.rs
+-rw-r--r--   0     1001      123      272 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/lib.rs
+-rw-r--r--   0     1001      123      719 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/operators/chunks.rs
+-rw-r--r--   0     1001      123      474 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/operators/context.rs
+-rw-r--r--   0     1001      123      223 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/operators/mod.rs
+-rw-r--r--   0     1001      123      430 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/operators/operator.rs
+-rw-r--r--   0     1001      123      626 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/operators/sink.rs
+-rw-r--r--   0     1001      123      241 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/operators/source.rs
+-rw-r--r--   0     1001      123        1 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/pipeline/config.rs
+-rw-r--r--   0     1001      123    20481 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/pipeline/convert.rs
+-rw-r--r--   0     1001      123    13982 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs
+-rw-r--r--   0     1001      123     1237 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/pipeline/mod.rs
+-rw-r--r--   0        0        0     3268 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/LICENSE
+-rw-r--r--   0     1001      123      234 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/binary/mod.rs
+-rw-r--r--   0     1001      123     3549 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs
+-rw-r--r--   0     1001      123    11023 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/interpolate.rs
+-rw-r--r--   0     1001      123     1679 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/list/count.rs
+-rw-r--r--   0     1001      123     2452 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/list/hash.rs
+-rw-r--r--   0     1001      123     7861 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs
+-rw-r--r--   0     1001      123      511 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/list/mod.rs
+-rw-r--r--   0     1001      123    22005 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs
+-rw-r--r--   0     1001      123     5269 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs
+-rw-r--r--   0     1001      123     2435 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs
+-rw-r--r--   0     1001      123      489 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/mod.rs
+-rw-r--r--   0     1001      123     9380 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs
+-rw-r--r--   0     1001      123     6795 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/set.rs
+-rw-r--r--   0     1001      123     7490 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/strings/case.rs
+-rw-r--r--   0     1001      123     8251 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs
+-rw-r--r--   0     1001      123     2345 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs
+-rw-r--r--   0     1001      123      514 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs
+-rw-r--r--   0     1001      123    14731 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs
+-rw-r--r--   0     1001      123     4053 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs
+-rw-r--r--   0     1001      123     2486 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/top_k.rs
+-rw-r--r--   0     1001      123     7727 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs
+-rw-r--r--   0     1001      123    18025 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/frame/join/mod.rs
+-rw-r--r--   0     1001      123     4174 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/frame/mod.rs
+-rw-r--r--   0     1001      123    10257 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/frame/pivot/mod.rs
+-rw-r--r--   0     1001      123    13486 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/frame/pivot/positioning.rs
+-rw-r--r--   0     1001      123      217 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/lib.rs
+-rw-r--r--   0     1001      123      290 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/prelude.rs
+-rw-r--r--   0     1001      123       25 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/series/mod.rs
+-rw-r--r--   0     1001      123     9623 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs
+-rw-r--r--   0     1001      123      118 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/series/ops/approx_algo/mod.rs
+-rw-r--r--   0     1001      123     2016 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/series/ops/approx_unique.rs
+-rw-r--r--   0     1001      123    11872 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs
+-rw-r--r--   0     1001      123     3680 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/series/ops/floor_divide.rs
+-rw-r--r--   0     1001      123     3423 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/series/ops/is_first.rs
+-rw-r--r--   0     1001      123     2975 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/series/ops/is_unique.rs
+-rw-r--r--   0     1001      123     3626 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/series/ops/log.rs
+-rw-r--r--   0     1001      123     1106 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/series/ops/mod.rs
+-rw-r--r--   0     1001      123     1769 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/series/ops/rolling.rs
+-rw-r--r--   0     1001      123     7642 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/series/ops/search_sorted.rs
+-rw-r--r--   0     1001      123     2500 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/series/ops/to_dummies.rs
+-rw-r--r--   0     1001      123     2067 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/series/ops/various.rs
+-rw-r--r--   0        0        0     5241 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/LICENSE
+-rw-r--r--   0     1001      123       45 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/constants.rs
+-rw-r--r--   0     1001      123    17248 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dot.rs
+-rw-r--r--   0     1001      123     4171 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/arithmetic.rs
+-rw-r--r--   0     1001      123      935 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/binary.rs
+-rw-r--r--   0     1001      123      650 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/cat.rs
+-rw-r--r--   0     1001      123     9424 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/dt.rs
+-rw-r--r--   0     1001      123    13169 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/expr.rs
+-rw-r--r--   0     1001      123      753 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/from.rs
+-rw-r--r--   0     1001      123       85 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/abs.rs
+-rw-r--r--   0     1001      123     1431 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs
+-rw-r--r--   0     1001      123     1327 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs
+-rw-r--r--   0     1001      123     4221 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs
+-rw-r--r--   0     1001      123     1910 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs
+-rw-r--r--   0     1001      123     1216 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs
+-rw-r--r--   0     1001      123      344 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/clip.rs
+-rw-r--r--   0     1001      123     1593 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs
+-rw-r--r--   0     1001      123    13227 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs
+-rw-r--r--   0     1001      123      810 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs
+-rw-r--r--   0     1001      123     2541 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs
+-rw-r--r--   0     1001      123     8119 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/list.rs
+-rw-r--r--   0     1001      123      581 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/log.rs
+-rw-r--r--   0     1001      123    19222 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs
+-rw-r--r--   0     1001      123      462 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/nan.rs
+-rw-r--r--   0     1001      123     3132 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs
+-rw-r--r--   0     1001      123      152 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/rolling.rs
+-rw-r--r--   0     1001      123      260 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/round.rs
+-rw-r--r--   0     1001      123      200 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/row_hash.rs
+-rw-r--r--   0     1001      123    13416 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs
+-rw-r--r--   0     1001      123      306 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/search_sorted.rs
+-rw-r--r--   0     1001      123     3812 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs
+-rw-r--r--   0     1001      123     1238 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs
+-rw-r--r--   0     1001      123      972 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs
+-rw-r--r--   0     1001      123    19923 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs
+-rw-r--r--   0     1001      123     1017 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs
+-rw-r--r--   0     1001      123     2700 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs
+-rw-r--r--   0     1001      123     5122 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs
+-rw-r--r--   0     1001      123      170 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/unique.rs
+-rw-r--r--   0     1001      123    43864 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/functions.rs
+-rw-r--r--   0     1001      123    10196 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/list.rs
+-rw-r--r--   0     1001      123     2181 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/meta.rs
+-rw-r--r--   0     1001      123    64804 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/mod.rs
+-rw-r--r--   0     1001      123       40 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/names.rs
+-rw-r--r--   0     1001      123     2100 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/options.rs
+-rw-r--r--   0     1001      123    15238 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/string.rs
+-rw-r--r--   0     1001      123     2715 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/struct_.rs
+-rw-r--r--   0     1001      123       38 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/frame/mod.rs
+-rw-r--r--   0     1001      123      933 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/frame/opt_state.rs
+-rw-r--r--   0     1001      123      466 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/global.rs
+-rw-r--r--   0     1001      123      175 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/lib.rs
+-rw-r--r--   0     1001      123     6825 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs
+-rw-r--r--   0     1001      123    11393 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs
+-rw-r--r--   0     1001      123    25656 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/alp.rs
+-rw-r--r--   0     1001      123     1622 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs
+-rw-r--r--   0     1001      123     1428 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/apply.rs
+-rw-r--r--   0     1001      123    24898 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/builder.rs
+-rw-r--r--   0     1001      123    29652 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/conversion.rs
+-rw-r--r--   0     1001      123      301 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/debug.rs
+-rw-r--r--   0     1001      123    15191 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/format.rs
+-rw-r--r--   0     1001      123      895 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs
+-rw-r--r--   0     1001      123      137 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/functions/explode.rs
+-rw-r--r--   0     1001      123     1169 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs
+-rw-r--r--   0     1001      123    11905 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs
+-rw-r--r--   0     1001      123     1330 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs
+-rw-r--r--   0     1001      123     9752 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/iterator.rs
+-rw-r--r--   0     1001      123    10463 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/lit.rs
+-rw-r--r--   0     1001      123     8115 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/mod.rs
+-rw-r--r--   0     1001      123     7416 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs
+-rw-r--r--   0     1001      123    15277 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs
+-rw-r--r--   0     1001      123     3250 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs
+-rw-r--r--   0     1001      123     3236 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs
+-rw-r--r--   0     1001      123     3994 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs
+-rw-r--r--   0     1001      123    14479 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs
+-rw-r--r--   0     1001      123     1556 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs
+-rw-r--r--   0     1001      123     6644 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs
+-rw-r--r--   0     1001      123     1222 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs
+-rw-r--r--   0     1001      123    28276 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs
+-rw-r--r--   0     1001      123     2571 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs
+-rw-r--r--   0     1001      123    15130 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs
+-rw-r--r--   0     1001      123     1755 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs
+-rw-r--r--   0     1001      123     3930 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs
+-rw-r--r--   0     1001      123     1799 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs
+-rw-r--r--   0     1001      123     3269 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs
+-rw-r--r--   0     1001      123     2638 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs
+-rw-r--r--   0     1001      123    15747 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs
+-rw-r--r--   0     1001      123    26502 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs
+-rw-r--r--   0     1001      123     2692 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs
+-rw-r--r--   0     1001      123     2639 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs
+-rw-r--r--   0     1001      123     3501 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs
+-rw-r--r--   0     1001      123    27361 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs
+-rw-r--r--   0     1001      123     3492 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs
+-rw-r--r--   0     1001      123    13845 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs
+-rw-r--r--   0     1001      123     3161 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs
+-rw-r--r--   0     1001      123     9725 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs
+-rw-r--r--   0     1001      123    19820 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs
+-rw-r--r--   0     1001      123    10187 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/options.rs
+-rw-r--r--   0     1001      123    15276 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/projection.rs
+-rw-r--r--   0     1001      123     4584 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs
+-rw-r--r--   0     1001      123    13038 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/schema.rs
+-rw-r--r--   0     1001      123      809 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/prelude.rs
+-rw-r--r--   0     1001      123    11879 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/utils.rs
+-rw-r--r--   0        0        0     2055 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/LICENSE
+-rw-r--r--   0     1001      123     3565 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/chunkedarray/date.rs
+-rw-r--r--   0     1001      123     6465 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/chunkedarray/datetime.rs
+-rw-r--r--   0     1001      123     3305 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/chunkedarray/duration.rs
+-rw-r--r--   0     1001      123     5607 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/chunkedarray/kernels.rs
+-rw-r--r--   0     1001      123     1062 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/chunkedarray/mod.rs
+-rw-r--r--   0     1001      123     7302 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs
+-rw-r--r--   0     1001      123     2582 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs
+-rw-r--r--   0     1001      123    10476 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs
+-rw-r--r--   0     1001      123      428 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/mod.rs
+-rw-r--r--   0     1001      123     7368 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs
+-rw-r--r--   0     1001      123     2717 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/chunkedarray/time.rs
+-rw-r--r--   0     1001      123    21192 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs
+-rw-r--r--   0     1001      123    20108 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs
+-rw-r--r--   0     1001      123     4115 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs
+-rw-r--r--   0     1001      123     9692 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs
+-rw-r--r--   0     1001      123     2960 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/date_range.rs
+-rw-r--r--   0     1001      123    31413 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/groupby/dynamic.rs
+-rw-r--r--   0     1001      123       88 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/groupby/mod.rs
+-rw-r--r--   0     1001      123      535 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/lib.rs
+-rw-r--r--   0     1001      123      320 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/prelude.rs
+-rw-r--r--   0     1001      123     1568 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/round.rs
+-rw-r--r--   0     1001      123     4028 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/series/_trait.rs
+-rw-r--r--   0     1001      123      136 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/series/implementations/boolean.rs
+-rw-r--r--   0     1001      123      140 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/series/implementations/categoricals.rs
+-rw-r--r--   0     1001      123      133 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/series/implementations/date.rs
+-rw-r--r--   0     1001      123      137 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/series/implementations/datetime.rs
+-rw-r--r--   0     1001      123      137 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/series/implementations/duration.rs
+-rw-r--r--   0     1001      123     1863 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/series/implementations/floats.rs
+-rw-r--r--   0     1001      123     1792 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/series/implementations/integers.rs
+-rw-r--r--   0     1001      123      133 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/series/implementations/list.rs
+-rw-r--r--   0     1001      123      486 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/series/implementations/mod.rs
+-rw-r--r--   0     1001      123      155 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/series/implementations/object.rs
+-rw-r--r--   0     1001      123      135 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/series/implementations/struct_.rs
+-rw-r--r--   0     1001      123      133 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/series/implementations/time.rs
+-rw-r--r--   0     1001      123      133 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/series/implementations/utf8.rs
+-rw-r--r--   0     1001      123    12466 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/series/mod.rs
+-rw-r--r--   0     1001      123     1630 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/truncate.rs
+-rw-r--r--   0     1001      123     7059 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/upsample.rs
+-rw-r--r--   0     1001      123     2567 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/utils.rs
+-rw-r--r--   0     1001      123     1524 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/windows/bounds.rs
+-rw-r--r--   0     1001      123     2008 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/windows/calendar.rs
+-rw-r--r--   0     1001      123    23538 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/windows/duration.rs
+-rw-r--r--   0     1001      123    20089 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/windows/groupby.rs
+-rw-r--r--   0     1001      123      503 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/windows/mod.rs
+-rw-r--r--   0     1001      123    24202 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/windows/test.rs
+-rw-r--r--   0     1001      123    11624 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-time/src/windows/window.rs
+-rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.7/local_dependencies/polars-utils/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-utils/LICENSE
+-rw-r--r--   0     1001      123     2645 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/arena.rs
+-rw-r--r--   0     1001      123     1373 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/atomic.rs
+-rw-r--r--   0     1001      123     2659 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/cell.rs
+-rw-r--r--   0     1001      123     1015 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/contention_pool.rs
+-rw-r--r--   0     1001      123      509 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/error.rs
+-rw-r--r--   0     1001      123      271 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/fmt.rs
+-rw-r--r--   0     1001      123      763 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/functions.rs
+-rw-r--r--   0     1001      123      514 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/hash.rs
+-rw-r--r--   0     1001      123     2709 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/iter/enumerate_idx.rs
+-rw-r--r--   0     1001      123       61 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/iter/mod.rs
+-rw-r--r--   0     1001      123      583 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/lib.rs
+-rw-r--r--   0     1001      123      573 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/macros.rs
+-rw-r--r--   0     1001      123      282 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/mem.rs
+-rw-r--r--   0     1001      123     1792 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/slice.rs
+-rw-r--r--   0     1001      123     2467 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/sort.rs
+-rw-r--r--   0     1001      123     1115 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/sync.rs
+-rw-r--r--   0     1001      123      504 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/sys.rs
+-rw-r--r--   0     1001      123      697 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/unwrap.rs
+-rw-r--r--   0     1001      123      616 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/wasm.rs
+-rw-r--r--   0        0        0    10541 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.7/local_dependencies/polars/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/LICENSE
+-rw-r--r--   0     1001      123     3249 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/Makefile
+-rw-r--r--   0     1001      123      215 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/build.rs
+-rw-r--r--   0     1001      123       78 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/clippy.toml
+-rw-r--r--   0     1001      123    17602 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/src/docs/eager.rs
+-rw-r--r--   0     1001      123     8778 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/src/docs/lazy.rs
+-rw-r--r--   0     1001      123       50 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/src/docs/mod.rs
+-rw-r--r--   0     1001      123     3797 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/src/docs/performance.rs
+-rw-r--r--   0     1001      123       59 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/src/export.rs
+-rw-r--r--   0     1001      123    20207 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/src/lib.rs
+-rw-r--r--   0     1001      123      387 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/src/prelude.rs
+-rw-r--r--   0     1001      123       44 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/src/sql.rs
+-rw-r--r--   0     1001      123     4272 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/core/date_like.rs
+-rw-r--r--   0     1001      123     2401 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/core/groupby.rs
+-rw-r--r--   0     1001      123    17826 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/core/joins.rs
+-rw-r--r--   0     1001      123      545 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/core/list.rs
+-rw-r--r--   0     1001      123      189 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/core/mod.rs
+-rw-r--r--   0     1001      123     6258 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/core/pivot.rs
+-rw-r--r--   0     1001      123     1102 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/core/random.rs
+-rw-r--r--   0     1001      123    10844 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/core/rolling_window.rs
+-rw-r--r--   0     1001      123     1093 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/core/series.rs
+-rw-r--r--   0     1001      123      370 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/core/utils.rs
+-rw-r--r--   0     1001      123    30013 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/io/csv.rs
+-rw-r--r--   0     1001      123     4490 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/io/ipc_stream.rs
+-rw-r--r--   0     1001      123     7044 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/io/json.rs
+-rw-r--r--   0     1001      123      378 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/io/mod.rs
+-rw-r--r--   0     1001      123      988 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/io/parquet.rs
+-rw-r--r--   0     1001      123     1530 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/joins.rs
+-rw-r--r--   0     1001      123     2452 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/aggregation.rs
+-rw-r--r--   0     1001      123      702 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/cse.rs
+-rw-r--r--   0     1001      123      500 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/explodes.rs
+-rw-r--r--   0     1001      123     2279 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/expressions/apply.rs
+-rw-r--r--   0     1001      123    10285 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/expressions/arity.rs
+-rw-r--r--   0     1001      123     1064 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/expressions/expand.rs
+-rw-r--r--   0     1001      123     1008 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/expressions/filter.rs
+-rw-r--r--   0     1001      123      428 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/expressions/is_in.rs
+-rw-r--r--   0     1001      123      121 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/expressions/mod.rs
+-rw-r--r--   0     1001      123      659 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/expressions/slice.rs
+-rw-r--r--   0     1001      123    10139 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/expressions/window.rs
+-rw-r--r--   0     1001      123      579 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/folds.rs
+-rw-r--r--   0     1001      123      557 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/functions.rs
+-rw-r--r--   0     1001      123     4482 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/groupby.rs
+-rw-r--r--   0     1001      123     1655 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs
+-rw-r--r--   0     1001      123      691 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/mod.rs
+-rw-r--r--   0     1001      123     5381 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/predicate_queries.rs
+-rw-r--r--   0     1001      123     4476 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/projection_queries.rs
+-rw-r--r--   0     1001      123     6444 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/queries.rs
+-rw-r--r--   0     1001      123      141 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/main.rs
+-rw-r--r--   0     1001      123    12591 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/schema.rs
+-rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.7/local_dependencies/polars-row/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-row/LICENSE
+-rw-r--r--   0     1001      123     8985 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-row/src/encode.rs
+-rw-r--r--   0     1001      123     4591 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-row/src/encodings/fixed.rs
+-rw-r--r--   0     1001      123       47 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-row/src/encodings/mod.rs
+-rw-r--r--   0     1001      123     4508 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-row/src/encodings/variable.rs
+-rw-r--r--   0     1001      123    13678 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-row/src/lib.rs
+-rw-r--r--   0     1001      123     2079 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-row/src/row.rs
+-rw-r--r--   0     1001      123      682 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-row/src/utils.rs
+-rw-r--r--   0        0        0     5450 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/LICENSE
+-rw-r--r--   0     1001      123    19606 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/arithmetic.rs
+-rw-r--r--   0     1001      123     8679 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/bitwise.rs
+-rw-r--r--   0     1001      123     2298 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/builder/binary.rs
+-rw-r--r--   0     1001      123     1207 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs
+-rw-r--r--   0     1001      123     1556 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/builder/from.rs
+-rw-r--r--   0     1001      123    20366 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/builder/list.rs
+-rw-r--r--   0     1001      123     8845 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/builder/mod.rs
+-rw-r--r--   0     1001      123     1410 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs
+-rw-r--r--   0     1001      123     2291 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs
+-rw-r--r--   0     1001      123    11560 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/cast.rs
+-rw-r--r--   0     1001      123    48300 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs
+-rw-r--r--   0     1001      123     9463 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs
+-rw-r--r--   0     1001      123      551 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/drop.rs
+-rw-r--r--   0     1001      123      963 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/float.rs
+-rw-r--r--   0     1001      123     5069 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/from.rs
+-rw-r--r--   0     1001      123    38411 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs
+-rw-r--r--   0     1001      123     1395 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs
+-rw-r--r--   0     1001      123       28 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/iterator/par/mod.rs
+-rw-r--r--   0     1001      123     1129 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs
+-rw-r--r--   0     1001      123       21 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/kernels/mod.rs
+-rw-r--r--   0     1001      123     2986 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/kernels/take.rs
+-rw-r--r--   0     1001      123     7728 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/list/iterator.rs
+-rw-r--r--   0     1001      123     2802 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/list/mod.rs
+-rw-r--r--   0     1001      123    19796 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs
+-rw-r--r--   0     1001      123     3688 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs
+-rw-r--r--   0     1001      123     4270 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs
+-rw-r--r--   0     1001      123    10220 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs
+-rw-r--r--   0     1001      123     1400 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs
+-rw-r--r--   0     1001      123      358 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/full.rs
+-rw-r--r--   0     1001      123      192 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/mod.rs
+-rw-r--r--   0     1001      123     2731 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs
+-rw-r--r--   0     1001      123     2172 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs
+-rw-r--r--   0     1001      123      925 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs
+-rw-r--r--   0     1001      123     6453 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs
+-rw-r--r--   0     1001      123     1604 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/date.rs
+-rw-r--r--   0     1001      123     4105 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs
+-rw-r--r--   0     1001      123     4443 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs
+-rw-r--r--   0     1001      123     2434 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/duration.rs
+-rw-r--r--   0     1001      123     2549 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/mod.rs
+-rw-r--r--   0     1001      123      476 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/struct_/from.rs
+-rw-r--r--   0     1001      123    15081 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs
+-rw-r--r--   0     1001      123     1182 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/time.rs
+-rw-r--r--   0     1001      123    23524 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/mod.rs
+-rw-r--r--   0     1001      123     7200 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ndarray.rs
+-rw-r--r--   0     1001      123     4484 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/object/builder.rs
+-rw-r--r--   0     1001      123     1547 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs
+-rw-r--r--   0     1001      123     3124 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs
+-rw-r--r--   0     1001      123     7054 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs
+-rw-r--r--   0     1001      123     3410 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs
+-rw-r--r--   0     1001      123      137 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/object/is_valid.rs
+-rw-r--r--   0     1001      123     4419 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/object/iterator.rs
+-rw-r--r--   0     1001      123     4826 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/object/mod.rs
+-rw-r--r--   0     1001      123     2853 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/object/registry.rs
+-rw-r--r--   0     1001      123      272 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/abs.rs
+-rw-r--r--   0     1001      123    32120 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs
+-rw-r--r--   0     1001      123     9946 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs
+-rw-r--r--   0     1001      123     2875 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs
+-rw-r--r--   0     1001      123     9670 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs
+-rw-r--r--   0     1001      123     2365 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/append.rs
+-rw-r--r--   0     1001      123    27269 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/apply.rs
+-rw-r--r--   0     1001      123    12799 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs
+-rw-r--r--   0     1001      123     6214 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs
+-rw-r--r--   0     1001      123    11537 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs
+-rw-r--r--   0     1001      123     1737 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs
+-rw-r--r--   0     1001      123     4801 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs
+-rw-r--r--   0     1001      123     6264 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs
+-rw-r--r--   0     1001      123    25614 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/explode.rs
+-rw-r--r--   0     1001      123     8339 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/extend.rs
+-rw-r--r--   0     1001      123    13777 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs
+-rw-r--r--   0     1001      123     5308 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/filter.rs
+-rw-r--r--   0     1001      123     4436 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/full.rs
+-rw-r--r--   0     1001      123        1 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/interpolate.rs
+-rw-r--r--   0     1001      123    15385 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs
+-rw-r--r--   0     1001      123        1 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/len.rs
+-rw-r--r--   0     1001      123    22376 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/mod.rs
+-rw-r--r--   0     1001      123     2403 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs
+-rw-r--r--   0     1001      123      593 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs
+-rw-r--r--   0     1001      123     2585 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs
+-rw-r--r--   0     1001      123     1539 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs
+-rw-r--r--   0     1001      123    10234 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs
+-rw-r--r--   0     1001      123    12518 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/set.rs
+-rw-r--r--   0     1001      123     6151 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/shift.rs
+-rw-r--r--   0     1001      123     2299 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs
+-rw-r--r--   0     1001      123     5467 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs
+-rw-r--r--   0     1001      123     7430 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs
+-rw-r--r--   0     1001      123    30762 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs
+-rw-r--r--   0     1001      123      380 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/sort/slice.rs
+-rw-r--r--   0     1001      123    20472 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs
+-rw-r--r--   0     1001      123     6630 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs
+-rw-r--r--   0     1001      123     1859 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs
+-rw-r--r--   0     1001      123    16256 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs
+-rw-r--r--   0     1001      123     5041 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs
+-rw-r--r--   0     1001      123     6064 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs
+-rw-r--r--   0     1001      123    11229 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs
+-rw-r--r--   0     1001      123    14620 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs
+-rw-r--r--   0     1001      123     7753 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/zip.rs
+-rw-r--r--   0     1001      123     9093 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/random.rs
+-rw-r--r--   0     1001      123     1959 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs
+-rw-r--r--   0     1001      123     2501 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/temporal/date.rs
+-rw-r--r--   0     1001      123    11998 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs
+-rw-r--r--   0     1001      123     3201 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs
+-rw-r--r--   0     1001      123      533 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs
+-rw-r--r--   0     1001      123     2724 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/temporal/time.rs
+-rw-r--r--   0     1001      123      872 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/to_vec.rs
+-rw-r--r--   0     1001      123     8113 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/trusted_len.rs
+-rw-r--r--   0     1001      123    25934 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs
+-rw-r--r--   0     1001      123     7689 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/cloud.rs
+-rw-r--r--   0     1001      123     1549 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/config.rs
+-rw-r--r--   0     1001      123     3946 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/datatypes/_serde.rs
+-rw-r--r--   0     1001      123     2650 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/datatypes/aliases.rs
+-rw-r--r--   0     1001      123    42410 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/datatypes/any_value.rs
+-rw-r--r--   0     1001      123    12083 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/datatypes/dtype.rs
+-rw-r--r--   0     1001      123     5456 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/datatypes/field.rs
+-rw-r--r--   0     1001      123     7675 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/datatypes/mod.rs
+-rw-r--r--   0     1001      123     2016 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/datatypes/time_unit.rs
+-rw-r--r--   0     1001      123      118 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/doc/changelog/mod.rs
+-rw-r--r--   0     1001      123      898 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs
+-rw-r--r--   0     1001      123      481 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/doc/changelog/v0_3.rs
+-rw-r--r--   0     1001      123      293 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/doc/changelog/v0_4.rs
+-rw-r--r--   0     1001      123      499 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/doc/changelog/v0_5.rs
+-rw-r--r--   0     1001      123      288 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/doc/changelog/v0_6.rs
+-rw-r--r--   0     1001      123     1071 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/doc/changelog/v0_7.rs
+-rw-r--r--   0     1001      123      819 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/doc/changelog/v0_8.rs
+-rw-r--r--   0     1001      123      596 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/doc/changelog/v0_9.rs
+-rw-r--r--   0     1001      123       43 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/doc/mod.rs
+-rw-r--r--   0     1001      123       25 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/error.rs
+-rw-r--r--   0     1001      123      433 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/export.rs
+-rw-r--r--   0     1001      123    36116 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/fmt.rs
+-rw-r--r--   0     1001      123     5177 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/arithmetic.rs
+-rw-r--r--   0     1001      123     7874 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/asof_join/asof.rs
+-rw-r--r--   0     1001      123    33715 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/asof_join/groups.rs
+-rw-r--r--   0     1001      123     6634 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/asof_join/mod.rs
+-rw-r--r--   0     1001      123      559 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/chunks.rs
+-rw-r--r--   0     1001      123     5179 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/cross_join.rs
+-rw-r--r--   0     1001      123    16609 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/explode.rs
+-rw-r--r--   0     1001      123     1019 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/from.rs
+-rw-r--r--   0     1001      123    16518 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs
+-rw-r--r--   0     1001      123     4115 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs
+-rw-r--r--   0     1001      123     7643 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs
+-rw-r--r--   0     1001      123    39255 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs
+-rw-r--r--   0     1001      123     5636 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs
+-rw-r--r--   0     1001      123      218 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/groupby/expr.rs
+-rw-r--r--   0     1001      123    15470 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/groupby/hashing.rs
+-rw-r--r--   0     1001      123    14048 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/groupby/into_groups.rs
+-rw-r--r--   0     1001      123    39375 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/groupby/mod.rs
+-rw-r--r--   0     1001      123    10593 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/groupby/perfect.rs
+-rw-r--r--   0     1001      123    17214 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/groupby/proxy.rs
+-rw-r--r--   0     1001      123    18264 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/hash_join/mod.rs
+-rw-r--r--   0     1001      123    22392 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs
+-rw-r--r--   0     1001      123     2413 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs
+-rw-r--r--   0     1001      123    16352 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs
+-rw-r--r--   0     1001      123     4295 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs
+-rw-r--r--   0     1001      123     6076 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs
+-rw-r--r--   0     1001      123     4247 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs
+-rw-r--r--   0     1001      123     3913 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs
+-rw-r--r--   0     1001      123    11879 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs
+-rw-r--r--   0     1001      123   124236 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/mod.rs
+-rw-r--r--   0     1001      123    27513 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/row/av_buffer.rs
+-rw-r--r--   0     1001      123     3732 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/row/dataframe.rs
+-rw-r--r--   0     1001      123     5976 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/row/mod.rs
+-rw-r--r--   0     1001      123     8795 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/row/transpose.rs
+-rw-r--r--   0     1001      123     2183 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/top_k.rs
+-rw-r--r--   0     1001      123     1388 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/upstream_traits.rs
+-rw-r--r--   0     1001      123    10935 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/functions.rs
+-rw-r--r--   0     1001      123     2149 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/hashing/fx.rs
+-rw-r--r--   0     1001      123     1503 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/hashing/identity.rs
+-rw-r--r--   0     1001      123      457 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/hashing/mod.rs
+-rw-r--r--   0     1001      123     2684 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/hashing/partition.rs
+-rw-r--r--   0     1001      123    17653 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/hashing/vector_hasher.rs
+-rw-r--r--   0     1001      123     1896 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/lib.rs
+-rw-r--r--   0     1001      123    15733 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/named_from.rs
+-rw-r--r--   0     1001      123     2411 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/prelude.rs
+-rw-r--r--   0     1001      123    16406 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/schema.rs
+-rw-r--r--   0     1001      123     4218 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/serde/chunked_array.rs
+-rw-r--r--   0     1001      123     6551 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/serde/mod.rs
+-rw-r--r--   0     1001      123     9929 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/serde/series.rs
+-rw-r--r--   0     1001      123    18441 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/any_value.rs
+-rw-r--r--   0     1001      123    28511 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs
+-rw-r--r--   0     1001      123      222 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/arithmetic/mod.rs
+-rw-r--r--   0     1001      123     3546 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/arithmetic/owned.rs
+-rw-r--r--   0     1001      123    13187 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/comparison.rs
+-rw-r--r--   0     1001      123    25008 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/from.rs
+-rw-r--r--   0     1001      123     9217 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/implementations/binary.rs
+-rw-r--r--   0     1001      123    10850 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/implementations/boolean.rs
+-rw-r--r--   0     1001      123    12962 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/implementations/categorical.rs
+-rw-r--r--   0     1001      123    18304 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/implementations/dates_time.rs
+-rw-r--r--   0     1001      123    15242 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/implementations/datetime.rs
+-rw-r--r--   0     1001      123     5829 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/implementations/decimal.rs
+-rw-r--r--   0     1001      123    15106 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/implementations/duration.rs
+-rw-r--r--   0     1001      123    14223 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/implementations/floats.rs
+-rw-r--r--   0     1001      123     6207 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/implementations/list.rs
+-rw-r--r--   0     1001      123    18305 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/implementations/mod.rs
+-rw-r--r--   0     1001      123     5336 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/implementations/null.rs
+-rw-r--r--   0     1001      123     8004 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/implementations/object.rs
+-rw-r--r--   0     1001      123    11029 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/implementations/struct_.rs
+-rw-r--r--   0     1001      123     9735 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/implementations/utf8.rs
+-rw-r--r--   0     1001      123     4471 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/into.rs
+-rw-r--r--   0     1001      123     6297 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/iterator.rs
+-rw-r--r--   0     1001      123    37684 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/mod.rs
+-rw-r--r--   0     1001      123      853 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/ops/diff.rs
+-rw-r--r--   0     1001      123     5204 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/ops/downcast.rs
+-rw-r--r--   0     1001      123     3601 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/ops/ewm.rs
+-rw-r--r--   0     1001      123      413 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/ops/extend.rs
+-rw-r--r--   0     1001      123      562 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/ops/mod.rs
+-rw-r--r--   0     1001      123     5974 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/ops/moment.rs
+-rw-r--r--   0     1001      123     2908 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/ops/null.rs
+-rw-r--r--   0     1001      123     1347 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/ops/pct_change.rs
+-rw-r--r--   0     1001      123     4247 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/ops/round.rs
+-rw-r--r--   0     1001      123     5072 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/ops/to_list.rs
+-rw-r--r--   0     1001      123     1476 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/ops/unique.rs
+-rw-r--r--   0     1001      123    18204 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/series_trait.rs
+-rw-r--r--   0     1001      123     2840 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/unstable.rs
+-rw-r--r--   0     1001      123     8117 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/testing.rs
+-rw-r--r--   0     1001      123      508 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/tests.rs
+-rw-r--r--   0     1001      123     1396 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/utils/flatten.rs
+-rw-r--r--   0     1001      123    31704 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/utils/mod.rs
+-rw-r--r--   0     1001      123     1598 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/utils/series.rs
+-rw-r--r--   0     1001      123    13773 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-core/src/utils/supertype.rs
+-rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/LICENSE
+-rw-r--r--   0     1001      123     1975 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/array/default_arrays.rs
+-rw-r--r--   0     1001      123     3160 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/array/get.rs
+-rw-r--r--   0     1001      123     6459 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/array/list.rs
+-rw-r--r--   0     1001      123     7771 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/array/mod.rs
+-rw-r--r--   0     1001      123      878 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/array/null.rs
+-rw-r--r--   0     1001      123     1125 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/array/slice.rs
+-rw-r--r--   0     1001      123     1807 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/array/utf8.rs
+-rw-r--r--   0     1001      123     2294 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/bit_util.rs
+-rw-r--r--   0     1001      123       17 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/bitmap/mod.rs
+-rw-r--r--   0     1001      123      819 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/bitmap/mutable.rs
+-rw-r--r--   0     1001      123      232 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/compute/cast.rs
+-rw-r--r--   0     1001      123       56 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/compute/mod.rs
+-rw-r--r--   0     1001      123     2962 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/compute/take/boolean.rs
+-rw-r--r--   0     1001      123    24907 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/compute/take/mod.rs
+-rw-r--r--   0     1001      123     1042 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/conversion.rs
+-rw-r--r--   0     1001      123     1609 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/data_types.rs
+-rw-r--r--   0     1001      123       25 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/error.rs
+-rw-r--r--   0     1001      123       28 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/export.rs
+-rw-r--r--   0     1001      123       26 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/floats/mod.rs
+-rw-r--r--   0     1001      123     2066 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/floats/ord.rs
+-rw-r--r--   0     1001      123     1273 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/index.rs
+-rw-r--r--   0     1001      123      915 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/is_valid.rs
+-rw-r--r--   0     1001      123     4740 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/agg_mean.rs
+-rw-r--r--   0     1001      123     1015 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/concatenate.rs
+-rw-r--r--   0     1001      123     5161 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/ewm/average.rs
+-rw-r--r--   0     1001      123     1808 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs
+-rw-r--r--   0     1001      123    25065 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs
+-rw-r--r--   0     1001      123     1406 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/float.rs
+-rw-r--r--   0     1001      123     4907 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/list.rs
+-rw-r--r--   0     1001      123     1895 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs
+-rw-r--r--   0     1001      123     9731 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/mod.rs
+-rw-r--r--   0     1001      123     3703 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs
+-rw-r--r--   0     1001      123     2022 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs
+-rw-r--r--   0     1001      123    18684 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs
+-rw-r--r--   0     1001      123     3924 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs
+-rw-r--r--   0     1001      123    11659 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs
+-rw-r--r--   0     1001      123     5504 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs
+-rw-r--r--   0     1001      123     8683 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs
+-rw-r--r--   0     1001      123     1749 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs
+-rw-r--r--   0     1001      123    14367 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs
+-rw-r--r--   0     1001      123     9070 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs
+-rw-r--r--   0     1001      123    11609 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs
+-rw-r--r--   0     1001      123     4698 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs
+-rw-r--r--   0     1001      123     8335 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs
+-rw-r--r--   0     1001      123     8109 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/window.rs
+-rw-r--r--   0     1001      123     4752 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/set.rs
+-rw-r--r--   0     1001      123     4529 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/sort_partition.rs
+-rw-r--r--   0     1001      123     2948 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs
+-rw-r--r--   0     1001      123     5974 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs
+-rw-r--r--   0     1001      123      231 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/sorted_join/mod.rs
+-rw-r--r--   0     1001      123      841 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/string.rs
+-rw-r--r--   0     1001      123     2310 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs
+-rw-r--r--   0     1001      123     4343 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs
+-rw-r--r--   0     1001      123     2606 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs
+-rw-r--r--   0     1001      123     4417 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/time.rs
+-rw-r--r--   0     1001      123      341 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/lib.rs
+-rw-r--r--   0     1001      123      434 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/prelude.rs
+-rw-r--r--   0     1001      123      534 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/slice.rs
+-rw-r--r--   0     1001      123      762 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/time_zone.rs
+-rw-r--r--   0     1001      123      998 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/trusted_len/boolean.rs
+-rw-r--r--   0     1001      123     2821 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/trusted_len/mod.rs
+-rw-r--r--   0     1001      123     2533 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs
+-rw-r--r--   0     1001      123      158 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/trusted_len/rev.rs
+-rw-r--r--   0     1001      123     5020 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/utils.rs
+-rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.7/local_dependencies/polars-sql/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-sql/LICENSE
+-rw-r--r--   0     1001      123    15314 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-sql/src/context.rs
+-rw-r--r--   0     1001      123    17592 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-sql/src/functions.rs
+-rw-r--r--   0     1001      123     1920 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-sql/src/keywords.rs
+-rw-r--r--   0     1001      123    28145 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-sql/src/lib.rs
+-rw-r--r--   0     1001      123    15237 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-sql/src/sql_expr.rs
+-rw-r--r--   0     1001      123     4572 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-sql/src/table_functions.rs
+-rw-r--r--   0        0        0     5977 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/LICENSE
+-rw-r--r--   0     1001      123     1796 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/dot.rs
+-rw-r--r--   0     1001      123     4359 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/dsl/eval.rs
+-rw-r--r--   0     1001      123     4505 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/dsl/functions.rs
+-rw-r--r--   0     1001      123      164 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/dsl/into.rs
+-rw-r--r--   0     1001      123     6754 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/dsl/list.rs
+-rw-r--r--   0     1001      123     2899 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/dsl/mod.rs
+-rw-r--r--   0     1001      123     1182 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs
+-rw-r--r--   0     1001      123     9278 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/frame/csv.rs
+-rw-r--r--   0     1001      123     4309 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/frame/file_list_reader.rs
+-rw-r--r--   0     1001      123     2261 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/frame/ipc.rs
+-rw-r--r--   0     1001      123    47176 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/frame/mod.rs
+-rw-r--r--   0     1001      123     3414 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/frame/ndjson.rs
+-rw-r--r--   0     1001      123     3440 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/frame/parquet.rs
+-rw-r--r--   0     1001      123     2892 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/frame/pivot.rs
+-rw-r--r--   0     1001      123      416 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/frame/python.rs
+-rw-r--r--   0     1001      123     6376 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/lib.rs
+-rw-r--r--   0     1001      123     1049 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs
+-rw-r--r--   0     1001      123      776 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs
+-rw-r--r--   0     1001      123      670 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs
+-rw-r--r--   0     1001      123     1284 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs
+-rw-r--r--   0     1001      123     3908 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs
+-rw-r--r--   0     1001      123     3577 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs
+-rw-r--r--   0     1001      123    13439 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs
+-rw-r--r--   0     1001      123     4335 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs
+-rw-r--r--   0     1001      123     6058 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs
+-rw-r--r--   0     1001      123     7074 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs
+-rw-r--r--   0     1001      123     2045 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs
+-rw-r--r--   0     1001      123     1677 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs
+-rw-r--r--   0     1001      123     2986 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs
+-rw-r--r--   0     1001      123     1963 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs
+-rw-r--r--   0     1001      123     4151 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs
+-rw-r--r--   0     1001      123     1208 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs
+-rw-r--r--   0     1001      123     2421 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs
+-rw-r--r--   0     1001      123      548 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs
+-rw-r--r--   0     1001      123     2197 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs
+-rw-r--r--   0     1001      123     1922 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs
+-rw-r--r--   0     1001      123      663 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs
+-rw-r--r--   0     1001      123     3702 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs
+-rw-r--r--   0     1001      123      838 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs
+-rw-r--r--   0     1001      123     1284 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/exotic.rs
+-rw-r--r--   0     1001      123    21873 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs
+-rw-r--r--   0     1001      123     2689 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs
+-rw-r--r--   0     1001      123    17432 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs
+-rw-r--r--   0     1001      123    17488 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs
+-rw-r--r--   0     1001      123     3153 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs
+-rw-r--r--   0     1001      123     6326 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs
+-rw-r--r--   0     1001      123     2003 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs
+-rw-r--r--   0     1001      123     5809 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs
+-rw-r--r--   0     1001      123     4131 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs
+-rw-r--r--   0     1001      123     5304 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs
+-rw-r--r--   0     1001      123    21103 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs
+-rw-r--r--   0     1001      123    10091 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs
+-rw-r--r--   0     1001      123     3929 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs
+-rw-r--r--   0     1001      123    11541 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs
+-rw-r--r--   0     1001      123     8331 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs
+-rw-r--r--   0     1001      123    14360 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs
+-rw-r--r--   0     1001      123    31819 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs
+-rw-r--r--   0     1001      123     2039 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs
+-rw-r--r--   0     1001      123      414 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/mod.rs
+-rw-r--r--   0     1001      123     2005 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs
+-rw-r--r--   0     1001      123    27366 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs
+-rw-r--r--   0     1001      123    18862 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs
+-rw-r--r--   0     1001      123       87 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/planner/mod.rs
+-rw-r--r--   0     1001      123     9425 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/state.rs
+-rw-r--r--   0     1001      123    20891 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/streaming/convert.rs
+-rw-r--r--   0     1001      123      219 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/streaming/mod.rs
+-rw-r--r--   0     1001      123     3333 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs
+-rw-r--r--   0     1001      123      722 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/prelude.rs
+-rw-r--r--   0     1001      123    14990 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/tests/aggregations.rs
+-rw-r--r--   0     1001      123     2339 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/tests/arity.rs
+-rw-r--r--   0     1001      123     7031 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/tests/cse.rs
+-rw-r--r--   0     1001      123    12749 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/tests/io.rs
+-rw-r--r--   0     1001      123     4207 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/tests/logical.rs
+-rw-r--r--   0     1001      123     4288 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/tests/mod.rs
+-rw-r--r--   0     1001      123    14812 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/tests/optimization_checks.rs
+-rw-r--r--   0     1001      123     6799 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/tests/predicate_queries.rs
+-rw-r--r--   0     1001      123     3158 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/tests/projection_queries.rs
+-rw-r--r--   0     1001      123    47910 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/tests/queries.rs
+-rw-r--r--   0     1001      123     8358 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/tests/streaming.rs
+-rw-r--r--   0     1001      123     2886 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/tests/tpch.rs
+-rw-r--r--   0     1001      123     1028 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/utils.rs
+-rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.7/local_dependencies/polars-algo/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-algo/LICENSE
+-rw-r--r--   0     1001      123     7265 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-algo/src/algo.rs
+-rw-r--r--   0     1001      123       88 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-algo/src/lib.rs
+-rw-r--r--   0     1001      123       28 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-algo/src/prelude.rs
+-rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.7/local_dependencies/polars-error/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-error/LICENSE
+-rw-r--r--   0     1001      123     6297 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-error/src/lib.rs
+-rw-r--r--   0        0        0     4341 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/LICENSE
+-rw-r--r--   0     1001      123     2383 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/avro/mod.rs
+-rw-r--r--   0     1001      123     3608 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/avro/read.rs
+-rw-r--r--   0     1001      123     2622 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/avro/write.rs
+-rw-r--r--   0     1001      123     4505 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/cloud/adaptors.rs
+-rw-r--r--   0     1001      123     9506 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/cloud/glob.rs
+-rw-r--r--   0     1001      123     3089 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/cloud/mod.rs
+-rw-r--r--   0     1001      123    28678 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/csv/buffer.rs
+-rw-r--r--   0     1001      123     1898 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/csv/mod.rs
+-rw-r--r--   0     1001      123    19712 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/csv/parser.rs
+-rw-r--r--   0     1001      123    21432 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/csv/read.rs
+-rw-r--r--   0     1001      123    10817 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs
+-rw-r--r--   0     1001      123    13909 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs
+-rw-r--r--   0     1001      123    31242 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/csv/read_impl/mod.rs
+-rw-r--r--   0     1001      123    11466 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/csv/splitfields.rs
+-rw-r--r--   0     1001      123    25183 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/csv/utils.rs
+-rw-r--r--   0     1001      123     2796 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/csv/write.rs
+-rw-r--r--   0     1001      123    13265 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/csv/write_impl.rs
+-rw-r--r--   0     1001      123      184 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/export.rs
+-rw-r--r--   0     1001      123     7586 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/ipc/ipc_file.rs
+-rw-r--r--   0     1001      123     9222 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/ipc/ipc_stream.rs
+-rw-r--r--   0     1001      123     3253 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/ipc/mmap.rs
+-rw-r--r--   0     1001      123      401 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/ipc/mod.rs
+-rw-r--r--   0     1001      123     8282 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/ipc/write.rs
+-rw-r--r--   0     1001      123     1471 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/ipc/write_async.rs
+-rw-r--r--   0     1001      123    11046 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/json.rs
+-rw-r--r--   0     1001      123     4864 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/lib.rs
+-rw-r--r--   0     1001      123     1969 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/mmap.rs
+-rw-r--r--   0     1001      123     7215 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/ndjson_core/buffer.rs
+-rw-r--r--   0     1001      123       39 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/ndjson_core/mod.rs
+-rw-r--r--   0     1001      123    12172 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/ndjson_core/ndjson.rs
+-rw-r--r--   0     1001      123      273 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/options.rs
+-rw-r--r--   0     1001      123     7360 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/parquet/async_impl.rs
+-rw-r--r--   0     1001      123     3093 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/parquet/mmap.rs
+-rw-r--r--   0     1001      123     3132 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/parquet/mod.rs
+-rw-r--r--   0     1001      123     4784 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/parquet/predicates.rs
+-rw-r--r--   0     1001      123     9606 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/parquet/read.rs
+-rw-r--r--   0     1001      123    16886 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/parquet/read_impl.rs
+-rw-r--r--   0     1001      123    10106 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/parquet/write.rs
+-rw-r--r--   0     1001      123     5334 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/partition.rs
+-rw-r--r--   0     1001      123     1455 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/predicates.rs
+-rw-r--r--   0     1001      123      628 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/prelude.rs
+-rw-r--r--   0     1001      123      417 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/tests.rs
+-rw-r--r--   0     1001      123     4467 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/local_dependencies/polars-io/src/utils.rs
+-rw-r--r--   0        0        0     4398 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.7/Cargo.toml
+-rw-r--r--   0     1001      123       76 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/.gitignore
+-rw-r--r--   0     1001      123     1055 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/LICENSE
+-rw-r--r--   0     1001      123     2414 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/Makefile
+-rw-r--r--   0     1001      123    12625 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/README.md
+-rw-r--r--   0     1001      123      651 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/build.rs
+-rw-r--r--   0     1001      123       32 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/.gitignore
+-rw-r--r--   0     1001      123      679 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/Makefile
+-rw-r--r--   0     1001      123      318 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/_templates/api_redirect.html
+-rw-r--r--   0     1001      123      151 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/_templates/autosummary/accessor.rst
+-rw-r--r--   0     1001      123      160 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/_templates/autosummary/accessor_attribute.rst
+-rw-r--r--   0     1001      123      168 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/_templates/autosummary/accessor_callable.rst
+-rw-r--r--   0     1001      123      157 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/_templates/autosummary/accessor_method.rst
+-rw-r--r--   0     1001      123      836 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/_templates/autosummary/class.rst
+-rw-r--r--   0     1001      123       94 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/_templates/autosummary/class_without_autosummary.rst
+-rw-r--r--   0     1001      123      406 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/_templates/sidebar-nav-bs.html
+-rw-r--r--   0     1001      123      450 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/requirements-docs.txt
+-rw-r--r--   0     1001      123     1567 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/_static/css/custom.css
+-rw-r--r--   0     1001      123     7302 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/conf.py
+-rw-r--r--   0     1001      123       51 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/index.rst
+-rw-r--r--   0     1001      123     6767 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/api.rst
+-rw-r--r--   0     1001      123     1694 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/config.rst
+-rw-r--r--   0     1001      123      274 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/dataframe/aggregation.rst
+-rw-r--r--   0     1001      123      221 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/dataframe/attributes.rst
+-rw-r--r--   0     1001      123      142 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/dataframe/computation.rst
+-rw-r--r--   0     1001      123      319 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/dataframe/descriptive.rst
+-rw-r--r--   0     1001      123      319 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/dataframe/export.rst
+-rw-r--r--   0     1001      123      464 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/dataframe/groupby.rst
+-rw-r--r--   0     1001      123      379 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/dataframe/index.rst
+-rw-r--r--   0     1001      123      189 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/dataframe/miscellaneous.rst
+-rw-r--r--   0     1001      123     1513 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/dataframe/modify_select.rst
+-rw-r--r--   0     1001      123      663 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/datatypes.rst
+-rw-r--r--   0     1001      123      421 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/exceptions.rst
+-rw-r--r--   0     1001      123      391 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/expressions/aggregation.rst
+-rw-r--r--   0     1001      123      309 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/expressions/binary.rst
+-rw-r--r--   0     1001      123      338 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/expressions/boolean.rst
+-rw-r--r--   0     1001      123      237 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/expressions/categories.rst
+-rw-r--r--   0     1001      123      221 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/expressions/columns.rst
+-rw-r--r--   0     1001      123     1061 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/expressions/computation.rst
+-rw-r--r--   0     1001      123     1114 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/expressions/functions.rst
+-rw-r--r--   0     1001      123      461 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/expressions/index.rst
+-rw-r--r--   0     1001      123      695 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/expressions/list.rst
+-rw-r--r--   0     1001      123      374 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/expressions/meta.rst
+-rw-r--r--   0     1001      123      125 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/expressions/miscellaneous.rst
+-rw-r--r--   0     1001      123      977 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/expressions/modify_select.rst
+-rw-r--r--   0     1001      123      639 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/expressions/operators.rst
+-rw-r--r--   0     1001      123      860 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/expressions/string.rst
+-rw-r--r--   0     1001      123      254 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/expressions/struct.rst
+-rw-r--r--   0     1001      123      968 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/expressions/temporal.rst
+-rw-r--r--   0     1001      123       98 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/expressions/window.rst
+-rw-r--r--   0     1001      123      692 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/functions.rst
+-rw-r--r--   0     1001      123      392 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/index.rst
+-rw-r--r--   0     1001      123     1269 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/io.rst
+-rw-r--r--   0     1001      123      252 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/lazyframe/aggregation.rst
+-rw-r--r--   0     1001      123      179 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/lazyframe/attributes.rst
+-rw-r--r--   0     1001      123      146 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/lazyframe/descriptive.rst
+-rw-r--r--   0     1001      123      497 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/lazyframe/groupby.rst
+-rw-r--r--   0     1001      123      354 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/lazyframe/index.rst
+-rw-r--r--   0     1001      123      455 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/lazyframe/miscellaneous.rst
+-rw-r--r--   0     1001      123      988 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/lazyframe/modify_select.rst
+-rw-r--r--   0     1001      123      358 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/series/aggregation.rst
+-rw-r--r--   0     1001      123      256 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/series/attributes.rst
+-rw-r--r--   0     1001      123      321 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/series/binary.rst
+-rw-r--r--   0     1001      123      117 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/series/boolean.rst
+-rw-r--r--   0     1001      123      241 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/series/categories.rst
+-rw-r--r--   0     1001      123     1103 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/series/computation.rst
+-rw-r--r--   0     1001      123      744 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/series/descriptive.rst
+-rw-r--r--   0     1001      123      240 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/series/export.rst
+-rw-r--r--   0     1001      123      428 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/series/index.rst
+-rw-r--r--   0     1001      123      749 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/series/list.rst
+-rw-r--r--   0     1001      123      236 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/series/miscellaneous.rst
+-rw-r--r--   0     1001      123     1077 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/series/modify_select.rst
+-rw-r--r--   0     1001      123      922 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/series/string.rst
+-rw-r--r--   0     1001      123      396 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/series/struct.rst
+-rw-r--r--   0     1001      123     1118 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/series/temporal.rst
+-rw-r--r--   0     1001      123      302 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/sql.rst
+-rw-r--r--   0     1001      123      647 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/testing.rst
+-rw-r--r--   0     1001      123      168 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/docs/source/reference/utils.rst
+-rw-r--r--   0     1001      123     6335 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/__init__.py
+-rw-r--r--   0     1001      123    13396 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/api.py
+-rw-r--r--   0     1001      123    25956 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/config.py
+-rw-r--r--   0     1001      123    27169 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/convert.py
+-rw-r--r--   0     1001      123       77 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/dataframe/__init__.py
+-rw-r--r--   0     1001      123     5057 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/dataframe/_html.py
+-rw-r--r--   0     1001      123   304087 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/dataframe/frame.py
+-rw-r--r--   0     1001      123    33240 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/dataframe/groupby.py
+-rw-r--r--   0     1001      123     2628 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/datatypes/__init__.py
+-rw-r--r--   0     1001      123    11397 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/datatypes/classes.py
+-rw-r--r--   0     1001      123     1577 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/datatypes/constants.py
+-rw-r--r--   0     1001      123     4430 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/datatypes/constructor.py
+-rw-r--r--   0     1001      123    15109 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/datatypes/convert.py
+-rw-r--r--   0     1001      123     7338 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/dependencies.py
+-rw-r--r--   0     1001      123     3436 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/exceptions.py
+-rw-r--r--   0     1001      123       61 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/expr/__init__.py
+-rw-r--r--   0     1001      123     2730 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/expr/binary.py
+-rw-r--r--   0     1001      123     1708 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/expr/categorical.py
+-rw-r--r--   0     1001      123    69359 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/expr/datetime.py
+-rw-r--r--   0     1001      123   250779 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/expr/expr.py
+-rw-r--r--   0     1001      123    22899 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/expr/list.py
+-rw-r--r--   0     1001      123     2059 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/expr/meta.py
+-rw-r--r--   0     1001      123    44737 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/expr/string.py
+-rw-r--r--   0     1001      123     5436 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/expr/struct.py
+-rw-r--r--   0     1001      123     1981 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/functions/__init__.py
+-rw-r--r--   0     1001      123    29688 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/functions/eager.py
+-rw-r--r--   0     1001      123    90827 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/functions/lazy.py
+-rw-r--r--   0     1001      123     6293 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/functions/whenthen.py
+-rw-r--r--   0     1001      123      280 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/internals.py
+-rw-r--r--   0     1001      123      978 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/io/__init__.py
+-rw-r--r--   0     1001      123     6264 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/io/_utils.py
+-rw-r--r--   0     1001      123      878 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/io/avro.py
+-rw-r--r--   0     1001      123      144 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/io/csv/__init__.py
+-rw-r--r--   0     1001      123     1082 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/io/csv/_utils.py
+-rw-r--r--   0     1001      123     4691 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/io/csv/batched_reader.py
+-rw-r--r--   0     1001      123    35533 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/io/csv/functions.py
+-rw-r--r--   0     1001      123     8655 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/io/database.py
+-rw-r--r--   0     1001      123    10988 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/io/delta.py
+-rw-r--r--   0     1001      123       75 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/io/excel/__init__.py
+-rw-r--r--   0     1001      123    18459 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/io/excel/_write_utils.py
+-rw-r--r--   0     1001      123     6476 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/io/excel/functions.py
+-rw-r--r--   0     1001      123      142 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/io/ipc/__init__.py
+-rw-r--r--   0     1001      123     1271 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/io/ipc/anonymous_scan.py
+-rw-r--r--   0     1001      123     5840 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/io/ipc/functions.py
+-rw-r--r--   0     1001      123      519 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/io/json.py
+-rw-r--r--   0     1001      123     2257 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/io/ndjson.py
+-rw-r--r--   0     1001      123      170 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/io/parquet/__init__.py
+-rw-r--r--   0     1001      123     1299 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/io/parquet/anonymous_scan.py
+-rw-r--r--   0     1001      123     7212 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/io/parquet/functions.py
+-rw-r--r--   0     1001      123      136 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/io/pyarrow_dataset/__init__.py
+-rw-r--r--   0     1001      123     2331 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/io/pyarrow_dataset/anonymous_scan.py
+-rw-r--r--   0     1001      123     3611 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/io/pyarrow_dataset/functions.py
+-rw-r--r--   0     1001      123       77 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/lazyframe/__init__.py
+-rw-r--r--   0     1001      123   166798 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/lazyframe/frame.py
+-rw-r--r--   0     1001      123    24178 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/lazyframe/groupby.py
+-rw-r--r--   0     1001      123        0 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/py.typed
+-rw-r--r--   0     1001      123       69 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/series/__init__.py
+-rw-r--r--   0     1001      123     1579 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/series/_numpy.py
+-rw-r--r--   0     1001      123     1920 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/series/binary.py
+-rw-r--r--   0     1001      123     1699 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/series/categorical.py
+-rw-r--r--   0     1001      123    47526 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/series/datetime.py
+-rw-r--r--   0     1001      123    12385 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/series/list.py
+-rw-r--r--   0     1001      123   164038 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/series/series.py
+-rw-r--r--   0     1001      123    27401 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/series/string.py
+-rw-r--r--   0     1001      123     2287 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/series/struct.py
+-rw-r--r--   0     1001      123     5375 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/series/utils.py
+-rw-r--r--   0     1001      123     7638 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/slice.py
+-rw-r--r--   0     1001      123       75 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/sql/__init__.py
+-rw-r--r--   0     1001      123     1351 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/sql/context.py
+-rw-r--r--   0     1001      123     4764 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/string_cache.py
+-rw-r--r--   0     1001      123      362 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/testing/__init__.py
+-rw-r--r--   0     1001      123      929 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/testing/_private.py
+-rw-r--r--   0     1001      123     3689 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/testing/_tempdir.py
+-rw-r--r--   0     1001      123    13597 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/testing/asserts.py
+-rw-r--r--   0     1001      123      684 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/testing/parametric/__init__.py
+-rw-r--r--   0     1001      123    25067 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/testing/parametric/primitives.py
+-rw-r--r--   0     1001      123     7359 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/testing/parametric/strategies.py
+-rw-r--r--   0     1001      123     5681 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/type_aliases.py
+-rw-r--r--   0     1001      123     1211 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/utils/__init__.py
+-rw-r--r--   0     1001      123    50687 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/utils/_construction.py
+-rw-r--r--   0     1001      123     2782 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/utils/_parse_expr_input.py
+-rw-r--r--   0     1001      123      721 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/utils/_scan.py
+-rw-r--r--   0     1001      123      687 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/utils/_wrap.py
+-rw-r--r--   0     1001      123      683 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/utils/build_info.py
+-rw-r--r--   0     1001      123     8812 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/utils/convert.py
+-rw-r--r--   0     1001      123     5789 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/utils/decorators.py
+-rw-r--r--   0     1001      123     1660 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/utils/meta.py
+-rw-r--r--   0     1001      123      514 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/utils/polars_version.py
+-rw-r--r--   0     1001      123     2339 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/utils/show_versions.py
+-rw-r--r--   0     1001      123    11592 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/polars/utils/various.py
+-rw-r--r--   0     1001      123     5378 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/pyproject.toml
+-rw-r--r--   0     1001      123      699 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/requirements-dev.txt
+-rw-r--r--   0     1001      123       70 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/requirements-lint.txt
+-rw-r--r--   0     1001      123     1640 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/scripts/check_stacklevels.py
+-rw-r--r--   0     1001      123    11023 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/src/apply/dataframe.rs
+-rw-r--r--   0     1001      123     8388 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/src/apply/mod.rs
+-rw-r--r--   0     1001      123    71480 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/src/apply/series.rs
+-rw-r--r--   0     1001      123       32 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/src/arrow_interop/mod.rs
+-rw-r--r--   0     1001      123     1306 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/src/arrow_interop/to_py.rs
+-rw-r--r--   0     1001      123     3902 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/src/arrow_interop/to_rust.rs
+-rw-r--r--   0     1001      123     5250 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/src/batched_csv.rs
+-rw-r--r--   0     1001      123    46606 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/src/conversion.rs
+-rw-r--r--   0     1001      123    45472 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/src/dataframe.rs
+-rw-r--r--   0     1001      123     3799 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/src/datatypes.rs
+-rw-r--r--   0     1001      123     3288 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/src/error.rs
+-rw-r--r--   0     1001      123     9482 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/src/file.rs
+-rw-r--r--   0     1001      123     7468 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/src/lazy/apply.rs
+-rw-r--r--   0     1001      123    33439 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/src/lazy/dataframe.rs
+-rw-r--r--   0     1001      123    62419 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/src/lazy/dsl.rs
+-rw-r--r--   0     1001      123     1082 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/src/lazy/meta.rs
+-rw-r--r--   0     1001      123      727 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/src/lazy/mod.rs
+-rw-r--r--   0     1001      123      212 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/src/lazy/utils.rs
+-rw-r--r--   0     1001      123    20992 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/src/lib.rs
+-rw-r--r--   0     1001      123     8642 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/src/npy.rs
+-rw-r--r--   0     1001      123     1029 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/src/object.rs
+-rw-r--r--   0     1001      123      122 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/src/prelude.rs
+-rw-r--r--   0     1001      123      435 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/src/py_modules.rs
+-rw-r--r--   0     1001      123    54535 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/src/series.rs
+-rw-r--r--   0     1001      123     3478 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/src/set.rs
+-rw-r--r--   0     1001      123      843 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/src/sql.rs
+-rw-r--r--   0     1001      123     2335 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/src/utils.rs
+-rw-r--r--   0     1001      123     6165 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/README.md
+-rw-r--r--   0     1001      123     2189 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/benchmark/groupby-datagen.R
+-rw-r--r--   0     1001      123     7945 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/benchmark/run_h2oai_benchmark.py
+-rw-r--r--   0     1001      123     6530 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/benchmark/test_release.py
+-rw-r--r--   0     1001      123     4589 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/docs/run_doctest.py
+-rw-r--r--   0     1001      123     1633 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/parametric/conftest.py
+-rw-r--r--   0     1001      123     3823 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/parametric/test_dataframe.py
+-rw-r--r--   0     1001      123     1692 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/parametric/test_lazyframe.py
+-rw-r--r--   0     1001      123     6863 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/parametric/test_series.py
+-rw-r--r--   0     1001      123     8299 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/parametric/test_testing.py
+-rw-r--r--   0     1001      123        0 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/__init__.py
+-rw-r--r--   0     1001      123     3382 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/conftest.py
+-rw-r--r--   0     1001      123       86 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/datatypes/__init__.py
+-rw-r--r--   0     1001      123      351 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/datatypes/test_binary.py
+-rw-r--r--   0     1001      123     1420 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/datatypes/test_bool.py
+-rw-r--r--   0     1001      123    12662 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/datatypes/test_categorical.py
+-rw-r--r--   0     1001      123     2766 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/datatypes/test_decimal.py
+-rw-r--r--   0     1001      123      280 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/datatypes/test_duration.py
+-rw-r--r--   0     1001      123    16033 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/datatypes/test_list.py
+-rw-r--r--   0     1001      123      284 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/datatypes/test_null.py
+-rw-r--r--   0     1001      123     2801 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/datatypes/test_object.py
+-rw-r--r--   0     1001      123    29644 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/datatypes/test_struct.py
+-rw-r--r--   0     1001      123    91606 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/datatypes/test_temporal.py
+-rw-r--r--   0     1001      123      418 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/datatypes/test_time.py
+-rw-r--r--   0     1001      123      218 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/conftest.py
+-rw-r--r--   0     1001      123       16 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/files/delta-table/.part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       16 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/files/delta-table/.part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       16 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/files/delta-table/_delta_log/.00000000000000000000.json.crc
+-rw-r--r--   0     1001      123       16 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/files/delta-table/_delta_log/.00000000000000000001.json.crc
+-rw-r--r--   0     1001      123      905 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json
+-rw-r--r--   0     1001      123      936 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json
+-rw-r--r--   0     1001      123      972 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet
+-rw-r--r--   0     1001      123      690 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet
+-rw-r--r--   0     1001      123        0 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/files/empty.csv
+-rw-r--r--   0     1001      123     5959 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/files/example.xlsx
+-rw-r--r--   0     1001      123      457 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/files/foods1.csv
+-rw-r--r--   0     1001      123     2351 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/files/foods1.ipc
+-rw-r--r--   0     1001      123     1713 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/files/foods1.ndjson
+-rw-r--r--   0     1001      123     1427 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/files/foods1.parquet
+-rw-r--r--   0     1001      123      455 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/files/foods2.csv
+-rw-r--r--   0     1001      123     2351 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/files/foods2.ipc
+-rw-r--r--   0     1001      123     1711 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/files/foods2.ndjson
+-rw-r--r--   0     1001      123     1916 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/files/foods2.parquet
+-rw-r--r--   0     1001      123      455 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/files/foods3.csv
+-rw-r--r--   0     1001      123      457 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/files/foods4.csv
+-rw-r--r--   0     1001      123      452 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/files/foods5.csv
+-rw-r--r--   0     1001      123       49 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/files/gzipped.csv
+-rw-r--r--   0     1001      123       57 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/files/small.csv
+-rw-r--r--   0     1001      123      756 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/files/small.parquet
+-rw-r--r--   0     1001      123     1937 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/test_avro.py
+-rw-r--r--   0     1001      123    39498 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/test_csv.py
+-rw-r--r--   0     1001      123     6360 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/test_database.py
+-rw-r--r--   0     1001      123     3456 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/test_delta.py
+-rw-r--r--   0     1001      123    11169 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/test_excel.py
+-rw-r--r--   0     1001      123     5919 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/test_ipc.py
+-rw-r--r--   0     1001      123     3720 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/test_json.py
+-rw-r--r--   0     1001      123     6849 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/test_lazy_csv.py
+-rw-r--r--   0     1001      123     2060 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/test_lazy_ipc.py
+-rw-r--r--   0     1001      123     2881 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/test_lazy_json.py
+-rw-r--r--   0     1001      123    11849 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/test_lazy_parquet.py
+-rw-r--r--   0     1001      123     2012 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/test_other.py
+-rw-r--r--   0     1001      123    13735 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/test_parquet.py
+-rw-r--r--   0     1001      123      612 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/test_pickle.py
+-rw-r--r--   0     1001      123     3259 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/io/test_pyarrow_dataset.py
+-rw-r--r--   0     1001      123      509 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/namespaces/__init__.py
+-rw-r--r--   0     1001      123     3218 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/namespaces/test_binary.py
+-rw-r--r--   0     1001      123     2489 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/namespaces/test_categorical.py
+-rw-r--r--   0     1001      123    15436 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/namespaces/test_datetime.py
+-rw-r--r--   0     1001      123    12750 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/namespaces/test_list.py
+-rw-r--r--   0     1001      123     1748 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/namespaces/test_meta.py
+-rw-r--r--   0     1001      123    23698 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/namespaces/test_string.py
+-rw-r--r--   0     1001      123    16930 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/namespaces/test_strptime.py
+-rw-r--r--   0     1001      123      982 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/namespaces/test_struct.py
+-rw-r--r--   0     1001      123       85 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/operations/__init__.py
+-rw-r--r--   0     1001      123     6238 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/operations/test_aggregations.py
+-rw-r--r--   0     1001      123     9412 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/operations/test_apply.py
+-rw-r--r--   0     1001      123     4390 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/operations/test_arithmetic.py
+-rw-r--r--   0     1001      123      956 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/operations/test_comparison.py
+-rw-r--r--   0     1001      123     2906 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/operations/test_drop.py
+-rw-r--r--   0     1001      123     8252 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/operations/test_explode.py
+-rw-r--r--   0     1001      123     3664 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/operations/test_filter.py
+-rw-r--r--   0     1001      123     1801 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/operations/test_folds.py
+-rw-r--r--   0     1001      123    22696 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/operations/test_groupby.py
+-rw-r--r--   0     1001      123     2959 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/operations/test_is_in.py
+-rw-r--r--   0     1001      123    16937 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/operations/test_join.py
+-rw-r--r--   0     1001      123    10467 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/operations/test_join_asof.py
+-rw-r--r--   0     1001      123      643 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/operations/test_melt.py
+-rw-r--r--   0     1001      123    10253 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/operations/test_pivot.py
+-rw-r--r--   0     1001      123    18639 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/operations/test_rolling.py
+-rw-r--r--   0     1001      123    19550 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/operations/test_sort.py
+-rw-r--r--   0     1001      123     3643 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/operations/test_statistics.py
+-rw-r--r--   0     1001      123     3631 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/operations/test_transpose.py
+-rw-r--r--   0     1001      123      771 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/operations/test_unique.py
+-rw-r--r--   0     1001      123     9814 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/operations/test_window.py
+-rw-r--r--   0     1001      123     4775 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/test_api.py
+-rw-r--r--   0     1001      123     1077 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/test_arity.py
+-rw-r--r--   0     1001      123    19856 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/test_cfg.py
+-rw-r--r--   0     1001      123    39286 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/test_constructors.py
+-rw-r--r--   0     1001      123      454 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/test_context.py
+-rw-r--r--   0     1001      123     1628 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/test_cse.py
+-rw-r--r--   0     1001      123     3497 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/test_datatypes.py
+-rw-r--r--   0     1001      123   120890 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/test_df.py
+-rw-r--r--   0     1001      123     1196 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/test_empty.py
+-rw-r--r--   0     1001      123    16867 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/test_errors.py
+-rw-r--r--   0     1001      123     2387 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/test_expr_multi_cols.py
+-rw-r--r--   0     1001      123    32643 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/test_exprs.py
+-rw-r--r--   0     1001      123     3305 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/test_fmt.py
+-rw-r--r--   0     1001      123    11420 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/test_functions.py
+-rw-r--r--   0     1001      123     3763 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/test_interchange.py
+-rw-r--r--   0     1001      123    33952 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/test_interop.py
+-rw-r--r--   0     1001      123    49534 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/test_lazy.py
+-rw-r--r--   0     1001      123     2369 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/test_polars_import.py
+-rw-r--r--   0     1001      123     4014 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/test_predicates.py
+-rw-r--r--   0     1001      123     6995 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/test_projections.py
+-rw-r--r--   0     1001      123    11550 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/test_queries.py
+-rw-r--r--   0     1001      123     4743 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/test_rows.py
+-rw-r--r--   0     1001      123    13181 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/test_schema.py
+-rw-r--r--   0     1001      123     2634 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/test_serde.py
+-rw-r--r--   0     1001      123    83663 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/test_series.py
+-rw-r--r--   0     1001      123     2561 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/test_sql.py
+-rw-r--r--   0     1001      123    13877 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/test_streaming.py
+-rw-r--r--   0     1001      123    10700 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/test_testing.py
+-rw-r--r--   0     1001      123       41 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/utils/__init__.py
+-rw-r--r--   0     1001      123      306 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/utils/test_build_info.py
+-rw-r--r--   0     1001      123      247 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/utils/test_show_versions.py
+-rw-r--r--   0     1001      123     4307 2023-04-22 20:09:11.000000 polars_u64_idx-0.17.7/tests/unit/utils/test_utils.py
+-rw-r--r--   0     1001      123    66145 2023-04-22 20:10:14.000000 polars_u64_idx-0.17.7/Cargo.lock
+-rw-r--r--   0        0        0    15163 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.7/PKG-INFO
```

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/Cargo.toml` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/LICENSE` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/operators/filter.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/operators/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/operators/function.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/operators/function.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/operators/projection.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/operators/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/operators/reproject.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/operators/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/io.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/io.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/memory.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/memory.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/slice.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/utils.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sources/csv.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sources/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sources/frame.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sources/frame.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sources/parquet.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sources/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sources/reproject.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sources/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/executors/sources/union.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/executors/sources/union.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/operators/chunks.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/operators/chunks.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/operators/sink.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/operators/sink.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/pipeline/convert.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/pipeline/convert.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-pipe/src/pipeline/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-pipe/src/pipeline/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/Cargo.toml` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/LICENSE` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/src/chunkedarray/date.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/src/chunkedarray/date.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/src/chunkedarray/datetime.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/src/chunkedarray/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/src/chunkedarray/duration.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/src/chunkedarray/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/src/chunkedarray/kernels.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/src/chunkedarray/kernels.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/src/chunkedarray/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/src/chunkedarray/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/src/chunkedarray/time.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/src/chunkedarray/time.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/src/date_range.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/src/date_range.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/src/groupby/dynamic.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/src/groupby/dynamic.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/src/lib.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/src/round.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/src/round.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/src/series/_trait.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/src/series/_trait.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/src/series/implementations/floats.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/src/series/implementations/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/src/series/implementations/integers.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/src/series/implementations/integers.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/src/series/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/src/series/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/src/truncate.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/src/truncate.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/src/upsample.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/src/upsample.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/src/utils.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/src/windows/bounds.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/src/windows/bounds.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/src/windows/calendar.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/src/windows/calendar.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/src/windows/duration.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/src/windows/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/src/windows/groupby.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/src/windows/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/src/windows/test.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/src/windows/test.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-time/src/windows/window.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/src/windows/window.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-utils/LICENSE` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/arena.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/arena.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/atomic.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/atomic.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/cell.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/cell.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/contention_pool.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/contention_pool.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/functions.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/hash.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/hash.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/iter/enumerate_idx.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/iter/enumerate_idx.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/lib.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/macros.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/macros.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/slice.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/sort.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/sync.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/sync.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/unwrap.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/unwrap.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-utils/src/wasm.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-utils/src/wasm.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-error/Cargo.toml` & `polars_u64_idx-0.17.7/local_dependencies/polars-error/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-error/LICENSE` & `polars_u64_idx-0.17.7/local_dependencies/polars-time/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-error/src/lib.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-error/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-sql/Cargo.toml` & `polars_u64_idx-0.17.7/local_dependencies/polars-sql/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-sql/LICENSE` & `polars_u64_idx-0.17.7/local_dependencies/polars-utils/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-sql/src/context.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-sql/src/context.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-sql/src/functions.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-sql/src/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-sql/src/keywords.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-sql/src/keywords.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-sql/src/lib.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-sql/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-sql/src/sql_expr.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-sql/src/sql_expr.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-sql/src/table_functions.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-sql/src/table_functions.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/Cargo.toml` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/LICENSE` & `polars_u64_idx-0.17.7/local_dependencies/polars/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/array/default_arrays.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/array/default_arrays.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/array/get.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/array/get.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/array/list.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/array/list.rs`

 * *Files 3% similar despite different names*

```diff
@@ -93,16 +93,24 @@
 
     pub fn finish(self, inner_dtype: Option<&DataType>) -> Result<ListArray<i64>> {
         // Safety:
         // offsets are monotonically increasing
         let offsets = unsafe { Offsets::new_unchecked(self.offsets) };
         let (inner_dtype, values) = if self.arrays.is_empty() {
             let len = *offsets.last() as usize;
-            let values = NullArray::new(DataType::Null, len).boxed();
-            (DataType::Null, values)
+            match inner_dtype {
+                None => {
+                    let values = NullArray::new(DataType::Null, len).boxed();
+                    (DataType::Null, values)
+                }
+                Some(inner_dtype) => {
+                    let values = new_null_array(inner_dtype.clone(), len);
+                    (inner_dtype.clone(), values)
+                }
+            }
         } else {
             let inner_dtype = inner_dtype.unwrap_or_else(|| self.arrays[0].data_type());
 
             // check if there is a dtype that is not `Null`
             // if we find it, we will convert the null arrays
             // to empty arrays of this dtype, otherwise the concat kernel fails.
             let mut non_null_dtype = None;
```

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/array/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/array/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/array/null.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/array/null.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/array/slice.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/array/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/array/utf8.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/array/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/bit_util.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/bit_util.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/bitmap/mutable.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/bitmap/mutable.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/compute/take/boolean.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/compute/take/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/compute/take/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/compute/take/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/conversion.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/data_types.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/data_types.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/floats/ord.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/floats/ord.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/index.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/index.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/is_valid.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/is_valid.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/agg_mean.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/agg_mean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/concatenate.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/concatenate.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/ewm/average.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/ewm/average.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/float.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/float.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/list.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/window.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/window.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/set.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/set.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/sort_partition.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/sort_partition.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/string.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/string.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/kernels/time.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/kernels/time.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/slice.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/time_zone.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/time_zone.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/trusted_len/boolean.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/trusted_len/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/trusted_len/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/trusted_len/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-arrow/src/utils.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/Cargo.toml` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/LICENSE` & `polars_u64_idx-0.17.7/local_dependencies/polars-row/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/avro/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/avro/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/avro/read.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/avro/read.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/avro/write.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/avro/write.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/cloud/adaptors.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/cloud/adaptors.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/cloud/glob.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/cloud/glob.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/cloud/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/cloud/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/csv/buffer.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/csv/buffer.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/csv/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/csv/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/csv/parser.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/csv/parser.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/csv/read.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/csv/read.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/csv/read_impl/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/csv/read_impl/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/csv/splitfields.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/csv/splitfields.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/csv/utils.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/csv/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/csv/write.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/csv/write.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/csv/write_impl.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/csv/write_impl.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/ipc/ipc_file.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/ipc/ipc_file.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/ipc/ipc_stream.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/ipc/ipc_stream.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/ipc/mmap.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/ipc/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/ipc/write.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/ipc/write.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/ipc/write_async.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/ipc/write_async.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/json.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/json.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/lib.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/mmap.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/ndjson_core/buffer.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/ndjson_core/buffer.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/ndjson_core/ndjson.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/ndjson_core/ndjson.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/parquet/async_impl.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/parquet/async_impl.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/parquet/mmap.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/parquet/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/parquet/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/parquet/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/parquet/predicates.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/parquet/predicates.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/parquet/read.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/parquet/read.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/parquet/read_impl.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/parquet/read_impl.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/parquet/write.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/parquet/write.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/partition.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/partition.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/predicates.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/predicates.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/prelude.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-io/src/utils.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-algo/Cargo.toml` & `polars_u64_idx-0.17.7/local_dependencies/polars-algo/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-algo/LICENSE` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-algo/src/algo.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-algo/src/algo.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/Cargo.toml` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 
 parquet = ["arrow/io_parquet"]
 
 # scale to terabytes?
 bigidx = ["polars-arrow/bigidx"]
 python = []
 
+serde = ["dep:serde", "smartstring/serde"]
 serde-lazy = ["serde", "polars-arrow/serde", "indexmap/serde", "smartstring/serde", "chrono/serde"]
 
 docs-selection = [
   "ndarray",
   "is_in",
   "rows",
   "docs",
```

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/LICENSE` & `polars_u64_idx-0.17.7/local_dependencies/polars-arrow/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/arithmetic.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/bitwise.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/bitwise.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/builder/binary.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/builder/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/builder/from.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/builder/from.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/builder/list.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/builder/list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/builder/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/builder/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/cast.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/cast.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/drop.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/float.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/float.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/from.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/from.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/kernels/take.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/kernels/take.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/list/iterator.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/list/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/list/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/list/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/date.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/date.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/duration.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/time.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/time.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ndarray.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ndarray.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/object/builder.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/object/builder.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/object/iterator.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/object/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/object/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/object/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/object/registry.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/object/registry.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/append.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/append.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/apply.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/explode.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/explode.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/extend.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/extend.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/filter.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/full.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/full.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/set.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/set.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/shift.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/shift.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/zip.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/zip.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/random.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/random.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/temporal/date.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/temporal/date.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/temporal/time.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/temporal/time.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/to_vec.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/to_vec.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/trusted_len.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/trusted_len.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/cloud.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/cloud.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/config.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/config.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/datatypes/_serde.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/datatypes/_serde.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/datatypes/aliases.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/datatypes/aliases.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/datatypes/any_value.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/datatypes/any_value.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/datatypes/dtype.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/datatypes/dtype.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/datatypes/field.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/datatypes/field.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 use smartstring::alias::String as SmartString;
 
 use super::*;
 
 /// Characterizes the name and the [`DataType`] of a column.
 #[derive(Clone, Debug, PartialEq, Eq)]
-#[cfg_attr(feature = "serde-lazy", derive(Serialize, Deserialize))]
+#[cfg_attr(
+    any(feature = "serde", feature = "serde-lazy"),
+    derive(Serialize, Deserialize)
+)]
 pub struct Field {
     pub name: SmartString,
     pub dtype: DataType,
 }
 
 impl Field {
     /// Creates a new `Field`.
```

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/datatypes/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/datatypes/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/datatypes/time_unit.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/datatypes/time_unit.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/doc/changelog/v0_7.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/doc/changelog/v0_7.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/doc/changelog/v0_8.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/doc/changelog/v0_8.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/doc/changelog/v0_9.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/doc/changelog/v0_9.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/fmt.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/fmt.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/arithmetic.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/asof_join/asof.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/asof_join/asof.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/asof_join/groups.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/asof_join/groups.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/asof_join/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/asof_join/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/chunks.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/chunks.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/cross_join.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/cross_join.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/explode.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/explode.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/from.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/from.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/groupby/hashing.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/groupby/hashing.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/groupby/into_groups.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/groupby/into_groups.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/groupby/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/groupby/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -257,15 +257,15 @@
 
         POOL.install(|| {
             self.selected_keys
                 .par_iter()
                 .map(|s| {
                     match groups {
                         GroupsProxy::Idx(groups) => {
-                            let mut iter = groups.iter().map(|(first, _idx)| first as usize);
+                            let mut iter = groups.first().iter().map(|first| *first as usize);
                             // Safety:
                             // groups are always in bounds
                             let mut out = unsafe { s.take_iter_unchecked(&mut iter) };
                             if groups.sorted {
                                 out.set_sorted_flag(s.is_sorted_flag());
                             };
                             out
```

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/groupby/proxy.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/groupby/proxy.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/hash_join/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/hash_join/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/row/av_buffer.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/row/av_buffer.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/row/dataframe.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/row/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/row/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/row/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/row/transpose.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/row/transpose.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/top_k.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/top_k.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/frame/upstream_traits.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/frame/upstream_traits.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/functions.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/hashing/fx.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/hashing/fx.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/hashing/identity.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/hashing/identity.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/hashing/partition.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/hashing/partition.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/hashing/vector_hasher.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/hashing/vector_hasher.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/lib.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/named_from.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/named_from.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/prelude.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/schema.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/serde/chunked_array.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/serde/chunked_array.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/serde/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/serde/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/serde/series.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/serde/series.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/any_value.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/any_value.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/arithmetic/owned.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/arithmetic/owned.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/comparison.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/comparison.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/from.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/from.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/implementations/binary.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/implementations/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/implementations/boolean.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/implementations/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/implementations/categorical.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/implementations/categorical.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/implementations/dates_time.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/implementations/dates_time.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/implementations/datetime.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/implementations/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/implementations/decimal.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/implementations/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/implementations/duration.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/implementations/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/implementations/floats.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/implementations/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/implementations/list.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/implementations/list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/implementations/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/implementations/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/implementations/null.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/implementations/null.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/implementations/object.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/implementations/object.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/implementations/struct_.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/implementations/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/implementations/utf8.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/implementations/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/into.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/into.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/iterator.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/ops/diff.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/ops/diff.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/ops/downcast.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/ops/downcast.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/ops/ewm.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/ops/ewm.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/ops/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/ops/moment.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/ops/moment.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/ops/null.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/ops/null.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/ops/pct_change.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/ops/pct_change.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/ops/round.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/ops/round.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/ops/to_list.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/ops/to_list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/ops/unique.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/ops/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/series_trait.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/series_trait.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/series/unstable.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/series/unstable.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/testing.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/testing.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/utils/flatten.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/utils/flatten.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/utils/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/utils/series.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/utils/series.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-core/src/utils/supertype.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-core/src/utils/supertype.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-row/Cargo.toml` & `polars_u64_idx-0.17.7/local_dependencies/polars-row/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-row/LICENSE` & `polars_u64_idx-0.17.7/local_dependencies/polars-sql/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-row/src/encode.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-row/src/encode.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-row/src/encodings/fixed.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-row/src/encodings/fixed.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-row/src/encodings/variable.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-row/src/encodings/variable.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-row/src/lib.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-row/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-row/src/row.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-row/src/row.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-row/src/utils.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-row/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/Cargo.toml` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/LICENSE` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/dot.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/dot.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/dsl/eval.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/dsl/eval.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/dsl/functions.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/dsl/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/dsl/list.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/dsl/list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/dsl/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/dsl/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/frame/csv.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/frame/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/frame/file_list_reader.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/frame/file_list_reader.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/frame/ipc.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/frame/ipc.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/frame/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/frame/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/frame/ndjson.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/frame/ndjson.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/frame/parquet.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/frame/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/frame/pivot.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/frame/pivot.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/lib.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/exotic.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/exotic.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/state.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/state.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/streaming/convert.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/streaming/convert.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/prelude.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/tests/aggregations.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/tests/aggregations.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/tests/arity.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/tests/arity.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/tests/cse.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/tests/cse.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/tests/io.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/tests/io.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/tests/logical.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/tests/logical.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/tests/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/tests/optimization_checks.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/tests/optimization_checks.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/tests/predicate_queries.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/tests/predicate_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/tests/projection_queries.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/tests/projection_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/tests/queries.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/tests/queries.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/tests/streaming.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/tests/streaming.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/tests/tpch.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/tests/tpch.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-lazy/src/utils.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-lazy/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/Cargo.toml` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/LICENSE` & `polars_u64_idx-0.17.7/local_dependencies/polars-algo/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/interpolate.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/interpolate.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/list/count.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/list/count.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/list/hash.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/list/hash.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/set.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/set.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/strings/case.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/strings/case.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/chunked_array/top_k.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/chunked_array/top_k.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/frame/join/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/frame/join/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/frame/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/frame/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/frame/pivot/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/frame/pivot/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/frame/pivot/positioning.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/frame/pivot/positioning.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/series/ops/approx_unique.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/series/ops/approx_unique.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/series/ops/floor_divide.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/series/ops/floor_divide.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/series/ops/is_first.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/series/ops/is_first.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/series/ops/is_unique.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/series/ops/is_unique.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/series/ops/log.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/series/ops/log.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/series/ops/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/series/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/series/ops/rolling.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/series/ops/rolling.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/series/ops/search_sorted.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/series/ops/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/series/ops/to_dummies.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/series/ops/to_dummies.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-ops/src/series/ops/various.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-ops/src/series/ops/various.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/Cargo.toml` & `polars_u64_idx-0.17.7/local_dependencies/polars/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/LICENSE` & `polars_u64_idx-0.17.7/local_dependencies/polars-error/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/Makefile` & `polars_u64_idx-0.17.7/local_dependencies/polars/Makefile`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/src/docs/eager.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/src/docs/eager.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/src/docs/lazy.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/src/docs/lazy.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/src/docs/performance.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/src/docs/performance.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/src/lib.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/core/date_like.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/core/date_like.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/core/groupby.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/core/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/core/joins.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/core/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/core/list.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/core/list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/core/pivot.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/core/pivot.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/core/random.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/core/random.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/core/rolling_window.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/core/rolling_window.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/core/series.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/core/series.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/io/csv.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/io/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/io/ipc_stream.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/io/ipc_stream.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/io/json.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/io/json.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/io/parquet.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/io/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/joins.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/aggregation.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/aggregation.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/cse.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/cse.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/expressions/apply.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/expressions/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/expressions/arity.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/expressions/arity.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/expressions/expand.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/expressions/expand.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/expressions/filter.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/expressions/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/expressions/slice.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/expressions/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/expressions/window.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/expressions/window.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/folds.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/folds.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/functions.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/groupby.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/predicate_queries.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/predicate_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/projection_queries.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/projection_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/lazy/queries.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/lazy/queries.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars/tests/it/schema.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars/tests/it/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/Cargo.toml` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/LICENSE` & `polars_u64_idx-0.17.7/local_dependencies/polars-io/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dot.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dot.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/arithmetic.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/binary.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/cat.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/cat.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/dt.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/dt.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/expr.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/expr.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/from.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/from.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/list.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/log.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/log.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -511,14 +511,15 @@
             Uppercase => map!(strings::uppercase),
             Lowercase => map!(strings::lowercase),
             Strip(matches) => map!(strings::strip, matches.as_deref()),
             LStrip(matches) => map!(strings::lstrip, matches.as_deref()),
             RStrip(matches) => map!(strings::rstrip, matches.as_deref()),
             #[cfg(feature = "string_from_radix")]
             FromRadix(radix, strict) => map!(strings::from_radix, radix, strict),
+            Slice(start, length) => map!(strings::str_slice, start, length),
         }
     }
 }
 
 impl From<BinaryFunction> for SpecialEq<Arc<dyn SeriesUdf>> {
     fn from(func: BinaryFunction) -> Self {
         use BinaryFunction::*;
```

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     Uppercase,
     Lowercase,
     Strip(Option<String>),
     RStrip(Option<String>),
     LStrip(Option<String>),
     #[cfg(feature = "string_from_radix")]
     FromRadix(u32, bool),
+    Slice(i64, Option<u64>),
 }
 
 impl StringFunction {
     pub(super) fn get_field(&self, mapper: FieldsMapper) -> PolarsResult<Field> {
         use StringFunction::*;
         match self {
             #[cfg(feature = "regex")]
@@ -78,15 +79,15 @@
             Zfill { .. } | LJust { .. } | RJust { .. } => mapper.with_same_dtype(),
             #[cfg(feature = "temporal")]
             Strptime(options) => mapper.with_dtype(options.date_dtype.clone()),
             #[cfg(feature = "concat_str")]
             ConcatVertical(_) | ConcatHorizontal(_) => mapper.with_dtype(DataType::Utf8),
             #[cfg(feature = "regex")]
             Replace { .. } => mapper.with_dtype(DataType::Utf8),
-            Uppercase | Lowercase | Strip(_) | LStrip(_) | RStrip(_) => {
+            Uppercase | Lowercase | Strip(_) | LStrip(_) | RStrip(_) | Slice(_, _) => {
                 mapper.with_dtype(DataType::Utf8)
             }
             #[cfg(feature = "string_from_radix")]
             FromRadix { .. } => mapper.with_dtype(DataType::Int32),
         }
     }
 }
@@ -119,14 +120,15 @@
             StringFunction::Uppercase => "uppercase",
             StringFunction::Lowercase => "lowercase",
             StringFunction::Strip(_) => "strip",
             StringFunction::LStrip(_) => "lstrip",
             StringFunction::RStrip(_) => "rstrip",
             #[cfg(feature = "string_from_radix")]
             StringFunction::FromRadix { .. } => "from_radix",
+            StringFunction::Slice(_, _) => "str_slice",
         };
 
         write!(f, "str.{s}")
     }
 }
 
 pub(super) fn uppercase(s: &Series) -> PolarsResult<Series> {
@@ -407,16 +409,16 @@
         polars_ensure!(
             out.null_count() == ca.null_count(),
             ComputeError:
             "strict conversion to date(time)s failed.\n\
             \n\
             You might want to try:\n\
             - setting `strict=False`,\n\
-            - explicitly specifying a `fmt`,\n\
-            - setting `utf=True` (if you are parsing datetimes with multiple offsets)."
+            - explicitly specifying a `format`,\n\
+            - setting `utc=True` (if you are parsing datetimes with multiple offsets)."
         );
     }
     Ok(out.into_series())
 }
 
 #[cfg(feature = "concat_str")]
 pub(super) fn concat(s: &Series, delimiter: &str) -> PolarsResult<Series> {
@@ -592,7 +594,11 @@
 }
 
 #[cfg(feature = "string_from_radix")]
 pub(super) fn from_radix(s: &Series, radix: u32, strict: bool) -> PolarsResult<Series> {
     let ca = s.utf8()?;
     ca.parse_int(radix, strict).map(|ok| ok.into_series())
 }
+pub(super) fn str_slice(s: &Series, start: i64, length: Option<u64>) -> PolarsResult<Series> {
+    let ca = s.utf8()?;
+    ca.str_slice(start, length).map(|ca| ca.into_series())
+}
```

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/functions.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/list.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/meta.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/meta.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/options.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/options.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/string.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/string.rs`

 * *Files 1% similar despite different names*

```diff
@@ -402,8 +402,16 @@
     /// Parse string in base radix into decimal
     pub fn from_radix(self, radix: u32, strict: bool) -> Expr {
         self.0
             .map_private(FunctionExpr::StringExpr(StringFunction::FromRadix(
                 radix, strict,
             )))
     }
+
+    /// Slice the string values.
+    pub fn str_slice(self, start: i64, length: Option<u64>) -> Expr {
+        self.0
+            .map_private(FunctionExpr::StringExpr(StringFunction::Slice(
+                start, length,
+            )))
+    }
 }
```

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/dsl/struct_.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/dsl/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/frame/opt_state.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/frame/opt_state.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/alp.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/alp.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/apply.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/builder.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/builder.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/conversion.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/format.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/format.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/iterator.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/lit.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/lit.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/options.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/options.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/projection.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs`

 * *Files 5% similar despite different names*

```diff
@@ -27,30 +27,30 @@
                         Some("True".to_string())
                     } else {
                         Some("False".to_string())
                     }
                 }
                 #[cfg(feature = "dtype-date")]
                 AnyValue::Date(v) => {
-                    // the function `_to_python_datetime` and `Date` have to be in scope
-                    // on the python side
-                    Some(format!("_to_python_datetime(value={v}, dtype=Date)"))
+                    // the function `_to_python_date` and the `Date`
+                    // dtype have to be in scope on the python side
+                    Some(format!("_to_python_date(value={v})"))
                 }
                 #[cfg(feature = "dtype-datetime")]
                 AnyValue::Datetime(v, tu, tz) => {
-                    // the function `_to_python_datetime` and `Datetime` have to be in scope
-                    // on the python side
+                    // the function `_to_python_datetime` and the `Datetime`
+                    // dtype have to be in scope on the python side
                     match tz {
                         None => Some(format!(
-                            "_to_python_datetime(value={}, dtype=Datetime, tu='{}')",
+                            "_to_python_datetime(value={}, tu='{}')",
                             v,
                             tu.to_ascii()
                         )),
                         Some(tz) => Some(format!(
-                            "to_python_datetime(value={}, dtype=Datetime, tu='{}', tz={})",
+                            "_to_python_datetime(value={}, tu='{}', tz={})",
                             v,
                             tu.to_ascii(),
                             tz
                         )),
                     }
                 }
                 // Activate once pyarrow supports them
```

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/logical_plan/schema.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/logical_plan/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/prelude.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/local_dependencies/polars-plan/src/utils.rs` & `polars_u64_idx-0.17.7/local_dependencies/polars-plan/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/Cargo.toml` & `polars_u64_idx-0.17.7/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "py-polars"
-version = "0.17.6"
+version = "0.17.7"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [workspace]
 # prevents package from thinking it's in the workspace
 [target.'cfg(any(not(target_os = "linux"), use_mimalloc))'.dependencies]
```

### Comparing `polars_u64_idx-0.17.6/LICENSE` & `polars_u64_idx-0.17.7/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/Makefile` & `polars_u64_idx-0.17.7/Makefile`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/README.md` & `polars_u64_idx-0.17.7/README.md`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/build.rs` & `polars_u64_idx-0.17.7/build.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/docs/Makefile` & `polars_u64_idx-0.17.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/docs/_templates/autosummary/class.rst` & `polars_u64_idx-0.17.7/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/docs/source/_static/css/custom.css` & `polars_u64_idx-0.17.7/docs/source/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/docs/source/conf.py` & `polars_u64_idx-0.17.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/docs/source/reference/api.rst` & `polars_u64_idx-0.17.7/docs/source/reference/api.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/docs/source/reference/config.rst` & `polars_u64_idx-0.17.7/docs/source/reference/config.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/docs/source/reference/dataframe/modify_select.rst` & `polars_u64_idx-0.17.7/docs/source/reference/dataframe/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/docs/source/reference/datatypes.rst` & `polars_u64_idx-0.17.7/docs/source/reference/datatypes.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/docs/source/reference/expressions/computation.rst` & `polars_u64_idx-0.17.7/docs/source/reference/expressions/computation.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/docs/source/reference/expressions/functions.rst` & `polars_u64_idx-0.17.7/docs/source/reference/expressions/functions.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/docs/source/reference/expressions/list.rst` & `polars_u64_idx-0.17.7/docs/source/reference/expressions/list.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/docs/source/reference/expressions/modify_select.rst` & `polars_u64_idx-0.17.7/docs/source/reference/expressions/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/docs/source/reference/expressions/operators.rst` & `polars_u64_idx-0.17.7/docs/source/reference/expressions/operators.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/docs/source/reference/expressions/string.rst` & `polars_u64_idx-0.17.7/docs/source/reference/expressions/string.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/docs/source/reference/expressions/temporal.rst` & `polars_u64_idx-0.17.7/docs/source/reference/expressions/temporal.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/docs/source/reference/functions.rst` & `polars_u64_idx-0.17.7/docs/source/reference/functions.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/docs/source/reference/io.rst` & `polars_u64_idx-0.17.7/docs/source/reference/io.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/docs/source/reference/lazyframe/modify_select.rst` & `polars_u64_idx-0.17.7/docs/source/reference/lazyframe/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/docs/source/reference/series/computation.rst` & `polars_u64_idx-0.17.7/docs/source/reference/series/computation.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/docs/source/reference/series/descriptive.rst` & `polars_u64_idx-0.17.7/docs/source/reference/series/descriptive.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/docs/source/reference/series/list.rst` & `polars_u64_idx-0.17.7/docs/source/reference/series/list.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/docs/source/reference/series/modify_select.rst` & `polars_u64_idx-0.17.7/docs/source/reference/series/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/docs/source/reference/series/string.rst` & `polars_u64_idx-0.17.7/docs/source/reference/series/string.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/docs/source/reference/series/temporal.rst` & `polars_u64_idx-0.17.7/docs/source/reference/series/temporal.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/docs/source/reference/testing.rst` & `polars_u64_idx-0.17.7/docs/source/reference/testing.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/__init__.py` & `polars_u64_idx-0.17.7/polars/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     UInt32,
     UInt64,
     Unknown,
     Utf8,
 )
 from polars.exceptions import (
     ArrowError,
+    ChronoFormatWarning,
     ColumnNotFoundError,
     ComputeError,
     DuplicateError,
     InvalidOperationError,
     NoDataError,
     PolarsPanicError,
     SchemaError,
@@ -182,14 +183,15 @@
 __all__ = [
     "api",
     "exceptions",
     # exceptions/errors
     "ArrowError",
     "ColumnNotFoundError",
     "ComputeError",
+    "ChronoFormatWarning",
     "DuplicateError",
     "InvalidOperationError",
     "NoDataError",
     "PolarsPanicError",
     "SchemaError",
     "SchemaFieldNotFoundError",
     "ShapeError",
```

### Comparing `polars_u64_idx-0.17.6/polars/api.py` & `polars_u64_idx-0.17.7/polars/api.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/config.py` & `polars_u64_idx-0.17.7/polars/config.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/convert.py` & `polars_u64_idx-0.17.7/polars/convert.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 import re
 from itertools import zip_longest
 from typing import TYPE_CHECKING, Any, Mapping, Sequence, overload
 
 from polars import internals as pli
 from polars.datatypes import (
     N_INFER_DEFAULT,
+    Categorical,
     List,
     Object,
     Struct,
+    Utf8,
 )
 from polars.dependencies import _PYARROW_AVAILABLE
 from polars.dependencies import pandas as pd
 from polars.dependencies import pyarrow as pa
 from polars.exceptions import NoDataError
 from polars.utils.various import _cast_repr_strings_with_schema, parse_version
 
@@ -244,33 +246,118 @@
         schema=schema,
         schema_overrides=schema_overrides,
         orient=orient,
         infer_schema_length=infer_schema_length,
     )
 
 
-def from_repr(tbl: str) -> DataFrame:
+def _from_dataframe_repr(m: re.Match[str]) -> DataFrame:
+    """Reconstruct a DataFrame from a regex-matched table repr."""
+    from polars.datatypes.convert import dtype_short_repr_to_dtype
+
+    # extract elements from table structure
+    lines = m.group().split("\n")[1:-1]
+    rows = [
+        [re.sub(r"^[\W+]*│", "", elem).strip() for elem in row]
+        for row in [re.split("[┆|]", row.rstrip("│ ")) for row in lines]
+        if len(row) > 1 or not re.search("├[╌┼]+┤", row[0])
+    ]
+
+    # determine beginning/end of the header block
+    table_body_start = 2
+    for idx, (elem, *_) in enumerate(rows):
+        if re.match(r"^\W*╞", elem):
+            table_body_start = idx
+            break
+
+    # handle headers with wrapped column names and determine headers/dtypes
+    header_block = ["".join(h).split("---") for h in zip(*rows[:table_body_start])]
+    headers, dtypes = (list(h) for h in zip_longest(*header_block))
+    body = rows[table_body_start + 1 :]
+
+    # transpose rows into columns, detect/omit truncated columns
+    coldata = list(zip(*(row for row in body if not all((e == "…") for e in row))))
+    for el in ("…", "..."):
+        if el in headers:
+            idx = headers.index(el)
+            for table_elem in (headers, dtypes):
+                table_elem.pop(idx)
+            if coldata:
+                coldata.pop(idx)
+
+    # init cols as utf8 Series, handle "null" -> None, create schema from repr dtype
+    data = [pli.Series([(None if v == "null" else v) for v in cd]) for cd in coldata]
+    schema = dict(zip(headers, (dtype_short_repr_to_dtype(d) for d in dtypes)))
+    for dtype in set(schema.values()):
+        if dtype in (List, Struct, Object):
+            raise NotImplementedError(
+                f"'from_repr' does not support {dtype.base_type()} dtype"
+            )
+
+    # construct DataFrame from string series and cast from repr to native dtype
+    df = pli.DataFrame(data=data, orient="col", schema=list(schema))
+    return _cast_repr_strings_with_schema(df, schema)
+
+
+def _from_series_repr(m: re.Match[str]) -> Series:
+    """Reconstruct a Series from a regex-matched series repr."""
+    from polars.datatypes.convert import dtype_short_repr_to_dtype
+
+    shape = m.groups()[0]
+    name = m.groups()[1][1:-1]
+    length = int(shape[1:-2] if shape else -1)
+    dtype = dtype_short_repr_to_dtype(m.groups()[2])
+
+    if length == 0:
+        string_values = []
+    else:
+        string_values = [
+            v.strip()
+            for v in re.findall(r"[\s>#]*(?:\t|\s{4,})([^\n]*)\n", m.groups()[-1])
+        ]
+        if string_values == ["[", "]"]:
+            string_values = []
+        elif string_values and string_values[0].lstrip("#> ") == "[":
+            string_values = string_values[1:]
+
+    values = string_values[:length] if length > 0 else string_values
+    values = [(None if v == "null" else v) for v in values if v not in ("…", "...")]
+
+    if not values:
+        return pli.Series(name=name, values=values, dtype=dtype)
+    else:
+        srs = pli.Series(name=name, values=values, dtype=Utf8)
+        if dtype is None:
+            return srs
+        elif dtype in (Categorical, Utf8):
+            return srs.str.replace('^"(.*)"$', r"$1").cast(dtype)
+
+        return _cast_repr_strings_with_schema(
+            srs.to_frame(), schema={srs.name: dtype}
+        ).to_series()
+
+
+def from_repr(tbl: str) -> DataFrame | Series:
     """
-    Debug function that reconstructs a DataFrame from a table repr.
+    Utility function that reconstructs a DataFrame or Series from the object's repr.
 
     Parameters
     ----------
     tbl
-        A string containing a polars table repr; does not need to be trimmed
-        of whitespace (or leading prompts) as the table will be found/extracted
-        automatically.
+        A string containing a polars DataFrame or Series repr; does not need
+        to be trimmed of whitespace (or leading prompts) as the repr will be
+        found/extracted automatically.
 
     Notes
     -----
-    This function handles the default UTF8_FULL and UTF8_FULL_CONDENSED format
+    This function handles the default UTF8_FULL and UTF8_FULL_CONDENSED DataFrame
     tables (with or without rounded corners). Truncated columns/rows are omitted,
     wrapped headers are accounted for, and dtypes identified.
 
-    Currently compound types such as List and Struct are not supported,
-    (and neither is Time) though support is planned.
+    Currently compound/nested types such as List and Struct are not supported.
 
     See Also
     --------
     polars.DataFrame.to_init_repr
     polars.Series.to_init_repr
 
     Examples
@@ -303,67 +390,39 @@
     └─────────────────┴───────────────────┴───────┴────────────────────────────────┘
     >>> df.schema
     {'source_actor_id': Int32,
      'source_channel_id': Int64,
      'ident': Utf8,
      'timestamp': Datetime(time_unit='us', time_zone='Asia/Tokyo')}
 
-    """
-    from polars.datatypes.convert import dtype_short_repr_to_dtype
+    srs = pl.from_repr'''
+    ... shape: (3,)
+    ... Series: 'a' [bool]
+    ... [
+    ...     true
+    ...     false
+    ...     true
+    ... ]
 
-    # pick dataframe table out of the given string
+    """
+    # find DataFrame table...
     m = re.search(r"([┌╭].*?[┘╯])", tbl, re.DOTALL)
-    if m is None:
-        raise ValueError("Table not found in the given string")
-
-    # extract elements from table structure
-    lines = m.group().split("\n")[1:-1]
-    rows = [
-        [re.sub(r"^[\W+]*│", "", elem).strip() for elem in row]
-        for row in [re.split("[┆|]", row.rstrip("│ ")) for row in lines]
-        if len(row) > 1 or not re.search("├[╌┼]+┤", row[0])
-    ]
-
-    # determine beginning/end of the header block
-    table_body_start = 2
-    for idx, (elem, *_) in enumerate(rows):
-        if re.match(r"^\W*╞", elem):
-            table_body_start = idx
-            break
-
-    # handle headers with wrapped column names and determine headers/dtypes
-    header_block = ["".join(h).split("---") for h in zip(*rows[:table_body_start])]
-    headers, dtypes = (list(h) for h in zip_longest(*header_block))
-    body = rows[table_body_start + 1 :]
-
-    # transpose rows into columns, detect/omit truncated columns
-    coldata = list(zip(*(row for row in body if not all((e == "…") for e in row))))
-    for el in ("…", "..."):
-        if el in headers:
-            idx = headers.index(el)
-            for table_elem in (headers, dtypes):
-                table_elem.pop(idx)
-            if coldata:
-                coldata.pop(idx)
+    if m is not None:
+        return _from_dataframe_repr(m)
 
-    # init cols as utf8 Series, handle "null" -> None, create schema from repr dtype
-    data = [pli.Series([(None if v == "null" else v) for v in cd]) for cd in coldata]
-    schema = dict(zip(headers, (dtype_short_repr_to_dtype(d) for d in dtypes)))
-    for tp in set(schema.values()):
-        # TODO: handle basic compound types
-        if tp in (List, Struct):
-            raise NotImplementedError(
-                f"'from_repr' does not (yet) support {tp} dtype columns"
-            )
-        elif tp == Object:
-            raise ValueError("'from_repr' does not (and cannot) support Object dtype")
+    # ...or Series in the given string
+    m = re.search(
+        pattern=r"(?:shape: (\(\d+,\))\n.*?)?Series:\s+([^\n]+)\s+\[([^\n]+)](.*)",
+        string=tbl,
+        flags=re.DOTALL,
+    )
+    if m is not None:
+        return _from_series_repr(m)
 
-    # construct DataFrame from string series and cast from repr to native dtype
-    df = pli.DataFrame(data=data, orient="col", schema=list(schema))
-    return _cast_repr_strings_with_schema(df, schema)
+    raise ValueError("No DataFrame or Series found in the given string")
 
 
 def from_numpy(
     data: np.ndarray[Any, Any],
     schema: SchemaDefinition | None = None,
     *,
     schema_overrides: SchemaDict | None = None,
```

### Comparing `polars_u64_idx-0.17.6/polars/dataframe/_html.py` & `polars_u64_idx-0.17.7/polars/dataframe/_html.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/dataframe/frame.py` & `polars_u64_idx-0.17.7/polars/dataframe/frame.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/dataframe/groupby.py` & `polars_u64_idx-0.17.7/polars/dataframe/groupby.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/datatypes/__init__.py` & `polars_u64_idx-0.17.7/polars/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/datatypes/classes.py` & `polars_u64_idx-0.17.7/polars/datatypes/classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -309,22 +309,19 @@
         inner
             The `DataType` of values within the list
 
         """
         self.inner = polars.datatypes.py_type_to_dtype(inner)
 
     def __eq__(self, other: PolarsDataType) -> bool:  # type: ignore[override]
-        # The comparison allows comparing objects to classes
-        # and specific inner types to none specific.
-        # if one of the arguments is not specific about its inner type
-        # we infer it as being equal.
-        # List[i64] == List[i64] == True
-        # List[i64] == List == True
-        # List[i64] == List[None] == True
-        # List[i64] == List[f32] == False
+        # This equality check allows comparison of type classes and type instances.
+        # If a parent type is not specific about its inner type, we infer it as equal:
+        # > list[i64] == list[i64] -> True
+        # > list[i64] == list[f32] -> False
+        # > list[i64] == list      -> True
 
         # allow comparing object instances to class
         if type(other) is DataTypeClass and issubclass(other, List):
             return True
         if isinstance(other, List):
             if self.inner is None or other.inner is None:
                 return True
```

### Comparing `polars_u64_idx-0.17.6/polars/datatypes/constants.py` & `polars_u64_idx-0.17.7/polars/datatypes/constants.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/datatypes/constructor.py` & `polars_u64_idx-0.17.7/polars/datatypes/constructor.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/datatypes/convert.py` & `polars_u64_idx-0.17.7/polars/datatypes/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,14 +227,15 @@
             Int64: "i64",
             UInt8: "u8",
             UInt16: "u16",
             UInt32: "u32",
             UInt64: "u64",
             Float32: "f32",
             Float64: "f64",
+            Decimal: "decimal",
             Boolean: "bool",
             Utf8: "str",
             List: "list",
             Date: "date",
             Datetime: "datetime",
             Duration: "duration",
             Time: "time",
@@ -444,17 +445,22 @@
     m = re.match(r"^(\w+)(?:\[(.+)\])?$", dtype_string)
     if m is None:
         return None
 
     dtype_base, subtype = m.groups()
     dtype = DataTypeMappings.REPR_TO_DTYPE.get(dtype_base)
     if dtype and subtype:
-        # TODO: better-handle nested types (such as List,Struct)
-        subtype = (s.strip("""'" """) for s in subtype.replace("μs", "us").split(","))
+        # TODO: further-improve handling for nested types (such as List,Struct)
         try:
+            if dtype == Decimal:
+                subtype = (None, int(subtype))
+            else:
+                subtype = (
+                    s.strip("'\" ") for s in subtype.replace("μs", "us").split(",")
+                )
             return dtype(*subtype)  # type: ignore[operator]
         except ValueError:
             pass
     return dtype
 
 
 def supported_numpy_char_code(dtype_char: str) -> bool:
```

### Comparing `polars_u64_idx-0.17.6/polars/dependencies.py` & `polars_u64_idx-0.17.7/polars/dependencies.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/exceptions.py` & `polars_u64_idx-0.17.7/polars/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,18 +62,31 @@
     """Exception raised when no rows are returned, but at least one row is expected."""
 
 
 class TooManyRowsReturnedError(RowsError):
     """Exception raised when more rows than expected are returned."""
 
 
+class ChronoFormatWarning(Warning):
+    """
+    Warning raised when a chrono format string contains dubious patterns.
+
+    Polars uses Rust's chrono crate to convert between string data and temporal data.
+    The patterns used by chrono differ slightly from Python's built-in datetime module.
+    Refer to the `chrono strftime documentation
+    <https://docs.rs/chrono/latest/chrono/format/strftime/index.html>`_ for the full
+    specification.
+    """
+
+
 __all__ = [
     "ArrowError",
     "ColumnNotFoundError",
     "ComputeError",
+    "ChronoFormatWarning",
     "DuplicateError",
     "InvalidOperationError",
     "NoDataError",
     "NoRowsReturnedError",
     "PolarsPanicError",
     "RowsError",
     "SchemaError",
```

### Comparing `polars_u64_idx-0.17.6/polars/expr/binary.py` & `polars_u64_idx-0.17.7/polars/expr/binary.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/expr/categorical.py` & `polars_u64_idx-0.17.7/polars/expr/categorical.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/expr/datetime.py` & `polars_u64_idx-0.17.7/polars/expr/datetime.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/expr/expr.py` & `polars_u64_idx-0.17.7/polars/expr/expr.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/expr/list.py` & `polars_u64_idx-0.17.7/polars/expr/list.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/expr/meta.py` & `polars_u64_idx-0.17.7/polars/expr/meta.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/expr/string.py` & `polars_u64_idx-0.17.7/polars/expr/string.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 from __future__ import annotations
 
 import warnings
 from typing import TYPE_CHECKING
 
-from polars.datatypes import (
-    DataType,
-    Date,
-    Datetime,
-    Time,
-    is_polars_dtype,
-    py_type_to_dtype,
-)
+from polars.datatypes import Date, Datetime, Time, py_type_to_dtype
+from polars.exceptions import ChronoFormatWarning
 from polars.utils import no_default
 from polars.utils._parse_expr_input import expr_to_lit_or_expr
 from polars.utils._wrap import wrap_expr
 from polars.utils.decorators import deprecated_alias
 from polars.utils.various import find_stacklevel
 
 if TYPE_CHECKING:
@@ -118,27 +112,15 @@
         │ 2021-04-22 │
         │ 2022-01-04 │
         │ 2022-01-31 │
         │ 2001-07-08 │
         └────────────┘
 
         """
-        if not is_polars_dtype(dtype):
-            raise ValueError(f"expected: {DataType} got: {dtype}")
-
-        if format is not None and "%f" in format:
-            raise ValueError(
-                "Directive '%f' is not supported in Python Polars, "
-                "as it differs from the Python standard library.\n"
-                "Instead, please use one of:\n"
-                " - '%.f'\n"
-                " - '%3f'\n"
-                " - '%6f'\n"
-                " - '%9f'"
-            )
+        _validate_format_argument(format)
 
         if tz_aware is no_default:
             tz_aware = False
         else:
             warnings.warn(
                 "`tz_aware` is now auto-inferred from `format` and will be removed "
                 "in a future version. You can safely drop this argument.",
@@ -1340,7 +1322,20 @@
         │ 65280 │
         │ 51966 │
         │ null  │
         └───────┘
 
         """
         return wrap_expr(self._pyexpr.str_parse_int(radix, strict))
+
+
+def _validate_format_argument(format: str | None) -> None:
+    if format is not None and ".%f" in format:
+        message = (
+            "Detected the pattern `.%f` in the chrono format string."
+            " This pattern should not be used to parse values after a decimal point."
+            " Use `%.f` instead."
+            " See the full specification: https://docs.rs/chrono/latest/chrono/format/strftime"
+        )
+        warnings.warn(
+            message, category=ChronoFormatWarning, stacklevel=find_stacklevel()
+        )
```

### Comparing `polars_u64_idx-0.17.6/polars/expr/struct.py` & `polars_u64_idx-0.17.7/polars/expr/struct.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/functions/__init__.py` & `polars_u64_idx-0.17.7/polars/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/functions/eager.py` & `polars_u64_idx-0.17.7/polars/functions/eager.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/functions/lazy.py` & `polars_u64_idx-0.17.7/polars/functions/lazy.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/functions/whenthen.py` & `polars_u64_idx-0.17.7/polars/functions/whenthen.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/io/__init__.py` & `polars_u64_idx-0.17.7/polars/io/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/io/_utils.py` & `polars_u64_idx-0.17.7/polars/io/_utils.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/io/avro.py` & `polars_u64_idx-0.17.7/polars/io/avro.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/io/csv/_utils.py` & `polars_u64_idx-0.17.7/polars/io/csv/_utils.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/io/csv/batched_reader.py` & `polars_u64_idx-0.17.7/polars/io/csv/batched_reader.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/io/csv/functions.py` & `polars_u64_idx-0.17.7/polars/io/csv/functions.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/io/database.py` & `polars_u64_idx-0.17.7/polars/io/database.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/io/delta.py` & `polars_u64_idx-0.17.7/polars/io/delta.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/io/excel/_write_utils.py` & `polars_u64_idx-0.17.7/polars/io/excel/_write_utils.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/io/excel/functions.py` & `polars_u64_idx-0.17.7/polars/io/excel/functions.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/io/ipc/anonymous_scan.py` & `polars_u64_idx-0.17.7/polars/io/ipc/anonymous_scan.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/io/ipc/functions.py` & `polars_u64_idx-0.17.7/polars/io/ipc/functions.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/io/json.py` & `polars_u64_idx-0.17.7/polars/io/json.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/io/ndjson.py` & `polars_u64_idx-0.17.7/polars/io/ndjson.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/io/parquet/anonymous_scan.py` & `polars_u64_idx-0.17.7/polars/io/parquet/anonymous_scan.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/io/parquet/functions.py` & `polars_u64_idx-0.17.7/polars/io/parquet/functions.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/io/pyarrow_dataset/anonymous_scan.py` & `polars_u64_idx-0.17.7/polars/io/pyarrow_dataset/anonymous_scan.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/io/pyarrow_dataset/functions.py` & `polars_u64_idx-0.17.7/polars/io/pyarrow_dataset/functions.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/lazyframe/frame.py` & `polars_u64_idx-0.17.7/polars/lazyframe/frame.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/lazyframe/groupby.py` & `polars_u64_idx-0.17.7/polars/lazyframe/groupby.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/series/_numpy.py` & `polars_u64_idx-0.17.7/polars/series/_numpy.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/series/binary.py` & `polars_u64_idx-0.17.7/polars/series/binary.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/series/categorical.py` & `polars_u64_idx-0.17.7/polars/series/categorical.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/series/datetime.py` & `polars_u64_idx-0.17.7/polars/series/datetime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from polars import functions as F
+from polars.datatypes import Date
 from polars.series.utils import expr_dispatch
 from polars.utils._wrap import wrap_s
-from polars.utils.convert import _to_python_datetime
+from polars.utils.convert import _to_python_date, _to_python_datetime
 from polars.utils.decorators import deprecated_alias
 
 if TYPE_CHECKING:
     import datetime as dt
 
     from polars.expr.expr import Expr
     from polars.polars import PySeries
@@ -93,15 +94,18 @@
         >>> date.dt.median()
         datetime.datetime(2001, 1, 2, 0, 0)
 
         """
         s = wrap_s(self._s)
         out = s.median()
         if out is not None:
-            return _to_python_datetime(int(out), s.dtype, s.time_unit)
+            if s.dtype == Date:
+                return _to_python_date(int(out))
+            else:
+                return _to_python_datetime(int(out), s.time_unit)
         return None
 
     def mean(self) -> dt.date | dt.datetime | None:
         """
         Return mean as python DateTime.
 
         Examples
@@ -119,15 +123,18 @@
         >>> date.dt.mean()
         datetime.datetime(2001, 1, 2, 0, 0)
 
         """
         s = wrap_s(self._s)
         out = s.mean()
         if out is not None:
-            return _to_python_datetime(int(out), s.dtype, s.time_unit)
+            if s.dtype == Date:
+                return _to_python_date(int(out))
+            else:
+                return _to_python_datetime(int(out), s.time_unit)
         return None
 
     @deprecated_alias(fmt="format")
     def strftime(self, format: str) -> Series:
         """
         Format Date/datetime with a formatting rule.
```

### Comparing `polars_u64_idx-0.17.6/polars/series/list.py` & `polars_u64_idx-0.17.7/polars/series/list.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/series/series.py` & `polars_u64_idx-0.17.7/polars/series/series.py`

 * *Files 0% similar despite different names*

```diff
@@ -3253,41 +3253,49 @@
                 tp = "datetime64[D]"
             elif self.dtype == Duration:
                 tp = f"timedelta64[{self.time_unit}]"
             else:
                 tp = f"datetime64[{self.time_unit}]"
             return arr.astype(tp)
 
+        def raise_no_zero_copy() -> None:
+            if zero_copy_only:
+                raise ValueError("Cannot return a zero-copy array")
+
         if (
             use_pyarrow
             and _PYARROW_AVAILABLE
             and self.dtype != Object
             and not self.is_temporal(excluding=Time)
         ):
             return self.to_arrow().to_numpy(
                 *args, zero_copy_only=zero_copy_only, writable=writable
             )
         elif self.dtype == Time:
+            raise_no_zero_copy()
             # note: there is no native numpy "time" dtype
             return np.array(self.to_list(), dtype="object")
         else:
             if not self.has_validity():
                 if self.is_temporal():
                     np_array = convert_to_date(self.view(ignore_nulls=True))
                 elif self.is_numeric():
                     np_array = self.view(ignore_nulls=True)
                 else:
+                    raise_no_zero_copy()
                     np_array = self._s.to_numpy()
 
             elif self.is_temporal():
                 np_array = convert_to_date(self.to_physical()._s.to_numpy())
             else:
+                raise_no_zero_copy()
                 np_array = self._s.to_numpy()
 
             if writable and not np_array.flags.writeable:
+                raise_no_zero_copy()
                 return np_array.copy()
             else:
                 return np_array
 
     def to_arrow(self) -> pa.Array:
         """
         Get the underlying Arrow Array.
```

### Comparing `polars_u64_idx-0.17.6/polars/series/string.py` & `polars_u64_idx-0.17.7/polars/series/string.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/series/struct.py` & `polars_u64_idx-0.17.7/polars/series/struct.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/series/utils.py` & `polars_u64_idx-0.17.7/polars/series/utils.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/slice.py` & `polars_u64_idx-0.17.7/polars/slice.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/sql/context.py` & `polars_u64_idx-0.17.7/polars/sql/context.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/string_cache.py` & `polars_u64_idx-0.17.7/polars/string_cache.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/testing/_private.py` & `polars_u64_idx-0.17.7/polars/testing/_private.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/testing/_tempdir.py` & `polars_u64_idx-0.17.7/polars/testing/_tempdir.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/testing/asserts.py` & `polars_u64_idx-0.17.7/polars/testing/asserts.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/testing/parametric/__init__.py` & `polars_u64_idx-0.17.7/polars/testing/parametric/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/testing/parametric/primitives.py` & `polars_u64_idx-0.17.7/polars/testing/parametric/primitives.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 from hypothesis.strategies._internal.utils import defines_strategy
 
 from polars.dataframe import DataFrame
 from polars.datatypes import (
     DTYPE_TEMPORAL_UNITS,
     FLOAT_DTYPES,
     Categorical,
+    DataType,
+    DataTypeClass,
     Datetime,
     Duration,
     List,
     is_polars_dtype,
     py_type_to_dtype,
 )
 from polars.series import Series
@@ -252,16 +254,16 @@
     min_size: int | None = 0,
     max_size: int | None = MAX_DATA_SIZE,
     strategy: SearchStrategy[object] | None = None,
     null_probability: float = 0.0,
     allow_infinities: bool = True,
     unique: bool = False,
     chunked: bool | None = None,
-    allowed_dtypes: Collection[PolarsDataType] | None = None,
-    excluded_dtypes: Collection[PolarsDataType] | None = None,
+    allowed_dtypes: Collection[PolarsDataType] | PolarsDataType | None = None,
+    excluded_dtypes: Collection[PolarsDataType] | PolarsDataType | None = None,
 ) -> SearchStrategy[Series]:
     """
     Strategy for producing a polars Series.
 
     Parameters
     ----------
     name : {str, strategy}, optional
@@ -321,14 +323,19 @@
         54666
         -35
         6414
         -63290
     ]
 
     """
+    if isinstance(allowed_dtypes, (DataType, DataTypeClass)):
+        allowed_dtypes = [allowed_dtypes]
+    if isinstance(excluded_dtypes, (DataType, DataTypeClass)):
+        excluded_dtypes = [excluded_dtypes]
+
     selectable_dtypes = [
         dtype
         for dtype in (allowed_dtypes or strategy_dtypes)
         if dtype not in (excluded_dtypes or ())
     ]
     if null_probability and (null_probability < 0 or null_probability > 1):
         raise InvalidArgument(
@@ -423,16 +430,16 @@
     size: int | None = None,
     min_size: int | None = 0,
     max_size: int | None = MAX_DATA_SIZE,
     chunked: bool | None = None,
     include_cols: Sequence[column] | None = None,
     null_probability: float | dict[str, float] = 0.0,
     allow_infinities: bool = True,
-    allowed_dtypes: Collection[PolarsDataType] | None = None,
-    excluded_dtypes: Collection[PolarsDataType] | None = None,
+    allowed_dtypes: Collection[PolarsDataType] | PolarsDataType | None = None,
+    excluded_dtypes: Collection[PolarsDataType] | PolarsDataType | None = None,
 ) -> SearchStrategy[DataFrame | LazyFrame]:
     """
     Provides a strategy for producing a DataFrame or LazyFrame.
 
     Parameters
     ----------
     cols : {int, columns}, optional
@@ -523,14 +530,18 @@
     │ 575050513 ┆ NaN        │
     └───────────┴────────────┘
     """  # noqa: 501
     _failed_frame_init_msgs_.clear()
 
     if isinstance(min_size, int) and min_cols in (0, None):
         min_cols = 1
+    if isinstance(allowed_dtypes, (DataType, DataTypeClass)):
+        allowed_dtypes = [allowed_dtypes]
+    if isinstance(excluded_dtypes, (DataType, DataTypeClass)):
+        excluded_dtypes = [excluded_dtypes]
 
     selectable_dtypes = [
         dtype
         for dtype in (allowed_dtypes or strategy_dtypes)
         if dtype not in (excluded_dtypes or ())
     ]
```

### Comparing `polars_u64_idx-0.17.6/polars/testing/parametric/strategies.py` & `polars_u64_idx-0.17.7/polars/testing/parametric/strategies.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from __future__ import annotations
 
+import os
 from datetime import datetime, timedelta
 from random import choice
 from string import ascii_letters, ascii_uppercase, digits, punctuation
 from typing import TYPE_CHECKING, Any, Sequence
 
 from hypothesis.strategies import (
     booleans,
     characters,
     dates,
     datetimes,
+    decimals,
     floats,
     from_type,
     integers,
     lists,
     sampled_from,
     text,
     timedeltas,
@@ -21,14 +23,15 @@
 )
 
 from polars.datatypes import (
     Boolean,
     Categorical,
     Date,
     Datetime,
+    Decimal,
     Duration,
     Float32,
     Float64,
     Int8,
     Int16,
     Int32,
     Int64,
@@ -63,14 +66,24 @@
 strategy_i32 = integers(min_value=-(2**31), max_value=(2**31) - 1)
 strategy_i64 = integers(min_value=-(2**63), max_value=(2**63) - 1)
 strategy_u8 = integers(min_value=0, max_value=(2**8) - 1)
 strategy_u16 = integers(min_value=0, max_value=(2**16) - 1)
 strategy_u32 = integers(min_value=0, max_value=(2**32) - 1)
 strategy_u64 = integers(min_value=0, max_value=(2**64) - 1)
 
+# TODO: once fixed, re-enable decimal nan/inf values.
+# TODO: vary the number of decimal places.
+strategy_decimal = decimals(
+    allow_nan=False,
+    allow_infinity=False,
+    min_value=-(2**66),
+    max_value=(2**66) - 1,
+    places=18,
+)
+
 strategy_ascii = text(max_size=8, alphabet=ascii_letters + digits + punctuation)
 strategy_categorical = text(max_size=2, alphabet=ascii_uppercase)
 strategy_utf8 = text(
     alphabet=characters(max_codepoint=1000, blacklist_categories=("Cs", "Cc")),
     max_size=8,
 )
 strategy_datetime_ns = datetimes(
@@ -109,14 +122,19 @@
     Duration("ns"): strategy_duration,
     Duration("us"): strategy_duration,
     Duration("ms"): strategy_duration,
     Duration: strategy_duration,
     Categorical: strategy_categorical,
     Utf8: strategy_utf8,
 }
+
+# note: decimal support is in early development and requires opt-in
+if os.environ.get("POLARS_ACTIVATE_DECIMAL") == "1":
+    scalar_strategies[Decimal] = strategy_decimal
+
 _strategy_dtypes = list(scalar_strategies) + [List]
 
 
 def _hash(elem: Any) -> int:
     """Hashing that can also handle lists (for 'unique' check)."""
     if isinstance(elem, list):
         return hash(tuple(_hash(e) for e in elem))
```

### Comparing `polars_u64_idx-0.17.6/polars/type_aliases.py` & `polars_u64_idx-0.17.7/polars/type_aliases.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/utils/__init__.py` & `polars_u64_idx-0.17.7/polars/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from polars.utils.build_info import build_info
 from polars.utils.convert import (
     _date_to_pl_date,
     _datetime_for_anyvalue,
     _datetime_for_anyvalue_windows,
     _time_to_pl_time,
     _timedelta_to_pl_timedelta,
+    _to_python_date,
     _to_python_datetime,
     _to_python_decimal,
     _to_python_time,
     _to_python_timedelta,
     _tzinfo_to_str,
 )
 from polars.utils.meta import get_idx_type, get_index_type, threadpool_size
@@ -30,14 +31,15 @@
     "get_index_type",
     "threadpool_size",
     # Required for Rust bindings
     "_date_to_pl_date",
     "_deserialize_and_execute",
     "_time_to_pl_time",
     "_timedelta_to_pl_timedelta",
+    "_to_python_date",
     "_to_python_datetime",
     "_to_python_decimal",
     "_to_python_time",
     "_to_python_timedelta",
     "_datetime_for_anyvalue",
     "_datetime_for_anyvalue_windows",
     "_tzinfo_to_str",
```

### Comparing `polars_u64_idx-0.17.6/polars/utils/_construction.py` & `polars_u64_idx-0.17.7/polars/utils/_construction.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/utils/_parse_expr_input.py` & `polars_u64_idx-0.17.7/polars/utils/_parse_expr_input.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/utils/_scan.py` & `polars_u64_idx-0.17.7/polars/utils/_scan.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/utils/_wrap.py` & `polars_u64_idx-0.17.7/polars/utils/_wrap.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/utils/build_info.py` & `polars_u64_idx-0.17.7/polars/utils/build_info.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/utils/convert.py` & `polars_u64_idx-0.17.7/polars/utils/convert.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from __future__ import annotations
 
-import functools
 import sys
 from datetime import datetime, time, timedelta, timezone
 from decimal import Context
+from functools import lru_cache
 from typing import TYPE_CHECKING, Any, Callable, Sequence, TypeVar, overload
 
-from polars.datatypes import Date, Datetime
 from polars.dependencies import _ZONEINFO_AVAILABLE, zoneinfo
 
 if TYPE_CHECKING:
     from collections.abc import Reversible
     from datetime import date, tzinfo
     from decimal import Decimal
 
-    from polars.type_aliases import PolarsDataType, TimeUnit
+    from polars.type_aliases import TimeUnit
 
     if sys.version_info >= (3, 10):
         from typing import ParamSpec
     else:
         from typing_extensions import ParamSpec
 
     P = ParamSpec("P")
@@ -31,15 +30,14 @@
     elif _ZONEINFO_AVAILABLE:
         from backports.zoneinfo._zoneinfo import ZoneInfo
 
     def get_zoneinfo(key: str) -> ZoneInfo:
         pass
 
 else:
-    from functools import lru_cache
 
     @lru_cache(None)
     def get_zoneinfo(key: str) -> ZoneInfo:
         return zoneinfo.ZoneInfo(key)
 
 
 # note: reversed views don't match as instances of MappingView
@@ -158,57 +156,53 @@
 
 EPOCH = datetime(1970, 1, 1).replace(tzinfo=None)
 EPOCH_UTC = datetime(1970, 1, 1, tzinfo=timezone.utc)
 
 _fromtimestamp = datetime.fromtimestamp
 
 
+@lru_cache(256)
+def _to_python_date(value: int | float) -> date:
+    """Convert polars int64 timestamp to Python date."""
+    return (EPOCH_UTC + timedelta(seconds=value * 86400)).date()
+
+
 def _to_python_datetime(
     value: int | float,
-    dtype: PolarsDataType,
     time_unit: TimeUnit | None = "ns",
     time_zone: str | None = None,
-) -> date | datetime:
-    """Convert polars int64 timestamp to Python date/datetime."""
-    if dtype == Date:
-        # important to create from utc; not doing this leads to
-        # inconsistencies dependent on the timezone you are in.
-        return (EPOCH_UTC + timedelta(seconds=value * 86400)).date()
-
-    elif dtype == Datetime:
-        if not time_zone:
-            if time_unit == "ns":
-                return EPOCH + timedelta(microseconds=value // 1000)
-            elif time_unit == "us":
-                return EPOCH + timedelta(microseconds=value)
-            elif time_unit == "ms":
-                return EPOCH + timedelta(milliseconds=value)
-            else:
-                raise ValueError(
-                    f"time_unit must be one of {{'ns','us','ms'}}, got {time_unit}"
-                )
-
-        elif _ZONEINFO_AVAILABLE:
-            if time_unit == "ns":
-                dt = EPOCH_UTC + timedelta(microseconds=value // 1000)
-            elif time_unit == "us":
-                dt = EPOCH_UTC + timedelta(microseconds=value)
-            elif time_unit == "ms":
-                dt = EPOCH_UTC + timedelta(milliseconds=value)
-            else:
-                raise ValueError(
-                    f"time_unit must be one of {{'ns','us','ms'}}, got {time_unit}"
-                )
-            return _localize(dt, time_zone)
+) -> datetime:
+    """Convert polars int64 timestamp to Python datetime."""
+    if not time_zone:
+        if time_unit == "us":
+            return EPOCH + timedelta(microseconds=value)
+        elif time_unit == "ns":
+            return EPOCH + timedelta(microseconds=value // 1000)
+        elif time_unit == "ms":
+            return EPOCH + timedelta(milliseconds=value)
         else:
-            raise ImportError(
-                "Install polars[timezone] to handle datetimes with timezones."
+            raise ValueError(
+                f"time_unit must be one of {{'ns','us','ms'}}, got {time_unit}"
             )
+    elif _ZONEINFO_AVAILABLE:
+        if time_unit == "us":
+            dt = EPOCH_UTC + timedelta(microseconds=value)
+        elif time_unit == "ns":
+            dt = EPOCH_UTC + timedelta(microseconds=value // 1000)
+        elif time_unit == "ms":
+            dt = EPOCH_UTC + timedelta(milliseconds=value)
+        else:
+            raise ValueError(
+                f"time_unit must be one of {{'ns','us','ms'}}, got {time_unit}"
+            )
+        return _localize(dt, time_zone)
     else:
-        raise NotImplementedError  # pragma: no cover
+        raise ImportError(
+            "Install polars[timezone] to handle datetimes with timezones."
+        )
 
 
 def _localize(dt: datetime, time_zone: str) -> datetime:
     # zone info installation should already be checked
     _tzinfo: ZoneInfo | tzinfo
     try:
         _tzinfo = get_zoneinfo(time_zone)
@@ -233,15 +227,15 @@
         dt = _localize(dt, "UTC")
     # returns (s, ms)
     return (dt.replace(microsecond=0).timestamp(), dt.microsecond)
 
 
 # cache here as we have a single tz per column
 # and this function will be called on every conversion
-@functools.lru_cache(16)
+@lru_cache(16)
 def _parse_fixed_tz_offset(offset: str) -> tzinfo:
     try:
         # use fromisoformat to parse the offset
         dt_offset = datetime.fromisoformat("2000-01-01T00:00:00" + offset)
 
         # alternatively, we parse the offset ourselves extracting hours and
         # minutes, then we can construct:
@@ -254,15 +248,15 @@
 
 def _to_python_decimal(
     sign: int, digits: Sequence[int], prec: int, scale: int
 ) -> Decimal:
     return _create_decimal_with_prec(prec)((sign, digits, scale))
 
 
-@functools.lru_cache(None)
+@lru_cache(None)
 def _create_decimal_with_prec(
     precision: int,
 ) -> Callable[[tuple[int, Sequence[int], int]], Decimal]:
     # pre-cache contexts so we don't have to spend time on recreating them every time
     return Context(prec=precision).create_decimal
```

### Comparing `polars_u64_idx-0.17.6/polars/utils/decorators.py` & `polars_u64_idx-0.17.7/polars/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/utils/meta.py` & `polars_u64_idx-0.17.7/polars/utils/meta.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/utils/polars_version.py` & `polars_u64_idx-0.17.7/polars/utils/polars_version.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/utils/show_versions.py` & `polars_u64_idx-0.17.7/polars/utils/show_versions.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/polars/utils/various.py` & `polars_u64_idx-0.17.7/polars/utils/various.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/pyproject.toml` & `polars_u64_idx-0.17.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/requirements-dev.txt` & `polars_u64_idx-0.17.7/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/scripts/check_stacklevels.py` & `polars_u64_idx-0.17.7/scripts/check_stacklevels.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/src/apply/dataframe.rs` & `polars_u64_idx-0.17.7/src/apply/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/src/apply/mod.rs` & `polars_u64_idx-0.17.7/src/apply/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/src/apply/series.rs` & `polars_u64_idx-0.17.7/src/apply/series.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/src/arrow_interop/to_py.rs` & `polars_u64_idx-0.17.7/src/arrow_interop/to_py.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/src/arrow_interop/to_rust.rs` & `polars_u64_idx-0.17.7/src/arrow_interop/to_rust.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/src/batched_csv.rs` & `polars_u64_idx-0.17.7/src/batched_csv.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/src/conversion.rs` & `polars_u64_idx-0.17.7/src/conversion.rs`

 * *Files 3% similar despite different names*

```diff
@@ -194,15 +194,14 @@
         *ptr.add(2) -= ZEROS;
     }
     len
 }
 
 impl IntoPy<PyObject> for Wrap<AnyValue<'_>> {
     fn into_py(self, py: Python) -> PyObject {
-        let pl = POLARS.as_ref(py);
         let utils = UTILS.as_ref(py);
         match self.0 {
             AnyValue::UInt8(v) => v.into_py(py),
             AnyValue::UInt16(v) => v.into_py(py),
             AnyValue::UInt32(v) => v.into_py(py),
             AnyValue::UInt64(v) => v.into_py(py),
             AnyValue::Int8(v) => v.into_py(py),
@@ -220,29 +219,22 @@
                     rev.get(idx)
                 } else {
                     unsafe { arr.deref_unchecked().value(idx as usize) }
                 };
                 s.into_py(py)
             }
             AnyValue::Date(v) => {
-                let convert = utils.getattr("_to_python_datetime").unwrap();
-                let py_date_dtype = pl.getattr("Date").unwrap();
-                convert.call1((v, py_date_dtype)).unwrap().into_py(py)
+                let convert = utils.getattr("_to_python_date").unwrap();
+                convert.call1((v,)).unwrap().into_py(py)
             }
             AnyValue::Datetime(v, time_unit, time_zone) => {
                 let convert = utils.getattr("_to_python_datetime").unwrap();
-                let py_datetime_dtype = pl.getattr("Datetime").unwrap();
                 let time_unit = time_unit.to_ascii();
                 convert
-                    .call1((
-                        v,
-                        py_datetime_dtype,
-                        time_unit,
-                        time_zone.as_ref().map(|s| s.as_str()),
-                    ))
+                    .call1((v, time_unit, time_zone.as_ref().map(|s| s.as_str())))
                     .unwrap()
                     .into_py(py)
             }
             AnyValue::Duration(v, time_unit) => {
                 let convert = utils.getattr("_to_python_timedelta").unwrap();
                 let time_unit = time_unit.to_ascii();
                 convert.call1((v, time_unit)).unwrap().into_py(py)
@@ -502,26 +494,22 @@
             .map(|opt_v| opt_v.map(|v| convert.call1((v, &time_unit)).unwrap()));
         PyList::new(py, iter).into_py(py)
     }
 }
 
 impl ToPyObject for Wrap<&DatetimeChunked> {
     fn to_object(&self, py: Python) -> PyObject {
-        let (pl, utils) = (POLARS.as_ref(py), UTILS.as_ref(py));
+        let utils = UTILS.as_ref(py);
         let convert = utils.getattr("_to_python_datetime").unwrap();
-        let py_date_dtype = pl.getattr("Datetime").unwrap();
         let time_unit = Wrap(self.0.time_unit()).to_object(py);
         let time_zone = self.0.time_zone().to_object(py);
-        let iter = self.0.into_iter().map(|opt_v| {
-            opt_v.map(|v| {
-                convert
-                    .call1((v, py_date_dtype, &time_unit, &time_zone))
-                    .unwrap()
-            })
-        });
+        let iter = self
+            .0
+            .into_iter()
+            .map(|opt_v| opt_v.map(|v| convert.call1((v, &time_unit, &time_zone)).unwrap()));
         PyList::new(py, iter).into_py(py)
     }
 }
 
 impl ToPyObject for Wrap<&TimeChunked> {
     fn to_object(&self, py: Python) -> PyObject {
         let utils = UTILS.as_ref(py);
@@ -532,21 +520,20 @@
             .map(|opt_v| opt_v.map(|v| convert.call1((v,)).unwrap()));
         PyList::new(py, iter).into_py(py)
     }
 }
 
 impl ToPyObject for Wrap<&DateChunked> {
     fn to_object(&self, py: Python) -> PyObject {
-        let (pl, utils) = (POLARS.as_ref(py), UTILS.as_ref(py));
-        let convert = utils.getattr("_to_python_datetime").unwrap();
-        let py_date_dtype = pl.getattr("Date").unwrap();
+        let utils = UTILS.as_ref(py);
+        let convert = utils.getattr("_to_python_date").unwrap();
         let iter = self
             .0
             .into_iter()
-            .map(|opt_v| opt_v.map(|v| convert.call1((v, py_date_dtype)).unwrap()));
+            .map(|opt_v| opt_v.map(|v| convert.call1((v,)).unwrap()));
         PyList::new(py, iter).into_py(py)
     }
 }
 
 impl ToPyObject for Wrap<&DecimalChunked> {
     fn to_object(&self, py: Python) -> PyObject {
         let utils = UTILS.as_ref(py);
```

### Comparing `polars_u64_idx-0.17.6/src/dataframe.rs` & `polars_u64_idx-0.17.7/src/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/src/datatypes.rs` & `polars_u64_idx-0.17.7/src/datatypes.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/src/error.rs` & `polars_u64_idx-0.17.7/src/error.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/src/file.rs` & `polars_u64_idx-0.17.7/src/file.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/src/lazy/apply.rs` & `polars_u64_idx-0.17.7/src/lazy/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/src/lazy/dataframe.rs` & `polars_u64_idx-0.17.7/src/lazy/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/src/lazy/dsl.rs` & `polars_u64_idx-0.17.7/src/lazy/dsl.rs`

 * *Files 0% similar despite different names*

```diff
@@ -650,23 +650,15 @@
     }
 
     pub fn str_lstrip(&self, matches: Option<String>) -> PyExpr {
         self.inner.clone().str().lstrip(matches).into()
     }
 
     pub fn str_slice(&self, start: i64, length: Option<u64>) -> PyExpr {
-        let function = move |s: Series| {
-            let ca = s.utf8()?;
-            Ok(Some(ca.str_slice(start, length)?.into_series()))
-        };
-        self.clone()
-            .inner
-            .map(function, GetOutput::from_type(DataType::Utf8))
-            .with_fmt("str.slice")
-            .into()
+        self.inner.clone().str().str_slice(start, length).into()
     }
 
     pub fn str_to_uppercase(&self) -> PyExpr {
         self.inner.clone().str().to_uppercase().into()
     }
 
     pub fn str_to_lowercase(&self) -> PyExpr {
```

### Comparing `polars_u64_idx-0.17.6/src/lazy/meta.rs` & `polars_u64_idx-0.17.7/src/lazy/meta.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/src/lazy/mod.rs` & `polars_u64_idx-0.17.7/src/lazy/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/src/lib.rs` & `polars_u64_idx-0.17.7/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/src/npy.rs` & `polars_u64_idx-0.17.7/src/npy.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/src/object.rs` & `polars_u64_idx-0.17.7/src/object.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/src/series.rs` & `polars_u64_idx-0.17.7/src/series.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/src/set.rs` & `polars_u64_idx-0.17.7/src/set.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/src/sql.rs` & `polars_u64_idx-0.17.7/src/sql.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/src/utils.rs` & `polars_u64_idx-0.17.7/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/README.md` & `polars_u64_idx-0.17.7/tests/README.md`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/benchmark/groupby-datagen.R` & `polars_u64_idx-0.17.7/tests/benchmark/groupby-datagen.R`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/benchmark/run_h2oai_benchmark.py` & `polars_u64_idx-0.17.7/tests/benchmark/run_h2oai_benchmark.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/benchmark/test_release.py` & `polars_u64_idx-0.17.7/tests/benchmark/test_release.py`

 * *Files 16% similar despite different names*

```diff
@@ -181,7 +181,33 @@
     assert df.with_columns(
         c=pl.when(pl.lit(nulls)).then(None).otherwise(pl.col("c"))
     ).groupby("idx").agg(aggs).sum().to_dict(False) == {
         "idx": [107583],
         "c_min": [133],
         "c_max": [276],
     }
+
+
+def test_categorical_vs_str_groupby() -> None:
+    # this triggers the perfect hash table
+    s = pl.Series("a", np.random.randint(0, 50, 100))
+    s_with_nulls = pl.select(
+        pl.when(s < 3).then(None).otherwise(s).alias("a")
+    ).to_series()
+
+    for s_ in [s, s_with_nulls]:
+        s_ = s_.cast(str)
+        cat_out = (
+            s_.cast(pl.Categorical)
+            .to_frame("a")
+            .groupby("a")
+            .agg(pl.first().alias("first"))
+        )
+
+        str_out = s_.to_frame("a").groupby("a").agg(pl.first().alias("first"))
+        cat_out.with_columns(pl.col("a").cast(str))
+        assert_frame_equal(
+            cat_out.with_columns(
+                pl.col("a").cast(str), pl.col("first").cast(pl.List(str))
+            ).sort("a"),
+            str_out.sort("a"),
+        )
```

### Comparing `polars_u64_idx-0.17.6/tests/docs/run_doctest.py` & `polars_u64_idx-0.17.7/tests/docs/run_doctest.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/parametric/conftest.py` & `polars_u64_idx-0.17.7/tests/parametric/conftest.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/parametric/test_dataframe.py` & `polars_u64_idx-0.17.7/tests/parametric/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/parametric/test_lazyframe.py` & `polars_u64_idx-0.17.7/tests/parametric/test_lazyframe.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/parametric/test_series.py` & `polars_u64_idx-0.17.7/tests/parametric/test_series.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -------------------------------------------------
 # Validate Series behaviour with parametric tests
 # -------------------------------------------------
 from __future__ import annotations
 
+# from decimal import Decimal as D
 from typing import no_type_check
 
 import numpy as np
 from hypothesis import given, settings
 from hypothesis.strategies import booleans, floats, sampled_from
 from numpy.testing import assert_array_equal
 
@@ -91,35 +92,31 @@
 
             # var:
             ewm_var_pl = s.ewm_var(bias=bias, **pl_params).fill_nan(None)
             ewm_var_pd = pl.Series(p.ewm(**pd_params).var(bias=bias))
             assert_series_equal(ewm_var_pl, ewm_var_pd, atol=1e-07)
 
 
-@given(
-    srs=series(max_size=10, dtype=pl.Int64),
-    start=sampled_from([-5, -4, -3, -2, -1, None, 0, 1, 2, 3, 4, 5]),
-    stop=sampled_from([-5, -4, -3, -2, -1, None, 0, 1, 2, 3, 4, 5]),
-    step=sampled_from([-5, -4, -3, -2, -1, None, 1, 2, 3, 4, 5]),
-)
-@settings(max_examples=500)
-def test_series_slice(
-    srs: pl.Series,
-    start: int | None,
-    stop: int | None,
-    step: int | None,
-) -> None:
-    py_data = srs.to_list()
-
-    s = slice(start, stop, step)
-    sliced_py_data = py_data[s]
-    sliced_pl_data = srs[s].to_list()
-
-    assert sliced_py_data == sliced_pl_data, f"slice [{start}:{stop}:{step}] failed"
-    assert_series_equal(srs, srs, check_exact=True)
+# TODO: once Decimal is a little further along, start actively probing it
+# @given(
+#     s=series(max_size=10, dtype=pl.Decimal, null_probability=0.1),
+# )
+# def test_series_decimal(
+#     s: pl.Series,
+# ) -> None:
+#     with pl.Config(activate_decimals=True):
+#         assert s.dtype == pl.Decimal
+#         assert s.to_list() == list(s)
+#
+#         s_div = s / D(123)
+#         s_mul = s * D(123)
+#         s_sub = s - D(123)
+#         s_add = s - D(123)
+#
+# etc...
 
 
 @given(
     s=series(min_size=1, max_size=10, dtype=pl.Datetime),
 )
 def test_series_datetime_timeunits(
     s: pl.Series,
@@ -160,14 +157,37 @@
         if isinstance(us, int)
     ):
         for ns, us in zip(s.dt.nanoseconds(), micros):
             assert ns == (us * 1000)
 
 
 @given(
+    srs=series(max_size=10, dtype=pl.Int64),
+    start=sampled_from([-5, -4, -3, -2, -1, None, 0, 1, 2, 3, 4, 5]),
+    stop=sampled_from([-5, -4, -3, -2, -1, None, 0, 1, 2, 3, 4, 5]),
+    step=sampled_from([-5, -4, -3, -2, -1, None, 1, 2, 3, 4, 5]),
+)
+@settings(max_examples=500)
+def test_series_slice(
+    srs: pl.Series,
+    start: int | None,
+    stop: int | None,
+    step: int | None,
+) -> None:
+    py_data = srs.to_list()
+
+    s = slice(start, stop, step)
+    sliced_py_data = py_data[s]
+    sliced_pl_data = srs[s].to_list()
+
+    assert sliced_py_data == sliced_pl_data, f"slice [{start}:{stop}:{step}] failed"
+    assert_series_equal(srs, srs, check_exact=True)
+
+
+@given(
     s=series(min_size=1, max_size=10, excluded_dtypes=[pl.Categorical]).filter(
         lambda x: (
             getattr(x.dtype, "time_unit", None) in (None, "us", "ns")
             and (x.dtype != pl.Utf8 or not x.str.contains("\x00").any())
         )
     ),
 )
```

### Comparing `polars_u64_idx-0.17.6/tests/parametric/test_testing.py` & `polars_u64_idx-0.17.7/tests/parametric/test_testing.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/conftest.py` & `polars_u64_idx-0.17.7/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/datatypes/test_bool.py` & `polars_u64_idx-0.17.7/tests/unit/datatypes/test_bool.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/datatypes/test_categorical.py` & `polars_u64_idx-0.17.7/tests/unit/datatypes/test_categorical.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/datatypes/test_decimal.py` & `polars_u64_idx-0.17.7/tests/unit/datatypes/test_decimal.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/datatypes/test_list.py` & `polars_u64_idx-0.17.7/tests/unit/datatypes/test_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -508,14 +508,21 @@
         pl.select(pl.struct(pl.Series("a", [date(2001, 1, 1)])).implode())
         .to_series()
         .new_from_index(0, 1)
     )
     assert s.dtype == pl.List(pl.Struct([pl.Field("a", pl.Date)]))
     assert s.to_list() == [[{"a": date(2001, 1, 1)}]]
 
+    # empty new_from_index # 8420
+    dtype = pl.List(pl.Struct({"c": pl.Boolean}))
+    s = pl.Series("b", values=[[]], dtype=dtype)
+    s = s.new_from_index(0, 2)
+    assert s.dtype == dtype
+    assert s.to_list() == [[], []]
+
 
 def test_list_recursive_time_unit_cast() -> None:
     values = [[datetime(2000, 1, 1, 0, 0, 0)]]
     dtype = pl.List(pl.Datetime("ns"))
     s = pl.Series(values)
     out = s.cast(dtype)
     assert out.dtype == dtype
```

### Comparing `polars_u64_idx-0.17.6/tests/unit/datatypes/test_object.py` & `polars_u64_idx-0.17.7/tests/unit/datatypes/test_object.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/datatypes/test_struct.py` & `polars_u64_idx-0.17.7/tests/unit/datatypes/test_struct.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/datatypes/test_temporal.py` & `polars_u64_idx-0.17.7/tests/unit/datatypes/test_temporal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1920,36 +1920,14 @@
 ) -> None:
     ts = pl.Series(["2020-01-01"]).str.strptime(pl.Datetime(time_unit))
     result = ts.dt.replace_time_zone(from_tz).dt.replace_time_zone(to_tz).item()
     expected = datetime(2020, 1, 1, 0, 0, tzinfo=tzinfo)
     assert result == expected
 
 
-def test_strptime_subseconds_datetime() -> None:
-    with pytest.raises(ValueError, match="not supported"):
-        pl.Series(["2023-02-05T05:10:10.074000"]).str.strptime(
-            pl.Datetime, "%Y-%m-%dT%H:%M:%S.%f"
-        )
-    result = (
-        pl.Series(["2023-02-05T05:10:10.074000"])
-        .str.strptime(pl.Datetime, "%Y-%m-%dT%H:%M:%S%.f")
-        .item()
-    )
-    expected = datetime(2023, 2, 5, 5, 10, 10, 74000)
-    assert result == expected
-
-
-def test_strptime_subseconds_time() -> None:
-    with pytest.raises(ValueError, match="not supported"):
-        pl.Series(["05:10:10.074000"]).str.strptime(pl.Time, "%H:%M:%S.%f")
-    result = pl.Series(["05:10:10.074000"]).str.strptime(pl.Time, "%H:%M:%S%.f").item()
-    expected = time(5, 10, 10, 74000)
-    assert result == expected
-
-
 def test_strptime_with_tz() -> None:
     result = (
         pl.Series(["2020-01-01 03:00:00"])
         .str.strptime(pl.Datetime("us", "Africa/Monrovia"))
         .item()
     )
     assert result == datetime(2020, 1, 1, 3, tzinfo=ZoneInfo(key="Africa/Monrovia"))
```

### Comparing `polars_u64_idx-0.17.6/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json` & `polars_u64_idx-0.17.7/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json` & `polars_u64_idx-0.17.7/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet` & `polars_u64_idx-0.17.7/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet` & `polars_u64_idx-0.17.7/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/io/files/example.xlsx` & `polars_u64_idx-0.17.7/tests/unit/io/files/example.xlsx`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/io/files/foods1.ipc` & `polars_u64_idx-0.17.7/tests/unit/io/files/foods1.ipc`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/io/files/foods1.ndjson` & `polars_u64_idx-0.17.7/tests/unit/io/files/foods1.ndjson`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/io/files/foods1.parquet` & `polars_u64_idx-0.17.7/tests/unit/io/files/foods1.parquet`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/io/files/foods2.ipc` & `polars_u64_idx-0.17.7/tests/unit/io/files/foods2.ipc`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/io/files/foods2.ndjson` & `polars_u64_idx-0.17.7/tests/unit/io/files/foods2.ndjson`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/io/files/foods2.parquet` & `polars_u64_idx-0.17.7/tests/unit/io/files/foods2.parquet`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/io/files/small.parquet` & `polars_u64_idx-0.17.7/tests/unit/io/files/small.parquet`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/io/test_avro.py` & `polars_u64_idx-0.17.7/tests/unit/io/test_avro.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/io/test_csv.py` & `polars_u64_idx-0.17.7/tests/unit/io/test_csv.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/io/test_database.py` & `polars_u64_idx-0.17.7/tests/unit/io/test_database.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/io/test_delta.py` & `polars_u64_idx-0.17.7/tests/unit/io/test_delta.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/io/test_excel.py` & `polars_u64_idx-0.17.7/tests/unit/io/test_excel.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/io/test_ipc.py` & `polars_u64_idx-0.17.7/tests/unit/io/test_ipc.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/io/test_json.py` & `polars_u64_idx-0.17.7/tests/unit/io/test_json.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/io/test_lazy_csv.py` & `polars_u64_idx-0.17.7/tests/unit/io/test_lazy_csv.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/io/test_lazy_ipc.py` & `polars_u64_idx-0.17.7/tests/unit/io/test_lazy_ipc.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/io/test_lazy_json.py` & `polars_u64_idx-0.17.7/tests/unit/io/test_lazy_json.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/io/test_lazy_parquet.py` & `polars_u64_idx-0.17.7/tests/unit/io/test_lazy_parquet.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/io/test_other.py` & `polars_u64_idx-0.17.7/tests/unit/io/test_other.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/io/test_parquet.py` & `polars_u64_idx-0.17.7/tests/unit/io/test_parquet.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/io/test_pickle.py` & `polars_u64_idx-0.17.7/tests/unit/io/test_pickle.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/io/test_pyarrow_dataset.py` & `polars_u64_idx-0.17.7/tests/unit/io/test_pyarrow_dataset.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/namespaces/test_binary.py` & `polars_u64_idx-0.17.7/tests/unit/namespaces/test_binary.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/namespaces/test_categorical.py` & `polars_u64_idx-0.17.7/tests/unit/namespaces/test_categorical.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/namespaces/test_datetime.py` & `polars_u64_idx-0.17.7/tests/unit/namespaces/test_datetime.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/namespaces/test_list.py` & `polars_u64_idx-0.17.7/tests/unit/namespaces/test_list.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/namespaces/test_meta.py` & `polars_u64_idx-0.17.7/tests/unit/namespaces/test_meta.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/namespaces/test_string.py` & `polars_u64_idx-0.17.7/tests/unit/namespaces/test_string.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/namespaces/test_strptime.py` & `polars_u64_idx-0.17.7/tests/unit/namespaces/test_strptime.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Module for testing ``.str.strptime`` of the string namespace.
 
 This method gets its own module due to its complexity.
 """
 from __future__ import annotations
 
 import sys
-from datetime import date, datetime, timedelta, timezone
+from datetime import date, datetime, time, timedelta, timezone
 from typing import TYPE_CHECKING
 
 import pytest
 
 import polars as pl
 from polars.exceptions import ArrowError, ComputeError
 from polars.testing import assert_series_equal
@@ -455,7 +455,44 @@
         ),
     ), pytest.warns(
         DeprecationWarning,
         match="`tz_aware` is now auto-inferred from `format` and will be removed "
         "in a future version. You can safely drop this argument.",
     ):
         pl.Series(["2020-01-01"]).str.strptime(pl.Datetime, tz_aware=True)
+
+
+@pytest.mark.parametrize(
+    ("data", "format", "expected"),
+    [
+        (
+            "2023-02-05T05:10:10.074000",
+            "%Y-%m-%dT%H:%M:%S%.f",
+            datetime(2023, 2, 5, 5, 10, 10, 74000),
+        ),
+    ],
+)
+def test_strptime_subseconds_datetime(data: str, format: str, expected: time) -> None:
+    s = pl.Series([data])
+    result = s.str.strptime(pl.Datetime, format).item()
+    assert result == expected
+
+
+@pytest.mark.parametrize(
+    ("data", "format", "expected"),
+    [
+        ("05:10:10.074000", "%H:%M:%S%.f", time(5, 10, 10, 74000)),
+        ("05:10:10.074000", "%T%.6f", time(5, 10, 10, 74000)),
+        ("05:10:10.074000", "%H:%M:%S%.3f", time(5, 10, 10, 74000)),
+    ],
+)
+def test_strptime_subseconds_time(data: str, format: str, expected: time) -> None:
+    s = pl.Series([data])
+    result = s.str.strptime(pl.Time, format).item()
+    assert result == expected
+
+
+def test_strptime_format_warning() -> None:
+    s = pl.Series(["05:10:10.074000"])
+    with pytest.warns(pl.ChronoFormatWarning, match=".%f"):
+        result = s.str.strptime(pl.Time, "%H:%M:%S.%f").item()
+    assert result == time(5, 10, 10, 74)
```

### Comparing `polars_u64_idx-0.17.6/tests/unit/namespaces/test_struct.py` & `polars_u64_idx-0.17.7/tests/unit/namespaces/test_struct.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/operations/test_aggregations.py` & `polars_u64_idx-0.17.7/tests/unit/operations/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/operations/test_apply.py` & `polars_u64_idx-0.17.7/tests/unit/operations/test_apply.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/operations/test_arithmetic.py` & `polars_u64_idx-0.17.7/tests/unit/operations/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/operations/test_comparison.py` & `polars_u64_idx-0.17.7/tests/unit/operations/test_comparison.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/operations/test_drop.py` & `polars_u64_idx-0.17.7/tests/unit/operations/test_drop.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/operations/test_explode.py` & `polars_u64_idx-0.17.7/tests/unit/operations/test_explode.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/operations/test_filter.py` & `polars_u64_idx-0.17.7/tests/unit/operations/test_filter.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/operations/test_folds.py` & `polars_u64_idx-0.17.7/tests/unit/operations/test_folds.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/operations/test_groupby.py` & `polars_u64_idx-0.17.7/tests/unit/operations/test_groupby.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/operations/test_is_in.py` & `polars_u64_idx-0.17.7/tests/unit/operations/test_is_in.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/operations/test_join.py` & `polars_u64_idx-0.17.7/tests/unit/operations/test_join.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/operations/test_join_asof.py` & `polars_u64_idx-0.17.7/tests/unit/operations/test_join_asof.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/operations/test_melt.py` & `polars_u64_idx-0.17.7/tests/unit/operations/test_melt.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/operations/test_pivot.py` & `polars_u64_idx-0.17.7/tests/unit/operations/test_pivot.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/operations/test_rolling.py` & `polars_u64_idx-0.17.7/tests/unit/operations/test_rolling.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/operations/test_sort.py` & `polars_u64_idx-0.17.7/tests/unit/operations/test_sort.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/operations/test_statistics.py` & `polars_u64_idx-0.17.7/tests/unit/operations/test_statistics.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/operations/test_transpose.py` & `polars_u64_idx-0.17.7/tests/unit/operations/test_transpose.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/operations/test_unique.py` & `polars_u64_idx-0.17.7/tests/unit/operations/test_unique.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/operations/test_window.py` & `polars_u64_idx-0.17.7/tests/unit/operations/test_window.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/test_api.py` & `polars_u64_idx-0.17.7/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/test_arity.py` & `polars_u64_idx-0.17.7/tests/unit/test_arity.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/test_cfg.py` & `polars_u64_idx-0.17.7/tests/unit/test_cfg.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/test_constructors.py` & `polars_u64_idx-0.17.7/tests/unit/test_constructors.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/test_cse.py` & `polars_u64_idx-0.17.7/tests/unit/test_cse.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/test_datatypes.py` & `polars_u64_idx-0.17.7/tests/unit/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/test_df.py` & `polars_u64_idx-0.17.7/tests/unit/test_df.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/test_empty.py` & `polars_u64_idx-0.17.7/tests/unit/test_empty.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/test_errors.py` & `polars_u64_idx-0.17.7/tests/unit/test_errors.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/test_expr_multi_cols.py` & `polars_u64_idx-0.17.7/tests/unit/test_expr_multi_cols.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/test_exprs.py` & `polars_u64_idx-0.17.7/tests/unit/test_exprs.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/test_fmt.py` & `polars_u64_idx-0.17.7/tests/unit/test_fmt.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/test_functions.py` & `polars_u64_idx-0.17.7/tests/unit/test_functions.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/test_interchange.py` & `polars_u64_idx-0.17.7/tests/unit/test_interchange.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/test_interop.py` & `polars_u64_idx-0.17.7/tests/unit/test_interop.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,25 @@
     pl_series_to_numpy_array = pl.Series(name, values, pl_dtype).to_numpy(
         use_pyarrow=use_pyarrow
     )
     numpy_array = np.asarray(values, dtype=np_dtype)
     assert_array_equal(pl_series_to_numpy_array, numpy_array)
 
 
+@pytest.mark.parametrize("use_pyarrow", [True, False])
+@pytest.mark.parametrize("has_null", [True, False])
+@pytest.mark.parametrize("dtype", [pl.Time, pl.Boolean, pl.Utf8])
+@no_type_check
+def test_to_numpy_no_zero_copy(use_pyarrow, has_null, dtype):
+    data = ["a", None] if dtype == pl.Utf8 else [0, None]
+    series = pl.Series(data if has_null else data[:1], dtype=dtype)
+    with pytest.raises(ValueError):
+        series.to_numpy(zero_copy_only=True, use_pyarrow=use_pyarrow)
+
+
 def test_from_pandas() -> None:
     df = pd.DataFrame(
         {
             "bools": [False, True, False],
             "bools_nulls": [None, True, False],
             "int": [1, 2, 3],
             "int_nulls": [1, None, 3],
@@ -737,18 +748,18 @@
     val = [[b"63A0B1C66575DD5708E1EB2B"]]
     arrow_array = pa.array(val, type=pa.list_(pa.binary(24)))
     s = pl.from_arrow(arrow_array)
     assert s.dtype == pl.List(pl.Binary)
     assert s.to_list() == val
 
 
-def test_from_repr() -> None:
+def test_dataframe_from_repr() -> None:
     # round-trip various types
     with pl.StringCache():
-        df = (
+        frame = (
             pl.LazyFrame(
                 {
                     "a": [1, 2, None],
                     "b": [4.5, 5.5, 6.5],
                     "c": ["x", "y", "z"],
                     "d": [True, False, True],
                     "e": [None, "", None],
@@ -764,61 +775,68 @@
             .with_columns(
                 pl.col("c").cast(pl.Categorical),
                 pl.col("h").cast(pl.Datetime("ns")),
             )
             .collect()
         )
 
-        assert df.schema == {
+        assert frame.schema == {
             "a": pl.Int64,
             "b": pl.Float64,
             "c": pl.Categorical,
             "d": pl.Boolean,
             "e": pl.Utf8,
             "f": pl.Date,
             "g": pl.Time,
             "h": pl.Datetime("ns"),
         }
-        assert_frame_equal(df, pl.from_repr(repr(df)))
+        df = cast(pl.DataFrame, pl.from_repr(repr(frame)))
+        assert_frame_equal(frame, df)
 
     # empty frame; confirm schema is inferred
-    df = pl.from_repr(
-        """
+    df = cast(
+        pl.DataFrame,
+        pl.from_repr(
+            """
         ┌─────┬─────┬─────┬─────┬─────┬───────┐
         │ id  ┆ q1  ┆ q2  ┆ q3  ┆ q4  ┆ total │
         │ --- ┆ --- ┆ --- ┆ --- ┆ --- ┆ ---   │
         │ str ┆ i8  ┆ i16 ┆ i32 ┆ i64 ┆ f64   │
         ╞═════╪═════╪═════╪═════╪═════╪═══════╡
         └─────┴─────┴─────┴─────┴─────┴───────┘
         """
+        ),
     )
     assert df.shape == (0, 6)
     assert df.rows() == []
     assert df.schema == {
         "id": pl.Utf8,
         "q1": pl.Int8,
         "q2": pl.Int16,
         "q3": pl.Int32,
         "q4": pl.Int64,
         "total": pl.Float64,
     }
 
-    df = pl.from_repr(
-        """
+    df = cast(
+        pl.DataFrame,
+        pl.from_repr(
+            """
         # >>> Missing cols with old-style ellipsis, nulls, commented out
         # ┌────────────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬──────┐
         # │ dt         ┆ c1  ┆ c2  ┆ c3  ┆ ... ┆ c96 ┆ c97 ┆ c98 ┆ c99  │
         # │ ---        ┆ --- ┆ --- ┆ --- ┆     ┆ --- ┆ --- ┆ --- ┆ ---  │
         # │ date       ┆ i32 ┆ i32 ┆ i32 ┆     ┆ i64 ┆ i64 ┆ i64 ┆ i64  │
         # ╞════════════╪═════╪═════╪═════╪═════╪═════╪═════╪═════╪══════╡
         # │ 2023-03-25 ┆ 1   ┆ 2   ┆ 3   ┆ ... ┆ 96  ┆ 97  ┆ 98  ┆ 99   │
         # │ 1999-12-31 ┆ 3   ┆ 6   ┆ 9   ┆ ... ┆ 288 ┆ 291 ┆ 294 ┆ null │
         # │ null       ┆ 9   ┆ 18  ┆ 27  ┆ ... ┆ 864 ┆ 873 ┆ 882 ┆ 891  │
         # └────────────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┴──────┘
         """
+        ),
     )
     assert df.schema == {
         "dt": pl.Date,
         "c1": pl.Int32,
         "c2": pl.Int32,
         "c3": pl.Int32,
         "c96": pl.Int64,
@@ -828,16 +846,18 @@
     }
     assert df.rows() == [
         (date(2023, 3, 25), 1, 2, 3, 96, 97, 98, 99),
         (date(1999, 12, 31), 3, 6, 9, 288, 291, 294, None),
         (None, 9, 18, 27, 864, 873, 882, 891),
     ]
 
-    df = pl.from_repr(
-        """
+    df = cast(
+        pl.DataFrame,
+        pl.from_repr(
+            """
         In [2]: with pl.Config() as cfg:
            ...:     pl.Config.set_tbl_formatting("UTF8_FULL", rounded_corners=True)
            ...:     print(df)
            ...:
         shape: (1, 5)
         ╭───────────┬────────────┬───┬───────┬────────────────────────────────╮
         │ source_ac ┆ source_cha ┆ … ┆ ident ┆ timestamp                      │
@@ -849,24 +869,85 @@
         ├╌╌╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌╌╌╌┼╌╌╌┼╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌┤
         │ …         ┆ …          ┆ … ┆ …     ┆ …                              │
         ├╌╌╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌╌╌╌┼╌╌╌┼╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌┤
         │ 803065983 ┆ 2055938745 ┆ … ┆ x:y:z ┆ 2023-03-25 12:38:18.050545 JST │
         ╰───────────┴────────────┴───┴───────┴────────────────────────────────╯
         # "Een fluitje van een cent..." :)
         """
+        ),
     )
     assert df.shape == (2, 4)
     assert df.schema == {
         "source_actor_id": pl.Int32,
         "source_channel_id": pl.Int64,
         "ident": pl.Utf8,
         "timestamp": pl.Datetime("us", "Asia/Tokyo"),
     }
 
 
+def test_series_from_repr() -> None:
+    with pl.StringCache():
+        frame = (
+            pl.LazyFrame(
+                {
+                    "a": [1, 2, None],
+                    "b": [4.5, 5.5, 6.5],
+                    "c": ["x", "y", "z"],
+                    "d": [True, False, True],
+                    "e": [None, "", None],
+                    "f": [date(2022, 7, 5), date(2023, 2, 5), date(2023, 8, 5)],
+                    "g": [time(0, 0, 0, 1), time(12, 30, 45), time(23, 59, 59, 999000)],
+                    "h": [
+                        datetime(2022, 7, 5, 10, 30, 45, 4560),
+                        datetime(2023, 10, 12, 20, 3, 8, 11),
+                        None,
+                    ],
+                },
+            )
+            .with_columns(
+                pl.col("c").cast(pl.Categorical),
+                pl.col("h").cast(pl.Datetime("ns")),
+            )
+            .collect()
+        )
+
+        for col in frame.columns:
+            srs = cast(pl.Series, pl.from_repr(repr(frame[col])))
+            assert_series_equal(srs, frame[col])
+
+    srs = cast(
+        pl.Series,
+        pl.from_repr(
+            """
+            Out[3]:
+            shape: (3,)
+            Series: 's' [str]
+            [
+                "a"
+                 …
+                "c"
+            ]
+            """
+        ),
+    )
+    assert_series_equal(srs, pl.Series("s", ["a", "c"]))
+
+    srs = cast(
+        pl.Series,
+        pl.from_repr(
+            """
+            Series: 'flt' [f32]
+            [
+            ]
+            """
+        ),
+    )
+    assert_series_equal(srs, pl.Series("flt", [], dtype=pl.Float32))
+
+
 def test_to_init_repr() -> None:
     # round-trip various types
     with pl.StringCache():
         df = (
             pl.LazyFrame(
                 {
                     "a": [1, 2, None],
```

### Comparing `polars_u64_idx-0.17.6/tests/unit/test_lazy.py` & `polars_u64_idx-0.17.7/tests/unit/test_lazy.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/test_polars_import.py` & `polars_u64_idx-0.17.7/tests/unit/test_polars_import.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/test_predicates.py` & `polars_u64_idx-0.17.7/tests/unit/test_predicates.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/test_projections.py` & `polars_u64_idx-0.17.7/tests/unit/test_projections.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/test_queries.py` & `polars_u64_idx-0.17.7/tests/unit/test_queries.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/test_rows.py` & `polars_u64_idx-0.17.7/tests/unit/test_rows.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/test_schema.py` & `polars_u64_idx-0.17.7/tests/unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/test_serde.py` & `polars_u64_idx-0.17.7/tests/unit/test_serde.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/test_series.py` & `polars_u64_idx-0.17.7/tests/unit/test_series.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/test_sql.py` & `polars_u64_idx-0.17.7/tests/unit/test_sql.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/test_streaming.py` & `polars_u64_idx-0.17.7/tests/unit/test_streaming.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/test_testing.py` & `polars_u64_idx-0.17.7/tests/unit/test_testing.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/tests/unit/utils/test_utils.py` & `polars_u64_idx-0.17.7/tests/unit/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.6/Cargo.lock` & `polars_u64_idx-0.17.7/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1744,15 +1744,15 @@
 checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "py-polars"
-version = "0.17.6"
+version = "0.17.7"
 dependencies = [
  "ahash",
  "built",
  "ciborium",
  "jemallocator",
  "lexical-core",
  "libc",
```

### Comparing `polars_u64_idx-0.17.6/PKG-INFO` & `polars_u64_idx-0.17.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars-u64-idx
-Version: 0.17.6
+Version: 0.17.7
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -13,51 +13,51 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: typing_extensions >= 4.0.1; python_version < '3.11'
-Requires-Dist: xlsx2csv >= 0.8.0; extra == 'xlsx2csv'
 Requires-Dist: numpy >= 1.16.0; extra == 'numpy'
-Requires-Dist: connectorx; extra == 'connectorx'
 Requires-Dist: pyarrow>=7.0.0; extra == 'pandas'
 Requires-Dist: pandas; extra == 'pandas'
 Requires-Dist: deltalake >= 0.8.0; extra == 'deltalake'
+Requires-Dist: fsspec; extra == 'fsspec'
 Requires-Dist: matplotlib; extra == 'matplotlib'
 Requires-Dist: pyarrow>=7.0.0; extra == 'pyarrow'
-Requires-Dist: xlsxwriter; extra == 'xlsxwriter'
+Requires-Dist: xlsx2csv >= 0.8.0; extra == 'xlsx2csv'
+Requires-Dist: connectorx; extra == 'connectorx'
+Requires-Dist: polars[pyarrow,pandas,numpy,fsspec,connectorx,xlsx2csv,deltalake,timezone,matplotlib,sqlalchemy,xlsxwriter]; extra == 'all'
 Requires-Dist: backports.zoneinfo; (python_version < '3.9') and extra == 'timezone'
 Requires-Dist: tzdata; (platform_system == 'Windows') and extra == 'timezone'
-Requires-Dist: polars[pyarrow,pandas,numpy,fsspec,connectorx,xlsx2csv,deltalake,timezone,matplotlib,sqlalchemy,xlsxwriter]; extra == 'all'
 Requires-Dist: sqlalchemy; extra == 'sqlalchemy'
 Requires-Dist: pandas; extra == 'sqlalchemy'
-Requires-Dist: fsspec; extra == 'fsspec'
-Provides-Extra: xlsx2csv
+Requires-Dist: xlsxwriter; extra == 'xlsxwriter'
 Provides-Extra: numpy
-Provides-Extra: connectorx
 Provides-Extra: pandas
 Provides-Extra: deltalake
+Provides-Extra: fsspec
 Provides-Extra: matplotlib
 Provides-Extra: pyarrow
-Provides-Extra: xlsxwriter
-Provides-Extra: timezone
+Provides-Extra: xlsx2csv
+Provides-Extra: connectorx
 Provides-Extra: all
+Provides-Extra: timezone
 Provides-Extra: sqlalchemy
-Provides-Extra: fsspec
+Provides-Extra: xlsxwriter
 License-File: LICENSE
 Summary: Blazingly fast DataFrame library
 Keywords: dataframe,arrow,out-of-core
 Author-email: Ritchie Vink <ritchie46@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Changelog, https://github.com/pola-rs/polars/releases
+Project-URL: Repository, https://github.com/pola-rs/polars
 Project-URL: Homepage, https://www.pola.rs/
 Project-URL: Documentation, https://pola-rs.github.io/polars/py-polars/html/reference/index.html
-Project-URL: Repository, https://github.com/pola-rs/polars
+Project-URL: Changelog, https://github.com/pola-rs/polars/releases
 
 <h1 align="center">
   <img src="https://raw.githubusercontent.com/pola-rs/polars-static/master/logos/polars_github_logo_rect_dark_name.svg">
   <br>
 </h1>
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,41 +1,41 @@
-Metadata-Version: 2.1 Name: polars-u64-idx Version: 0.17.6 Classifier:
+Metadata-Version: 2.1 Name: polars-u64-idx Version: 0.17.7 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Rust Classifier: Topic ::
 Scientific/Engineering Requires-Dist: typing_extensions >= 4.0.1;
-python_version < '3.11' Requires-Dist: xlsx2csv >= 0.8.0; extra == 'xlsx2csv'
-Requires-Dist: numpy >= 1.16.0; extra == 'numpy' Requires-Dist: connectorx;
-extra == 'connectorx' Requires-Dist: pyarrow>=7.0.0; extra == 'pandas'
-Requires-Dist: pandas; extra == 'pandas' Requires-Dist: deltalake >= 0.8.0;
-extra == 'deltalake' Requires-Dist: matplotlib; extra == 'matplotlib' Requires-
-Dist: pyarrow>=7.0.0; extra == 'pyarrow' Requires-Dist: xlsxwriter; extra ==
-'xlsxwriter' Requires-Dist: backports.zoneinfo; (python_version < '3.9') and
-extra == 'timezone' Requires-Dist: tzdata; (platform_system == 'Windows') and
-extra == 'timezone' Requires-Dist: polars
+python_version < '3.11' Requires-Dist: numpy >= 1.16.0; extra == 'numpy'
+Requires-Dist: pyarrow>=7.0.0; extra == 'pandas' Requires-Dist: pandas; extra
+== 'pandas' Requires-Dist: deltalake >= 0.8.0; extra == 'deltalake' Requires-
+Dist: fsspec; extra == 'fsspec' Requires-Dist: matplotlib; extra ==
+'matplotlib' Requires-Dist: pyarrow>=7.0.0; extra == 'pyarrow' Requires-Dist:
+xlsx2csv >= 0.8.0; extra == 'xlsx2csv' Requires-Dist: connectorx; extra ==
+'connectorx' Requires-Dist: polars
 [pyarrow,pandas,numpy,fsspec,connectorx,xlsx2csv,deltalake,timezone,matplotlib,sqlalchemy,xlsxwriter];
-extra == 'all' Requires-Dist: sqlalchemy; extra == 'sqlalchemy' Requires-Dist:
-pandas; extra == 'sqlalchemy' Requires-Dist: fsspec; extra == 'fsspec'
-Provides-Extra: xlsx2csv Provides-Extra: numpy Provides-Extra: connectorx
-Provides-Extra: pandas Provides-Extra: deltalake Provides-Extra: matplotlib
-Provides-Extra: pyarrow Provides-Extra: xlsxwriter Provides-Extra: timezone
-Provides-Extra: all Provides-Extra: sqlalchemy Provides-Extra: fsspec License-
-File: LICENSE Summary: Blazingly fast DataFrame library Keywords:
+extra == 'all' Requires-Dist: backports.zoneinfo; (python_version < '3.9') and
+extra == 'timezone' Requires-Dist: tzdata; (platform_system == 'Windows') and
+extra == 'timezone' Requires-Dist: sqlalchemy; extra == 'sqlalchemy' Requires-
+Dist: pandas; extra == 'sqlalchemy' Requires-Dist: xlsxwriter; extra ==
+'xlsxwriter' Provides-Extra: numpy Provides-Extra: pandas Provides-Extra:
+deltalake Provides-Extra: fsspec Provides-Extra: matplotlib Provides-Extra:
+pyarrow Provides-Extra: xlsx2csv Provides-Extra: connectorx Provides-Extra: all
+Provides-Extra: timezone Provides-Extra: sqlalchemy Provides-Extra: xlsxwriter
+License-File: LICENSE Summary: Blazingly fast DataFrame library Keywords:
 dataframe,arrow,out-of-core Author-email: Ritchie Vink
 gmail.com> Requires-Python: >=3.7 Description-Content-Type: text/markdown;
-charset=UTF-8; variant=GFM Project-URL: Changelog, https://github.com/pola-rs/
-polars/releases Project-URL: Homepage, https://www.pola.rs/ Project-URL:
-Documentation, https://pola-rs.github.io/polars/py-polars/html/reference/
-index.html Project-URL: Repository, https://github.com/pola-rs/polars
+charset=UTF-8; variant=GFM Project-URL: Repository, https://github.com/pola-rs/
+polars Project-URL: Homepage, https://www.pola.rs/ Project-URL: Documentation,
+https://pola-rs.github.io/polars/py-polars/html/reference/index.html Project-
+URL: Changelog, https://github.com/pola-rs/polars/releases
  ****** [https://raw.githubusercontent.com/pola-rs/polars-static/master/logos/
                     polars_github_logo_rect_dark_name.svg]
                                      ******
 [rust_docs] [Build_and_test] [https://img.shields.io/crates/v/polars.svg] [PyPi
  Latest_Release] [NPM_Latest_Release] [R-universe_Latest_Release] [DOI_Latest
                                    Release]
   Documentation: Python - Rust - Node.js - R | StackOverflow: Python - Rust -
```

