# Comparing `tmp/liblip-0.90.tar.gz` & `tmp/liblip-0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liblip-0.90.tar", last modified: Thu Apr  6 04:47:15 2023, max compression
+gzip compressed data, was "liblip-0.91.tar", last modified: Thu Apr 13 07:18:38 2023, max compression
```

## Comparing `liblip-0.90.tar` & `liblip-0.91.tar`

### file list

```diff
@@ -1,142 +1,145 @@
-drwxr-xr-x   0 nhenseler   (501) staff       (20)        0 2023-04-06 04:47:15.922672 liblip-0.90/
--rw-r--r--   0 nhenseler   (501) staff       (20)     7652 2022-04-26 03:16:57.000000 liblip-0.90/LICENSE.txt
--rw-rw-r--   0 nhenseler   (501) staff       (20)      401 2022-07-22 05:34:26.000000 liblip-0.90/MANIFEST.in
--rw-r--r--   0 nhenseler   (501) staff       (20)     2913 2023-04-06 04:47:15.922198 liblip-0.90/PKG-INFO
--rw-rw-r--   0 nhenseler   (501) staff       (20)     2564 2022-06-21 05:47:23.000000 liblip-0.90/README.md
-drwxr-xr-x   0 nhenseler   (501) staff       (20)        0 2023-04-06 04:47:15.293585 liblip-0.90/dist/
--rw-r--r--   0 nhenseler   (501) staff       (20)   374533 2023-04-06 04:47:14.000000 liblip-0.90/dist/liblip-0.90-cp39-cp39-macosx_10_9_x86_64.whl
-drwxr-xr-x   0 nhenseler   (501) staff       (20)        0 2023-04-06 04:47:15.310772 liblip-0.90/docs/
--rw-------   0 nhenseler   (501) staff       (20)   269989 2022-06-15 02:32:51.000000 liblip-0.90/docs/liblip2.pdf
--rw-r--r--   0 nhenseler   (501) staff       (20)       38 2023-04-06 04:47:15.922807 liblip-0.90/setup.cfg
--rw-r--r--   0 nhenseler   (501) staff       (20)      973 2023-04-06 04:23:58.000000 liblip-0.90/setup.py
-drwxr-xr-x   0 nhenseler   (501) staff       (20)        0 2023-04-06 04:47:15.815210 liblip-0.90/src/
--rw-r--r--   0 nhenseler   (501) staff       (20)     7753 2022-08-02 03:50:27.000000 liblip-0.90/src/build_liblip.nh.py
--rw-------   0 nhenseler   (501) staff       (20)     7899 2023-03-15 05:29:24.000000 liblip-0.90/src/build_liblip.py
--rw-rw-r--   0 nhenseler   (501) staff       (20)    30172 2021-11-01 07:21:28.000000 liblip-0.90/src/dliblip.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)    20331 2006-05-03 02:52:18.000000 liblip-0.90/src/forest.cpp
--rw-rw-r--   0 nhenseler   (501) staff       (20)    12147 2022-10-28 00:10:32.000000 liblip-0.90/src/forest.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)    24323 2006-05-11 08:00:00.000000 liblip-0.90/src/glpavl.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)     4835 2006-05-11 08:00:00.000000 liblip-0.90/src/glpavl.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)     2568 2006-05-11 08:00:00.000000 liblip-0.90/src/glpbfi.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)     2173 2006-05-11 08:00:00.000000 liblip-0.90/src/glpbfi.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)     9339 2006-05-11 08:00:00.000000 liblip-0.90/src/glpdmp.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)     2839 2006-05-11 08:00:00.000000 liblip-0.90/src/glpdmp.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)    19209 2006-05-11 08:00:00.000000 liblip-0.90/src/glphbm.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)     4687 2006-05-11 08:00:00.000000 liblip-0.90/src/glphbm.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)   109626 2006-05-11 08:00:00.000000 liblip-0.90/src/glpiet.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    25349 2006-05-11 08:00:00.000000 liblip-0.90/src/glpiet.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)    28535 2006-05-11 08:00:00.000000 liblip-0.90/src/glpinv.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)     7472 2006-05-11 08:00:00.000000 liblip-0.90/src/glpinv.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)    25402 2006-05-11 08:00:00.000000 liblip-0.90/src/glpios.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)    71134 2006-05-11 08:00:00.000000 liblip-0.90/src/glpios1.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    23171 2006-05-11 08:00:00.000000 liblip-0.90/src/glpios2.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    51076 2021-11-01 00:54:56.000000 liblip-0.90/src/glpios3.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    34775 2006-05-11 08:00:00.000000 liblip-0.90/src/glpipm.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)     1451 2006-05-11 08:00:00.000000 liblip-0.90/src/glpipm.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)    11686 2006-05-11 08:00:00.000000 liblip-0.90/src/glpipp.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)    24541 2006-05-11 08:00:00.000000 liblip-0.90/src/glpipp1.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    46090 2021-11-01 00:54:56.000000 liblip-0.90/src/glpipp2.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)     1235 2006-05-11 08:00:00.000000 liblip-0.90/src/glpk.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)     7145 2006-05-11 08:00:00.000000 liblip-0.90/src/glplib.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)     2108 2006-05-11 08:00:00.000000 liblip-0.90/src/glplib1a.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)     2679 2006-05-11 08:00:00.000000 liblip-0.90/src/glplib1b.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    18290 2006-05-11 08:00:00.000000 liblip-0.90/src/glplib2.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    10491 2006-05-11 08:00:00.000000 liblip-0.90/src/glplib3.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)     6251 2006-05-11 08:00:00.000000 liblip-0.90/src/glplib4.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    12283 2006-05-11 08:00:00.000000 liblip-0.90/src/glplpp.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)    27239 2006-05-11 08:00:00.000000 liblip-0.90/src/glplpp1.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    61774 2006-05-11 08:00:00.000000 liblip-0.90/src/glplpp2.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    50103 2006-05-11 08:00:00.000000 liblip-0.90/src/glplpx.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)    56895 2006-05-11 08:00:00.000000 liblip-0.90/src/glplpx1.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    36870 2006-05-11 08:00:00.000000 liblip-0.90/src/glplpx2.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    13102 2006-05-11 08:00:00.000000 liblip-0.90/src/glplpx3.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    17130 2006-05-11 08:00:00.000000 liblip-0.90/src/glplpx4.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    30788 2006-05-11 08:00:00.000000 liblip-0.90/src/glplpx5.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    40906 2006-05-11 08:00:00.000000 liblip-0.90/src/glplpx6a.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    21456 2006-05-11 08:00:00.000000 liblip-0.90/src/glplpx6b.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    13769 2006-05-11 08:00:00.000000 liblip-0.90/src/glplpx6c.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    28370 2006-05-11 08:00:00.000000 liblip-0.90/src/glplpx6d.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    53622 2006-05-11 08:00:00.000000 liblip-0.90/src/glplpx7.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    36085 2006-05-11 08:00:00.000000 liblip-0.90/src/glplpx7a.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    25760 2006-05-11 08:00:00.000000 liblip-0.90/src/glplpx7b.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)   117149 2006-05-11 08:00:00.000000 liblip-0.90/src/glplpx8a.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    24591 2006-05-11 08:00:00.000000 liblip-0.90/src/glplpx8b.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    41564 2006-05-11 08:00:00.000000 liblip-0.90/src/glplpx8c.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)     7668 2006-05-11 08:00:00.000000 liblip-0.90/src/glplpx8d.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    19056 2006-05-11 08:00:00.000000 liblip-0.90/src/glplpx8e.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    71972 2006-05-11 08:00:00.000000 liblip-0.90/src/glpluf.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    16519 2006-05-11 08:00:00.000000 liblip-0.90/src/glpluf.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)    27131 2006-05-11 08:00:00.000000 liblip-0.90/src/glpmat.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)     5307 2006-05-11 08:00:00.000000 liblip-0.90/src/glpmat.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)    14025 2006-05-11 08:00:00.000000 liblip-0.90/src/glpmip.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)    25727 2006-05-11 08:00:00.000000 liblip-0.90/src/glpmip1.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    44349 2021-11-01 00:54:56.000000 liblip-0.90/src/glpmip2.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    83432 2006-05-11 08:00:00.000000 liblip-0.90/src/glpmpl.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)   151015 2021-11-01 01:01:42.000000 liblip-0.90/src/glpmpl1.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    45377 2006-05-11 08:00:00.000000 liblip-0.90/src/glpmpl2.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)   185816 2021-11-01 00:57:20.000000 liblip-0.90/src/glpmpl3.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    45632 2006-05-11 08:00:00.000000 liblip-0.90/src/glpmpl4.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    18410 2006-05-11 08:00:00.000000 liblip-0.90/src/glpqmd.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)     2404 2006-05-11 08:00:00.000000 liblip-0.90/src/glpqmd.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)     6227 2006-05-11 08:00:00.000000 liblip-0.90/src/glprng.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)     2076 2006-05-11 08:00:00.000000 liblip-0.90/src/glprng.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)    17970 2006-05-11 08:00:00.000000 liblip-0.90/src/glpspx.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)    69092 2006-05-11 08:00:00.000000 liblip-0.90/src/glpspx1.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)    50759 2006-05-11 08:00:00.000000 liblip-0.90/src/glpspx2.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)     7166 2006-05-11 08:00:00.000000 liblip-0.90/src/glpstr.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)     2784 2006-05-11 08:00:00.000000 liblip-0.90/src/glpstr.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)    23925 2006-05-11 08:00:00.000000 liblip-0.90/src/glptsp.c
--rw-rw-r--   0 nhenseler   (501) staff       (20)     4480 2006-05-11 08:00:00.000000 liblip-0.90/src/glptsp.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)    14312 2022-07-12 02:41:10.000000 liblip-0.90/src/interpol.cpp
--rw-rw-r--   0 nhenseler   (501) staff       (20)     9379 2022-07-06 05:57:56.000000 liblip-0.90/src/interpol.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)     5237 2006-05-03 02:52:16.000000 liblip-0.90/src/jama_cholesky.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)    28352 2006-05-03 02:52:16.000000 liblip-0.90/src/jama_eig.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)     6955 2006-05-03 02:52:16.000000 liblip-0.90/src/jama_lu.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)     7348 2006-05-03 02:52:16.000000 liblip-0.90/src/jama_qr.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)    14442 2006-05-03 02:52:18.000000 liblip-0.90/src/jama_svd.h
--rw-------   0 nhenseler   (501) staff       (20)     3354 2023-03-27 06:39:04.000000 liblip-0.90/src/liblip values.h
--rw-------   0 nhenseler   (501) staff       (20)    15129 2023-03-15 05:20:31.000000 liblip-0.90/src/liblip.cpp
-drwxr-xr-x   0 nhenseler   (501) staff       (20)        0 2023-04-06 04:47:15.819683 liblip-0.90/src/liblip.egg-info/
--rw-r--r--   0 nhenseler   (501) staff       (20)     6148 2023-03-16 00:24:24.000000 liblip-0.90/src/liblip.egg-info/.DS_Store
--rw-r--r--   0 nhenseler   (501) staff       (20)     2913 2023-04-06 04:47:14.000000 liblip-0.90/src/liblip.egg-info/PKG-INFO
--rw-r--r--   0 nhenseler   (501) staff       (20)     2333 2023-04-06 04:47:14.000000 liblip-0.90/src/liblip.egg-info/SOURCES.txt
--rw-r--r--   0 nhenseler   (501) staff       (20)        1 2023-04-06 04:47:14.000000 liblip-0.90/src/liblip.egg-info/dependency_links.txt
--rw-r--r--   0 nhenseler   (501) staff       (20)       12 2023-04-06 04:47:14.000000 liblip-0.90/src/liblip.egg-info/requires.txt
--rw-r--r--   0 nhenseler   (501) staff       (20)       15 2023-04-06 04:47:14.000000 liblip-0.90/src/liblip.egg-info/top_level.txt
--rw-------   0 nhenseler   (501) staff       (20)     8379 2023-03-15 05:20:31.000000 liblip-0.90/src/liblip.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)     8230 2022-08-02 03:50:00.000000 liblip-0.90/src/liblip.nh.h
--rw-r--r--   0 nhenseler   (501) staff       (20)    79553 2023-04-06 04:45:49.000000 liblip-0.90/src/liblip.py
--rw-rw-r--   0 nhenseler   (501) staff       (20)      385 2006-05-03 02:52:18.000000 liblip-0.90/src/liblipc.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)    12923 2022-06-15 05:12:04.000000 liblip-0.90/src/memblock.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)    87596 2022-06-23 07:12:34.000000 liblip-0.90/src/slipint.cpp
--rw-rw-r--   0 nhenseler   (501) staff       (20)    20928 2022-10-28 00:30:05.000000 liblip-0.90/src/slipint.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)     1744 2006-05-03 02:52:18.000000 liblip-0.90/src/tnt.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)     4873 2006-05-03 02:52:18.000000 liblip-0.90/src/tnt_array1d.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)     3082 2006-05-03 02:52:18.000000 liblip-0.90/src/tnt_array1d_utils.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)     5171 2006-05-03 02:52:18.000000 liblip-0.90/src/tnt_array2d.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)     4613 2006-05-03 02:52:18.000000 liblip-0.90/src/tnt_array2d_utils.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)     5209 2006-05-03 02:52:18.000000 liblip-0.90/src/tnt_array3d.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)     3738 2006-05-03 02:52:18.000000 liblip-0.90/src/tnt_array3d_utils.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)    10757 2006-05-03 02:52:18.000000 liblip-0.90/src/tnt_cmat.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)     5315 2006-05-03 02:52:18.000000 liblip-0.90/src/tnt_fortran_array1d.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)     4015 2006-05-03 02:52:18.000000 liblip-0.90/src/tnt_fortran_array1d_utils.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)     4395 2006-05-03 02:52:18.000000 liblip-0.90/src/tnt_fortran_array2d.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)     4050 2006-05-03 02:52:18.000000 liblip-0.90/src/tnt_fortran_array2d_utils.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)     4489 2006-05-03 02:52:18.000000 liblip-0.90/src/tnt_fortran_array3d.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)     4676 2006-05-03 02:52:18.000000 liblip-0.90/src/tnt_fortran_array3d_utils.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)     4392 2006-05-03 02:52:18.000000 liblip-0.90/src/tnt_i_refvec.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)      913 2021-11-01 00:39:36.000000 liblip-0.90/src/tnt_math_utils.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)     2805 2022-06-17 02:50:12.000000 liblip-0.90/src/tnt_sparse_matrix_csr 5.54.44 pm 5.54.44 pm.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)     2805 2022-06-17 02:50:12.000000 liblip-0.90/src/tnt_sparse_matrix_csr.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)     1713 2006-05-03 02:52:18.000000 liblip-0.90/src/tnt_stopwatch.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)     1565 2006-05-03 02:52:18.000000 liblip-0.90/src/tnt_subscript.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)     7175 2006-05-03 02:52:18.000000 liblip-0.90/src/tnt_vec.h
--rw-rw-r--   0 nhenseler   (501) staff       (20)     1042 2006-05-03 02:52:18.000000 liblip-0.90/src/tnt_version.h
-drwxr-xr-x   0 nhenseler   (501) staff       (20)        0 2023-04-06 04:47:15.874347 liblip-0.90/tests/
-drwxr-xr-x   0 nhenseler   (501) staff       (20)        0 2023-04-06 04:47:15.920337 liblip-0.90/tests/.ipynb_checkpoints/
--rw-r--r--   0 nhenseler   (501) staff       (20)   558003 2022-07-22 06:01:37.000000 liblip-0.90/tests/.ipynb_checkpoints/test_wrapper_3d-checkpoint.ipynb
--rw-r--r--   0 nhenseler   (501) staff       (20)     1766 2022-11-03 08:20:51.000000 liblip-0.90/tests/test_for_model_comparison.py
--rw-r--r--   0 nhenseler   (501) staff       (20)     1932 2022-07-15 05:15:38.000000 liblip-0.90/tests/test_no_wrapper.py
--rw-r--r--   0 nhenseler   (501) staff       (20)     1553 2023-03-08 04:28:17.000000 liblip-0.90/tests/test_performance.py
--rw-r--r--   0 nhenseler   (501) staff       (20)    35649 2023-02-23 06:56:41.000000 liblip-0.90/tests/test_wrapper.py
--rw-r--r--   0 nhenseler   (501) staff       (20)   541398 2022-07-25 09:58:53.000000 liblip-0.90/tests/test_wrapper_3d.ipynb
+drwxr-xr-x   0 nhenseler   (501) staff       (20)        0 2023-04-13 07:18:38.016372 liblip-0.91/
+-rw-r--r--   0 nhenseler   (501) staff       (20)     7652 2022-04-26 03:16:57.000000 liblip-0.91/LICENSE.txt
+-rw-rw-r--   0 nhenseler   (501) staff       (20)      401 2022-07-22 05:34:26.000000 liblip-0.91/MANIFEST.in
+-rw-r--r--   0 nhenseler   (501) staff       (20)     2913 2023-04-13 07:18:38.015803 liblip-0.91/PKG-INFO
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     2564 2022-06-21 05:47:23.000000 liblip-0.91/README.md
+drwxr-xr-x   0 nhenseler   (501) staff       (20)        0 2023-04-13 07:18:37.499987 liblip-0.91/dist/
+-rw-r--r--   0 nhenseler   (501) staff       (20)   384426 2023-04-13 07:18:36.000000 liblip-0.91/dist/liblip-0.91-cp39-cp39-macosx_10_9_x86_64.whl
+drwxr-xr-x   0 nhenseler   (501) staff       (20)        0 2023-04-13 07:18:37.523603 liblip-0.91/docs/
+-rw-------   0 nhenseler   (501) staff       (20)   269989 2022-06-15 02:32:51.000000 liblip-0.91/docs/liblip2.pdf
+-rw-r--r--   0 nhenseler   (501) staff       (20)       38 2023-04-13 07:18:38.016562 liblip-0.91/setup.cfg
+-rw-r--r--   0 nhenseler   (501) staff       (20)      973 2023-04-13 06:15:37.000000 liblip-0.91/setup.py
+drwxr-xr-x   0 nhenseler   (501) staff       (20)        0 2023-04-13 07:18:37.884371 liblip-0.91/src/
+-rw-------   0 nhenseler   (501) staff       (20)     7899 2023-03-15 05:29:24.000000 liblip-0.91/src/build_liblip.bak.py
+-rw-r--r--   0 nhenseler   (501) staff       (20)     7753 2022-08-02 03:50:27.000000 liblip-0.91/src/build_liblip.nh.py
+-rw-------   0 nhenseler   (501) staff       (20)    10912 2023-04-13 06:43:07.000000 liblip-0.91/src/build_liblip.py
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    30172 2021-11-01 07:21:28.000000 liblip-0.91/src/dliblip.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    20331 2006-05-03 02:52:18.000000 liblip-0.91/src/forest.cpp
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    12147 2022-10-28 00:10:32.000000 liblip-0.91/src/forest.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    24323 2006-05-11 08:00:00.000000 liblip-0.91/src/glpavl.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     4835 2006-05-11 08:00:00.000000 liblip-0.91/src/glpavl.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     2568 2006-05-11 08:00:00.000000 liblip-0.91/src/glpbfi.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     2173 2006-05-11 08:00:00.000000 liblip-0.91/src/glpbfi.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     9339 2006-05-11 08:00:00.000000 liblip-0.91/src/glpdmp.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     2839 2006-05-11 08:00:00.000000 liblip-0.91/src/glpdmp.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    19209 2006-05-11 08:00:00.000000 liblip-0.91/src/glphbm.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     4687 2006-05-11 08:00:00.000000 liblip-0.91/src/glphbm.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)   109626 2006-05-11 08:00:00.000000 liblip-0.91/src/glpiet.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    25349 2006-05-11 08:00:00.000000 liblip-0.91/src/glpiet.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    28535 2006-05-11 08:00:00.000000 liblip-0.91/src/glpinv.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     7472 2006-05-11 08:00:00.000000 liblip-0.91/src/glpinv.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    25402 2006-05-11 08:00:00.000000 liblip-0.91/src/glpios.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    71134 2006-05-11 08:00:00.000000 liblip-0.91/src/glpios1.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    23171 2006-05-11 08:00:00.000000 liblip-0.91/src/glpios2.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    51076 2021-11-01 00:54:56.000000 liblip-0.91/src/glpios3.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    34775 2006-05-11 08:00:00.000000 liblip-0.91/src/glpipm.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     1451 2006-05-11 08:00:00.000000 liblip-0.91/src/glpipm.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    11686 2006-05-11 08:00:00.000000 liblip-0.91/src/glpipp.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    24541 2006-05-11 08:00:00.000000 liblip-0.91/src/glpipp1.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    46090 2021-11-01 00:54:56.000000 liblip-0.91/src/glpipp2.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     1235 2006-05-11 08:00:00.000000 liblip-0.91/src/glpk.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     7145 2006-05-11 08:00:00.000000 liblip-0.91/src/glplib.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     2108 2006-05-11 08:00:00.000000 liblip-0.91/src/glplib1a.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     2679 2006-05-11 08:00:00.000000 liblip-0.91/src/glplib1b.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    18290 2006-05-11 08:00:00.000000 liblip-0.91/src/glplib2.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    10491 2006-05-11 08:00:00.000000 liblip-0.91/src/glplib3.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     6251 2006-05-11 08:00:00.000000 liblip-0.91/src/glplib4.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    12283 2006-05-11 08:00:00.000000 liblip-0.91/src/glplpp.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    27239 2006-05-11 08:00:00.000000 liblip-0.91/src/glplpp1.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    61774 2006-05-11 08:00:00.000000 liblip-0.91/src/glplpp2.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    50103 2006-05-11 08:00:00.000000 liblip-0.91/src/glplpx.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    56895 2006-05-11 08:00:00.000000 liblip-0.91/src/glplpx1.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    36870 2006-05-11 08:00:00.000000 liblip-0.91/src/glplpx2.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    13102 2006-05-11 08:00:00.000000 liblip-0.91/src/glplpx3.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    17130 2006-05-11 08:00:00.000000 liblip-0.91/src/glplpx4.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    30788 2006-05-11 08:00:00.000000 liblip-0.91/src/glplpx5.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    40906 2006-05-11 08:00:00.000000 liblip-0.91/src/glplpx6a.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    21456 2006-05-11 08:00:00.000000 liblip-0.91/src/glplpx6b.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    13769 2006-05-11 08:00:00.000000 liblip-0.91/src/glplpx6c.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    28370 2006-05-11 08:00:00.000000 liblip-0.91/src/glplpx6d.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    53622 2006-05-11 08:00:00.000000 liblip-0.91/src/glplpx7.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    36085 2006-05-11 08:00:00.000000 liblip-0.91/src/glplpx7a.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    25760 2006-05-11 08:00:00.000000 liblip-0.91/src/glplpx7b.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)   117149 2006-05-11 08:00:00.000000 liblip-0.91/src/glplpx8a.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    24591 2006-05-11 08:00:00.000000 liblip-0.91/src/glplpx8b.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    41564 2006-05-11 08:00:00.000000 liblip-0.91/src/glplpx8c.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     7668 2006-05-11 08:00:00.000000 liblip-0.91/src/glplpx8d.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    19056 2006-05-11 08:00:00.000000 liblip-0.91/src/glplpx8e.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    71972 2006-05-11 08:00:00.000000 liblip-0.91/src/glpluf.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    16519 2006-05-11 08:00:00.000000 liblip-0.91/src/glpluf.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    27131 2006-05-11 08:00:00.000000 liblip-0.91/src/glpmat.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     5307 2006-05-11 08:00:00.000000 liblip-0.91/src/glpmat.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    14025 2006-05-11 08:00:00.000000 liblip-0.91/src/glpmip.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    25727 2006-05-11 08:00:00.000000 liblip-0.91/src/glpmip1.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    44349 2021-11-01 00:54:56.000000 liblip-0.91/src/glpmip2.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    83432 2006-05-11 08:00:00.000000 liblip-0.91/src/glpmpl.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)   151015 2021-11-01 01:01:42.000000 liblip-0.91/src/glpmpl1.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    45377 2006-05-11 08:00:00.000000 liblip-0.91/src/glpmpl2.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)   185816 2021-11-01 00:57:20.000000 liblip-0.91/src/glpmpl3.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    45632 2006-05-11 08:00:00.000000 liblip-0.91/src/glpmpl4.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    18410 2006-05-11 08:00:00.000000 liblip-0.91/src/glpqmd.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     2404 2006-05-11 08:00:00.000000 liblip-0.91/src/glpqmd.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     6227 2006-05-11 08:00:00.000000 liblip-0.91/src/glprng.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     2076 2006-05-11 08:00:00.000000 liblip-0.91/src/glprng.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    17970 2006-05-11 08:00:00.000000 liblip-0.91/src/glpspx.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    69092 2006-05-11 08:00:00.000000 liblip-0.91/src/glpspx1.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    50759 2006-05-11 08:00:00.000000 liblip-0.91/src/glpspx2.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     7166 2006-05-11 08:00:00.000000 liblip-0.91/src/glpstr.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     2784 2006-05-11 08:00:00.000000 liblip-0.91/src/glpstr.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    23925 2006-05-11 08:00:00.000000 liblip-0.91/src/glptsp.c
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     4480 2006-05-11 08:00:00.000000 liblip-0.91/src/glptsp.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    14312 2022-07-12 02:41:10.000000 liblip-0.91/src/interpol.cpp
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     9379 2022-07-06 05:57:56.000000 liblip-0.91/src/interpol.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     5237 2006-05-03 02:52:16.000000 liblip-0.91/src/jama_cholesky.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    28352 2006-05-03 02:52:16.000000 liblip-0.91/src/jama_eig.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     6955 2006-05-03 02:52:16.000000 liblip-0.91/src/jama_lu.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     7348 2006-05-03 02:52:16.000000 liblip-0.91/src/jama_qr.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    14442 2006-05-03 02:52:18.000000 liblip-0.91/src/jama_svd.h
+-rw-------   0 nhenseler   (501) staff       (20)     3354 2023-03-27 06:39:04.000000 liblip-0.91/src/liblip values.h
+-rw-------   0 nhenseler   (501) staff       (20)     8379 2023-03-15 05:20:31.000000 liblip-0.91/src/liblip.bak.h
+-rw-r--r--   0 nhenseler   (501) staff       (20)    79553 2023-04-06 04:45:49.000000 liblip-0.91/src/liblip.bak.py
+-rw-------   0 nhenseler   (501) staff       (20)    22100 2023-04-13 06:36:36.000000 liblip-0.91/src/liblip.cpp
+drwxr-xr-x   0 nhenseler   (501) staff       (20)        0 2023-04-13 07:18:37.903535 liblip-0.91/src/liblip.egg-info/
+-rw-r--r--   0 nhenseler   (501) staff       (20)     6148 2023-03-16 00:24:24.000000 liblip-0.91/src/liblip.egg-info/.DS_Store
+-rw-r--r--   0 nhenseler   (501) staff       (20)     2913 2023-04-13 07:18:36.000000 liblip-0.91/src/liblip.egg-info/PKG-INFO
+-rw-r--r--   0 nhenseler   (501) staff       (20)     2392 2023-04-13 07:18:36.000000 liblip-0.91/src/liblip.egg-info/SOURCES.txt
+-rw-r--r--   0 nhenseler   (501) staff       (20)        1 2023-04-13 07:18:36.000000 liblip-0.91/src/liblip.egg-info/dependency_links.txt
+-rw-r--r--   0 nhenseler   (501) staff       (20)       12 2023-04-13 07:18:36.000000 liblip-0.91/src/liblip.egg-info/requires.txt
+-rw-r--r--   0 nhenseler   (501) staff       (20)       15 2023-04-13 07:18:36.000000 liblip-0.91/src/liblip.egg-info/top_level.txt
+-rw-------   0 nhenseler   (501) staff       (20)    11093 2023-04-13 06:43:28.000000 liblip-0.91/src/liblip.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     8230 2022-08-02 03:50:00.000000 liblip-0.91/src/liblip.nh.h
+-rw-------   0 nhenseler   (501) staff       (20)    78700 2023-04-13 07:14:54.000000 liblip-0.91/src/liblip.py
+-rw-rw-r--   0 nhenseler   (501) staff       (20)      385 2006-05-03 02:52:18.000000 liblip-0.91/src/liblipc.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    12923 2022-06-15 05:12:04.000000 liblip-0.91/src/memblock.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    87596 2022-06-23 07:12:34.000000 liblip-0.91/src/slipint.cpp
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    20928 2022-10-28 00:30:05.000000 liblip-0.91/src/slipint.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     1744 2006-05-03 02:52:18.000000 liblip-0.91/src/tnt.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     4873 2006-05-03 02:52:18.000000 liblip-0.91/src/tnt_array1d.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     3082 2006-05-03 02:52:18.000000 liblip-0.91/src/tnt_array1d_utils.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     5171 2006-05-03 02:52:18.000000 liblip-0.91/src/tnt_array2d.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     4613 2006-05-03 02:52:18.000000 liblip-0.91/src/tnt_array2d_utils.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     5209 2006-05-03 02:52:18.000000 liblip-0.91/src/tnt_array3d.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     3738 2006-05-03 02:52:18.000000 liblip-0.91/src/tnt_array3d_utils.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)    10757 2006-05-03 02:52:18.000000 liblip-0.91/src/tnt_cmat.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     5315 2006-05-03 02:52:18.000000 liblip-0.91/src/tnt_fortran_array1d.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     4015 2006-05-03 02:52:18.000000 liblip-0.91/src/tnt_fortran_array1d_utils.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     4395 2006-05-03 02:52:18.000000 liblip-0.91/src/tnt_fortran_array2d.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     4050 2006-05-03 02:52:18.000000 liblip-0.91/src/tnt_fortran_array2d_utils.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     4489 2006-05-03 02:52:18.000000 liblip-0.91/src/tnt_fortran_array3d.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     4676 2006-05-03 02:52:18.000000 liblip-0.91/src/tnt_fortran_array3d_utils.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     4392 2006-05-03 02:52:18.000000 liblip-0.91/src/tnt_i_refvec.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)      913 2021-11-01 00:39:36.000000 liblip-0.91/src/tnt_math_utils.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     2805 2022-06-17 02:50:12.000000 liblip-0.91/src/tnt_sparse_matrix_csr 5.54.44 pm 5.54.44 pm.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     2805 2022-06-17 02:50:12.000000 liblip-0.91/src/tnt_sparse_matrix_csr.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     1713 2006-05-03 02:52:18.000000 liblip-0.91/src/tnt_stopwatch.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     1565 2006-05-03 02:52:18.000000 liblip-0.91/src/tnt_subscript.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     7175 2006-05-03 02:52:18.000000 liblip-0.91/src/tnt_vec.h
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     1042 2006-05-03 02:52:18.000000 liblip-0.91/src/tnt_version.h
+drwxr-xr-x   0 nhenseler   (501) staff       (20)        0 2023-04-13 07:18:37.966961 liblip-0.91/tests/
+drwxr-xr-x   0 nhenseler   (501) staff       (20)        0 2023-04-13 07:18:38.013444 liblip-0.91/tests/.ipynb_checkpoints/
+-rw-r--r--   0 nhenseler   (501) staff       (20)   558003 2022-07-22 06:01:37.000000 liblip-0.91/tests/.ipynb_checkpoints/test_wrapper_3d-checkpoint.ipynb
+-rw-r--r--   0 nhenseler   (501) staff       (20)     1766 2022-11-03 08:20:51.000000 liblip-0.91/tests/test_for_model_comparison.py
+-rw-r--r--   0 nhenseler   (501) staff       (20)     1932 2022-07-15 05:15:38.000000 liblip-0.91/tests/test_no_wrapper.py
+-rw-r--r--   0 nhenseler   (501) staff       (20)     1553 2023-03-08 04:28:17.000000 liblip-0.91/tests/test_performance.py
+-rw-r--r--   0 nhenseler   (501) staff       (20)    35649 2023-02-23 06:56:41.000000 liblip-0.91/tests/test_wrapper.py
+-rw-r--r--   0 nhenseler   (501) staff       (20)   541398 2022-07-25 09:58:53.000000 liblip-0.91/tests/test_wrapper_3d.ipynb
```

### Comparing `liblip-0.90/LICENSE.txt` & `liblip-0.91/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `liblip-0.90/PKG-INFO` & `liblip-0.91/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liblip
-Version: 0.90
+Version: 0.91
 Summary: Library for multivariate scattered data interpolation
 Home-page: UNKNOWN
 Author: Gleb Beliakov, Norbert Henseler
 Author-email: gleb.beliakov@deakin.edu.au, norbert.henseler@deakin.edu.au
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `liblip-0.90/README.md` & `liblip-0.91/README.md`

 * *Files identical despite different names*

### Comparing `liblip-0.90/docs/liblip2.pdf` & `liblip-0.91/docs/liblip2.pdf`

 * *Files identical despite different names*

### Comparing `liblip-0.90/setup.py` & `liblip-0.91/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup( 
     name="liblip",
-    version="0.90",
+    version="0.91",
     description="Library for multivariate scattered data interpolation",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="",
     author='Gleb Beliakov, Norbert Henseler',
     author_email='gleb.beliakov@deakin.edu.au, norbert.henseler@deakin.edu.au',
     license_file='LICENSE.txt',
```

### Comparing `liblip-0.90/src/build_liblip.nh.py` & `liblip-0.91/src/build_liblip.nh.py`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/build_liblip.py` & `liblip-0.91/src/build_liblip.bak.py`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/dliblip.h` & `liblip-0.91/src/dliblip.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/forest.cpp` & `liblip-0.91/src/forest.cpp`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/forest.h` & `liblip-0.91/src/forest.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpavl.c` & `liblip-0.91/src/glpavl.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpavl.h` & `liblip-0.91/src/glpavl.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpbfi.c` & `liblip-0.91/src/glpbfi.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpbfi.h` & `liblip-0.91/src/glpbfi.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpdmp.c` & `liblip-0.91/src/glpdmp.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpdmp.h` & `liblip-0.91/src/glpdmp.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glphbm.c` & `liblip-0.91/src/glphbm.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glphbm.h` & `liblip-0.91/src/glphbm.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpiet.c` & `liblip-0.91/src/glpiet.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpiet.h` & `liblip-0.91/src/glpiet.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpinv.c` & `liblip-0.91/src/glpinv.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpinv.h` & `liblip-0.91/src/glpinv.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpios.h` & `liblip-0.91/src/glpios.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpios1.c` & `liblip-0.91/src/glpios1.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpios2.c` & `liblip-0.91/src/glpios2.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpios3.c` & `liblip-0.91/src/glpios3.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpipm.c` & `liblip-0.91/src/glpipm.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpipm.h` & `liblip-0.91/src/glpipm.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpipp.h` & `liblip-0.91/src/glpipp.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpipp1.c` & `liblip-0.91/src/glpipp1.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpipp2.c` & `liblip-0.91/src/glpipp2.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpk.h` & `liblip-0.91/src/glpk.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glplib.h` & `liblip-0.91/src/glplib.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glplib1a.c` & `liblip-0.91/src/glplib1a.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glplib1b.c` & `liblip-0.91/src/glplib1b.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glplib2.c` & `liblip-0.91/src/glplib2.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glplib3.c` & `liblip-0.91/src/glplib3.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glplib4.c` & `liblip-0.91/src/glplib4.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glplpp.h` & `liblip-0.91/src/glplpp.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glplpp1.c` & `liblip-0.91/src/glplpp1.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glplpp2.c` & `liblip-0.91/src/glplpp2.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glplpx.h` & `liblip-0.91/src/glplpx.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glplpx1.c` & `liblip-0.91/src/glplpx1.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glplpx2.c` & `liblip-0.91/src/glplpx2.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glplpx3.c` & `liblip-0.91/src/glplpx3.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glplpx4.c` & `liblip-0.91/src/glplpx4.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glplpx5.c` & `liblip-0.91/src/glplpx5.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glplpx6a.c` & `liblip-0.91/src/glplpx6a.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glplpx6b.c` & `liblip-0.91/src/glplpx6b.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glplpx6c.c` & `liblip-0.91/src/glplpx6c.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glplpx6d.c` & `liblip-0.91/src/glplpx6d.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glplpx7.c` & `liblip-0.91/src/glplpx7.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glplpx7a.c` & `liblip-0.91/src/glplpx7a.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glplpx7b.c` & `liblip-0.91/src/glplpx7b.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glplpx8a.c` & `liblip-0.91/src/glplpx8a.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glplpx8b.c` & `liblip-0.91/src/glplpx8b.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glplpx8c.c` & `liblip-0.91/src/glplpx8c.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glplpx8d.c` & `liblip-0.91/src/glplpx8d.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glplpx8e.c` & `liblip-0.91/src/glplpx8e.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpluf.c` & `liblip-0.91/src/glpluf.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpluf.h` & `liblip-0.91/src/glpluf.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpmat.c` & `liblip-0.91/src/glpmat.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpmat.h` & `liblip-0.91/src/glpmat.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpmip.h` & `liblip-0.91/src/glpmip.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpmip1.c` & `liblip-0.91/src/glpmip1.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpmip2.c` & `liblip-0.91/src/glpmip2.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpmpl.h` & `liblip-0.91/src/glpmpl.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpmpl1.c` & `liblip-0.91/src/glpmpl1.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpmpl2.c` & `liblip-0.91/src/glpmpl2.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpmpl3.c` & `liblip-0.91/src/glpmpl3.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpmpl4.c` & `liblip-0.91/src/glpmpl4.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpqmd.c` & `liblip-0.91/src/glpqmd.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpqmd.h` & `liblip-0.91/src/glpqmd.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glprng.c` & `liblip-0.91/src/glprng.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glprng.h` & `liblip-0.91/src/glprng.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpspx.h` & `liblip-0.91/src/glpspx.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpspx1.c` & `liblip-0.91/src/glpspx1.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpspx2.c` & `liblip-0.91/src/glpspx2.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpstr.c` & `liblip-0.91/src/glpstr.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glpstr.h` & `liblip-0.91/src/glpstr.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glptsp.c` & `liblip-0.91/src/glptsp.c`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/glptsp.h` & `liblip-0.91/src/glptsp.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/interpol.cpp` & `liblip-0.91/src/interpol.cpp`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/interpol.h` & `liblip-0.91/src/interpol.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/jama_cholesky.h` & `liblip-0.91/src/jama_cholesky.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/jama_eig.h` & `liblip-0.91/src/jama_eig.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/jama_lu.h` & `liblip-0.91/src/jama_lu.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/jama_qr.h` & `liblip-0.91/src/jama_qr.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/jama_svd.h` & `liblip-0.91/src/jama_svd.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/liblip values.h` & `liblip-0.91/src/liblip values.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/liblip.cpp` & `liblip-0.91/src/liblip.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -185,15 +185,27 @@
 	return umgl.at( id)->Value(umgl.at( id)->Dim-1,x); // need to compute the slack variable 
 }
 
 LIBEXP  double	STCValueExplicit( int id, double* x )
 {
 	return umgl.at( id)->ValueExplicit(umgl.at( id)->Dim-1,x);
 }
+LIBEXP  double	STCValues( int id, double* x ,  int num, double* results)
+{
+for (int i=0;i<num;i++) 	
+	results[i] = umgl.at( id)->Value( (umgl.at( id)->Dim-1), x+ i*(umgl.at( id)->Dim-1));  
+return results[num-1];	
+}
 
+LIBEXP  double	STCValuesExplicit( int id, double* x , int num, double* results)
+{
+	for (int i=0;i<num;i++) 	
+	results[i] = umgl.at( id)->ValueExplicit( umgl.at( id)->Dim-1, x+ i* (umgl.at( id)->Dim-1));  
+return results[num-1];
+}
 
 LIBEXP  void	STCFreeMemory( int id) {umgl.at( id)->FreeMemory();}
 
 // additional functions
 LIBEXP void LipIntConstruct( int id)
 {
 	umgl.at( id)->Construct();
@@ -220,44 +232,85 @@
 }
 
 LIBEXP double LipIntValueDim( int id, int dim, double* x)
 {
 	return umgl.at( id)->Value( dim, x);
 }
 
+LIBEXP double LipIntValuesExplicitDim( int id, int dim, double* x, int num, double* results)
+{
+for (int i=0;i<num;i++) 	
+	results[i] = umgl.at( id)->ValueExplicit( dim, x+ i* dim);  
+return results[num-1];		
+
+}
+
+LIBEXP double LipIntValuesDim( int id, int dim, double* x, int num, double* results)
+{
+for (int i=0;i<num;i++) 	
+	results[i] = umgl.at( id)->Value( dim, x+ i* dim);  
+return results[num-1];	
+}
+
 LIBEXP void LipIntSetData( int id, int dim, int K, double* x, double* y, int test)
 {
 	umgl.at( id)->SetData( dim, K, x, y, test);
 }
 
 
 /*--------------------------------------------------------*/
 /* interface to the members of SLipInt class */
 
 LIBEXP double	LipIntValues( int id, int *Dim, int *Ndata, double* x, double* Xd,double* y,  double* Lipconst, int* Index, int num, double* results)
 { for (int i=0;i<num;i++) 	
-	results[i] = umsli.at( id)->Value(*Dim, *Ndata, x+ i* sizeof(double)* *Dim, Xd, y, *Lipconst, Index); 
+	results[i] = umsli.at( id)->Value(*Dim, *Ndata, x+ i* *Dim, Xd, y, *Lipconst, Index); 
 return results[num-1];
 }
 
 LIBEXP double	LipIntValue( int id, int *Dim, int *Ndata, double* x, double* Xd,double* y,  double* Lipconst, int* Index)
 { return umsli.at( id)->Value(*Dim, *Ndata, x, Xd, y, *Lipconst, Index); }
 
 LIBEXP double	LipIntValueAuto( int id, int *Dim, int *Ndata, double* x,double* Xd, double* y, int* Index)
 { return umsli.at( id)->Value(*Dim, *Ndata, x, Xd,y, Index); }
 
+LIBEXP double	LipIntValuesAuto( int id, int *Dim, int *Ndata, double* x,double* Xd, double* y, int* Index, int num, double* results)
+{	for (int i=0;i<num;i++) 	
+	results[i] = umsli.at( id)->Value(*Dim, *Ndata, x+ i*  *Dim, Xd,y, Index);  
+return results[num-1];
+
+}
+
 LIBEXP double	LipIntValueCons( int id, int* Dim, int* Ndata, int* Cons, double* x, double* Xd,double* y,  double* Lipconst, int* Index)
 { return umsli.at( id)->ValueCons(*Dim, *Ndata, Cons, x, Xd, y, *Lipconst, Index); }
 
-LIBEXP double	LipIntValueConsLeftRegion( int id, int* Dim, int* Ndata, int* Cons, double* x, double* Xd,double* y,  double* Lipconst, double* Region, int* Index)
+LIBEXP double	LipIntValuesCons( int id, int* Dim, int* Ndata, int* Cons, double* x, double* Xd,double* y,  double* Lipconst, int* Index, int num, double* results)
+{for (int i=0;i<num;i++) 	
+	results[i] = umsli.at( id)->ValueCons(*Dim, *Ndata, Cons, x+ i*  *Dim, Xd,y, *Lipconst, Index);  
+return results[num-1];
+ }
+
+LIBEXP double	LipIntValuesConsLeftRegion( int id, int* Dim, int* Ndata, int* Cons, double* x, double* Xd,double* y,  double* Lipconst, double* Region, int* Index, int num, double* results)
+{for (int i=0;i<num;i++) 	
+	results[i] = umsli.at( id)->ValueConsLeftRegion(*Dim, *Ndata, Cons, x+ i*  *Dim, Xd,y, *Lipconst, Region, Index);  
+return results[num-1]; 
+}
+
+LIBEXP double	LipIntValueConsLeftRegion( int id, int* Dim, int* Ndata, int* Cons, double* x, double* Xd,double* y,  double* Lipconst, double* Region, int* Index, int num, double* results)
 { return umsli.at( id)->ValueConsLeftRegion( *Dim, *Ndata, Cons, x, Xd, y, *Lipconst, Region, Index); }
 
 LIBEXP double	LipIntValueConsRightRegion( int id, int* Dim, int* Ndata, int* Cons, double* x, double* Xd,double* y,  double* Lipconst, double* Region, int* Index)
 { return umsli.at( id)->ValueConsRightRegion( *Dim, *Ndata, Cons, x, Xd, y, *Lipconst, Region, Index); }
 
+LIBEXP double	LipIntValuesConsRightRegion( int id, int* Dim, int* Ndata, int* Cons, double* x, double* Xd,double* y,  double* Lipconst, double* Region, int* Index, int num, double* results)
+{ for (int i=0;i<num;i++) 	
+	results[i] = umsli.at( id)->ValueConsRightRegion(*Dim, *Ndata, Cons, x+ i* *Dim, Xd,y, *Lipconst, Region, Index);  
+return results[num-1];
+}
+
+
 
 LIBEXP double	LipIntValueLocal( int id, int* Dim, int* Ndata, double* x, double* Xd,double* y)
 { 
 	return umsli.at( id)->ValueLocal(*Dim, *Ndata, x, Xd,y);
 }
 
 LIBEXP double	LipIntValueLocalCons( int id, int* Dim, int* Ndata,int* Cons, double* x, double* Xd,double* y)
@@ -265,14 +318,41 @@
 
 LIBEXP double	LipIntValueLocalConsLeftRegion( int id, int* Dim, int* Ndata,int* Cons, double* x, double* Xd,double* y, double* Region)
 { return umsli.at( id)->ValueLocalConsLeftRegion(*Dim, *Ndata, Cons, x, Xd,y,Region); }
 
 LIBEXP double	LipIntValueLocalConsRightRegion( int id, int* Dim, int* Ndata,int* Cons, double* x, double* Xd,double* y, double* Region)
 { return umsli.at( id)->ValueLocalConsRightRegion(*Dim, *Ndata, Cons, x, Xd,y,Region); }
 
+LIBEXP double	LipIntValuesLocal( int id, int* Dim, int* Ndata, double* x, double* Xd,double* y, int num, double* results)
+{ 
+for (int i=0;i<num;i++) 	
+	results[i] = umsli.at( id)->ValueLocal(*Dim, *Ndata, x+ i*  *Dim, Xd,y);  
+return results[num-1];
+}
+
+LIBEXP double	LipIntValuesLocalCons( int id, int* Dim, int* Ndata,int* Cons, double* x, double* Xd,double* y, int num, double* results)
+{ 
+for (int i=0;i<num;i++) 	
+	results[i] = umsli.at( id)->ValueLocalCons(*Dim, *Ndata, Cons, x+ i*  *Dim, Xd,y);  
+return results[num-1];
+}
+
+LIBEXP double	LipIntValuesLocalConsLeftRegion( int id, int* Dim, int* Ndata,int* Cons, double* x, double* Xd,double* y, double* Region, int num, double* results)
+{ 
+for (int i=0;i<num;i++) 	
+	results[i] = umsli.at( id)->ValueLocalConsLeftRegion(*Dim, *Ndata, Cons, x+ i*  *Dim, Xd,y,Region);  
+return results[num-1];
+}
+
+LIBEXP double	LipIntValuesLocalConsRightRegion( int id, int* Dim, int* Ndata,int* Cons, double* x, double* Xd,double* y, double* Region, int num, double* results)
+{ for (int i=0;i<num;i++) 	
+	results[i] = umsli.at( id)->ValueLocalConsRightRegion(*Dim, *Ndata, Cons, x+ i*  *Dim, Xd,y,Region);  
+return results[num-1];
+}
+
 
 LIBEXP void	LipIntComputeLipschitz( int id, int* Dim, int* Ndata, double* x, double* y)
 {  umsli.at( id)->ComputeLipschitz(*Dim, *Ndata, x, y); }
 
 LIBEXP void	LipIntComputeLocalLipschitz(  int id, int* Dim, int* Ndata, double* x, double* y)
 { 	
 	umsli.at( id)->ComputeLocalLipschitz(*Dim, *Ndata, x, y);
@@ -356,17 +436,92 @@
 LIBEXP double	LipIntInfValueLocalConsLeftRegion( int id, int* Dim, int* Ndata,int* Cons, double* x, double* Xd,double* y, double* Region)
 { return umslii.at( id)->ValueLocalConsLeftRegion(*Dim, *Ndata, Cons, x, Xd,y,Region); }
 
 LIBEXP double	LipIntInfValueLocalConsRightRegion( int id, int* Dim, int* Ndata,int* Cons, double* x, double* Xd,double* y, double* Region)
 { return umslii.at( id)->ValueLocalConsRightRegion(*Dim, *Ndata, Cons, x, Xd,y,Region); }
 
 
+
+LIBEXP double	LipIntInfValues( int id, int* Dim, int* Ndata, double* x, double* Xd,double* y,  double* Lipconst, int* Index, int num, double* results)
+{
+	for (int i=0;i<num;i++) 	
+	results[i] = umslii.at( id)->Value(*Dim, *Ndata,  x+ i*  *Dim, Xd,y,*Lipconst, Index);  
+return results[num-1];
+}
+
+LIBEXP double	LipIntInfValuesAuto( int id, int* Dim, int* Ndata, double* x,double* Xd, double* y, int* Index, int num, double* results)
+{ 
+	for (int i=0;i<num;i++) 	
+	results[i] = umslii.at( id)->Value(*Dim, *Ndata,  x+ i*  *Dim, Xd,y, Index);  
+return results[num-1];
+}
+
+LIBEXP double	LipIntInfValuesCons( int id, int* Dim, int* Ndata, int* Cons, double* x, double* Xd,double* y,  double* Lipconst, int* Index, int num, double* results)
+{ 
+	for (int i=0;i<num;i++) 	
+	results[i] = umslii.at( id)->ValueCons(*Dim, *Ndata, Cons, x+ i*  *Dim, Xd,y,*Lipconst, Index);  
+return results[num-1];
+}
+
+LIBEXP double	LipIntInfValuesConsLeftRegion( int id, int* Dim, int* Ndata, int* Cons, double* x, double* Xd,double* y,  double* Lipconst, double* Region, int* Index, int num, double* results)
+{ 	for (int i=0;i<num;i++) 	
+	results[i] = umslii.at( id)->ValueConsLeftRegion(*Dim, *Ndata, Cons, x+ i*  *Dim, Xd,y,*Lipconst, Region, Index);  
+return results[num-1];
+}
+
+LIBEXP double	LipIntInfValuesConsRightRegion( int id, int* Dim, int* Ndata, int* Cons, double* x, double* Xd,double* y,  double* Lipconst, double* Region, int* Index, int num, double* results)
+{ 	for (int i=0;i<num;i++) 	
+	results[i] = umslii.at( id)->ValueConsRightRegion(*Dim, *Ndata, Cons, x+ i*  *Dim, Xd,y,*Lipconst, Region, Index);  
+return results[num-1];
+}
+
+				
+/*
+LIBEXP double	LipIntInfValueLocal( int id, int* Dim, int* Ndata, double* x, double* Xd,double* y)
+{ return umslii.at( id)->ValueLocal(*Dim, *Ndata, x, Xd,y); }
+
+LIBEXP double	LipIntInfValueLocalCons( int id, int *Dim, int* Ndata,int* Cons, double* x, double* Xd,double* y)
+{ return umslii.at( id)->ValueLocalCons(*Dim, *Ndata, Cons, x, Xd,y); }
+
+LIBEXP double	LipIntInfValueLocalConsLeftRegion( int id, int* Dim, int* Ndata,int* Cons, double* x, double* Xd,double* y, double* Region)
+{ return umslii.at( id)->ValueLocalConsLeftRegion(*Dim, *Ndata, Cons, x, Xd,y,Region); }
+
+LIBEXP double	LipIntInfValueLocalConsRightRegion( int id, int* Dim, int* Ndata,int* Cons, double* x, double* Xd,double* y, double* Region)
+{ return umslii.at( id)->ValueLocalConsRightRegion(*Dim, *Ndata, Cons, x, Xd,y,Region); }
+*/
+
+LIBEXP double	LipIntInfValuesLocal( int id, int* Dim, int* Ndata, double* x, double* Xd,double* y, int num, double* results)
+{ 
+ 	for (int i=0;i<num;i++) 	
+	results[i] = umslii.at( id)->ValueLocal(*Dim, *Ndata,  x+ i* *Dim, Xd,y);  
+return results[num-1];
+}
+
+LIBEXP double	LipIntInfValuesLocalCons( int id, int *Dim, int* Ndata,int* Cons, double* x, double* Xd,double* y, int num, double* results)
+{  	for (int i=0;i<num;i++) 	
+	results[i] = umslii.at( id)->ValueLocalCons(*Dim, *Ndata, Cons, x+ i*  *Dim, Xd,y);  
+return results[num-1];
+}
+
+LIBEXP double	LipIntInfValuesLocalConsLeftRegion( int id, int* Dim, int* Ndata,int* Cons, double* x, double* Xd,double* y, double* Region, int num, double* results)
+{  	for (int i=0;i<num;i++) 	
+	results[i] = umslii.at( id)->ValueLocalConsLeftRegion(*Dim, *Ndata, Cons, x+ i*  *Dim, Xd,y, Region);  
+return results[num-1];
+ }
+
+LIBEXP double	LipIntInfValuesLocalConsRightRegion( int id, int* Dim, int* Ndata,int* Cons, double* x, double* Xd,double* y, double* Region, int num, double* results)
+{  	for (int i=0;i<num;i++) 	
+	results[i] = umslii.at( id)->ValueLocalConsRightRegion(*Dim, *Ndata, Cons, x+ i*  *Dim, Xd,y, Region);  
+return results[num-1];
+}
+
+
 LIBEXP void	LipIntInfComputeLipschitz( int id, int* Dim, int* Ndata, double* x, double* y)
 {  
-	std::cout << "LipIntInfComputeLipschitz: " << id << std::endl;
+//	std::cout << "LipIntInfComputeLipschitz: " << id << std::endl;
 	umslii.at( id)->ComputeLipschitz(*Dim, *Ndata, x, y); }
 
 LIBEXP void	LipIntInfComputeLocalLipschitz(int id, int* Dim, int* Ndata, double* x, double* y)
 { 
 	umslii.at( id)->ComputeLocalLipschitz(*Dim, *Ndata, x, y);
 }
```

### Comparing `liblip-0.90/src/liblip.egg-info/.DS_Store` & `liblip-0.91/src/liblip.egg-info/.DS_Store`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/liblip.egg-info/PKG-INFO` & `liblip-0.91/src/liblip.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liblip
-Version: 0.90
+Version: 0.91
 Summary: Library for multivariate scattered data interpolation
 Home-page: UNKNOWN
 Author: Gleb Beliakov, Norbert Henseler
 Author-email: gleb.beliakov@deakin.edu.au, norbert.henseler@deakin.edu.au
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `liblip-0.90/src/liblip.egg-info/SOURCES.txt` & `liblip-0.91/src/liblip.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 setup.py
-dist/liblip-0.90-cp39-cp39-macosx_10_9_x86_64.whl
+dist/liblip-0.91-cp39-cp39-macosx_10_9_x86_64.whl
 docs/liblip2.pdf
+src/build_liblip.bak.py
 src/build_liblip.nh.py
 src/build_liblip.py
 src/dliblip.h
 src/forest.cpp
 src/forest.h
 src/glpavl.c
 src/glpavl.h
@@ -85,14 +86,16 @@
 src/interpol.h
 src/jama_cholesky.h
 src/jama_eig.h
 src/jama_lu.h
 src/jama_qr.h
 src/jama_svd.h
 src/liblip values.h
+src/liblip.bak.h
+src/liblip.bak.py
 src/liblip.cpp
 src/liblip.h
 src/liblip.nh.h
 src/liblip.py
 src/liblipc.h
 src/memblock.h
 src/slipint.cpp
```

### Comparing `liblip-0.90/src/liblip.h` & `liblip-0.91/src/liblip.bak.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/liblip.nh.h` & `liblip-0.91/src/liblip.nh.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/liblip.py` & `liblip-0.91/src/liblip.bak.py`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/memblock.h` & `liblip-0.91/src/memblock.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/slipint.cpp` & `liblip-0.91/src/slipint.cpp`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/slipint.h` & `liblip-0.91/src/slipint.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/tnt.h` & `liblip-0.91/src/tnt.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/tnt_array1d.h` & `liblip-0.91/src/tnt_array1d.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/tnt_array1d_utils.h` & `liblip-0.91/src/tnt_array1d_utils.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/tnt_array2d.h` & `liblip-0.91/src/tnt_array2d.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/tnt_array2d_utils.h` & `liblip-0.91/src/tnt_array2d_utils.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/tnt_array3d.h` & `liblip-0.91/src/tnt_array3d.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/tnt_array3d_utils.h` & `liblip-0.91/src/tnt_array3d_utils.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/tnt_cmat.h` & `liblip-0.91/src/tnt_cmat.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/tnt_fortran_array1d.h` & `liblip-0.91/src/tnt_fortran_array1d.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/tnt_fortran_array1d_utils.h` & `liblip-0.91/src/tnt_fortran_array1d_utils.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/tnt_fortran_array2d.h` & `liblip-0.91/src/tnt_fortran_array2d.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/tnt_fortran_array2d_utils.h` & `liblip-0.91/src/tnt_fortran_array2d_utils.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/tnt_fortran_array3d.h` & `liblip-0.91/src/tnt_fortran_array3d.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/tnt_fortran_array3d_utils.h` & `liblip-0.91/src/tnt_fortran_array3d_utils.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/tnt_i_refvec.h` & `liblip-0.91/src/tnt_i_refvec.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/tnt_math_utils.h` & `liblip-0.91/src/tnt_math_utils.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/tnt_sparse_matrix_csr 5.54.44 pm 5.54.44 pm.h` & `liblip-0.91/src/tnt_sparse_matrix_csr 5.54.44 pm 5.54.44 pm.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/tnt_sparse_matrix_csr.h` & `liblip-0.91/src/tnt_sparse_matrix_csr.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/tnt_stopwatch.h` & `liblip-0.91/src/tnt_stopwatch.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/tnt_subscript.h` & `liblip-0.91/src/tnt_subscript.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/tnt_vec.h` & `liblip-0.91/src/tnt_vec.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/src/tnt_version.h` & `liblip-0.91/src/tnt_version.h`

 * *Files identical despite different names*

### Comparing `liblip-0.90/tests/.ipynb_checkpoints/test_wrapper_3d-checkpoint.ipynb` & `liblip-0.91/tests/.ipynb_checkpoints/test_wrapper_3d-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `liblip-0.90/tests/test_for_model_comparison.py` & `liblip-0.91/tests/test_for_model_comparison.py`

 * *Files identical despite different names*

### Comparing `liblip-0.90/tests/test_no_wrapper.py` & `liblip-0.91/tests/test_no_wrapper.py`

 * *Files identical despite different names*

### Comparing `liblip-0.90/tests/test_performance.py` & `liblip-0.91/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `liblip-0.90/tests/test_wrapper.py` & `liblip-0.91/tests/test_wrapper.py`

 * *Files identical despite different names*

### Comparing `liblip-0.90/tests/test_wrapper_3d.ipynb` & `liblip-0.91/tests/test_wrapper_3d.ipynb`

 * *Files identical despite different names*

