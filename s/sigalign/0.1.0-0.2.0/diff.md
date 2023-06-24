# Comparing `tmp/sigalign-0.1.0.tar.gz` & `tmp/sigalign-0.2.0.tar.gz`

## Comparing `sigalign-0.1.0.tar` & `sigalign-0.2.0.tar`

### file list

```diff
@@ -1,84 +1,83 @@
--rw-r--r--   0        0        0      854 1970-01-01 00:00:00.000000 sigalign-0.1.0/local_dependencies/sigalign/Cargo.toml
--rw-r--r--   0      501       20      380 2022-09-16 02:27:33.000000 sigalign-0.1.0/local_dependencies/sigalign/.gitignore
--rw-r--r--   0      501       20      216 2022-02-03 03:50:01.000000 sigalign-0.1.0/local_dependencies/sigalign/benches/benchmark.rs
--rw-r--r--   0      501       20      983 2022-10-19 07:08:18.000000 sigalign-0.1.0/local_dependencies/sigalign/benches/test_data/mod.rs
--rw-r--r--   0      501       20     1008 2022-02-03 03:50:03.000000 sigalign-0.1.0/local_dependencies/sigalign/benches/to_json/mod.rs
--rw-r--r--   0      501       20    37649 2022-11-02 10:06:55.000000 sigalign-0.1.0/local_dependencies/sigalign/src/aligner/algorithm/common_steps/backtrace/backtrace_wave_front.rs
--rw-r--r--   0      501       20     5136 2022-11-03 06:25:02.000000 sigalign-0.1.0/local_dependencies/sigalign/src/aligner/algorithm/common_steps/backtrace/mod.rs
--rw-r--r--   0      501       20      437 2022-11-03 06:25:35.000000 sigalign-0.1.0/local_dependencies/sigalign/src/aligner/algorithm/common_steps/extend/mod.rs
--rw-r--r--   0      501       20    11446 2022-11-06 00:27:35.000000 sigalign-0.1.0/local_dependencies/sigalign/src/aligner/algorithm/common_steps/extend/wave_front/fill.rs
--rw-r--r--   0      501       20     4177 2022-11-04 01:32:54.000000 sigalign-0.1.0/local_dependencies/sigalign/src/aligner/algorithm/common_steps/extend/wave_front/mod.rs
--rw-r--r--   0      501       20     1390 2022-11-02 10:05:24.000000 sigalign-0.1.0/local_dependencies/sigalign/src/aligner/algorithm/common_steps/merging/mod.rs
--rw-r--r--   0      501       20      515 2022-11-03 06:25:50.000000 sigalign-0.1.0/local_dependencies/sigalign/src/aligner/algorithm/common_steps/mod.rs
--rw-r--r--   0      501       20     6099 2022-11-02 10:05:13.000000 sigalign-0.1.0/local_dependencies/sigalign/src/aligner/algorithm/common_steps/pos_table/mod.rs
--rw-r--r--   0      501       20      821 2022-11-02 10:05:02.000000 sigalign-0.1.0/local_dependencies/sigalign/src/aligner/algorithm/common_steps/spare_penalty/mod.rs
--rw-r--r--   0      501       20        0 2022-03-15 06:41:28.000000 sigalign-0.1.0/local_dependencies/sigalign/src/aligner/algorithm/local/backtrace.rs
--rw-r--r--   0      501       20    11650 2022-11-02 10:02:57.000000 sigalign-0.1.0/local_dependencies/sigalign/src/aligner/algorithm/local/extend.rs
--rw-r--r--   0      501       20    15624 2022-11-03 06:26:16.000000 sigalign-0.1.0/local_dependencies/sigalign/src/aligner/algorithm/local/mod.rs
--rw-r--r--   0      501       20     9618 2022-11-02 10:03:31.000000 sigalign-0.1.0/local_dependencies/sigalign/src/aligner/algorithm/local/valid_position_candidate.rs
--rw-r--r--   0      501       20      756 2022-11-03 06:26:43.000000 sigalign-0.1.0/local_dependencies/sigalign/src/aligner/algorithm/mod.rs
--rw-r--r--   0      501       20    37512 2022-11-03 06:26:29.000000 sigalign-0.1.0/local_dependencies/sigalign/src/aligner/algorithm/semi_global/mod.rs
--rw-r--r--   0      501       20     6926 2022-11-02 09:57:10.000000 sigalign-0.1.0/local_dependencies/sigalign/src/aligner/alignment_condition.rs
--rw-r--r--   0      501       20      868 2022-11-02 09:58:58.000000 sigalign-0.1.0/local_dependencies/sigalign/src/aligner/feature/cmp.rs
--rw-r--r--   0      501       20      978 2022-11-02 09:58:47.000000 sigalign-0.1.0/local_dependencies/sigalign/src/aligner/feature/debug.rs
--rw-r--r--   0      501       20     1165 2022-11-02 09:58:36.000000 sigalign-0.1.0/local_dependencies/sigalign/src/aligner/feature/extension_workspace.rs
--rw-r--r--   0      501       20      547 2022-11-02 09:59:57.000000 sigalign-0.1.0/local_dependencies/sigalign/src/aligner/feature/mod.rs
--rw-r--r--   0      501       20     1073 2022-11-02 09:57:24.000000 sigalign-0.1.0/local_dependencies/sigalign/src/aligner/feature/print_status.rs
--rw-r--r--   0      501       20     1386 2022-11-02 09:53:06.000000 sigalign-0.1.0/local_dependencies/sigalign/src/aligner/local.rs
--rw-r--r--   0      501       20     4785 2022-10-20 04:53:15.000000 sigalign-0.1.0/local_dependencies/sigalign/src/aligner/mod.rs
--rw-r--r--   0      501       20     1392 2022-11-02 09:53:20.000000 sigalign-0.1.0/local_dependencies/sigalign/src/aligner/semi_global.rs
--rw-r--r--   0      501       20     4800 2022-11-02 09:53:40.000000 sigalign-0.1.0/local_dependencies/sigalign/src/aligner/wave_front_cache.rs
--rw-r--r--   0      501       20    12915 2022-11-02 10:12:33.000000 sigalign-0.1.0/local_dependencies/sigalign/src/alignment/fasta.rs
--rw-r--r--   0      501       20      744 2022-11-02 10:13:44.000000 sigalign-0.1.0/local_dependencies/sigalign/src/alignment/mod.rs
--rw-r--r--   0      501       20     3505 2022-11-02 10:13:03.000000 sigalign-0.1.0/local_dependencies/sigalign/src/alignment/query.rs
--rw-r--r--   0      501       20        0 2022-01-25 00:16:55.000000 sigalign-0.1.0/local_dependencies/sigalign/src/builder/aligner.rs
--rw-r--r--   0      501       20      484 2022-10-19 06:56:34.000000 sigalign-0.1.0/local_dependencies/sigalign/src/builder/mod.rs
--rw-r--r--   0      501       20     7641 2022-11-02 10:14:57.000000 sigalign-0.1.0/local_dependencies/sigalign/src/builder/reference/mod.rs
--rw-r--r--   0      501       20     1727 2022-11-02 10:14:19.000000 sigalign-0.1.0/local_dependencies/sigalign/src/builder/reference/pattern_finder_option.rs
--rw-r--r--   0      501       20     4455 2022-11-02 10:14:37.000000 sigalign-0.1.0/local_dependencies/sigalign/src/builder/reference/sequence_type_option.rs
--rw-r--r--   0      501       20      734 2022-11-02 09:52:29.000000 sigalign-0.1.0/local_dependencies/sigalign/src/core/conditions.rs
--rw-r--r--   0      501       20      817 2022-11-02 09:52:19.000000 sigalign-0.1.0/local_dependencies/sigalign/src/core/mod.rs
--rw-r--r--   0      501       20     2127 2022-11-03 07:55:11.000000 sigalign-0.1.0/local_dependencies/sigalign/src/core/result.rs
--rw-r--r--   0      501       20     4487 2022-11-14 04:29:02.000000 sigalign-0.1.0/local_dependencies/sigalign/src/lib.rs
--rw-r--r--   0      501       20     1517 2022-11-02 10:19:22.000000 sigalign-0.1.0/local_dependencies/sigalign/src/reference/feature/debug.rs
--rw-r--r--   0      501       20     2213 2022-11-02 10:19:10.000000 sigalign-0.1.0/local_dependencies/sigalign/src/reference/feature/io.rs
--rw-r--r--   0      501       20      381 2022-11-02 10:18:56.000000 sigalign-0.1.0/local_dependencies/sigalign/src/reference/feature/labeling.rs
--rw-r--r--   0      501       20      455 2022-11-02 10:20:06.000000 sigalign-0.1.0/local_dependencies/sigalign/src/reference/feature/mod.rs
--rw-r--r--   0      501       20      795 2022-11-02 10:19:34.000000 sigalign-0.1.0/local_dependencies/sigalign/src/reference/feature/reference_interface.rs
--rw-r--r--   0      501       20      496 2022-11-02 10:19:43.000000 sigalign-0.1.0/local_dependencies/sigalign/src/reference/feature/reverse_complement.rs
--rw-r--r--   0      501       20      919 2022-11-02 10:19:51.000000 sigalign-0.1.0/local_dependencies/sigalign/src/reference/feature/set_search_range.rs
--rw-r--r--   0      501       20     2146 2022-11-02 10:28:41.000000 sigalign-0.1.0/local_dependencies/sigalign/src/reference/mod.rs
--rw-r--r--   0      501       20      335 2022-11-02 10:20:20.000000 sigalign-0.1.0/local_dependencies/sigalign/src/reference/requirement/divide.rs
--rw-r--r--   0      501       20      343 2022-11-02 10:20:29.000000 sigalign-0.1.0/local_dependencies/sigalign/src/reference/requirement/io.rs
--rw-r--r--   0      501       20      134 2022-11-02 10:20:41.000000 sigalign-0.1.0/local_dependencies/sigalign/src/reference/requirement/mod.rs
--rw-r--r--   0      501       20    11132 2022-11-15 00:47:43.000000 sigalign-0.1.0/local_dependencies/sigalign/src/reference/sequence_storage/in_memory/mod.rs
--rw-r--r--   0      501       20     4114 2022-11-02 10:23:40.000000 sigalign-0.1.0/local_dependencies/sigalign/src/reference/sequence_storage/in_memory/reverse_complement.rs
--rw-r--r--   0      501       20     3406 2022-11-02 10:27:12.000000 sigalign-0.1.0/local_dependencies/sigalign/src/reference/sequence_storage/indexed_fasta/mod.rs
--rw-r--r--   0      501       20     2230 2022-11-02 10:26:24.000000 sigalign-0.1.0/local_dependencies/sigalign/src/reference/sequence_storage/indexed_fasta/reverse_complement.rs
--rw-r--r--   0      501       20     2595 2022-11-03 06:27:19.000000 sigalign-0.1.0/local_dependencies/sigalign/src/reference/sequence_storage/mod.rs
--rw-r--r--   0      501       20     2394 2022-11-02 10:22:19.000000 sigalign-0.1.0/local_dependencies/sigalign/src/reference/structure/mod.rs
--rw-r--r--   0      501       20      540 2022-11-02 10:21:22.000000 sigalign-0.1.0/local_dependencies/sigalign/src/reference/structure/pattern_finder/debug.rs
--rw-r--r--   0      501       20     6072 2022-11-03 10:13:13.000000 sigalign-0.1.0/local_dependencies/sigalign/src/reference/structure/pattern_finder.rs
--rw-r--r--   0      501       20     4706 2022-11-02 10:22:12.000000 sigalign-0.1.0/local_dependencies/sigalign/src/reference/structure/sequence_type.rs
--rw-r--r--   0      501       20      552 2022-11-03 09:10:43.000000 sigalign-0.1.0/local_dependencies/sigalign/src/result/fasta_result.rs
--rw-r--r--   0      501       20      708 2022-11-03 07:42:13.000000 sigalign-0.1.0/local_dependencies/sigalign/src/result/labeled_result.rs
--rw-r--r--   0      501       20      627 2022-11-02 10:18:07.000000 sigalign-0.1.0/local_dependencies/sigalign/src/result/mod.rs
--rw-r--r--   0      501       20     1261 2022-11-02 10:17:19.000000 sigalign-0.1.0/local_dependencies/sigalign/src/result/result_counts.rs
--rw-r--r--   0      501       20     4290 2022-11-02 10:17:28.000000 sigalign-0.1.0/local_dependencies/sigalign/src/result/to_json.rs
--rw-r--r--   0      501       20     1728 2022-11-02 10:17:57.000000 sigalign-0.1.0/local_dependencies/sigalign/src/result/to_labeled.rs
--rw-r--r--   0      501       20        0 2022-11-14 04:30:46.000000 sigalign-0.1.0/local_dependencies/sigalign/src/tests/mod.rs
--rw-r--r--   0      501       20      343 2022-01-20 07:58:18.000000 sigalign-0.1.0/local_dependencies/sigalign/src/util/error_encoding.rs
--rw-r--r--   0      501       20     1528 2022-11-02 10:15:28.000000 sigalign-0.1.0/local_dependencies/sigalign/src/util/file_reader.rs
--rw-r--r--   0      501       20      353 2022-11-02 10:31:36.000000 sigalign-0.1.0/local_dependencies/sigalign/src/util/mod.rs
--rw-r--r--   0      501       20      527 2022-09-19 04:22:38.000000 sigalign-0.1.0/local_dependencies/sigalign/src/util/path_reader.rs
--rw-r--r--   0      501       20      418 2022-01-20 07:50:00.000000 sigalign-0.1.0/local_dependencies/sigalign/src/util/sequence_manipulation.rs
--rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 sigalign-0.1.0/Cargo.toml
--rw-r--r--   0      501       20      685 2022-11-15 04:59:09.000000 sigalign-0.1.0/.gitignore
--rw-r--r--   0      501       20     1214 2022-11-15 05:06:32.000000 sigalign-0.1.0/README.md
--rw-r--r--   0      501       20      542 2022-11-15 04:58:27.000000 sigalign-0.1.0/pyproject.toml
--rw-r--r--   0      501       20     2996 2022-11-15 04:15:36.000000 sigalign-0.1.0/src/aligner.rs
--rw-r--r--   0      501       20      578 2022-11-14 07:08:09.000000 sigalign-0.1.0/src/lib.rs
--rw-r--r--   0      501       20     5505 2022-11-15 01:36:24.000000 sigalign-0.1.0/src/reference.rs
--rw-r--r--   0      501       20     3734 2022-11-15 04:22:44.000000 sigalign-0.1.0/src/result.rs
--rw-r--r--   0      501       20     2140 2022-11-15 01:36:46.000000 sigalign-0.1.0/src/sequence_storage.rs
--rw-r--r--   0        0        0     1849 1970-01-01 00:00:00.000000 sigalign-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      935 1970-01-01 00:00:00.000000 sigalign-0.2.0/local_dependencies/sigalign/Cargo.toml
+-rw-r--r--   0      501       20      380 2022-09-16 02:27:33.000000 sigalign-0.2.0/local_dependencies/sigalign/.gitignore
+-rw-r--r--   0      501       20     4877 2023-05-30 06:21:15.000000 sigalign-0.2.0/local_dependencies/sigalign/src/algorithm/anchor/mod.rs
+-rw-r--r--   0      501       20     4220 2023-04-27 01:19:46.000000 sigalign-0.2.0/local_dependencies/sigalign/src/algorithm/anchor/unsafe_marking.rs
+-rw-r--r--   0      501       20     1892 2023-04-27 01:19:46.000000 sigalign-0.2.0/local_dependencies/sigalign/src/algorithm/extension/mod.rs
+-rw-r--r--   0      501       20     5959 2023-05-29 07:01:22.000000 sigalign-0.2.0/local_dependencies/sigalign/src/algorithm/local/extend/mod.rs
+-rw-r--r--   0      501       20     6286 2023-04-27 01:19:46.000000 sigalign-0.2.0/local_dependencies/sigalign/src/algorithm/local/extend/valid_position_candidate.rs
+-rw-r--r--   0      501       20     7949 2023-05-30 10:25:50.000000 sigalign-0.2.0/local_dependencies/sigalign/src/algorithm/local/mod.rs
+-rw-r--r--   0      501       20     3453 2023-05-26 01:45:38.000000 sigalign-0.2.0/local_dependencies/sigalign/src/algorithm/local/spare_penalty.rs
+-rw-r--r--   0      501       20      793 2023-05-29 06:28:11.000000 sigalign-0.2.0/local_dependencies/sigalign/src/algorithm/mod.rs
+-rw-r--r--   0      501       20    22740 2023-04-27 01:19:46.000000 sigalign-0.2.0/local_dependencies/sigalign/src/algorithm/semi_global/extend/backtrace/mod.rs
+-rw-r--r--   0      501       20     8888 2023-05-29 07:01:36.000000 sigalign-0.2.0/local_dependencies/sigalign/src/algorithm/semi_global/extend/mod.rs
+-rw-r--r--   0      501       20     7283 2023-05-30 10:25:53.000000 sigalign-0.2.0/local_dependencies/sigalign/src/algorithm/semi_global/mod.rs
+-rw-r--r--   0      501       20     4090 2023-05-30 11:25:00.000000 sigalign-0.2.0/local_dependencies/sigalign/src/algorithm/spare_penalty/mod.rs
+-rw-r--r--   0      501       20     2368 2023-04-27 01:19:46.000000 sigalign-0.2.0/local_dependencies/sigalign/src/algorithm/traversed/mod.rs
+-rw-r--r--   0      501       20    34715 2023-04-27 01:19:46.000000 sigalign-0.2.0/local_dependencies/sigalign/src/algorithm/wave_front/backtrace.rs
+-rw-r--r--   0      501       20    11789 2023-04-27 01:19:46.000000 sigalign-0.2.0/local_dependencies/sigalign/src/algorithm/wave_front/fill.rs
+-rw-r--r--   0      501       20     1218 2023-04-27 01:19:46.000000 sigalign-0.2.0/local_dependencies/sigalign/src/algorithm/wave_front/match_counter.rs
+-rw-r--r--   0      501       20     4703 2023-04-27 01:19:46.000000 sigalign-0.2.0/local_dependencies/sigalign/src/algorithm/wave_front/mod.rs
+-rw-r--r--   0      501       20     2919 2023-06-24 06:26:06.000000 sigalign-0.2.0/local_dependencies/sigalign/src/aligner/alignments/labeled.rs
+-rw-r--r--   0      501       20     2618 2023-06-24 06:26:12.000000 sigalign-0.2.0/local_dependencies/sigalign/src/aligner/alignments/mod.rs
+-rw-r--r--   0      501       20     2497 2023-06-01 04:44:31.000000 sigalign-0.2.0/local_dependencies/sigalign/src/aligner/allocation_strategy/mod.rs
+-rw-r--r--   0      501       20     1373 2023-06-01 04:49:25.000000 sigalign-0.2.0/local_dependencies/sigalign/src/aligner/debug/mod.rs
+-rw-r--r--   0      501       20     5442 2023-06-21 05:20:34.000000 sigalign-0.2.0/local_dependencies/sigalign/src/aligner/mod.rs
+-rw-r--r--   0      501       20     3507 2023-06-01 04:15:41.000000 sigalign-0.2.0/local_dependencies/sigalign/src/aligner/mode/local/mod.rs
+-rw-r--r--   0      501       20      879 2023-06-01 04:49:13.000000 sigalign-0.2.0/local_dependencies/sigalign/src/aligner/mode/mod.rs
+-rw-r--r--   0      501       20     3133 2023-06-01 04:17:19.000000 sigalign-0.2.0/local_dependencies/sigalign/src/aligner/mode/semi_global/mod.rs
+-rw-r--r--   0      501       20     1423 2023-05-30 10:55:08.000000 sigalign-0.2.0/local_dependencies/sigalign/src/aligner/mode/wave_front_pool/double.rs
+-rw-r--r--   0      501       20      863 2023-05-30 10:55:07.000000 sigalign-0.2.0/local_dependencies/sigalign/src/aligner/mode/wave_front_pool/mod.rs
+-rw-r--r--   0      501       20     1227 2023-05-30 10:55:09.000000 sigalign-0.2.0/local_dependencies/sigalign/src/aligner/mode/wave_front_pool/single.rs
+-rw-r--r--   0      501       20     7359 2023-06-02 02:58:31.000000 sigalign-0.2.0/local_dependencies/sigalign/src/aligner/regulator/mod.rs
+-rw-r--r--   0      501       20     1426 2023-05-30 04:35:43.000000 sigalign-0.2.0/local_dependencies/sigalign/src/core/mod.rs
+-rw-r--r--   0      501       20      589 2023-04-27 01:19:46.000000 sigalign-0.2.0/local_dependencies/sigalign/src/core/regulators.rs
+-rw-r--r--   0      501       20     1483 2023-04-27 01:19:46.000000 sigalign-0.2.0/local_dependencies/sigalign/src/core/sequence_length.rs
+-rw-r--r--   0      501       20     2530 2023-06-21 03:57:58.000000 sigalign-0.2.0/local_dependencies/sigalign/src/lib.rs
+-rw-r--r--   0      501       20      242 2023-06-05 10:09:37.000000 sigalign-0.2.0/local_dependencies/sigalign/src/reference/debug/mod.rs
+-rw-r--r--   0      501       20     1619 2023-06-21 06:18:15.000000 sigalign-0.2.0/local_dependencies/sigalign/src/reference/extensions/io.rs
+-rw-r--r--   0      501       20      687 2023-06-21 06:57:05.000000 sigalign-0.2.0/local_dependencies/sigalign/src/reference/extensions/label.rs
+-rw-r--r--   0      501       20      563 2023-06-21 05:58:34.000000 sigalign-0.2.0/local_dependencies/sigalign/src/reference/extensions/mod.rs
+-rw-r--r--   0      501       20     5303 2023-06-23 05:26:45.000000 sigalign-0.2.0/local_dependencies/sigalign/src/reference/mod.rs
+-rw-r--r--   0      501       20     5853 2023-06-22 06:28:26.000000 sigalign-0.2.0/local_dependencies/sigalign/src/reference/pattern_index/lfi/dynamic.rs
+-rw-r--r--   0      501       20     6569 2023-06-22 06:28:15.000000 sigalign-0.2.0/local_dependencies/sigalign/src/reference/pattern_index/lfi/mod.rs
+-rw-r--r--   0      501       20     2595 2023-06-21 04:01:56.000000 sigalign-0.2.0/local_dependencies/sigalign/src/reference/pattern_index/mod.rs
+-rw-r--r--   0      501       20     1899 2023-06-05 10:26:11.000000 sigalign-0.2.0/local_dependencies/sigalign/src/reference/pattern_index/utils/mod.rs
+-rw-r--r--   0      501       20     1073 2023-06-01 05:57:50.000000 sigalign-0.2.0/local_dependencies/sigalign/src/reference/pattern_search/mod.rs
+-rw-r--r--   0      501       20     1857 2023-06-21 06:54:13.000000 sigalign-0.2.0/local_dependencies/sigalign/src/reference/sequence_storage/in_memory/io.rs
+-rw-r--r--   0      501       20      477 2023-06-21 06:53:52.000000 sigalign-0.2.0/local_dependencies/sigalign/src/reference/sequence_storage/in_memory/label.rs
+-rw-r--r--   0      501       20    10596 2023-06-21 06:54:41.000000 sigalign-0.2.0/local_dependencies/sigalign/src/reference/sequence_storage/in_memory/mod.rs
+-rw-r--r--   0      501       20     4100 2023-06-02 01:47:57.000000 sigalign-0.2.0/local_dependencies/sigalign/src/reference/sequence_storage/in_memory/reverse_complement.rs
+-rw-r--r--   0      501       20     3356 2023-04-27 01:19:46.000000 sigalign-0.2.0/local_dependencies/sigalign/src/reference/sequence_storage/indexed_fasta/mod.rs
+-rw-r--r--   0      501       20     2230 2023-04-27 01:19:46.000000 sigalign-0.2.0/local_dependencies/sigalign/src/reference/sequence_storage/indexed_fasta/reverse_complement.rs
+-rw-r--r--   0      501       20     1255 2023-06-21 03:58:26.000000 sigalign-0.2.0/local_dependencies/sigalign/src/reference/sequence_storage/mod.rs
+-rw-r--r--   0      501       20      532 2023-06-02 05:20:42.000000 sigalign-0.2.0/local_dependencies/sigalign/src/reference/sequence_type/extensions.rs
+-rw-r--r--   0      501       20      643 2023-06-02 05:20:43.000000 sigalign-0.2.0/local_dependencies/sigalign/src/reference/sequence_type/mod.rs
+-rw-r--r--   0      501       20     1283 2023-06-21 04:22:16.000000 sigalign-0.2.0/local_dependencies/sigalign/src/reference/set_search_range/mod.rs
+-rw-r--r--   0      501       20      974 2023-06-21 07:13:07.000000 sigalign-0.2.0/local_dependencies/sigalign/src/results/count_results.rs
+-rw-r--r--   0      501       20     2583 2023-06-19 06:56:42.000000 sigalign-0.2.0/local_dependencies/sigalign/src/results/deduplicate.rs
+-rw-r--r--   0      501       20     2320 2023-06-23 06:19:57.000000 sigalign-0.2.0/local_dependencies/sigalign/src/results/fasta.rs
+-rw-r--r--   0      501       20     1654 2023-06-21 07:08:14.000000 sigalign-0.2.0/local_dependencies/sigalign/src/results/labeled.rs
+-rw-r--r--   0      501       20     2229 2023-06-23 06:18:24.000000 sigalign-0.2.0/local_dependencies/sigalign/src/results/mod.rs
+-rw-r--r--   0      501       20     1950 2023-06-21 07:11:44.000000 sigalign-0.2.0/local_dependencies/sigalign/src/results/to_json.rs
+-rw-r--r--   0      501       20     1539 2023-04-27 01:19:46.000000 sigalign-0.2.0/local_dependencies/sigalign/src/utils/file_reader.rs
+-rw-r--r--   0      501       20      608 2023-05-31 01:13:21.000000 sigalign-0.2.0/local_dependencies/sigalign/src/utils/functions.rs
+-rw-r--r--   0      501       20      307 2023-06-19 06:26:18.000000 sigalign-0.2.0/local_dependencies/sigalign/src/utils/mod.rs
+-rw-r--r--   0      501       20      494 2023-04-27 01:19:46.000000 sigalign-0.2.0/local_dependencies/sigalign/src/utils/path_reader.rs
+-rw-r--r--   0      501       20     2025 2023-06-05 10:25:37.000000 sigalign-0.2.0/local_dependencies/sigalign/src/utils/sequence_manipulation.rs
+-rw-r--r--   0      501       20      856 2023-05-30 06:55:13.000000 sigalign-0.2.0/local_dependencies/sigalign/src/wrapper/aligner/debug.rs
+-rw-r--r--   0      501       20     1677 2023-06-01 06:09:34.000000 sigalign-0.2.0/local_dependencies/sigalign/src/wrapper/aligner/mod.rs
+-rw-r--r--   0      501       20     3299 2023-06-01 06:08:15.000000 sigalign-0.2.0/local_dependencies/sigalign/src/wrapper/aligner/mode.rs
+-rw-r--r--   0      501       20      158 2023-06-22 02:43:10.000000 sigalign-0.2.0/local_dependencies/sigalign/src/wrapper/mod.rs
+-rw-r--r--   0      501       20     1394 2023-06-23 05:27:12.000000 sigalign-0.2.0/local_dependencies/sigalign/src/wrapper/reference/mod.rs
+-rw-r--r--   0        0        0      461 1970-01-01 00:00:00.000000 sigalign-0.2.0/Cargo.toml
+-rw-r--r--   0      501       20      685 2022-11-15 04:59:09.000000 sigalign-0.2.0/.gitignore
+-rw-r--r--   0      501       20     5617 2023-06-24 08:49:09.000000 sigalign-0.2.0/README.md
+-rw-r--r--   0      501       20      716 2023-06-24 12:43:28.000000 sigalign-0.2.0/pyproject.toml
+-rw-r--r--   0      501       20     6332 2023-06-24 07:57:25.000000 sigalign-0.2.0/src/aligner/mod.rs
+-rw-r--r--   0      501       20      386 2023-06-23 15:04:01.000000 sigalign-0.2.0/src/lib.rs
+-rw-r--r--   0      501       20     8094 2023-06-24 07:43:44.000000 sigalign-0.2.0/src/reference/mod.rs
+-rw-r--r--   0      501       20    10450 2023-06-24 07:37:05.000000 sigalign-0.2.0/src/results/mod.rs
+-rw-r--r--   0      501       20     1417 2023-06-24 07:25:32.000000 sigalign-0.2.0/src/results/py_debug.rs
+-rw-r--r--   0      501       20     3623 2023-06-24 07:28:04.000000 sigalign-0.2.0/src/results/to_flat_result.rs
+-rw-r--r--   0      501       20    54971 2023-06-24 08:18:47.000000 sigalign-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0     6338 1970-01-01 00:00:00.000000 sigalign-0.2.0/PKG-INFO
```

