# Comparing `tmp/ngsfragments-2.0.3.tar.gz` & `tmp/ngsfragments-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngsfragments-2.0.3.tar", max compression
+gzip compressed data, was "ngsfragments-2.0.4.tar", max compression
```

## Comparing `ngsfragments-2.0.3.tar` & `ngsfragments-2.0.4.tar`

### file list

```diff
@@ -1,660 +1,660 @@
--rwxr-xr-x   0        0        0    17895 2022-07-20 15:26:56.000000 ngsfragments-2.0.3/LICENSE.md
--rwxr-xr-x   0        0        0      898 2022-07-20 15:27:17.000000 ngsfragments-2.0.3/README.md
--rwxr-xr-x   0        0        0    18935 2023-05-17 14:27:58.055055 ngsfragments-2.0.3/build.py
--rwxr-xr-x   0        0        0     2971 2022-07-20 15:27:17.000000 ngsfragments-2.0.3/cy_build.py
--rwxr-xr-x   0        0        0    10408 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/INSTALL
--rwxr-xr-x   0        0        0     3540 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/LICENSE
--rwxr-xr-x   0        0        0    37612 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/Makefile
--rwxr-xr-x   0        0        0    59421 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/NEWS
--rwxr-xr-x   0        0        0      273 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/README
--rwxr-xr-x   0        0        0     7784 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/README.large_positions.md
--rwxr-xr-x   0        0        0    22063 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/bcf_sr_sort.c
--rwxr-xr-x   0        0        0     3869 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/bcf_sr_sort.h
--rwxr-xr-x   0        0        0    81402 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/bgzf.c
--rwxr-xr-x   0        0        0     5527 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/bgzip.1
--rwxr-xr-x   0        0        0    15526 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/bgzip.c
--rw-r--r--   0        0        0     4122 2022-07-20 16:25:07.000000 ngsfragments-2.0.3/htslib/config.h
--rwxr-xr-x   0        0        0     3823 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/config.h.in
--rwxr-xr-x   0        0        0    36334 2023-05-17 14:30:53.388960 ngsfragments-2.0.3/htslib/config.log
--rw-r--r--   0        0        0     3977 2023-05-17 14:30:53.143521 ngsfragments-2.0.3/htslib/config.mk
--rwxr-xr-x   0        0        0     3546 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/config.mk.in
--rwxr-xr-x   0        0        0    29819 2023-05-17 14:30:52.876329 ngsfragments-2.0.3/htslib/config.status
--rwxr-xr-x   0        0        0      801 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/config_vars.h
--rwxr-xr-x   0        0        0   193602 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/configure
--rwxr-xr-x   0        0        0    17917 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/configure.ac
--rwxr-xr-x   0        0        0     2420 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/cram/cram.h
--rwxr-xr-x   0        0        0   121685 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/cram/cram_codecs.c
--rwxr-xr-x   0        0        0     8507 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/cram/cram_codecs.h
--rwxr-xr-x   0        0        0   124456 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/cram/cram_decode.c
--rwxr-xr-x   0        0        0     3695 2022-07-20 15:27:01.000000 ngsfragments-2.0.3/htslib/cram/cram_decode.h
--rwxr-xr-x   0        0        0   124228 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/cram/cram_encode.c
--rwxr-xr-x   0        0        0     3630 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/cram/cram_encode.h
--rwxr-xr-x   0        0        0    13526 2022-07-20 15:27:01.000000 ngsfragments-2.0.3/htslib/cram/cram_external.c
--rwxr-xr-x   0        0        0    22609 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/cram/cram_index.c
--rwxr-xr-x   0        0        0     3866 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/cram/cram_index.h
--rwxr-xr-x   0        0        0   170538 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/cram/cram_io.c
--rwxr-xr-x   0        0        0    18202 2022-07-20 15:27:01.000000 ngsfragments-2.0.3/htslib/cram/cram_io.h
--rwxr-xr-x   0        0        0     2911 2022-07-20 15:27:01.000000 ngsfragments-2.0.3/htslib/cram/cram_samtools.h
--rwxr-xr-x   0        0        0     7036 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/cram/cram_stats.c
--rwxr-xr-x   0        0        0     2273 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/cram/cram_stats.h
--rwxr-xr-x   0        0        0    28993 2022-07-20 15:27:01.000000 ngsfragments-2.0.3/htslib/cram/cram_structs.h
--rwxr-xr-x   0        0        0    17233 2022-07-20 15:27:01.000000 ngsfragments-2.0.3/htslib/cram/mFILE.c
--rwxr-xr-x   0        0        0     3075 2022-07-20 15:27:01.000000 ngsfragments-2.0.3/htslib/cram/mFILE.h
--rwxr-xr-x   0        0        0     3371 2022-07-20 15:27:01.000000 ngsfragments-2.0.3/htslib/cram/misc.h
--rwxr-xr-x   0        0        0    13991 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/cram/open_trace_file.c
--rwxr-xr-x   0        0        0     5027 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/cram/open_trace_file.h
--rwxr-xr-x   0        0        0     6816 2022-07-20 15:27:01.000000 ngsfragments-2.0.3/htslib/cram/os.h
--rwxr-xr-x   0        0        0     5049 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/cram/pooled_alloc.c
--rwxr-xr-x   0        0        0     2185 2022-07-20 15:27:01.000000 ngsfragments-2.0.3/htslib/cram/pooled_alloc.h
--rwxr-xr-x   0        0        0     4422 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/cram/string_alloc.c
--rwxr-xr-x   0        0        0     2356 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/cram/string_alloc.h
--rwxr-xr-x   0        0        0     6757 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/errmod.c
--rwxr-xr-x   0        0        0     6262 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/faidx.5
--rwxr-xr-x   0        0        0    27085 2022-07-20 15:27:01.000000 ngsfragments-2.0.3/htslib/faidx.c
--rwxr-xr-x   0        0        0    79879 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/header.c
--rwxr-xr-x   0        0        0    10466 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/header.h
--rwxr-xr-x   0        0        0    39697 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/hfile.c
--rwxr-xr-x   0        0        0     4426 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/hfile_gcs.c
--rwxr-xr-x   0        0        0     8028 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/hfile_internal.h
--rwxr-xr-x   0        0        0    48933 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/hfile_libcurl.c
--rwxr-xr-x   0        0        0    36420 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/hfile_s3.c
--rwxr-xr-x   0        0        0    24147 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/hfile_s3_write.c
--rwxr-xr-x   0        0        0   145540 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/hts.c
--rwxr-xr-x   0        0        0    20714 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/hts_expr.c
--rwxr-xr-x   0        0        0     5756 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/hts_internal.h
--rwxr-xr-x   0        0        0     1981 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/hts_os.c
--rwxr-xr-x   0        0        0     2160 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/LICENSE.md
--rwxr-xr-x   0        0        0     1442 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/htscodecs/NEWS
--rwxr-xr-x   0        0        0    29564 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/htscodecs/arith_dynamic.c
--rwxr-xr-x   0        0        0     2371 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/htscodecs/arith_dynamic.h
--rwxr-xr-x   0        0        0     3426 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/htscodecs/c_range_coder.h
--rwxr-xr-x   0        0        0     5630 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/htscodecs/c_simple_model.h
--rwxr-xr-x   0        0        0    40365 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/htscodecs/fqzcomp_qual.c
--rwxr-xr-x   0        0        0     6183 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/htscodecs/fqzcomp_qual.h
--rwxr-xr-x   0        0        0     1957 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/htscodecs/htscodecs.c
--rwxr-xr-x   0        0        0     2286 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/htscodecs/htscodecs.h
--rwxr-xr-x   0        0        0     3557 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/htscodecs/htscodecs_endian.h
--rwxr-xr-x   0        0        0     9091 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/htscodecs/pack.c
--rwxr-xr-x   0        0        0     3257 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/htscodecs/pack.h
--rwxr-xr-x   0        0        0     3972 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/htscodecs/pooled_alloc.h
--rwxr-xr-x   0        0        0    18532 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/htscodecs/rANS_byte.h
--rwxr-xr-x   0        0        0    24585 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/htscodecs/rANS_static.c
--rwxr-xr-x   0        0        0     2037 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/htscodecs/rANS_static.h
--rwxr-xr-x   0        0        0     2414 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/htscodecs/rANS_static4x16.h
--rwxr-xr-x   0        0        0    43110 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/htscodecs/rANS_static4x16pr.c
--rwxr-xr-x   0        0        0    13920 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/htscodecs/rANS_word.h
--rwxr-xr-x   0        0        0     5225 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/htscodecs/rle.c
--rwxr-xr-x   0        0        0     3690 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/htscodecs/rle.h
--rwxr-xr-x   0        0        0    51137 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/htscodecs/tokenise_name3.c
--rwxr-xr-x   0        0        0     2557 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/htscodecs/tokenise_name3.h
--rwxr-xr-x   0        0        0     5615 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/htscodecs/utils.h
--rwxr-xr-x   0        0        0     7224 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/htscodecs/varint.h
--rwxr-xr-x   0        0        0     9004 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/htscodecs/varint2.h
--rwxr-xr-x   0        0        0       37 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/htscodecs/version.h
--rwxr-xr-x   0        0        0      856 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/arith.test
--rwxr-xr-x   0        0        0     2896 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/arith_dynamic_fuzz.c
--rwxr-xr-x   0        0        0     7402 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/arith_dynamic_test.c
--rwxr-xr-x   0        0        0    11615 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q4.0
--rwxr-xr-x   0        0        0    10831 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q4.1
--rwxr-xr-x   0        0        0    10774 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q4.128
--rwxr-xr-x   0        0        0    10329 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q4.129
--rwxr-xr-x   0        0        0    11095 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q4.192
--rwxr-xr-x   0        0        0    10283 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q4.193
--rwxr-xr-x   0        0        0    13360 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q4.64
--rwxr-xr-x   0        0        0    10484 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q4.65
--rwxr-xr-x   0        0        0    11448 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q4.8
--rwxr-xr-x   0        0        0    11083 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q4.9
--rwxr-xr-x   0        0        0    49949 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q40+dir.0
--rwxr-xr-x   0        0        0    49034 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q40+dir.1
--rwxr-xr-x   0        0        0    51242 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q40+dir.64
--rwxr-xr-x   0        0        0    49061 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q40+dir.65
--rwxr-xr-x   0        0        0    49820 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q40+dir.8
--rwxr-xr-x   0        0        0    49448 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q40+dir.9
--rwxr-xr-x   0        0        0    32752 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q8.0
--rwxr-xr-x   0        0        0    31331 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q8.1
--rwxr-xr-x   0        0        0    32063 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q8.128
--rwxr-xr-x   0        0        0    31084 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q8.129
--rwxr-xr-x   0        0        0    32267 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q8.192
--rwxr-xr-x   0        0        0    30931 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q8.193
--rwxr-xr-x   0        0        0    35211 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q8.64
--rwxr-xr-x   0        0        0    30907 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q8.65
--rwxr-xr-x   0        0        0    32597 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/qvar.0
--rwxr-xr-x   0        0        0    31982 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/qvar.1
--rwxr-xr-x   0        0        0    33237 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/qvar.64
--rwxr-xr-x   0        0        0    31993 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/qvar.65
--rwxr-xr-x   0        0        0     9307 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/q4.0
--rwxr-xr-x   0        0        0     9618 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/q4.1
--rwxr-xr-x   0        0        0     9453 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/q4.2
--rwxr-xr-x   0        0        0    10481 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/q4.3
--rwxr-xr-x   0        0        0    47712 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/q40+dir.0
--rwxr-xr-x   0        0        0    43803 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/q40+dir.1
--rwxr-xr-x   0        0        0    47233 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/q40+dir.2
--rwxr-xr-x   0        0        0    48485 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/q40+dir.3
--rwxr-xr-x   0        0        0    30012 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/q8.0
--rwxr-xr-x   0        0        0    33742 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/q8.1
--rwxr-xr-x   0        0        0    30982 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/q8.2
--rwxr-xr-x   0        0        0    31709 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/q8.3
--rwxr-xr-x   0        0        0    32868 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/qvar.0
--rwxr-xr-x   0        0        0    35007 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/qvar.1
--rwxr-xr-x   0        0        0    32400 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/qvar.2
--rwxr-xr-x   0        0        0    32073 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/qvar.3
--rwxr-xr-x   0        0        0   152000 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/q4
--rwxr-xr-x   0        0        0   103000 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/q40+dir
--rwxr-xr-x   0        0        0   147383 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/q8
--rwxr-xr-x   0        0        0    62441 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/qvar
--rwxr-xr-x   0        0        0    11660 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q4.0
--rwxr-xr-x   0        0        0    10848 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q4.1
--rwxr-xr-x   0        0        0    10902 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q4.128
--rwxr-xr-x   0        0        0    10890 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q4.129
--rwxr-xr-x   0        0        0    11225 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q4.192
--rwxr-xr-x   0        0        0    10825 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q4.193
--rwxr-xr-x   0        0        0    12878 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q4.64
--rwxr-xr-x   0        0        0    10672 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q4.65
--rwxr-xr-x   0        0        0    11731 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q4.8
--rwxr-xr-x   0        0        0    11111 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q4.9
--rwxr-xr-x   0        0        0    50247 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q40+dir.0
--rwxr-xr-x   0        0        0    49449 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q40+dir.1
--rwxr-xr-x   0        0        0    50072 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q40+dir.8
--rwxr-xr-x   0        0        0    50072 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q40+dir.9
--rwxr-xr-x   0        0        0    33088 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q8.0
--rwxr-xr-x   0        0        0    31372 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q8.1
--rwxr-xr-x   0        0        0    32237 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q8.128
--rwxr-xr-x   0        0        0    31258 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q8.129
--rwxr-xr-x   0        0        0    32024 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q8.192
--rwxr-xr-x   0        0        0    31146 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q8.193
--rwxr-xr-x   0        0        0    33458 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q8.64
--rwxr-xr-x   0        0        0    31025 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q8.65
--rwxr-xr-x   0        0        0    32987 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/qvar.0
--rwxr-xr-x   0        0        0    32261 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/qvar.1
--rwxr-xr-x   0        0        0    11674 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x8/q4.0
--rwxr-xr-x   0        0        0    10870 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x8/q4.1
--rwxr-xr-x   0        0        0    50258 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x8/q40+dir.0
--rwxr-xr-x   0        0        0    50537 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x8/q40+dir.1
--rwxr-xr-x   0        0        0    33099 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x8/q8.0
--rwxr-xr-x   0        0        0    31428 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x8/q8.1
--rwxr-xr-x   0        0        0    32997 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x8/qvar.0
--rwxr-xr-x   0        0        0    32832 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x8/qvar.1
--rwxr-xr-x   0        0        0      753 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/fqzcomp.test
--rwxr-xr-x   0        0        0     3055 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/fqzcomp_qual_fuzz.c
--rwxr-xr-x   0        0        0    12136 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/fqzcomp_qual_test.c
--rwxr-xr-x   0        0        0    45893 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/01.names
--rwxr-xr-x   0        0        0    41060 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/02.names
--rwxr-xr-x   0        0        0    77358 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/03.names
--rwxr-xr-x   0        0        0    32489 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/05.names
--rwxr-xr-x   0        0        0    86076 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/08.names
--rwxr-xr-x   0        0        0    18000 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/09.names
--rwxr-xr-x   0        0        0    38232 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/10.names
--rwxr-xr-x   0        0        0    32912 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/20.names
--rwxr-xr-x   0        0        0    39455 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/nv.names
--rwxr-xr-x   0        0        0    38516 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/nv2.names
--rwxr-xr-x   0        0        0    36899 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/rr.names
--rwxr-xr-x   0        0        0     3842 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/01.names.1
--rwxr-xr-x   0        0        0     3566 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/01.names.11
--rwxr-xr-x   0        0        0     2424 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/01.names.13
--rwxr-xr-x   0        0        0     2087 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/01.names.15
--rwxr-xr-x   0        0        0     2051 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/01.names.17
--rwxr-xr-x   0        0        0     2049 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/01.names.19
--rwxr-xr-x   0        0        0     2471 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/01.names.3
--rwxr-xr-x   0        0        0     2334 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/01.names.5
--rwxr-xr-x   0        0        0     2234 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/01.names.7
--rwxr-xr-x   0        0        0     2234 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/01.names.9
--rwxr-xr-x   0        0        0     7041 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/02.names.1
--rwxr-xr-x   0        0        0     6468 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/02.names.11
--rwxr-xr-x   0        0        0     4797 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/02.names.13
--rwxr-xr-x   0        0        0     4749 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/02.names.15
--rwxr-xr-x   0        0        0     4695 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/02.names.17
--rwxr-xr-x   0        0        0     4695 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/02.names.19
--rwxr-xr-x   0        0        0     4983 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/02.names.3
--rwxr-xr-x   0        0        0     4983 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/02.names.5
--rwxr-xr-x   0        0        0     4922 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/02.names.7
--rwxr-xr-x   0        0        0     4918 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/02.names.9
--rwxr-xr-x   0        0        0    11237 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/03.names.1
--rwxr-xr-x   0        0        0     9798 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/03.names.11
--rwxr-xr-x   0        0        0     7291 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/03.names.13
--rwxr-xr-x   0        0        0     7255 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/03.names.15
--rwxr-xr-x   0        0        0     7069 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/03.names.17
--rwxr-xr-x   0        0        0     7068 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/03.names.19
--rwxr-xr-x   0        0        0     7822 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/03.names.3
--rwxr-xr-x   0        0        0     7822 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/03.names.5
--rwxr-xr-x   0        0        0     7521 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/03.names.7
--rwxr-xr-x   0        0        0     7521 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/03.names.9
--rwxr-xr-x   0        0        0     5356 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/05.names.1
--rwxr-xr-x   0        0        0     4869 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/05.names.11
--rwxr-xr-x   0        0        0     3405 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/05.names.13
--rwxr-xr-x   0        0        0     3404 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/05.names.15
--rwxr-xr-x   0        0        0     3377 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/05.names.17
--rwxr-xr-x   0        0        0     3377 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/05.names.19
--rwxr-xr-x   0        0        0     3600 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/05.names.3
--rwxr-xr-x   0        0        0     3600 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/05.names.5
--rwxr-xr-x   0        0        0     3534 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/05.names.7
--rwxr-xr-x   0        0        0     3534 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/05.names.9
--rwxr-xr-x   0        0        0     7324 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/08.names.1
--rwxr-xr-x   0        0        0     6804 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/08.names.11
--rwxr-xr-x   0        0        0     4895 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/08.names.13
--rwxr-xr-x   0        0        0     4894 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/08.names.15
--rwxr-xr-x   0        0        0     4805 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/08.names.17
--rwxr-xr-x   0        0        0     4805 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/08.names.19
--rwxr-xr-x   0        0        0     5291 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/08.names.3
--rwxr-xr-x   0        0        0     5291 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/08.names.5
--rwxr-xr-x   0        0        0     5160 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/08.names.7
--rwxr-xr-x   0        0        0     5160 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/08.names.9
--rwxr-xr-x   0        0        0     5411 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/09.names.1
--rwxr-xr-x   0        0        0     4898 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/09.names.11
--rwxr-xr-x   0        0        0     3427 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/09.names.13
--rwxr-xr-x   0        0        0     3427 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/09.names.15
--rwxr-xr-x   0        0        0     3366 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/09.names.17
--rwxr-xr-x   0        0        0     3366 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/09.names.19
--rwxr-xr-x   0        0        0     3598 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/09.names.3
--rwxr-xr-x   0        0        0     3598 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/09.names.5
--rwxr-xr-x   0        0        0     3493 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/09.names.7
--rwxr-xr-x   0        0        0     3493 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/09.names.9
--rwxr-xr-x   0        0        0     6881 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/10.names.1
--rwxr-xr-x   0        0        0     6204 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/10.names.11
--rwxr-xr-x   0        0        0     4567 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/10.names.13
--rwxr-xr-x   0        0        0     4558 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/10.names.15
--rwxr-xr-x   0        0        0     4472 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/10.names.17
--rwxr-xr-x   0        0        0     4472 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/10.names.19
--rwxr-xr-x   0        0        0     4843 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/10.names.3
--rwxr-xr-x   0        0        0     4843 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/10.names.5
--rwxr-xr-x   0        0        0     4746 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/10.names.7
--rwxr-xr-x   0        0        0     4744 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/10.names.9
--rwxr-xr-x   0        0        0     2956 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/20.names.1
--rwxr-xr-x   0        0        0     2732 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/20.names.11
--rwxr-xr-x   0        0        0     1626 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/20.names.13
--rwxr-xr-x   0        0        0     1625 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/20.names.15
--rwxr-xr-x   0        0        0     1600 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/20.names.17
--rwxr-xr-x   0        0        0     1600 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/20.names.19
--rwxr-xr-x   0        0        0     1695 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/20.names.3
--rwxr-xr-x   0        0        0     1695 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/20.names.5
--rwxr-xr-x   0        0        0     1632 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/20.names.7
--rwxr-xr-x   0        0        0     1632 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/20.names.9
--rwxr-xr-x   0        0        0     7168 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv.names.1
--rwxr-xr-x   0        0        0     6426 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv.names.11
--rwxr-xr-x   0        0        0     4825 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv.names.13
--rwxr-xr-x   0        0        0     4787 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv.names.15
--rwxr-xr-x   0        0        0     4767 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv.names.17
--rwxr-xr-x   0        0        0     4767 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv.names.19
--rwxr-xr-x   0        0        0     4989 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv.names.3
--rwxr-xr-x   0        0        0     4989 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv.names.5
--rwxr-xr-x   0        0        0     4937 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv.names.7
--rwxr-xr-x   0        0        0     4937 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv.names.9
--rwxr-xr-x   0        0        0     1718 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv2.names.1
--rwxr-xr-x   0        0        0     1411 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv2.names.11
--rwxr-xr-x   0        0        0      836 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv2.names.13
--rwxr-xr-x   0        0        0      809 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv2.names.15
--rwxr-xr-x   0        0        0      747 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv2.names.17
--rwxr-xr-x   0        0        0      747 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv2.names.19
--rwxr-xr-x   0        0        0      903 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv2.names.3
--rwxr-xr-x   0        0        0      903 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv2.names.5
--rwxr-xr-x   0        0        0      846 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv2.names.7
--rwxr-xr-x   0        0        0      846 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv2.names.9
--rwxr-xr-x   0        0        0     9012 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/rr.names.1
--rwxr-xr-x   0        0        0     8513 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/rr.names.11
--rwxr-xr-x   0        0        0     6066 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/rr.names.13
--rwxr-xr-x   0        0        0     5979 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/rr.names.15
--rwxr-xr-x   0        0        0     5963 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/rr.names.17
--rwxr-xr-x   0        0        0     5963 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/rr.names.19
--rwxr-xr-x   0        0        0     6288 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/rr.names.3
--rwxr-xr-x   0        0        0     6286 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/rr.names.5
--rwxr-xr-x   0        0        0     6230 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/rr.names.7
--rwxr-xr-x   0        0        0     6230 2022-07-20 15:27:08.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/rr.names.9
--rwxr-xr-x   0        0        0     3807 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/rANS_static4x16pr_fuzz.c
--rwxr-xr-x   0        0        0     7770 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/rANS_static4x16pr_test.c
--rwxr-xr-x   0        0        0     3951 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/rANS_static_fuzz.c
--rwxr-xr-x   0        0        0     7315 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/rANS_static_test.c
--rwxr-xr-x   0        0        0      842 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/rans4x16.test
--rwxr-xr-x   0        0        0      742 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/rans4x8.test
--rwxr-xr-x   0        0        0      667 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/tok3.test
--rwxr-xr-x   0        0        0     2973 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/tokenise_name3_fuzz.c
--rwxr-xr-x   0        0        0     5533 2022-07-20 15:27:07.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/tokenise_name3_test.c
--rwxr-xr-x   0        0        0    10245 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htscodecs/tests/varint_test.c
--rw-r--r--   0        0        0      162 2023-05-17 14:30:53.205615 ngsfragments-2.0.3/htslib/htscodecs.mk
--rwxr-xr-x   0        0        0      123 2022-07-20 15:27:01.000000 ngsfragments-2.0.3/htslib/htscodecs.mk.in
--rwxr-xr-x   0        0        0     3083 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/htscodecs_bundled.mk
--rwxr-xr-x   0        0        0     1710 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/htscodecs_external.mk
--rwxr-xr-x   0        0        0     3856 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/htsfile.1
--rwxr-xr-x   0        0        0     9607 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/htsfile.c
--rwxr-xr-x   0        0        0    16081 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/htslib/bgzf.h
--rwxr-xr-x   0        0        0    16837 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/htslib/cram.h
--rwxr-xr-x   0        0        0    12934 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/htslib/faidx.h
--rwxr-xr-x   0        0        0    12877 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/htslib/hfile.h
--rwxr-xr-x   0        0        0    52935 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/htslib/hts.h
--rwxr-xr-x   0        0        0     3989 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/htslib/hts_defs.h
--rwxr-xr-x   0        0        0    11485 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/htslib/hts_endian.h
--rwxr-xr-x   0        0        0     3760 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/htslib/hts_expr.h
--rwxr-xr-x   0        0        0     3944 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/htslib/hts_log.h
--rwxr-xr-x   0        0        0     2533 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/htslib/hts_os.h
--rwxr-xr-x   0        0        0     5605 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/htslib/kbitset.h
--rwxr-xr-x   0        0        0     2828 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/htslib/kfunc.h
--rwxr-xr-x   0        0        0    22899 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/htslib/khash.h
--rwxr-xr-x   0        0        0     4050 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/htslib/khash_str2int.h
--rwxr-xr-x   0        0        0     5135 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/htslib/klist.h
--rwxr-xr-x   0        0        0     3362 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/htslib/knetfile.h
--rwxr-xr-x   0        0        0     3295 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/htslib/kroundup.h
--rwxr-xr-x   0        0        0     8830 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/htslib/kseq.h
--rwxr-xr-x   0        0        0    11480 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/htslib/ksort.h
--rwxr-xr-x   0        0        0    11090 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/htslib/kstring.h
--rwxr-xr-x   0        0        0     8881 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/htslib/regidx.h
--rwxr-xr-x   0        0        0    78275 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/htslib/sam.h
--rwxr-xr-x   0        0        0    15800 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/htslib/synced_bcf_reader.h
--rwxr-xr-x   0        0        0     4942 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/htslib/tbx.h
--rwxr-xr-x   0        0        0    12747 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/htslib/thread_pool.h
--rwxr-xr-x   0        0        0    62511 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/htslib/vcf.h
--rwxr-xr-x   0        0        0     1686 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/htslib/vcf_sweep.h
--rwxr-xr-x   0        0        0     4919 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/htslib/vcfutils.h
--rwxr-xr-x   0        0        0     4561 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/htslib-s3-plugin.7
--rwxr-xr-x   0        0        0     6530 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/htslib.mk
--rwxr-xr-x   0        0        0      490 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/htslib.pc.in
--rw-r--r--   0        0        0      784 2023-05-17 14:30:53.270448 ngsfragments-2.0.3/htslib/htslib.pc.tmp
--rwxr-xr-x   0        0        0     3312 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/htslib_vars.mk
--rwxr-xr-x   0        0        0    10879 2022-07-20 15:27:01.000000 ngsfragments-2.0.3/htslib/kfunc.c
--rwxr-xr-x   0        0        0    10570 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/kstring.c
--rwxr-xr-x   0        0        0     2604 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/m4/hts_hide_dynamic_syms.m4
--rwxr-xr-x   0        0        0     8273 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/m4/hts_prog_cc_warnings.m4
--rwxr-xr-x   0        0        0    10244 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/m4/pkg.m4
--rwxr-xr-x   0        0        0    10656 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/md5.c
--rwxr-xr-x   0        0        0     8488 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/multipart.c
--rwxr-xr-x   0        0        0     2345 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/os/lzma_stub.h
--rwxr-xr-x   0        0        0     2704 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/os/rand.c
--rwxr-xr-x   0        0        0     6501 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/plugin.c
--rwxr-xr-x   0        0        0    16107 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/probaln.c
--rwxr-xr-x   0        0        0    11748 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/realn.c
--rwxr-xr-x   0        0        0    19883 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/regidx.c
--rwxr-xr-x   0        0        0     7744 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/region.c
--rwxr-xr-x   0        0        0     2789 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/sam.5
--rwxr-xr-x   0        0        0   168295 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/sam.c
--rwxr-xr-x   0        0        0     3368 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/sam_internal.h
--rwxr-xr-x   0        0        0    43102 2022-07-20 15:27:01.000000 ngsfragments-2.0.3/htslib/synced_bcf_reader.c
--rwxr-xr-x   0        0        0     6954 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/tabix.1
--rwxr-xr-x   0        0        0    26296 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/tabix.c
--rwxr-xr-x   0        0        0    15686 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/tbx.c
--rwxr-xr-x   0        0        0      751 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/auxf#values.sam
--rwxr-xr-x   0        0        0     5152 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/auxf#values_java.cram
--rwxr-xr-x   0        0        0       29 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/test/auxf.fa
--rwxr-xr-x   0        0        0       18 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/auxf.fa.fai
--rwxr-xr-x   0        0        0      518 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/test/bcf-sr/merge.noidx.a.vcf
--rwxr-xr-x   0        0        0      128 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/test/bcf-sr/merge.noidx.abc.expected.out
--rwxr-xr-x   0        0        0      634 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/test/bcf-sr/merge.noidx.b.vcf
--rwxr-xr-x   0        0        0      634 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/test/bcf-sr/merge.noidx.c.vcf
--rwxr-xr-x   0        0        0      518 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/test/bcf-sr/merge.noidx.hdr_order.vcf
--rwxr-xr-x   0        0        0      518 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/test/bcf-sr/merge.noidx.rec_order.vcf
--rwxr-xr-x   0        0        0       15 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/bgziptest.txt
--rwxr-xr-x   0        0        0      181 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/bgziptest.txt.gz
--rwxr-xr-x   0        0        0       88 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/bgziptest.txt.gz.gzi
--rwxr-xr-x   0        0        0      148 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/c1#bounds.sam
--rwxr-xr-x   0        0        0      337 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/c1#clip.sam
--rwxr-xr-x   0        0        0      433 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/c1#noseq.sam
--rwxr-xr-x   0        0        0      388 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/c1#pad1.sam
--rwxr-xr-x   0        0        0      527 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/c1#pad2.sam
--rwxr-xr-x   0        0        0      665 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/c1#pad3.sam
--rwxr-xr-x   0        0        0      429 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/c1#unknown.sam
--rwxr-xr-x   0        0        0       15 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/test/c1.fa
--rwxr-xr-x   0        0        0       14 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/c1.fa.fai
--rwxr-xr-x   0        0        0      847 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/test/c2#pad.sam
--rwxr-xr-x   0        0        0       14 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/c2.fa
--rwxr-xr-x   0        0        0       12 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/c2.fa.fai
--rwxr-xr-x   0        0        0      341 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/ce#1.sam
--rwxr-xr-x   0        0        0   322632 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/ce#1000.sam
--rwxr-xr-x   0        0        0      645 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/ce#2.sam
--rwxr-xr-x   0        0        0     1872 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/ce#5.sam
--rwxr-xr-x   0        0        0     1836 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/test/ce#5b.sam
--rwxr-xr-x   0        0        0     6784 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/test/ce#5b_java.cram
--rwxr-xr-x   0        0        0  2147244 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/ce#large_seq.sam
--rwxr-xr-x   0        0        0      547 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/ce#supp.sam
--rwxr-xr-x   0        0        0     1638 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/ce#tag_depadded.sam
--rwxr-xr-x   0        0        0     1650 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/ce#tag_padded.sam
--rwxr-xr-x   0        0        0     1325 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/test/ce#unmap.sam
--rwxr-xr-x   0        0        0     2747 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/ce#unmap1.sam
--rwxr-xr-x   0        0        0     5525 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/ce#unmap2.sam
--rwxr-xr-x   0        0        0  1060702 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/ce.fa
--rwxr-xr-x   0        0        0      230 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/ce.fa.fai
--rwxr-xr-x   0        0        0      268 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/colons.bam
--rwxr-xr-x   0        0        0      424 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/colons.bam.bai
--rwxr-xr-x   0        0        0     6474 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/compare_sam.pl
--rwxr-xr-x   0        0        0     4307 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/cross_validate.sh
--rwxr-xr-x   0        0        0        0 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/emptyfile
--rwxr-xr-x   0        0        0      289 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/test/faidx.fa
--rwxr-xr-x   0        0        0    48599 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/fastqs.fq
--rwxr-xr-x   0        0        0     4951 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/fastqs_README.txt
--rwxr-xr-x   0        0        0     2438 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/fieldarith.c
--rwxr-xr-x   0        0        0      910 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/fieldarith.sam
--rwxr-xr-x   0        0        0      241 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/formatcols.vcf
--rwxr-xr-x   0        0        0      226 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/formatmissing-out.vcf
--rwxr-xr-x   0        0        0      226 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/test/formatmissing.vcf
--rwxr-xr-x   0        0        0     3964 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/fuzz/hts_open_fuzzer.c
--rwxr-xr-x   0        0        0     3562 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/test/header_syms.pl
--rwxr-xr-x   0        0        0    12012 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/hfile.c
--rwxr-xr-x   0        0        0    17620 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/hts_endian.c
--rwxr-xr-x   0        0        0      776 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/index.bam.bai
--rwxr-xr-x   0        0        0      130 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/index.bam.csi
--rwxr-xr-x   0        0        0      144 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/index.bcf.csi
--rwxr-xr-x   0        0        0       83 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/index.cram.crai
--rwxr-xr-x   0        0        0    54185 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/index.sam
--rwxr-xr-x   0        0        0      776 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/index.sam.gz.bai
--rwxr-xr-x   0        0        0      130 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/index.sam.gz.csi
--rwxr-xr-x   0        0        0    68888 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/test/index.vcf
--rwxr-xr-x   0        0        0      159 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/index.vcf.gz.csi
--rwxr-xr-x   0        0        0      213 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/index.vcf.gz.tbi
--rwxr-xr-x   0        0        0    54375 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/index_dos.sam
--rwxr-xr-x   0        0        0      594 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/longrefs/index.expected1.vcf
--rwxr-xr-x   0        0        0       83 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/longrefs/index.expected2.vcf
--rwxr-xr-x   0        0        0    21491 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/longrefs/index.vcf
--rwxr-xr-x   0        0        0    31717 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/longrefs/longref.sam
--rwxr-xr-x   0        0        0     8300 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/longrefs/longref_itr.expected.sam
--rwxr-xr-x   0        0        0    15015 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/longrefs/longref_multi.expected.sam
--rwxr-xr-x   0        0        0     3255 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/maintainer/check_copyright.pl
--rwxr-xr-x   0        0        0     2734 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/maintainer/check_spaces.pl
--rwxr-xr-x   0        0        0     1017 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/md#1.sam
--rwxr-xr-x   0        0        0       45 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/md.fa
--rwxr-xr-x   0        0        0       13 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/md.fa.fai
--rwxr-xr-x   0        0        0      274 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/mpileup/c1#pad1.out
--rwxr-xr-x   0        0        0     2024 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/mpileup/c1#pad1.sam
--rwxr-xr-x   0        0        0      355 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/mpileup/c1#pad2.out
--rwxr-xr-x   0        0        0     2311 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/mpileup/c1#pad2.sam
--rwxr-xr-x   0        0        0      134 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/mpileup/c1#pad3.out
--rwxr-xr-x   0        0        0     2393 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/mpileup/c1#pad3.sam
--rwxr-xr-x   0        0        0      130 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/mpileup/mp_D.out
--rwxr-xr-x   0        0        0     1534 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/mpileup/mp_D.sam
--rwxr-xr-x   0        0        0      197 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/mpileup/mp_DI.out
--rwxr-xr-x   0        0        0     1747 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/mpileup/mp_DI.sam
--rwxr-xr-x   0        0        0      135 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/mpileup/mp_I.out
--rwxr-xr-x   0        0        0     1821 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/mpileup/mp_I.sam
--rwxr-xr-x   0        0        0      181 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/mpileup/mp_ID.out
--rwxr-xr-x   0        0        0     1958 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/mpileup/mp_ID.sam
--rwxr-xr-x   0        0        0      122 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/mpileup/mp_N.out
--rwxr-xr-x   0        0        0     1739 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/mpileup/mp_N.sam
--rwxr-xr-x   0        0        0      275 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/mpileup/mp_N2.out
--rwxr-xr-x   0        0        0     2152 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/mpileup/mp_N2.sam
--rwxr-xr-x   0        0        0      169 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/mpileup/mp_P.out
--rwxr-xr-x   0        0        0     1796 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/mpileup/mp_P.sam
--rwxr-xr-x   0        0        0     2582 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/mpileup/mpileup.tst
--rwxr-xr-x   0        0        0     1294 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/mpileup/small.bam
--rwxr-xr-x   0        0        0     3330 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/mpileup/small.out
--rwxr-xr-x   0        0        0     1295 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/mpileup/test-pileup.sh
--rwxr-xr-x   0        0        0     1691 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/no_hdr_sq_1.bam
--rwxr-xr-x   0        0        0       94 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/no_hdr_sq_1.bam.csi
--rwxr-xr-x   0        0        0     2019 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/no_hdr_sq_1.expected.sam
--rwxr-xr-x   0        0        0      325 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/noroundtrip-out.vcf
--rwxr-xr-x   0        0        0      271 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/noroundtrip.vcf
--rwxr-xr-x   0        0        0     7002 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/pileup.c
--rwxr-xr-x   0        0        0     5072 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/plugins-dlhts.c
--rwxr-xr-x   0        0        0    13337 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/range.bam
--rwxr-xr-x   0        0        0      360 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/range.bam.bai
--rwxr-xr-x   0        0        0    11182 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/range.cram
--rwxr-xr-x   0        0        0       94 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/range.cram.crai
--rwxr-xr-x   0        0        0     3496 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/range.out
--rwxr-xr-x   0        0        0      719 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/realn01.fa
--rwxr-xr-x   0        0        0       21 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/realn01.fa.fai
--rwxr-xr-x   0        0        0     1843 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/realn01.sam
--rwxr-xr-x   0        0        0     2157 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/realn01_exp-a.sam
--rwxr-xr-x   0        0        0     2157 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/realn01_exp-e.sam
--rwxr-xr-x   0        0        0     2157 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/realn01_exp.sam
--rwxr-xr-x   0        0        0     3758 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/realn02-r.sam
--rwxr-xr-x   0        0        0     4284 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/realn02.fa
--rwxr-xr-x   0        0        0       17 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/realn02.fa.fai
--rwxr-xr-x   0        0        0     2894 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/test/realn02.sam
--rwxr-xr-x   0        0        0     3758 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/realn02_exp-a.sam
--rwxr-xr-x   0        0        0     3758 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/realn02_exp-e.sam
--rwxr-xr-x   0        0        0     3758 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/test/realn02_exp.sam
--rwxr-xr-x   0        0        0    78940 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/sam.c
--rwxr-xr-x   0        0        0     1291 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/sam_filter/filter.sh
--rwxr-xr-x   0        0        0     2610 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/sam_filter/filter.tst
--rwxr-xr-x   0        0        0        2 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/sam_filter/func1.out
--rwxr-xr-x   0        0        0        3 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/sam_filter/func2.out
--rwxr-xr-x   0        0        0        2 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/sam_filter/func3.out
--rwxr-xr-x   0        0        0        4 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/sam_filter/func4.out
--rwxr-xr-x   0        0        0        3 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/sam_filter/int1.out
--rwxr-xr-x   0        0        0        3 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/sam_filter/int2.out
--rwxr-xr-x   0        0        0        3 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/sam_filter/int3.out
--rwxr-xr-x   0        0        0      485 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/sam_filter/string1.out
--rwxr-xr-x   0        0        0      451 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/sam_filter/string2.out
--rwxr-xr-x   0        0        0      748 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/sam_filter/string3.out
--rwxr-xr-x   0        0        0     1136 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/sam_filter/string4.out
--rwxr-xr-x   0        0        0      498 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/sam_filter/string5.out
--rwxr-xr-x   0        0        0      319 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/sam_filter/string6.out
--rwxr-xr-x   0        0        0      410 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/sam_filter/string7.out
--rwxr-xr-x   0        0        0     5587 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/simple_test_driver.sh
--rwxr-xr-x   0        0        0       47 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/tabix/bed_file.Y.100200.out
--rwxr-xr-x   0        0        0     1857 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/tabix/bed_file.bed
--rwxr-xr-x   0        0        0      407 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/tabix/bed_file.separate.out
--rwxr-xr-x   0        0        0      405 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/tabix/gff_file.X.2934832.2935190.out
--rwxr-xr-x   0        0        0     5618 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/tabix/gff_file.gff
--rwxr-xr-x   0        0        0      288 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/tabix/large_chr.20.1.2147483647.out
--rwxr-xr-x   0        0        0      622 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/tabix/large_chr.vcf
--rwxr-xr-x   0        0        0     3023 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/tabix/tabix.tst
--rwxr-xr-x   0        0        0     1312 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/tabix/test-tabix.sh
--rwxr-xr-x   0        0        0       67 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/tabix/vcf_file.1.3000151.out
--rwxr-xr-x   0        0        0       74 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/tabix/vcf_file.2.3199812.out
--rwxr-xr-x   0        0        0     2719 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/tabix/vcf_file.bcf
--rwxr-xr-x   0        0        0     2543 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/tabix/vcf_file.vcf
--rwxr-xr-x   0        0        0       98 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/tabix.out
--rwxr-xr-x   0        0        0     5167 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/test-bcf-sr.c
--rwxr-xr-x   0        0        0    19566 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/test-bcf-sr.pl
--rwxr-xr-x   0        0        0     8964 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/test-bcf-translate.c
--rwxr-xr-x   0        0        0      869 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/test-bcf-translate.out
--rwxr-xr-x   0        0        0     2602 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/test-logging.pl
--rwxr-xr-x   0        0        0     7064 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/test-parse-reg.c
--rwxr-xr-x   0        0        0    16871 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/test-regidx.c
--rwxr-xr-x   0        0        0    23890 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/test/test-vcf-api.c
--rwxr-xr-x   0        0        0     2064 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/test-vcf-api.out
--rwxr-xr-x   0        0        0     2024 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/test-vcf-hdr-in.vcf
--rwxr-xr-x   0        0        0     1349 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/test-vcf-hdr.out
--rwxr-xr-x   0        0        0     3840 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/test-vcf-sweep.c
--rwxr-xr-x   0        0        0       92 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/test-vcf-sweep.out
--rwxr-xr-x   0        0        0    39913 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/test.pl
--rwxr-xr-x   0        0        0    31594 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/test_bgzf.c
--rwxr-xr-x   0        0        0     6966 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/test/test_expr.c
--rwxr-xr-x   0        0        0     2869 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/test_index.c
--rwxr-xr-x   0        0        0     3308 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/test/test_introspection.c
--rwxr-xr-x   0        0        0     3639 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/test_kfunc.c
--rwxr-xr-x   0        0        0    12102 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/test_kstring.c
--rwxr-xr-x   0        0        0     5057 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/test_realn.c
--rwxr-xr-x   0        0        0     8892 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/test_str2int.c
--rwxr-xr-x   0        0        0    14460 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/test_view.c
--rwxr-xr-x   0        0        0     1688 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/thrash_threads1.c
--rwxr-xr-x   0        0        0     1621 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/test/thrash_threads2.c
--rwxr-xr-x   0        0        0     1729 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/test/thrash_threads3.c
--rwxr-xr-x   0        0        0     2273 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/thrash_threads4.c
--rwxr-xr-x   0        0        0     2176 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/thrash_threads5.c
--rwxr-xr-x   0        0        0     3412 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/thrash_threads6.c
--rwxr-xr-x   0        0        0     3661 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/thrash_threads7.c
--rwxr-xr-x   0        0        0     2938 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/thread_pool.md
--rwxr-xr-x   0        0        0     2108 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/with-shlib.sh
--rwxr-xr-x   0        0        0     1070 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/test/xx#MD.sam
--rwxr-xr-x   0        0        0     1159 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/xx#MD2.sam
--rwxr-xr-x   0        0        0       71 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/xx#blank.sam
--rwxr-xr-x   0        0        0   905485 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/xx#large_aux.sam
--rwxr-xr-x   0        0        0      651 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/xx#large_aux2.sam
--rwxr-xr-x   0        0        0    22668 2022-07-20 15:27:06.000000 ngsfragments-2.0.3/htslib/test/xx#large_aux_java.cram
--rwxr-xr-x   0        0        0      254 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/xx#minimal.sam
--rwxr-xr-x   0        0        0      304 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/xx#pair.sam
--rwxr-xr-x   0        0        0      298 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/xx#repeated.sam
--rwxr-xr-x   0        0        0      517 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/xx#rg.sam
--rwxr-xr-x   0        0        0     1028 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/xx#tlen.sam
--rwxr-xr-x   0        0        0     1096 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/xx#tlen2.sam
--rwxr-xr-x   0        0        0      267 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/xx#triplet.sam
--rwxr-xr-x   0        0        0      320 2022-07-20 15:27:04.000000 ngsfragments-2.0.3/htslib/test/xx#unsorted.sam
--rwxr-xr-x   0        0        0       86 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/xx.fa
--rwxr-xr-x   0        0        0       44 2022-07-20 15:27:05.000000 ngsfragments-2.0.3/htslib/test/xx.fa.fai
--rwxr-xr-x   0        0        0    11957 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/textutils.c
--rwxr-xr-x   0        0        0    14771 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/textutils_internal.h
--rwxr-xr-x   0        0        0    45617 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/thread_pool.c
--rwxr-xr-x   0        0        0     5853 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/thread_pool_internal.h
--rwxr-xr-x   0        0        0     3543 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/vcf.5
--rwxr-xr-x   0        0        0   163400 2022-07-20 15:27:09.000000 ngsfragments-2.0.3/htslib/vcf.c
--rwxr-xr-x   0        0        0     5570 2022-07-20 15:27:01.000000 ngsfragments-2.0.3/htslib/vcf_sweep.c
--rwxr-xr-x   0        0        0    33937 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/vcfutils.c
--rwxr-xr-x   0        0        0       33 2022-07-20 15:27:02.000000 ngsfragments-2.0.3/htslib/version.h
--rwxr-xr-x   0        0        0     2050 2022-07-20 15:27:03.000000 ngsfragments-2.0.3/htslib/version.sh
--rw-r--r--   0        0        0    10244 2023-05-17 14:05:23.719714 ngsfragments-2.0.3/ngsfragments/.DS_Store
--rwxr-xr-x   0        0        0      373 2023-05-17 14:40:17.916128 ngsfragments-2.0.3/ngsfragments/__init__.py
--rwxr-xr-x   0        0        0      187 2023-05-17 14:30:53.525375 ngsfragments-2.0.3/ngsfragments/config.py
--rwxr-xr-x   0        0        0      167 2023-03-21 14:48:14.313666 ngsfragments-2.0.3/ngsfragments/correct/__init__.py
--rw-r--r--   0        0        0     2307 2023-05-11 20:03:38.317861 ngsfragments-2.0.3/ngsfragments/correct/correct_intervals.py
--rwxr-xr-x   0        0        0     5810 2023-05-11 20:02:33.042562 ngsfragments-2.0.3/ngsfragments/correct/correction.py
--rwxr-xr-x   0        0        0       92 2022-10-10 20:36:54.000000 ngsfragments-2.0.3/ngsfragments/correct/cylowess/__init__.py
--rw-r--r--   0        0        0   482168 2023-03-21 14:00:47.861831 ngsfragments-2.0.3/ngsfragments/correct/cylowess/cylowess.c
--rw-r--r--   0        0        0   122648 2023-05-17 14:31:15.704092 ngsfragments-2.0.3/ngsfragments/correct/cylowess/cylowess.cpython-310-darwin.so
--rw-r--r--   0        0        0    21292 2023-03-21 14:00:31.232217 ngsfragments-2.0.3/ngsfragments/correct/cylowess/cylowess.pyx
--rwxr-xr-x   0        0        0       92 2023-02-07 15:14:21.258083 ngsfragments-2.0.3/ngsfragments/coverage/__init__.py
--rw-r--r--   0        0        0     7595 2023-05-15 20:07:54.689766 ngsfragments-2.0.3/ngsfragments/coverage/coverage.py
--rw-r--r--   0        0        0      903 2023-05-15 20:08:26.702773 ngsfragments-2.0.3/ngsfragments/coverage/midpoint.py
--rw-r--r--   0        0        0     5152 2023-05-15 20:09:35.205474 ngsfragments-2.0.3/ngsfragments/coverage/wps.py
--rwxr-xr-x   0        0        0     5060 2023-05-15 19:58:24.489625 ngsfragments-2.0.3/ngsfragments/fragments.py
--rwxr-xr-x   0        0        0       82 2023-02-01 19:26:53.531065 ngsfragments-2.0.3/ngsfragments/io/__init__.py
--rw-r--r--   0        0        0  1003390 2023-02-01 19:58:16.917570 ngsfragments-2.0.3/ngsfragments/io/parse_sam/ReadSam.c
--rw-r--r--   0        0        0  1146848 2023-05-17 14:31:15.702701 ngsfragments-2.0.3/ngsfragments/io/parse_sam/ReadSam.cpython-310-darwin.so
--rwxr-xr-x   0        0        0     2651 2022-12-14 19:52:53.000000 ngsfragments-2.0.3/ngsfragments/io/parse_sam/ReadSam.pxd
--rwxr-xr-x   0        0        0     5730 2022-12-14 20:20:03.000000 ngsfragments-2.0.3/ngsfragments/io/parse_sam/ReadSam.pyx
--rwxr-xr-x   0        0        0       99 2022-07-20 15:26:56.000000 ngsfragments-2.0.3/ngsfragments/io/parse_sam/__init__.py
--rwxr-xr-x   0        0        0     7494 2022-12-14 20:33:54.000000 ngsfragments-2.0.3/ngsfragments/io/parse_sam/read_intervals.c
--rwxr-xr-x   0        0        0     1406 2022-12-14 19:52:12.000000 ngsfragments-2.0.3/ngsfragments/io/parse_sam/read_intervals.h
--rwxr-xr-x   0        0        0     7885 2022-07-20 15:26:56.000000 ngsfragments-2.0.3/ngsfragments/io/parse_sam/read_intervals_v0.c
--rw-r--r--   0        0        0     2823 2023-05-15 20:13:08.300015 ngsfragments-2.0.3/ngsfragments/io/read_sam.py
--rwxr-xr-x   0        0        0       80 2023-02-10 22:01:53.060407 ngsfragments-2.0.3/ngsfragments/metrics/__init__.py
--rw-r--r--   0        0        0     3820 2023-05-15 20:12:08.740246 ngsfragments-2.0.3/ngsfragments/metrics/gc_metrics.py
--rw-r--r--   0        0        0    10545 2023-05-11 20:08:15.832145 ngsfragments-2.0.3/ngsfragments/metrics/gene_activity.py
--rw-r--r--   0        0        0      267 2023-03-05 16:12:26.726790 ngsfragments-2.0.3/ngsfragments/metrics/wps_metrics.py
--rw-r--r--   0        0        0     6148 2023-02-10 21:54:33.607661 ngsfragments-2.0.3/ngsfragments/peak_calling/.DS_Store
--rw-r--r--   0        0        0   916514 2023-02-10 22:01:41.328107 ngsfragments-2.0.3/ngsfragments/peak_calling/CallPeaks.c
--rw-r--r--   0        0        0   220576 2023-05-17 14:31:15.703627 ngsfragments-2.0.3/ngsfragments/peak_calling/CallPeaks.cpython-310-darwin.so
--rwxr-xr-x   0        0        0      475 2023-02-10 21:54:21.291585 ngsfragments-2.0.3/ngsfragments/peak_calling/CallPeaks.pxd
--rwxr-xr-x   0        0        0     2786 2023-02-10 21:54:06.026216 ngsfragments-2.0.3/ngsfragments/peak_calling/CallPeaks.pyx
--rw-r--r--   0        0        0   852272 2022-09-15 14:37:09.000000 ngsfragments-2.0.3/ngsfragments/peak_calling/RunningMean.c
--rw-r--r--   0        0        0   142536 2023-05-17 14:31:15.703299 ngsfragments-2.0.3/ngsfragments/peak_calling/RunningMean.cpython-310-darwin.so
--rwxr-xr-x   0        0        0      519 2022-07-20 15:26:57.000000 ngsfragments-2.0.3/ngsfragments/peak_calling/RunningMean.pxd
--rwxr-xr-x   0        0        0      681 2022-07-20 15:26:57.000000 ngsfragments-2.0.3/ngsfragments/peak_calling/RunningMean.pyx
--rw-r--r--   0        0        0   864899 2022-09-15 14:37:06.000000 ngsfragments-2.0.3/ngsfragments/peak_calling/RunningMedian.c
--rw-r--r--   0        0        0   143792 2023-05-17 14:31:15.703073 ngsfragments-2.0.3/ngsfragments/peak_calling/RunningMedian.cpython-310-darwin.so
--rwxr-xr-x   0        0        0      557 2022-07-20 15:26:57.000000 ngsfragments-2.0.3/ngsfragments/peak_calling/RunningMedian.pxd
--rwxr-xr-x   0        0        0     1973 2022-07-20 15:26:57.000000 ngsfragments-2.0.3/ngsfragments/peak_calling/RunningMedian.pyx
--rwxr-xr-x   0        0        0      196 2023-02-01 18:05:20.025593 ngsfragments-2.0.3/ngsfragments/peak_calling/__init__.py
--rwxr-xr-x   0        0        0     1056 2022-07-20 15:26:57.000000 ngsfragments-2.0.3/ngsfragments/peak_calling/running_mean.c
--rwxr-xr-x   0        0        0      283 2022-07-20 15:26:57.000000 ngsfragments-2.0.3/ngsfragments/peak_calling/running_mean.h
--rwxr-xr-x   0        0        0     8413 2022-07-20 15:26:57.000000 ngsfragments-2.0.3/ngsfragments/peak_calling/sklist_pd.c
--rwxr-xr-x   0        0        0     1158 2022-07-20 15:26:57.000000 ngsfragments-2.0.3/ngsfragments/peak_calling/sklist_pd.h
--rwxr-xr-x   0        0        0       75 2022-07-20 15:26:57.000000 ngsfragments-2.0.3/ngsfragments/plot/__init__.py
--rwxr-xr-x   0        0        0     4657 2022-07-20 15:26:57.000000 ngsfragments-2.0.3/ngsfragments/plot/plot_bokeh.py
--rwxr-xr-x   0        0        0    13815 2023-05-17 13:34:28.507840 ngsfragments-2.0.3/ngsfragments/plot/plot_plt.py
--rw-r--r--   0        0        0     6148 2023-05-11 20:09:53.010855 ngsfragments-2.0.3/ngsfragments/segment/.DS_Store
--rwxr-xr-x   0        0        0      139 2023-05-13 14:22:26.939358 ngsfragments-2.0.3/ngsfragments/segment/__init__.py
--rwxr-xr-x   0        0        0     3649 2023-05-13 14:23:49.399762 ngsfragments-2.0.3/ngsfragments/segment/cnv.py
--rwxr-xr-x   0        0        0    22506 2023-05-12 20:21:02.644767 ngsfragments-2.0.3/ngsfragments/segment/cnv_pipeline.py
--rwxr-xr-x   0        0        0    16333 2023-05-12 20:43:03.845216 ngsfragments-2.0.3/ngsfragments/segment/cnv_utilities.py
--rwxr-xr-x   0        0        0       97 2022-07-20 15:26:56.000000 ngsfragments-2.0.3/ngsfragments/segment/smooth_cnv/__init__.py
--rwxr-xr-x   0        0        0     2924 2022-07-20 15:26:56.000000 ngsfragments-2.0.3/ngsfragments/segment/smooth_cnv/smoothCNV.c
--rwxr-xr-x   0        0        0      285 2022-07-20 15:26:57.000000 ngsfragments-2.0.3/ngsfragments/segment/smooth_cnv/smoothCNV.h
--rw-r--r--   0        0        0   926261 2023-02-01 19:58:17.916519 ngsfragments-2.0.3/ngsfragments/segment/smooth_cnv/smooth_cnv.c
--rw-r--r--   0        0        0   159088 2023-05-17 14:31:15.703895 ngsfragments-2.0.3/ngsfragments/segment/smooth_cnv/smooth_cnv.cpython-310-darwin.so
--rwxr-xr-x   0        0        0      304 2022-07-20 15:26:56.000000 ngsfragments-2.0.3/ngsfragments/segment/smooth_cnv/smooth_cnv.pxd
--rwxr-xr-x   0        0        0     1469 2022-07-20 15:26:56.000000 ngsfragments-2.0.3/ngsfragments/segment/smooth_cnv/smooth_cnv.pyx
--rwxr-xr-x   0        0        0      104 2023-03-21 14:53:46.744822 ngsfragments-2.0.3/ngsfragments/sequence/__init__.py
--rw-r--r--   0        0        0     1488 2023-02-01 21:52:11.526397 ngsfragments-2.0.3/ngsfragments/sequence/kmer_query.py
--rw-r--r--   0        0        0      458 2023-01-31 18:53:12.818067 ngsfragments-2.0.3/ngsfragments/sequence/sequence_query.py
--rwxr-xr-x   0        0        0       61 2023-01-31 21:54:53.387281 ngsfragments-2.0.3/ngsfragments/sequence/snp_calling/__init__.py
--rw-r--r--   0        0        0   975270 2023-02-01 19:58:19.931481 ngsfragments-2.0.3/ngsfragments/sequence/snp_calling/snp_calling.c
--rw-r--r--   0        0        0      815 2023-02-01 12:46:55.639263 ngsfragments-2.0.3/ngsfragments/sequence/snp_calling/snp_calling.pxd
--rw-r--r--   0        0        0     5077 2023-02-01 13:17:00.089609 ngsfragments-2.0.3/ngsfragments/sequence/snp_calling/snp_calling.pyx
--rwxr-xr-x   0        0        0     6870 2023-05-15 15:11:02.820550 ngsfragments-2.0.3/ngsfragments/utilities.py
--rw-r--r--   0        0        0     2635 2023-05-17 14:41:03.841426 ngsfragments-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     3073 1970-01-01 00:00:00.000000 ngsfragments-2.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0    17895 2022-07-20 15:26:56.000000 ngsfragments-2.0.4/LICENSE.md
+-rwxr-xr-x   0        0        0      898 2022-07-20 15:27:17.000000 ngsfragments-2.0.4/README.md
+-rwxr-xr-x   0        0        0    18935 2023-05-17 14:27:58.055055 ngsfragments-2.0.4/build.py
+-rwxr-xr-x   0        0        0     3094 2023-05-17 16:12:18.128008 ngsfragments-2.0.4/cy_build.py
+-rwxr-xr-x   0        0        0    10408 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/INSTALL
+-rwxr-xr-x   0        0        0     3540 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/LICENSE
+-rwxr-xr-x   0        0        0    37612 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/Makefile
+-rwxr-xr-x   0        0        0    59421 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/NEWS
+-rwxr-xr-x   0        0        0      273 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/README
+-rwxr-xr-x   0        0        0     7784 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/README.large_positions.md
+-rwxr-xr-x   0        0        0    22063 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/bcf_sr_sort.c
+-rwxr-xr-x   0        0        0     3869 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/bcf_sr_sort.h
+-rwxr-xr-x   0        0        0    81402 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/bgzf.c
+-rwxr-xr-x   0        0        0     5527 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/bgzip.1
+-rwxr-xr-x   0        0        0    15526 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/bgzip.c
+-rw-r--r--   0        0        0     4122 2022-07-20 16:25:07.000000 ngsfragments-2.0.4/htslib/config.h
+-rwxr-xr-x   0        0        0     3823 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/config.h.in
+-rwxr-xr-x   0        0        0    36411 2023-05-17 16:19:32.487973 ngsfragments-2.0.4/htslib/config.log
+-rw-r--r--   0        0        0     3977 2023-05-17 16:19:32.235494 ngsfragments-2.0.4/htslib/config.mk
+-rwxr-xr-x   0        0        0     3546 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/config.mk.in
+-rwxr-xr-x   0        0        0    29819 2023-05-17 16:19:31.967184 ngsfragments-2.0.4/htslib/config.status
+-rwxr-xr-x   0        0        0      801 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/config_vars.h
+-rwxr-xr-x   0        0        0   193602 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/configure
+-rwxr-xr-x   0        0        0    17917 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/configure.ac
+-rwxr-xr-x   0        0        0     2420 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/cram/cram.h
+-rwxr-xr-x   0        0        0   121685 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/cram/cram_codecs.c
+-rwxr-xr-x   0        0        0     8507 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/cram/cram_codecs.h
+-rwxr-xr-x   0        0        0   124456 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/cram/cram_decode.c
+-rwxr-xr-x   0        0        0     3695 2022-07-20 15:27:01.000000 ngsfragments-2.0.4/htslib/cram/cram_decode.h
+-rwxr-xr-x   0        0        0   124228 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/cram/cram_encode.c
+-rwxr-xr-x   0        0        0     3630 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/cram/cram_encode.h
+-rwxr-xr-x   0        0        0    13526 2022-07-20 15:27:01.000000 ngsfragments-2.0.4/htslib/cram/cram_external.c
+-rwxr-xr-x   0        0        0    22609 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/cram/cram_index.c
+-rwxr-xr-x   0        0        0     3866 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/cram/cram_index.h
+-rwxr-xr-x   0        0        0   170538 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/cram/cram_io.c
+-rwxr-xr-x   0        0        0    18202 2022-07-20 15:27:01.000000 ngsfragments-2.0.4/htslib/cram/cram_io.h
+-rwxr-xr-x   0        0        0     2911 2022-07-20 15:27:01.000000 ngsfragments-2.0.4/htslib/cram/cram_samtools.h
+-rwxr-xr-x   0        0        0     7036 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/cram/cram_stats.c
+-rwxr-xr-x   0        0        0     2273 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/cram/cram_stats.h
+-rwxr-xr-x   0        0        0    28993 2022-07-20 15:27:01.000000 ngsfragments-2.0.4/htslib/cram/cram_structs.h
+-rwxr-xr-x   0        0        0    17233 2022-07-20 15:27:01.000000 ngsfragments-2.0.4/htslib/cram/mFILE.c
+-rwxr-xr-x   0        0        0     3075 2022-07-20 15:27:01.000000 ngsfragments-2.0.4/htslib/cram/mFILE.h
+-rwxr-xr-x   0        0        0     3371 2022-07-20 15:27:01.000000 ngsfragments-2.0.4/htslib/cram/misc.h
+-rwxr-xr-x   0        0        0    13991 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/cram/open_trace_file.c
+-rwxr-xr-x   0        0        0     5027 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/cram/open_trace_file.h
+-rwxr-xr-x   0        0        0     6816 2022-07-20 15:27:01.000000 ngsfragments-2.0.4/htslib/cram/os.h
+-rwxr-xr-x   0        0        0     5049 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/cram/pooled_alloc.c
+-rwxr-xr-x   0        0        0     2185 2022-07-20 15:27:01.000000 ngsfragments-2.0.4/htslib/cram/pooled_alloc.h
+-rwxr-xr-x   0        0        0     4422 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/cram/string_alloc.c
+-rwxr-xr-x   0        0        0     2356 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/cram/string_alloc.h
+-rwxr-xr-x   0        0        0     6757 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/errmod.c
+-rwxr-xr-x   0        0        0     6262 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/faidx.5
+-rwxr-xr-x   0        0        0    27085 2022-07-20 15:27:01.000000 ngsfragments-2.0.4/htslib/faidx.c
+-rwxr-xr-x   0        0        0    79879 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/header.c
+-rwxr-xr-x   0        0        0    10466 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/header.h
+-rwxr-xr-x   0        0        0    39697 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/hfile.c
+-rwxr-xr-x   0        0        0     4426 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/hfile_gcs.c
+-rwxr-xr-x   0        0        0     8028 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/hfile_internal.h
+-rwxr-xr-x   0        0        0    48933 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/hfile_libcurl.c
+-rwxr-xr-x   0        0        0    36420 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/hfile_s3.c
+-rwxr-xr-x   0        0        0    24147 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/hfile_s3_write.c
+-rwxr-xr-x   0        0        0   145540 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/hts.c
+-rwxr-xr-x   0        0        0    20714 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/hts_expr.c
+-rwxr-xr-x   0        0        0     5756 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/hts_internal.h
+-rwxr-xr-x   0        0        0     1981 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/hts_os.c
+-rwxr-xr-x   0        0        0     2160 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/LICENSE.md
+-rwxr-xr-x   0        0        0     1442 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/htscodecs/NEWS
+-rwxr-xr-x   0        0        0    29564 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/htscodecs/arith_dynamic.c
+-rwxr-xr-x   0        0        0     2371 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/htscodecs/arith_dynamic.h
+-rwxr-xr-x   0        0        0     3426 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/htscodecs/c_range_coder.h
+-rwxr-xr-x   0        0        0     5630 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/htscodecs/c_simple_model.h
+-rwxr-xr-x   0        0        0    40365 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/htscodecs/fqzcomp_qual.c
+-rwxr-xr-x   0        0        0     6183 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/htscodecs/fqzcomp_qual.h
+-rwxr-xr-x   0        0        0     1957 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/htscodecs/htscodecs.c
+-rwxr-xr-x   0        0        0     2286 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/htscodecs/htscodecs.h
+-rwxr-xr-x   0        0        0     3557 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/htscodecs/htscodecs_endian.h
+-rwxr-xr-x   0        0        0     9091 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/htscodecs/pack.c
+-rwxr-xr-x   0        0        0     3257 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/htscodecs/pack.h
+-rwxr-xr-x   0        0        0     3972 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/htscodecs/pooled_alloc.h
+-rwxr-xr-x   0        0        0    18532 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/htscodecs/rANS_byte.h
+-rwxr-xr-x   0        0        0    24585 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/htscodecs/rANS_static.c
+-rwxr-xr-x   0        0        0     2037 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/htscodecs/rANS_static.h
+-rwxr-xr-x   0        0        0     2414 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/htscodecs/rANS_static4x16.h
+-rwxr-xr-x   0        0        0    43110 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/htscodecs/rANS_static4x16pr.c
+-rwxr-xr-x   0        0        0    13920 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/htscodecs/rANS_word.h
+-rwxr-xr-x   0        0        0     5225 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/htscodecs/rle.c
+-rwxr-xr-x   0        0        0     3690 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/htscodecs/rle.h
+-rwxr-xr-x   0        0        0    51137 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/htscodecs/tokenise_name3.c
+-rwxr-xr-x   0        0        0     2557 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/htscodecs/tokenise_name3.h
+-rwxr-xr-x   0        0        0     5615 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/htscodecs/utils.h
+-rwxr-xr-x   0        0        0     7224 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/htscodecs/varint.h
+-rwxr-xr-x   0        0        0     9004 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/htscodecs/varint2.h
+-rwxr-xr-x   0        0        0       37 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/htscodecs/version.h
+-rwxr-xr-x   0        0        0      856 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/arith.test
+-rwxr-xr-x   0        0        0     2896 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/arith_dynamic_fuzz.c
+-rwxr-xr-x   0        0        0     7402 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/arith_dynamic_test.c
+-rwxr-xr-x   0        0        0    11615 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q4.0
+-rwxr-xr-x   0        0        0    10831 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q4.1
+-rwxr-xr-x   0        0        0    10774 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q4.128
+-rwxr-xr-x   0        0        0    10329 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q4.129
+-rwxr-xr-x   0        0        0    11095 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q4.192
+-rwxr-xr-x   0        0        0    10283 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q4.193
+-rwxr-xr-x   0        0        0    13360 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q4.64
+-rwxr-xr-x   0        0        0    10484 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q4.65
+-rwxr-xr-x   0        0        0    11448 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q4.8
+-rwxr-xr-x   0        0        0    11083 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q4.9
+-rwxr-xr-x   0        0        0    49949 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q40+dir.0
+-rwxr-xr-x   0        0        0    49034 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q40+dir.1
+-rwxr-xr-x   0        0        0    51242 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q40+dir.64
+-rwxr-xr-x   0        0        0    49061 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q40+dir.65
+-rwxr-xr-x   0        0        0    49820 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q40+dir.8
+-rwxr-xr-x   0        0        0    49448 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q40+dir.9
+-rwxr-xr-x   0        0        0    32752 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q8.0
+-rwxr-xr-x   0        0        0    31331 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q8.1
+-rwxr-xr-x   0        0        0    32063 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q8.128
+-rwxr-xr-x   0        0        0    31084 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q8.129
+-rwxr-xr-x   0        0        0    32267 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q8.192
+-rwxr-xr-x   0        0        0    30931 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q8.193
+-rwxr-xr-x   0        0        0    35211 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q8.64
+-rwxr-xr-x   0        0        0    30907 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q8.65
+-rwxr-xr-x   0        0        0    32597 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/qvar.0
+-rwxr-xr-x   0        0        0    31982 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/qvar.1
+-rwxr-xr-x   0        0        0    33237 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/qvar.64
+-rwxr-xr-x   0        0        0    31993 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/qvar.65
+-rwxr-xr-x   0        0        0     9307 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/q4.0
+-rwxr-xr-x   0        0        0     9618 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/q4.1
+-rwxr-xr-x   0        0        0     9453 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/q4.2
+-rwxr-xr-x   0        0        0    10481 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/q4.3
+-rwxr-xr-x   0        0        0    47712 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/q40+dir.0
+-rwxr-xr-x   0        0        0    43803 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/q40+dir.1
+-rwxr-xr-x   0        0        0    47233 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/q40+dir.2
+-rwxr-xr-x   0        0        0    48485 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/q40+dir.3
+-rwxr-xr-x   0        0        0    30012 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/q8.0
+-rwxr-xr-x   0        0        0    33742 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/q8.1
+-rwxr-xr-x   0        0        0    30982 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/q8.2
+-rwxr-xr-x   0        0        0    31709 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/q8.3
+-rwxr-xr-x   0        0        0    32868 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/qvar.0
+-rwxr-xr-x   0        0        0    35007 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/qvar.1
+-rwxr-xr-x   0        0        0    32400 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/qvar.2
+-rwxr-xr-x   0        0        0    32073 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/qvar.3
+-rwxr-xr-x   0        0        0   152000 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/q4
+-rwxr-xr-x   0        0        0   103000 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/q40+dir
+-rwxr-xr-x   0        0        0   147383 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/q8
+-rwxr-xr-x   0        0        0    62441 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/qvar
+-rwxr-xr-x   0        0        0    11660 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q4.0
+-rwxr-xr-x   0        0        0    10848 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q4.1
+-rwxr-xr-x   0        0        0    10902 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q4.128
+-rwxr-xr-x   0        0        0    10890 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q4.129
+-rwxr-xr-x   0        0        0    11225 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q4.192
+-rwxr-xr-x   0        0        0    10825 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q4.193
+-rwxr-xr-x   0        0        0    12878 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q4.64
+-rwxr-xr-x   0        0        0    10672 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q4.65
+-rwxr-xr-x   0        0        0    11731 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q4.8
+-rwxr-xr-x   0        0        0    11111 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q4.9
+-rwxr-xr-x   0        0        0    50247 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q40+dir.0
+-rwxr-xr-x   0        0        0    49449 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q40+dir.1
+-rwxr-xr-x   0        0        0    50072 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q40+dir.8
+-rwxr-xr-x   0        0        0    50072 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q40+dir.9
+-rwxr-xr-x   0        0        0    33088 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q8.0
+-rwxr-xr-x   0        0        0    31372 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q8.1
+-rwxr-xr-x   0        0        0    32237 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q8.128
+-rwxr-xr-x   0        0        0    31258 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q8.129
+-rwxr-xr-x   0        0        0    32024 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q8.192
+-rwxr-xr-x   0        0        0    31146 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q8.193
+-rwxr-xr-x   0        0        0    33458 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q8.64
+-rwxr-xr-x   0        0        0    31025 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q8.65
+-rwxr-xr-x   0        0        0    32987 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/qvar.0
+-rwxr-xr-x   0        0        0    32261 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/qvar.1
+-rwxr-xr-x   0        0        0    11674 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x8/q4.0
+-rwxr-xr-x   0        0        0    10870 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x8/q4.1
+-rwxr-xr-x   0        0        0    50258 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x8/q40+dir.0
+-rwxr-xr-x   0        0        0    50537 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x8/q40+dir.1
+-rwxr-xr-x   0        0        0    33099 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x8/q8.0
+-rwxr-xr-x   0        0        0    31428 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x8/q8.1
+-rwxr-xr-x   0        0        0    32997 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x8/qvar.0
+-rwxr-xr-x   0        0        0    32832 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x8/qvar.1
+-rwxr-xr-x   0        0        0      753 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/fqzcomp.test
+-rwxr-xr-x   0        0        0     3055 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/fqzcomp_qual_fuzz.c
+-rwxr-xr-x   0        0        0    12136 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/fqzcomp_qual_test.c
+-rwxr-xr-x   0        0        0    45893 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/01.names
+-rwxr-xr-x   0        0        0    41060 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/02.names
+-rwxr-xr-x   0        0        0    77358 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/03.names
+-rwxr-xr-x   0        0        0    32489 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/05.names
+-rwxr-xr-x   0        0        0    86076 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/08.names
+-rwxr-xr-x   0        0        0    18000 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/09.names
+-rwxr-xr-x   0        0        0    38232 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/10.names
+-rwxr-xr-x   0        0        0    32912 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/20.names
+-rwxr-xr-x   0        0        0    39455 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/nv.names
+-rwxr-xr-x   0        0        0    38516 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/nv2.names
+-rwxr-xr-x   0        0        0    36899 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/rr.names
+-rwxr-xr-x   0        0        0     3842 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/01.names.1
+-rwxr-xr-x   0        0        0     3566 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/01.names.11
+-rwxr-xr-x   0        0        0     2424 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/01.names.13
+-rwxr-xr-x   0        0        0     2087 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/01.names.15
+-rwxr-xr-x   0        0        0     2051 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/01.names.17
+-rwxr-xr-x   0        0        0     2049 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/01.names.19
+-rwxr-xr-x   0        0        0     2471 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/01.names.3
+-rwxr-xr-x   0        0        0     2334 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/01.names.5
+-rwxr-xr-x   0        0        0     2234 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/01.names.7
+-rwxr-xr-x   0        0        0     2234 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/01.names.9
+-rwxr-xr-x   0        0        0     7041 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/02.names.1
+-rwxr-xr-x   0        0        0     6468 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/02.names.11
+-rwxr-xr-x   0        0        0     4797 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/02.names.13
+-rwxr-xr-x   0        0        0     4749 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/02.names.15
+-rwxr-xr-x   0        0        0     4695 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/02.names.17
+-rwxr-xr-x   0        0        0     4695 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/02.names.19
+-rwxr-xr-x   0        0        0     4983 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/02.names.3
+-rwxr-xr-x   0        0        0     4983 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/02.names.5
+-rwxr-xr-x   0        0        0     4922 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/02.names.7
+-rwxr-xr-x   0        0        0     4918 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/02.names.9
+-rwxr-xr-x   0        0        0    11237 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/03.names.1
+-rwxr-xr-x   0        0        0     9798 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/03.names.11
+-rwxr-xr-x   0        0        0     7291 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/03.names.13
+-rwxr-xr-x   0        0        0     7255 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/03.names.15
+-rwxr-xr-x   0        0        0     7069 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/03.names.17
+-rwxr-xr-x   0        0        0     7068 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/03.names.19
+-rwxr-xr-x   0        0        0     7822 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/03.names.3
+-rwxr-xr-x   0        0        0     7822 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/03.names.5
+-rwxr-xr-x   0        0        0     7521 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/03.names.7
+-rwxr-xr-x   0        0        0     7521 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/03.names.9
+-rwxr-xr-x   0        0        0     5356 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/05.names.1
+-rwxr-xr-x   0        0        0     4869 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/05.names.11
+-rwxr-xr-x   0        0        0     3405 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/05.names.13
+-rwxr-xr-x   0        0        0     3404 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/05.names.15
+-rwxr-xr-x   0        0        0     3377 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/05.names.17
+-rwxr-xr-x   0        0        0     3377 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/05.names.19
+-rwxr-xr-x   0        0        0     3600 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/05.names.3
+-rwxr-xr-x   0        0        0     3600 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/05.names.5
+-rwxr-xr-x   0        0        0     3534 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/05.names.7
+-rwxr-xr-x   0        0        0     3534 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/05.names.9
+-rwxr-xr-x   0        0        0     7324 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/08.names.1
+-rwxr-xr-x   0        0        0     6804 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/08.names.11
+-rwxr-xr-x   0        0        0     4895 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/08.names.13
+-rwxr-xr-x   0        0        0     4894 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/08.names.15
+-rwxr-xr-x   0        0        0     4805 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/08.names.17
+-rwxr-xr-x   0        0        0     4805 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/08.names.19
+-rwxr-xr-x   0        0        0     5291 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/08.names.3
+-rwxr-xr-x   0        0        0     5291 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/08.names.5
+-rwxr-xr-x   0        0        0     5160 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/08.names.7
+-rwxr-xr-x   0        0        0     5160 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/08.names.9
+-rwxr-xr-x   0        0        0     5411 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/09.names.1
+-rwxr-xr-x   0        0        0     4898 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/09.names.11
+-rwxr-xr-x   0        0        0     3427 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/09.names.13
+-rwxr-xr-x   0        0        0     3427 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/09.names.15
+-rwxr-xr-x   0        0        0     3366 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/09.names.17
+-rwxr-xr-x   0        0        0     3366 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/09.names.19
+-rwxr-xr-x   0        0        0     3598 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/09.names.3
+-rwxr-xr-x   0        0        0     3598 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/09.names.5
+-rwxr-xr-x   0        0        0     3493 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/09.names.7
+-rwxr-xr-x   0        0        0     3493 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/09.names.9
+-rwxr-xr-x   0        0        0     6881 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/10.names.1
+-rwxr-xr-x   0        0        0     6204 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/10.names.11
+-rwxr-xr-x   0        0        0     4567 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/10.names.13
+-rwxr-xr-x   0        0        0     4558 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/10.names.15
+-rwxr-xr-x   0        0        0     4472 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/10.names.17
+-rwxr-xr-x   0        0        0     4472 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/10.names.19
+-rwxr-xr-x   0        0        0     4843 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/10.names.3
+-rwxr-xr-x   0        0        0     4843 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/10.names.5
+-rwxr-xr-x   0        0        0     4746 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/10.names.7
+-rwxr-xr-x   0        0        0     4744 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/10.names.9
+-rwxr-xr-x   0        0        0     2956 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/20.names.1
+-rwxr-xr-x   0        0        0     2732 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/20.names.11
+-rwxr-xr-x   0        0        0     1626 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/20.names.13
+-rwxr-xr-x   0        0        0     1625 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/20.names.15
+-rwxr-xr-x   0        0        0     1600 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/20.names.17
+-rwxr-xr-x   0        0        0     1600 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/20.names.19
+-rwxr-xr-x   0        0        0     1695 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/20.names.3
+-rwxr-xr-x   0        0        0     1695 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/20.names.5
+-rwxr-xr-x   0        0        0     1632 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/20.names.7
+-rwxr-xr-x   0        0        0     1632 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/20.names.9
+-rwxr-xr-x   0        0        0     7168 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv.names.1
+-rwxr-xr-x   0        0        0     6426 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv.names.11
+-rwxr-xr-x   0        0        0     4825 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv.names.13
+-rwxr-xr-x   0        0        0     4787 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv.names.15
+-rwxr-xr-x   0        0        0     4767 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv.names.17
+-rwxr-xr-x   0        0        0     4767 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv.names.19
+-rwxr-xr-x   0        0        0     4989 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv.names.3
+-rwxr-xr-x   0        0        0     4989 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv.names.5
+-rwxr-xr-x   0        0        0     4937 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv.names.7
+-rwxr-xr-x   0        0        0     4937 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv.names.9
+-rwxr-xr-x   0        0        0     1718 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv2.names.1
+-rwxr-xr-x   0        0        0     1411 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv2.names.11
+-rwxr-xr-x   0        0        0      836 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv2.names.13
+-rwxr-xr-x   0        0        0      809 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv2.names.15
+-rwxr-xr-x   0        0        0      747 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv2.names.17
+-rwxr-xr-x   0        0        0      747 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv2.names.19
+-rwxr-xr-x   0        0        0      903 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv2.names.3
+-rwxr-xr-x   0        0        0      903 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv2.names.5
+-rwxr-xr-x   0        0        0      846 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv2.names.7
+-rwxr-xr-x   0        0        0      846 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv2.names.9
+-rwxr-xr-x   0        0        0     9012 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/rr.names.1
+-rwxr-xr-x   0        0        0     8513 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/rr.names.11
+-rwxr-xr-x   0        0        0     6066 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/rr.names.13
+-rwxr-xr-x   0        0        0     5979 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/rr.names.15
+-rwxr-xr-x   0        0        0     5963 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/rr.names.17
+-rwxr-xr-x   0        0        0     5963 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/rr.names.19
+-rwxr-xr-x   0        0        0     6288 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/rr.names.3
+-rwxr-xr-x   0        0        0     6286 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/rr.names.5
+-rwxr-xr-x   0        0        0     6230 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/rr.names.7
+-rwxr-xr-x   0        0        0     6230 2022-07-20 15:27:08.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/rr.names.9
+-rwxr-xr-x   0        0        0     3807 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/rANS_static4x16pr_fuzz.c
+-rwxr-xr-x   0        0        0     7770 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/rANS_static4x16pr_test.c
+-rwxr-xr-x   0        0        0     3951 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/rANS_static_fuzz.c
+-rwxr-xr-x   0        0        0     7315 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/rANS_static_test.c
+-rwxr-xr-x   0        0        0      842 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/rans4x16.test
+-rwxr-xr-x   0        0        0      742 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/rans4x8.test
+-rwxr-xr-x   0        0        0      667 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/tok3.test
+-rwxr-xr-x   0        0        0     2973 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/tokenise_name3_fuzz.c
+-rwxr-xr-x   0        0        0     5533 2022-07-20 15:27:07.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/tokenise_name3_test.c
+-rwxr-xr-x   0        0        0    10245 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htscodecs/tests/varint_test.c
+-rw-r--r--   0        0        0      162 2023-05-17 16:19:32.293841 ngsfragments-2.0.4/htslib/htscodecs.mk
+-rwxr-xr-x   0        0        0      123 2022-07-20 15:27:01.000000 ngsfragments-2.0.4/htslib/htscodecs.mk.in
+-rwxr-xr-x   0        0        0     3083 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/htscodecs_bundled.mk
+-rwxr-xr-x   0        0        0     1710 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/htscodecs_external.mk
+-rwxr-xr-x   0        0        0     3856 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/htsfile.1
+-rwxr-xr-x   0        0        0     9607 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/htsfile.c
+-rwxr-xr-x   0        0        0    16081 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/htslib/bgzf.h
+-rwxr-xr-x   0        0        0    16837 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/htslib/cram.h
+-rwxr-xr-x   0        0        0    12934 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/htslib/faidx.h
+-rwxr-xr-x   0        0        0    12877 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/htslib/hfile.h
+-rwxr-xr-x   0        0        0    52935 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/htslib/hts.h
+-rwxr-xr-x   0        0        0     3989 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/htslib/hts_defs.h
+-rwxr-xr-x   0        0        0    11485 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/htslib/hts_endian.h
+-rwxr-xr-x   0        0        0     3760 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/htslib/hts_expr.h
+-rwxr-xr-x   0        0        0     3944 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/htslib/hts_log.h
+-rwxr-xr-x   0        0        0     2533 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/htslib/hts_os.h
+-rwxr-xr-x   0        0        0     5605 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/htslib/kbitset.h
+-rwxr-xr-x   0        0        0     2828 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/htslib/kfunc.h
+-rwxr-xr-x   0        0        0    22899 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/htslib/khash.h
+-rwxr-xr-x   0        0        0     4050 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/htslib/khash_str2int.h
+-rwxr-xr-x   0        0        0     5135 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/htslib/klist.h
+-rwxr-xr-x   0        0        0     3362 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/htslib/knetfile.h
+-rwxr-xr-x   0        0        0     3295 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/htslib/kroundup.h
+-rwxr-xr-x   0        0        0     8830 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/htslib/kseq.h
+-rwxr-xr-x   0        0        0    11480 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/htslib/ksort.h
+-rwxr-xr-x   0        0        0    11090 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/htslib/kstring.h
+-rwxr-xr-x   0        0        0     8881 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/htslib/regidx.h
+-rwxr-xr-x   0        0        0    78275 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/htslib/sam.h
+-rwxr-xr-x   0        0        0    15800 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/htslib/synced_bcf_reader.h
+-rwxr-xr-x   0        0        0     4942 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/htslib/tbx.h
+-rwxr-xr-x   0        0        0    12747 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/htslib/thread_pool.h
+-rwxr-xr-x   0        0        0    62511 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/htslib/vcf.h
+-rwxr-xr-x   0        0        0     1686 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/htslib/vcf_sweep.h
+-rwxr-xr-x   0        0        0     4919 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/htslib/vcfutils.h
+-rwxr-xr-x   0        0        0     4561 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/htslib-s3-plugin.7
+-rwxr-xr-x   0        0        0     6530 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/htslib.mk
+-rwxr-xr-x   0        0        0      490 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/htslib.pc.in
+-rw-r--r--   0        0        0      784 2023-05-17 16:19:32.364304 ngsfragments-2.0.4/htslib/htslib.pc.tmp
+-rwxr-xr-x   0        0        0     3312 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/htslib_vars.mk
+-rwxr-xr-x   0        0        0    10879 2022-07-20 15:27:01.000000 ngsfragments-2.0.4/htslib/kfunc.c
+-rwxr-xr-x   0        0        0    10570 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/kstring.c
+-rwxr-xr-x   0        0        0     2604 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/m4/hts_hide_dynamic_syms.m4
+-rwxr-xr-x   0        0        0     8273 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/m4/hts_prog_cc_warnings.m4
+-rwxr-xr-x   0        0        0    10244 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/m4/pkg.m4
+-rwxr-xr-x   0        0        0    10656 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/md5.c
+-rwxr-xr-x   0        0        0     8488 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/multipart.c
+-rwxr-xr-x   0        0        0     2345 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/os/lzma_stub.h
+-rwxr-xr-x   0        0        0     2704 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/os/rand.c
+-rwxr-xr-x   0        0        0     6501 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/plugin.c
+-rwxr-xr-x   0        0        0    16107 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/probaln.c
+-rwxr-xr-x   0        0        0    11748 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/realn.c
+-rwxr-xr-x   0        0        0    19883 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/regidx.c
+-rwxr-xr-x   0        0        0     7744 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/region.c
+-rwxr-xr-x   0        0        0     2789 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/sam.5
+-rwxr-xr-x   0        0        0   168295 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/sam.c
+-rwxr-xr-x   0        0        0     3368 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/sam_internal.h
+-rwxr-xr-x   0        0        0    43102 2022-07-20 15:27:01.000000 ngsfragments-2.0.4/htslib/synced_bcf_reader.c
+-rwxr-xr-x   0        0        0     6954 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/tabix.1
+-rwxr-xr-x   0        0        0    26296 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/tabix.c
+-rwxr-xr-x   0        0        0    15686 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/tbx.c
+-rwxr-xr-x   0        0        0      751 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/auxf#values.sam
+-rwxr-xr-x   0        0        0     5152 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/auxf#values_java.cram
+-rwxr-xr-x   0        0        0       29 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/test/auxf.fa
+-rwxr-xr-x   0        0        0       18 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/auxf.fa.fai
+-rwxr-xr-x   0        0        0      518 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/test/bcf-sr/merge.noidx.a.vcf
+-rwxr-xr-x   0        0        0      128 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/test/bcf-sr/merge.noidx.abc.expected.out
+-rwxr-xr-x   0        0        0      634 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/test/bcf-sr/merge.noidx.b.vcf
+-rwxr-xr-x   0        0        0      634 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/test/bcf-sr/merge.noidx.c.vcf
+-rwxr-xr-x   0        0        0      518 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/test/bcf-sr/merge.noidx.hdr_order.vcf
+-rwxr-xr-x   0        0        0      518 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/test/bcf-sr/merge.noidx.rec_order.vcf
+-rwxr-xr-x   0        0        0       15 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/bgziptest.txt
+-rwxr-xr-x   0        0        0      181 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/bgziptest.txt.gz
+-rwxr-xr-x   0        0        0       88 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/bgziptest.txt.gz.gzi
+-rwxr-xr-x   0        0        0      148 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/c1#bounds.sam
+-rwxr-xr-x   0        0        0      337 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/c1#clip.sam
+-rwxr-xr-x   0        0        0      433 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/c1#noseq.sam
+-rwxr-xr-x   0        0        0      388 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/c1#pad1.sam
+-rwxr-xr-x   0        0        0      527 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/c1#pad2.sam
+-rwxr-xr-x   0        0        0      665 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/c1#pad3.sam
+-rwxr-xr-x   0        0        0      429 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/c1#unknown.sam
+-rwxr-xr-x   0        0        0       15 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/test/c1.fa
+-rwxr-xr-x   0        0        0       14 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/c1.fa.fai
+-rwxr-xr-x   0        0        0      847 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/test/c2#pad.sam
+-rwxr-xr-x   0        0        0       14 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/c2.fa
+-rwxr-xr-x   0        0        0       12 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/c2.fa.fai
+-rwxr-xr-x   0        0        0      341 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/ce#1.sam
+-rwxr-xr-x   0        0        0   322632 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/ce#1000.sam
+-rwxr-xr-x   0        0        0      645 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/ce#2.sam
+-rwxr-xr-x   0        0        0     1872 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/ce#5.sam
+-rwxr-xr-x   0        0        0     1836 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/test/ce#5b.sam
+-rwxr-xr-x   0        0        0     6784 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/test/ce#5b_java.cram
+-rwxr-xr-x   0        0        0  2147244 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/ce#large_seq.sam
+-rwxr-xr-x   0        0        0      547 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/ce#supp.sam
+-rwxr-xr-x   0        0        0     1638 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/ce#tag_depadded.sam
+-rwxr-xr-x   0        0        0     1650 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/ce#tag_padded.sam
+-rwxr-xr-x   0        0        0     1325 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/test/ce#unmap.sam
+-rwxr-xr-x   0        0        0     2747 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/ce#unmap1.sam
+-rwxr-xr-x   0        0        0     5525 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/ce#unmap2.sam
+-rwxr-xr-x   0        0        0  1060702 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/ce.fa
+-rwxr-xr-x   0        0        0      230 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/ce.fa.fai
+-rwxr-xr-x   0        0        0      268 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/colons.bam
+-rwxr-xr-x   0        0        0      424 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/colons.bam.bai
+-rwxr-xr-x   0        0        0     6474 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/compare_sam.pl
+-rwxr-xr-x   0        0        0     4307 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/cross_validate.sh
+-rwxr-xr-x   0        0        0        0 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/emptyfile
+-rwxr-xr-x   0        0        0      289 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/test/faidx.fa
+-rwxr-xr-x   0        0        0    48599 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/fastqs.fq
+-rwxr-xr-x   0        0        0     4951 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/fastqs_README.txt
+-rwxr-xr-x   0        0        0     2438 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/fieldarith.c
+-rwxr-xr-x   0        0        0      910 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/fieldarith.sam
+-rwxr-xr-x   0        0        0      241 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/formatcols.vcf
+-rwxr-xr-x   0        0        0      226 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/formatmissing-out.vcf
+-rwxr-xr-x   0        0        0      226 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/test/formatmissing.vcf
+-rwxr-xr-x   0        0        0     3964 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/fuzz/hts_open_fuzzer.c
+-rwxr-xr-x   0        0        0     3562 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/test/header_syms.pl
+-rwxr-xr-x   0        0        0    12012 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/hfile.c
+-rwxr-xr-x   0        0        0    17620 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/hts_endian.c
+-rwxr-xr-x   0        0        0      776 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/index.bam.bai
+-rwxr-xr-x   0        0        0      130 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/index.bam.csi
+-rwxr-xr-x   0        0        0      144 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/index.bcf.csi
+-rwxr-xr-x   0        0        0       83 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/index.cram.crai
+-rwxr-xr-x   0        0        0    54185 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/index.sam
+-rwxr-xr-x   0        0        0      776 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/index.sam.gz.bai
+-rwxr-xr-x   0        0        0      130 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/index.sam.gz.csi
+-rwxr-xr-x   0        0        0    68888 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/test/index.vcf
+-rwxr-xr-x   0        0        0      159 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/index.vcf.gz.csi
+-rwxr-xr-x   0        0        0      213 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/index.vcf.gz.tbi
+-rwxr-xr-x   0        0        0    54375 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/index_dos.sam
+-rwxr-xr-x   0        0        0      594 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/longrefs/index.expected1.vcf
+-rwxr-xr-x   0        0        0       83 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/longrefs/index.expected2.vcf
+-rwxr-xr-x   0        0        0    21491 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/longrefs/index.vcf
+-rwxr-xr-x   0        0        0    31717 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/longrefs/longref.sam
+-rwxr-xr-x   0        0        0     8300 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/longrefs/longref_itr.expected.sam
+-rwxr-xr-x   0        0        0    15015 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/longrefs/longref_multi.expected.sam
+-rwxr-xr-x   0        0        0     3255 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/maintainer/check_copyright.pl
+-rwxr-xr-x   0        0        0     2734 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/maintainer/check_spaces.pl
+-rwxr-xr-x   0        0        0     1017 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/md#1.sam
+-rwxr-xr-x   0        0        0       45 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/md.fa
+-rwxr-xr-x   0        0        0       13 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/md.fa.fai
+-rwxr-xr-x   0        0        0      274 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/mpileup/c1#pad1.out
+-rwxr-xr-x   0        0        0     2024 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/mpileup/c1#pad1.sam
+-rwxr-xr-x   0        0        0      355 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/mpileup/c1#pad2.out
+-rwxr-xr-x   0        0        0     2311 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/mpileup/c1#pad2.sam
+-rwxr-xr-x   0        0        0      134 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/mpileup/c1#pad3.out
+-rwxr-xr-x   0        0        0     2393 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/mpileup/c1#pad3.sam
+-rwxr-xr-x   0        0        0      130 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/mpileup/mp_D.out
+-rwxr-xr-x   0        0        0     1534 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/mpileup/mp_D.sam
+-rwxr-xr-x   0        0        0      197 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/mpileup/mp_DI.out
+-rwxr-xr-x   0        0        0     1747 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/mpileup/mp_DI.sam
+-rwxr-xr-x   0        0        0      135 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/mpileup/mp_I.out
+-rwxr-xr-x   0        0        0     1821 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/mpileup/mp_I.sam
+-rwxr-xr-x   0        0        0      181 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/mpileup/mp_ID.out
+-rwxr-xr-x   0        0        0     1958 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/mpileup/mp_ID.sam
+-rwxr-xr-x   0        0        0      122 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/mpileup/mp_N.out
+-rwxr-xr-x   0        0        0     1739 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/mpileup/mp_N.sam
+-rwxr-xr-x   0        0        0      275 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/mpileup/mp_N2.out
+-rwxr-xr-x   0        0        0     2152 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/mpileup/mp_N2.sam
+-rwxr-xr-x   0        0        0      169 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/mpileup/mp_P.out
+-rwxr-xr-x   0        0        0     1796 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/mpileup/mp_P.sam
+-rwxr-xr-x   0        0        0     2582 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/mpileup/mpileup.tst
+-rwxr-xr-x   0        0        0     1294 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/mpileup/small.bam
+-rwxr-xr-x   0        0        0     3330 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/mpileup/small.out
+-rwxr-xr-x   0        0        0     1295 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/mpileup/test-pileup.sh
+-rwxr-xr-x   0        0        0     1691 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/no_hdr_sq_1.bam
+-rwxr-xr-x   0        0        0       94 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/no_hdr_sq_1.bam.csi
+-rwxr-xr-x   0        0        0     2019 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/no_hdr_sq_1.expected.sam
+-rwxr-xr-x   0        0        0      325 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/noroundtrip-out.vcf
+-rwxr-xr-x   0        0        0      271 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/noroundtrip.vcf
+-rwxr-xr-x   0        0        0     7002 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/pileup.c
+-rwxr-xr-x   0        0        0     5072 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/plugins-dlhts.c
+-rwxr-xr-x   0        0        0    13337 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/range.bam
+-rwxr-xr-x   0        0        0      360 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/range.bam.bai
+-rwxr-xr-x   0        0        0    11182 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/range.cram
+-rwxr-xr-x   0        0        0       94 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/range.cram.crai
+-rwxr-xr-x   0        0        0     3496 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/range.out
+-rwxr-xr-x   0        0        0      719 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/realn01.fa
+-rwxr-xr-x   0        0        0       21 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/realn01.fa.fai
+-rwxr-xr-x   0        0        0     1843 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/realn01.sam
+-rwxr-xr-x   0        0        0     2157 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/realn01_exp-a.sam
+-rwxr-xr-x   0        0        0     2157 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/realn01_exp-e.sam
+-rwxr-xr-x   0        0        0     2157 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/realn01_exp.sam
+-rwxr-xr-x   0        0        0     3758 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/realn02-r.sam
+-rwxr-xr-x   0        0        0     4284 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/realn02.fa
+-rwxr-xr-x   0        0        0       17 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/realn02.fa.fai
+-rwxr-xr-x   0        0        0     2894 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/test/realn02.sam
+-rwxr-xr-x   0        0        0     3758 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/realn02_exp-a.sam
+-rwxr-xr-x   0        0        0     3758 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/realn02_exp-e.sam
+-rwxr-xr-x   0        0        0     3758 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/test/realn02_exp.sam
+-rwxr-xr-x   0        0        0    78940 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/sam.c
+-rwxr-xr-x   0        0        0     1291 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/sam_filter/filter.sh
+-rwxr-xr-x   0        0        0     2610 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/sam_filter/filter.tst
+-rwxr-xr-x   0        0        0        2 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/sam_filter/func1.out
+-rwxr-xr-x   0        0        0        3 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/sam_filter/func2.out
+-rwxr-xr-x   0        0        0        2 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/sam_filter/func3.out
+-rwxr-xr-x   0        0        0        4 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/sam_filter/func4.out
+-rwxr-xr-x   0        0        0        3 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/sam_filter/int1.out
+-rwxr-xr-x   0        0        0        3 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/sam_filter/int2.out
+-rwxr-xr-x   0        0        0        3 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/sam_filter/int3.out
+-rwxr-xr-x   0        0        0      485 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/sam_filter/string1.out
+-rwxr-xr-x   0        0        0      451 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/sam_filter/string2.out
+-rwxr-xr-x   0        0        0      748 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/sam_filter/string3.out
+-rwxr-xr-x   0        0        0     1136 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/sam_filter/string4.out
+-rwxr-xr-x   0        0        0      498 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/sam_filter/string5.out
+-rwxr-xr-x   0        0        0      319 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/sam_filter/string6.out
+-rwxr-xr-x   0        0        0      410 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/sam_filter/string7.out
+-rwxr-xr-x   0        0        0     5587 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/simple_test_driver.sh
+-rwxr-xr-x   0        0        0       47 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/tabix/bed_file.Y.100200.out
+-rwxr-xr-x   0        0        0     1857 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/tabix/bed_file.bed
+-rwxr-xr-x   0        0        0      407 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/tabix/bed_file.separate.out
+-rwxr-xr-x   0        0        0      405 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/tabix/gff_file.X.2934832.2935190.out
+-rwxr-xr-x   0        0        0     5618 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/tabix/gff_file.gff
+-rwxr-xr-x   0        0        0      288 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/tabix/large_chr.20.1.2147483647.out
+-rwxr-xr-x   0        0        0      622 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/tabix/large_chr.vcf
+-rwxr-xr-x   0        0        0     3023 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/tabix/tabix.tst
+-rwxr-xr-x   0        0        0     1312 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/tabix/test-tabix.sh
+-rwxr-xr-x   0        0        0       67 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/tabix/vcf_file.1.3000151.out
+-rwxr-xr-x   0        0        0       74 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/tabix/vcf_file.2.3199812.out
+-rwxr-xr-x   0        0        0     2719 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/tabix/vcf_file.bcf
+-rwxr-xr-x   0        0        0     2543 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/tabix/vcf_file.vcf
+-rwxr-xr-x   0        0        0       98 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/tabix.out
+-rwxr-xr-x   0        0        0     5167 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/test-bcf-sr.c
+-rwxr-xr-x   0        0        0    19566 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/test-bcf-sr.pl
+-rwxr-xr-x   0        0        0     8964 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/test-bcf-translate.c
+-rwxr-xr-x   0        0        0      869 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/test-bcf-translate.out
+-rwxr-xr-x   0        0        0     2602 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/test-logging.pl
+-rwxr-xr-x   0        0        0     7064 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/test-parse-reg.c
+-rwxr-xr-x   0        0        0    16871 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/test-regidx.c
+-rwxr-xr-x   0        0        0    23890 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/test/test-vcf-api.c
+-rwxr-xr-x   0        0        0     2064 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/test-vcf-api.out
+-rwxr-xr-x   0        0        0     2024 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/test-vcf-hdr-in.vcf
+-rwxr-xr-x   0        0        0     1349 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/test-vcf-hdr.out
+-rwxr-xr-x   0        0        0     3840 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/test-vcf-sweep.c
+-rwxr-xr-x   0        0        0       92 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/test-vcf-sweep.out
+-rwxr-xr-x   0        0        0    39913 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/test.pl
+-rwxr-xr-x   0        0        0    31594 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/test_bgzf.c
+-rwxr-xr-x   0        0        0     6966 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/test/test_expr.c
+-rwxr-xr-x   0        0        0     2869 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/test_index.c
+-rwxr-xr-x   0        0        0     3308 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/test/test_introspection.c
+-rwxr-xr-x   0        0        0     3639 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/test_kfunc.c
+-rwxr-xr-x   0        0        0    12102 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/test_kstring.c
+-rwxr-xr-x   0        0        0     5057 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/test_realn.c
+-rwxr-xr-x   0        0        0     8892 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/test_str2int.c
+-rwxr-xr-x   0        0        0    14460 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/test_view.c
+-rwxr-xr-x   0        0        0     1688 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/thrash_threads1.c
+-rwxr-xr-x   0        0        0     1621 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/test/thrash_threads2.c
+-rwxr-xr-x   0        0        0     1729 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/test/thrash_threads3.c
+-rwxr-xr-x   0        0        0     2273 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/thrash_threads4.c
+-rwxr-xr-x   0        0        0     2176 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/thrash_threads5.c
+-rwxr-xr-x   0        0        0     3412 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/thrash_threads6.c
+-rwxr-xr-x   0        0        0     3661 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/thrash_threads7.c
+-rwxr-xr-x   0        0        0     2938 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/thread_pool.md
+-rwxr-xr-x   0        0        0     2108 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/with-shlib.sh
+-rwxr-xr-x   0        0        0     1070 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/test/xx#MD.sam
+-rwxr-xr-x   0        0        0     1159 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/xx#MD2.sam
+-rwxr-xr-x   0        0        0       71 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/xx#blank.sam
+-rwxr-xr-x   0        0        0   905485 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/xx#large_aux.sam
+-rwxr-xr-x   0        0        0      651 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/xx#large_aux2.sam
+-rwxr-xr-x   0        0        0    22668 2022-07-20 15:27:06.000000 ngsfragments-2.0.4/htslib/test/xx#large_aux_java.cram
+-rwxr-xr-x   0        0        0      254 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/xx#minimal.sam
+-rwxr-xr-x   0        0        0      304 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/xx#pair.sam
+-rwxr-xr-x   0        0        0      298 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/xx#repeated.sam
+-rwxr-xr-x   0        0        0      517 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/xx#rg.sam
+-rwxr-xr-x   0        0        0     1028 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/xx#tlen.sam
+-rwxr-xr-x   0        0        0     1096 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/xx#tlen2.sam
+-rwxr-xr-x   0        0        0      267 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/xx#triplet.sam
+-rwxr-xr-x   0        0        0      320 2022-07-20 15:27:04.000000 ngsfragments-2.0.4/htslib/test/xx#unsorted.sam
+-rwxr-xr-x   0        0        0       86 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/xx.fa
+-rwxr-xr-x   0        0        0       44 2022-07-20 15:27:05.000000 ngsfragments-2.0.4/htslib/test/xx.fa.fai
+-rwxr-xr-x   0        0        0    11957 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/textutils.c
+-rwxr-xr-x   0        0        0    14771 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/textutils_internal.h
+-rwxr-xr-x   0        0        0    45617 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/thread_pool.c
+-rwxr-xr-x   0        0        0     5853 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/thread_pool_internal.h
+-rwxr-xr-x   0        0        0     3543 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/vcf.5
+-rwxr-xr-x   0        0        0   163400 2022-07-20 15:27:09.000000 ngsfragments-2.0.4/htslib/vcf.c
+-rwxr-xr-x   0        0        0     5570 2022-07-20 15:27:01.000000 ngsfragments-2.0.4/htslib/vcf_sweep.c
+-rwxr-xr-x   0        0        0    33937 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/vcfutils.c
+-rwxr-xr-x   0        0        0       33 2022-07-20 15:27:02.000000 ngsfragments-2.0.4/htslib/version.h
+-rwxr-xr-x   0        0        0     2050 2022-07-20 15:27:03.000000 ngsfragments-2.0.4/htslib/version.sh
+-rw-r--r--   0        0        0    10244 2023-05-17 14:05:23.719714 ngsfragments-2.0.4/ngsfragments/.DS_Store
+-rwxr-xr-x   0        0        0      373 2023-05-17 16:12:39.406569 ngsfragments-2.0.4/ngsfragments/__init__.py
+-rwxr-xr-x   0        0        0      187 2023-05-17 16:19:32.629996 ngsfragments-2.0.4/ngsfragments/config.py
+-rwxr-xr-x   0        0        0      167 2023-03-21 14:48:14.313666 ngsfragments-2.0.4/ngsfragments/correct/__init__.py
+-rw-r--r--   0        0        0     2307 2023-05-11 20:03:38.317861 ngsfragments-2.0.4/ngsfragments/correct/correct_intervals.py
+-rwxr-xr-x   0        0        0     5810 2023-05-11 20:02:33.042562 ngsfragments-2.0.4/ngsfragments/correct/correction.py
+-rwxr-xr-x   0        0        0       92 2022-10-10 20:36:54.000000 ngsfragments-2.0.4/ngsfragments/correct/cylowess/__init__.py
+-rw-r--r--   0        0        0   482168 2023-03-21 14:00:47.861831 ngsfragments-2.0.4/ngsfragments/correct/cylowess/cylowess.c
+-rw-r--r--   0        0        0   122648 2023-05-17 16:19:54.420733 ngsfragments-2.0.4/ngsfragments/correct/cylowess/cylowess.cpython-310-darwin.so
+-rw-r--r--   0        0        0    21292 2023-03-21 14:00:31.232217 ngsfragments-2.0.4/ngsfragments/correct/cylowess/cylowess.pyx
+-rwxr-xr-x   0        0        0       92 2023-02-07 15:14:21.258083 ngsfragments-2.0.4/ngsfragments/coverage/__init__.py
+-rw-r--r--   0        0        0     7595 2023-05-15 20:07:54.689766 ngsfragments-2.0.4/ngsfragments/coverage/coverage.py
+-rw-r--r--   0        0        0      903 2023-05-15 20:08:26.702773 ngsfragments-2.0.4/ngsfragments/coverage/midpoint.py
+-rw-r--r--   0        0        0     5152 2023-05-15 20:09:35.205474 ngsfragments-2.0.4/ngsfragments/coverage/wps.py
+-rwxr-xr-x   0        0        0     5060 2023-05-15 19:58:24.489625 ngsfragments-2.0.4/ngsfragments/fragments.py
+-rwxr-xr-x   0        0        0       82 2023-02-01 19:26:53.531065 ngsfragments-2.0.4/ngsfragments/io/__init__.py
+-rw-r--r--   0        0        0  1003390 2023-02-01 19:58:16.917570 ngsfragments-2.0.4/ngsfragments/io/parse_sam/ReadSam.c
+-rw-r--r--   0        0        0  1146848 2023-05-17 16:19:54.419371 ngsfragments-2.0.4/ngsfragments/io/parse_sam/ReadSam.cpython-310-darwin.so
+-rwxr-xr-x   0        0        0     2651 2022-12-14 19:52:53.000000 ngsfragments-2.0.4/ngsfragments/io/parse_sam/ReadSam.pxd
+-rwxr-xr-x   0        0        0     5730 2022-12-14 20:20:03.000000 ngsfragments-2.0.4/ngsfragments/io/parse_sam/ReadSam.pyx
+-rwxr-xr-x   0        0        0       99 2022-07-20 15:26:56.000000 ngsfragments-2.0.4/ngsfragments/io/parse_sam/__init__.py
+-rwxr-xr-x   0        0        0     7494 2022-12-14 20:33:54.000000 ngsfragments-2.0.4/ngsfragments/io/parse_sam/read_intervals.c
+-rwxr-xr-x   0        0        0     1406 2022-12-14 19:52:12.000000 ngsfragments-2.0.4/ngsfragments/io/parse_sam/read_intervals.h
+-rwxr-xr-x   0        0        0     7885 2022-07-20 15:26:56.000000 ngsfragments-2.0.4/ngsfragments/io/parse_sam/read_intervals_v0.c
+-rw-r--r--   0        0        0     2823 2023-05-15 20:13:08.300015 ngsfragments-2.0.4/ngsfragments/io/read_sam.py
+-rwxr-xr-x   0        0        0       80 2023-02-10 22:01:53.060407 ngsfragments-2.0.4/ngsfragments/metrics/__init__.py
+-rw-r--r--   0        0        0     3820 2023-05-15 20:12:08.740246 ngsfragments-2.0.4/ngsfragments/metrics/gc_metrics.py
+-rw-r--r--   0        0        0    10545 2023-05-11 20:08:15.832145 ngsfragments-2.0.4/ngsfragments/metrics/gene_activity.py
+-rw-r--r--   0        0        0      267 2023-03-05 16:12:26.726790 ngsfragments-2.0.4/ngsfragments/metrics/wps_metrics.py
+-rw-r--r--   0        0        0     6148 2023-02-10 21:54:33.607661 ngsfragments-2.0.4/ngsfragments/peak_calling/.DS_Store
+-rw-r--r--   0        0        0   916514 2023-02-10 22:01:41.328107 ngsfragments-2.0.4/ngsfragments/peak_calling/CallPeaks.c
+-rw-r--r--   0        0        0   220576 2023-05-17 16:19:54.420304 ngsfragments-2.0.4/ngsfragments/peak_calling/CallPeaks.cpython-310-darwin.so
+-rwxr-xr-x   0        0        0      475 2023-02-10 21:54:21.291585 ngsfragments-2.0.4/ngsfragments/peak_calling/CallPeaks.pxd
+-rwxr-xr-x   0        0        0     2786 2023-02-10 21:54:06.026216 ngsfragments-2.0.4/ngsfragments/peak_calling/CallPeaks.pyx
+-rw-r--r--   0        0        0   852272 2022-09-15 14:37:09.000000 ngsfragments-2.0.4/ngsfragments/peak_calling/RunningMean.c
+-rw-r--r--   0        0        0   142536 2023-05-17 16:19:54.420046 ngsfragments-2.0.4/ngsfragments/peak_calling/RunningMean.cpython-310-darwin.so
+-rwxr-xr-x   0        0        0      519 2022-07-20 15:26:57.000000 ngsfragments-2.0.4/ngsfragments/peak_calling/RunningMean.pxd
+-rwxr-xr-x   0        0        0      681 2022-07-20 15:26:57.000000 ngsfragments-2.0.4/ngsfragments/peak_calling/RunningMean.pyx
+-rw-r--r--   0        0        0   864899 2022-09-15 14:37:06.000000 ngsfragments-2.0.4/ngsfragments/peak_calling/RunningMedian.c
+-rw-r--r--   0        0        0   143792 2023-05-17 16:19:54.419815 ngsfragments-2.0.4/ngsfragments/peak_calling/RunningMedian.cpython-310-darwin.so
+-rwxr-xr-x   0        0        0      557 2022-07-20 15:26:57.000000 ngsfragments-2.0.4/ngsfragments/peak_calling/RunningMedian.pxd
+-rwxr-xr-x   0        0        0     1973 2022-07-20 15:26:57.000000 ngsfragments-2.0.4/ngsfragments/peak_calling/RunningMedian.pyx
+-rwxr-xr-x   0        0        0      196 2023-02-01 18:05:20.025593 ngsfragments-2.0.4/ngsfragments/peak_calling/__init__.py
+-rwxr-xr-x   0        0        0     1056 2022-07-20 15:26:57.000000 ngsfragments-2.0.4/ngsfragments/peak_calling/running_mean.c
+-rwxr-xr-x   0        0        0      283 2022-07-20 15:26:57.000000 ngsfragments-2.0.4/ngsfragments/peak_calling/running_mean.h
+-rwxr-xr-x   0        0        0     8413 2022-07-20 15:26:57.000000 ngsfragments-2.0.4/ngsfragments/peak_calling/sklist_pd.c
+-rwxr-xr-x   0        0        0     1158 2022-07-20 15:26:57.000000 ngsfragments-2.0.4/ngsfragments/peak_calling/sklist_pd.h
+-rwxr-xr-x   0        0        0       75 2022-07-20 15:26:57.000000 ngsfragments-2.0.4/ngsfragments/plot/__init__.py
+-rwxr-xr-x   0        0        0     4657 2022-07-20 15:26:57.000000 ngsfragments-2.0.4/ngsfragments/plot/plot_bokeh.py
+-rwxr-xr-x   0        0        0    13815 2023-05-17 13:34:28.507840 ngsfragments-2.0.4/ngsfragments/plot/plot_plt.py
+-rw-r--r--   0        0        0     6148 2023-05-11 20:09:53.010855 ngsfragments-2.0.4/ngsfragments/segment/.DS_Store
+-rwxr-xr-x   0        0        0      139 2023-05-13 14:22:26.939358 ngsfragments-2.0.4/ngsfragments/segment/__init__.py
+-rwxr-xr-x   0        0        0     3649 2023-05-13 14:23:49.399762 ngsfragments-2.0.4/ngsfragments/segment/cnv.py
+-rwxr-xr-x   0        0        0    22506 2023-05-12 20:21:02.644767 ngsfragments-2.0.4/ngsfragments/segment/cnv_pipeline.py
+-rwxr-xr-x   0        0        0    16333 2023-05-12 20:43:03.845216 ngsfragments-2.0.4/ngsfragments/segment/cnv_utilities.py
+-rwxr-xr-x   0        0        0       97 2022-07-20 15:26:56.000000 ngsfragments-2.0.4/ngsfragments/segment/smooth_cnv/__init__.py
+-rwxr-xr-x   0        0        0     2924 2022-07-20 15:26:56.000000 ngsfragments-2.0.4/ngsfragments/segment/smooth_cnv/smoothCNV.c
+-rwxr-xr-x   0        0        0      285 2022-07-20 15:26:57.000000 ngsfragments-2.0.4/ngsfragments/segment/smooth_cnv/smoothCNV.h
+-rw-r--r--   0        0        0   926261 2023-02-01 19:58:17.916519 ngsfragments-2.0.4/ngsfragments/segment/smooth_cnv/smooth_cnv.c
+-rw-r--r--   0        0        0   159088 2023-05-17 16:19:54.420519 ngsfragments-2.0.4/ngsfragments/segment/smooth_cnv/smooth_cnv.cpython-310-darwin.so
+-rwxr-xr-x   0        0        0      304 2022-07-20 15:26:56.000000 ngsfragments-2.0.4/ngsfragments/segment/smooth_cnv/smooth_cnv.pxd
+-rwxr-xr-x   0        0        0     1469 2022-07-20 15:26:56.000000 ngsfragments-2.0.4/ngsfragments/segment/smooth_cnv/smooth_cnv.pyx
+-rwxr-xr-x   0        0        0      104 2023-03-21 14:53:46.744822 ngsfragments-2.0.4/ngsfragments/sequence/__init__.py
+-rw-r--r--   0        0        0     1488 2023-02-01 21:52:11.526397 ngsfragments-2.0.4/ngsfragments/sequence/kmer_query.py
+-rw-r--r--   0        0        0      458 2023-01-31 18:53:12.818067 ngsfragments-2.0.4/ngsfragments/sequence/sequence_query.py
+-rwxr-xr-x   0        0        0       61 2023-01-31 21:54:53.387281 ngsfragments-2.0.4/ngsfragments/sequence/snp_calling/__init__.py
+-rw-r--r--   0        0        0   975270 2023-02-01 19:58:19.931481 ngsfragments-2.0.4/ngsfragments/sequence/snp_calling/snp_calling.c
+-rw-r--r--   0        0        0      815 2023-02-01 12:46:55.639263 ngsfragments-2.0.4/ngsfragments/sequence/snp_calling/snp_calling.pxd
+-rw-r--r--   0        0        0     5077 2023-02-01 13:17:00.089609 ngsfragments-2.0.4/ngsfragments/sequence/snp_calling/snp_calling.pyx
+-rwxr-xr-x   0        0        0     6870 2023-05-15 15:11:02.820550 ngsfragments-2.0.4/ngsfragments/utilities.py
+-rw-r--r--   0        0        0     2635 2023-05-17 16:15:02.256000 ngsfragments-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3073 1970-01-01 00:00:00.000000 ngsfragments-2.0.4/PKG-INFO
```

### Comparing `ngsfragments-2.0.3/LICENSE.md` & `ngsfragments-2.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/README.md` & `ngsfragments-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/build.py` & `ngsfragments-2.0.4/build.py`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/cy_build.py` & `ngsfragments-2.0.4/cy_build.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 try:
     from Cython.Distutils import build_ext
 except ImportError:
     from setuptools.command.build_ext import build_ext
 
 from distutils.extension import Extension
-from distutils.sysconfig import get_config_vars, get_python_lib, get_python_version
+from distutils.sysconfig import get_config_var, get_config_vars, get_python_version
 from pkg_resources import Distribution
 
 
 if sys.platform == 'darwin':
     config_vars = get_config_vars()
     config_vars['LDSHARED'] = config_vars['LDSHARED'].replace('-bundle', '')
     config_vars['SHLIB_EXT'] = '.so'
@@ -61,15 +61,16 @@
 
         if sys.platform == 'darwin':
             # The idea is to give shared libraries an install name of the form
             # `@rpath/<library-name.so>`, and to set the rpath equal to
             # @loader_path. This will allow Python packages to find the library
             # in the expected place, while still giving enough flexibility to
             # external applications to link against the library.
-            relative_module_path = ext.name.replace(".", os.sep) + get_config_vars()["SO"]
+            #relative_module_path = ext.name.replace(".", os.sep) + get_config_vars()["SO"]
+            relative_module_path = ext.name.replace(".", os.sep) + (get_config_var('EXT_SUFFIX') or get_config_var('SO'))
             library_path = os.path.join(
                 "@rpath", os.path.basename(relative_module_path)
             )
 
             if not ext.extra_link_args:
                 ext.extra_link_args = []
             ext.extra_link_args += ['-dynamiclib',
```

