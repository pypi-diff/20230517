# Comparing `tmp/ChannelAttribution-2.1.3.tar.gz` & `tmp/ChannelAttribution-2.1.4.tar.gz`

## Comparing `ChannelAttribution-2.1.3.tar` & `ChannelAttribution-2.1.4.tar`

### file list

```diff
@@ -1,614 +1,614 @@
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/
--rw-rw-r--   0 davide    (1000) davide    (1000)       69 2022-02-07 12:21:40.000000 ChannelAttribution-2.1.3/MANIFEST.in
--rw-rw-r--   0 davide    (1000) davide    (1000)      792 2022-02-07 12:21:40.000000 ChannelAttribution-2.1.3/LICENSE.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)     2308 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/PKG-INFO
--rw-rw-r--   0 davide    (1000) davide    (1000)      114 2022-02-07 12:21:40.000000 ChannelAttribution-2.1.3/pyproject.toml
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/
--rw-rw-r--   0 davide    (1000) davide    (1000)    55709 2022-02-07 12:21:40.000000 ChannelAttribution-2.1.3/src/cypack/ChannelAttribution.pyx
--rw-rw-r--   0 davide    (1000) davide    (1000)    39541 2022-02-07 12:21:40.000000 ChannelAttribution-2.1.3/src/cypack/functions.cpp
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/data/
--rw-rw-r--   0 davide    (1000) davide    (1000)   507116 2022-02-07 12:21:40.000000 ChannelAttribution-2.1.3/src/cypack/data/Data.csv
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/
--rw-rw-r--   0 davide    (1000) davide    (1000)    30011 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/
--rw-rw-r--   0 davide    (1000) davide    (1000)    11803 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_cube_slices_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1294 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/CubeToMatOp_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4113 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_hypot_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    18630 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/auxlib_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1114 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cor_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    14153 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_mean_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2062 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_shift.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1788 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_min_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1600 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_static_check.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2628 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/hdf5_name.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1650 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/span.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1216 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_cov_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     9041 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/def_atlas.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2635 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_join_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4094 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_kron_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1994 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_hist.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3543 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_elem2_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     8483 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_div.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2622 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_strans.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1581 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_find_unique.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3546 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_resize_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3971 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_chi2rnd_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     7031 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/podarray_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1313 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_normalise_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    11433 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_all_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     7440 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/BaseCube_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    21305 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_elem.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1951 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_polyval_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1331 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_nonzeros_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1273 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_prod_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4704 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_svd.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2250 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/unwrap_cube.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     5212 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_SortEigenvalue.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1437 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/GlueCube_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    97754 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1184 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_range_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1554 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_kmeans.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)      815 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/compiler_setup_post.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2792 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cond_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1132 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_trimat_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4833 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_cube_each_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    14171 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_approx_equal.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3717 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_chi2rnd.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2354 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_reverse_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1923 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_stddev.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1288 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cumsum_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    18866 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_ostream_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1752 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_index_max_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1458 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_chi2rnd_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    11193 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/config.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1537 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtGlueCube_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    11016 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fft_engine.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     9571 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/band_helper.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1479 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SizeMat_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4068 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/def_superlu.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1106 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_hist_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    20201 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_norm_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1216 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_cor_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    11768 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_SymEigsSolver_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2442 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_inplace_trans.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3041 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_eig_pair.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2896 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_var.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    14416 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/running_stat_vec_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    18533 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_times_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    10585 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_diagmat_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1739 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_quantile.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1574 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_trapz_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    15000 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpBase_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1104 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_resize_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     8959 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpRow_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3990 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_reverse_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4436 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_inv_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1194 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/compiler_extra.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2768 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_rel_comparators.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2763 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_sum.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3247 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_mean_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)   106690 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/def_lapack.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1359 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_diagvec_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2133 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Op_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1292 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/distr_param.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1704 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sort_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1525 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_cov.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2500 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_schur.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2617 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Op_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3643 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_hess.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2648 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_stddev_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1478 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_version.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2037 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_UpperHessenbergEigen_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    11396 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_as_scalar.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4433 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpBase_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    19223 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_elem2_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2902 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/eOpCube_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1493 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_hypot_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     9043 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_schur.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2547 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_UpperHessenbergQR_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1046 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_stddev_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     5282 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_powmat_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1724 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtGlue_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2539 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_var_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     5410 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_randi.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1511 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_polyfit_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1743 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_affmul_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    24709 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpProxy.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    30357 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_each_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    13014 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mul_gemv.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1349 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_SparseGenMatProd_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1175 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_pinv_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1899 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mp_misc.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1474 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_strans_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3520 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_eigs_gen.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2836 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_join_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3161 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_randperm.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2304 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_expmat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1684 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_histc.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    13212 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_cmath.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1562 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_range.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1016 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_toeplitz_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1149 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_repmat_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3349 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_norm_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3407 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_trimat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    10296 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_join_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2287 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/eGlue_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    12332 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cx_scalar_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    27214 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_max_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1296 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_polyval_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    12134 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_plus.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    16131 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpSubview_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3844 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/csv_name.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1323 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_unique.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1509 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_hist_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     6523 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_min_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3143 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_elem_helper_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1237 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_reverse_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2428 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Gen_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)   151041 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpMat_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1870 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtSpOp_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1620 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtSpGlue_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2704 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtOpCube_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1421 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/include_hdf5.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3783 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_dotext_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     5550 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_shift_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    19411 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/arrayops_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2174 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_trimat_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1139 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_chol_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2320 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/GenCube_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3854 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_relational_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2752 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_mean.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4787 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sort_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1674 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpOp_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3516 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_symmat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1541 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SizeCube_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1869 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_all.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1453 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_intersect_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    23212 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_accu.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2125 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/access.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1426 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_trapz.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2961 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_fft.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2114 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/xvec_htrans_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     5402 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_solve_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3493 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_relational_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1565 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_htrans_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2816 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_sprandu.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3176 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_cube_schur.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)   122818 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Cube_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    21615 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spdiagview_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     5512 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_expmat_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4054 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_eig_gen.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1295 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/cond_rel_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4176 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_config.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3299 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SizeCube_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    34646 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_times_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3272 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_field_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1723 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_inv_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     6523 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_max_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     7793 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/MapMat_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2344 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_max_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4214 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_wishrnd.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1991 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_schur_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     6978 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/gmm_full_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2231 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_eps.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1433 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtSpGlue_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4191 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_UpperHessenbergEigen_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     8197 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_interp2.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4867 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_rng_cxx11.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1906 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_toeplitz_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2455 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_sum_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2134 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/typedef_elem_check.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    12978 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_affmul_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    11286 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/config.hpp.cmake
--rw-rw-r--   0 davide    (1000) davide    (1000)     1244 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_nonzeros.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3959 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_min_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    10732 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/def_arpack.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1799 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_TridiagEigen_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1882 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_reverse.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2005 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_chol.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1632 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_vectorise_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3156 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_fft2.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    65539 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/gmm_diag_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2828 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_times_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1998 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_wishrnd_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3129 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/gmm_misc_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1687 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_diff.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1989 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_trans.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     5617 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_quantile_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1377 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/include_atlas.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2508 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_DoubleShiftQR_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3486 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_logmat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4322 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_reshape.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1647 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sp_plus_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1493 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_atan2_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     9582 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_var_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     9985 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_index_min_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     9700 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/translate_arpack.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    81970 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/translate_lapack.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3297 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_roots_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4559 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_histc_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2841 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/OpCube_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2517 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/OpCube_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1345 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_DenseGenMatProd_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1134 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_normalise_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    13647 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mul_herk.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1346 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_spones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2554 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_vectorise_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3575 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_dot_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    10728 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mul_gemm_mixed.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    11090 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_join.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    12376 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_field_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    14274 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_htrans_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4694 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_size.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     5279 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_max.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2110 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_speye.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1496 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_htrans_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    47137 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/eglue_core_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1651 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_reshape_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1650 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_shuffle.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1083 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cond_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    15762 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/diagmat_proxy.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3372 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_polyfit_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    11062 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sqrtmat_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3395 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_intersect_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     5866 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/memory.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1450 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_diagvec.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    11776 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_GenEigsSolver_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3275 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_ostream_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1904 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_trunc_exp.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    44133 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Mat_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3420 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_normalise_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     6528 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/sympd_helper.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2399 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/podarray_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1989 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/xtrans_mat_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2444 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_resize.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1602 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_flip_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3966 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/typedef_mat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     8945 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_misc_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    11139 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/constants.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1839 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_clamp_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3710 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_sort_index.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    12603 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_logmat_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2521 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtOp_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1293 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_diff_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    25327 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpMat_iterators_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1505 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_orth_null_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1768 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_plus_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1168 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_cross_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    16312 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_trace.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     5465 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_max_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     7405 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_UpperHessenbergQR_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3257 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sort_index_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1293 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cumprod_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    11543 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_rng.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3786 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/eGlue_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2013 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_var_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     9015 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_reshape_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4995 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_diff_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3110 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_strans_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    10351 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/translate_blas.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2278 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpToDOp_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2132 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_any_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     6062 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_flip_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1321 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_merge_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2739 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpCol_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     6993 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/constants_old.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1594 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpGlue_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     5203 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_misc_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    64647 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_cube_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2570 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sp_minus_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    61755 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/field_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2729 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_mvnrnd.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2344 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_min_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    10441 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Row_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1114 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cov_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    16374 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_min_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)      989 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_sum_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    11190 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_forward.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     9829 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_solve.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     9154 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_svds.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    34942 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Row_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2637 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cov_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2371 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/wall_clock_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4538 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_eig_sym.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2746 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_clamp.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    13125 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/translate_atlas.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     7523 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_cube_relational.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    11015 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/injector_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2132 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_all_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1473 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtGlueCube_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    72198 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/unwrap.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    11453 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_misc_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4420 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sort_index_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2566 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/injector_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3156 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_index_min.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     7012 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_dot.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3156 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_index_max.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     7304 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_find.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1747 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_cumprod.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    17717 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/compiler_setup.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2071 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/eGlueCube_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     6262 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_hist_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1226 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_cross.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     6065 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Base_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3610 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_det.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     5430 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_shuffle_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3504 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_kron_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3111 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_ostream.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2782 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_eye.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3112 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_TridiagEigen_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2382 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_symmat_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2736 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpRow_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     7185 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Gen_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2725 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_toeplitz_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1633 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/CubeToMatOp_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1656 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_kron_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    11121 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_str.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1734 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_quantile_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3869 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_strans_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4273 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/translate_superlu.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     5925 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_each_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    14147 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_merge_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    22905 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_elem1_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2563 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_powmat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3035 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_find_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     9455 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_DoubleShiftQR_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1191 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_symmat_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1323 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_repmat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    21404 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2234 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_range_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    10419 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_diagmat_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1266 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpToDOp_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4834 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_cube_plus.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4772 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_cube_minus.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    31865 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/debug.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3543 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spdiagview_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2002 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_fft_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1788 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_max_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1333 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_powmat_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     8023 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_relational_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    67945 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/gmm_full_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1736 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_cumsum.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     5492 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_spsolve.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3034 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/eOp_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2815 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_cube_times.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1742 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_polyfit.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2604 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_syl_lyap.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    13320 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/diskio_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     7365 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_wishrnd_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3165 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_log_det.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1458 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_expmat_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1345 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_cx_attrib.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     5327 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/GenCube_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    33981 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpSubview_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3830 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_ones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1533 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_toeplitz.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2113 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtSpOp_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    15573 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_find_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1506 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_histc_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    10494 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_any_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3377 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_cube_slices_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2365 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtOpCube_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2285 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_cross_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    12570 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_minus.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)   112626 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/diskio_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1527 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_cor.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1181 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_reverse_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    32307 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpSubview_iterators_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    12770 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mul_gemm.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4444 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/sp_auxlib_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    17558 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_conv_to.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2221 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_pinv.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4316 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_prod_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     7051 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_relational_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     8752 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_trig.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1329 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_roots_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     5525 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_log_normpdf.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    35544 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpMat_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2356 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sum_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2103 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_prod.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1723 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/GenSpecialiser.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3020 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/eglue_core_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    20647 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/hdf5_misc.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3695 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cumsum_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2691 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/BaseCube_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     9903 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/include_superlu.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1691 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_min_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2257 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_mean_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2054 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_cov_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1330 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_repelem.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     5103 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/upgrade_val.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4850 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_mvnrnd_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3019 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_mixed_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    12428 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sum_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4533 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_cube_div.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2704 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SizeMat_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1673 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/xtrans_mat_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     9148 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_schur_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1328 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_kron_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1914 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpOp_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1976 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_minus_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     6611 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_randg.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4160 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/eGlueCube_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2197 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_diagmat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2097 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_diagmat_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4150 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_orth_null_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3334 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_repmat_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     5681 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_atan2_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3035 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cor_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     8593 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_fft_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2923 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/strip.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1825 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_unique_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    15975 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/field_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     9985 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_index_max_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     9996 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/restrictors.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     5705 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_regspace.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2491 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_chol_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2523 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_normalise.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     8241 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpCol_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2409 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_kron.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     5459 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_min_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)   200436 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Mat_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1211 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_DenseGenMatProd_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1606 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_conv_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3030 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_find_unique_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     5293 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_times_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    12474 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_misc.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1774 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_diagmat_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     5937 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_normcdf.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)   178262 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/auxlib_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     8610 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_mean_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    26376 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/traits.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    10452 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Col_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     5655 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/running_stat_vec_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     8867 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_cube_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1605 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_intersect.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    11241 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_median_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2269 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_lu.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2186 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Glue_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    22986 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/ProxyCube.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    27217 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_min_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3856 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_rng_cxx98.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     7250 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_plus_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3963 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/unwrap_spmat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     7192 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/eop_core_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1691 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_max_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3733 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_trapz_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2002 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/cond_rel_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    35001 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Col_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     5112 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/typedef_elem.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    11657 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_join_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1248 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_polyval.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     6009 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_clamp_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     7737 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_inv.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1162 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_elem_helper_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2651 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpValProxy_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2352 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sqrtmat_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2790 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_hist_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1445 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtGlue_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1780 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_numel.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3005 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/running_stat_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    10234 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_relational_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3957 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_max_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4329 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_randu.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3860 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_SymEigsSolver_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1359 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Glue_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     5233 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_symmat_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     7223 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_norm.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3586 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_unique_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    12651 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mul_syrk.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2850 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_sprandn.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2410 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_orth_null.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2390 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtOp_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3915 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_elem1_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2706 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_repelem_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4355 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_randn.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    49167 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/sp_auxlib_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2162 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_conv.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1219 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_SparseGenMatProd_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1181 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_toeplitz_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2356 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_vectorise_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    13170 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_dot_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     8194 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_princomp_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3707 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/diagview_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    19380 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Base_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    26690 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Cube_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3452 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_trimat_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4450 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_princomp.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4103 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_htrans_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1869 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_any.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     9932 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_trimat_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4025 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_GenEigsSolver_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     8559 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/running_stat_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    34555 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/MapMat_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1225 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/GlueCube_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     8897 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_conv_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     7196 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_var_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1752 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_index_min_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     6739 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sp_minus_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2152 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_cor_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2047 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_princomp_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4648 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_repmat_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3374 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_diagvec_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     7179 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/gmm_diag_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1579 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_shift_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    15254 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_mixed_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     8408 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_minus_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2473 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/trimat_helper.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    10257 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/def_blas.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     9947 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/typedef_mat_fixed.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    20246 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/eop_aux.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2358 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_vectorise.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1363 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_cond.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3320 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_eigs_sym.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1364 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/wall_clock_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2925 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_nonzeros_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3858 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/eOpCube_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2027 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_trunc_log.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    10985 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_times.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2195 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_misc_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3747 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sp_plus_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     8852 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_vectorise_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2229 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_EigsSelect.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3291 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_n_unique.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1528 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_dotext_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    15656 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_max_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     6638 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/def_hdf5.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2524 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/eOp_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1697 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpGlue_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4487 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_sort.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    22436 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_cube_each_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4137 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_pinv_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1173 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_symmat_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1566 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/xvec_htrans_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1497 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_relational_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3638 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/gmm_misc_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3365 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_sqrtmat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     3706 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cumprod_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    89635 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Proxy.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1783 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_rank.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4051 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cx_scalar_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    21581 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/diagview_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     5360 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_normalise_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2040 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_qr.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1138 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_repmat_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     5279 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_min.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     4705 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_zeros.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1698 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_median.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     5912 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/arrayops_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     6557 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpValProxy_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1152 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_repelem_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     5455 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_normpdf.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1691 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_flip.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    20110 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_strans_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1287 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_shuffle_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2555 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_logmat_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     2595 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_inplace_strans.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1868 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_qz.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     8822 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_interp1.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     8602 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_relational.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1860 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_find_unique_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    14914 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/promote_type.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1978 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_median_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1718 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_mvnrnd_bones.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)     1616 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_roots.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    31181 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/eop_core_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)    17293 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_solve_meat.hpp
--rw-rw-r--   0 davide    (1000) davide    (1000)      516 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/NOTICE.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)    11358 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/LICENSE.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)    18591 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/README.md
--rw-rw-r--   0 davide    (1000) davide    (1000)     2245 2022-02-07 12:21:40.000000 ChannelAttribution-2.1.3/src/cypack/functions.h
--rw-rw-r--   0 davide    (1000) davide    (1000)      180 2022-02-07 12:21:40.000000 ChannelAttribution-2.1.3/src/cypack/__init__.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     1453 2022-02-07 12:21:40.000000 ChannelAttribution-2.1.3/src/cypack/generate_doc.py
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/ChannelAttribution.egg-info/
--rw-rw-r--   0 davide    (1000) davide    (1000)        1 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/ChannelAttribution.egg-info/dependency_links.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)        1 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/ChannelAttribution.egg-info/not-zip-safe
--rw-rw-r--   0 davide    (1000) davide    (1000)     2308 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/ChannelAttribution.egg-info/PKG-INFO
--rw-rw-r--   0 davide    (1000) davide    (1000)      498 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/ChannelAttribution.egg-info/SOURCES.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)       13 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/ChannelAttribution.egg-info/requires.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)       26 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/src/ChannelAttribution.egg-info/top_level.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)      545 2022-02-07 12:21:40.000000 ChannelAttribution-2.1.3/setup.py
--rw-rw-r--   0 davide    (1000) davide    (1000)      811 2022-02-07 12:21:40.000000 ChannelAttribution-2.1.3/README.md
--rw-rw-r--   0 davide    (1000) davide    (1000)     1574 2022-02-07 12:54:11.000000 ChannelAttribution-2.1.3/setup.cfg
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/
+-rw-rw-r--   0 davide    (1000) davide    (1000)       69 2023-05-17 09:09:30.000000 ChannelAttribution-2.1.4/MANIFEST.in
+-rw-rw-r--   0 davide    (1000) davide    (1000)      792 2023-05-17 09:09:30.000000 ChannelAttribution-2.1.4/LICENSE.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2308 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/PKG-INFO
+-rw-rw-r--   0 davide    (1000) davide    (1000)      114 2023-05-17 09:09:30.000000 ChannelAttribution-2.1.4/pyproject.toml
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/
+-rw-rw-r--   0 davide    (1000) davide    (1000)    59686 2023-05-17 09:09:30.000000 ChannelAttribution-2.1.4/src/cypack/ChannelAttribution.pyx
+-rw-rw-r--   0 davide    (1000) davide    (1000)    39541 2023-05-17 09:09:30.000000 ChannelAttribution-2.1.4/src/cypack/functions.cpp
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/data/
+-rw-rw-r--   0 davide    (1000) davide    (1000)   507116 2023-05-17 09:09:30.000000 ChannelAttribution-2.1.4/src/cypack/data/Data.csv
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/
+-rw-rw-r--   0 davide    (1000) davide    (1000)    30011 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/
+-rw-rw-r--   0 davide    (1000) davide    (1000)    11803 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_cube_slices_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1294 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/CubeToMatOp_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4113 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_hypot_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    18630 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/auxlib_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1114 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cor_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    14153 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_mean_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2062 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_shift.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1788 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_min_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1600 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_static_check.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2628 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/hdf5_name.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1650 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/span.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1216 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_cov_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     9041 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/def_atlas.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2635 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_join_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4094 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_kron_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1994 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_hist.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3543 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_elem2_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     8483 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_div.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2622 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_strans.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1581 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_find_unique.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3546 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_resize_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3971 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_chi2rnd_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     7031 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/podarray_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1313 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_normalise_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    11433 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_all_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     7440 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/BaseCube_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    21305 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_elem.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1951 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_polyval_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1331 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_nonzeros_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1273 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_prod_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4704 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_svd.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2250 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/unwrap_cube.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     5212 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_SortEigenvalue.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1437 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/GlueCube_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    97754 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1184 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_range_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1554 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_kmeans.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)      815 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/compiler_setup_post.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2792 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cond_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1132 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_trimat_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4833 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_cube_each_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    14171 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_approx_equal.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3717 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_chi2rnd.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2354 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_reverse_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1923 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_stddev.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1288 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cumsum_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    18866 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_ostream_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1752 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_index_max_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1458 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_chi2rnd_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    11193 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/config.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1537 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtGlueCube_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    11016 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fft_engine.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     9571 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/band_helper.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1479 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SizeMat_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4068 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/def_superlu.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1106 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_hist_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    20201 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_norm_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1216 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_cor_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    11768 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_SymEigsSolver_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2442 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_inplace_trans.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3041 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_eig_pair.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2896 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_var.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    14416 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/running_stat_vec_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    18533 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_times_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    10585 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_diagmat_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1739 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_quantile.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1574 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_trapz_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    15000 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpBase_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1104 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_resize_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     8959 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpRow_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3990 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_reverse_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4436 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_inv_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1194 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/compiler_extra.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2768 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_rel_comparators.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2763 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_sum.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3247 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_mean_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)   106690 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/def_lapack.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1359 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_diagvec_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2133 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Op_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1292 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/distr_param.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1704 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sort_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1525 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_cov.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2500 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_schur.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2617 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Op_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3643 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_hess.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2648 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_stddev_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1478 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_version.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2037 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_UpperHessenbergEigen_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    11396 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_as_scalar.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4433 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpBase_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    19223 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_elem2_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2902 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/eOpCube_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1493 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_hypot_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     9043 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_schur.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2547 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_UpperHessenbergQR_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1046 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_stddev_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     5282 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_powmat_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1724 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtGlue_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2539 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_var_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     5410 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_randi.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1511 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_polyfit_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1743 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_affmul_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    24709 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpProxy.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    30357 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_each_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    13014 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mul_gemv.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1349 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_SparseGenMatProd_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1175 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_pinv_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1899 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mp_misc.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1474 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_strans_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3520 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_eigs_gen.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2836 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_join_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3161 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_randperm.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2304 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_expmat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1684 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_histc.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    13212 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_cmath.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1562 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_range.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1016 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_toeplitz_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1149 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_repmat_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3349 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_norm_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3407 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_trimat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    10296 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_join_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2287 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/eGlue_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    12332 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cx_scalar_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    27214 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_max_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1296 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_polyval_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    12134 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_plus.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    16131 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpSubview_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3844 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/csv_name.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1323 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_unique.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1509 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_hist_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     6523 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_min_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3143 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_elem_helper_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1237 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_reverse_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2428 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Gen_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)   151041 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpMat_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1870 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtSpOp_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1620 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtSpGlue_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2704 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtOpCube_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1421 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/include_hdf5.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3783 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_dotext_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     5550 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_shift_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    19411 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/arrayops_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2174 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_trimat_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1139 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_chol_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2320 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/GenCube_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3854 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_relational_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2752 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_mean.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4787 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sort_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1674 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpOp_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3516 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_symmat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1541 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SizeCube_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1869 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_all.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1453 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_intersect_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    23212 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_accu.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2125 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/access.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1426 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_trapz.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2961 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_fft.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2114 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/xvec_htrans_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     5402 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_solve_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3493 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_relational_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1565 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_htrans_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2816 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_sprandu.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3176 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_cube_schur.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)   122818 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Cube_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    21615 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spdiagview_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     5512 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_expmat_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4054 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_eig_gen.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1295 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/cond_rel_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4176 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_config.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3299 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SizeCube_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    34646 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_times_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3272 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_field_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1723 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_inv_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     6523 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_max_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     7793 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/MapMat_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2344 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_max_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4214 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_wishrnd.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1991 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_schur_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     6978 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/gmm_full_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2231 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_eps.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1433 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtSpGlue_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4191 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_UpperHessenbergEigen_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     8197 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_interp2.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4867 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_rng_cxx11.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1906 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_toeplitz_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2455 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_sum_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2134 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/typedef_elem_check.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    12978 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_affmul_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    11286 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/config.hpp.cmake
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1244 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_nonzeros.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3959 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_min_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    10732 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/def_arpack.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1799 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_TridiagEigen_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1882 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_reverse.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2005 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_chol.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1632 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_vectorise_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3156 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_fft2.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    65539 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/gmm_diag_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2828 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_times_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1998 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_wishrnd_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3129 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/gmm_misc_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1687 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_diff.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1989 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_trans.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     5617 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_quantile_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1377 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/include_atlas.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2508 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_DoubleShiftQR_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3486 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_logmat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4322 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_reshape.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1647 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sp_plus_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1493 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_atan2_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     9582 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_var_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     9985 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_index_min_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     9700 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/translate_arpack.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    81970 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/translate_lapack.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3297 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_roots_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4559 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_histc_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2841 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/OpCube_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2517 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/OpCube_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1345 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_DenseGenMatProd_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1134 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_normalise_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    13647 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mul_herk.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1346 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_spones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2554 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_vectorise_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3575 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_dot_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    10728 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mul_gemm_mixed.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    11090 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_join.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    12376 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_field_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    14274 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_htrans_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4694 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_size.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     5279 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_max.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2110 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_speye.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1496 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_htrans_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    47137 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/eglue_core_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1651 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_reshape_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1650 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_shuffle.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1083 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cond_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    15762 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/diagmat_proxy.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3372 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_polyfit_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    11062 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sqrtmat_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3395 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_intersect_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     5866 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/memory.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1450 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_diagvec.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    11776 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_GenEigsSolver_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3275 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_ostream_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1904 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_trunc_exp.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    44133 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Mat_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3420 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_normalise_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     6528 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/sympd_helper.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2399 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/podarray_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1989 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/xtrans_mat_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2444 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_resize.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1602 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_flip_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3966 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/typedef_mat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     8945 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_misc_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    11139 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/constants.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1839 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_clamp_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3710 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_sort_index.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    12603 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_logmat_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2521 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtOp_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1293 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_diff_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    25327 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpMat_iterators_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1505 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_orth_null_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1768 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_plus_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1168 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_cross_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    16312 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_trace.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     5465 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_max_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     7405 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_UpperHessenbergQR_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3257 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sort_index_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1293 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cumprod_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    11543 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_rng.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3786 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/eGlue_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2013 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_var_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     9015 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_reshape_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4995 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_diff_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3110 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_strans_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    10351 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/translate_blas.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2278 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpToDOp_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2132 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_any_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     6062 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_flip_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1321 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_merge_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2739 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpCol_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     6993 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/constants_old.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1594 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpGlue_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     5203 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_misc_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    64647 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_cube_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2570 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sp_minus_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    61755 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/field_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2729 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_mvnrnd.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2344 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_min_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    10441 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Row_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1114 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cov_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    16374 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_min_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)      989 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_sum_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    11190 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_forward.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     9829 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_solve.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     9154 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_svds.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    34942 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Row_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2637 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cov_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2371 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/wall_clock_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4538 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_eig_sym.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2746 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_clamp.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    13125 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/translate_atlas.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     7523 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_cube_relational.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    11015 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/injector_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2132 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_all_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1473 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtGlueCube_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    72198 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/unwrap.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    11453 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_misc_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4420 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sort_index_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2566 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/injector_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3156 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_index_min.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     7012 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_dot.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3156 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_index_max.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     7304 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_find.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1747 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_cumprod.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    17717 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/compiler_setup.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2071 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/eGlueCube_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     6262 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_hist_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1226 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_cross.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     6065 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Base_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3610 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_det.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     5430 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_shuffle_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3504 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_kron_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3111 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_ostream.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2782 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_eye.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3112 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_TridiagEigen_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2382 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_symmat_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2736 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpRow_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     7185 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Gen_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2725 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_toeplitz_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1633 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/CubeToMatOp_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1656 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_kron_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    11121 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_str.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1734 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_quantile_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3869 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_strans_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4273 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/translate_superlu.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     5925 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_each_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    14147 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_merge_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    22905 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_elem1_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2563 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_powmat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3035 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_find_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     9455 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_DoubleShiftQR_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1191 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_symmat_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1323 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_repmat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    21404 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2234 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_range_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    10419 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_diagmat_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1266 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpToDOp_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4834 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_cube_plus.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4772 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_cube_minus.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    31865 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/debug.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3543 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spdiagview_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2002 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_fft_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1788 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_max_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1333 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_powmat_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     8023 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_relational_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    67945 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/gmm_full_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1736 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_cumsum.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     5492 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_spsolve.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3034 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/eOp_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2815 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_cube_times.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1742 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_polyfit.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2604 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_syl_lyap.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    13320 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/diskio_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     7365 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_wishrnd_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3165 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_log_det.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1458 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_expmat_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1345 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_cx_attrib.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     5327 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/GenCube_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    33981 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpSubview_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3830 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_ones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1533 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_toeplitz.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2113 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtSpOp_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    15573 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_find_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1506 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_histc_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    10494 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_any_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3377 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_cube_slices_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2365 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtOpCube_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2285 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_cross_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    12570 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_minus.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)   112626 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/diskio_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1527 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_cor.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1181 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_reverse_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    32307 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpSubview_iterators_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    12770 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mul_gemm.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4444 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/sp_auxlib_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    17558 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_conv_to.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2221 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_pinv.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4316 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_prod_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     7051 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_relational_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     8752 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_trig.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1329 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_roots_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     5525 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_log_normpdf.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    35544 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpMat_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2356 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sum_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2103 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_prod.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1723 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/GenSpecialiser.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3020 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/eglue_core_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    20647 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/hdf5_misc.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3695 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cumsum_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2691 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/BaseCube_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     9903 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/include_superlu.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1691 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_min_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2257 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_mean_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2054 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_cov_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1330 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_repelem.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     5103 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/upgrade_val.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4850 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_mvnrnd_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3019 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_mixed_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    12428 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sum_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4533 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_cube_div.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2704 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SizeMat_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1673 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/xtrans_mat_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     9148 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_schur_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1328 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_kron_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1914 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpOp_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1976 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_minus_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     6611 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_randg.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4160 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/eGlueCube_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2197 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_diagmat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2097 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_diagmat_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4150 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_orth_null_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3334 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_repmat_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     5681 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_atan2_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3035 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cor_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     8593 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_fft_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2923 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/strip.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1825 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_unique_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    15975 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/field_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     9985 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_index_max_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     9996 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/restrictors.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     5705 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_regspace.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2491 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_chol_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2523 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_normalise.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     8241 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpCol_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2409 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_kron.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     5459 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_min_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)   200436 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Mat_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1211 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_DenseGenMatProd_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1606 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_conv_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3030 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_find_unique_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     5293 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_times_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    12474 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_misc.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1774 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_diagmat_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     5937 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_normcdf.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)   178262 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/auxlib_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     8610 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_mean_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    26376 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/traits.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    10452 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Col_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     5655 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/running_stat_vec_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     8867 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_cube_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1605 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_intersect.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    11241 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_median_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2269 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_lu.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2186 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Glue_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    22986 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/ProxyCube.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    27217 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_min_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3856 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_rng_cxx98.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     7250 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_plus_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3963 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/unwrap_spmat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     7192 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/eop_core_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1691 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_max_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3733 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_trapz_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2002 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/cond_rel_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    35001 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Col_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     5112 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/typedef_elem.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    11657 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_join_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1248 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_polyval.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     6009 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_clamp_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     7737 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_inv.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1162 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_elem_helper_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2651 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpValProxy_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2352 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sqrtmat_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2790 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_hist_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1445 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtGlue_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1780 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_numel.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3005 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/running_stat_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    10234 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_relational_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3957 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_max_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4329 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_randu.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3860 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_SymEigsSolver_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1359 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Glue_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     5233 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_symmat_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     7223 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_norm.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3586 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_unique_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    12651 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mul_syrk.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2850 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_sprandn.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2410 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_orth_null.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2390 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtOp_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3915 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_elem1_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2706 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_repelem_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4355 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_randn.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    49167 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/sp_auxlib_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2162 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_conv.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1219 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_SparseGenMatProd_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1181 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_toeplitz_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2356 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_vectorise_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    13170 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_dot_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     8194 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_princomp_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3707 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/diagview_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    19380 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Base_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    26690 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Cube_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3452 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_trimat_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4450 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_princomp.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4103 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_htrans_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1869 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_any.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     9932 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_trimat_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4025 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_GenEigsSolver_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     8559 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/running_stat_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    34555 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/MapMat_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1225 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/GlueCube_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     8897 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_conv_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     7196 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_var_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1752 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_index_min_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     6739 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sp_minus_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2152 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_cor_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2047 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_princomp_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4648 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_repmat_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3374 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_diagvec_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     7179 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/gmm_diag_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1579 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_shift_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    15254 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_mixed_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     8408 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_minus_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2473 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/trimat_helper.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    10257 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/def_blas.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     9947 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/typedef_mat_fixed.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    20246 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/eop_aux.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2358 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_vectorise.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1363 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_cond.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3320 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_eigs_sym.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1364 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/wall_clock_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2925 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_nonzeros_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3858 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/eOpCube_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2027 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_trunc_log.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    10985 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_times.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2195 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_misc_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3747 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sp_plus_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     8852 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_vectorise_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2229 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_EigsSelect.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3291 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_n_unique.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1528 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_dotext_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    15656 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_max_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     6638 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/def_hdf5.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2524 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/eOp_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1697 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpGlue_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4487 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_sort.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    22436 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_cube_each_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4137 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_pinv_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1173 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_symmat_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1566 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/xvec_htrans_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1497 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_relational_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3638 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/gmm_misc_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3365 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_sqrtmat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3706 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cumprod_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    89635 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Proxy.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1783 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_rank.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4051 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cx_scalar_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    21581 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/diagview_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     5360 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_normalise_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2040 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_qr.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1138 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_repmat_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     5279 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_min.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4705 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_zeros.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1698 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_median.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     5912 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/arrayops_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     6557 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpValProxy_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1152 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_repelem_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     5455 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_normpdf.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1691 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_flip.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    20110 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_strans_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1287 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_shuffle_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2555 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_logmat_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2595 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_inplace_strans.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1868 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_qz.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     8822 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_interp1.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     8602 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_relational.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1860 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_find_unique_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    14914 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/promote_type.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1978 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_median_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1718 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_mvnrnd_bones.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1616 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_roots.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    31181 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/eop_core_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)    17293 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_solve_meat.hpp
+-rw-rw-r--   0 davide    (1000) davide    (1000)      516 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/NOTICE.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)    11358 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/LICENSE.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)    18591 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/README.md
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2245 2023-05-17 09:09:30.000000 ChannelAttribution-2.1.4/src/cypack/functions.h
+-rw-rw-r--   0 davide    (1000) davide    (1000)      180 2023-05-17 09:09:30.000000 ChannelAttribution-2.1.4/src/cypack/__init__.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1453 2023-05-17 09:09:30.000000 ChannelAttribution-2.1.4/src/cypack/generate_doc.py
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/ChannelAttribution.egg-info/
+-rw-rw-r--   0 davide    (1000) davide    (1000)        1 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/ChannelAttribution.egg-info/dependency_links.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)        1 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/ChannelAttribution.egg-info/not-zip-safe
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2308 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/ChannelAttribution.egg-info/PKG-INFO
+-rw-rw-r--   0 davide    (1000) davide    (1000)      498 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/ChannelAttribution.egg-info/SOURCES.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)       13 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/ChannelAttribution.egg-info/requires.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)       26 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/src/ChannelAttribution.egg-info/top_level.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)      545 2023-05-17 09:09:30.000000 ChannelAttribution-2.1.4/setup.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)      811 2023-05-17 09:09:30.000000 ChannelAttribution-2.1.4/README.md
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1574 2023-05-17 09:22:51.000000 ChannelAttribution-2.1.4/setup.cfg
```

