# Comparing `tmp/pyxtal-0.5.8.tar.gz` & `tmp/pyxtal-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/qiangzhu/Desktop/github/PyXtal/dist/.tmp-26n5y_i3/pyxtal-0.5.8.tar", last modified: Sat Jul  8 02:39:13 2023, max compression
+gzip compressed data, was "/Users/qiangzhu/Desktop/github/PyXtal/dist/.tmp-zuebty0n/pyxtal-0.5.9.tar", last modified: Sat Jul 22 21:47:58 2023, max compression
```

## Comparing `pyxtal-0.5.8.tar` & `pyxtal-0.5.9.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-07-08 02:39:13.000000 pyxtal-0.5.8/
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1084 2022-06-13 19:36:20.000000 pyxtal-0.5.8/LICENSE.txt
--rwxr-xr-x   0 qiangzhu   (501) staff       (20)       83 2023-07-08 00:55:55.000000 pyxtal-0.5.8/MANIFEST.in
--rw-r--r--   0 qiangzhu   (501) staff       (20)     5203 2023-07-08 02:39:13.000000 pyxtal-0.5.8/PKG-INFO
--rw-r--r--   0 qiangzhu   (501) staff       (20)     4692 2022-07-27 22:43:15.000000 pyxtal-0.5.8/README.md
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-07-08 02:39:13.000000 pyxtal-0.5.8/pyxtal/
--rw-r--r--   0 qiangzhu   (501) staff       (20)    31648 2022-08-14 23:14:59.000000 pyxtal-0.5.8/pyxtal/XRD.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)   105417 2023-07-08 02:10:23.000000 pyxtal-0.5.8/pyxtal/__init__.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     5985 2022-06-21 15:19:36.000000 pyxtal-0.5.8/pyxtal/block_crystal.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1784 2022-06-23 22:59:32.000000 pyxtal-0.5.8/pyxtal/constants.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    13810 2022-06-21 13:41:23.000000 pyxtal-0.5.8/pyxtal/crystal.py
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-07-08 02:39:13.000000 pyxtal-0.5.8/pyxtal/database/
--rw-r--r--   0 qiangzhu   (501) staff       (20)    22281 2022-06-17 19:11:39.000000 pyxtal-0.5.8/pyxtal/database/HM_Full.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)        0 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/__init__.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     6824 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/atomic_scattering_params.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2120 2022-08-11 19:04:42.000000 pyxtal-0.5.8/pyxtal/database/bonds.json
--rw-------   0 qiangzhu   (501) staff       (20)     2950 2022-01-27 19:42:36.000000 pyxtal-0.5.8/pyxtal/database/bug.json
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-07-08 02:39:13.000000 pyxtal-0.5.8/pyxtal/database/cifs/
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2051 2021-12-27 22:37:10.000000 pyxtal-0.5.8/pyxtal/database/cifs/0-G62.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1921 2021-11-09 00:08:43.000000 pyxtal-0.5.8/pyxtal/database/cifs/1-G59.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      367 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/191.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2043 2021-12-27 00:51:46.000000 pyxtal-0.5.8/pyxtal/database/cifs/2-G71.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2373 2021-12-27 00:21:38.000000 pyxtal-0.5.8/pyxtal/database/cifs/3-G139.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     5688 2021-11-09 00:08:43.000000 pyxtal-0.5.8/pyxtal/database/cifs/4-G225.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2940 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/ACBNZA01.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     9863 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/AXOSOW01.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1184 2022-04-27 19:27:52.000000 pyxtal-0.5.8/pyxtal/database/cifs/Al2SiO5_mp-4753_symmetrized.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1009 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/BTO-Amm2.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1323 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/BTO.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1534 2022-04-28 13:54:25.000000 pyxtal-0.5.8/pyxtal/database/cifs/CuAu_mp-582681_symmetrized.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     4636 2022-06-17 15:45:22.000000 pyxtal-0.5.8/pyxtal/database/cifs/FAU.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     3542 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/database/cifs/Fd3.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     6258 2022-06-17 19:14:34.000000 pyxtal-0.5.8/pyxtal/database/cifs/Fd3.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)     4992 2021-12-29 18:59:05.000000 pyxtal-0.5.8/pyxtal/database/cifs/Fd3m.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     9559 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/GUMMUW.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      885 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/GeF2.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2946 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/HAHCOI.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      221 2022-06-17 19:31:24.000000 pyxtal-0.5.8/pyxtal/database/cifs/I41amd.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1836 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/database/cifs/I4_132.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)    10505 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/JAPWIH.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)   441469 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/LAGNAL.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     7132 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/LUFHAW.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2001 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/LiCs.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)    12413 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/MERQIM.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1238 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/MPWO.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     4577 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/NaCl.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1416 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/NaSb3F10.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1180 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/NbO2.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1696 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/NiS-Cm.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1134 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/database/cifs/P3_112.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1498 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/database/cifs/P4_332.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      226 2022-06-17 19:18:01.000000 pyxtal-0.5.8/pyxtal/database/cifs/P4nmm.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1205 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/database/cifs/P6_422.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     6482 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/PAHYON01.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1184 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/PPO.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1086 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/PVO.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1222 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/database/cifs/Pm3.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      230 2022-06-17 19:19:37.000000 pyxtal-0.5.8/pyxtal/database/cifs/Pmmn.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)      286 2022-06-17 19:13:51.000000 pyxtal-0.5.8/pyxtal/database/cifs/Pn3.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)      286 2022-06-17 19:13:21.000000 pyxtal-0.5.8/pyxtal/database/cifs/Pn3m.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1605 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/database/cifs/R-3.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1933 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/database/cifs/R-3c.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      986 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/database/cifs/R32.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     3542 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/TMPPIO03.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)    13289 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/WEXBOS.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)   177150 2022-06-17 20:12:44.000000 pyxtal-0.5.8/pyxtal/database/cifs/YICMOP.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)        0 2023-07-08 02:10:33.000000 pyxtal-0.5.8/pyxtal/database/cifs/__init__.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2546 2022-07-27 19:22:51.000000 pyxtal-0.5.8/pyxtal/database/cifs/anthracene.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2703 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/aspirin-c.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)    12951 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/aspirin.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1509 2022-07-27 00:49:00.000000 pyxtal-0.5.8/pyxtal/database/cifs/benzene.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      733 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/bug.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)    17895 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/coumarin.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2260 2022-01-18 15:40:54.000000 pyxtal-0.5.8/pyxtal/database/cifs/dist_6_0.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2260 2022-01-18 15:40:53.000000 pyxtal-0.5.8/pyxtal/database/cifs/dist_6_1.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     7884 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/gdh.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1964 2022-08-22 20:08:21.000000 pyxtal-0.5.8/pyxtal/database/cifs/ht_KNbBO.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     5997 2022-08-22 18:10:54.000000 pyxtal-0.5.8/pyxtal/database/cifs/ht_cristobalite.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1251 2022-08-22 18:21:32.000000 pyxtal-0.5.8/pyxtal/database/cifs/ht_quartz.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1864 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/ice.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2869 2022-08-22 20:08:21.000000 pyxtal-0.5.8/pyxtal/database/cifs/lt_KNbBO.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      931 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/lt_cristobalite.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      866 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/lt_quartz.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1541 2022-07-27 00:49:34.000000 pyxtal-0.5.8/pyxtal/database/cifs/naphthalene.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)   317844 2021-11-23 20:29:41.000000 pyxtal-0.5.8/pyxtal/database/cifs/resorcinol.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      473 2022-01-21 16:08:56.000000 pyxtal-0.5.8/pyxtal/database/cifs/sim-0.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)      488 2022-01-21 16:08:55.000000 pyxtal-0.5.8/pyxtal/database/cifs/sim-1.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)     4786 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/xxvi.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)  1103778 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/clusters.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2617 2022-06-23 00:39:04.000000 pyxtal-0.5.8/pyxtal/database/collection.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    19164 2022-06-14 14:22:59.000000 pyxtal-0.5.8/pyxtal/database/element.py
--rw-r--r--   0 qiangzhu   (501) staff       (20) 10480157 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/k_subgroup.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)    20717 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/layer.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)    25842 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/layer_generators.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)    58872 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/layer_symmetry.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)    90734 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/molecules.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)   130892 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/point.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)   146327 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/point_generators.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)   301944 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/point_symmetry.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)    18501 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/rod.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)    21935 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/rod_generators.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)    44320 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/rod_symmetry.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)     5478 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/symbols.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)  1245398 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/t_subgroup.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)   259897 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/wyckoff_generators.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)   251719 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/wyckoff_list.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)   117892 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/database/wyckoff_sets.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)   627207 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/database/wyckoff_symmetry.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)     8405 2023-06-28 06:05:35.000000 pyxtal-0.5.8/pyxtal/db.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    18843 2023-07-08 02:00:23.000000 pyxtal-0.5.8/pyxtal/descriptor.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    42770 2023-04-04 17:06:21.000000 pyxtal-0.5.8/pyxtal/elasticity.py
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-07-08 02:39:13.000000 pyxtal-0.5.8/pyxtal/interface/
--rw-r--r--   0 qiangzhu   (501) staff       (20)    13515 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/interface/LJ.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)        0 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/interface/__init__.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    27602 2023-07-01 12:59:09.000000 pyxtal-0.5.8/pyxtal/interface/dftb.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    14489 2023-06-23 09:35:50.000000 pyxtal-0.5.8/pyxtal/interface/gulp.py
--rwxr-xr-x   0 qiangzhu   (501) staff       (20)    19477 2022-01-06 13:19:42.000000 pyxtal-0.5.8/pyxtal/interface/lammpslib.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     8403 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/interface/vasp.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    31490 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/interface/vasprun.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    23034 2022-09-24 05:16:49.000000 pyxtal-0.5.8/pyxtal/io.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    67553 2023-06-22 22:47:40.000000 pyxtal-0.5.8/pyxtal/lattice.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    18090 2023-07-08 01:32:18.000000 pyxtal-0.5.8/pyxtal/molecular_crystal.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    63216 2022-11-18 06:08:23.000000 pyxtal-0.5.8/pyxtal/molecule.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2758 2022-08-09 01:18:08.000000 pyxtal-0.5.8/pyxtal/msg.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    30344 2023-06-23 21:31:46.000000 pyxtal-0.5.8/pyxtal/operations.py
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-07-08 02:39:13.000000 pyxtal-0.5.8/pyxtal/optimize/
--rw-r--r--   0 qiangzhu   (501) staff       (20)        0 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/optimize/__init__.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     5636 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/optimize/fire.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    12084 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/optimize/fire2.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    14967 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/optimize/myscipy_optimize.py
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-07-08 02:39:13.000000 pyxtal-0.5.8/pyxtal/potentials/
--rw-r--r--   0 qiangzhu   (501) staff       (20)  1820580 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/potentials/CuAg.eam.alloy
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1652 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/potentials/LJ_cluster.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)      837 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/potentials/Si.tersoff
--rw-r--r--   0 qiangzhu   (501) staff       (20)     3991 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/potentials/SiCGe.tersoff
--rwxr-xr-x   0 qiangzhu   (501) staff       (20)       26 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/potentials/__init__.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    16972 2023-06-23 22:45:29.000000 pyxtal-0.5.8/pyxtal/representation.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    46380 2023-06-05 08:59:34.000000 pyxtal-0.5.8/pyxtal/supergroup.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)   130447 2023-06-24 19:46:55.000000 pyxtal-0.5.8/pyxtal/symmetry.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    43692 2023-07-08 02:00:44.000000 pyxtal-0.5.8/pyxtal/test_all.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    11061 2023-07-08 00:51:34.000000 pyxtal-0.5.8/pyxtal/tolerance.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    17663 2023-06-25 10:12:42.000000 pyxtal-0.5.8/pyxtal/util.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)       22 2023-07-08 00:52:50.000000 pyxtal-0.5.8/pyxtal/version.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    13329 2022-09-09 18:39:24.000000 pyxtal-0.5.8/pyxtal/viz.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    40631 2023-07-08 01:50:50.000000 pyxtal-0.5.8/pyxtal/wyckoff_site.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    21212 2023-06-05 08:57:39.000000 pyxtal-0.5.8/pyxtal/wyckoff_split.py
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-07-08 02:39:13.000000 pyxtal-0.5.8/pyxtal.egg-info/
--rw-r--r--   0 qiangzhu   (501) staff       (20)     5203 2023-07-08 02:39:13.000000 pyxtal-0.5.8/pyxtal.egg-info/PKG-INFO
--rw-r--r--   0 qiangzhu   (501) staff       (20)     4250 2023-07-08 02:39:13.000000 pyxtal-0.5.8/pyxtal.egg-info/SOURCES.txt
--rw-r--r--   0 qiangzhu   (501) staff       (20)        1 2023-07-08 02:39:13.000000 pyxtal-0.5.8/pyxtal.egg-info/dependency_links.txt
--rw-r--r--   0 qiangzhu   (501) staff       (20)      160 2023-07-08 02:39:13.000000 pyxtal-0.5.8/pyxtal.egg-info/requires.txt
--rw-r--r--   0 qiangzhu   (501) staff       (20)        7 2023-07-08 02:39:13.000000 pyxtal-0.5.8/pyxtal.egg-info/top_level.txt
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-07-08 02:39:13.000000 pyxtal-0.5.8/scripts/
--rwxr-xr-x   0 qiangzhu   (501) staff       (20)     4296 2023-06-27 08:23:49.000000 pyxtal-0.5.8/scripts/pyxtal_main.py
--rwxr-xr-x   0 qiangzhu   (501) staff       (20)      960 2021-08-17 15:48:09.000000 pyxtal-0.5.8/scripts/pyxtal_symmetry.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)      125 2023-07-08 02:39:13.000000 pyxtal-0.5.8/setup.cfg
--rwxr-xr-x   0 qiangzhu   (501) staff       (20)     1798 2023-07-08 00:50:33.000000 pyxtal-0.5.8/setup.py
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-07-22 21:47:58.000000 pyxtal-0.5.9/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1084 2022-06-13 19:36:20.000000 pyxtal-0.5.9/LICENSE.txt
+-rwxr-xr-x   0 qiangzhu   (501) staff       (20)       83 2023-07-08 00:55:55.000000 pyxtal-0.5.9/MANIFEST.in
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     5203 2023-07-22 21:47:58.000000 pyxtal-0.5.9/PKG-INFO
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     4692 2022-07-27 22:43:15.000000 pyxtal-0.5.9/README.md
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-07-22 21:47:58.000000 pyxtal-0.5.9/pyxtal/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    31648 2022-08-14 23:14:59.000000 pyxtal-0.5.9/pyxtal/XRD.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   106149 2023-07-18 21:26:38.000000 pyxtal-0.5.9/pyxtal/__init__.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     5985 2022-06-21 15:19:36.000000 pyxtal-0.5.9/pyxtal/block_crystal.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1784 2022-06-23 22:59:32.000000 pyxtal-0.5.9/pyxtal/constants.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    13810 2023-07-18 15:07:44.000000 pyxtal-0.5.9/pyxtal/crystal.py
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-07-22 21:47:58.000000 pyxtal-0.5.9/pyxtal/database/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    22281 2022-06-17 19:11:39.000000 pyxtal-0.5.9/pyxtal/database/HM_Full.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)        0 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/__init__.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     6824 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/atomic_scattering_params.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2120 2022-08-11 19:04:42.000000 pyxtal-0.5.9/pyxtal/database/bonds.json
+-rw-------   0 qiangzhu   (501) staff       (20)     2950 2022-01-27 19:42:36.000000 pyxtal-0.5.9/pyxtal/database/bug.json
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-07-22 21:47:58.000000 pyxtal-0.5.9/pyxtal/database/cifs/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2051 2021-12-27 22:37:10.000000 pyxtal-0.5.9/pyxtal/database/cifs/0-G62.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1921 2021-11-09 00:08:43.000000 pyxtal-0.5.9/pyxtal/database/cifs/1-G59.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      367 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/191.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2043 2021-12-27 00:51:46.000000 pyxtal-0.5.9/pyxtal/database/cifs/2-G71.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2373 2021-12-27 00:21:38.000000 pyxtal-0.5.9/pyxtal/database/cifs/3-G139.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     5688 2021-11-09 00:08:43.000000 pyxtal-0.5.9/pyxtal/database/cifs/4-G225.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2940 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/ACBNZA01.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     9863 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/AXOSOW01.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1184 2022-04-27 19:27:52.000000 pyxtal-0.5.9/pyxtal/database/cifs/Al2SiO5_mp-4753_symmetrized.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1009 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/BTO-Amm2.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1323 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/BTO.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1534 2022-04-28 13:54:25.000000 pyxtal-0.5.9/pyxtal/database/cifs/CuAu_mp-582681_symmetrized.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     4636 2022-06-17 15:45:22.000000 pyxtal-0.5.9/pyxtal/database/cifs/FAU.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     3542 2021-08-17 15:48:09.000000 pyxtal-0.5.9/pyxtal/database/cifs/Fd3.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     6258 2022-06-17 19:14:34.000000 pyxtal-0.5.9/pyxtal/database/cifs/Fd3.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     4992 2021-12-29 18:59:05.000000 pyxtal-0.5.9/pyxtal/database/cifs/Fd3m.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     9559 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/GUMMUW.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      885 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/GeF2.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2946 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/HAHCOI.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      221 2022-06-17 19:31:24.000000 pyxtal-0.5.9/pyxtal/database/cifs/I41amd.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1836 2021-08-17 15:48:09.000000 pyxtal-0.5.9/pyxtal/database/cifs/I4_132.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    10505 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/JAPWIH.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   441469 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/LAGNAL.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     7132 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/LUFHAW.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2001 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/LiCs.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    12413 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/MERQIM.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1238 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/MPWO.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     4577 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/NaCl.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1416 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/NaSb3F10.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1180 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/NbO2.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1696 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/NiS-Cm.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1134 2021-08-17 15:48:09.000000 pyxtal-0.5.9/pyxtal/database/cifs/P3_112.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1498 2021-08-17 15:48:09.000000 pyxtal-0.5.9/pyxtal/database/cifs/P4_332.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      226 2022-06-17 19:18:01.000000 pyxtal-0.5.9/pyxtal/database/cifs/P4nmm.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1205 2021-08-17 15:48:09.000000 pyxtal-0.5.9/pyxtal/database/cifs/P6_422.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     6482 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/PAHYON01.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1184 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/PPO.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1086 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/PVO.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1222 2021-08-17 15:48:09.000000 pyxtal-0.5.9/pyxtal/database/cifs/Pm3.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      230 2022-06-17 19:19:37.000000 pyxtal-0.5.9/pyxtal/database/cifs/Pmmn.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      286 2022-06-17 19:13:51.000000 pyxtal-0.5.9/pyxtal/database/cifs/Pn3.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      286 2022-06-17 19:13:21.000000 pyxtal-0.5.9/pyxtal/database/cifs/Pn3m.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1605 2021-08-17 15:48:09.000000 pyxtal-0.5.9/pyxtal/database/cifs/R-3.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1933 2021-08-17 15:48:09.000000 pyxtal-0.5.9/pyxtal/database/cifs/R-3c.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      986 2021-08-17 15:48:09.000000 pyxtal-0.5.9/pyxtal/database/cifs/R32.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     3542 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/TMPPIO03.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    13289 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/WEXBOS.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   177150 2022-06-17 20:12:44.000000 pyxtal-0.5.9/pyxtal/database/cifs/YICMOP.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)        0 2023-07-08 02:10:33.000000 pyxtal-0.5.9/pyxtal/database/cifs/__init__.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2546 2022-07-27 19:22:51.000000 pyxtal-0.5.9/pyxtal/database/cifs/anthracene.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2703 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/aspirin-c.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    12951 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/aspirin.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1509 2022-07-27 00:49:00.000000 pyxtal-0.5.9/pyxtal/database/cifs/benzene.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      733 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/bug.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    17895 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/coumarin.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2260 2022-01-18 15:40:54.000000 pyxtal-0.5.9/pyxtal/database/cifs/dist_6_0.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2260 2022-01-18 15:40:53.000000 pyxtal-0.5.9/pyxtal/database/cifs/dist_6_1.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     7884 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/gdh.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1964 2022-08-22 20:08:21.000000 pyxtal-0.5.9/pyxtal/database/cifs/ht_KNbBO.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     5997 2022-08-22 18:10:54.000000 pyxtal-0.5.9/pyxtal/database/cifs/ht_cristobalite.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1251 2022-08-22 18:21:32.000000 pyxtal-0.5.9/pyxtal/database/cifs/ht_quartz.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1864 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/ice.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2869 2022-08-22 20:08:21.000000 pyxtal-0.5.9/pyxtal/database/cifs/lt_KNbBO.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      931 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/lt_cristobalite.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      866 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/lt_quartz.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1541 2022-07-27 00:49:34.000000 pyxtal-0.5.9/pyxtal/database/cifs/naphthalene.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   317844 2021-11-23 20:29:41.000000 pyxtal-0.5.9/pyxtal/database/cifs/resorcinol.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      473 2022-01-21 16:08:56.000000 pyxtal-0.5.9/pyxtal/database/cifs/sim-0.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      488 2022-01-21 16:08:55.000000 pyxtal-0.5.9/pyxtal/database/cifs/sim-1.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     4786 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/cifs/xxvi.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)  1103778 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/clusters.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2617 2022-06-23 00:39:04.000000 pyxtal-0.5.9/pyxtal/database/collection.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    19164 2022-06-14 14:22:59.000000 pyxtal-0.5.9/pyxtal/database/element.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20) 10480157 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/k_subgroup.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    20717 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/layer.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    25842 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/layer_generators.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    58872 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/layer_symmetry.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    90734 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/molecules.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   130892 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/point.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   146327 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/point_generators.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   301944 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/point_symmetry.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    18501 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/rod.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    21935 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/rod_generators.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    44320 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/rod_symmetry.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     5478 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/symbols.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)  1245398 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/t_subgroup.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   259897 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/wyckoff_generators.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   251719 2021-08-17 15:48:08.000000 pyxtal-0.5.9/pyxtal/database/wyckoff_list.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   117892 2021-08-17 15:48:09.000000 pyxtal-0.5.9/pyxtal/database/wyckoff_sets.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   627207 2021-08-17 15:48:09.000000 pyxtal-0.5.9/pyxtal/database/wyckoff_symmetry.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     8405 2023-07-18 16:54:32.000000 pyxtal-0.5.9/pyxtal/db.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    18839 2023-07-08 02:46:18.000000 pyxtal-0.5.9/pyxtal/descriptor.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    42770 2023-04-04 17:06:21.000000 pyxtal-0.5.9/pyxtal/elasticity.py
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-07-22 21:47:58.000000 pyxtal-0.5.9/pyxtal/interface/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    13515 2021-08-17 15:48:09.000000 pyxtal-0.5.9/pyxtal/interface/LJ.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)        0 2021-08-17 15:48:09.000000 pyxtal-0.5.9/pyxtal/interface/__init__.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    27602 2023-07-01 12:59:09.000000 pyxtal-0.5.9/pyxtal/interface/dftb.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    14489 2023-06-23 09:35:50.000000 pyxtal-0.5.9/pyxtal/interface/gulp.py
+-rwxr-xr-x   0 qiangzhu   (501) staff       (20)    19477 2022-01-06 13:19:42.000000 pyxtal-0.5.9/pyxtal/interface/lammpslib.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     8403 2021-08-17 15:48:09.000000 pyxtal-0.5.9/pyxtal/interface/vasp.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    31490 2021-08-17 15:48:09.000000 pyxtal-0.5.9/pyxtal/interface/vasprun.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    23034 2022-09-24 05:16:49.000000 pyxtal-0.5.9/pyxtal/io.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    67553 2023-06-22 22:47:40.000000 pyxtal-0.5.9/pyxtal/lattice.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    18090 2023-07-08 01:32:18.000000 pyxtal-0.5.9/pyxtal/molecular_crystal.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    63216 2022-11-18 06:08:23.000000 pyxtal-0.5.9/pyxtal/molecule.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2758 2022-08-09 01:18:08.000000 pyxtal-0.5.9/pyxtal/msg.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    30344 2023-06-23 21:31:46.000000 pyxtal-0.5.9/pyxtal/operations.py
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-07-22 21:47:58.000000 pyxtal-0.5.9/pyxtal/optimize/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)        0 2021-08-17 15:48:09.000000 pyxtal-0.5.9/pyxtal/optimize/__init__.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     5636 2021-08-17 15:48:09.000000 pyxtal-0.5.9/pyxtal/optimize/fire.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    12084 2021-08-17 15:48:09.000000 pyxtal-0.5.9/pyxtal/optimize/fire2.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    14967 2021-08-17 15:48:09.000000 pyxtal-0.5.9/pyxtal/optimize/myscipy_optimize.py
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-07-22 21:47:58.000000 pyxtal-0.5.9/pyxtal/potentials/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)  1820580 2021-08-17 15:48:09.000000 pyxtal-0.5.9/pyxtal/potentials/CuAg.eam.alloy
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1652 2021-08-17 15:48:09.000000 pyxtal-0.5.9/pyxtal/potentials/LJ_cluster.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      837 2021-08-17 15:48:09.000000 pyxtal-0.5.9/pyxtal/potentials/Si.tersoff
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     3991 2021-08-17 15:48:09.000000 pyxtal-0.5.9/pyxtal/potentials/SiCGe.tersoff
+-rwxr-xr-x   0 qiangzhu   (501) staff       (20)       26 2021-08-17 15:48:09.000000 pyxtal-0.5.9/pyxtal/potentials/__init__.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    16972 2023-06-23 22:45:29.000000 pyxtal-0.5.9/pyxtal/representation.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    46380 2023-06-05 08:59:34.000000 pyxtal-0.5.9/pyxtal/supergroup.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   130447 2023-07-15 02:02:20.000000 pyxtal-0.5.9/pyxtal/symmetry.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    43692 2023-07-08 02:00:44.000000 pyxtal-0.5.9/pyxtal/test_all.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    11061 2023-07-08 00:51:34.000000 pyxtal-0.5.9/pyxtal/tolerance.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    18088 2023-07-22 21:39:01.000000 pyxtal-0.5.9/pyxtal/util.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)       22 2023-07-22 21:39:07.000000 pyxtal-0.5.9/pyxtal/version.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    13329 2022-09-09 18:39:24.000000 pyxtal-0.5.9/pyxtal/viz.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    40718 2023-07-22 21:39:01.000000 pyxtal-0.5.9/pyxtal/wyckoff_site.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    21212 2023-06-05 08:57:39.000000 pyxtal-0.5.9/pyxtal/wyckoff_split.py
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-07-22 21:47:58.000000 pyxtal-0.5.9/pyxtal.egg-info/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     5203 2023-07-22 21:47:58.000000 pyxtal-0.5.9/pyxtal.egg-info/PKG-INFO
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     4250 2023-07-22 21:47:58.000000 pyxtal-0.5.9/pyxtal.egg-info/SOURCES.txt
+-rw-r--r--   0 qiangzhu   (501) staff       (20)        1 2023-07-22 21:47:58.000000 pyxtal-0.5.9/pyxtal.egg-info/dependency_links.txt
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      160 2023-07-22 21:47:58.000000 pyxtal-0.5.9/pyxtal.egg-info/requires.txt
+-rw-r--r--   0 qiangzhu   (501) staff       (20)        7 2023-07-22 21:47:58.000000 pyxtal-0.5.9/pyxtal.egg-info/top_level.txt
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-07-22 21:47:58.000000 pyxtal-0.5.9/scripts/
+-rwxr-xr-x   0 qiangzhu   (501) staff       (20)     4296 2023-06-27 08:23:49.000000 pyxtal-0.5.9/scripts/pyxtal_main.py
+-rwxr-xr-x   0 qiangzhu   (501) staff       (20)      960 2021-08-17 15:48:09.000000 pyxtal-0.5.9/scripts/pyxtal_symmetry.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      125 2023-07-22 21:47:58.000000 pyxtal-0.5.9/setup.cfg
+-rwxr-xr-x   0 qiangzhu   (501) staff       (20)     1798 2023-07-22 13:53:02.000000 pyxtal-0.5.9/setup.py
```

### Comparing `pyxtal-0.5.8/LICENSE.txt` & `pyxtal-0.5.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/PKG-INFO` & `pyxtal-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pyxtal
-Version: 0.5.8
+Version: 0.5.9
 Summary: Python code for generation of crystal structures based on symmetry constraints.
 Home-page: https://github.com/qzhu2017/PyXtal
 Author: Scott Fredericks, Qiang Zhu
 Author-email: qiang.zhu@unlv.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7, <=3.11