### Comparing `ngsfragments-2.0.3/htslib/INSTALL` & `ngsfragments-2.0.4/htslib/INSTALL`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/LICENSE` & `ngsfragments-2.0.4/htslib/LICENSE`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/Makefile` & `ngsfragments-2.0.4/htslib/Makefile`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/NEWS` & `ngsfragments-2.0.4/htslib/NEWS`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/README.large_positions.md` & `ngsfragments-2.0.4/htslib/README.large_positions.md`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/bcf_sr_sort.c` & `ngsfragments-2.0.4/htslib/bcf_sr_sort.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/bcf_sr_sort.h` & `ngsfragments-2.0.4/htslib/bcf_sr_sort.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/bgzf.c` & `ngsfragments-2.0.4/htslib/bgzf.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/bgzip.1` & `ngsfragments-2.0.4/htslib/bgzip.1`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/bgzip.c` & `ngsfragments-2.0.4/htslib/bgzip.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/config.h` & `ngsfragments-2.0.4/htslib/config.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/config.h.in` & `ngsfragments-2.0.4/htslib/config.h.in`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/config.log` & `ngsfragments-2.0.4/htslib/config.log`

 * *Files 1% similar despite different names*

```diff
@@ -26,20 +26,21 @@
 	 Darwin Kernel Version 22.1.0: Sun Oct  9 20:15:52 PDT 2022; root:xnu-8792.41.9~2/RELEASE_ARM64_T8112
 Kernel configured for up to 8 processors.
 8 processors are physically available.
 8 processors are logically available.
 Processor type: i486 (Intel 80486)
 Processors active: 0 1 2 3 4 5 6 7
 Primary memory available: 16.00 gigabytes
-Default processor set: 446 tasks, 3359 threads, 8 processors
-Load average: 4.37, Mach factor: 3.64
+Default processor set: 387 tasks, 3189 threads, 8 processors
+Load average: 4.79, Mach factor: 3.92
 /bin/machine           = unknown
 /usr/bin/oslevel       = unknown
 /bin/universe          = unknown
 
+PATH: /var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmpp9gbs1ko/.venv/bin
 PATH: /Users/ksmith10/.local/bin
 PATH: /opt/anaconda3/envs/ailist/bin
 PATH: /opt/anaconda3/condabin
 PATH: /Library/Frameworks/Python.framework/Versions/3.11/bin
 PATH: /usr/local/bin
 PATH: /System/Cryptexes/App/usr/bin
 PATH: /usr/bin
@@ -247,15 +248,15 @@
 configure:4444: clang -o conftest  -Wno-unused-result -Wsign-compare -Wunreachable-code -DNDEBUG -fwrapv -O2 -Wall  -fPIC  -O2  -isystem /opt/anaconda3/envs/ailist/include -fPIC   -O2 -isystem /opt/anaconda3/envs/ailist/include  -fvisibility=hidden  -Wl,-rpath,/opt/anaconda3/envs/ailist/lib -L/opt/anaconda3/envs/ailist/lib -Wl,-rpath,/opt/anaconda3/envs/ailist/lib -L/opt/anaconda3/envs/ailist/lib -fvisibility=hidden conftest.c  >&5
 configure:4444: $? = 0
 configure:4444: result: yes
 configure:4444: checking for srand48_deterministic
 configure:4444: clang -o conftest  -Wno-unused-result -Wsign-compare -Wunreachable-code -DNDEBUG -fwrapv -O2 -Wall  -fPIC  -O2  -isystem /opt/anaconda3/envs/ailist/include -fPIC   -O2 -isystem /opt/anaconda3/envs/ailist/include  -fvisibility=hidden  -Wl,-rpath,/opt/anaconda3/envs/ailist/lib -L/opt/anaconda3/envs/ailist/lib -Wl,-rpath,/opt/anaconda3/envs/ailist/lib -L/opt/anaconda3/envs/ailist/lib -fvisibility=hidden conftest.c  >&5
 Undefined symbols for architecture x86_64:
   "_srand48_deterministic", referenced from:
-      _main in conftest-bf3d9d.o
+      _main in conftest-0d864c.o
 ld: symbol(s) not found for architecture x86_64
 clang: error: linker command failed with exit code 1 (use -v to see invocation)
 configure:4444: $? = 1
 configure: failed program was:
 | /* confdefs.h */
 | #define PACKAGE_NAME "HTSlib"
 | #define PACKAGE_TARNAME "htslib"
```