### Comparing `sigalign-0.1.0/local_dependencies/sigalign/Cargo.toml` & `sigalign-0.2.0/local_dependencies/sigalign/Cargo.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 [package]
 name = "sigalign"
-version = "0.2.0"
+version = "0.3.0-alpha.1"
 authors = ["baku4 <bahkhun@gamil.com>"]
-edition = "2018"
+edition = "2021"
 description = "Pairwise alignment algorithm using gap-affine penalty for nucleotide and amino-acid sequences."
 readme = "../README.md"
 repository = "https://github.com/baku4/sigalign/"
 license = "MIT"
 keywords = ["alignment", "nucleotide", "bioinformatics", "bio"]
 categories = ["science"]
+resolver = "2"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
-anyhow = "1.0.44"
 num = "0.4.0"
+num-traits = "0.2.15"
+thiserror = "1.0.38"
+ahash = "0.8.0"
 byteorder = "1.4.3"
-lt-fm-index = "0.5.6"
-capwriter = "0.1.1"
-fm-index = "0.1.2"
+bytemuck = "1.13.0"
+capwriter = "0.2.0"
 faimm = "0.3.0"
-serde = "1.0.127"
-serde_json = "1.0.68"
+serde = "1.0.152"
+serde_json = "1.0.93"
 seq_io = "0.3.1"