+Requires-Python: >=3.7, <=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 <img src="https://raw.githubusercontent.com/qzhu2017/PyXtal/master/images/512px_type1.png" alt="PyXtal" width="300"/>
 
 [![Documentation Status](https://readthedocs.org/projects/pyxtal/badge/?version=latest)](https://pyxtal.readthedocs.io/en/latest/?badge=latest)
 [![Test Status](https://github.com/qzhu2017/PyXtal/workflows/tests/badge.svg)](https://github.com/qzhu2017/PyXtal/actions)
```

### Comparing `pyxtal-0.5.8/README.md` & `pyxtal-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/XRD.py` & `pyxtal-0.5.9/pyxtal/XRD.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/__init__.py` & `pyxtal-0.5.9/pyxtal/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1459,46 +1459,62 @@
         """
 
         from pyxtal.symmetry import choose_wyckoff
 
         if self.molecular:
             raise RuntimeError("Cannot support the molecular crystal")
 
-        self.group = Group(group)
+        if type(group) == Group:
+            self.group = group
+        else:
+            self.group = Group(group)
+ 
         self.lattice = lattice
         self.dim = 3
         self.factor = 1.0
         self.PBC = [1, 1, 1]
         self.numIons = numIons
         self.species = species
         numIons_added = np.zeros(len(numIons), dtype=int)
         _sites = []
 
         if len(sites) != len(species):
             print(len(sites), len(species))
             raise RuntimeError("Inconsistency between sites and species")
 
         for sp, wps in zip(species, sites):
-            if type(wps) is dict:
-                for pair in wps.items():
-                    (key, pos) = pair
+            for wp in wps:
+                if type(wp) is dict:
+                    for pair in wp.items():
+                        (key, pos) = pair
+                        _wp = choose_wyckoff(self.group, site=key)
+                        if _wp is not False:
+                            if _wp.get_dof() == 0: #fixed pos
+                                pt = [0.0, 0.0, 0.0]
+                            else:
+                                pt = _wp.get_all_positions(pos)[0]
+                            _sites.append(atom_site(_wp, pt, sp))
+                        else:
+                            raise RuntimeError("Cannot interpret site", key)
+                elif len(wp) == 4: # tuple:
+                    (key, x, y, z) = wp
                     _wp = choose_wyckoff(self.group, site=key)
                     if _wp is not False:
                         if _wp.get_dof() == 0: #fixed pos
                             pt = [0.0, 0.0, 0.0]
                         else:
-                            pt = _wp.get_all_positions(pos)[0]
+                            pt = _wp.get_all_positions([x, y, z])[0]
                         _sites.append(atom_site(_wp, pt, sp))
                     else:
                         raise RuntimeError("Cannot interpret site", key)
-            else: #List of atomic coordinates
-                wp0 = self.group[0]
-                for pos in wps:
-                    pt, _wp, _ = wp0.merge(pos, lattice.matrix, tol=0.1)
-                    _sites.append(atom_site(_wp, pt, sp))
+                else: #List of atomic coordinates
+                    wp0 = self.group[0]
+                    for pos in wps:
+                        pt, _wp, _ = wp0.merge(pos, lattice.matrix, tol=0.1)
+                        _sites.append(atom_site(_wp, pt, sp))
 
         self.atom_sites = _sites
         self.standard_setting = True
         self.valid = True
         self.source = 'Build'
         self._get_formula()
```

### Comparing `pyxtal-0.5.8/pyxtal/block_crystal.py` & `pyxtal-0.5.9/pyxtal/block_crystal.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/constants.py` & `pyxtal-0.5.9/pyxtal/constants.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/crystal.py` & `pyxtal-0.5.9/pyxtal/crystal.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/HM_Full.csv` & `pyxtal-0.5.9/pyxtal/database/HM_Full.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/atomic_scattering_params.json` & `pyxtal-0.5.9/pyxtal/database/atomic_scattering_params.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/bonds.json` & `pyxtal-0.5.9/pyxtal/database/bonds.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/bug.json` & `pyxtal-0.5.9/pyxtal/database/bug.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/0-G62.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/0-G62.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/1-G59.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/1-G59.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/2-G71.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/2-G71.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/3-G139.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/3-G139.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/4-G225.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/4-G225.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/ACBNZA01.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/ACBNZA01.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/AXOSOW01.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/AXOSOW01.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/Al2SiO5_mp-4753_symmetrized.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/Al2SiO5_mp-4753_symmetrized.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/BTO-Amm2.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/BTO-Amm2.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/BTO.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/BTO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/CuAu_mp-582681_symmetrized.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/CuAu_mp-582681_symmetrized.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/FAU.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/FAU.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/Fd3.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/Fd3.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/Fd3.vasp` & `pyxtal-0.5.9/pyxtal/database/cifs/Fd3.vasp`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/Fd3m.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/Fd3m.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/GUMMUW.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/GUMMUW.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/GeF2.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/GeF2.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/HAHCOI.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/HAHCOI.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/I4_132.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/I4_132.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/JAPWIH.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/JAPWIH.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/LAGNAL.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/LAGNAL.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/LUFHAW.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/LUFHAW.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/LiCs.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/LiCs.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/MERQIM.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/MERQIM.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/MPWO.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/MPWO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/NaCl.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/NaCl.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/NaSb3F10.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/NaSb3F10.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/NbO2.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/NbO2.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/NiS-Cm.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/NiS-Cm.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/P3_112.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/P3_112.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/P4_332.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/P4_332.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/P6_422.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/P6_422.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/PAHYON01.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/PAHYON01.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/PPO.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/PPO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/PVO.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/PVO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/Pm3.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/Pm3.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/R-3.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/R-3.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/R-3c.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/R-3c.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/R32.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/R32.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/TMPPIO03.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/TMPPIO03.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/WEXBOS.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/WEXBOS.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/YICMOP.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/YICMOP.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/anthracene.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/anthracene.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/aspirin-c.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/aspirin-c.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/aspirin.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/aspirin.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/benzene.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/benzene.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/bug.vasp` & `pyxtal-0.5.9/pyxtal/database/cifs/bug.vasp`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/coumarin.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/coumarin.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/dist_6_0.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/dist_6_0.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/dist_6_1.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/dist_6_1.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/gdh.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/gdh.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/ht_KNbBO.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/ht_KNbBO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/ht_cristobalite.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/ht_cristobalite.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/ht_quartz.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/ht_quartz.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/ice.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/ice.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/lt_KNbBO.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/lt_KNbBO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/lt_cristobalite.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/lt_cristobalite.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/lt_quartz.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/lt_quartz.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/naphthalene.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/naphthalene.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/resorcinol.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/resorcinol.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/cifs/xxvi.cif` & `pyxtal-0.5.9/pyxtal/database/cifs/xxvi.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/clusters.json` & `pyxtal-0.5.9/pyxtal/database/clusters.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/collection.py` & `pyxtal-0.5.9/pyxtal/database/collection.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/element.py` & `pyxtal-0.5.9/pyxtal/database/element.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/k_subgroup.json` & `pyxtal-0.5.9/pyxtal/database/k_subgroup.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/layer.csv` & `pyxtal-0.5.9/pyxtal/database/layer.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/layer_generators.csv` & `pyxtal-0.5.9/pyxtal/database/layer_generators.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/layer_symmetry.csv` & `pyxtal-0.5.9/pyxtal/database/layer_symmetry.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/molecules.json` & `pyxtal-0.5.9/pyxtal/database/molecules.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/point.csv` & `pyxtal-0.5.9/pyxtal/database/point.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/point_generators.csv` & `pyxtal-0.5.9/pyxtal/database/point_generators.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/point_symmetry.csv` & `pyxtal-0.5.9/pyxtal/database/point_symmetry.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/rod.csv` & `pyxtal-0.5.9/pyxtal/database/rod.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/rod_generators.csv` & `pyxtal-0.5.9/pyxtal/database/rod_generators.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/rod_symmetry.csv` & `pyxtal-0.5.9/pyxtal/database/rod_symmetry.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/symbols.json` & `pyxtal-0.5.9/pyxtal/database/symbols.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/t_subgroup.json` & `pyxtal-0.5.9/pyxtal/database/t_subgroup.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/wyckoff_generators.csv` & `pyxtal-0.5.9/pyxtal/database/wyckoff_generators.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/wyckoff_list.csv` & `pyxtal-0.5.9/pyxtal/database/wyckoff_list.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/wyckoff_sets.json` & `pyxtal-0.5.9/pyxtal/database/wyckoff_sets.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/database/wyckoff_symmetry.csv` & `pyxtal-0.5.9/pyxtal/database/wyckoff_symmetry.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/db.py` & `pyxtal-0.5.9/pyxtal/db.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/descriptor.py` & `pyxtal-0.5.9/pyxtal/descriptor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Module for crystal packing descriptor from energy decomposition
 """
 import numpy as np
+import pyshtools as pysh
 from scipy.stats import qmc
 from scipy.spatial.transform import Rotation
 from scipy.optimize import minimize
 from scipy.special import sph_harm
 
 def _qlm(dists, l=4):
     '''
@@ -281,15 +282,14 @@
         xtal: pyxtal structure
         model: 'molecule' or 'contact'
         max_d: maximum intermolecular distances
         lmax: maximum bandwidth for spherical harmonic expansion
         sigma: Gaussian width to project into the unit sphere
         N: number of grid points on the unit sphere
     """
-    import pyshtools as pysh
 
     def __init__(self, xtal, model='molecule', max_d=10, 
         factor=2.2, lmax=13, sigma=0.1, N=10000):
 
         for i in range(len(xtal.mol_sites)):
             try:
                 numbers = xtal.mol_sites[i].molecule.mol.atomic_numbers
```

### Comparing `pyxtal-0.5.8/pyxtal/elasticity.py` & `pyxtal-0.5.9/pyxtal/elasticity.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/interface/LJ.py` & `pyxtal-0.5.9/pyxtal/interface/LJ.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/interface/dftb.py` & `pyxtal-0.5.9/pyxtal/interface/dftb.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/interface/gulp.py` & `pyxtal-0.5.9/pyxtal/interface/gulp.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/interface/lammpslib.py` & `pyxtal-0.5.9/pyxtal/interface/lammpslib.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/interface/vasp.py` & `pyxtal-0.5.9/pyxtal/interface/vasp.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/interface/vasprun.py` & `pyxtal-0.5.9/pyxtal/interface/vasprun.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/io.py` & `pyxtal-0.5.9/pyxtal/io.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/lattice.py` & `pyxtal-0.5.9/pyxtal/lattice.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/molecular_crystal.py` & `pyxtal-0.5.9/pyxtal/molecular_crystal.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/molecule.py` & `pyxtal-0.5.9/pyxtal/molecule.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/msg.py` & `pyxtal-0.5.9/pyxtal/msg.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/operations.py` & `pyxtal-0.5.9/pyxtal/operations.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/optimize/fire.py` & `pyxtal-0.5.9/pyxtal/optimize/fire.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/optimize/fire2.py` & `pyxtal-0.5.9/pyxtal/optimize/fire2.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/optimize/myscipy_optimize.py` & `pyxtal-0.5.9/pyxtal/optimize/myscipy_optimize.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/potentials/CuAg.eam.alloy` & `pyxtal-0.5.9/pyxtal/potentials/CuAg.eam.alloy`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/potentials/LJ_cluster.py` & `pyxtal-0.5.9/pyxtal/potentials/LJ_cluster.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/potentials/Si.tersoff` & `pyxtal-0.5.9/pyxtal/potentials/Si.tersoff`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/potentials/SiCGe.tersoff` & `pyxtal-0.5.9/pyxtal/potentials/SiCGe.tersoff`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/representation.py` & `pyxtal-0.5.9/pyxtal/representation.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/supergroup.py` & `pyxtal-0.5.9/pyxtal/supergroup.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/symmetry.py` & `pyxtal-0.5.9/pyxtal/symmetry.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/test_all.py` & `pyxtal-0.5.9/pyxtal/test_all.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/tolerance.py` & `pyxtal-0.5.9/pyxtal/tolerance.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/util.py` & `pyxtal-0.5.9/pyxtal/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -484,34 +484,44 @@
         s1, e1 = id*N_atoms, (id+1)*N_atoms
         s2, e2 = i*N_atoms, (i+1)*N_atoms
         pos1[s2:e2, :] += pos0[s1:e1, :] - shifts[i].dot(atoms.cell[:])
 
     atoms.set_positions(pos1)
     return atoms
 
-def generate_wp_lib(spg_list, composition, max_wp=None, min_wp=None, 
-                    max_fu=None, min_fu=None, N_max=1000):
+def generate_wp_lib(spg_list, composition, 
+                    num_wp=(None, None), 
+                    num_fu=(None, None), 
+                    num_dof=(None, None), 
+                    N_max=1000):
     """
     Generate wps according to the composition constraint (e.g., SiO2)
 
     Args;
         - spg_list: list of space group choices
         - composition: chemical compositions [1, 2]
-        - max_wp: the number of maximum wp sites
-        - min_wp: the number of minimum wp sites
+        - num_wp: (min_wp, max_wp)
+        - num_fu: (min_fu, max_fu)
+        - num_dof: (min_dof, max_dof)
 
     Returns:
-        a list of wps [spg, ([wp1, ...], ... [wp1, ...]), wp_dof]
+        a list of wps [spg, ([wp1, ...], ... [wp1, ...]), dof]
     """
 
     from pyxtal.symmetry import Group
 
     composition = np.array(composition, dtype=int)
+    (min_wp, max_wp) = num_wp
+    (min_fu, max_fu) = num_fu
+    (min_dof, max_dof) = num_dof
+
     if max_wp is None: max_wp = len(composition)
     if min_wp is None: min_wp = len(composition)
+    if min_dof is None: min_dof = 1
+    if max_dof is None: max_dof = 1000
     #print(max_wp, min_wp)
     wps = []
     for sg in spg_list:
         g = Group(sg)
         lat_dof = g.get_lattice_dof()
         # determine the upper and lower limit 
         if min_fu is None: min_fu = max([int(len(g[-1])/min(composition)), 1])
@@ -519,20 +529,24 @@
         count = 0
         for i in range(max_fu, min_fu-1, -1):
             letters, _, wp_ids = g.list_wyckoff_combinations(
                     composition*i, max_wp=max_wp, 
                     min_wp=min_wp, Nmax=100000)
             for j, wp in enumerate(wp_ids):
                 wp_dofs = 0
+                num = 0
                 for wp0 in wp:
                     for id in wp0:
                         wp_dofs += g[id].get_dof()
+                        num += g[id].multiplicity
                 #print(sg, wp, letters[j])
-                wps.append((sg, wp, lat_dof + wp_dofs))
-            count += len(letters)
+                num_dof = lat_dof + wp_dofs
+                if min_dof <= num_dof <= max_dof:
+                    wps.append((num, sg, wp, lat_dof + wp_dofs))
+                    count += 1
             if count >= N_max:
                 break
     return wps 
  
 
 if __name__ == "__main__":
     from argparse import ArgumentParser
```

### Comparing `pyxtal-0.5.8/pyxtal/viz.py` & `pyxtal-0.5.9/pyxtal/viz.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal/wyckoff_site.py` & `pyxtal-0.5.9/pyxtal/wyckoff_site.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,16 +75,18 @@
                 }
         return dict0
 
     def _get_dof(self):
         """
         get the number of dof for the given structures:
         """
-        freedom = np.trace(self.wp.ops[0].rotation_matrix) > 0
-        self.dof = len(freedom[freedom==True])
+        self.dof = self.wp.get_dof()
+        #freedom = np.trace(self.wp.ops[0].rotation_matrix) > 0
+        #self.dof = len(freedom[freedom==True])
+        #self.dof = len(freedom[freedom==True])
 
 
     @classmethod
     def load_dict(cls, dicts):
         """
         load the sites from a dictionary
         """
```

### Comparing `pyxtal-0.5.8/pyxtal/wyckoff_split.py` & `pyxtal-0.5.9/pyxtal/wyckoff_split.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/pyxtal.egg-info/PKG-INFO` & `pyxtal-0.5.9/pyxtal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pyxtal
-Version: 0.5.8
+Version: 0.5.9
 Summary: Python code for generation of crystal structures based on symmetry constraints.
 Home-page: https://github.com/qzhu2017/PyXtal
 Author: Scott Fredericks, Qiang Zhu
 Author-email: qiang.zhu@unlv.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7, <=3.11
+Requires-Python: >=3.7, <=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 <img src="https://raw.githubusercontent.com/qzhu2017/PyXtal/master/images/512px_type1.png" alt="PyXtal" width="300"/>
 
 [![Documentation Status](https://readthedocs.org/projects/pyxtal/badge/?version=latest)](https://pyxtal.readthedocs.io/en/latest/?badge=latest)
 [![Test Status](https://github.com/qzhu2017/PyXtal/workflows/tests/badge.svg)](https://github.com/qzhu2017/PyXtal/actions)
```

### Comparing `pyxtal-0.5.8/pyxtal.egg-info/SOURCES.txt` & `pyxtal-0.5.9/pyxtal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/scripts/pyxtal_main.py` & `pyxtal-0.5.9/scripts/pyxtal_main.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/scripts/pyxtal_symmetry.py` & `pyxtal-0.5.9/scripts/pyxtal_symmetry.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.8/setup.py` & `pyxtal-0.5.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,21 +40,21 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "spglib>=1.10.4",
-        "pymatgen>=2022.0.12",
+        "pymatgen>=2022.0.17",
         "pandas>=0.24.2",
         "networkx>=2.3",
         "py3Dmol>=0.8.0",
         'ase>=3.18.0',  #covered by pymatgen
         'numba>=0.55.2', #now supports numpy 1.22
         'scipy>=1.7.3',
         'importlib_metadata>=1.4',
         'pyshtools>=4.10.3',
         #"openbabel>=3.0.0",
     ],
-    python_requires=">=3.7, <=3.11", #add the restriction for now issue #189
+    python_requires=">=3.7, <=3.12", #add the restriction for now issue #189
     license="MIT",
 )
```