### Comparing `ngsfragments-2.0.3/htslib/config.mk` & `ngsfragments-2.0.4/htslib/config.mk`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/config.mk.in` & `ngsfragments-2.0.4/htslib/config.mk.in`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/config.status` & `ngsfragments-2.0.4/htslib/config.status`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/config_vars.h` & `ngsfragments-2.0.4/htslib/config_vars.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/configure` & `ngsfragments-2.0.4/htslib/configure`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/configure.ac` & `ngsfragments-2.0.4/htslib/configure.ac`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/cram/cram.h` & `ngsfragments-2.0.4/htslib/cram/cram.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/cram/cram_codecs.c` & `ngsfragments-2.0.4/htslib/cram/cram_codecs.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/cram/cram_codecs.h` & `ngsfragments-2.0.4/htslib/cram/cram_codecs.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/cram/cram_decode.c` & `ngsfragments-2.0.4/htslib/cram/cram_decode.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/cram/cram_decode.h` & `ngsfragments-2.0.4/htslib/cram/cram_decode.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/cram/cram_encode.c` & `ngsfragments-2.0.4/htslib/cram/cram_encode.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/cram/cram_encode.h` & `ngsfragments-2.0.4/htslib/cram/cram_encode.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/cram/cram_external.c` & `ngsfragments-2.0.4/htslib/cram/cram_external.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/cram/cram_index.c` & `ngsfragments-2.0.4/htslib/cram/cram_index.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/cram/cram_index.h` & `ngsfragments-2.0.4/htslib/cram/cram_index.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/cram/cram_io.c` & `ngsfragments-2.0.4/htslib/cram/cram_io.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/cram/cram_io.h` & `ngsfragments-2.0.4/htslib/cram/cram_io.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/cram/cram_samtools.h` & `ngsfragments-2.0.4/htslib/cram/cram_samtools.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/cram/cram_stats.c` & `ngsfragments-2.0.4/htslib/cram/cram_stats.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/cram/cram_stats.h` & `ngsfragments-2.0.4/htslib/cram/cram_stats.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/cram/cram_structs.h` & `ngsfragments-2.0.4/htslib/cram/cram_structs.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/cram/mFILE.c` & `ngsfragments-2.0.4/htslib/cram/mFILE.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/cram/mFILE.h` & `ngsfragments-2.0.4/htslib/cram/mFILE.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/cram/misc.h` & `ngsfragments-2.0.4/htslib/cram/misc.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/cram/open_trace_file.c` & `ngsfragments-2.0.4/htslib/cram/open_trace_file.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/cram/open_trace_file.h` & `ngsfragments-2.0.4/htslib/cram/open_trace_file.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/cram/os.h` & `ngsfragments-2.0.4/htslib/cram/os.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/cram/pooled_alloc.c` & `ngsfragments-2.0.4/htslib/cram/pooled_alloc.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/cram/pooled_alloc.h` & `ngsfragments-2.0.4/htslib/cram/pooled_alloc.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/cram/string_alloc.c` & `ngsfragments-2.0.4/htslib/cram/string_alloc.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/cram/string_alloc.h` & `ngsfragments-2.0.4/htslib/cram/string_alloc.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/errmod.c` & `ngsfragments-2.0.4/htslib/errmod.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/faidx.5` & `ngsfragments-2.0.4/htslib/faidx.5`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/faidx.c` & `ngsfragments-2.0.4/htslib/faidx.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/header.c` & `ngsfragments-2.0.4/htslib/header.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/header.h` & `ngsfragments-2.0.4/htslib/header.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/hfile.c` & `ngsfragments-2.0.4/htslib/hfile.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/hfile_gcs.c` & `ngsfragments-2.0.4/htslib/hfile_gcs.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/hfile_internal.h` & `ngsfragments-2.0.4/htslib/hfile_internal.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/hfile_libcurl.c` & `ngsfragments-2.0.4/htslib/hfile_libcurl.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/hfile_s3.c` & `ngsfragments-2.0.4/htslib/hfile_s3.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/hfile_s3_write.c` & `ngsfragments-2.0.4/htslib/hfile_s3_write.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/hts.c` & `ngsfragments-2.0.4/htslib/hts.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/hts_expr.c` & `ngsfragments-2.0.4/htslib/hts_expr.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/hts_internal.h` & `ngsfragments-2.0.4/htslib/hts_internal.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/hts_os.c` & `ngsfragments-2.0.4/htslib/hts_os.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/LICENSE.md` & `ngsfragments-2.0.4/htslib/htscodecs/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/NEWS` & `ngsfragments-2.0.4/htslib/htscodecs/NEWS`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/htscodecs/arith_dynamic.c` & `ngsfragments-2.0.4/htslib/htscodecs/htscodecs/arith_dynamic.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/htscodecs/arith_dynamic.h` & `ngsfragments-2.0.4/htslib/htscodecs/htscodecs/arith_dynamic.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/htscodecs/c_range_coder.h` & `ngsfragments-2.0.4/htslib/htscodecs/htscodecs/c_range_coder.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/htscodecs/c_simple_model.h` & `ngsfragments-2.0.4/htslib/htscodecs/htscodecs/c_simple_model.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/htscodecs/fqzcomp_qual.c` & `ngsfragments-2.0.4/htslib/htscodecs/htscodecs/fqzcomp_qual.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/htscodecs/fqzcomp_qual.h` & `ngsfragments-2.0.4/htslib/htscodecs/htscodecs/fqzcomp_qual.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/htscodecs/htscodecs.c` & `ngsfragments-2.0.4/htslib/htscodecs/htscodecs/htscodecs.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/htscodecs/htscodecs.h` & `ngsfragments-2.0.4/htslib/htscodecs/htscodecs/htscodecs.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/htscodecs/htscodecs_endian.h` & `ngsfragments-2.0.4/htslib/htscodecs/htscodecs/htscodecs_endian.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/htscodecs/pack.c` & `ngsfragments-2.0.4/htslib/htscodecs/htscodecs/pack.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/htscodecs/pack.h` & `ngsfragments-2.0.4/htslib/htscodecs/htscodecs/pack.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/htscodecs/pooled_alloc.h` & `ngsfragments-2.0.4/htslib/htscodecs/htscodecs/pooled_alloc.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/htscodecs/rANS_byte.h` & `ngsfragments-2.0.4/htslib/htscodecs/htscodecs/rANS_byte.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/htscodecs/rANS_static.c` & `ngsfragments-2.0.4/htslib/htscodecs/htscodecs/rANS_static.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/htscodecs/rANS_static.h` & `ngsfragments-2.0.4/htslib/htscodecs/htscodecs/rANS_static.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/htscodecs/rANS_static4x16.h` & `ngsfragments-2.0.4/htslib/htscodecs/htscodecs/rANS_static4x16.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/htscodecs/rANS_static4x16pr.c` & `ngsfragments-2.0.4/htslib/htscodecs/htscodecs/rANS_static4x16pr.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/htscodecs/rANS_word.h` & `ngsfragments-2.0.4/htslib/htscodecs/htscodecs/rANS_word.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/htscodecs/rle.c` & `ngsfragments-2.0.4/htslib/htscodecs/htscodecs/rle.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/htscodecs/rle.h` & `ngsfragments-2.0.4/htslib/htscodecs/htscodecs/rle.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/htscodecs/tokenise_name3.c` & `ngsfragments-2.0.4/htslib/htscodecs/htscodecs/tokenise_name3.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/htscodecs/tokenise_name3.h` & `ngsfragments-2.0.4/htslib/htscodecs/htscodecs/tokenise_name3.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/htscodecs/utils.h` & `ngsfragments-2.0.4/htslib/htscodecs/htscodecs/utils.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/htscodecs/varint.h` & `ngsfragments-2.0.4/htslib/htscodecs/htscodecs/varint.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/htscodecs/varint2.h` & `ngsfragments-2.0.4/htslib/htscodecs/htscodecs/varint2.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/arith.test` & `ngsfragments-2.0.4/htslib/htscodecs/tests/arith.test`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/arith_dynamic_fuzz.c` & `ngsfragments-2.0.4/htslib/htscodecs/tests/arith_dynamic_fuzz.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/arith_dynamic_test.c` & `ngsfragments-2.0.4/htslib/htscodecs/tests/arith_dynamic_test.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q4.0` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q4.0`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q4.1` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q4.1`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q4.128` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q4.128`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q4.129` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q4.129`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q4.192` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q4.192`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q4.193` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q4.193`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q4.64` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q4.64`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q4.65` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q4.65`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q4.8` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q4.8`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q4.9` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q4.9`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q40+dir.0` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q40+dir.0`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q40+dir.1` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q40+dir.1`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q40+dir.64` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q40+dir.64`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q40+dir.65` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q40+dir.65`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q40+dir.8` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q40+dir.8`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q40+dir.9` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q40+dir.9`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q8.0` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q8.0`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q8.1` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q8.1`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q8.128` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q8.128`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q8.129` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q8.129`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q8.192` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q8.192`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q8.193` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q8.193`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q8.64` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q8.64`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/q8.65` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/q8.65`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/qvar.0` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/qvar.0`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/qvar.1` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/qvar.1`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/qvar.64` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/qvar.64`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/arith/qvar.65` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/arith/qvar.65`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/q4.0` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/q4.0`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/q4.1` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/q4.1`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/q4.2` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/q4.2`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/q4.3` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/q4.3`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/q40+dir.0` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/q40+dir.0`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/q40+dir.1` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/q40+dir.1`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/q40+dir.2` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/q40+dir.2`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/q40+dir.3` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/q40+dir.3`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/q8.0` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/q8.0`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/q8.1` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/q8.1`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/q8.2` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/q8.2`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/q8.3` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/q8.3`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/qvar.0` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/qvar.0`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/qvar.1` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/qvar.1`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/qvar.2` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/qvar.2`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/fqzcomp/qvar.3` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/fqzcomp/qvar.3`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/q4` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/q4`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/q40+dir` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/q40+dir`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/q8` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/q8`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/qvar` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/qvar`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q4.0` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q4.0`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q4.1` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q4.1`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q4.128` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q4.128`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q4.129` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q4.129`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q4.192` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q4.192`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q4.193` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q4.193`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q4.64` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q4.64`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q4.65` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q4.65`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q4.8` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q4.8`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q4.9` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q4.9`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q40+dir.0` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q40+dir.0`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q40+dir.1` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q40+dir.1`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q40+dir.8` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q40+dir.8`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q40+dir.9` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q40+dir.9`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q8.0` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q8.0`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q8.1` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q8.1`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q8.128` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q8.128`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q8.129` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q8.129`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q8.192` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q8.192`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q8.193` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q8.193`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q8.64` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q8.64`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/q8.65` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/q8.65`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/qvar.0` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/qvar.0`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x16/qvar.1` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x16/qvar.1`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x8/q4.0` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x8/q4.0`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x8/q4.1` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x8/q4.1`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x8/q40+dir.0` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x8/q40+dir.0`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x8/q40+dir.1` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x8/q40+dir.1`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x8/q8.0` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x8/q8.0`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x8/q8.1` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x8/q8.1`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x8/qvar.0` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x8/qvar.0`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/dat/r4x8/qvar.1` & `ngsfragments-2.0.4/htslib/htscodecs/tests/dat/r4x8/qvar.1`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/fqzcomp.test` & `ngsfragments-2.0.4/htslib/htscodecs/tests/fqzcomp.test`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/fqzcomp_qual_fuzz.c` & `ngsfragments-2.0.4/htslib/htscodecs/tests/fqzcomp_qual_fuzz.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/fqzcomp_qual_test.c` & `ngsfragments-2.0.4/htslib/htscodecs/tests/fqzcomp_qual_test.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/01.names` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/01.names`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/02.names` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/02.names`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/03.names` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/03.names`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/05.names` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/05.names`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/08.names` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/08.names`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/09.names` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/09.names`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/10.names` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/10.names`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/20.names` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/20.names`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/nv.names` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/nv.names`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/nv2.names` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/nv2.names`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/rr.names` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/rr.names`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/01.names.1` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/01.names.1`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/01.names.11` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/01.names.11`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/01.names.13` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/01.names.13`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/01.names.15` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/01.names.15`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/01.names.17` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/01.names.17`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/01.names.19` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/01.names.19`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/01.names.3` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/01.names.3`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/01.names.5` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/01.names.5`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/01.names.7` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/01.names.7`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/01.names.9` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/01.names.9`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/02.names.1` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/02.names.1`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/02.names.11` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/02.names.11`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/02.names.13` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/02.names.13`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/02.names.15` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/02.names.15`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/02.names.17` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/02.names.17`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/02.names.19` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/02.names.19`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/02.names.3` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/02.names.3`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/02.names.5` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/02.names.5`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/02.names.7` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/02.names.7`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/02.names.9` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/02.names.9`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/03.names.1` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/03.names.1`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/03.names.11` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/03.names.11`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/03.names.13` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/03.names.13`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/03.names.15` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/03.names.15`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/03.names.17` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/03.names.17`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/03.names.19` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/03.names.19`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/03.names.3` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/03.names.3`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/03.names.5` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/03.names.5`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/03.names.7` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/03.names.7`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/03.names.9` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/03.names.9`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/05.names.1` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/05.names.1`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/05.names.11` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/05.names.11`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/05.names.13` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/05.names.13`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/05.names.15` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/05.names.15`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/05.names.17` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/05.names.17`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/05.names.19` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/05.names.19`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/05.names.3` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/05.names.3`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/05.names.5` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/05.names.5`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/05.names.7` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/05.names.7`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/05.names.9` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/05.names.9`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/08.names.1` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/08.names.1`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/08.names.11` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/08.names.11`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/08.names.13` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/08.names.13`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/08.names.15` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/08.names.15`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/08.names.17` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/08.names.17`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/08.names.19` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/08.names.19`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/08.names.3` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/08.names.3`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/08.names.5` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/08.names.5`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/08.names.7` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/08.names.7`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/08.names.9` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/08.names.9`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/09.names.1` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/09.names.1`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/09.names.11` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/09.names.11`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/09.names.13` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/09.names.13`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/09.names.15` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/09.names.15`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/09.names.17` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/09.names.17`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/09.names.19` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/09.names.19`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/09.names.3` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/09.names.3`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/09.names.5` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/09.names.5`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/09.names.7` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/09.names.7`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/09.names.9` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/09.names.9`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/10.names.1` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/10.names.1`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/10.names.11` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/10.names.11`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/10.names.13` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/10.names.13`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/10.names.15` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/10.names.15`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/10.names.17` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/10.names.17`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/10.names.19` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/10.names.19`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/10.names.3` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/10.names.3`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/10.names.5` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/10.names.5`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/10.names.7` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/10.names.7`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/10.names.9` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/10.names.9`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/20.names.1` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/20.names.1`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/20.names.11` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/20.names.11`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/20.names.13` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/20.names.13`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/20.names.15` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/20.names.15`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/20.names.17` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/20.names.17`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/20.names.19` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/20.names.19`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/20.names.3` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/20.names.3`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/20.names.5` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/20.names.5`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/20.names.7` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/20.names.7`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/20.names.9` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/20.names.9`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv.names.1` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv.names.1`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv.names.11` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv.names.11`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv.names.13` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv.names.13`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv.names.15` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv.names.15`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv.names.17` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv.names.17`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv.names.19` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv.names.19`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv.names.3` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv.names.3`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv.names.5` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv.names.5`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv.names.7` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv.names.7`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv.names.9` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv.names.9`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv2.names.1` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv2.names.1`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv2.names.11` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv2.names.11`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv2.names.13` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv2.names.13`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv2.names.15` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv2.names.15`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv2.names.17` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv2.names.17`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv2.names.19` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv2.names.19`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv2.names.3` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv2.names.3`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv2.names.5` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv2.names.5`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv2.names.7` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv2.names.7`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/nv2.names.9` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/nv2.names.9`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/rr.names.1` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/rr.names.1`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/rr.names.11` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/rr.names.11`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/rr.names.13` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/rr.names.13`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/rr.names.15` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/rr.names.15`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/rr.names.17` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/rr.names.17`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/rr.names.19` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/rr.names.19`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/rr.names.3` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/rr.names.3`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/rr.names.5` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/rr.names.5`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/rr.names.7` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/rr.names.7`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/names/tok3/rr.names.9` & `ngsfragments-2.0.4/htslib/htscodecs/tests/names/tok3/rr.names.9`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/rANS_static4x16pr_fuzz.c` & `ngsfragments-2.0.4/htslib/htscodecs/tests/rANS_static4x16pr_fuzz.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/rANS_static4x16pr_test.c` & `ngsfragments-2.0.4/htslib/htscodecs/tests/rANS_static4x16pr_test.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/rANS_static_fuzz.c` & `ngsfragments-2.0.4/htslib/htscodecs/tests/rANS_static_fuzz.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/rANS_static_test.c` & `ngsfragments-2.0.4/htslib/htscodecs/tests/rANS_static_test.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/rans4x16.test` & `ngsfragments-2.0.4/htslib/htscodecs/tests/rans4x16.test`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/rans4x8.test` & `ngsfragments-2.0.4/htslib/htscodecs/tests/rans4x8.test`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/tok3.test` & `ngsfragments-2.0.4/htslib/htscodecs/tests/tok3.test`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/tokenise_name3_fuzz.c` & `ngsfragments-2.0.4/htslib/htscodecs/tests/tokenise_name3_fuzz.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/tokenise_name3_test.c` & `ngsfragments-2.0.4/htslib/htscodecs/tests/tokenise_name3_test.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs/tests/varint_test.c` & `ngsfragments-2.0.4/htslib/htscodecs/tests/varint_test.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs_bundled.mk` & `ngsfragments-2.0.4/htslib/htscodecs_bundled.mk`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htscodecs_external.mk` & `ngsfragments-2.0.4/htslib/htscodecs_external.mk`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htsfile.1` & `ngsfragments-2.0.4/htslib/htsfile.1`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htsfile.c` & `ngsfragments-2.0.4/htslib/htsfile.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib/bgzf.h` & `ngsfragments-2.0.4/htslib/htslib/bgzf.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib/cram.h` & `ngsfragments-2.0.4/htslib/htslib/cram.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib/faidx.h` & `ngsfragments-2.0.4/htslib/htslib/faidx.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib/hfile.h` & `ngsfragments-2.0.4/htslib/htslib/hfile.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib/hts.h` & `ngsfragments-2.0.4/htslib/htslib/hts.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib/hts_defs.h` & `ngsfragments-2.0.4/htslib/htslib/hts_defs.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib/hts_endian.h` & `ngsfragments-2.0.4/htslib/htslib/hts_endian.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib/hts_expr.h` & `ngsfragments-2.0.4/htslib/htslib/hts_expr.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib/hts_log.h` & `ngsfragments-2.0.4/htslib/htslib/hts_log.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib/hts_os.h` & `ngsfragments-2.0.4/htslib/htslib/hts_os.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib/kbitset.h` & `ngsfragments-2.0.4/htslib/htslib/kbitset.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib/kfunc.h` & `ngsfragments-2.0.4/htslib/htslib/kfunc.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib/khash.h` & `ngsfragments-2.0.4/htslib/htslib/khash.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib/khash_str2int.h` & `ngsfragments-2.0.4/htslib/htslib/khash_str2int.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib/klist.h` & `ngsfragments-2.0.4/htslib/htslib/klist.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib/knetfile.h` & `ngsfragments-2.0.4/htslib/htslib/knetfile.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib/kroundup.h` & `ngsfragments-2.0.4/htslib/htslib/kroundup.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib/kseq.h` & `ngsfragments-2.0.4/htslib/htslib/kseq.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib/ksort.h` & `ngsfragments-2.0.4/htslib/htslib/ksort.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib/kstring.h` & `ngsfragments-2.0.4/htslib/htslib/kstring.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib/regidx.h` & `ngsfragments-2.0.4/htslib/htslib/regidx.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib/sam.h` & `ngsfragments-2.0.4/htslib/htslib/sam.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib/synced_bcf_reader.h` & `ngsfragments-2.0.4/htslib/htslib/synced_bcf_reader.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib/tbx.h` & `ngsfragments-2.0.4/htslib/htslib/tbx.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib/thread_pool.h` & `ngsfragments-2.0.4/htslib/htslib/thread_pool.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib/vcf.h` & `ngsfragments-2.0.4/htslib/htslib/vcf.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib/vcf_sweep.h` & `ngsfragments-2.0.4/htslib/htslib/vcf_sweep.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib/vcfutils.h` & `ngsfragments-2.0.4/htslib/htslib/vcfutils.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib-s3-plugin.7` & `ngsfragments-2.0.4/htslib/htslib-s3-plugin.7`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib.mk` & `ngsfragments-2.0.4/htslib/htslib.mk`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib.pc.tmp` & `ngsfragments-2.0.4/htslib/htslib.pc.tmp`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/htslib_vars.mk` & `ngsfragments-2.0.4/htslib/htslib_vars.mk`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/kfunc.c` & `ngsfragments-2.0.4/htslib/kfunc.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/kstring.c` & `ngsfragments-2.0.4/htslib/kstring.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/m4/hts_hide_dynamic_syms.m4` & `ngsfragments-2.0.4/htslib/m4/hts_hide_dynamic_syms.m4`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/m4/hts_prog_cc_warnings.m4` & `ngsfragments-2.0.4/htslib/m4/hts_prog_cc_warnings.m4`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/m4/pkg.m4` & `ngsfragments-2.0.4/htslib/m4/pkg.m4`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/md5.c` & `ngsfragments-2.0.4/htslib/md5.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/multipart.c` & `ngsfragments-2.0.4/htslib/multipart.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/os/lzma_stub.h` & `ngsfragments-2.0.4/htslib/os/lzma_stub.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/os/rand.c` & `ngsfragments-2.0.4/htslib/os/rand.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/plugin.c` & `ngsfragments-2.0.4/htslib/plugin.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/probaln.c` & `ngsfragments-2.0.4/htslib/probaln.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/realn.c` & `ngsfragments-2.0.4/htslib/realn.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/regidx.c` & `ngsfragments-2.0.4/htslib/regidx.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/region.c` & `ngsfragments-2.0.4/htslib/region.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/sam.5` & `ngsfragments-2.0.4/htslib/sam.5`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/sam.c` & `ngsfragments-2.0.4/htslib/sam.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/sam_internal.h` & `ngsfragments-2.0.4/htslib/sam_internal.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/synced_bcf_reader.c` & `ngsfragments-2.0.4/htslib/synced_bcf_reader.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/tabix.1` & `ngsfragments-2.0.4/htslib/tabix.1`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/tabix.c` & `ngsfragments-2.0.4/htslib/tabix.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/tbx.c` & `ngsfragments-2.0.4/htslib/tbx.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/auxf#values.sam` & `ngsfragments-2.0.4/htslib/test/auxf#values.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/auxf#values_java.cram` & `ngsfragments-2.0.4/htslib/test/auxf#values_java.cram`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/bcf-sr/merge.noidx.a.vcf` & `ngsfragments-2.0.4/htslib/test/bcf-sr/merge.noidx.a.vcf`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/bcf-sr/merge.noidx.b.vcf` & `ngsfragments-2.0.4/htslib/test/bcf-sr/merge.noidx.b.vcf`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/bcf-sr/merge.noidx.c.vcf` & `ngsfragments-2.0.4/htslib/test/bcf-sr/merge.noidx.c.vcf`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/bcf-sr/merge.noidx.hdr_order.vcf` & `ngsfragments-2.0.4/htslib/test/bcf-sr/merge.noidx.hdr_order.vcf`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/bcf-sr/merge.noidx.rec_order.vcf` & `ngsfragments-2.0.4/htslib/test/bcf-sr/merge.noidx.rec_order.vcf`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/c1#pad2.sam` & `ngsfragments-2.0.4/htslib/test/c1#pad2.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/c1#pad3.sam` & `ngsfragments-2.0.4/htslib/test/c1#pad3.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/c2#pad.sam` & `ngsfragments-2.0.4/htslib/test/c2#pad.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/ce#1000.sam` & `ngsfragments-2.0.4/htslib/test/ce#1000.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/ce#2.sam` & `ngsfragments-2.0.4/htslib/test/ce#2.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/ce#5.sam` & `ngsfragments-2.0.4/htslib/test/ce#5.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/ce#5b.sam` & `ngsfragments-2.0.4/htslib/test/ce#5b.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/ce#5b_java.cram` & `ngsfragments-2.0.4/htslib/test/ce#5b_java.cram`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/ce#large_seq.sam` & `ngsfragments-2.0.4/htslib/test/ce#large_seq.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/ce#supp.sam` & `ngsfragments-2.0.4/htslib/test/ce#supp.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/ce#tag_depadded.sam` & `ngsfragments-2.0.4/htslib/test/ce#tag_depadded.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/ce#tag_padded.sam` & `ngsfragments-2.0.4/htslib/test/ce#tag_padded.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/ce#unmap.sam` & `ngsfragments-2.0.4/htslib/test/ce#unmap.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/ce#unmap1.sam` & `ngsfragments-2.0.4/htslib/test/ce#unmap1.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/ce#unmap2.sam` & `ngsfragments-2.0.4/htslib/test/ce#unmap2.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/ce.fa` & `ngsfragments-2.0.4/htslib/test/ce.fa`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/compare_sam.pl` & `ngsfragments-2.0.4/htslib/test/compare_sam.pl`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/cross_validate.sh` & `ngsfragments-2.0.4/htslib/test/cross_validate.sh`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/fastqs.fq` & `ngsfragments-2.0.4/htslib/test/fastqs.fq`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/fastqs_README.txt` & `ngsfragments-2.0.4/htslib/test/fastqs_README.txt`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/fieldarith.c` & `ngsfragments-2.0.4/htslib/test/fieldarith.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/fieldarith.sam` & `ngsfragments-2.0.4/htslib/test/fieldarith.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/fuzz/hts_open_fuzzer.c` & `ngsfragments-2.0.4/htslib/test/fuzz/hts_open_fuzzer.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/header_syms.pl` & `ngsfragments-2.0.4/htslib/test/header_syms.pl`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/hfile.c` & `ngsfragments-2.0.4/htslib/test/hfile.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/hts_endian.c` & `ngsfragments-2.0.4/htslib/test/hts_endian.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/index.bam.bai` & `ngsfragments-2.0.4/htslib/test/index.bam.bai`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/index.sam` & `ngsfragments-2.0.4/htslib/test/index.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/index.sam.gz.bai` & `ngsfragments-2.0.4/htslib/test/index.sam.gz.bai`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/index.vcf` & `ngsfragments-2.0.4/htslib/test/index.vcf`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/index_dos.sam` & `ngsfragments-2.0.4/htslib/test/index_dos.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/longrefs/index.expected1.vcf` & `ngsfragments-2.0.4/htslib/test/longrefs/index.expected1.vcf`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/longrefs/index.vcf` & `ngsfragments-2.0.4/htslib/test/longrefs/index.vcf`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/longrefs/longref.sam` & `ngsfragments-2.0.4/htslib/test/longrefs/longref.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/longrefs/longref_itr.expected.sam` & `ngsfragments-2.0.4/htslib/test/longrefs/longref_itr.expected.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/longrefs/longref_multi.expected.sam` & `ngsfragments-2.0.4/htslib/test/longrefs/longref_multi.expected.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/maintainer/check_copyright.pl` & `ngsfragments-2.0.4/htslib/test/maintainer/check_copyright.pl`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/maintainer/check_spaces.pl` & `ngsfragments-2.0.4/htslib/test/maintainer/check_spaces.pl`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/md#1.sam` & `ngsfragments-2.0.4/htslib/test/md#1.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/mpileup/c1#pad1.sam` & `ngsfragments-2.0.4/htslib/test/mpileup/c1#pad1.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/mpileup/c1#pad2.sam` & `ngsfragments-2.0.4/htslib/test/mpileup/c1#pad2.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/mpileup/c1#pad3.sam` & `ngsfragments-2.0.4/htslib/test/mpileup/c1#pad3.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/mpileup/mp_D.sam` & `ngsfragments-2.0.4/htslib/test/mpileup/mp_D.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/mpileup/mp_DI.sam` & `ngsfragments-2.0.4/htslib/test/mpileup/mp_DI.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/mpileup/mp_I.sam` & `ngsfragments-2.0.4/htslib/test/mpileup/mp_I.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/mpileup/mp_ID.sam` & `ngsfragments-2.0.4/htslib/test/mpileup/mp_ID.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/mpileup/mp_N.sam` & `ngsfragments-2.0.4/htslib/test/mpileup/mp_N.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/mpileup/mp_N2.sam` & `ngsfragments-2.0.4/htslib/test/mpileup/mp_N2.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/mpileup/mp_P.sam` & `ngsfragments-2.0.4/htslib/test/mpileup/mp_P.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/mpileup/mpileup.tst` & `ngsfragments-2.0.4/htslib/test/mpileup/mpileup.tst`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/mpileup/small.bam` & `ngsfragments-2.0.4/htslib/test/mpileup/small.bam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/mpileup/small.out` & `ngsfragments-2.0.4/htslib/test/mpileup/small.out`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/mpileup/test-pileup.sh` & `ngsfragments-2.0.4/htslib/test/mpileup/test-pileup.sh`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/no_hdr_sq_1.bam` & `ngsfragments-2.0.4/htslib/test/no_hdr_sq_1.bam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/no_hdr_sq_1.expected.sam` & `ngsfragments-2.0.4/htslib/test/no_hdr_sq_1.expected.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/pileup.c` & `ngsfragments-2.0.4/htslib/test/pileup.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/plugins-dlhts.c` & `ngsfragments-2.0.4/htslib/test/plugins-dlhts.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/range.bam` & `ngsfragments-2.0.4/htslib/test/range.bam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/range.cram` & `ngsfragments-2.0.4/htslib/test/range.cram`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/range.out` & `ngsfragments-2.0.4/htslib/test/range.out`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/realn01.fa` & `ngsfragments-2.0.4/htslib/test/realn01.fa`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/realn01.sam` & `ngsfragments-2.0.4/htslib/test/realn01.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/realn01_exp-a.sam` & `ngsfragments-2.0.4/htslib/test/realn01_exp-a.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/realn01_exp-e.sam` & `ngsfragments-2.0.4/htslib/test/realn01_exp-e.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/realn01_exp.sam` & `ngsfragments-2.0.4/htslib/test/realn01_exp.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/realn02-r.sam` & `ngsfragments-2.0.4/htslib/test/realn02-r.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/realn02.fa` & `ngsfragments-2.0.4/htslib/test/realn02.fa`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/realn02.sam` & `ngsfragments-2.0.4/htslib/test/realn02.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/realn02_exp-a.sam` & `ngsfragments-2.0.4/htslib/test/realn02_exp-a.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/realn02_exp-e.sam` & `ngsfragments-2.0.4/htslib/test/realn02_exp-e.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/realn02_exp.sam` & `ngsfragments-2.0.4/htslib/test/realn02_exp.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/sam.c` & `ngsfragments-2.0.4/htslib/test/sam.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/sam_filter/filter.sh` & `ngsfragments-2.0.4/htslib/test/sam_filter/filter.sh`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/sam_filter/filter.tst` & `ngsfragments-2.0.4/htslib/test/sam_filter/filter.tst`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/sam_filter/string3.out` & `ngsfragments-2.0.4/htslib/test/sam_filter/string3.out`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/sam_filter/string4.out` & `ngsfragments-2.0.4/htslib/test/sam_filter/string4.out`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/simple_test_driver.sh` & `ngsfragments-2.0.4/htslib/test/simple_test_driver.sh`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/tabix/bed_file.bed` & `ngsfragments-2.0.4/htslib/test/tabix/bed_file.bed`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/tabix/gff_file.gff` & `ngsfragments-2.0.4/htslib/test/tabix/gff_file.gff`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/tabix/large_chr.vcf` & `ngsfragments-2.0.4/htslib/test/tabix/large_chr.vcf`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/tabix/tabix.tst` & `ngsfragments-2.0.4/htslib/test/tabix/tabix.tst`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/tabix/test-tabix.sh` & `ngsfragments-2.0.4/htslib/test/tabix/test-tabix.sh`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/tabix/vcf_file.bcf` & `ngsfragments-2.0.4/htslib/test/tabix/vcf_file.bcf`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/tabix/vcf_file.vcf` & `ngsfragments-2.0.4/htslib/test/tabix/vcf_file.vcf`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/test-bcf-sr.c` & `ngsfragments-2.0.4/htslib/test/test-bcf-sr.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/test-bcf-sr.pl` & `ngsfragments-2.0.4/htslib/test/test-bcf-sr.pl`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/test-bcf-translate.c` & `ngsfragments-2.0.4/htslib/test/test-bcf-translate.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/test-bcf-translate.out` & `ngsfragments-2.0.4/htslib/test/test-bcf-translate.out`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/test-logging.pl` & `ngsfragments-2.0.4/htslib/test/test-logging.pl`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/test-parse-reg.c` & `ngsfragments-2.0.4/htslib/test/test-parse-reg.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/test-regidx.c` & `ngsfragments-2.0.4/htslib/test/test-regidx.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/test-vcf-api.c` & `ngsfragments-2.0.4/htslib/test/test-vcf-api.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/test-vcf-api.out` & `ngsfragments-2.0.4/htslib/test/test-vcf-api.out`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/test-vcf-hdr-in.vcf` & `ngsfragments-2.0.4/htslib/test/test-vcf-hdr-in.vcf`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/test-vcf-hdr.out` & `ngsfragments-2.0.4/htslib/test/test-vcf-hdr.out`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/test-vcf-sweep.c` & `ngsfragments-2.0.4/htslib/test/test-vcf-sweep.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/test.pl` & `ngsfragments-2.0.4/htslib/test/test.pl`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/test_bgzf.c` & `ngsfragments-2.0.4/htslib/test/test_bgzf.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/test_expr.c` & `ngsfragments-2.0.4/htslib/test/test_expr.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/test_index.c` & `ngsfragments-2.0.4/htslib/test/test_index.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/test_introspection.c` & `ngsfragments-2.0.4/htslib/test/test_introspection.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/test_kfunc.c` & `ngsfragments-2.0.4/htslib/test/test_kfunc.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/test_kstring.c` & `ngsfragments-2.0.4/htslib/test/test_kstring.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/test_realn.c` & `ngsfragments-2.0.4/htslib/test/test_realn.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/test_str2int.c` & `ngsfragments-2.0.4/htslib/test/test_str2int.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/test_view.c` & `ngsfragments-2.0.4/htslib/test/test_view.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/thrash_threads1.c` & `ngsfragments-2.0.4/htslib/test/thrash_threads1.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/thrash_threads2.c` & `ngsfragments-2.0.4/htslib/test/thrash_threads2.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/thrash_threads3.c` & `ngsfragments-2.0.4/htslib/test/thrash_threads3.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/thrash_threads4.c` & `ngsfragments-2.0.4/htslib/test/thrash_threads4.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/thrash_threads5.c` & `ngsfragments-2.0.4/htslib/test/thrash_threads5.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/thrash_threads6.c` & `ngsfragments-2.0.4/htslib/test/thrash_threads6.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/thrash_threads7.c` & `ngsfragments-2.0.4/htslib/test/thrash_threads7.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/thread_pool.md` & `ngsfragments-2.0.4/htslib/test/thread_pool.md`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/with-shlib.sh` & `ngsfragments-2.0.4/htslib/test/with-shlib.sh`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/xx#MD.sam` & `ngsfragments-2.0.4/htslib/test/xx#MD.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/xx#MD2.sam` & `ngsfragments-2.0.4/htslib/test/xx#MD2.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/xx#large_aux.sam` & `ngsfragments-2.0.4/htslib/test/xx#large_aux.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/xx#large_aux2.sam` & `ngsfragments-2.0.4/htslib/test/xx#large_aux2.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/xx#large_aux_java.cram` & `ngsfragments-2.0.4/htslib/test/xx#large_aux_java.cram`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/xx#rg.sam` & `ngsfragments-2.0.4/htslib/test/xx#rg.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/xx#tlen.sam` & `ngsfragments-2.0.4/htslib/test/xx#tlen.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/test/xx#tlen2.sam` & `ngsfragments-2.0.4/htslib/test/xx#tlen2.sam`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/textutils.c` & `ngsfragments-2.0.4/htslib/textutils.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/textutils_internal.h` & `ngsfragments-2.0.4/htslib/textutils_internal.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/thread_pool.c` & `ngsfragments-2.0.4/htslib/thread_pool.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/thread_pool_internal.h` & `ngsfragments-2.0.4/htslib/thread_pool_internal.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/vcf.5` & `ngsfragments-2.0.4/htslib/vcf.5`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/vcf.c` & `ngsfragments-2.0.4/htslib/vcf.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/vcf_sweep.c` & `ngsfragments-2.0.4/htslib/vcf_sweep.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/vcfutils.c` & `ngsfragments-2.0.4/htslib/vcfutils.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/htslib/version.sh` & `ngsfragments-2.0.4/htslib/version.sh`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/.DS_Store` & `ngsfragments-2.0.4/ngsfragments/.DS_Store`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/correct/correct_intervals.py` & `ngsfragments-2.0.4/ngsfragments/correct/correct_intervals.py`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/correct/correction.py` & `ngsfragments-2.0.4/ngsfragments/correct/correction.py`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/correct/cylowess/cylowess.c` & `ngsfragments-2.0.4/ngsfragments/correct/cylowess/cylowess.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/correct/cylowess/cylowess.cpython-310-darwin.so` & `ngsfragments-2.0.4/ngsfragments/correct/cylowess/cylowess.cpython-310-darwin.so`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/correct/cylowess/cylowess.pyx` & `ngsfragments-2.0.4/ngsfragments/correct/cylowess/cylowess.pyx`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/coverage/coverage.py` & `ngsfragments-2.0.4/ngsfragments/coverage/coverage.py`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/coverage/midpoint.py` & `ngsfragments-2.0.4/ngsfragments/coverage/midpoint.py`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/coverage/wps.py` & `ngsfragments-2.0.4/ngsfragments/coverage/wps.py`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/fragments.py` & `ngsfragments-2.0.4/ngsfragments/fragments.py`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/io/parse_sam/ReadSam.c` & `ngsfragments-2.0.4/ngsfragments/io/parse_sam/ReadSam.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/io/parse_sam/ReadSam.cpython-310-darwin.so` & `ngsfragments-2.0.4/ngsfragments/io/parse_sam/ReadSam.cpython-310-darwin.so`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/io/parse_sam/ReadSam.pxd` & `ngsfragments-2.0.4/ngsfragments/io/parse_sam/ReadSam.pxd`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/io/parse_sam/ReadSam.pyx` & `ngsfragments-2.0.4/ngsfragments/io/parse_sam/ReadSam.pyx`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/io/parse_sam/read_intervals.c` & `ngsfragments-2.0.4/ngsfragments/io/parse_sam/read_intervals.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/io/parse_sam/read_intervals.h` & `ngsfragments-2.0.4/ngsfragments/io/parse_sam/read_intervals.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/io/parse_sam/read_intervals_v0.c` & `ngsfragments-2.0.4/ngsfragments/io/parse_sam/read_intervals_v0.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/io/read_sam.py` & `ngsfragments-2.0.4/ngsfragments/io/read_sam.py`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/metrics/gc_metrics.py` & `ngsfragments-2.0.4/ngsfragments/metrics/gc_metrics.py`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/metrics/gene_activity.py` & `ngsfragments-2.0.4/ngsfragments/metrics/gene_activity.py`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/peak_calling/.DS_Store` & `ngsfragments-2.0.4/ngsfragments/peak_calling/.DS_Store`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/peak_calling/CallPeaks.c` & `ngsfragments-2.0.4/ngsfragments/peak_calling/CallPeaks.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/peak_calling/CallPeaks.cpython-310-darwin.so` & `ngsfragments-2.0.4/ngsfragments/peak_calling/CallPeaks.cpython-310-darwin.so`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/peak_calling/CallPeaks.pyx` & `ngsfragments-2.0.4/ngsfragments/peak_calling/CallPeaks.pyx`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/peak_calling/RunningMean.c` & `ngsfragments-2.0.4/ngsfragments/peak_calling/RunningMean.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/peak_calling/RunningMean.cpython-310-darwin.so` & `ngsfragments-2.0.4/ngsfragments/peak_calling/RunningMean.cpython-310-darwin.so`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/peak_calling/RunningMean.pxd` & `ngsfragments-2.0.4/ngsfragments/peak_calling/RunningMean.pxd`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/peak_calling/RunningMean.pyx` & `ngsfragments-2.0.4/ngsfragments/peak_calling/RunningMean.pyx`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/peak_calling/RunningMedian.c` & `ngsfragments-2.0.4/ngsfragments/peak_calling/RunningMedian.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/peak_calling/RunningMedian.cpython-310-darwin.so` & `ngsfragments-2.0.4/ngsfragments/peak_calling/RunningMedian.cpython-310-darwin.so`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/peak_calling/RunningMedian.pxd` & `ngsfragments-2.0.4/ngsfragments/peak_calling/RunningMedian.pxd`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/peak_calling/RunningMedian.pyx` & `ngsfragments-2.0.4/ngsfragments/peak_calling/RunningMedian.pyx`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/peak_calling/running_mean.c` & `ngsfragments-2.0.4/ngsfragments/peak_calling/running_mean.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/peak_calling/sklist_pd.c` & `ngsfragments-2.0.4/ngsfragments/peak_calling/sklist_pd.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/peak_calling/sklist_pd.h` & `ngsfragments-2.0.4/ngsfragments/peak_calling/sklist_pd.h`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/plot/plot_bokeh.py` & `ngsfragments-2.0.4/ngsfragments/plot/plot_bokeh.py`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/plot/plot_plt.py` & `ngsfragments-2.0.4/ngsfragments/plot/plot_plt.py`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/segment/.DS_Store` & `ngsfragments-2.0.4/ngsfragments/segment/.DS_Store`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/segment/cnv.py` & `ngsfragments-2.0.4/ngsfragments/segment/cnv.py`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/segment/cnv_pipeline.py` & `ngsfragments-2.0.4/ngsfragments/segment/cnv_pipeline.py`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/segment/cnv_utilities.py` & `ngsfragments-2.0.4/ngsfragments/segment/cnv_utilities.py`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/segment/smooth_cnv/smoothCNV.c` & `ngsfragments-2.0.4/ngsfragments/segment/smooth_cnv/smoothCNV.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/segment/smooth_cnv/smooth_cnv.c` & `ngsfragments-2.0.4/ngsfragments/segment/smooth_cnv/smooth_cnv.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/segment/smooth_cnv/smooth_cnv.cpython-310-darwin.so` & `ngsfragments-2.0.4/ngsfragments/segment/smooth_cnv/smooth_cnv.cpython-310-darwin.so`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/segment/smooth_cnv/smooth_cnv.pyx` & `ngsfragments-2.0.4/ngsfragments/segment/smooth_cnv/smooth_cnv.pyx`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/sequence/kmer_query.py` & `ngsfragments-2.0.4/ngsfragments/sequence/kmer_query.py`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/sequence/snp_calling/snp_calling.c` & `ngsfragments-2.0.4/ngsfragments/sequence/snp_calling/snp_calling.c`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/sequence/snp_calling/snp_calling.pxd` & `ngsfragments-2.0.4/ngsfragments/sequence/snp_calling/snp_calling.pxd`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/sequence/snp_calling/snp_calling.pyx` & `ngsfragments-2.0.4/ngsfragments/sequence/snp_calling/snp_calling.pyx`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/ngsfragments/utilities.py` & `ngsfragments-2.0.4/ngsfragments/utilities.py`

 * *Files identical despite different names*