### Comparing `ChannelAttribution-2.1.3/LICENSE.txt` & `ChannelAttribution-2.1.4/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ChannelAttribution: Markov model for online multi-channel attribution
-Copyright (C) 2015 - 2022  Davide Altomare and David Loris <https://channelattribution.io>
+Copyright (C) 2015 - 2023  Davide Altomare and David Loris <https://channelattribution.io>
 
 ChannelAttribution is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 ChannelAttribution is distributed in the hope that it will be useful,
```

### Comparing `ChannelAttribution-2.1.3/PKG-INFO` & `ChannelAttribution-2.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChannelAttribution
-Version: 2.1.3
+Version: 2.1.4
 Summary: Markov Model for Online Multi-Channel Attribution
 Home-page: https://channelattribution.io
 Author: Davide Altomare, David Loris
 Author-email: info@channelattribution.io
 License: GPLv3
 Project-URL: Documentation, https://channelattribution.io
 Project-URL: Code, https://gitlab.com/session-tech/ChannelAttribution
```

### Comparing `ChannelAttribution-2.1.3/src/cypack/ChannelAttribution.pyx` & `ChannelAttribution-2.1.4/src/cypack/ChannelAttribution.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ChannelAttribution: Markov model for online multi-channel attribution
-# Copyright (C) 2015 - 2022  Davide Altomare and David Loris <https://channelattribution.io>
+# Copyright (C) 2015 - 2023  Davide Altomare and David Loris <https://channelattribution.io>
 
 # ChannelAttribution is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # ChannelAttribution is distributed in the hope that it will be useful,