-bytemuck = "1.12.1"
-ahash = "0.8.0"
 
-[dev-dependencies]
-criterion = "0.3.5"
+[dependencies.lt-fm-index]
+version = "0.7.0-alpha.1"
+[target.'cfg(not(target_arch = "wasm32"))'.dependencies.lt-fm-index]
+version = "0.7.0-alpha.1"
+features = ["fastbwt"]
 
 [features]
 short_key = []
-four_dp = []
-
-[[bench]]
-name = "benchmark"
-harness = false
```

### Comparing `sigalign-0.1.0/local_dependencies/sigalign/src/aligner/algorithm/common_steps/extend/wave_front/fill.rs` & `sigalign-0.2.0/local_dependencies/sigalign/src/algorithm/wave_front/fill.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,141 +1,146 @@
+use crate::core::regulators::{
+	Penalty, 
+};
 use super::{
-	Penalties, 
-    Sequence,
+    WaveFront, WaveEndPoint, WaveFrontScore, Components, Component, BackTraceMarker,
+    MatchCounter, ForwardMatchCounter, ReverseMatchCounter,
 };
-use super::{WaveFront, WaveEndPoint, WaveFrontScore, Components, Component, BackTraceMarker, MatchCounter};
 
 impl WaveFront {
+    #[inline]
     pub fn align_right_to_end_point(
         &mut self,
-        ref_seq: Sequence,
-        qry_seq: Sequence,
-        penalties: &Penalties,
-        spare_penalty: usize,
+        tgt_seq: &[u8],
+        qry_seq: &[u8],
+        penalties: &Penalty,
+        spare_penalty: u32,
     ) {
-        self.align_to_end_point(ref_seq, qry_seq, penalties, spare_penalty, &consecutive_match_forward)
+        self.align_to_end_point::<ForwardMatchCounter>(tgt_seq, qry_seq, penalties, spare_penalty)
     }
+    #[inline]
     pub fn align_left_to_end_point(
         &mut self,
-        ref_seq: Sequence,
-        qry_seq: Sequence,
-        penalties: &Penalties,
-        spare_penalty: usize,
+        tgt_seq: &[u8],
+        qry_seq: &[u8],
+        penalties: &Penalty,
+        spare_penalty: u32,
     ) {
-        self.align_to_end_point(ref_seq, qry_seq, penalties, spare_penalty, &consecutive_match_reverse)
+        self.align_to_end_point::<ReverseMatchCounter>(tgt_seq, qry_seq, penalties, spare_penalty)
     }
-    fn align_to_end_point(
+    #[inline]
+    fn align_to_end_point<C: MatchCounter>(
         &mut self,
-        ref_seq: Sequence,
-        qry_seq: Sequence,
-        penalties: &Penalties,
-        spare_penalty: usize,
-        match_counter: MatchCounter,
+        tgt_seq: &[u8],
+        qry_seq: &[u8],
+        penalties: &Penalty,
+        spare_penalty: u32,
     ) {
-        let ref_len = ref_seq.len();
+        let tgt_len = tgt_seq.len();
         let qry_len = qry_seq.len();
 
-        let first_match_count = match_counter(ref_seq, qry_seq, 0, 0);
+        let first_match_count = C::count_consecutive_match(tgt_seq, qry_seq, 0, 0);
 
         self.wave_front_scores[0].add_first_components(first_match_count);
 
-        if first_match_count as usize >= ref_len || first_match_count as usize >= qry_len {
-            let end_point = WaveEndPoint { score: 0, k: Some(0) };
+        if first_match_count as usize >= tgt_len || first_match_count as usize >= qry_len {
+            let end_point = WaveEndPoint { penalty: 0, k: Some(0) };
             self.end_point = end_point;
         } else {
-            let end_point = self.fill_wave_front_scores_until_end(
-                ref_seq,
+            let end_point = self.fill_wave_front_scores_until_end::<C>(
+                tgt_seq,
                 qry_seq,
                 spare_penalty,
                 penalties,
-                match_counter
             );
             self.end_point = end_point;
         }
     }
-    fn fill_wave_front_scores_until_end(
+    #[inline]
+    fn fill_wave_front_scores_until_end<C: MatchCounter>(
         &mut self,
-        ref_seq: Sequence,
-        qry_seq: Sequence,
-        mut spare_penalty: usize,
-        penalties: &Penalties,
-        match_counter: MatchCounter,
+        tgt_seq: &[u8],
+        qry_seq: &[u8],
+        mut spare_penalty: u32,
+        penalties: &Penalty,
     ) -> WaveEndPoint {
-        if self.wave_front_scores.len() <= spare_penalty {
-            spare_penalty = self.wave_front_scores.len() - 1;
+        if self.wave_front_scores.len() as u32 <= spare_penalty {
+            spare_penalty = (self.wave_front_scores.len() - 1) as u32;
         }
-        for score in 1..=spare_penalty {
-            self.update_components_of_next_wave_front_score(score, penalties);
+        for penalty in 1..=spare_penalty {
+            self.update_components_of_next_wave_front_score(penalty, penalties);
            
-            let optional_last_k = self.wave_front_scores[score].extend_components_until_end(ref_seq, qry_seq, match_counter);
+            let optional_last_k = self.wave_front_scores[penalty as usize].extend_components_until_end::<C>(tgt_seq, qry_seq);
 
             if let Some(last_k) = optional_last_k {
-                return WaveEndPoint { score: score, k: Some(last_k) };
+                return WaveEndPoint { penalty: penalty as usize, k: Some(last_k) };
             }
         }
 
-        WaveEndPoint { score: spare_penalty, k: None }
+        WaveEndPoint { penalty: spare_penalty as usize, k: None }
     }
+    #[inline]
     fn update_components_of_next_wave_front_score(
         &mut self,
-        score: usize,
-        penalties: &Penalties,
+        penalty: u32,
+        penalties: &Penalty,
     ) {
         let mismatch_penalty = &penalties.x;
         let gap_open_penalty = &penalties.o;
         let gap_extend_penalty = &penalties.e;
 
-        let max_k = self.wave_front_scores[score].max_k;
-        let new_components_by_k = &self.wave_front_scores[score].components_by_k;
-        // TODO: Faster init
+        let max_k = self.wave_front_scores[penalty as usize].max_k;
+        let new_components_by_k = &self.wave_front_scores[penalty as usize].components_by_k;
         unsafe {
-            new_components_by_k.iter().for_each(
-                |v| *(v as *const Components as *mut Components) = Components::default()
-            );
+            let ptr = new_components_by_k.as_ptr() as *mut u8;
+            let byte_count = new_components_by_k.len() * std::mem::size_of::<Components>();
+            std::ptr::write_bytes(ptr, 0, byte_count);
         }
 
         // (1) From score: s-o-e
-        if let Some(pre_score) = score.checked_sub(gap_open_penalty + gap_extend_penalty) {
-            let pre_wave_front_score = &self.wave_front_scores[pre_score];
+        if let Some(pre_score) = penalty.checked_sub(gap_open_penalty + gap_extend_penalty) {
+            let pre_wave_front_score = &self.wave_front_scores[pre_score as usize];
             new_components_by_k.iter().enumerate().for_each(|(index_of_k, component)| {
                 let k = index_of_k as i32 - max_k;
                 let new_components_of_k = component as *const Components as *mut Components;
                 // 1. Update I from M & M from I
                 if let Some(pre_components) = pre_wave_front_score.components_of_k_checked(k-1) {
                     let pre_m_component = &pre_components.m;
                     if pre_m_component.bt != BackTraceMarker::Empty {
                         // Update I
                         unsafe {
                             (*new_components_of_k).i = Component {
                                 fr: pre_m_component.fr + 1,
                                 deletion_count: pre_m_component.deletion_count,
                                 bt: BackTraceMarker::FromM,
+                                traversed: false,
                             };
                         }
                     }
                 }
                 // 2. Update D from M & M from D
                 if let Some(pre_components) = pre_wave_front_score.components_of_k_checked(k+1) {
                     let pre_m_component = &pre_components.m;
                     if pre_m_component.bt != BackTraceMarker::Empty {
                         // Update D
                         unsafe {
                             (*new_components_of_k).d = Component {
                                 fr: pre_m_component.fr,
                                 deletion_count: pre_m_component.deletion_count + 1,
                                 bt: BackTraceMarker::FromM,
+                                traversed: false,
                             };
                         }
                     }
                 }
             });
         }
         // (2) From score: s-e
-        if let Some(pre_score) = score.checked_sub(*gap_extend_penalty) {
-            let pre_wave_front_score = &self.wave_front_scores[pre_score];
+        if let Some(pre_score) = penalty.checked_sub(*gap_extend_penalty) {
+            let pre_wave_front_score = &self.wave_front_scores[pre_score as usize];
             new_components_by_k.iter().enumerate().for_each(|(index_of_k, component)| {
                 let k = index_of_k as i32 - max_k;
                 let new_components_of_k = component as *const Components as *mut Components;
                 // 1. Update I from I
                 if let Some(pre_components) = pre_wave_front_score.components_of_k_checked(k-1) {
                     let pre_i_component = &pre_components.i;
 
@@ -143,14 +148,15 @@
                         // Update I
                         unsafe {
                             if (*new_components_of_k).i.bt == BackTraceMarker::Empty || (*new_components_of_k).i.fr < pre_i_component.fr + 1 {
                                 (*new_components_of_k).i = Component {
                                     fr: pre_i_component.fr + 1,
                                     deletion_count: pre_i_component.deletion_count,
                                     bt: BackTraceMarker::FromI,
+                                    traversed: false,
                                 };
                             }
                         };
                     }
                 }
                 // 2. Update D from D
                 if let Some(pre_components) = pre_wave_front_score.components_of_k_checked(k+1) {
@@ -159,115 +165,113 @@
                         // Update D
                         unsafe {
                             if (*new_components_of_k).d.bt == BackTraceMarker::Empty || (*new_components_of_k).d.fr < pre_d_component.fr {
                                 (*new_components_of_k).d = Component {
                                     fr: pre_d_component.fr,
                                     deletion_count: pre_d_component.deletion_count + 1,
                                     bt: BackTraceMarker::FromD,
+                                    traversed: false,
                                 };
                             };
                         }
                     }
                 }
             });
         }
         // (3) From score: s-x
-        if let Some(pre_score) = score.checked_sub(*mismatch_penalty) {
-            let pre_wave_front_score = &self.wave_front_scores[pre_score];
+        if let Some(pre_score) = penalty.checked_sub(*mismatch_penalty) {
+            let pre_wave_front_score = &self.wave_front_scores[pre_score as usize];
             new_components_by_k.iter().enumerate().for_each(|(index_of_k, component)| {
                 let k = index_of_k as i32 - max_k;
                 let new_components_of_k = component as *const Components as *mut Components;
                 // 1. Update M from M
                 let pre_component_index = (pre_wave_front_score.max_k + k) as usize;
 
                 if let Some(pre_components) = pre_wave_front_score.components_by_k.get(pre_component_index) {
                     let pre_m_component = &pre_components.m;
                     // Update M
                     unsafe {
                         (*new_components_of_k).m = Component {
                             fr: pre_m_component.fr + 1,
                             deletion_count: pre_m_component.deletion_count,
                             bt: BackTraceMarker::FromM,
+                            traversed: false,
                         };
                     }
                 }
                 unsafe {
                     // 2. Update M from I
                     if (*new_components_of_k).i.bt != BackTraceMarker::Empty {
                         if (*new_components_of_k).m.bt == BackTraceMarker::Empty || (*new_components_of_k).i.fr >= (*new_components_of_k).m.fr {
                             (*new_components_of_k).m = Component {
                                 fr: (*new_components_of_k).i.fr,
                                 deletion_count: (*new_components_of_k).i.deletion_count,
                                 bt: BackTraceMarker::FromI,
+                                traversed: false,
                             };
                         };
                     }
                     // 3. Update M from D
                     if (*new_components_of_k).d.bt != BackTraceMarker::Empty {
                         if (*new_components_of_k).m.bt == BackTraceMarker::Empty || (*new_components_of_k).d.fr >= (*new_components_of_k).m.fr {
                             (*new_components_of_k).m = Component {
                                 fr: (*new_components_of_k).d.fr,
                                 deletion_count: (*new_components_of_k).d.deletion_count,
                                 bt: BackTraceMarker::FromD,
+                                traversed: false,
                             };
                         };
                     }
                 }
             });
         }
     }
 }
 
 impl WaveFrontScore {
+    #[inline]
     fn add_first_components(&mut self, first_match_count: i32) {
         self.components_by_k = vec![Components::new_start_point(first_match_count)];
     }
-    fn extend_components_until_end(
+    #[inline]
+    fn extend_components_until_end<C: MatchCounter>(
         &mut self,
-        ref_seq: Sequence,
-        qry_seq: Sequence,
-        match_counter: MatchCounter,
+        tgt_seq: &[u8],
+        qry_seq: &[u8],
     ) -> Option<i32> {
         for (components, k) in self.components_by_k.iter_mut().zip(-self.max_k..=self.max_k) {
             let m_component = &mut components.m;
 
             if m_component.bt != BackTraceMarker::Empty {
                 // Extend & update
                 let mut v = (m_component.fr - k) as usize;
                 let mut h = m_component.fr as usize;
-                let match_count = match_counter(ref_seq, qry_seq, v, h);
+                let match_count = C::count_consecutive_match(tgt_seq, qry_seq, v, h);
                 m_component.fr += match_count;
                 // Check exit condition
                 v += match_count as usize;
                 h += match_count as usize;
-                if h >= ref_seq.len() || v >= qry_seq.len() {
+                if h >= tgt_seq.len() || v >= qry_seq.len() {
                     return Some(k);
                 }
             };
         }
         None
     }
 }
 
-//TODO: Apply SIMD
-fn consecutive_match_forward(ref_seq: &[u8], qry_seq: &[u8], v: usize, h: usize) -> i32 {
-    let mut fr_to_add: i32 = 0;
-    for (v1, v2) in qry_seq[v..].iter().zip(ref_seq[h..].iter()) {
-        if *v1 == *v2 {
-            fr_to_add += 1;
-        } else {
-            return fr_to_add
-        }
-    }
-    fr_to_add
-}
-fn consecutive_match_reverse(ref_seq: &[u8], qry_seq: &[u8], v: usize, h: usize) -> i32 {
-    let mut fr_to_add: i32 = 0;
-    for (v1, v2) in qry_seq[..qry_seq.len()-v].iter().rev().zip(ref_seq[..ref_seq.len()-h].iter().rev()) {
-        if *v1 == *v2 {
-            fr_to_add += 1;
-        } else {
-            return fr_to_add
+#[cfg(test)]
+mod tests {
+    use super::*;
+    #[test]
+    fn test_if_the_default_value_of_component_is_filled_with_zero() {
+        let components = Components::default();
+        unsafe {
+            let my_struct_bytes: [u8; std::mem::size_of::<Components>()] = std::mem::transmute(components);
+            let all_zero = my_struct_bytes.iter().all(|&byte| byte == 0);
+    
+            assert!(all_zero, "Not all bytes in the struct are zero");
         }
+
+        println!("All bytes in the struct are zero")
     }
-    fr_to_add
 }
```

### Comparing `sigalign-0.1.0/local_dependencies/sigalign/src/aligner/algorithm/common_steps/pos_table/mod.rs` & `sigalign-0.2.0/local_dependencies/sigalign/src/algorithm/anchor/mod.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,189 +1,147 @@
-use super::{
-    Sequence,
-    ReferenceInterface,
-    Reference, SequenceStorage,
+use crate::core::{
+    BufferedPatternSearch,
 };
-use crate::AHashMap;
+use ahash::AHashMap;
 
-pub type AnchorIndex = (usize, usize);
-
-// Sorted record positions by pattern
-#[derive(Debug, Clone, PartialEq, Eq)]
-pub struct PosTable(pub Vec<Vec<AnchorPosition>>);
+mod unsafe_marking;
+pub use unsafe_marking::{
+    mark_anchor_as_extended,
+    mark_traversed_anchors_as_skipped,
+};
 
+/**
+Anchor Table: Sorted target positions by pattern
+  - 1: Pattern index
+  - 2: Anchor sorted by target position
+If the locations of consecutive patterns are ungapped -> merge to one Anchor
+*/
 #[derive(Debug, Clone, PartialEq, Eq)]
-pub struct AnchorPosition {
-    pub record_position: usize,
-    pub pattern_count: usize,
+pub struct Anchor {
+    pub target_position: u32,
+    pub pattern_count: u32,
+    pub extension_index: u32,
+    pub extended: bool,
+    pub skipped: bool,
 }
-
-impl PosTable {
-    pub fn new_by_record<S: SequenceStorage>(
-        reference: &Reference<S>,
-        query: Sequence,
-        pattern_size: usize,
-    ) -> AHashMap<usize, Self> {
+#[derive(Debug, Clone, PartialEq, Eq)]
+pub struct AnchorTable(
+    pub Vec<Vec<Anchor>>
+);
+pub type AnchorIndex = (u32, u32);
+
+impl AnchorTable {
+    pub fn new_by_target_index<R: BufferedPatternSearch>(
+        reference: &R,
+        query: &[u8],
+        pattern_size: u32,
+    ) -> AHashMap<u32, Self> {
         let qry_len = query.len();
-        let pattern_count = qry_len / pattern_size;
+        let pattern_count = qry_len / pattern_size as usize;
 
-        let mut pos_table_by_record: AHashMap<usize, Self> = AHashMap::new();
+        let mut anchor_table_by_target_index: AHashMap<u32, Self> = AHashMap::new();
 
-        for pattern_index in 0..pattern_count {
-            let qry_pos = pattern_index * pattern_size;
-            let pattern = &query[qry_pos..qry_pos+pattern_size];
+        (0..pattern_count).for_each(|pattern_index| {
+            let qry_pos = pattern_index * pattern_size as usize;
+            let pattern = &query[qry_pos..qry_pos+pattern_size as usize];
             
-            let reference_location = reference.locate(pattern);
+            let pattern_locations = reference.locate(pattern);
 
-            for record_location in reference_location {
-                match pos_table_by_record.get_mut(&record_location.record_index) {
-                    Some(pos_table) => {
-                        pos_table.add_new_positions(pattern_index, record_location.positions)
+            pattern_locations.into_iter().for_each(|pattern_location| {
+                match anchor_table_by_target_index.get_mut(&pattern_location.target_index) {
+                    Some(anchor_table) => {
+                        anchor_table.add_new_positions(
+                            pattern_index,
+                            pattern_location.sorted_positions,
+                        )
                     },
                     None => {
                         let mut new_pos_table = Self::new_empty(pattern_count);
-                        new_pos_table.add_new_positions(pattern_index, record_location.positions);
-                        pos_table_by_record.insert(record_location.record_index, new_pos_table);
+                        new_pos_table.add_new_positions(
+                            pattern_index,
+                            pattern_location.sorted_positions,
+                        );
+                        anchor_table_by_target_index.insert(pattern_location.target_index, new_pos_table);
                     }
                 }
-            }
-        }
+            });
+        });
 
-        pos_table_by_record.iter_mut().for_each(|(_, pos_table)| {
+        anchor_table_by_target_index.iter_mut().for_each(|(_, pos_table)| {
             pos_table.merge_ungapped_anchors(pattern_size);
         });
 
-        pos_table_by_record
-    }
-
-    // For New
-    fn new_empty(pattern_count: usize) -> Self {
-        Self(vec![Vec::new(); pattern_count])
+        anchor_table_by_target_index
     }
     fn add_new_positions(
         &mut self,
         pattern_index: usize,
-        sorted_record_positions: Vec<usize>,
+        sorted_target_positions: Vec<u32>,
     ) {
-        self.0[pattern_index] = AnchorPosition::new_of_vector(sorted_record_positions);
+        self.0[pattern_index] = Anchor::new_vec(sorted_target_positions);
+    }
+    fn new_empty(pattern_count: usize) -> Self {
+        Self(vec![Vec::new(); pattern_count])
     }
-    // For Merge
-    fn merge_ungapped_anchors(&mut self, pattern_size: usize) {
+    fn merge_ungapped_anchors(&mut self, pattern_size: u32) {
         let pattern_count = self.0.len();
 
         for right_index in (1..pattern_count).rev() {
             let (splitted_left, splitted_right) = self.0.split_at_mut(right_index);
 
             let left = &mut splitted_left[right_index-1];
             let right = &mut splitted_right[0];
 
-            AnchorPosition::merge_right_to_left(left, right, pattern_size);
+            Anchor::merge_right_to_left(left, right, pattern_size);
         }
     }
 }
 
-impl AnchorPosition {
-    fn new_of_vector(sorted_record_positions: Vec<usize>) -> Vec<Self> {
-        sorted_record_positions.into_iter().map(|pos| {
+impl Anchor {
+    fn new_vec(sorted_target_positions: Vec<u32>) -> Vec<Self> {
+        sorted_target_positions.into_iter().map(|pos| {
             Self {
-                record_position: pos,
+                target_position: pos,
                 pattern_count: 1,
+                extension_index: 0,
+                extended: false,
+                skipped: false,
             }
         }).collect()
     }
-    fn merge_right_to_left(left_anchor_positions: &mut Vec<Self>, right_anchor_positions: &mut Vec<Self>, pattern_size: usize) {
-        let left_count = left_anchor_positions.len();
-        let mut right_count = right_anchor_positions.len();
+    fn merge_right_to_left(left: &mut Vec<Self>, right: &mut Vec<Self>, pattern_size: u32) {
+        let left_count = left.len();
+        let mut right_count = right.len();
 
         if (left_count == 0) || (right_count == 0) {
             return
         }
 
         let mut left_index = 0;
         let mut right_index = 0;
 
         while (left_index < left_count) && (right_index < right_count) {
-            let left_anchor_position = &mut left_anchor_positions[left_index];
-            let right_anchor_position = &right_anchor_positions[right_index];
-            let right_record_position = right_anchor_position.record_position;
-
-            match (left_anchor_position.record_position + pattern_size).checked_sub(right_record_position) {
-                Some(record_position_gap) => {
-                    if record_position_gap == 0 {
+            let left_anchor_position = &mut left[left_index];
+            let right_anchor_position = &right[right_index];
+            let right_target_position = right_anchor_position.target_position;
+
+            match (left_anchor_position.target_position + pattern_size).checked_sub(right_target_position) {
+                Some(target_position_gap) => {
+                    if target_position_gap == 0 {
                         let right_pattern_count = right_anchor_position.pattern_count;
                         left_anchor_position.pattern_count += right_pattern_count;
 
-                        right_anchor_positions.remove(right_index);
+                        right.remove(right_index);
 
                         left_index += 1;
                         right_count -= 1;
                     } else {
                         right_index += 1;
                     }
                 },
                 None => {
                     left_index += 1;
                 },
             }
         }
     }
 }
-
-
-#[cfg(test)]
-mod tests {
-    use super::*;
-
-    #[test]
-    fn merge_ungapped_anchors_for_pos_table() {
-        let mut pos_table = PosTable::new_empty(3);
-
-        let pattern_size = 10;
-
-        pos_table.add_new_positions(0, vec![20, 50, 80]);
-        pos_table.add_new_positions(1, vec![10, 30, 70, 90]);
-        pos_table.add_new_positions(2, vec![0, 80, 100, 150]);
-
-        pos_table.merge_ungapped_anchors(pattern_size);
-
-        let answer = PosTable(
-            vec![
-                vec![
-                    AnchorPosition {
-                        record_position: 20,
-                        pattern_count: 2,
-                    },
-                    AnchorPosition {
-                        record_position: 50,
-                        pattern_count: 1,
-                    },
-                    AnchorPosition {
-                        record_position: 80,
-                        pattern_count: 3,
-                    },
-                ],
-                vec![
-                    AnchorPosition {
-                        record_position: 10,
-                        pattern_count: 1,
-                    },
-                    AnchorPosition {
-                        record_position: 70,
-                        pattern_count: 2,
-                    },
-                ],
-                vec![
-                    AnchorPosition {
-                        record_position: 0,
-                        pattern_count: 1,
-                    },
-                    AnchorPosition {
-                        record_position: 150,
-                        pattern_count: 1,
-                    },
-                ],
-            ],
-        );
-
-        assert_eq!(pos_table, answer);
-    }
-}
```

### Comparing `sigalign-0.1.0/local_dependencies/sigalign/src/aligner/alignment_condition.rs` & `sigalign-0.2.0/local_dependencies/sigalign/src/aligner/regulator/mod.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,76 +1,64 @@
-use super::{Result, error_msg};
-use super::{
-	Penalties, PRECISION_SCALE, Cutoff, MinPenaltyForPattern,
-	AlignmentResult, AnchorAlignmentResult,
+use crate::core::regulators::{
+    Penalty, PREC_SCALE, Cutoff, MinPenaltyForPattern,
 };
-use num::integer;
-
-const MINIMUM_PATTERN_SIZE: usize = 4;
-
-pub fn calculate_max_pattern_size(cutoff: &Cutoff, min_penalty_for_pattern: &MinPenaltyForPattern) -> usize {
-    let mut n = 1;
-    loop { // TODO: Optimize
-        let upper_bound = ((cutoff.minimum_aligned_length + 4)  as f32 / (2*n)  as f32 - 2_f32).ceil();
-        let lower_bound = ((cutoff.minimum_aligned_length + 4)  as f32 / (2*n + 2)  as f32 - 2_f32).ceil();
-        let max_penalty = (
-            (
-                (
-                    (PRECISION_SCALE * n * (min_penalty_for_pattern.odd + min_penalty_for_pattern.even))
-                )
-                + 4 * cutoff.maximum_penalty_per_scale
-            ) as f32 / (2 * (n+1) * cutoff.maximum_penalty_per_scale) as f32
-        ).ceil() - 2_f32;
-
-        let pattern_size = max_penalty.min(upper_bound);
+use crate::results::{
+    AlignmentResult, AnchorAlignmentResult,
+};
+use thiserror::Error;
+use num::integer::{div_ceil, gcd};
 
-        if pattern_size >= lower_bound {
-            return pattern_size as usize
-        }
-        n += 1;
-    }
+#[derive(Error, Debug)]
+pub enum RegulatorError {
+    #[error("Cutoff is too low to detect the pattern.")]
+    LowCutoff,
+    #[error("Gap extend penalty only allow positive integer.")]
+    InvalidGapExtendPenalty,
+    #[error("Maximum penalty per length only allow positive value.")]
+    InvalidMPpL,
 }
 
 #[derive(Debug, Clone, PartialEq, Eq, PartialOrd, Ord)]
-pub struct AlignmentCondition {
-    pub penalties: Penalties,
+pub struct AlignmentRegulator {
+    pub penalties: Penalty,
     pub cutoff: Cutoff,
     pub min_penalty_for_pattern: MinPenaltyForPattern,
-    pub gcd_for_compression: usize,
-    pub pattern_size: usize,
+    pub gcd_for_compression: u32,
+    pub pattern_size: u32,
 }
 
-impl AlignmentCondition {
+const MINIMUM_PATTERN_SIZE: u32 = 4;
+impl AlignmentRegulator {
     /// Generate new aligner.
     pub fn new(
-        mismatch_penalty: usize,
-        gap_open_penalty: usize,
-        gap_extend_penalty: usize,
-        minimum_aligned_length: usize,
+        mismatch_penalty: u32,
+        gap_open_penalty: u32,
+        gap_extend_penalty: u32,
+        minimum_aligned_length: u32,
         maximum_penalty_per_length: f32,
-    ) -> Result<Self> {
+    ) -> Result<Self, RegulatorError> {
         if gap_extend_penalty == 0 {
-            error_msg!("Gap extend penalty only allow positive integer.");
+            return Err(RegulatorError::InvalidGapExtendPenalty);
         } else if maximum_penalty_per_length <= 0.0 {
-            error_msg!("Maximum penalty per length only allow positive value.");
+            return Err(RegulatorError::InvalidMPpL);
         }
 
-        let penalties = Penalties::new(mismatch_penalty, gap_open_penalty, gap_extend_penalty);
+        let penalties = Penalty::new(mismatch_penalty, gap_open_penalty, gap_extend_penalty);
         let cutoff = Cutoff::new(minimum_aligned_length, maximum_penalty_per_length);
 
         let aligner = Self::new_with_penalties_and_cutoff(penalties, cutoff);
 
         let pattern_size = &aligner.pattern_size;
         if *pattern_size < MINIMUM_PATTERN_SIZE {
-            error_msg!("Auto calculated pattern size({}) should reach at least {}", pattern_size, MINIMUM_PATTERN_SIZE);
+            return Err(RegulatorError::LowCutoff);
         }
 
         Ok(aligner)
     }
-    fn new_with_penalties_and_cutoff(mut penalties: Penalties, mut cutoff: Cutoff) -> Self {
+    fn new_with_penalties_and_cutoff(mut penalties: Penalty, mut cutoff: Cutoff) -> Self {
         let gcd = penalties.gcd_of_penalties();
         penalties.divide_by_gcd(gcd);
         cutoff.divide_by_gcd(gcd);
 
         let min_penalty_for_pattern = MinPenaltyForPattern::new(&penalties);
         let max_pattern_size = calculate_max_pattern_size(&cutoff, &min_penalty_for_pattern);
         
@@ -85,89 +73,124 @@
     pub fn result_of_uncompressed_penalty(&self, mut reference_alignment_result: AlignmentResult) -> AlignmentResult {
         if self.gcd_for_compression != 1 {
             reference_alignment_result.multiply_gcd(self.gcd_for_compression);
         }
         
         reference_alignment_result
     }
-    /// Get penalties
-    pub fn get_penalties(&self) -> [usize; 3] {
-        [
-            self.penalties.x * self.gcd_for_compression,
-            self.penalties.o * self.gcd_for_compression,
-            self.penalties.e * self.gcd_for_compression,
-        ]
-    }
-    /// Get similarity cutoff
-    pub fn get_similarity_cutoff(&self) -> (usize, f32) {
-        (
-            self.cutoff.minimum_aligned_length,
-            (self.cutoff.maximum_penalty_per_scale * self.gcd_for_compression) as f32 / PRECISION_SCALE as f32,
-        )
+    /// Get mismatch penalty
+    pub fn get_mismatch_penalty(&self) -> u32 {
+        self.penalties.x * self.gcd_for_compression
+    }
+    /// Get gap-open penalty
+    pub fn get_gap_open_penalty(&self) -> u32 {
+        self.penalties.o * self.gcd_for_compression
+    }
+    /// Get gap-extend penalty
+    pub fn get_gap_extend_penalty(&self) -> u32 {
+        self.penalties.e * self.gcd_for_compression
+    }
+    /// Get minimum aligned length
+    pub fn get_minimum_aligned_length(&self) -> u32 {
+        self.cutoff.minimum_aligned_length
+    }
+    /// Get maximum penalty per length
+    pub fn get_maximum_penalty_per_length(&self) -> f32 {
+        (self.cutoff.maximum_scaled_penalty_per_length * self.gcd_for_compression) as f32 / PREC_SCALE as f32
     }
     /// Get size of pattern
-    pub fn get_pattern_size(&self) -> usize {
+    pub fn get_pattern_size(&self) -> u32 {
         self.pattern_size
     }
 }
 
+#[inline]
+fn calculate_max_pattern_size(
+    cutoff: &Cutoff,
+    min_penalty_for_pattern: &MinPenaltyForPattern,
+) -> u32 {
+    let mut m = 1;
+    let mut upper_bound = div_ceil(
+        cutoff.minimum_aligned_length + 4,
+        2,
+    ) - 2;
+    loop {
+        let lower_bound = (
+            (cutoff.minimum_aligned_length + 4)  as f32 / (2*m + 2) as f32
+            - 1_f32
+        ).ceil() as u32;
+        let max_penalty = div_ceil(
+            PREC_SCALE * m * (min_penalty_for_pattern.odd + min_penalty_for_pattern.even)
+            + (4 * cutoff.maximum_scaled_penalty_per_length),
+            2 * cutoff.maximum_scaled_penalty_per_length * (m+1)
+        ) - 2;
+
+        let pattern_size = max_penalty.min(upper_bound);
+        if pattern_size >= lower_bound {
+            return pattern_size as u32
+        }
+        m += 1;
+        upper_bound = lower_bound - 1;
+    }
+}
+
 impl AlignmentResult {
-    fn multiply_gcd(&mut self, gcd: usize) {
+    fn multiply_gcd(&mut self, gcd: u32) {
         self.0.iter_mut().for_each(|record_alignment_result| {
             record_alignment_result.alignments.iter_mut().for_each(|alignment_result| {
                 alignment_result.multiply_gcd(gcd);
             })
         })
     }
 }
 
 impl AnchorAlignmentResult {
-    fn multiply_gcd(&mut self, gcd: usize) {
+    fn multiply_gcd(&mut self, gcd: u32) {
         self.penalty *= gcd;
     }
 }
 
-impl Penalties {
-    fn new(mismatch: usize, gap_open: usize, gap_extend: usize) -> Self {
+impl Penalty {
+    fn new(mismatch: u32, gap_open: u32, gap_extend: u32) -> Self {
         Self {
             x: mismatch,
             o: gap_open,
             e: gap_extend,
         }
     }
-    fn gcd_of_penalties(&self) -> usize {
-        integer::gcd(integer::gcd(self.x, self.o), self.e)
+    fn gcd_of_penalties(&self) -> u32 {
+        gcd(gcd(self.x, self.o), self.e)
     }
-    fn divide_by_gcd(&mut self, gcd: usize) {
+    fn divide_by_gcd(&mut self, gcd: u32) {
         self.x /= gcd;
         self.o /= gcd;
         self.e /= gcd;
     }
 }
 
 impl Cutoff {
-    fn new(minimum_aligned_length: usize, maximum_penalty_per_length: f32) -> Self {
-        let maximum_penalty_per_scale = (maximum_penalty_per_length * PRECISION_SCALE as f32) as usize;
+    fn new(minimum_aligned_length: u32, maximum_penalty_per_length: f32) -> Self {
+        let maximum_penalty_per_scale = (maximum_penalty_per_length * PREC_SCALE as f32) as u32;
         Self::new_with_scaled_max_ppl(minimum_aligned_length, maximum_penalty_per_scale)
     }
-    fn new_with_scaled_max_ppl(minimum_aligned_length: usize, maximum_penalty_per_scale: usize) -> Self {
+    fn new_with_scaled_max_ppl(minimum_aligned_length: u32, maximum_penalty_per_scale: u32) -> Self {
         Self {
             minimum_aligned_length,
-            maximum_penalty_per_scale,
+            maximum_scaled_penalty_per_length: maximum_penalty_per_scale,
         }
     }
-    fn divide_by_gcd(&mut self, gcd: usize) {
-        self.maximum_penalty_per_scale /= gcd;
+    fn divide_by_gcd(&mut self, gcd: u32) {
+        self.maximum_scaled_penalty_per_length /= gcd;
     }
 }
 
 impl MinPenaltyForPattern {
-    fn new(penalties: &Penalties) -> Self {
-        let odd: usize;
-        let even: usize;
+    fn new(penalties: &Penalty) -> Self {
+        let odd: u32;
+        let even: u32;
         if penalties.x <= penalties.o + penalties.e {
             odd = penalties.x;
             if penalties.x * 2 <= penalties.o + (penalties.e * 2) {
                 even = penalties.x;
             } else {
                 even = penalties.o + (penalties.e * 2) - penalties.x;
             }
@@ -184,29 +207,29 @@
 
 #[cfg(test)]
 mod tests {
     use super::*;
 
     #[test]
     fn test_gcd_calculation_for_penalties() {
-        let mut penalties = Penalties::new(4, 6, 2);
+        let mut penalties = Penalty::new(4, 6, 2);
         let gcd = penalties.gcd_of_penalties();
         assert_eq!(gcd, 2);
         penalties.divide_by_gcd(gcd);
-        assert_eq!(penalties, Penalties::new(2, 3, 1));
+        assert_eq!(penalties, Penalty::new(2, 3, 1));
 
-        let mut penalties = Penalties::new(4, 5, 3);
+        let mut penalties = Penalty::new(4, 5, 3);
         let gcd = penalties.gcd_of_penalties();
         assert_eq!(gcd, 1);
         penalties.divide_by_gcd(gcd);
-        assert_eq!(penalties, Penalties::new(4, 5, 3));
+        assert_eq!(penalties, Penalty::new(4, 5, 3));
     }
 
     #[allow(dead_code)]
     fn print_calculate_maximum_kmer() {
-        let penalties = Penalties::new(4, 6, 2);
+        let penalties = Penalty::new(4, 6, 2);
         let cutoff = Cutoff::new(50, 0.15);
         let min_penalty_for_pattern = MinPenaltyForPattern::new(&penalties);
         let pattern_size = calculate_max_pattern_size(&cutoff, &min_penalty_for_pattern);
         println!("{}", pattern_size);
     }
 }
```

### Comparing `sigalign-0.1.0/local_dependencies/sigalign/src/core/conditions.rs` & `sigalign-0.2.0/local_dependencies/sigalign/src/core/regulators.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-// Alignment conditions that affect the alignment result
+/// Alignment regulators
+///   - Type is determined by machine's pointer width
+
+pub const PREC_SCALE: u32 = 100_000; // Ensuring accuracy to the fourth decimal place.
+
 #[derive(Debug, Clone, PartialEq, Eq, PartialOrd, Ord)]
-pub struct Penalties {
-    pub x: usize,
-    pub o: usize,
-    pub e: usize,
+pub struct Penalty {
+    pub x: u32,
+    pub o: u32,
+    pub e: u32,
 }
 
-#[cfg(not(feature = "four_dp"))]
-pub const PRECISION_SCALE: usize = 10_000; // Ensuring accuracy to the third decimal place.
-#[cfg(feature = "four_dp")]
-pub const PRECISION_SCALE: usize = 100_000; // Ensuring accuracy to the fourth decimal place.
-
 #[derive(Debug, Clone, PartialEq, Eq, PartialOrd, Ord)]
 pub struct Cutoff {
-    pub minimum_aligned_length: usize,
-    pub maximum_penalty_per_scale: usize,
+    pub minimum_aligned_length: u32,
+    pub maximum_scaled_penalty_per_length: u32,
 }
 
 #[derive(Debug, Clone, PartialEq, Eq, PartialOrd, Ord)]
 pub struct MinPenaltyForPattern {
-    pub odd: usize,
-    pub even: usize,
+    pub odd: u32,
+    pub even: u32,
 }
```

### Comparing `sigalign-0.1.0/local_dependencies/sigalign/src/core/result.rs` & `sigalign-0.2.0/local_dependencies/sigalign/src/results/mod.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,73 @@
-// Result of alignment
-use crate::{Deserialize, Serialize};
+/*!
+Alignment results.
+*/ 
+use serde::{Deserialize, Serialize};
 
 #[derive(Debug, Clone, Serialize, Deserialize)]
 pub struct AlignmentResult(
-    pub Vec<RecordAlignmentResult>
+    pub Vec<TargetAlignmentResult>
 );
 
 #[derive(Debug, Clone)]
 #[derive(Serialize, Deserialize)]
-#[cfg_attr(feature = "short_key", serde(rename = "RecAln"))]
-pub struct RecordAlignmentResult {
+#[cfg_attr(feature = "short_key", serde(rename = "TgtAln"))]
+pub struct TargetAlignmentResult {
     #[cfg_attr(feature = "short_key", serde(rename = "idx"))]
-    pub index: usize,
+    pub index: u32,
     #[cfg_attr(feature = "short_key", serde(rename = "aln"))]
     pub alignments: Vec<AnchorAlignmentResult>,
 }
 
 #[derive(Debug, PartialEq, Eq, Hash, Clone)]
 #[derive(Serialize, Deserialize)]
 #[cfg_attr(feature = "short_key", serde(rename = "AncAln"))]
 pub struct AnchorAlignmentResult {
     #[cfg_attr(feature = "short_key", serde(rename = "pen"))]
-    pub penalty: usize,
+    pub penalty: u32,
     #[cfg_attr(feature = "short_key", serde(rename = "len"))]
-    pub length: usize,
+    pub length: u32,
     #[cfg_attr(feature = "short_key", serde(rename = "pos"))]
     pub position: AlignmentPosition,
     #[cfg_attr(feature = "short_key", serde(rename = "ops"))]
-    pub operations: Vec<AlignmentOperation>,
+    pub operations: Vec<AlignmentOperations>,
 }
 
 #[derive(Debug, PartialEq, Eq, Hash, Clone)]
 #[derive(Serialize, Deserialize)]
 pub struct AlignmentPosition {
-    #[cfg_attr(feature = "short_key", serde(rename = "rec"))]
-    pub record: (usize, usize),
     #[cfg_attr(feature = "short_key", serde(rename = "qry"))]
-    pub query: (usize, usize),
+    pub query: (u32, u32),
+    #[cfg_attr(feature = "short_key", serde(rename = "tgt"))]
+    pub target: (u32, u32),
 }
 
 #[derive(Debug, PartialEq, Eq, Hash, Clone)]
 #[derive(Serialize, Deserialize)]
 #[cfg_attr(feature = "short_key", serde(rename = "Operation"))]
-pub struct AlignmentOperation {
+pub struct AlignmentOperations {
     #[cfg_attr(feature = "short_key", serde(rename = "op"))]
-    pub case: AlignmentCase,
+    pub operation: AlignmentOperation,
     #[cfg_attr(feature = "short_key", serde(rename = "n"))]
     pub count: u32,
 }
 
 #[derive(Debug, PartialEq, Eq, Hash, Clone)]
 #[derive(Serialize, Deserialize)]
-pub enum AlignmentCase {
+pub enum AlignmentOperation {
     #[cfg_attr(feature = "short_key", serde(rename = "M"))]
     Match,
     #[cfg_attr(feature = "short_key", serde(rename = "S"))]
     Subst,
     #[cfg_attr(feature = "short_key", serde(rename = "I"))]
     Insertion,
     #[cfg_attr(feature = "short_key", serde(rename = "D"))]
     Deletion,
 }
+
+pub mod labeled;
+pub mod fasta;
+mod to_json;
+
+// Features
+mod count_results;
+mod deduplicate;
```

### Comparing `sigalign-0.1.0/local_dependencies/sigalign/src/reference/feature/set_search_range.rs` & `sigalign-0.2.0/local_dependencies/sigalign/src/reference/set_search_range/mod.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,41 @@
 use super::{
-    Result, error_msg,
-};
-use super::{
-    Reference, SequenceStorage,
+    Reference,
+    PatternIndex,
+    SequenceStorage,
 };
 
-impl<S> Reference<S> where
+use thiserror::Error;
+/// Defines the potential errors when attempting to set the search range.
+#[derive(Debug, Error)]
+pub enum SetSearchRangeError {
+    #[error("Target index cannot be empty")]
+    EmptyIndexError,
+    #[error("Index cannot be over the total target")]
+    IndexOutOfRangeError,
+}
+
+impl<I, S> Reference<I, S> where
+    I: PatternIndex,
     S: SequenceStorage,
 {
-    pub fn set_search_range(&mut self, mut target_record_index: Vec<u32>) -> Result<()> {
-        target_record_index.sort();
-        let last_record_index = match target_record_index.last() {
+    pub fn get_search_range(&self) -> &[u32] {
+        &self.search_range
+    }
+    pub fn set_search_range(&mut self, mut target_index: Vec<u32>) -> Result<(), SetSearchRangeError> {
+        target_index.sort_unstable();
+        let last_record_index = match target_index.last() {
             Some(v) => v,
-            None => error_msg!("Record index cannot be empty")
+            None => return Err(SetSearchRangeError::EmptyIndexError),
         };
-        let total_record_count = self.sequence_storage.total_record_count() as u32;
-        if total_record_count < *last_record_index {
-            error_msg!("Record index is out of bound")
+        let total_target_count = self.sequence_storage.num_targets() as u32;
+        if total_target_count < *last_record_index {
+            return Err(SetSearchRangeError::IndexOutOfRangeError);
         } else {
-            self.set_search_range_unchecked(target_record_index);
+            self.set_search_range_unchecked(target_index);
             Ok(())
         }
     }
-    pub fn set_search_range_unchecked(&mut self, sorted_inbound_target_record_index: Vec<u32>) {
-        self.target_record_index = sorted_inbound_target_record_index;
+    fn set_search_range_unchecked(&mut self, sorted_target_index: Vec<u32>) {
+        self.search_range = sorted_target_index;
     }
-}
+}
```

### Comparing `sigalign-0.1.0/local_dependencies/sigalign/src/reference/sequence_storage/in_memory/mod.rs` & `sigalign-0.2.0/local_dependencies/sigalign/src/reference/sequence_storage/in_memory/mod.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,316 +1,276 @@
 use super::{
-    Result,
-    SequenceBuffer,
+    SequenceStorage, SequenceBuffer,
+    ConcatenatedSequenceWithBoundaries,
 };
-use super::{
-    SequenceStorage, JoinedSequence,
-    // traits
-    Divisible, Serializable, SizeAware,
+use crate::reference::extensions::{
+    Serialize,
+    EstimateSize,
     LabelStorage,
-    RcStorage,
 };
+use crate::utils::{FastaReader, reverse_complement_of_dna};
 
-use crate::util::{FastaReader, reverse_complement_of_nucleotide_sequence};
-
-use capwriter::{Saveable, Loadable};
-use serde::{Serialize, Deserialize};
+// mod reverse_complement;
+// pub use reverse_complement::InMemoryRcStorage;
 
-mod reverse_complement;
-pub use reverse_complement::InMemoryRcStorage;
 
+// TODO: Debug impl manually
 /// Basic `SequenceStorage` implementation
-#[derive(Debug, Clone, PartialEq, Eq, Serialize, Deserialize)]
+#[derive(Debug, Clone, PartialEq, Eq)]
 pub struct InMemoryStorage {
-    record_count: usize,
-    combined_sequence: Vec<u8>,
+    target_count: usize,
+    concatenated_sequence: Vec<u8>,
     sequence_index: Vec<usize>,
-    combined_label: String,
+    concatenated_label: String,
     label_index: Vec<usize>,
 }
+pub struct InMemoryBuffer {
+    pointer: *const u8,
+    len: usize,
+}
+
+// Sequence Storage
+impl SequenceStorage for InMemoryStorage {
+    type Buffer = InMemoryBuffer;
+
+    fn num_targets(&self) -> u32 {
+        self.target_count as u32
+    }
+    fn get_buffer(&self) -> Self::Buffer {
+        InMemoryBuffer {
+            pointer: self.concatenated_sequence.as_ptr(),
+            len: 0,
+        }
+    }
+    fn fill_buffer(&self, target_index: u32, buffer: &mut Self::Buffer) {
+        let start_index = self.sequence_index[target_index as usize];
+        buffer.pointer = &self.concatenated_sequence[start_index];
+        buffer.len = self.sequence_index[target_index as usize +1] - start_index;
+    }
+    fn get_concatenated_sequence_with_boundaries(&self) -> ConcatenatedSequenceWithBoundaries {
+        ConcatenatedSequenceWithBoundaries {
+            concatenated_sequence: self.concatenated_sequence.to_vec(),
+            boundaries: self.sequence_index.iter().map(|x| *x as u64).collect(),
+        }
+    }
+}
+impl SequenceBuffer for InMemoryBuffer {
+    fn buffered_sequence(&self) -> &[u8] {
+        unsafe { std::slice::from_raw_parts(self.pointer, self.len) }
+    }
+}
 
 impl InMemoryStorage {
     pub fn new() -> Self {
         Self {
-            record_count: 0,
-            combined_sequence: Vec::new(),
+            target_count: 0,
+            concatenated_sequence: Vec::new(),
             sequence_index: vec![0],
-            combined_label: String::new(),
+            concatenated_label: String::new(),
             label_index: vec![0],
         }
     }
-    pub fn add_record(
+    pub fn add_target(
         &mut self,
-        sequence: &[u8],
         label: &str,
+        sequence: &[u8],
     ) {
-        self.record_count += 1;
-        self.combined_sequence.extend_from_slice(sequence);
-        self.sequence_index.push(self.combined_sequence.len());
-        self.combined_label.push_str(label);
-        self.label_index.push(self.combined_label.len());
+        self.target_count += 1;
+        self.concatenated_sequence.extend_from_slice(sequence);
+        self.sequence_index.push(self.concatenated_sequence.len());
+        self.concatenated_label.push_str(label);
+        self.label_index.push(self.concatenated_label.len());
     }
-    pub fn add_fasta_file<P>(&mut self, file_path: P) -> Result<()> where
+    pub fn add_fasta_file<P>(&mut self, file_path: P) -> Result<(), std::io::Error> where
         P: AsRef<std::path::Path> + std::fmt::Debug,
     {
-        let fasta_reader = FastaReader::from_file_path(file_path)?;
+        let fasta_reader = FastaReader::from_path(file_path)?;
         self.add_from_fasta_reader(fasta_reader);
         Ok(())
     }
     pub fn add_fasta_bytes(&mut self, fasta_bytes: &[u8]) {
         let fasta_reader = FastaReader::from_bytes(fasta_bytes);
         self.add_from_fasta_reader(fasta_reader);
     }
     fn add_from_fasta_reader<R>(&mut self, fasta_reader: FastaReader<R>) where
         R: std::io::Read,
     {
         fasta_reader.for_each(|(label, sequence)| {
-            self.add_record(&sequence, &label);
+            self.add_target(&label, &sequence);
         });
     }
     pub fn to_reverse_complement(&self) -> Self {
-        let mut new_combined_sequence: Vec<u8> = Vec::with_capacity(self.combined_sequence.len());
-        (0..self.record_count).for_each(|idx| {
+        let mut new_combined_sequence: Vec<u8> = Vec::with_capacity(self.concatenated_sequence.len());
+        (0..self.target_count).for_each(|idx| {
             let start_idx = self.sequence_index[idx];
             let end_idx = self.sequence_index[idx+1];
-            let org_seq = &self.combined_sequence[start_idx..end_idx];
-            let mut rc_seq = reverse_complement_of_nucleotide_sequence(org_seq);
+            let org_seq = &self.concatenated_sequence[start_idx..end_idx];
+            let mut rc_seq = reverse_complement_of_dna(org_seq);
             new_combined_sequence.append(&mut rc_seq);
         });
 
         Self {
-            record_count: self.record_count,
-            combined_sequence: new_combined_sequence,
+            target_count: self.target_count,
+            concatenated_sequence: new_combined_sequence,
             sequence_index: self.sequence_index.clone(),
-            combined_label: self.combined_label.clone(),
+            concatenated_label: self.concatenated_label.clone(),
             label_index: self.label_index.clone(),
         }
     }
+    pub fn append_reverse_complement(&mut self) {
+        // combined_sequence
+        self.concatenated_sequence.reserve(self.concatenated_sequence.len());
+        (0..self.target_count).for_each(|idx| {
+            let start_idx = self.sequence_index[idx];
+            let end_idx = self.sequence_index[idx+1];
+            let org_seq = &self.concatenated_sequence[start_idx..end_idx];
+            let mut rc_seq = reverse_complement_of_dna(org_seq);
+            self.concatenated_sequence.append(&mut rc_seq);
+        });
+        // sequence_index
+        {
+            self.sequence_index.reserve(self.target_count);
+            let last_seq_idx = *self.sequence_index.last().unwrap();
+            for idx in 1..=self.target_count {
+                let v = self.sequence_index[idx];
+                self.sequence_index.push(v+last_seq_idx);
+            };
+        }
+        // combined_label
+        self.concatenated_label.push_str(&self.concatenated_label.clone());
+        // label_index
+        {
+            self.label_index.reserve(self.target_count);
+            let last_label_idx = *self.label_index.last().unwrap();
+            for idx in 1..=self.target_count {
+                let v = self.label_index[idx];
+                self.label_index.push(v+last_label_idx);
+            };
+        }
+        // record_count
+        self.target_count <<= 1;
+    }
     pub fn merge(&mut self, other: Self) {
         let Self {
-            record_count: other_record_count,
-            combined_sequence: mut other_combined_sequence,
+            target_count: other_record_count,
+            concatenated_sequence: mut other_combined_sequence,
             sequence_index: other_sequence_index,
-            combined_label: other_combined_label,
+            concatenated_label: other_combined_label,
             label_index: other_label_index,
         } = other;
         // record_count
-        self.record_count += other_record_count;
-        // combined_sequence
-        self.combined_sequence.append(&mut other_combined_sequence);
+        self.target_count += other_record_count;
+        // concatenated_sequence
+        self.concatenated_sequence.append(&mut other_combined_sequence);
         // sequence_index
         let last_seq_idx = *self.sequence_index.last().unwrap();
         self.sequence_index.reserve(other_record_count);
         other_sequence_index[1..].iter().for_each(|v| {
             self.sequence_index.push(v+last_seq_idx);
         });
-        // combined_label
-        self.combined_label.push_str(&other_combined_label);
+        // concatenated_label
+        self.concatenated_label.push_str(&other_combined_label);
         // label_index
         let last_label_idx = *self.label_index.last().unwrap();
         self.label_index.reserve(other_record_count);
         other_label_index[1..].iter().for_each(|v| {
             self.label_index.push(v+last_label_idx);
         });
     }
-    pub fn get_sequence_safely(&self, record_index: usize) -> Option<Vec<u8>> {
-        if record_index >= self.record_count {
+    pub fn get_sequence_safely(&self, target_index: u32) -> Option<Vec<u8>> {
+        if target_index as usize >= self.target_count {
             return None
         }
-        
         let mut buffer = self.get_buffer();
-        self.fill_sequence_buffer(record_index, &mut buffer);
-        let seq = buffer.request_sequence().to_vec();
+        self.fill_buffer(target_index, &mut buffer);
+        let seq = buffer.buffered_sequence().to_vec();
         Some(seq)
     }
-    pub fn get_label_safely(&self, record_index: usize) -> Option<String> {
-        if record_index >= self.record_count {
+    pub fn get_label_safely(&self, target_index: u32) -> Option<String> {
+        if target_index as usize >= self.target_count {
             return None
         }
-        
-        Some(self.label_of_record(record_index))
+        Some(self.label_of_target_unchecked(target_index))
     }
 }
 
-pub struct InMemoryBuffer {
-    pointer: *const u8,
-    len: usize,
-}
-
-impl SequenceBuffer for InMemoryBuffer {
-    fn request_sequence(&self) -> &[u8] {
-        unsafe { std::slice::from_raw_parts(self.pointer, self.len) }
-    }
-}
-
-// Sequence Storage
-impl SequenceStorage for InMemoryStorage {
-    type Buffer = InMemoryBuffer;
-
-    fn total_record_count(&self) -> usize {
-        self.record_count
-    }
-    fn get_buffer(&self) -> Self::Buffer {
-        InMemoryBuffer {
-            pointer: self.combined_sequence.as_ptr(),
-            len: 0,
-        }
-    }
-    fn fill_sequence_buffer(&self, record_index: usize, buffer: &mut Self::Buffer) {
-        let start_index = self.sequence_index[record_index];
-        buffer.pointer = &self.combined_sequence[start_index];
-        buffer.len = self.sequence_index[record_index+1] - start_index;
-    }
-    fn get_joined_sequence(&self) -> JoinedSequence {
-        JoinedSequence::new(
-            self.combined_sequence.to_vec(),
-            self.sequence_index.iter().map(|x| *x as u64).collect(),
-        )
-    }
-}
-
-// Label Storage
-impl LabelStorage for InMemoryStorage {
-    fn label_of_record(&self, record_index: usize) -> String {
-        String::from(&self.combined_label[
-            self.label_index[record_index]..self.label_index[record_index+1]
-        ])
-    }
-}
-
-use crate::{EndianType};
-use byteorder::{ReadBytesExt, WriteBytesExt};
-
-// Serializable
-impl Serializable for InMemoryStorage {
-    fn save_to<W>(&self, mut writer: W) -> Result<()> where
-        W: std::io::Write
-    {
-        // 1. Write record_count
-        writer.write_u64::<EndianType>(self.record_count as u64)?;
-        // 2. Write combined_sequence
-        self.combined_sequence.save_to(&mut writer)?;
-        // 3. Write sequence_index
-        self.sequence_index.save_to(&mut writer)?;
-        // 4. Write combined_label
-        let combined_label_byte = self.combined_label.as_bytes();
-        combined_label_byte.save_to(&mut writer)?;
-        // 5. Write label_index
-        self.label_index.save_to(&mut writer)?;
-
-        Ok(())
-    }
-    fn load_from<R>(mut reader: R) -> Result<Self> where
-        R: std::io::Read,
-        Self: Sized,
-    {
-        // 1. Read record_count
-        let record_count = reader.read_u64::<EndianType>()? as usize;
-        // 2. Read combined_sequence
-        let combined_sequence = Vec::load_from(&mut reader)?;
-        // 3. Read sequence_index
-        let sequence_index = Vec::load_from(&mut reader)?;
-        // 4. Read combined_label
-        let combined_label_byte = Vec::<u8>::load_from(&mut reader)?;
-        let combined_label = unsafe {
-            String::from_utf8_unchecked(combined_label_byte)
-        };
-        // 5. Read label_index
-        let label_index = Vec::load_from(&mut reader)?;
-
-        Ok(Self {
-            record_count,
-            combined_sequence,
-            sequence_index,
-            combined_label,
-            label_index,
-        })
-    }
-}
-
-// SizeAware
-impl SizeAware for InMemoryStorage {
-    fn size_of(&self) -> usize {
-        8 // record_count
-        + self.combined_sequence.size_of() // combined_sequence
-        + self.sequence_index.size_of() // sequence_index
-        + self.combined_label.as_bytes().size_of() // combined_label
-        + self.label_index.size_of() // label_index
-    }
-}
-
-// Divisible
-impl Divisible for InMemoryStorage {
-    fn split_by_max_length(self, max_seq_len: usize) -> Result<Vec<Self>> {
-        // Get record index range list
-        let record_index_range_list = self.record_index_range_list_of_max_length(max_seq_len);
-
-        // Split
-        let splitted = self.split_using_record_index_range_list(record_index_range_list);
-
-        Ok(splitted)
-    }
-}
-impl InMemoryStorage {
-    fn record_index_range_list_of_max_length(&self, max_seq_len: usize) -> Vec<(usize, usize)> {
-        let mut record_index_range_list = Vec::new(); // (start index, last index)
-        let mut start_record_index = 0;
-
-        'outer: loop {
-            let mut first_max_over_record_index = start_record_index + 1;
-
-            while self.sequence_index[first_max_over_record_index] - self.sequence_index[start_record_index] <= max_seq_len {
-                first_max_over_record_index += 1;
-                if first_max_over_record_index == self.sequence_index.len() - 1 {
-                    record_index_range_list.push((start_record_index, first_max_over_record_index));
-                    break 'outer;
-                }
-            }
-
-            // accumulated_length > max_length
-            if first_max_over_record_index == start_record_index + 1 { // One record exceed the max length
-                record_index_range_list.push((start_record_index, first_max_over_record_index));
-                start_record_index = first_max_over_record_index;
-            } else {
-                record_index_range_list.push((start_record_index, first_max_over_record_index - 1));
-                start_record_index = first_max_over_record_index - 1;
-            }
-        }
-        record_index_range_list
-    }
-    fn split_using_record_index_range_list(self, record_index_range_list: Vec<(usize, usize)>) -> Vec<Self> {
-        record_index_range_list.into_iter().map(|(start_record_index, last_record_index)| {
-            // record_count
-            let record_count = last_record_index - start_record_index;
-
-            // combined_sequence
-            let sequence_start_index = self.sequence_index[start_record_index];
-            let sequence_end_index = self.sequence_index[last_record_index];
+// Features
+mod io;
+mod label;
+
+
+// // Divisible
+// impl Divide for InMemoryStorage {
+//     fn divide_into(self, max_seq_len: usize) -> Result<Vec<Self>> {
+//         // Get record index range list
+//         let record_index_range_list = self.record_index_range_list_of_max_length(max_seq_len);
+
+//         // Split
+//         let splitted = self.split_using_record_index_range_list(record_index_range_list);
+
+//         Ok(splitted)
+//     }
+// }
+// impl InMemoryStorage {
+//     fn record_index_range_list_of_max_length(&self, max_seq_len: usize) -> Vec<(usize, usize)> {
+//         let mut record_index_range_list = Vec::new(); // (start index, last index)
+//         let mut start_record_index = 0;
+
+//         'outer: loop {
+//             let mut first_max_over_record_index = start_record_index + 1;
+
+//             while self.sequence_index[first_max_over_record_index] - self.sequence_index[start_record_index] <= max_seq_len {
+//                 first_max_over_record_index += 1;
+//                 if first_max_over_record_index == self.sequence_index.len() - 1 {
+//                     record_index_range_list.push((start_record_index, first_max_over_record_index));
+//                     break 'outer;
+//                 }
+//             }
+
+//             // accumulated_length > max_length
+//             if first_max_over_record_index == start_record_index + 1 { // One record exceed the max length
+//                 record_index_range_list.push((start_record_index, first_max_over_record_index));
+//                 start_record_index = first_max_over_record_index;
+//             } else {
+//                 record_index_range_list.push((start_record_index, first_max_over_record_index - 1));
+//                 start_record_index = first_max_over_record_index - 1;
+//             }
+//         }
+//         record_index_range_list
+//     }
+//     fn split_using_record_index_range_list(self, record_index_range_list: Vec<(usize, usize)>) -> Vec<Self> {
+//         record_index_range_list.into_iter().map(|(start_record_index, last_record_index)| {
+//             // record_count
+//             let record_count = last_record_index - start_record_index;
+
+//             // combined_sequence
+//             let sequence_start_index = self.sequence_index[start_record_index];
+//             let sequence_end_index = self.sequence_index[last_record_index];
             
-            let combined_sequence = self.combined_sequence[sequence_start_index..sequence_end_index].to_vec();
+//             let combined_sequence = self.concatenated_sequence[sequence_start_index..sequence_end_index].to_vec();
 
-            // sequence_index
-            let sequence_index: Vec<usize> = self.sequence_index[start_record_index..=last_record_index].iter().map(|v| {
-                v - sequence_start_index
-            }).collect();
-
-            // combined_label
-            let label_start_index = self.label_index[start_record_index];
-            let label_end_index = self.label_index[last_record_index];
-
-            let combined_label = self.combined_label[label_start_index..label_end_index].to_string();
-
-            // label_index
-            let label_index: Vec<usize> = self.label_index[start_record_index..=last_record_index].iter().map(|v| {
-                v - label_start_index
-            }).collect();
-
-            Self {
-                record_count,
-                combined_sequence,
-                sequence_index,
-                combined_label,
-                label_index,
-            }
-        }).collect()
-    }
-}
+//             // sequence_index
+//             let sequence_index: Vec<usize> = self.sequence_index[start_record_index..=last_record_index].iter().map(|v| {
+//                 v - sequence_start_index
+//             }).collect();
+
+//             // combined_label
+//             let label_start_index = self.label_index[start_record_index];
+//             let label_end_index = self.label_index[last_record_index];
+
+//             let combined_label = self.combined_label[label_start_index..label_end_index].to_string();
+
+//             // label_index
+//             let label_index: Vec<usize> = self.label_index[start_record_index..=last_record_index].iter().map(|v| {
+//                 v - label_start_index
+//             }).collect();
+
+//             Self {
+//                 target_count: record_count,
+//                 concatenated_sequence: combined_sequence,
+//                 sequence_index,
+//                 combined_label,
+//                 label_index,
+//             }
+//         }).collect()
+//     }
+// }
```

### Comparing `sigalign-0.1.0/local_dependencies/sigalign/src/reference/sequence_storage/in_memory/reverse_complement.rs` & `sigalign-0.2.0/local_dependencies/sigalign/src/reference/sequence_storage/in_memory/reverse_complement.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 use super::{
     Result,
 };
 use super::{
     SequenceStorage, JoinedSequence,
     // traits
-    Divisible, Serializable, SizeAware,
+    Divide, Serialize, EstimateSize,
     LabelStorage,
     RcStorage,
 };
 
 use super::{InMemoryStorage, InMemoryBuffer};
 
 use crate::util::{FastaReader, reverse_complement_of_nucleotide_sequence};
@@ -76,15 +76,15 @@
 impl LabelStorage for InMemoryRcStorage {
     fn label_of_record(&self, record_index: usize) -> String {
         self.0.label_of_record(record_index)
     }
 }
 
 // Serializable
-impl Serializable for InMemoryRcStorage {
+impl Serialize for InMemoryRcStorage {
     fn save_to<W>(&self, writer: W) -> Result<()> where
         W: std::io::Write
     {
         self.0.save_to(writer)?;
         Ok(())
     }
     fn load_from<R>(reader: R) -> Result<Self> where
@@ -93,23 +93,23 @@
     {
         let in_memory_storage = InMemoryStorage::load_from(reader)?;
         Ok(Self(in_memory_storage))
     }
 }
 
 // SizeAware
-impl SizeAware for InMemoryRcStorage {
+impl EstimateSize for InMemoryRcStorage {
     fn size_of(&self) -> usize {
         self.0.size_of()
     }
 }
 
 // Divisible
-impl Divisible for InMemoryRcStorage {
-    fn split_by_max_length(self, max_seq_len: usize) -> Result<Vec<Self>> {
+impl Divide for InMemoryRcStorage {
+    fn divide_into(self, max_seq_len: usize) -> Result<Vec<Self>> {
         // Get record index range list
         let record_index_range_list = self.0.record_index_range_list_of_max_length(max_seq_len);
 
         // Adjust all range to even number
         let adjusted_record_index_range_list = record_index_range_list.into_iter()
             .filter_map(|(mut v1, mut v2)| {
                 if v1 % 2 == 1 {
```

### Comparing `sigalign-0.1.0/local_dependencies/sigalign/src/reference/sequence_storage/indexed_fasta/mod.rs` & `sigalign-0.2.0/local_dependencies/sigalign/src/reference/sequence_storage/indexed_fasta/mod.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,15 @@
 use super::{
-    Result,
-    SequenceBuffer,
+    SequenceStorage, SequenceBuffer,
+    ConcatenatedSequenceWithBoundaries,
 };
-use super::{
-    SequenceStorage,
-    // Trait
-    Serializable, SizeAware,
-    RcStorage,
-};
-
+use crate::utils::{path_to_byte, byte_to_pathbuf};
 use std::io::{Read, Write};
 use std::path::{Path, PathBuf};
 
-use crate::util::{path_to_byte, byte_to_pathbuf};
-
 use capwriter::{Saveable, Loadable};
 use faimm::IndexedFasta as FaiIndexedFasta;
 
 mod reverse_complement;
 pub use reverse_complement::IndexedFastaRcStorage;
 
 /// Basic `SequenceStorage` implementation
@@ -83,15 +75,15 @@
     }
 }
 
 use crate::{EndianType};
 use byteorder::{ReadBytesExt, WriteBytesExt};
 
 // Serializable
-impl Serializable for IndexedFastaStorage {
+impl Serialize for IndexedFastaStorage {
     fn save_to<W>(&self, mut writer: W) -> Result<()> where W: Write {
         // 1. Write total_record_count
         writer.write_u64::<EndianType>(self.total_record_count as u64)?;
         // 2. Write fasta_file_path_buf
         let byte = path_to_byte(&self.fasta_file_path_buf)?;
         byte.save_to(writer)?;
 
@@ -108,13 +100,13 @@
             total_record_count,
             fasta_file_path_buf,
         })
     }
 }
 
 // SizeAware
-impl SizeAware for IndexedFastaStorage {
+impl EstimateSize for IndexedFastaStorage {
     fn size_of(&self) -> usize {
         let byte_of_path = self.fasta_file_path_buf.to_str().unwrap().as_bytes();
         8 + byte_of_path.size_of()
     }
 }
```

### Comparing `sigalign-0.1.0/local_dependencies/sigalign/src/reference/sequence_storage/indexed_fasta/reverse_complement.rs` & `sigalign-0.2.0/local_dependencies/sigalign/src/reference/sequence_storage/indexed_fasta/reverse_complement.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 use super::{
     Result,
 };
 use super::{
     SequenceStorage,
     // Trait
-    Serializable, SizeAware,
+    Serialize, EstimateSize,
     RcStorage,
 };
 use super::{
     IndexedFastaStorage,
     IndexedFastaBuffer,
 };
 
@@ -63,23 +63,23 @@
         } else {
             true
         }
     }
 }
 
 // Serializable
-impl Serializable for IndexedFastaRcStorage {
+impl Serialize for IndexedFastaRcStorage {
     fn save_to<W>(&self, writer: W) -> Result<()> where W: Write {
         self.0.save_to(writer)
     }
     fn load_from<R>(reader: R) -> Result<Self> where R: Read, Self: Sized {
         let indexed_fasta_storage = IndexedFastaStorage::load_from(reader)?;
         Ok(Self(indexed_fasta_storage))
     }
 }
 
 // SizeAware
-impl SizeAware for IndexedFastaRcStorage {
+impl EstimateSize for IndexedFastaRcStorage {
     fn size_of(&self) -> usize {
         self.0.size_of()
     }
 }
```

### Comparing `sigalign-0.1.0/local_dependencies/sigalign/src/result/result_counts.rs` & `sigalign-0.2.0/local_dependencies/sigalign/src/results/count_results.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,43 @@
 use super::{
     AlignmentResult,
-    RecordAlignmentResult,
-};
-use super::{
-    FastaAlignmentResult,
-    ReadAlignmentResult,
-    FastaAlignmentLabeledResult,
-    ReadAlignmentLabeledResult,
-    AlignmentLabeledResult,
-    RecordAlignmentLabeledResult,
+    TargetAlignmentResult,
+    fasta::{
+        FastaAlignmentResult,
+        ReadAlignmentResult,
+    },
+    labeled::{
+        LabeledAlignmentResult,
+        LabeledTargetAlignmentResult,
+    }
 };
 
-impl FastaAlignmentResult {
+impl AlignmentResult {
     pub fn result_counts(&self) -> usize {
         self.0.iter().map(|x| x.result_counts()).sum()
     }
 }
-impl FastaAlignmentLabeledResult {
+impl TargetAlignmentResult {
     pub fn result_counts(&self) -> usize {
-        self.0.iter().map(|x| x.result_counts()).sum()
+        self.alignments.len()
     }
 }
-impl ReadAlignmentResult {
+impl FastaAlignmentResult {
     pub fn result_counts(&self) -> usize {
-        self.result.result_counts()
+        self.0.iter().map(|x| x.result_counts()).sum()
     }
 }
-impl ReadAlignmentLabeledResult {
+impl ReadAlignmentResult {
     pub fn result_counts(&self) -> usize {
         self.result.result_counts()
     }
 }
-impl AlignmentResult {
-    pub fn result_counts(&self) -> usize {
-        self.0.iter().map(|x| x.result_counts()).sum()
-    }
-}
-impl AlignmentLabeledResult {
+impl LabeledAlignmentResult {
     pub fn result_counts(&self) -> usize {
         self.0.iter().map(|x| x.result_counts()).sum()
     }
 }
-impl RecordAlignmentResult {
+impl LabeledTargetAlignmentResult {
     pub fn result_counts(&self) -> usize {
         self.alignments.len()
     }
-}
-impl RecordAlignmentLabeledResult {
-    pub fn result_counts(&self) -> usize {
-        self.alignments.len()
-    }
-}
+}
```

### Comparing `sigalign-0.1.0/local_dependencies/sigalign/src/util/file_reader.rs` & `sigalign-0.2.0/local_dependencies/sigalign/src/utils/file_reader.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-use crate::Result;
-
 use std::path::Path;
 use std::io::Read;
 use std::fs::File;
 
 use seq_io::fasta::{
     Reader as SeqIoReader,
     Record,
 };
 
+/// The reader of FASTA formatted file
 pub struct FastaReader<R: Read> {
     reader: SeqIoReader<R>,
 }
 
 impl<R: Read> FastaReader<R> {
     pub fn new(reader: R) -> Self {
         let reader = SeqIoReader::new(reader);
         Self {
             reader
         }
     }
 }
 impl FastaReader<File> {
-    pub fn from_file_path<P: AsRef<Path>>(file_path: P) -> Result<Self> {
-        let reader = SeqIoReader::from_path(file_path)?;
+    pub fn from_path<P: AsRef<Path>>(path: P) -> Result<Self, std::io::Error> {
+        let reader = SeqIoReader::from_path(path)?;
         Ok(Self {
             reader
         })
     }
 }
 impl<'a> FastaReader<&'a [u8]> {
     pub fn from_bytes(bytes: &'a [u8]) -> Self {
@@ -35,18 +34,18 @@
     }
 }
 impl<R: Read> Iterator for FastaReader<R> {
     type Item = (String, Vec<u8>);
 
     fn next(&mut self) -> Option<Self::Item> {
         match self.reader.next() {
-            Some(Ok(record)) => {
+            Some(Ok(seq)) => {
                 Some((
-                    String::from_utf8(record.id_bytes().to_vec()).unwrap(),
-                    record.to_owned_record().seq,
+                    String::from_utf8(seq.id_bytes().to_vec()).unwrap(),
+                    seq.to_owned_record().seq,
                 ))
             },
             _ => {
                 None
             },
         }
     }
```

### Comparing `sigalign-0.1.0/.gitignore` & `sigalign-0.2.0/.gitignore`

 * *Files identical despite different names*