### Comparing `ngsfragments-2.0.3/pyproject.toml` & `ngsfragments-2.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ngsfragments"
-version = "2.0.3"
+version = "2.0.4"
 description = "Python package for Next Generation Sequencing fragment manipulation"
 authors = ["Kyle S. Smith <kyle.smith@stjude.org>"]
 maintainers = ["Kyle S. Smith <kyle.smith@stjude.org>"]
 repository = "https://github.com/kylessmith/ngsfragments"
 documentation = "https://www.biosciencestack.com/static/ngsfragments/docs/index.html"
 keywords = ["cython", "interval", "ngsfragments", "c"]
 readme = 'README.md'
@@ -36,15 +36,15 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.23.5"
 cython = "^0.29.32"
 pandas = "^1.5.2"
 ailist = "^2.1.0"
 linear_segment = "^1.1.0"
-pysam = "^0.20.0"
+pysam = "^0.21.0"
 intervalframe = "^1.1.3"
 matplotlib = "^3.7.1"
 bokeh = "^3.1.0"
 scipy = "^1.9.1"
 statsmodels = "^0.13.5"
 seaborn = "^0.12.2"
 projectframe = "^1.0.0"
```

### Comparing `ngsfragments-2.0.3/PKG-INFO` & `ngsfragments-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngsfragments
-Version: 2.0.3
+Version: 2.0.4
 Summary: Python package for Next Generation Sequencing fragment manipulation
 Home-page: https://github.com/kylessmith/ngsfragments
 License: GPL-2.0-or-later
 Keywords: cython,interval,ngsfragments,c
 Author: Kyle S. Smith
 Author-email: kyle.smith@stjude.org
 Maintainer: Kyle S. Smith
@@ -34,15 +34,15 @@
 Requires-Dist: hmmCNV (>=1.0.1,<2.0.0)
 Requires-Dist: intervalframe (>=1.1.3,<2.0.0)
 Requires-Dist: linear_segment (>=1.1.0,<2.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
 Requires-Dist: pandas (>=1.5.2,<2.0.0)
 Requires-Dist: projectframe (>=1.0.0,<2.0.0)
-Requires-Dist: pysam (>=0.20.0,<0.21.0)
+Requires-Dist: pysam (>=0.21.0,<0.22.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: scipy (>=1.9.1,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: statsmodels (>=0.13.5,<0.14.0)
 Project-URL: Documentation, https://www.biosciencestack.com/static/ngsfragments/docs/index.html
 Project-URL: Repository, https://github.com/kylessmith/ngsfragments
 Description-Content-Type: text/markdown
```