@@ -25,16 +25,16 @@
 import numpy as np
 import os
 import re
 import sys
 import matplotlib.pyplot as plt 
 import importlib
 
-__version="2.1.3"
-print("Looking for attribution at path level? Try markov_model_local_api() or ask for ChannelAttributionPro at info@channelattribution.io! Visit https://channelattribution.io for more information.")
+__version="2.1.4"
+print("*** Looking to run more advanced attribution? Try ChannelAttribution Pro for free! Visit https://channelattribution.io/product")
 print("Version: " + str(__version))
 
 cdef extern from "functions.h":
     pair[vector[string], list[vector[double]]] heuristic_models_cpp(vector[string]&, vector[unsigned long int]&, vector[double]&, string sep);
             
     list[vector[double]] choose_order_cpp(vector[string]& vy, vector[unsigned long int]& vc, vector[unsigned long int]& vn, unsigned long int max_order, string sep, unsigned long int ncore, unsigned long int roc_npt);
     
@@ -64,15 +64,15 @@
 **Markov Model for Online Multi-Channel Attribution**
 Advertisers use a variety of online marketing channels to reach consumers and they want to know the degree each channel contributes to their marketing success. This is called online multichannel attribution problem. In many cases, advertisers approach this problem through some simple heuristics methods that do not take into account any customer interactions and often tend to underestimate the importance of small channels in marketing contribution. This package provides a function that approaches the attribution problem in a probabilistic way. It uses a k-order Markov representation to identify structural correlations in the customer journey data. This would allow advertisers to give a more reliable assessment of the marketing contribution of each channel. The approach basically follows the one presented in Eva Anderl, Ingo Becker, Florian v. Wangenheim,
 Jan H. Schumann (2014). Differently from them, we solved the estimation process using stochastic simulations. In this way it is also possible to take into account conversion values and their variability in the computation of the channel importance. The package also contains a function that estimates three heuristic models (first-touch, last-touch and linear-touch approach) for the same problem.
 
 
 """
     
-def heuristic_models(Data,var_path,var_conv,var_value=None, sep=">"):
+def heuristic_models(Data,var_path,var_conv,var_value=None, sep=">", flg_adv=True):
 
     """
             
     Estimate three heuristic models (first-touch, last-touch and linear) from customer journey data.
     
     Parameters
     ----------
@@ -81,15 +81,17 @@
     var_path: string
         column of Data containing paths.
     var_conv : string
         column of Data containing total conversions for each path.
     var_value : string, optional, default None
         column of Data containing revenue for each path.
     sep : string, default ">"
-        separator between the channels.    
+        separator between the channels.
+    flg_adv : bool, default True
+        if True, ChannelAttribution Pro banner is printed.
     
     Returns
     -------
     DataFrame        
         (column) channel_name : channel names
         (column) first_touch_conversions : conversions attributed to each channel using first touch attribution.
         (column) first_touch_value : revenues attributed to each channel using first touch attribution.
@@ -152,19 +154,22 @@
     if len(vv)==0:
     
         res=pd.DataFrame({'channel_name':pd.Series(res0[0]).str.decode('utf-8'),'first_touch':res0[1][0],'last_touch':res0[1][1],'linear_touch':res0[1][2]})
     
     else:
     
         res=pd.DataFrame({'channel_name':pd.Series(res0[0]).str.decode('utf-8'),'first_touch_conversions':res0[1][0], 'first_touch_value':res0[1][3], 'last_touch_conversions':res0[1][1], 'last_touch_value':res0[1][4], 'linear_touch_conversions':res0[1][2], 'linear_touch_value':res0[1][5]})
+    
+    if flg_adv==True:
+        print("*** Looking to run more advanced attribution? Try ChannelAttribution Pro for free! Visit https://channelattribution.io/product")
 
     return(res)
 
     
-def choose_order(Data,var_path,var_conv,var_null,max_order=10,sep=">",ncore=1,roc_npt=100,plot=True):
+def choose_order(Data,var_path,var_conv,var_null,max_order=10,sep=">",ncore=1,roc_npt=100,plot=True, flg_adv=True):
 
     """
     
     Find the minimum Markov Model order that gives a good representation of customers’ behaviour for data considered. It requires paths that do not lead to conversion as input. Minimum order is found maximizing a penalized area under ROC curve.
     
     Parameters
     ----------
@@ -182,14 +187,16 @@
         separator between the channels.    
     ncore : int, default 1
         number of threads to be used in computation.        
     roc_npt: int, default 100
         number of points to be used for the approximation of roc curve.    
     plot: bool, default True
         if True, a plot with penalized auc with respect to order will be displayed.
+    flg_adv : bool, default True
+        if True, ChannelAttribution Pro banner is printed.
     
     Returns
     -------
     list        
         roc : list DataFrame one for each order considered
             (column) tpr: true positive rate
             (column) fpr: false positive rate
@@ -283,21 +290,23 @@
     order=order[order<=(best_order+1)]
     
     res_auc=pd.DataFrame({'order':order,'auc':auc,'pauc':pauc})
     
     res_roc=dict()
     for k in range(best_order+1):
         res_roc['order='+str(k+1)]=pd.DataFrame({'fpr':res0[2*k],'tpr':res0[2*k+1]})
-
+    
+    if flg_adv==True:
+        print("*** Looking to run more advanced attribution? Try ChannelAttribution Pro for free! Visit https://channelattribution.io/product")
     
     return(res_auc,res_roc,best_order)
             
     
         
-def markov_model(Data,var_path,var_conv,var_value=None,var_null=None,order=1,nsim_start=1e5,max_step=None,out_more=False,sep=">",ncore=1, nfold=10, seed=0, conv_par=0.05,rate_step_sim=1.5,verbose=True):
+def markov_model(Data,var_path,var_conv,var_value=None,var_null=None,order=1,nsim_start=1e5,max_step=None,out_more=False,sep=">",ncore=1, nfold=10, seed=0, conv_par=0.05,rate_step_sim=1.5,verbose=True, flg_adv=True):
 
     '''
     
     Estimate a k-order Markov model from customer journey data. Differently from markov_model, this function iterates estimation until a desidered convergence is reached and enables multiprocessing.
     
     Parameters
     ----------
@@ -329,14 +338,16 @@
         random seed. Giving this parameter the same value over different runs guarantees that results will not vary.    
     conv_par : double, default 0.05
         convergence parameter for the algorithm. The estimation process ends when the percentage of variation of the results over different repetions is less than convergence parameter.    
     rate_step_sim : double, default 0
         number of simulations used at each iteration is equal to the number of simulations used at previous iteration multiplied by rate_step_sim.    
     verbose : bool, default True
         if True, additional information about process convergence will be shown.    
+    flg_adv : bool, default True
+        if True, ChannelAttribution Pro banner is printed.
             
     Returns
     -------
     list of DataFrames
         result: Dataframe
             (column) channel_name : channel names
             (column) total_conversions : conversions attributed to each channel
@@ -491,19 +502,21 @@
         res=dict()
         
         res['result']=pd.DataFrame({'channel_name':pd.Series(res0[0][2]).str.decode('utf-8'),'total_conversions':res0[1][0],'total_conversion_value':res0[1][3]})
         res['transition_matrix']=pd.DataFrame({'channel_from':pd.Series(res0[0][0]).str.decode('utf-8'),'channel_to':pd.Series(res0[0][1]).str.decode('utf-8'),'transition_probability':res0[1][2]})
     
         res['removal_effects']=pd.DataFrame({'channel_name':pd.Series(res0[0][2]).str.decode('utf-8'),'removal_effects_conversion':res0[1][1],'removal_effects_conversion_value':res0[1][4]})        
     
+    if flg_adv==True:
+        print("*** Looking to run more advanced attribution? Try ChannelAttribution Pro for free! Visit https://channelattribution.io/product")
     
     return(res)
     
 
-def transition_matrix(Data,var_path,var_conv,var_null,order=1,sep=">",flg_equal=True):
+def transition_matrix(Data,var_path,var_conv,var_null,order=1,sep=">",flg_equal=True, flg_adv=True):
 
     '''
 
     Estimate a k-order transition matrix from customer journey data.
     
     Parameters
     ----------
@@ -517,14 +530,16 @@
         column of Data containing total paths that do not lead to conversion.
     order : int, default 1
         Markov model order.        
     sep : string, default ">"
         separator between the channels.    
     flg_equal: bool, default True
         if True, transitions from a channel to itself will be considered.    
+    flg_adv : bool, default True
+        if True, ChannelAttribution Pro banner is printed.
                     
     Returns
     -------
     list of DataFrames
         channels: Dataframe
             (column) id_channel : channel ids
             (column) channel_name : channel names
@@ -543,15 +558,14 @@
     >>> Data = pd.read_csv('https://channelattribution.io/csv/Data.csv',sep=";")
 
     Estimate a second-order transition matrix using total conversions and paths that do not lead to conversion 
     
     >>> transition_matrix(Data, "path", "total_conversions", var_null="total_null", order=2)
                     
     '''
-    
      
     if ("DataFrame" not in str(type(Data))):
         raise NameError("Data must be a DataFrame")
     
     if type(var_path)==str:
         if var_path not in Data.columns:
             raise NameError("var_path must be a column of Data")
@@ -583,20 +597,23 @@
         raise NameError("flg_equal must be False or True")
                     
     res0=__transition_matrix_1(vy=Data[var_path].str.encode('utf-8'),vc=Data[var_conv],vn=Data[var_null],order=order,sep=sep.encode("utf-8"), flg_equal=int(flg_equal))
     
     res=dict()
     res['channels']=pd.DataFrame({'id_channel':range(1,len(res0[0][2])+1), 'channel_name':pd.Series(res0[0][2]).str.decode('utf-8')})
     res['transition_matrix']=pd.DataFrame({'channel_from':pd.Series(res0[0][0]).str.decode('utf-8'),'channel_to':pd.Series(res0[0][1]).str.decode('utf-8'),'transition_probability':res0[1]})
+    
+    if flg_adv==True:
+        print("*** Looking to run more advanced attribution? Try ChannelAttribution Pro for free! Visit https://channelattribution.io/product")
 
     return(res)
     
     
     
-def auto_markov_model(Data, var_path, var_conv, var_null, var_value=None, max_order=10, roc_npt=100, plot=False, nsim_start=1e5, max_step=None, out_more=False, sep=">", ncore=1, nfold=10, seed=0, conv_par=0.05, rate_step_sim=1.5, verbose=True):
+def auto_markov_model(Data, var_path, var_conv, var_null, var_value=None, max_order=10, roc_npt=100, plot=False, nsim_start=1e5, max_step=None, out_more=False, sep=">", ncore=1, nfold=10, seed=0, conv_par=0.05, rate_step_sim=1.5, verbose=True, flg_adv=True):
 
     '''
     
     Parameters
     ----------
     Data : DataFrame
         customer journeys.
@@ -630,14 +647,16 @@
         random seed. Giving this parameter the same value over different runs guarantees that results will not vary.    
     conv_par : double, default 0.05
         convergence parameter for the algorithm. The estimation process ends when the percentage of variation of the results over different repetions is less than convergence parameter.    
     rate_step_sim : double, default 0
         number of simulations used at each iteration is equal to the number of simulations used at previous iteration multiplied by rate_step_sim.    
     verbose : bool, default True
         if True, additional information about process convergence will be shown.    
+    flg_adv : bool, default True
+        if True, ChannelAttribution Pro banner is printed.
             
     Returns
     -------
     list of DataFrames
         result: Dataframe
             (column) channel_name : channel names
             (column) total_conversions : conversions attributed to each channel
@@ -743,676 +762,681 @@
         raise NameError("verbose must be False or True")
     
     if (var_value==None):
         vv = pd.Series(None,dtype='float64')
     else:
         vv=Data[var_value]
             
-    [res_auc,res_roc,best_order] = choose_order(Data, var_path, var_conv, var_null, max_order = max_order, sep = sep, ncore = ncore, roc_npt = roc_npt, plot = plot)
+    [res_auc,res_roc,best_order] = choose_order(Data, var_path, var_conv, var_null, max_order = max_order, sep = sep, ncore = ncore, roc_npt = roc_npt, plot = plot, flg_adv=False)
     
-    res = markov_model(Data, var_path, var_conv, var_value = var_value, var_null = var_null, order = best_order, nsim_start = nsim_start, max_step = max_step, out_more = out_more, sep = sep, ncore = ncore, nfold = nfold, seed = seed, conv_par = conv_par, rate_step_sim = rate_step_sim, verbose = verbose)
+    res = markov_model(Data, var_path, var_conv, var_value = var_value, var_null = var_null, order = best_order, nsim_start = nsim_start, max_step = max_step, out_more = out_more, sep = sep, ncore = ncore, nfold = nfold, seed = seed, conv_par = conv_par, rate_step_sim = rate_step_sim, verbose = verbose, flg_adv=False)
+    
+    if flg_adv==True:
+        print("*** Looking to run more advanced attribution? Try ChannelAttribution Pro for free! Visit https://channelattribution.io/product")
     
     return(res)
     
 
 #######################################################################################################################################################################
 #APIS
 #######################################################################################################################################################################
 
+if 0!=0:
 
-def __import_libs_for_api():
-    global pysftp
-    global tarfile
-    global uuid
-    global time
-    global shutil
-    global Fernet
-    global json
-    global requests
-    global socket
-    import pysftp
-    import tarfile
-    import uuid
-    import time
-    import shutil
-    from cryptography.fernet import Fernet
-    import json
-    import requests
-    import socket
-    
-def __check_libs_for_api():
-    res=1
-    libs=['pysftp','tarfile','uuid','time','urllib','shutil','cryptography','json','requests']
-    no_libs=[]
-    for lib0 in libs:
-        ck=importlib.util.find_spec(lib0)
-        if ck==None:
-            no_libs= no_libs+[lib0]
-    if len(no_libs)>0:
-        print("There are some missing libraries you need for using our apis. Install them with:")
-        print("pip install " + " ".join(no_libs))
-        res=0
-    return(res)
-
-def __f_list_files(sftp):
-    directory_structure = sftp.listdir_attr()
-    vattr=[]
-    for attr in directory_structure:
-        vattr=vattr+[attr.filename]
-        #print(attr.filename, attr)
-    return(vattr)
-
-def __f_save_to_crypted(data,filename,key,cipher_suite):
-    data=data.to_json(orient="records")
-    data=str.encode(data)
-    
-    cipher_text = cipher_suite.encrypt(data)
-    
-    f = open(filename, "wb")
-    f.write(cipher_text)
-    f.close()
-    
-    tar = tarfile.open(filename+".tar.gz", "w:gz")
-    tar.add(filename, arcname=filename)
-    tar.close()
+    def __import_libs_for_api():
+        global pysftp
+        global tarfile
+        global uuid
+        global time
+        global shutil
+        global Fernet
+        global json
+        global requests
+        global socket
+        import pysftp
+        import tarfile
+        import uuid
+        import time
+        import shutil
+        from cryptography.fernet import Fernet
+        import json
+        import requests
+        import socket
+        
+    def __check_libs_for_api():
+        res=1
+        libs=['pysftp','tarfile','uuid','time','urllib','shutil','cryptography','json','requests']
+        no_libs=[]
+        for lib0 in libs:
+            ck=importlib.util.find_spec(lib0)
+            if ck==None:
+                no_libs= no_libs+[lib0]
+        if len(no_libs)>0:
+            print("There are some missing libraries you need for using our apis. Install them with:")
+            print("pip install " + " ".join(no_libs))
+            res=0
+        return(res)
+    
+    def __f_list_files(sftp):
+        directory_structure = sftp.listdir_attr()
+        vattr=[]
+        for attr in directory_structure:
+            vattr=vattr+[attr.filename]
+            #print(attr.filename, attr)
+        return(vattr)
     
-    return(0)
- 
-def __f_save_to_crypted_list(list_Data,filename,key,cipher_suite):
-    tar = tarfile.open(filename+".tar.gz", "w:gz")
-    for filename0 in list_Data.keys():
-        
-        data=list_Data[filename0]
-        
+    def __f_save_to_crypted(data,filename,key,cipher_suite):
         data=data.to_json(orient="records")
         data=str.encode(data)
-
+        
         cipher_text = cipher_suite.encrypt(data)
-
-        f = open(filename0, "wb")
+        
+        f = open(filename, "wb")
         f.write(cipher_text)
         f.close()
-
-        tar.add(filename0, arcname=filename0)
-        os.remove(filename0)
-    tar.close()
-
-    return(0)
-
-def __f_put_file(filename0,sftp,ntry=12):
-    z=0
-    flg_ok=0
-    list_files=[]
-    while (filename0 not in list_files) and (z<ntry):
-        sftp.put(filename0, filename0)
-        list_files=__f_list_files(sftp)
-        if filename0 in list_files:
-            flg_ok=1
-            break
+        
+        tar = tarfile.open(filename+".tar.gz", "w:gz")
+        tar.add(filename, arcname=filename)
+        tar.close()
+        
+        return(0)
+    
+    def __f_save_to_crypted_list(list_Data,filename,key,cipher_suite):
+        tar = tarfile.open(filename+".tar.gz", "w:gz")
+        for filename0 in list_Data.keys():
+            
+            data=list_Data[filename0]
+            
+            data=data.to_json(orient="records")
+            data=str.encode(data)
+    
+            cipher_text = cipher_suite.encrypt(data)
+    
+            f = open(filename0, "wb")
+            f.write(cipher_text)
+            f.close()
+    
+            tar.add(filename0, arcname=filename0)
+            os.remove(filename0)
+        tar.close()
+    
+        return(0)
+    
+    def __f_put_file(filename0,sftp,ntry=12):
+        z=0
+        flg_ok=0
+        list_files=[]
+        while (filename0 not in list_files) and (z<ntry):
+            sftp.put(filename0, filename0)
+            list_files=__f_list_files(sftp)
+            if filename0 in list_files:
+                flg_ok=1
+                break
+            else:
+                time.sleep(5)
+            z=z+1
+        if flg_ok==1:
+            print("Your data has been encrypted and sent to our server for the execution.")
         else:
-            time.sleep(5)
-        z=z+1
-    if flg_ok==1:
-        print("Your data has been encrypted and sent to our server for the execution.")
-    else:
-        ValueError("put_file: timeout reached.")
+            ValueError("put_file: timeout reached.")
+        
+        return(0)
     
-    return(0)
-
-def __f_get_file(filename0,sftp,ntry=12):
-    z=0
-    flg_ok=0
-    ck_file=False
-    while (ck_file==False) and (z<ntry):
-        sftp.get(filename0, filename0)
-        ck_file=os.path.exists(filename0)
-        if ck_file:
-            flg_ok=1
-            break
+    def __f_get_file(filename0,sftp,ntry=12):
+        z=0
+        flg_ok=0
+        ck_file=False
+        while (ck_file==False) and (z<ntry):
+            sftp.get(filename0, filename0)
+            ck_file=os.path.exists(filename0)
+            if ck_file:
+                flg_ok=1
+                break
+            else:
+                time.sleep(5)
+            z=z+1
+        if flg_ok==1:
+            print("Your output has been retrieved from our server.")
         else:
-            time.sleep(5)
-        z=z+1
-    if flg_ok==1:
-        print("Your output has been retrieved from our server.")
-    else:
-        ValueError("get_file: timeout reached.")
-    
-    return(0)
-
-def __f_initialize_connection(server,token):
-    
-    filename = str(uuid.uuid4())
-    os.mkdir(filename)
-    os.chdir(filename)
-    
-    url='https://{0}/api/api.php?type=pw&filename={1}&token={2}'.format(server,filename,token)
-    #print(url)
-    info = requests.get(url)
-    info=info.text.split("\n")
-    Username=info[0]
-    Password=info[1][0:-1]
-
-    sftp=pysftp.Connection(host=socket.gethostbyname(server) , username=Username, password=Password)
-    sftp.cwd('/{0}'.format(Username))
-    
-    return([filename,sftp])
-
-def __f_send_to_server(Data,is_list,filename,server,sftp):
-    
-    url='https://{0}/api/max_size.php'.format(server)
-    resp=requests.get(url)
-    msb=int(resp.text)
-    
-    #filename = str(uuid.uuid4())
-    key = Fernet.generate_key()
-    cipher_suite = Fernet(key)
-
-    print("Encrypting your data...")
-
-    if is_list==False:
-        __f_save_to_crypted(Data,filename,key,cipher_suite)
-        os.remove(filename)
-    else:
-        __f_save_to_crypted_list(Data,filename,key,cipher_suite)
+            ValueError("get_file: timeout reached.")
         
-    if os.path.getsize(filename+".tar.gz")<(msb*1e6):
-        print("Sending your encrypted data to our server...")
-        print("filename: " + filename)
-        print("key: " + key.decode("utf-8"))
-    
-        __f_put_file(filename+".tar.gz",sftp,ntry=12)
-        os.remove(filename+".tar.gz")
-        return([key,cipher_suite])
-    else:
-        print("Your filesize exceed "+ str(msb) +" Mb which is the maximum size allowed")
-        os.remove(filename+".tar.gz")
-        return([-1,-1])
-
-def __f_retrieve_from_server(filename,sftp):
+        return(0)
     
-    print("Retrieving output...")
-    
-    __f_get_file(filename+"-O.tar.gz",sftp,ntry=100)
-    sftp.remove(filename+"-O.tar.gz")
-
-    tar = tarfile.open(filename+"-O.tar.gz", "r:gz")
-    tar.extractall()
-    tar.close()
-    os.remove(filename+"-O.tar.gz")
+    def __f_initialize_connection(server,token):
+        
+        filename = str(uuid.uuid4())
+        os.mkdir(filename)
+        os.chdir(filename)
+        
+        url='https://{0}/api/api.php?type=pw&filename={1}&token={2}'.format(server,filename,token)
+        #print(url)
+        info = requests.get(url)
+        info=info.text.split("\n")
+        Username=info[0]
+        Password=info[1][0:-1]
     
-    return(0)
-
-def generate_token(email,job,company):
-
-    '''
+        sftp=pysftp.Connection(host=socket.gethostbyname(server) , username=Username, password=Password)
+        sftp.cwd('/{0}'.format(Username))
+        
+        return([filename,sftp])
     
-    You can use this function to generate a token that enables the use of our apis for making path-level attribution. An email containing your personal token will be sent to the email address indicated. 
+    def __f_send_to_server(Data,is_list,filename,server,sftp):
+        
+        url='https://{0}/api/max_size.php'.format(server)
+        resp=requests.get(url)
+        msb=int(resp.text)
+        
+        #filename = str(uuid.uuid4())
+        key = Fernet.generate_key()
+        cipher_suite = Fernet(key)
     
-    Parameters
-    ----------
-    email : string
-        a string with your business/university email at which we will send your personal token
-    job : string
-        a string describing your job
-    company: string
-        a string containing the name of your company/university
-                        
+        print("Encrypting your data...")
     
-    Examples
-    --------
+        if is_list==False:
+            __f_save_to_crypted(Data,filename,key,cipher_suite)
+            os.remove(filename)
+        else:
+            __f_save_to_crypted_list(Data,filename,key,cipher_suite)
+            
+        if os.path.getsize(filename+".tar.gz")<(msb*1e6):
+            print("Sending your encrypted data to our server...")
+            print("filename: " + filename)
+            print("key: " + key.decode("utf-8"))
+        
+            __f_put_file(filename+".tar.gz",sftp,ntry=12)
+            os.remove(filename+".tar.gz")
+            return([key,cipher_suite])
+        else:
+            print("Your filesize exceed "+ str(msb) +" Mb which is the maximum size allowed")
+            os.remove(filename+".tar.gz")
+            return([-1,-1])
     
-    generate_token("mario.rossi@data.com","data scientist","data.com")
+    def __f_retrieve_from_server(filename,sftp):
+        
+        print("Retrieving output...")
+        
+        __f_get_file(filename+"-O.tar.gz",sftp,ntry=100)
+        sftp.remove(filename+"-O.tar.gz")
     
-    '''
+        tar = tarfile.open(filename+"-O.tar.gz", "r:gz")
+        tar.extractall()
+        tar.close()
+        os.remove(filename+"-O.tar.gz")
+        
+        return(0)
     
-    server = "api.channelattribution.net"
+    def generate_token(email,job,company):
     
-    try:
-        ck_libs=__check_libs_for_api()
+        '''
+        
+        You can use this function to generate a token that enables the use of our apis for making path-level attribution. An email containing your personal token will be sent to the email address indicated. 
+        
+        Parameters
+        ----------
+        email : string
+            a string with your business/university email at which we will send your personal token
+        job : string
+            a string describing your job
+        company: string
+            a string containing the name of your company/university
+                            
         
-        if ck_libs==1:
+        Examples
+        --------
         
-            __import_libs_for_api()
+        generate_token("mario.rossi@data.com","data scientist","data.com")
         
-            if email==None:
-                raise NameError("email must be specified")
+        '''
+        
+        server = "api.channelattribution.net"
+        
+        try:
+            ck_libs=__check_libs_for_api()
             
-            if job==None:
-                raise NameError("job must be specified")
-                
-            if company==None:
-                raise NameError("company must be specified")
+            if ck_libs==1:
             
-            regex = r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b'
+                __import_libs_for_api()
             
-            def check(email):
-                if(re.fullmatch(regex, email)):
-                    return(1)
+                if email==None:
+                    raise NameError("email must be specified")
+                
+                if job==None:
+                    raise NameError("job must be specified")
                     
-                else:
-                    return(0)
-            
-            if check(email)==0:
-                print("Insert a valid email address")
-                return(-1)
-            else:
-                job=re.sub("[^0-9a-zA-Z]+", "_", job)
-                company=re.sub("[^0-9a-zA-Z]+", "_", company)
+                if company==None:
+                    raise NameError("company must be specified")
                 
-            token = str(uuid.uuid4())
+                regex = r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b'
                 
-            url="https://{0}/api/token_registration.php?mail={1}&job={2}&company={3}&token={4}".format(server,email,job,company,token)
-            resp=requests.get(url)
-            resp=resp.text
+                def check(email):
+                    if(re.fullmatch(regex, email)):
+                        return(1)
+                        
+                    else:
+                        return(0)
+                
+                if check(email)==0:
+                    print("Insert a valid email address")
+                    return(-1)
+                else:
+                    job=re.sub("[^0-9a-zA-Z]+", "_", job)
+                    company=re.sub("[^0-9a-zA-Z]+", "_", company)
+                    
+                token = str(uuid.uuid4())
+                    
+                url="https://{0}/api/token_registration.php?mail={1}&job={2}&company={3}&token={4}".format(server,email,job,company,token)
+                resp=requests.get(url)
+                resp=resp.text
+                
+                if resp[0]=='1':
+                    print("Your token has been sent to your email address.")
+                    return(0)
+                else:
+                    print("Token generation failed. Try again.")
+                    return(-1)
             
-            if resp[0]=='1':
-                print("Your token has been sent to your email address.")
-                return(0)
-            else:
-                print("Token generation failed. Try again.")
-                return(-1)
+        else:    
+            print("Your token has not been created. Try again or write to info@channelattribution.io")
+            return(-1)
         
-    else:    
-        print("Your token has not been created. Try again or write to info@channelattribution.io")
-        return(-1)
-    
-
-def markov_model_local_api(token, Data,var_path, var_conv,var_value=None, var_null=None, order=1, sep=">", ncore=1, conv_par_glob=0.05,
-conv_par_loc=0.01,verbose=True):
-
-    '''
-    Through this function, you can make path-level attribution using Markov model. It requires a token that can be generated using the function "generate_token". Your Data will be encrypted and sent to our server for being elaborated and the output will be returned. We will not share your Data or store it, it will be canceled at the end of the elaboration. If you prefer to make path attribution locally, you can write us at info@channelattribution.net.
-    
-    Parameters
-    ----------
-    token : string
-        your personal token generated with function "generate_token"
-    Data : DataFrame
-        customer journeys.
-    var_path: string
-        column of Data containing paths.
-    var_conv : string
-        column of Data containing total conversions for each path.
-    var_value : string, default None
-        column of Data containing revenue for each path
-    var_null : string, default None
-        column of Data containing total paths that do not lead to conversion.
-    order : int, default 1
-        Markov Model order to be considered.
-    sep : string, default ">"
-        separator between the channels.
-    ncore : int, default 1
-        number of threads to be used in computation.
-    conv_par_glob : float, default 0.05
-        convergence parameter for the global attribution. The estimation process ends when the percentage of variation of the results over dierent repetitions is less than conv_par_loc (this is equal to conv_par parameter of function "markov_model")
-    conv_par_loc : float, default 0.05
-        convergence parameter for the local attribution. The estimation process ends when the percentage difference between global and aggregated local attribution is less than conv_par_loc
-    verbose : bool, default True
-        if True, additional information about process convergence will be shown.
-            
-    Returns
-    -------
-    list
-        path_attribution: Dataframe
-            (column) path : path.
-            (column) idpath : path identification number.
-            (column) channel : channel name.
-            (column) weight_total_conversion : percentage of conversions associated to channel for the path considered.
-            (column) weight_total_conversion_value : percentage of conversion value associated to channel for the path considered.
-        removal_effects: Dataframe
-            (column) channel_name : channel name.
-            (column) removal_effects_conversion : removal effects for conversion attribution from global attribution.
-            (column) removal_effects_value : removal effects for value attribution from global attribution.
-        corrective_factors: list
-            total conversions: Dataframe
-                (column) channel : channel name
-                (column) perc_corr_j : correction percentage at iteration j from the iterative matching process between global and local attribution.
-            total conversion_value: Dataframe
-                (column) channel : channel name
-                (column) perc_corr_j : correction percentage at iteration j from the iterative matching process between global and local attribution.
-                        
-    Examples
-    --------
-    
-    Load Data
-    
-    >>> import pandas as pd    
-    >>> from ChannelAttribution import *
-    >>> Data = pd.read_csv('https://channelattribution.io/csv/Data.csv',sep=";")
-    
-    Path level attribution 
     
-    >>> res=markov_model_local_api(token, Data,var_path="path", var_conv="total_conversions", \\ 
-    >>> var_value="total_conversion_value", var_null="total_null", order=1, sep=">")
-    
-    '''
+    def markov_model_local_api(token, Data,var_path, var_conv,var_value=None, var_null=None, order=1, sep=">", ncore=1, conv_par_glob=0.05,
+    conv_par_loc=0.01,verbose=True):
     
-    server = "api.channelattribution.net"
-    
-    try:
-        ck_libs=__check_libs_for_api()
+        '''
+        Through this function, you can make path-level attribution using Markov model. It requires a token that can be generated using the function "generate_token". Your Data will be encrypted and sent to our server for being elaborated and the output will be returned. We will not share your Data or store it, it will be canceled at the end of the elaboration. If you prefer to make path attribution locally, you can write us at info@channelattribution.net.
         
-        if ck_libs==1:
+        Parameters
+        ----------
+        token : string
+            your personal token generated with function "generate_token"
+        Data : DataFrame
+            customer journeys.
+        var_path: string
+            column of Data containing paths.
+        var_conv : string
+            column of Data containing total conversions for each path.
+        var_value : string, default None
+            column of Data containing revenue for each path
+        var_null : string, default None
+            column of Data containing total paths that do not lead to conversion.
+        order : int, default 1
+            Markov Model order to be considered.
+        sep : string, default ">"
+            separator between the channels.
+        ncore : int, default 1
+            number of threads to be used in computation.
+        conv_par_glob : float, default 0.05
+            convergence parameter for the global attribution. The estimation process ends when the percentage of variation of the results over dierent repetitions is less than conv_par_loc (this is equal to conv_par parameter of function "markov_model")
+        conv_par_loc : float, default 0.05
+            convergence parameter for the local attribution. The estimation process ends when the percentage difference between global and aggregated local attribution is less than conv_par_loc
+        verbose : bool, default True
+            if True, additional information about process convergence will be shown.
+                
+        Returns
+        -------
+        list
+            path_attribution: Dataframe
+                (column) path : path.
+                (column) idpath : path identification number.
+                (column) channel : channel name.
+                (column) weight_total_conversion : percentage of conversions associated to channel for the path considered.
+                (column) weight_total_conversion_value : percentage of conversion value associated to channel for the path considered.
+            removal_effects: Dataframe
+                (column) channel_name : channel name.
+                (column) removal_effects_conversion : removal effects for conversion attribution from global attribution.
+                (column) removal_effects_value : removal effects for value attribution from global attribution.
+            corrective_factors: list
+                total conversions: Dataframe
+                    (column) channel : channel name
+                    (column) perc_corr_j : correction percentage at iteration j from the iterative matching process between global and local attribution.
+                total conversion_value: Dataframe
+                    (column) channel : channel name
+                    (column) perc_corr_j : correction percentage at iteration j from the iterative matching process between global and local attribution.
+                            
+        Examples
+        --------
+        
+        Load Data
+        
+        >>> import pandas as pd    
+        >>> from ChannelAttribution import *
+        >>> Data = pd.read_csv('https://channelattribution.io/csv/Data.csv',sep=";")
+        
+        Path level attribution 
+        
+        >>> res=markov_model_local_api(token, Data,var_path="path", var_conv="total_conversions", \\ 
+        >>> var_value="total_conversion_value", var_null="total_null", order=1, sep=">")
+        
+        '''
         
-            __import_libs_for_api()
-            
-            if "NoneType" in str(type(token)):
-                raise NameError("token must be specified. Use function generate_token(email,job,company)")
-            else:
-                if "str" not in str(type(token)):
-                    print("token must be a string")
+        server = "api.channelattribution.net"
+        
+        try:
+            ck_libs=__check_libs_for_api()
             
-            if "NoneType" in str(type(Data)):
-                raise NameError("Data must be specified")
-            else:
-                if "DataFrame" not in str(type(Data)):
-                     raise NameError("Data must be a DataFrame")
-                    
-            if "NoneType" in str(type(var_path)):
-                raise NameError("var_path must be specified")
-            else:
-                if "str" not in str(type(var_path)):
-                    print("var_path must be a string")
-                else:
-                    var_path_old=var_path
-                    var_path=re.sub(r"\s+", '_', var_path)
-                    Data.rename(columns={var_path_old: var_path},inplace=True)
+            if ck_libs==1:
             
-            if "NoneType" in str(type(var_conv)):
-                raise NameError("var_conv must be specified")
-            else:
-                if "str" not in str(type(var_conv)):
-                    print("var_conv must be a string")
+                __import_libs_for_api()
+                
+                if "NoneType" in str(type(token)):
+                    raise NameError("token must be specified. Use function generate_token(email,job,company)")
                 else:
-                    var_conv_old=var_conv
-                    var_conv=re.sub(r"\s+", '_', var_conv)
-                    Data.rename(columns={var_conv_old: var_conv},inplace=True)
-            
-            if "NoneType" not in str(type(var_value)):
-                var_value=re.sub(r"\s+", '_', var_value)
-            else:
-                if "str" not in str(type(var_value)):
-                    print("var_value must be a string")
+                    if "str" not in str(type(token)):
+                        print("token must be a string")
+                
+                if "NoneType" in str(type(Data)):
+                    raise NameError("Data must be specified")
                 else:
-                    var_value_old=var_value
-                    var_value=re.sub(r"\s+", '_', var_value)
-                    Data.rename(columns={var_value_old: var_value},inplace=True)
-                    
-            if "NoneType" not in str(type(var_null)):
-                var_null=re.sub(r"\s+", '_', var_null)
-            else:
-                if "str" not in type(var_null):
-                    print("var_null must be a string")
+                    if "DataFrame" not in str(type(Data)):
+                         raise NameError("Data must be a DataFrame")
+                        
+                if "NoneType" in str(type(var_path)):
+                    raise NameError("var_path must be specified")
                 else:
-                    var_null_old=var_null
-                    var_null=re.sub(r"\s+", '_', var_null)
-                    Data.rename(columns={var_null_old: var_null},inplace=True)
+                    if "str" not in str(type(var_path)):
+                        print("var_path must be a string")
+                    else:
+                        var_path_old=var_path
+                        var_path=re.sub(r"\s+", '_', var_path)
+                        Data.rename(columns={var_path_old: var_path},inplace=True)
                 
-            if "NoneType" not in str(type(order)):
-                if "int" not in str(type(order)):
-                    print("order must be a int")
+                if "NoneType" in str(type(var_conv)):
+                    raise NameError("var_conv must be specified")
                 else:
-                    if order<1:
-                        print("order must be > 0")
-            else:
-                print("order must be specified")
+                    if "str" not in str(type(var_conv)):
+                        print("var_conv must be a string")
+                    else:
+                        var_conv_old=var_conv
+                        var_conv=re.sub(r"\s+", '_', var_conv)
+                        Data.rename(columns={var_conv_old: var_conv},inplace=True)
                 
-            if "NoneType" not in str(type(sep)):
-                if "str" not in str(type(sep)):
-                    print("sep must be a string")
-            else:
-                print("sep must be specified")
-                
-            if "NoneType" not in str(type(conv_par_glob)):
-                if "float" not in str(type(conv_par_glob)):
-                    print("conv_par_glob must be a float")
+                if "NoneType" not in str(type(var_value)):
+                    var_value=re.sub(r"\s+", '_', var_value)
                 else:
-                    if conv_par_glob<=0:
-                        print("conv_par_glob must be > 0")
+                    if "str" not in str(type(var_value)):
+                        print("var_value must be a string")
+                    else:
+                        var_value_old=var_value
+                        var_value=re.sub(r"\s+", '_', var_value)
+                        Data.rename(columns={var_value_old: var_value},inplace=True)
                         
-            if "NoneType" not in str(type(conv_par_loc)):
-                if "float" not in str(type(conv_par_loc)):
-                    print("conv_par_loc must be a float")
+                if "NoneType" not in str(type(var_null)):
+                    var_null=re.sub(r"\s+", '_', var_null)
                 else:
-                    if conv_par_loc<=0:
-                        print("conv_par_loc must be > 0")
-                        
-            if "NoneType" not in str(type(verbose)):
-                if "bool" not in str(type(verbose)):
-                    print("verbose must be True or False")
+                    if "str" not in type(var_null):
+                        print("var_null must be a string")
+                    else:
+                        var_null_old=var_null
+                        var_null=re.sub(r"\s+", '_', var_null)
+                        Data.rename(columns={var_null_old: var_null},inplace=True)
+                    
+                if "NoneType" not in str(type(order)):
+                    if "int" not in str(type(order)):
+                        print("order must be a int")
+                    else:
+                        if order<1:
+                            print("order must be > 0")
+                else:
+                    print("order must be specified")
                     
-            
-            path0=os.getcwd()
-            
-            #initialize connection
-            
-            [filename,sftp]=__f_initialize_connection(server,token)
-            
-            #send input to server
-            
-            [key,cipher_suite]=__f_send_to_server(Data,False,filename,server,sftp)
-            
-            if key!=-1:
-                #elaborate on server
+                if "NoneType" not in str(type(sep)):
+                    if "str" not in str(type(sep)):
+                        print("sep must be a string")
+                else:
+                    print("sep must be specified")
+                    
+                if "NoneType" not in str(type(conv_par_glob)):
+                    if "float" not in str(type(conv_par_glob)):
+                        print("conv_par_glob must be a float")
+                    else:
+                        if conv_par_glob<=0:
+                            print("conv_par_glob must be > 0")
+                            
+                if "NoneType" not in str(type(conv_par_loc)):
+                    if "float" not in str(type(conv_par_loc)):
+                        print("conv_par_loc must be a float")
+                    else:
+                        if conv_par_loc<=0:
+                            print("conv_par_loc must be > 0")
+                            
+                if "NoneType" not in str(type(verbose)):
+                    if "bool" not in str(type(verbose)):
+                        print("verbose must be True or False")
+                        
                 
-                print("Asking to our server to start the elaboration...")
-                url='https://{0}/api/api.php?type=markov-model-local&filename={1}&key={2}&var_path={3}&var_conv={4}&var_value={5}&var_null={6}&order={7}&sep={8}&ncore={9}&conv_par_glob={10}&conv_par_loc={11}&verbose={12}&token={13}'.format(server,filename,key.decode("utf-8"),var_path,var_conv,var_value,var_null,order,sep,ncore,conv_par_glob,conv_par_loc,verbose,token)
-                #print(url)
-                resp=requests.get(url)
-                resp=resp.text
-                print(resp)
+                path0=os.getcwd()
                 
-                if "token_ko" not in resp:
-                    ''''
-                      cipher_suite = Fernet(str.encode(key))
-                    '''
-                    #retrieving output
-                    
-                    __f_retrieve_from_server(filename,sftp)
-                    
-                    print("Composing output...")
-                    
-                    res=dict()
-                    for elem in ['path_attribution','removal_effects','corrective_factors']:
-                        cipher_text = open(elem, 'r').read()
-                        plain_text = cipher_suite.decrypt(str.encode(cipher_text),)
-                        res[elem]=pd.read_json(plain_text,orient='records')
-                        
-                    tmp=res['corrective_factors'].copy()
-                    tmp1=tmp[tmp.type=='total_conversions']
-                    del tmp1['type']
-                    tmp2=tmp[tmp.type=='total_conversion_value']
-                    del tmp2['type']
-                    
-                    res['corrective_factors']=dict()
-                    res['corrective_factors']['total_conversions']=tmp1 
-                    res['corrective_factors']['total_conversion_value']=tmp2 
-                    
-                    shutil.rmtree(path0+'/'+filename)
-                    os.chdir(path0)
+                #initialize connection
+                
+                [filename,sftp]=__f_initialize_connection(server,token)
+                
+                #send input to server
+                
+                [key,cipher_suite]=__f_send_to_server(Data,False,filename,server,sftp)
+                
+                if key!=-1:
+                    #elaborate on server
                     
-                    print("Your data has been cancelled from our server")
-                    print("Elaboration finished!")
+                    print("Asking to our server to start the elaboration...")
+                    url='https://{0}/api/api.php?type=markov-model-local&filename={1}&key={2}&var_path={3}&var_conv={4}&var_value={5}&var_null={6}&order={7}&sep={8}&ncore={9}&conv_par_glob={10}&conv_par_loc={11}&verbose={12}&token={13}'.format(server,filename,key.decode("utf-8"),var_path,var_conv,var_value,var_null,order,sep,ncore,conv_par_glob,conv_par_loc,verbose,token)
+                    #print(url)
+                    resp=requests.get(url)
+                    resp=resp.text
+                    print(resp)
+                    
+                    if "token_ko" not in resp:
+                        ''''
+                          cipher_suite = Fernet(str.encode(key))
+                        '''
+                        #retrieving output
+                        
+                        __f_retrieve_from_server(filename,sftp)
+                        
+                        print("Composing output...")
+                        
+                        res=dict()
+                        for elem in ['path_attribution','removal_effects','corrective_factors']:
+                            cipher_text = open(elem, 'r').read()
+                            plain_text = cipher_suite.decrypt(str.encode(cipher_text),)
+                            res[elem]=pd.read_json(plain_text,orient='records')
+                            
+                        tmp=res['corrective_factors'].copy()
+                        tmp1=tmp[tmp.type=='total_conversions']
+                        del tmp1['type']
+                        tmp2=tmp[tmp.type=='total_conversion_value']
+                        del tmp2['type']
+                        
+                        res['corrective_factors']=dict()
+                        res['corrective_factors']['total_conversions']=tmp1 
+                        res['corrective_factors']['total_conversion_value']=tmp2 
+                        
+                        shutil.rmtree(path0+'/'+filename)
+                        os.chdir(path0)
+                        
+                        print("Your data has been cancelled from our server")
+                        print("Elaboration finished!")
+                        
+                        return(res)
+                    else:
+                        print("Your token is not valid. Try again or try to generate a new one.")
+                        return(-1)
                     
-                    return(res)
                 else:
-                    print("Your token is not valid. Try again or try to generate a new one.")
                     return(-1)
                 
             else:
                 return(-1)
             
-        else:
+        except:
+            url='https://{0}/api/remove_data.php?filename={1}'.format(server,filename)
+            resp=requests.get(url)
+            print("Your data has been cancelled from our server")
+            print("Elaboration interrupted with errors. Try again or write to info@channelattribution.io")
             return(-1)
+            #raise
         
-    except:
-        url='https://{0}/api/remove_data.php?filename={1}'.format(server,filename)
-        resp=requests.get(url)
-        print("Your data has been cancelled from our server")
-        print("Elaboration interrupted with errors. Try again or write to info@channelattribution.io")
-        return(-1)
-        #raise
-    
-def new_paths_attribution_api(token, tab_new,var_path,Tab_re,D_tab_corr,sep=">"):
-
-    '''
-    
-    Through this function, you can make path-level attribution using Markov model on paths you have not observed before. This function can be also used in real-time attribution. It requires a token that can be generated using the function "generate_token". Your Data will be encrypted and sent to our server for being elaborated and the output will be returned. We will not share your Data or store it, it will be canceled at the end of the elaboration. If you prefer to make path attribution locally, you can write us at info@channelattribution.io.
-    
-    Parameters
-    ----------
-    token : string
-        your personal token generated with generate_token function.
-    tab_new : DataFrame containing new paths for which you want to make path level attribution.
-        paths
-    var_path: string
-        column of tab_new containing paths.
-    Tab_re : DataFrame
-        removal effects from global attribution.
-    D_tab_corr : list of DataFrames
-        corrective factors from local attribution.
-    sep : string, default ">"
-        separator between the channels.
-
-            
-    Returns
-    -------
-    DataFrame
-        result: Dataframe
-            (column) path : path.
-            (column) idpath : path identification number.
-            (column) channel : channel name.
-            (column) weight_total_conversion : percentage of conversions associated to channel for the path considered.
-            (column) weight_total_conversion_value : percentage of conversion value associated to channel for the path considered.
-                        
-    Examples
-    --------
-    
-    Load Data
-    
-    >>> import pandas as pd    
-    >>> from ChannelAttribution import *
-    >>> Data = pd.read_csv('https://channelattribution.io/csv/Data.csv',sep=";")
+    def new_paths_attribution_api(token, tab_new,var_path,Tab_re,D_tab_corr,sep=">"):
     
-    Path level attribution 
-    
-    >>> res=markov_model_local_api(token, Data,var_path="path", var_conv="total_conversions", \\
-    >>> var_value="total_conversion_value", var_null="total_null", order=1, sep=">")
-    
-    Path level attribution on new paths
-    
-    >>> res_new=new_paths_attribution_api(token, tab_new,var_path="path", \\ 
-    >>> Tab_re=res['removal_effects'],D_tab_corr=res['corrective_factors'],sep=">")
-    
-    '''
+        '''
+        
+        Through this function, you can make path-level attribution using Markov model on paths you have not observed before. This function can be also used in real-time attribution. It requires a token that can be generated using the function "generate_token". Your Data will be encrypted and sent to our server for being elaborated and the output will be returned. We will not share your Data or store it, it will be canceled at the end of the elaboration. If you prefer to make path attribution locally, you can write us at info@channelattribution.io.
+        
+        Parameters
+        ----------
+        token : string
+            your personal token generated with generate_token function.
+        tab_new : DataFrame containing new paths for which you want to make path level attribution.
+            paths
+        var_path: string
+            column of tab_new containing paths.
+        Tab_re : DataFrame
+            removal effects from global attribution.
+        D_tab_corr : list of DataFrames
+            corrective factors from local attribution.
+        sep : string, default ">"
+            separator between the channels.
     
-    server = "api.channelattribution.net"
-
-    try:
-        ck_libs=__check_libs_for_api()
+                
+        Returns
+        -------
+        DataFrame
+            result: Dataframe
+                (column) path : path.
+                (column) idpath : path identification number.
+                (column) channel : channel name.
+                (column) weight_total_conversion : percentage of conversions associated to channel for the path considered.
+                (column) weight_total_conversion_value : percentage of conversion value associated to channel for the path considered.
+                            
+        Examples
+        --------
         
-        if ck_libs==1:
+        Load Data
         
-            __import_libs_for_api()
+        >>> import pandas as pd    
+        >>> from ChannelAttribution import *
+        >>> Data = pd.read_csv('https://channelattribution.io/csv/Data.csv',sep=";")
         
-            if "NoneType" in str(type(token)):
-                raise NameError("token must be specified. Use function generate_token(email,job,company)")
-            else:
-                if "str" not in str(type(token)):
-                    print("token must be a string")
-            
-            if "NoneType" in str(type(tab_new)):
-                raise NameError("tab_new must be specified")
-            else:
-                if "DataFrame" not in str(type(tab_new)):
-                     raise NameError("tab_new must be a DataFrame")
-                    
-            if "NoneType" in str(type(var_path)):
-                raise NameError("var_path must be specified")
-            else:
-                if "str" not in str(type(var_path)):
-                    print("var_path must be a string")
-                else:
-                    var_path_old=var_path
-                    var_path=re.sub(r"\s+", '_', var_path)
-                    tab_new.rename(columns={var_path_old: var_path},inplace=True)
+        Path level attribution 
+        
+        >>> res=markov_model_local_api(token, Data,var_path="path", var_conv="total_conversions", \\
+        >>> var_value="total_conversion_value", var_null="total_null", order=1, sep=">")
+        
+        Path level attribution on new paths
+        
+        >>> res_new=new_paths_attribution_api(token, tab_new,var_path="path", \\ 
+        >>> Tab_re=res['removal_effects'],D_tab_corr=res['corrective_factors'],sep=">")
+        
+        '''
+        
+        server = "api.channelattribution.net"
+    
+        try:
+            ck_libs=__check_libs_for_api()
             
-            if "NoneType" in str(type(Tab_re)):
-                raise NameError("Tab_re must be specified")
-            else:
-                if "DataFrame" not in str(type(Tab_re)):
-                     raise NameError("Tab_re must be a DataFrame")
+            if ck_libs==1:
             
-            if "NoneType" in str(type(D_tab_corr)):
-                raise NameError("D_tab_corr must be specified")
-            else:
-                if "dict" not in str(type(D_tab_corr)):
-                     raise NameError("D_tab_corr must be a dictionary")
+                __import_libs_for_api()
             
-            if "NoneType" not in str(type(sep)):
-                if "str" not in str(type(sep)):
-                    print("sep must be a string")
-            else:
-                print("sep must be specified")
+                if "NoneType" in str(type(token)):
+                    raise NameError("token must be specified. Use function generate_token(email,job,company)")
+                else:
+                    if "str" not in str(type(token)):
+                        print("token must be a string")
                 
-            
-            path0=os.getcwd()
-            
-            #initialize connection
-            
-            [filename,sftp]=__f_initialize_connection(server,token)
-            
-            #send input to server
-            
-            list_Data=dict()
-            list_Data['tab_new']=tab_new
-            list_Data['Tab_re']=Tab_re
-            list_Data['D_tab_corr_conv']=D_tab_corr['total_conversions']
-            list_Data['D_tab_corr_value']=D_tab_corr['total_conversion_value']
-            
-            [key,cipher_suite]=__f_send_to_server(list_Data,True,filename,server,sftp)
-            
-            if key!=-1:
-                # #elaborate on server
+                if "NoneType" in str(type(tab_new)):
+                    raise NameError("tab_new must be specified")
+                else:
+                    if "DataFrame" not in str(type(tab_new)):
+                         raise NameError("tab_new must be a DataFrame")
+                        
+                if "NoneType" in str(type(var_path)):
+                    raise NameError("var_path must be specified")
+                else:
+                    if "str" not in str(type(var_path)):
+                        print("var_path must be a string")
+                    else:
+                        var_path_old=var_path
+                        var_path=re.sub(r"\s+", '_', var_path)
+                        tab_new.rename(columns={var_path_old: var_path},inplace=True)
                 
-                print("Asking to our server to start the elaboration...")
-                url='https://{0}/api/api.php?type=new-paths-attribution&filename={1}&key={2}&var_path={3}&sep={4}&token={5}'.format(server,filename,key.decode("utf-8"),var_path,sep,token)
-                #print(url)
-                resp=requests.get(url)
-                resp=resp.text
-                print(resp)
+                if "NoneType" in str(type(Tab_re)):
+                    raise NameError("Tab_re must be specified")
+                else:
+                    if "DataFrame" not in str(type(Tab_re)):
+                         raise NameError("Tab_re must be a DataFrame")
                 
-                if "token_ko" not in resp:
-                    
-                    #retrieving output
-                    
-                    __f_retrieve_from_server(filename,sftp)
-                    
-                    print("Composing output...")
+                if "NoneType" in str(type(D_tab_corr)):
+                    raise NameError("D_tab_corr must be specified")
+                else:
+                    if "dict" not in str(type(D_tab_corr)):
+                         raise NameError("D_tab_corr must be a dictionary")
+                
+                if "NoneType" not in str(type(sep)):
+                    if "str" not in str(type(sep)):
+                        print("sep must be a string")
+                else:
+                    print("sep must be specified")
                     
-                    cipher_text = open(filename+'-O', 'r').read()
-                    plain_text = cipher_suite.decrypt(str.encode(cipher_text))
-                    res=pd.read_json(plain_text,orient='records')
+                
+                path0=os.getcwd()
+                
+                #initialize connection
+                
+                [filename,sftp]=__f_initialize_connection(server,token)
+                
+                #send input to server
+                
+                list_Data=dict()
+                list_Data['tab_new']=tab_new
+                list_Data['Tab_re']=Tab_re
+                list_Data['D_tab_corr_conv']=D_tab_corr['total_conversions']
+                list_Data['D_tab_corr_value']=D_tab_corr['total_conversion_value']
+                
+                [key,cipher_suite]=__f_send_to_server(list_Data,True,filename,server,sftp)
+                
+                if key!=-1:
+                    # #elaborate on server
                     
-                    shutil.rmtree(path0+'/'+filename)
-                    os.chdir(path0)
+                    print("Asking to our server to start the elaboration...")
+                    url='https://{0}/api/api.php?type=new-paths-attribution&filename={1}&key={2}&var_path={3}&sep={4}&token={5}'.format(server,filename,key.decode("utf-8"),var_path,sep,token)
+                    #print(url)
+                    resp=requests.get(url)
+                    resp=resp.text
+                    print(resp)
                     
-                    print("Your data has been cancelled from our server")
-                    print("Elaboration finished!") 
+                    if "token_ko" not in resp:
+                        
+                        #retrieving output
+                        
+                        __f_retrieve_from_server(filename,sftp)
+                        
+                        print("Composing output...")
+                        
+                        cipher_text = open(filename+'-O', 'r').read()
+                        plain_text = cipher_suite.decrypt(str.encode(cipher_text))
+                        res=pd.read_json(plain_text,orient='records')
+                        
+                        shutil.rmtree(path0+'/'+filename)
+                        os.chdir(path0)
+                        
+                        print("Your data has been cancelled from our server")
+                        print("Elaboration finished!") 
+                        
+                        return(res)
                     
-                    return(res)
+                    else:
+                        print("Your token is not valid. Try again or try to generate a new one.")
+                        return(-1)
                 
                 else:
-                    print("Your token is not valid. Try again or try to generate a new one.")
                     return(-1)
             
-            else:
-                return(-1)
-        
-    except:
-        url='https://{0}/api/remove_data.php?filename={1}'.format(server,filename)
-        resp=requests.get(url)
-        print("Your data has been cancelled from our server")
-        print("Elaboration interrupted with errors. Try again or write to info@channelattribution.io")
-        return(-1)
-        
-        
+        except:
+            url='https://{0}/api/remove_data.php?filename={1}'.format(server,filename)
+            resp=requests.get(url)
+            print("Your data has been cancelled from our server")
+            print("Elaboration interrupted with errors. Try again or write to info@channelattribution.io")
+            return(-1)
+            
+            
+
```

### Comparing `ChannelAttribution-2.1.3/src/cypack/functions.cpp` & `ChannelAttribution-2.1.4/src/cypack/functions.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ChannelAttribution: Markov model for online multi-channel attribution
-// Copyright (C) 2015 - 2022  Davide Altomare and David Loris <https://channelattribution.io>
+// Copyright (C) 2015 - 2023  Davide Altomare and David Loris <https://channelattribution.io>
 
 // ChannelAttribution is free software: you can redistribute it and/or modify
 // it under the terms of the GNU General Public License as published by
 // the Free Software Foundation, either version 3 of the License, or
 // (at your option) any later version.
 
 // ChannelAttribution is distributed in the hope that it will be useful,
```

### Comparing `ChannelAttribution-2.1.3/src/cypack/data/Data.csv` & `ChannelAttribution-2.1.4/src/cypack/data/Data.csv`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_cube_slices_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_cube_slices_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/CubeToMatOp_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/CubeToMatOp_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_hypot_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_hypot_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/auxlib_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/auxlib_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cor_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cor_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_mean_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_mean_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_shift.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_shift.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_min_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_min_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_static_check.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_static_check.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/hdf5_name.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/hdf5_name.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/span.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/span.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_cov_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_cov_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/def_atlas.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/def_atlas.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_join_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_join_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_kron_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_kron_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_hist.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_hist.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_elem2_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_elem2_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_div.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_div.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_strans.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_strans.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_find_unique.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_find_unique.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_resize_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_resize_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_chi2rnd_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_chi2rnd_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/podarray_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/podarray_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_normalise_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_normalise_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_all_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_all_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/BaseCube_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/BaseCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_elem.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_elem.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_polyval_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_polyval_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_nonzeros_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_nonzeros_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_prod_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_prod_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_svd.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_svd.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/unwrap_cube.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/unwrap_cube.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_SortEigenvalue.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_SortEigenvalue.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/GlueCube_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/GlueCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_range_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_range_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_kmeans.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_kmeans.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/compiler_setup_post.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/compiler_setup_post.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cond_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cond_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_trimat_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_trimat_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_cube_each_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_cube_each_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_approx_equal.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_approx_equal.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_chi2rnd.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_chi2rnd.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_reverse_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_reverse_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_stddev.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_stddev.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cumsum_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cumsum_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_ostream_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_ostream_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_index_max_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_index_max_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_chi2rnd_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_chi2rnd_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/config.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/config.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtGlueCube_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtGlueCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fft_engine.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fft_engine.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/band_helper.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/band_helper.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SizeMat_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SizeMat_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/def_superlu.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/def_superlu.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_hist_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_hist_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_norm_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_norm_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_cor_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_cor_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_SymEigsSolver_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_SymEigsSolver_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_inplace_trans.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_inplace_trans.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_eig_pair.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_eig_pair.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_var.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_var.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/running_stat_vec_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/running_stat_vec_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_times_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_times_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_diagmat_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_diagmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_quantile.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_quantile.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_trapz_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_trapz_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpBase_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpBase_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_resize_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_resize_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpRow_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpRow_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_reverse_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_reverse_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_inv_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_inv_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/compiler_extra.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/compiler_extra.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_rel_comparators.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_rel_comparators.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_sum.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_sum.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_mean_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_mean_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/def_lapack.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/def_lapack.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_diagvec_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_diagvec_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Op_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Op_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/distr_param.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/distr_param.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sort_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sort_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_cov.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_cov.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_schur.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_schur.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Op_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Op_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_hess.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_hess.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_stddev_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_stddev_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_version.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_version.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_UpperHessenbergEigen_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_UpperHessenbergEigen_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_as_scalar.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_as_scalar.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpBase_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpBase_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_elem2_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_elem2_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/eOpCube_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/eOpCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_hypot_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_hypot_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_schur.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_schur.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_UpperHessenbergQR_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_UpperHessenbergQR_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_stddev_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_stddev_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_powmat_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_powmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtGlue_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtGlue_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_var_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_var_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_randi.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_randi.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_polyfit_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_polyfit_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_affmul_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_affmul_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpProxy.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpProxy.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_each_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_each_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mul_gemv.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mul_gemv.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_SparseGenMatProd_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_SparseGenMatProd_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_pinv_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_pinv_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mp_misc.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mp_misc.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_strans_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_strans_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_eigs_gen.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_eigs_gen.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_join_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_join_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_randperm.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_randperm.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_expmat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_expmat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_histc.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_histc.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_cmath.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_cmath.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_range.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_range.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_toeplitz_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_toeplitz_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_repmat_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_repmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_norm_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_norm_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_trimat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_trimat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_join_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_join_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/eGlue_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/eGlue_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cx_scalar_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cx_scalar_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_max_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_max_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_polyval_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_polyval_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_plus.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_plus.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpSubview_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpSubview_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/csv_name.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/csv_name.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_unique.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_unique.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_hist_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_hist_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_min_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_min_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_elem_helper_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_elem_helper_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_reverse_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_reverse_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Gen_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Gen_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpMat_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpMat_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtSpOp_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtSpOp_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtSpGlue_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtSpGlue_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtOpCube_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtOpCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/include_hdf5.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/include_hdf5.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_dotext_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_dotext_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_shift_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_shift_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/arrayops_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/arrayops_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_trimat_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_trimat_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_chol_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_chol_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/GenCube_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/GenCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_relational_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_relational_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_mean.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_mean.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sort_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sort_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpOp_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpOp_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_symmat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_symmat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SizeCube_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SizeCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_all.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_all.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_intersect_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_intersect_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_accu.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_accu.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/access.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/access.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_trapz.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_trapz.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_fft.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_fft.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/xvec_htrans_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/xvec_htrans_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_solve_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_solve_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_relational_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_relational_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_htrans_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_htrans_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_sprandu.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_sprandu.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_cube_schur.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_cube_schur.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Cube_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Cube_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spdiagview_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spdiagview_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_expmat_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_expmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_eig_gen.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_eig_gen.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/cond_rel_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/cond_rel_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_config.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_config.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SizeCube_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SizeCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_times_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_times_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_field_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_field_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_inv_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_inv_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_max_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_max_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/MapMat_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/MapMat_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_max_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_max_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_wishrnd.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_wishrnd.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_schur_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_schur_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/gmm_full_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/gmm_full_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_eps.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_eps.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtSpGlue_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtSpGlue_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_UpperHessenbergEigen_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_UpperHessenbergEigen_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_interp2.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_interp2.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_rng_cxx11.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_rng_cxx11.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_toeplitz_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_toeplitz_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_sum_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_sum_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/typedef_elem_check.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/typedef_elem_check.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_affmul_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_affmul_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/config.hpp.cmake` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/config.hpp.cmake`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_nonzeros.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_nonzeros.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_min_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_min_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/def_arpack.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/def_arpack.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_TridiagEigen_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_TridiagEigen_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_reverse.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_reverse.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_chol.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_chol.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_vectorise_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_vectorise_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_fft2.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_fft2.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/gmm_diag_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/gmm_diag_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_times_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_times_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_wishrnd_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_wishrnd_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/gmm_misc_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/gmm_misc_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_diff.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_diff.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_trans.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_trans.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_quantile_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_quantile_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/include_atlas.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/include_atlas.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_DoubleShiftQR_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_DoubleShiftQR_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_logmat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_logmat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_reshape.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_reshape.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sp_plus_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sp_plus_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_atan2_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_atan2_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_var_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_var_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_index_min_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_index_min_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/translate_arpack.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/translate_arpack.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/translate_lapack.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/translate_lapack.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_roots_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_roots_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_histc_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_histc_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/OpCube_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/OpCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/OpCube_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/OpCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_DenseGenMatProd_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_DenseGenMatProd_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_normalise_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_normalise_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mul_herk.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mul_herk.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_spones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_spones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_vectorise_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_vectorise_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_dot_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_dot_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mul_gemm_mixed.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mul_gemm_mixed.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_join.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_join.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_field_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_field_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_htrans_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_htrans_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_size.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_size.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_max.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_max.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_speye.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_speye.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_htrans_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_htrans_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/eglue_core_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/eglue_core_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_reshape_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_reshape_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_shuffle.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_shuffle.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cond_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cond_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/diagmat_proxy.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/diagmat_proxy.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_polyfit_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_polyfit_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sqrtmat_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sqrtmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_intersect_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_intersect_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/memory.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/memory.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_diagvec.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_diagvec.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_GenEigsSolver_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_GenEigsSolver_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_ostream_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_ostream_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_trunc_exp.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_trunc_exp.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Mat_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Mat_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_normalise_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_normalise_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/sympd_helper.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/sympd_helper.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/podarray_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/podarray_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/xtrans_mat_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/xtrans_mat_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_resize.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_resize.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_flip_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_flip_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/typedef_mat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/typedef_mat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_misc_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_misc_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/constants.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/constants.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_clamp_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_clamp_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_sort_index.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_sort_index.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_logmat_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_logmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtOp_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtOp_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_diff_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_diff_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpMat_iterators_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpMat_iterators_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_orth_null_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_orth_null_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_plus_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_plus_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_cross_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_cross_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_trace.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_trace.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_max_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_max_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_UpperHessenbergQR_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_UpperHessenbergQR_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sort_index_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sort_index_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cumprod_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cumprod_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_rng.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_rng.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/eGlue_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/eGlue_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_var_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_var_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_reshape_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_reshape_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_diff_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_diff_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_strans_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_strans_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/translate_blas.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/translate_blas.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpToDOp_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpToDOp_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_any_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_any_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_flip_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_flip_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_merge_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_merge_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpCol_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpCol_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/constants_old.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/constants_old.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpGlue_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpGlue_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_misc_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_misc_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_cube_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_cube_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sp_minus_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sp_minus_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/field_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/field_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_mvnrnd.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_mvnrnd.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_min_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_min_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Row_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Row_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cov_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cov_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_min_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_min_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_sum_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_sum_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_forward.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_forward.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_solve.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_solve.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_svds.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_svds.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Row_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Row_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cov_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cov_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/wall_clock_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/wall_clock_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_eig_sym.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_eig_sym.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_clamp.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_clamp.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/translate_atlas.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/translate_atlas.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_cube_relational.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_cube_relational.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/injector_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/injector_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_all_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_all_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtGlueCube_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtGlueCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/unwrap.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/unwrap.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_misc_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_misc_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sort_index_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sort_index_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/injector_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/injector_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_index_min.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_index_min.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_dot.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_dot.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_index_max.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_index_max.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_find.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_find.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_cumprod.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_cumprod.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/compiler_setup.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/compiler_setup.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/eGlueCube_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/eGlueCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_hist_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_hist_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_cross.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_cross.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Base_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Base_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_det.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_det.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_shuffle_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_shuffle_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_kron_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_kron_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_ostream.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_ostream.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_eye.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_eye.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_TridiagEigen_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_TridiagEigen_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_symmat_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_symmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpRow_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpRow_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Gen_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Gen_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_toeplitz_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_toeplitz_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/CubeToMatOp_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/CubeToMatOp_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_kron_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_kron_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_str.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_str.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_quantile_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_quantile_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_strans_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_strans_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/translate_superlu.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/translate_superlu.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_each_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_each_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_merge_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_merge_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_elem1_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_elem1_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_powmat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_powmat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_find_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_find_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_DoubleShiftQR_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_DoubleShiftQR_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_symmat_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_symmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_repmat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_repmat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_range_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_range_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_diagmat_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_diagmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpToDOp_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpToDOp_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_cube_plus.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_cube_plus.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_cube_minus.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_cube_minus.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/debug.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/debug.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spdiagview_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spdiagview_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_fft_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_fft_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_max_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_max_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_powmat_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_powmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_relational_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_relational_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/gmm_full_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/gmm_full_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_cumsum.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_cumsum.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_spsolve.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_spsolve.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/eOp_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/eOp_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_cube_times.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_cube_times.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_polyfit.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_polyfit.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_syl_lyap.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_syl_lyap.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/diskio_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/diskio_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_wishrnd_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_wishrnd_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_log_det.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_log_det.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_expmat_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_expmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_cx_attrib.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_cx_attrib.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/GenCube_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/GenCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpSubview_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpSubview_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_ones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_ones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_toeplitz.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_toeplitz.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtSpOp_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtSpOp_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_find_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_find_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_histc_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_histc_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_any_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_any_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_cube_slices_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_cube_slices_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtOpCube_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtOpCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_cross_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_cross_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_minus.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_minus.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/diskio_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/diskio_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_cor.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_cor.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_reverse_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_reverse_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpSubview_iterators_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpSubview_iterators_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mul_gemm.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mul_gemm.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/sp_auxlib_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/sp_auxlib_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_conv_to.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_conv_to.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_pinv.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_pinv.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_prod_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_prod_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_relational_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_relational_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_trig.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_trig.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_roots_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_roots_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_log_normpdf.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_log_normpdf.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpMat_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpMat_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sum_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sum_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_prod.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_prod.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/GenSpecialiser.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/GenSpecialiser.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/eglue_core_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/eglue_core_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/hdf5_misc.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/hdf5_misc.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cumsum_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cumsum_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/BaseCube_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/BaseCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/include_superlu.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/include_superlu.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_min_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_min_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_mean_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_mean_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_cov_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_cov_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_repelem.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_repelem.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/upgrade_val.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/upgrade_val.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_mvnrnd_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_mvnrnd_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_mixed_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_mixed_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sum_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sum_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_cube_div.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_cube_div.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SizeMat_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SizeMat_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/xtrans_mat_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/xtrans_mat_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_schur_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_schur_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_kron_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_kron_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpOp_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpOp_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_minus_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_minus_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_randg.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_randg.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/eGlueCube_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/eGlueCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_diagmat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_diagmat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_diagmat_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_diagmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_orth_null_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_orth_null_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_repmat_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_repmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_atan2_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_atan2_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cor_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cor_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_fft_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_fft_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/strip.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/strip.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_unique_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_unique_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/field_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/field_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_index_max_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_index_max_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/restrictors.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/restrictors.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_regspace.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_regspace.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_chol_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_chol_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_normalise.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_normalise.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpCol_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpCol_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_kron.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_kron.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_min_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_min_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Mat_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Mat_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_DenseGenMatProd_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_DenseGenMatProd_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_conv_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_conv_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_find_unique_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_find_unique_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_times_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_times_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_misc.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_misc.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_diagmat_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_diagmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_normcdf.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_normcdf.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/auxlib_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/auxlib_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_mean_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_mean_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/traits.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/traits.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Col_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Col_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/running_stat_vec_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/running_stat_vec_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_cube_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_cube_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_intersect.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_intersect.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_median_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_median_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_lu.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_lu.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Glue_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Glue_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/ProxyCube.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/ProxyCube.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_min_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_min_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_rng_cxx98.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/arma_rng_cxx98.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_plus_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_plus_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/unwrap_spmat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/unwrap_spmat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/eop_core_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/eop_core_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_max_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_max_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_trapz_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_trapz_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/cond_rel_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/cond_rel_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Col_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Col_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/typedef_elem.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/typedef_elem.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_join_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_join_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_polyval.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_polyval.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_clamp_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_clamp_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_inv.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_inv.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_elem_helper_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_elem_helper_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpValProxy_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpValProxy_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sqrtmat_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sqrtmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_hist_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_hist_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtGlue_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtGlue_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_numel.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_numel.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/running_stat_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/running_stat_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_relational_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_relational_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_max_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_max_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_randu.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_randu.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_SymEigsSolver_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_SymEigsSolver_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Glue_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Glue_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_symmat_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_symmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_norm.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_norm.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_unique_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_unique_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mul_syrk.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mul_syrk.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_sprandn.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_sprandn.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_orth_null.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_orth_null.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtOp_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/mtOp_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_elem1_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_elem1_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_repelem_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_repelem_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_randn.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_randn.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/sp_auxlib_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/sp_auxlib_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_conv.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_conv.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_SparseGenMatProd_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_SparseGenMatProd_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_toeplitz_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_toeplitz_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_vectorise_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_vectorise_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_dot_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_dot_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_princomp_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_princomp_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/diagview_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/diagview_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Base_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Base_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Cube_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Cube_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_trimat_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_trimat_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_princomp.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_princomp.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_htrans_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_htrans_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_any.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_any.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_trimat_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_trimat_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_GenEigsSolver_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_GenEigsSolver_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/running_stat_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/running_stat_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/MapMat_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/MapMat_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/GlueCube_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/GlueCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_conv_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_conv_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_var_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_var_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_index_min_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_index_min_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sp_minus_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sp_minus_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_cor_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_cor_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_princomp_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_princomp_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_repmat_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_repmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_diagvec_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_diagvec_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/gmm_diag_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/gmm_diag_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_shift_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_shift_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_mixed_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_mixed_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_minus_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_minus_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/trimat_helper.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/trimat_helper.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/def_blas.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/def_blas.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/typedef_mat_fixed.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/typedef_mat_fixed.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/eop_aux.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/eop_aux.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_vectorise.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_vectorise.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_cond.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_cond.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_eigs_sym.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_eigs_sym.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/wall_clock_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/wall_clock_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_nonzeros_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_nonzeros_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/eOpCube_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/eOpCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_trunc_log.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_trunc_log.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_times.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_times.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_misc_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_misc_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sp_plus_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_sp_plus_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_vectorise_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_vectorise_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_EigsSelect.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/newarp_EigsSelect.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_n_unique.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_n_unique.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_dotext_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_dotext_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_max_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_max_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/def_hdf5.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/def_hdf5.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/eOp_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/eOp_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpGlue_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpGlue_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_sort.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_sort.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_cube_each_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/subview_cube_each_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_pinv_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_pinv_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_symmat_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_symmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/xvec_htrans_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/xvec_htrans_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_relational_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spglue_relational_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/gmm_misc_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/gmm_misc_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_sqrtmat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_sqrtmat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cumprod_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cumprod_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/Proxy.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/Proxy.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_rank.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_rank.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cx_scalar_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_cx_scalar_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/diagview_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/diagview_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_normalise_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_normalise_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_qr.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_qr.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_repmat_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/spop_repmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_min.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_min.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_zeros.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_zeros.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_median.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_median.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/arrayops_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/arrayops_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpValProxy_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/SpValProxy_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_repelem_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_repelem_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_normpdf.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_normpdf.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_flip.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_flip.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_strans_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_strans_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_shuffle_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_shuffle_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_logmat_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_logmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_inplace_strans.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_inplace_strans.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_qz.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_qz.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_interp1.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_interp1.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_relational.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/operator_relational.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_find_unique_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_find_unique_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/promote_type.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/promote_type.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_median_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/op_median_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_mvnrnd_bones.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_mvnrnd_bones.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_roots.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/fn_roots.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/eop_core_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/eop_core_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_solve_meat.hpp` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/include/armadillo_bits/glue_solve_meat.hpp`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/NOTICE.txt` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/LICENSE.txt` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/armadillo-9.860.2/README.md` & `ChannelAttribution-2.1.4/src/cypack/armadillo-9.860.2/README.md`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/src/cypack/functions.h` & `ChannelAttribution-2.1.4/src/cypack/functions.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ChannelAttribution: Markov model for online multi-channel attribution
-// Copyright (C) 2015 - 2022  Davide Altomare and David Loris <https://channelattribution.io>
+// Copyright (C) 2015 - 2023  Davide Altomare and David Loris <https://channelattribution.io>
 
 // ChannelAttribution is free software: you can redistribute it and/or modify
 // it under the terms of the GNU General Public License as published by
 // the Free Software Foundation, either version 3 of the License, or
 // (at your option) any later version.
 
 // ChannelAttribution is distributed in the hope that it will be useful,
```

### Comparing `ChannelAttribution-2.1.3/src/cypack/generate_doc.py` & `ChannelAttribution-2.1.4/src/cypack/generate_doc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #ChannelAttribution: Markov model for online multi-channel attribution
-#Copyright (C) 2015 - 2022  Davide Altomare and David Loris <https://channelattribution.io>
+#Copyright (C) 2015 - 2023  Davide Altomare and David Loris <https://channelattribution.io>
 #
 #ChannelAttribution is free software: you can redistribute it and/or modify
 #it under the terms of the GNU General Public License as published by
 #the Free Software Foundation, either version 3 of the License, or
 #(at your option) any later version.
 #
 #ChannelAttribution is distributed in the hope that it will be useful,
```

### Comparing `ChannelAttribution-2.1.3/src/ChannelAttribution.egg-info/PKG-INFO` & `ChannelAttribution-2.1.4/src/ChannelAttribution.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChannelAttribution
-Version: 2.1.3
+Version: 2.1.4
 Summary: Markov Model for Online Multi-Channel Attribution
 Home-page: https://channelattribution.io
 Author: Davide Altomare, David Loris
 Author-email: info@channelattribution.io
 License: GPLv3
 Project-URL: Documentation, https://channelattribution.io
 Project-URL: Code, https://gitlab.com/session-tech/ChannelAttribution
```

### Comparing `ChannelAttribution-2.1.3/setup.py` & `ChannelAttribution-2.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/README.md` & `ChannelAttribution-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ChannelAttribution-2.1.3/setup.cfg` & `ChannelAttribution-2.1.4/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ChannelAttribution
-version = 2.1.3
+version = 2.1.4
 description = Markov Model for Online Multi-Channel Attribution
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = GPLv3
 author = Davide Altomare, David Loris
 author_email = info@channelattribution.io
 url = https://channelattribution.io
```

