# Comparing `tmp/femagtools-1.2.6.tar.gz` & `tmp/femagtools-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "femagtools-1.2.6.tar", last modified: Wed Apr  5 06:38:55 2023, max compression
+gzip compressed data, was "femagtools-1.2.7.tar", last modified: Thu Apr 13 07:50:58 2023, max compression
```

## Comparing `femagtools-1.2.6.tar` & `femagtools-1.2.7.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-04-05 06:38:55.808471 femagtools-1.2.6/
--rw-r--r--   0 tar        (210) tar        (210)     1316 2023-02-15 20:03:56.000000 femagtools-1.2.6/LICENSE
--rw-r--r--   0 tar        (210) tar        (210)       35 2023-02-15 20:03:56.000000 femagtools-1.2.6/MANIFEST.in
--rw-r--r--   0 tar        (210) tar        (210)     5262 2023-04-05 06:38:55.808471 femagtools-1.2.6/PKG-INFO
--rw-r--r--   0 tar        (210) tar        (210)     3072 2023-02-14 18:11:00.000000 femagtools-1.2.6/README.md
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-04-05 06:38:55.794471 femagtools-1.2.6/femagtools/
--rw-r--r--   0 tar        (210) tar        (210)     1630 2023-04-05 06:37:39.000000 femagtools-1.2.6/femagtools/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)     2250 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/airgap.py
--rw-r--r--   0 tar        (210) tar        (210)    12122 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/amazon.py
--rw-r--r--   0 tar        (210) tar        (210)     9741 2023-02-14 18:11:00.000000 femagtools-1.2.6/femagtools/amela.py
--rw-r--r--   0 tar        (210) tar        (210)     7706 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/asm.py
--rwxr-xr-x   0 tar        (210) tar        (210)    68684 2023-02-14 18:11:00.000000 femagtools-1.2.6/femagtools/bch.py
--rw-r--r--   0 tar        (210) tar        (210)     2923 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/bchxml.py
--rw-r--r--   0 tar        (210) tar        (210)    10766 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/condor.py
--rw-r--r--   0 tar        (210) tar        (210)     1076 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/conductor.py
--rw-r--r--   0 tar        (210) tar        (210)     3087 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/config.py
--rw-r--r--   0 tar        (210) tar        (210)    23706 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/convert.py
--rw-r--r--   0 tar        (210) tar        (210)     7017 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/dakota.py
--rwxr-xr-x   0 tar        (210) tar        (210)     4064 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/dakota_femag.py
--rw-r--r--   0 tar        (210) tar        (210)     5573 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/dakotaout.py
--rw-r--r--   0 tar        (210) tar        (210)     7460 2023-03-24 14:45:00.000000 femagtools-1.2.6/femagtools/docker.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-04-05 06:38:55.796471 femagtools-1.2.6/femagtools/dxfsl/
--rw-r--r--   0 tar        (210) tar        (210)        0 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/dxfsl/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)    52503 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/dxfsl/area.py
--rw-r--r--   0 tar        (210) tar        (210)     8990 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/dxfsl/conv.py
--rw-r--r--   0 tar        (210) tar        (210)    18787 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/dxfsl/converter.py
--rw-r--r--   0 tar        (210) tar        (210)     1266 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/dxfsl/corner.py
--rw-r--r--   0 tar        (210) tar        (210)     1861 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/dxfsl/dumprenderer.py
--rw-r--r--   0 tar        (210) tar        (210)    23233 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/dxfsl/fslrenderer.py
--rw-r--r--   0 tar        (210) tar        (210)     9835 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/dxfsl/functions.py
--rw-r--r--   0 tar        (210) tar        (210)   132506 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/dxfsl/geom.py
--rw-r--r--   0 tar        (210) tar        (210)    27661 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/dxfsl/machine.py
--rw-r--r--   0 tar        (210) tar        (210)    12311 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/dxfsl/plotrenderer.py
--rw-r--r--   0 tar        (210) tar        (210)    43088 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/dxfsl/shape.py
--rw-r--r--   0 tar        (210) tar        (210)     1224 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/erg.py
--rw-r--r--   0 tar        (210) tar        (210)    40477 2023-02-21 19:53:03.000000 femagtools-1.2.6/femagtools/femag.py
--rw-r--r--   0 tar        (210) tar        (210)     7466 2023-02-15 20:03:56.000000 femagtools-1.2.6/femagtools/forcedens.py
--rw-r--r--   0 tar        (210) tar        (210)    28180 2023-02-21 19:53:03.000000 femagtools-1.2.6/femagtools/fsl.py
--rw-r--r--   0 tar        (210) tar        (210)     3017 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/getset.py
--rw-r--r--   0 tar        (210) tar        (210)     3903 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/gmsh.py
--rw-r--r--   0 tar        (210) tar        (210)    17166 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/google.py
--rw-r--r--   0 tar        (210) tar        (210)     1561 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/grid.py
--rw-r--r--   0 tar        (210) tar        (210)    41557 2023-02-14 18:11:00.000000 femagtools-1.2.6/femagtools/isa7.py
--rw-r--r--   0 tar        (210) tar        (210)     2790 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/jcf2msh.py
--rw-r--r--   0 tar        (210) tar        (210)     1779 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/jhb.py
--rw-r--r--   0 tar        (210) tar        (210)    11320 2023-02-14 18:11:00.000000 femagtools-1.2.6/femagtools/job.py
--rw-r--r--   0 tar        (210) tar        (210)     2261 2022-08-24 07:36:25.000000 femagtools-1.2.6/femagtools/losscoeffs.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-04-05 06:38:55.796471 femagtools-1.2.6/femagtools/machine/
--rw-r--r--   0 tar        (210) tar        (210)     5613 2023-02-14 18:11:00.000000 femagtools-1.2.6/femagtools/machine/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)     5604 2023-04-05 06:37:05.000000 femagtools-1.2.6/femagtools/machine/effloss.py
--rw-r--r--   0 tar        (210) tar        (210)    34847 2023-02-14 18:11:00.000000 femagtools-1.2.6/femagtools/machine/im.py
--rwxr-xr-x   0 tar        (210) tar        (210)    30631 2023-04-05 06:37:05.000000 femagtools-1.2.6/femagtools/machine/pm.py
--rw-r--r--   0 tar        (210) tar        (210)    21743 2023-02-14 18:11:00.000000 femagtools-1.2.6/femagtools/machine/sizing.py
--rw-r--r--   0 tar        (210) tar        (210)    14584 2023-02-14 18:11:00.000000 femagtools-1.2.6/femagtools/machine/sm.py
--rw-r--r--   0 tar        (210) tar        (210)    16143 2023-02-14 18:11:00.000000 femagtools-1.2.6/femagtools/machine/utils.py
--rw-r--r--   0 tar        (210) tar        (210)     1093 2023-02-15 20:03:56.000000 femagtools-1.2.6/femagtools/magnet.py
--rw-r--r--   0 tar        (210) tar        (210)    38043 2023-02-16 09:09:33.000000 femagtools-1.2.6/femagtools/mcv.py
--rw-r--r--   0 tar        (210) tar        (210)     1833 2023-02-14 18:11:00.000000 femagtools-1.2.6/femagtools/me.py
--rw-r--r--   0 tar        (210) tar        (210)    14106 2023-02-14 18:11:00.000000 femagtools-1.2.6/femagtools/model.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-04-05 06:38:55.797471 femagtools-1.2.6/femagtools/moo/
--rw-r--r--   0 tar        (210) tar        (210)      175 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/moo/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)     5493 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/moo/algorithm.py
--rw-r--r--   0 tar        (210) tar        (210)    10100 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/moo/population.py
--rw-r--r--   0 tar        (210) tar        (210)     2391 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/moo/problem.py
--rw-r--r--   0 tar        (210) tar        (210)     2825 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/moproblem.py
--rw-r--r--   0 tar        (210) tar        (210)     8265 2023-04-05 06:37:05.000000 femagtools-1.2.6/femagtools/multiproc.py
--rw-r--r--   0 tar        (210) tar        (210)     1841 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/mxw2msh.py
--rw-r--r--   0 tar        (210) tar        (210)    12781 2023-02-14 18:11:00.000000 femagtools-1.2.6/femagtools/nc.py
--rw-r--r--   0 tar        (210) tar        (210)     2052 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/netlist.py
--rw-r--r--   0 tar        (210) tar        (210)     3099 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/ntib.py
--rw-r--r--   0 tar        (210) tar        (210)     8685 2023-02-21 19:53:03.000000 femagtools-1.2.6/femagtools/opt.py
--rw-r--r--   0 tar        (210) tar        (210)    18733 2023-04-05 06:37:05.000000 femagtools-1.2.6/femagtools/parstudy.py
--rw-r--r--   0 tar        (210) tar        (210)    57795 2023-04-05 06:37:05.000000 femagtools-1.2.6/femagtools/plot.py
--rw-r--r--   0 tar        (210) tar        (210)     6536 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/poc.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-04-05 06:38:55.805471 femagtools-1.2.6/femagtools/templates/
--rw-r--r--   0 tar        (210) tar        (210)      874 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/FE-losses.mako
--rw-r--r--   0 tar        (210) tar        (210)      242 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/airgapinduc.mako
--rw-r--r--   0 tar        (210) tar        (210)     2879 2022-09-28 06:51:55.000000 femagtools-1.2.6/femagtools/templates/asyn_motor.mako
--rw-r--r--   0 tar        (210) tar        (210)     2483 2022-09-28 06:51:55.000000 femagtools-1.2.6/femagtools/templates/basic_modpar.mako
--rw-r--r--   0 tar        (210) tar        (210)     1911 2023-02-14 18:11:00.000000 femagtools-1.2.6/femagtools/templates/calc_field_ts.mako
--rw-r--r--   0 tar        (210) tar        (210)      997 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/cogg_calc.mako
--rw-r--r--   0 tar        (210) tar        (210)      400 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/colorgrad.mako
--rw-r--r--   0 tar        (210) tar        (210)     1264 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/com_motor_sim.mako
--rw-r--r--   0 tar        (210) tar        (210)      472 2023-02-14 18:11:00.000000 femagtools-1.2.6/femagtools/templates/conduct-data.mako
--rw-r--r--   0 tar        (210) tar        (210)      437 2023-02-14 18:11:00.000000 femagtools-1.2.6/femagtools/templates/connect_models.mako
--rw-r--r--   0 tar        (210) tar        (210)     1350 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/cu_losses.mako
--rw-r--r--   0 tar        (210) tar        (210)     1672 2023-02-14 18:11:00.000000 femagtools-1.2.6/femagtools/templates/ec-rotorbar.mako
--rw-r--r--   0 tar        (210) tar        (210)     1983 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/fe-contr.mako
--rw-r--r--   0 tar        (210) tar        (210)     4289 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/gen_winding.mako
--rw-r--r--   0 tar        (210) tar        (210)      560 2023-02-14 18:11:00.000000 femagtools-1.2.6/femagtools/templates/inductances.mako
--rw-r--r--   0 tar        (210) tar        (210)     1270 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/ld_lq_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)      600 2023-02-14 18:11:00.000000 femagtools-1.2.6/femagtools/templates/leak_dist_wind.mako
--rw-r--r--   0 tar        (210) tar        (210)      770 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/leak_evol_wind.mako
--rw-r--r--   0 tar        (210) tar        (210)      431 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/leak_tooth_wind.mako
--rw-r--r--   0 tar        (210) tar        (210)     1271 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/magnet-data.mako
--rw-r--r--   0 tar        (210) tar        (210)      788 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/magnetFC2.mako
--rw-r--r--   0 tar        (210) tar        (210)     1372 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/magnetIron.mako
--rw-r--r--   0 tar        (210) tar        (210)     1426 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/magnetIron2.mako
--rw-r--r--   0 tar        (210) tar        (210)     2315 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/magnetIron3.mako
--rw-r--r--   0 tar        (210) tar        (210)     1413 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/magnetIron4.mako
--rw-r--r--   0 tar        (210) tar        (210)     1376 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/magnetIron5.mako
--rw-r--r--   0 tar        (210) tar        (210)     2208 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/magnetIronV.mako
--rw-r--r--   0 tar        (210) tar        (210)     2010 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/magnetSector.mako
--rw-r--r--   0 tar        (210) tar        (210)      727 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/magnetSectorLinear.mako
--rw-r--r--   0 tar        (210) tar        (210)     1295 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/magnetShell.mako
--rw-r--r--   0 tar        (210) tar        (210)     4080 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/magnetShell2.mako
--rw-r--r--   0 tar        (210) tar        (210)     1094 2023-02-14 18:11:00.000000 femagtools-1.2.6/femagtools/templates/mesh-airgap.mako
--rw-r--r--   0 tar        (210) tar        (210)     2298 2023-02-14 18:11:00.000000 femagtools-1.2.6/femagtools/templates/modal_analysis.mako
--rw-r--r--   0 tar        (210) tar        (210)     1202 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/mult_cal_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)      345 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/new_model.mako
--rw-r--r--   0 tar        (210) tar        (210)     3209 2023-02-14 18:11:00.000000 femagtools-1.2.6/femagtools/templates/noloadflux-rot.mako
--rw-r--r--   0 tar        (210) tar        (210)     4661 2023-02-14 18:11:00.000000 femagtools-1.2.6/femagtools/templates/noloadflux.mako
--rw-r--r--   0 tar        (210) tar        (210)     3146 2023-02-14 18:11:00.000000 femagtools-1.2.6/femagtools/templates/noloadfluxdc.mako
--rw-r--r--   0 tar        (210) tar        (210)      313 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/open.mako
--rw-r--r--   0 tar        (210) tar        (210)      630 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/plots.mako
--rw-r--r--   0 tar        (210) tar        (210)     1373 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/pm_sym_f_cur.mako
--rw-r--r--   0 tar        (210) tar        (210)     2319 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/pm_sym_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)      925 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/pm_sym_loss.mako
--rw-r--r--   0 tar        (210) tar        (210)     1251 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/psd_psq_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)      643 2023-02-14 18:11:00.000000 femagtools-1.2.6/femagtools/templates/ring.mako
--rw-r--r--   0 tar        (210) tar        (210)      973 2022-09-28 06:51:55.000000 femagtools-1.2.6/femagtools/templates/rot_hsm.mako
--rw-r--r--   0 tar        (210) tar        (210)     2280 2022-09-28 06:51:55.000000 femagtools-1.2.6/femagtools/templates/rotorAsyn.mako
--rw-r--r--   0 tar        (210) tar        (210)     1908 2023-02-14 18:11:00.000000 femagtools-1.2.6/femagtools/templates/rotorKs2.mako
--rw-r--r--   0 tar        (210) tar        (210)     1910 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/rotor_msh.mako
--rw-r--r--   0 tar        (210) tar        (210)      753 2022-09-28 06:51:55.000000 femagtools-1.2.6/femagtools/templates/rotor_winding.mako
--rw-r--r--   0 tar        (210) tar        (210)     1981 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/shortcircuit.mako
--rw-r--r--   0 tar        (210) tar        (210)     2077 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/srm.mako
--rw-r--r--   0 tar        (210) tar        (210)      761 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/stator1.mako
--rw-r--r--   0 tar        (210) tar        (210)      599 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/stator2.mako
--rw-r--r--   0 tar        (210) tar        (210)      724 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/stator3Linear.mako
--rw-r--r--   0 tar        (210) tar        (210)     1179 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/stator4.mako
--rw-r--r--   0 tar        (210) tar        (210)      893 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/statorBG.mako
--rw-r--r--   0 tar        (210) tar        (210)     2071 2023-02-14 18:11:00.000000 femagtools-1.2.6/femagtools/templates/statorRing.mako
--rw-r--r--   0 tar        (210) tar        (210)     4073 2023-02-14 18:11:00.000000 femagtools-1.2.6/femagtools/templates/statorRotor3.mako
--rw-r--r--   0 tar        (210) tar        (210)     1799 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/stator_msh.mako
--rw-r--r--   0 tar        (210) tar        (210)     1761 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/templates/torq_calc.mako
--rw-r--r--   0 tar        (210) tar        (210)     5791 2022-08-24 07:36:25.000000 femagtools-1.2.6/femagtools/tks.py
--rw-r--r--   0 tar        (210) tar        (210)    47280 2023-02-14 18:11:00.000000 femagtools-1.2.6/femagtools/ts.py
--rw-r--r--   0 tar        (210) tar        (210)     2444 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/vbf.py
--rw-r--r--   0 tar        (210) tar        (210)     8595 2022-08-07 12:24:45.000000 femagtools-1.2.6/femagtools/vtu.py
--rw-r--r--   0 tar        (210) tar        (210)    22279 2023-03-24 14:45:00.000000 femagtools-1.2.6/femagtools/windings.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-04-05 06:38:55.795471 femagtools-1.2.6/femagtools.egg-info/
--rw-r--r--   0 tar        (210) tar        (210)     5262 2023-04-05 06:38:55.000000 femagtools-1.2.6/femagtools.egg-info/PKG-INFO
--rw-r--r--   0 tar        (210) tar        (210)     4861 2023-04-05 06:38:55.000000 femagtools-1.2.6/femagtools.egg-info/SOURCES.txt
--rw-r--r--   0 tar        (210) tar        (210)        1 2023-04-05 06:38:55.000000 femagtools-1.2.6/femagtools.egg-info/dependency_links.txt
--rw-r--r--   0 tar        (210) tar        (210)      191 2023-04-05 06:38:55.000000 femagtools-1.2.6/femagtools.egg-info/entry_points.txt
--rw-r--r--   0 tar        (210) tar        (210)      144 2023-04-05 06:38:55.000000 femagtools-1.2.6/femagtools.egg-info/requires.txt
--rw-r--r--   0 tar        (210) tar        (210)       11 2023-04-05 06:38:55.000000 femagtools-1.2.6/femagtools.egg-info/top_level.txt
--rw-r--r--   0 tar        (210) tar        (210)     1369 2023-02-15 20:03:56.000000 femagtools-1.2.6/pyproject.toml
--rw-r--r--   0 tar        (210) tar        (210)       38 2023-04-05 06:38:55.808471 femagtools-1.2.6/setup.cfg
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-04-05 06:38:55.808471 femagtools-1.2.6/tests/
--rw-r--r--   0 tar        (210) tar        (210)     1065 2022-08-07 12:24:45.000000 femagtools-1.2.6/tests/test_airgap_induction.py
--rw-r--r--   0 tar        (210) tar        (210)      646 2023-02-14 18:11:00.000000 femagtools-1.2.6/tests/test_amela.py
--rw-r--r--   0 tar        (210) tar        (210)     1398 2022-08-07 12:24:45.000000 femagtools-1.2.6/tests/test_asm.py
--rwxr-xr-x   0 tar        (210) tar        (210)    14755 2023-02-14 18:11:00.000000 femagtools-1.2.6/tests/test_bchreader.py
--rw-r--r--   0 tar        (210) tar        (210)      332 2022-08-07 12:24:45.000000 femagtools-1.2.6/tests/test_conductor.py
--rw-r--r--   0 tar        (210) tar        (210)     6171 2022-08-07 12:24:45.000000 femagtools-1.2.6/tests/test_convert.py
--rw-r--r--   0 tar        (210) tar        (210)     1077 2023-04-05 06:37:05.000000 femagtools-1.2.6/tests/test_effloss.py
--rw-r--r--   0 tar        (210) tar        (210)      523 2022-08-07 12:24:45.000000 femagtools-1.2.6/tests/test_erg.py
--rw-r--r--   0 tar        (210) tar        (210)     1934 2023-02-16 09:09:33.000000 femagtools-1.2.6/tests/test_femag.py
--rw-r--r--   0 tar        (210) tar        (210)      533 2022-08-07 12:24:45.000000 femagtools-1.2.6/tests/test_forcedens.py
--rwxr-xr-x   0 tar        (210) tar        (210)    16079 2023-02-14 18:11:00.000000 femagtools-1.2.6/tests/test_fsl.py
--rw-r--r--   0 tar        (210) tar        (210)      662 2022-08-07 12:24:45.000000 femagtools-1.2.6/tests/test_im.py
--rw-r--r--   0 tar        (210) tar        (210)     2923 2022-08-07 12:24:45.000000 femagtools-1.2.6/tests/test_isa7.py
--rw-r--r--   0 tar        (210) tar        (210)      824 2022-08-07 12:24:45.000000 femagtools-1.2.6/tests/test_jhb.py
--rw-r--r--   0 tar        (210) tar        (210)      981 2022-08-07 12:24:45.000000 femagtools-1.2.6/tests/test_job.py
--rw-r--r--   0 tar        (210) tar        (210)     2012 2022-08-24 07:36:25.000000 femagtools-1.2.6/tests/test_losscoeffs.py
--rwxr-xr-x   0 tar        (210) tar        (210)    12906 2023-02-14 18:11:00.000000 femagtools-1.2.6/tests/test_machine.py
--rwxr-xr-x   0 tar        (210) tar        (210)     2608 2022-08-07 12:24:45.000000 femagtools-1.2.6/tests/test_magncurv.py
--rw-r--r--   0 tar        (210) tar        (210)      276 2022-08-07 12:24:45.000000 femagtools-1.2.6/tests/test_magnet.py
--rwxr-xr-x   0 tar        (210) tar        (210)     2118 2022-08-07 12:24:45.000000 femagtools-1.2.6/tests/test_mcvreader.py
--rwxr-xr-x   0 tar        (210) tar        (210)     3922 2022-08-07 12:24:45.000000 femagtools-1.2.6/tests/test_mcvwriter.py
--rw-r--r--   0 tar        (210) tar        (210)      192 2023-02-14 18:11:00.000000 femagtools-1.2.6/tests/test_me.py
--rwxr-xr-x   0 tar        (210) tar        (210)     2372 2022-08-07 12:24:45.000000 femagtools-1.2.6/tests/test_model.py
--rw-r--r--   0 tar        (210) tar        (210)     3116 2022-08-07 12:24:45.000000 femagtools-1.2.6/tests/test_nc.py
--rw-r--r--   0 tar        (210) tar        (210)     1323 2023-02-14 18:11:00.000000 femagtools-1.2.6/tests/test_parident.py
--rw-r--r--   0 tar        (210) tar        (210)     3200 2023-03-02 15:44:17.000000 femagtools-1.2.6/tests/test_parstudy.py
--rwxr-xr-x   0 tar        (210) tar        (210)     5816 2022-08-07 12:24:45.000000 femagtools-1.2.6/tests/test_pocfile.py
--rw-r--r--   0 tar        (210) tar        (210)     1109 2023-02-14 18:11:00.000000 femagtools-1.2.6/tests/test_sizing.py
--rw-r--r--   0 tar        (210) tar        (210)    83510 2022-08-07 12:24:45.000000 femagtools-1.2.6/tests/test_sm.py
--rwxr-xr-x   0 tar        (210) tar        (210)      766 2022-08-24 07:36:25.000000 femagtools-1.2.6/tests/test_tksreader.py
--rw-r--r--   0 tar        (210) tar        (210)     1825 2022-08-07 12:24:45.000000 femagtools-1.2.6/tests/test_ts.py
--rwxr-xr-x   0 tar        (210) tar        (210)      832 2022-08-07 12:24:45.000000 femagtools-1.2.6/tests/test_vbfreader.py
--rw-r--r--   0 tar        (210) tar        (210)      868 2022-08-07 12:24:45.000000 femagtools-1.2.6/tests/test_vtu.py
--rw-r--r--   0 tar        (210) tar        (210)     4912 2023-03-24 14:45:00.000000 femagtools-1.2.6/tests/test_windings.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-04-13 07:50:58.694537 femagtools-1.2.7/
+-rw-r--r--   0 tar        (210) tar        (210)     1316 2023-02-15 20:03:56.000000 femagtools-1.2.7/LICENSE
+-rw-r--r--   0 tar        (210) tar        (210)       35 2023-02-15 20:03:56.000000 femagtools-1.2.7/MANIFEST.in
+-rw-r--r--   0 tar        (210) tar        (210)     5262 2023-04-13 07:50:58.694537 femagtools-1.2.7/PKG-INFO
+-rw-r--r--   0 tar        (210) tar        (210)     3072 2023-02-14 18:11:00.000000 femagtools-1.2.7/README.md
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-04-13 07:50:58.677537 femagtools-1.2.7/femagtools/
+-rw-r--r--   0 tar        (210) tar        (210)     1630 2023-04-13 07:48:48.000000 femagtools-1.2.7/femagtools/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)     2250 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/airgap.py
+-rw-r--r--   0 tar        (210) tar        (210)    12122 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/amazon.py
+-rw-r--r--   0 tar        (210) tar        (210)     9741 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/amela.py
+-rw-r--r--   0 tar        (210) tar        (210)     7706 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/asm.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    68684 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/bch.py
+-rw-r--r--   0 tar        (210) tar        (210)     2923 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/bchxml.py
+-rw-r--r--   0 tar        (210) tar        (210)    10766 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/condor.py
+-rw-r--r--   0 tar        (210) tar        (210)     1076 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/conductor.py
+-rw-r--r--   0 tar        (210) tar        (210)     3087 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/config.py
+-rw-r--r--   0 tar        (210) tar        (210)    23706 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/convert.py
+-rw-r--r--   0 tar        (210) tar        (210)     7017 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/dakota.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     4064 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/dakota_femag.py
+-rw-r--r--   0 tar        (210) tar        (210)     5573 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/dakotaout.py
+-rw-r--r--   0 tar        (210) tar        (210)     7460 2023-03-24 14:45:00.000000 femagtools-1.2.7/femagtools/docker.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-04-13 07:50:58.680537 femagtools-1.2.7/femagtools/dxfsl/
+-rw-r--r--   0 tar        (210) tar        (210)        0 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/dxfsl/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)    52503 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/dxfsl/area.py
+-rw-r--r--   0 tar        (210) tar        (210)     8990 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/dxfsl/conv.py
+-rw-r--r--   0 tar        (210) tar        (210)    18787 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/dxfsl/converter.py
+-rw-r--r--   0 tar        (210) tar        (210)     1266 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/dxfsl/corner.py
+-rw-r--r--   0 tar        (210) tar        (210)     1861 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/dxfsl/dumprenderer.py
+-rw-r--r--   0 tar        (210) tar        (210)    23233 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/dxfsl/fslrenderer.py
+-rw-r--r--   0 tar        (210) tar        (210)     9835 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/dxfsl/functions.py
+-rw-r--r--   0 tar        (210) tar        (210)   132506 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/dxfsl/geom.py
+-rw-r--r--   0 tar        (210) tar        (210)    27661 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/dxfsl/machine.py
+-rw-r--r--   0 tar        (210) tar        (210)    12311 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/dxfsl/plotrenderer.py
+-rw-r--r--   0 tar        (210) tar        (210)    43088 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/dxfsl/shape.py
+-rw-r--r--   0 tar        (210) tar        (210)     1224 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/erg.py
+-rw-r--r--   0 tar        (210) tar        (210)    40619 2023-04-13 07:48:25.000000 femagtools-1.2.7/femagtools/femag.py
+-rw-r--r--   0 tar        (210) tar        (210)     7466 2023-02-15 20:03:56.000000 femagtools-1.2.7/femagtools/forcedens.py
+-rw-r--r--   0 tar        (210) tar        (210)    28180 2023-02-21 19:53:03.000000 femagtools-1.2.7/femagtools/fsl.py
+-rw-r--r--   0 tar        (210) tar        (210)     3017 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/getset.py
+-rw-r--r--   0 tar        (210) tar        (210)     3903 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/gmsh.py
+-rw-r--r--   0 tar        (210) tar        (210)    17166 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/google.py
+-rw-r--r--   0 tar        (210) tar        (210)     1561 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/grid.py
+-rw-r--r--   0 tar        (210) tar        (210)    41556 2023-04-13 07:48:25.000000 femagtools-1.2.7/femagtools/isa7.py
+-rw-r--r--   0 tar        (210) tar        (210)     2790 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/jcf2msh.py
+-rw-r--r--   0 tar        (210) tar        (210)     1779 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/jhb.py
+-rw-r--r--   0 tar        (210) tar        (210)    11320 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/job.py
+-rw-r--r--   0 tar        (210) tar        (210)     2261 2022-08-24 07:36:25.000000 femagtools-1.2.7/femagtools/losscoeffs.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-04-13 07:50:58.681537 femagtools-1.2.7/femagtools/machine/
+-rw-r--r--   0 tar        (210) tar        (210)     5613 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/machine/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)     5604 2023-04-05 06:37:05.000000 femagtools-1.2.7/femagtools/machine/effloss.py
+-rw-r--r--   0 tar        (210) tar        (210)    34847 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/machine/im.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    30631 2023-04-05 06:37:05.000000 femagtools-1.2.7/femagtools/machine/pm.py
+-rw-r--r--   0 tar        (210) tar        (210)    21743 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/machine/sizing.py
+-rw-r--r--   0 tar        (210) tar        (210)    14584 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/machine/sm.py
+-rw-r--r--   0 tar        (210) tar        (210)    16143 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/machine/utils.py
+-rw-r--r--   0 tar        (210) tar        (210)     1093 2023-02-15 20:03:56.000000 femagtools-1.2.7/femagtools/magnet.py
+-rw-r--r--   0 tar        (210) tar        (210)    38043 2023-02-16 09:09:33.000000 femagtools-1.2.7/femagtools/mcv.py
+-rw-r--r--   0 tar        (210) tar        (210)     1833 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/me.py
+-rw-r--r--   0 tar        (210) tar        (210)    14106 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/model.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-04-13 07:50:58.682537 femagtools-1.2.7/femagtools/moo/
+-rw-r--r--   0 tar        (210) tar        (210)      175 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/moo/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)     5493 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/moo/algorithm.py
+-rw-r--r--   0 tar        (210) tar        (210)    10100 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/moo/population.py
+-rw-r--r--   0 tar        (210) tar        (210)     2391 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/moo/problem.py
+-rw-r--r--   0 tar        (210) tar        (210)     2825 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/moproblem.py
+-rw-r--r--   0 tar        (210) tar        (210)     8265 2023-04-05 06:37:05.000000 femagtools-1.2.7/femagtools/multiproc.py
+-rw-r--r--   0 tar        (210) tar        (210)     1841 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/mxw2msh.py
+-rw-r--r--   0 tar        (210) tar        (210)    12781 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/nc.py
+-rw-r--r--   0 tar        (210) tar        (210)     2052 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/netlist.py
+-rw-r--r--   0 tar        (210) tar        (210)     3099 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/ntib.py
+-rw-r--r--   0 tar        (210) tar        (210)     8685 2023-02-21 19:53:03.000000 femagtools-1.2.7/femagtools/opt.py
+-rw-r--r--   0 tar        (210) tar        (210)    18733 2023-04-05 06:37:05.000000 femagtools-1.2.7/femagtools/parstudy.py
+-rw-r--r--   0 tar        (210) tar        (210)    57795 2023-04-05 06:37:05.000000 femagtools-1.2.7/femagtools/plot.py
+-rw-r--r--   0 tar        (210) tar        (210)     6536 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/poc.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-04-13 07:50:58.688537 femagtools-1.2.7/femagtools/templates/
+-rw-r--r--   0 tar        (210) tar        (210)      874 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/FE-losses.mako
+-rw-r--r--   0 tar        (210) tar        (210)      242 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/airgapinduc.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2879 2022-09-28 06:51:55.000000 femagtools-1.2.7/femagtools/templates/asyn_motor.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2483 2022-09-28 06:51:55.000000 femagtools-1.2.7/femagtools/templates/basic_modpar.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1911 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/templates/calc_field_ts.mako
+-rw-r--r--   0 tar        (210) tar        (210)      997 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/cogg_calc.mako
+-rw-r--r--   0 tar        (210) tar        (210)      400 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/colorgrad.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1264 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/com_motor_sim.mako
+-rw-r--r--   0 tar        (210) tar        (210)      472 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/templates/conduct-data.mako
+-rw-r--r--   0 tar        (210) tar        (210)      437 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/templates/connect_models.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1350 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/cu_losses.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1672 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/templates/ec-rotorbar.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1983 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/fe-contr.mako
+-rw-r--r--   0 tar        (210) tar        (210)     4289 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/gen_winding.mako
+-rw-r--r--   0 tar        (210) tar        (210)      560 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/templates/inductances.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1270 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/ld_lq_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)      600 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/templates/leak_dist_wind.mako
+-rw-r--r--   0 tar        (210) tar        (210)      770 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/leak_evol_wind.mako
+-rw-r--r--   0 tar        (210) tar        (210)      431 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/leak_tooth_wind.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1271 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/magnet-data.mako
+-rw-r--r--   0 tar        (210) tar        (210)      788 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/magnetFC2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1372 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/magnetIron.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1426 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/magnetIron2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2315 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/magnetIron3.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1413 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/magnetIron4.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1376 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/magnetIron5.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2208 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/magnetIronV.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2010 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/magnetSector.mako
+-rw-r--r--   0 tar        (210) tar        (210)      727 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/magnetSectorLinear.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1295 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/magnetShell.mako
+-rw-r--r--   0 tar        (210) tar        (210)     4080 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/magnetShell2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1094 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/templates/mesh-airgap.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2298 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/templates/modal_analysis.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1202 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/mult_cal_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)      345 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/new_model.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3209 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/templates/noloadflux-rot.mako
+-rw-r--r--   0 tar        (210) tar        (210)     4661 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/templates/noloadflux.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3146 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/templates/noloadfluxdc.mako
+-rw-r--r--   0 tar        (210) tar        (210)      313 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/open.mako
+-rw-r--r--   0 tar        (210) tar        (210)      630 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/plots.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1373 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/pm_sym_f_cur.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2319 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/pm_sym_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)      925 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/pm_sym_loss.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1251 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/psd_psq_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)      643 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/templates/ring.mako
+-rw-r--r--   0 tar        (210) tar        (210)      973 2022-09-28 06:51:55.000000 femagtools-1.2.7/femagtools/templates/rot_hsm.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2280 2022-09-28 06:51:55.000000 femagtools-1.2.7/femagtools/templates/rotorAsyn.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1908 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/templates/rotorKs2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1910 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/rotor_msh.mako
+-rw-r--r--   0 tar        (210) tar        (210)      753 2022-09-28 06:51:55.000000 femagtools-1.2.7/femagtools/templates/rotor_winding.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1981 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/shortcircuit.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2077 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/srm.mako
+-rw-r--r--   0 tar        (210) tar        (210)      761 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/stator1.mako
+-rw-r--r--   0 tar        (210) tar        (210)      599 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/stator2.mako
+-rw-r--r--   0 tar        (210) tar        (210)      724 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/stator3Linear.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1179 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/stator4.mako
+-rw-r--r--   0 tar        (210) tar        (210)      893 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/statorBG.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2071 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/templates/statorRing.mako
+-rw-r--r--   0 tar        (210) tar        (210)     4073 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/templates/statorRotor3.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1799 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/stator_msh.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1761 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/torq_calc.mako
+-rw-r--r--   0 tar        (210) tar        (210)     5791 2022-08-24 07:36:25.000000 femagtools-1.2.7/femagtools/tks.py
+-rw-r--r--   0 tar        (210) tar        (210)    47280 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/ts.py
+-rw-r--r--   0 tar        (210) tar        (210)     2444 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/vbf.py
+-rw-r--r--   0 tar        (210) tar        (210)     8595 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/vtu.py
+-rw-r--r--   0 tar        (210) tar        (210)    22279 2023-03-24 14:45:00.000000 femagtools-1.2.7/femagtools/windings.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-04-13 07:50:58.678537 femagtools-1.2.7/femagtools.egg-info/
+-rw-r--r--   0 tar        (210) tar        (210)     5262 2023-04-13 07:50:58.000000 femagtools-1.2.7/femagtools.egg-info/PKG-INFO
+-rw-r--r--   0 tar        (210) tar        (210)     4861 2023-04-13 07:50:58.000000 femagtools-1.2.7/femagtools.egg-info/SOURCES.txt
+-rw-r--r--   0 tar        (210) tar        (210)        1 2023-04-13 07:50:58.000000 femagtools-1.2.7/femagtools.egg-info/dependency_links.txt
+-rw-r--r--   0 tar        (210) tar        (210)      191 2023-04-13 07:50:58.000000 femagtools-1.2.7/femagtools.egg-info/entry_points.txt
+-rw-r--r--   0 tar        (210) tar        (210)      144 2023-04-13 07:50:58.000000 femagtools-1.2.7/femagtools.egg-info/requires.txt
+-rw-r--r--   0 tar        (210) tar        (210)       11 2023-04-13 07:50:58.000000 femagtools-1.2.7/femagtools.egg-info/top_level.txt
+-rw-r--r--   0 tar        (210) tar        (210)     1369 2023-02-15 20:03:56.000000 femagtools-1.2.7/pyproject.toml
+-rw-r--r--   0 tar        (210) tar        (210)       38 2023-04-13 07:50:58.694537 femagtools-1.2.7/setup.cfg
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-04-13 07:50:58.694537 femagtools-1.2.7/tests/
+-rw-r--r--   0 tar        (210) tar        (210)     1065 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_airgap_induction.py
+-rw-r--r--   0 tar        (210) tar        (210)      646 2023-02-14 18:11:00.000000 femagtools-1.2.7/tests/test_amela.py
+-rw-r--r--   0 tar        (210) tar        (210)     1398 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_asm.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    14755 2023-02-14 18:11:00.000000 femagtools-1.2.7/tests/test_bchreader.py
+-rw-r--r--   0 tar        (210) tar        (210)      332 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_conductor.py
+-rw-r--r--   0 tar        (210) tar        (210)     6171 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_convert.py
+-rw-r--r--   0 tar        (210) tar        (210)     1077 2023-04-05 06:37:05.000000 femagtools-1.2.7/tests/test_effloss.py
+-rw-r--r--   0 tar        (210) tar        (210)      523 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_erg.py
+-rw-r--r--   0 tar        (210) tar        (210)     1934 2023-02-16 09:09:33.000000 femagtools-1.2.7/tests/test_femag.py
+-rw-r--r--   0 tar        (210) tar        (210)      533 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_forcedens.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    16079 2023-02-14 18:11:00.000000 femagtools-1.2.7/tests/test_fsl.py
+-rw-r--r--   0 tar        (210) tar        (210)      662 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_im.py
+-rw-r--r--   0 tar        (210) tar        (210)     2923 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_isa7.py
+-rw-r--r--   0 tar        (210) tar        (210)      824 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_jhb.py
+-rw-r--r--   0 tar        (210) tar        (210)      981 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_job.py
+-rw-r--r--   0 tar        (210) tar        (210)     2012 2022-08-24 07:36:25.000000 femagtools-1.2.7/tests/test_losscoeffs.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    12906 2023-02-14 18:11:00.000000 femagtools-1.2.7/tests/test_machine.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     2608 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_magncurv.py
+-rw-r--r--   0 tar        (210) tar        (210)      276 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_magnet.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     2118 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_mcvreader.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     3922 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_mcvwriter.py
+-rw-r--r--   0 tar        (210) tar        (210)      192 2023-02-14 18:11:00.000000 femagtools-1.2.7/tests/test_me.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     2372 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_model.py
+-rw-r--r--   0 tar        (210) tar        (210)     3116 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_nc.py
+-rw-r--r--   0 tar        (210) tar        (210)     1323 2023-02-14 18:11:00.000000 femagtools-1.2.7/tests/test_parident.py
+-rw-r--r--   0 tar        (210) tar        (210)     3200 2023-03-02 15:44:17.000000 femagtools-1.2.7/tests/test_parstudy.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     5816 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_pocfile.py
+-rw-r--r--   0 tar        (210) tar        (210)     1109 2023-02-14 18:11:00.000000 femagtools-1.2.7/tests/test_sizing.py
+-rw-r--r--   0 tar        (210) tar        (210)    83510 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_sm.py
+-rwxr-xr-x   0 tar        (210) tar        (210)      766 2022-08-24 07:36:25.000000 femagtools-1.2.7/tests/test_tksreader.py
+-rw-r--r--   0 tar        (210) tar        (210)     1825 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_ts.py
+-rwxr-xr-x   0 tar        (210) tar        (210)      832 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_vbfreader.py
+-rw-r--r--   0 tar        (210) tar        (210)      868 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_vtu.py
+-rw-r--r--   0 tar        (210) tar        (210)     4912 2023-03-24 14:45:00.000000 femagtools-1.2.7/tests/test_windings.py
```

### Comparing `femagtools-1.2.6/LICENSE` & `femagtools-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/PKG-INFO` & `femagtools-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femagtools
-Version: 1.2.6
+Version: 1.2.7
 Summary: Python API for FEMAG
 Author-email: Ronald Tanner <tar@semafor.ch>, Dapu Zhang <d.zhan@gtisoft.com>, Beat Holm <hob@semafor.ch>, Günther Amsler <amg@semafor.ch>, Nicolas Mauchle <mau@semafor.ch>
 License: Copyright (c) 2016-2023, Semafor Informatik & Energie AG, Basel
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions
```

### Comparing `femagtools-1.2.6/README.md` & `femagtools-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/__init__.py` & `femagtools-1.2.7/femagtools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
     Python bindings for FEMAG
 
 
 
 """
 __title__ = 'femagtools'
-__version__ = '1.2.6'
+__version__ = '1.2.7'
 __author__ = 'Ronald Tanner'
 __license__ = 'BSD'
 __copyright__ = 'Copyright 2016-2022 SEMAFOR Informatik & Energie AG'
 
 from .asm import read
 from .bch import Reader
 from .model import MachineModel
```

### Comparing `femagtools-1.2.6/femagtools/airgap.py` & `femagtools-1.2.7/femagtools/airgap.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/amazon.py` & `femagtools-1.2.7/femagtools/amazon.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/amela.py` & `femagtools-1.2.7/femagtools/amela.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/asm.py` & `femagtools-1.2.7/femagtools/asm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/bch.py` & `femagtools-1.2.7/femagtools/bch.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/bchxml.py` & `femagtools-1.2.7/femagtools/bchxml.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/condor.py` & `femagtools-1.2.7/femagtools/condor.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/conductor.py` & `femagtools-1.2.7/femagtools/conductor.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/config.py` & `femagtools-1.2.7/femagtools/config.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/convert.py` & `femagtools-1.2.7/femagtools/convert.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/dakota.py` & `femagtools-1.2.7/femagtools/dakota.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/dakota_femag.py` & `femagtools-1.2.7/femagtools/dakota_femag.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/dakotaout.py` & `femagtools-1.2.7/femagtools/dakotaout.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/docker.py` & `femagtools-1.2.7/femagtools/docker.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/dxfsl/area.py` & `femagtools-1.2.7/femagtools/dxfsl/area.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/dxfsl/conv.py` & `femagtools-1.2.7/femagtools/dxfsl/conv.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/dxfsl/converter.py` & `femagtools-1.2.7/femagtools/dxfsl/converter.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/dxfsl/corner.py` & `femagtools-1.2.7/femagtools/dxfsl/corner.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/dxfsl/dumprenderer.py` & `femagtools-1.2.7/femagtools/dxfsl/dumprenderer.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/dxfsl/fslrenderer.py` & `femagtools-1.2.7/femagtools/dxfsl/fslrenderer.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/dxfsl/functions.py` & `femagtools-1.2.7/femagtools/dxfsl/functions.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/dxfsl/geom.py` & `femagtools-1.2.7/femagtools/dxfsl/geom.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/dxfsl/machine.py` & `femagtools-1.2.7/femagtools/dxfsl/machine.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/dxfsl/plotrenderer.py` & `femagtools-1.2.7/femagtools/dxfsl/plotrenderer.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/dxfsl/shape.py` & `femagtools-1.2.7/femagtools/dxfsl/shape.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/erg.py` & `femagtools-1.2.7/femagtools/erg.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/femag.py` & `femagtools-1.2.7/femagtools/femag.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,16 +53,20 @@
                     b'\x1b' in line or  # ignore terminal escape seq
                     b'\n' == line or
                     b'Start:' in line or
                     b'Stop:' in line or
                         b'Elapsed time:' in line):
                     continue
                 if line:
-                    logger.info(" > %s",
-                                line.decode().strip())
+                    try:
+                        logger.info(" > %s",
+                                    line.decode().strip())
+                    except UnicodeDecodeError:
+                        # ignore
+                        pass
 
 
 def get_shortCircuit_parameters(bch, nload):
     try:
         if nload < 0:
             nload = 0
         if nload > 2:
```

### Comparing `femagtools-1.2.6/femagtools/forcedens.py` & `femagtools-1.2.7/femagtools/forcedens.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/fsl.py` & `femagtools-1.2.7/femagtools/fsl.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/getset.py` & `femagtools-1.2.7/femagtools/getset.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/gmsh.py` & `femagtools-1.2.7/femagtools/gmsh.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/google.py` & `femagtools-1.2.7/femagtools/google.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/grid.py` & `femagtools-1.2.7/femagtools/grid.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/isa7.py` & `femagtools-1.2.7/femagtools/isa7.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # -*- coding: utf-8 -*-
 """
     femagtools.isa7
     ~~~~~~~~~~~~~~~
 
     Read FEMAG I7/ISA7 model files
 """
-from collections import Counter
-import numpy as np
 import re
-import pdb
 import sys
 import struct
 import logging
+from collections import Counter
+import numpy as np
 
 logger = logging.getLogger('femagtools.isa7')
 
 
 class Reader(object):
     """
     Open and Read I7/ISA7 file
@@ -396,15 +395,15 @@
             chunksize = struct.calcsize("=" + fmt_)
             offset = self.pos
             for j in range(blockSize // chunksize):
                 unpacked.append(struct.unpack_from("=" + fmt_,
                                                    self.file,
                                                    offset))
                 offset += chunksize
-            logger.info("%s: %d %d", fmt_, blockSize, len(unpacked))
+            logger.debug("%s: %d %d", fmt_, blockSize, len(unpacked))
         except struct.error as e:
             logger.warning("Invalid Blocksize %s",
                            blockSize)
 
         self.pos += blockSize + 4
 
         fmt_ = ""
@@ -469,28 +468,28 @@
         self.points = [Point(x, y)
                        for x, y in zip(reader.POINT_ISA_POINT_REC_PT_CO_X,
                                        reader.POINT_ISA_POINT_REC_PT_CO_Y)]
 
         self.lines = [Line(self.points[abs(pk1) - 1], self.points[abs(pk2) - 1])
                       for pk1, pk2 in zip(reader.LINE_ISA_LINE_REC_LN_PNT_1,
                                           reader.LINE_ISA_LINE_REC_LN_PNT_2)]
-        logger.info("Nodes")
+        logger.debug("Nodes")
         self.nodes = [
             Node(n + 1,
                  reader.NODE_ISA_NODE_REC_ND_BND_CND[n],
                  reader.NODE_ISA_NODE_REC_ND_PER_NOD[n],
                  reader.NODE_ISA_ND_CO_RAD[n],
                  reader.NODE_ISA_ND_CO_PHI[n],
                  reader.NODE_ISA_NODE_REC_ND_CO_1[n],
                  reader.NODE_ISA_NODE_REC_ND_CO_2[n],
                  reader.NODE_ISA_NODE_REC_ND_VP_RE[n],
                  reader.NODE_ISA_NODE_REC_ND_VP_IM[n])
             for n in range(len(reader.NODE_ISA_NODE_REC_ND_BND_CND))]
 
-        logger.info("Nodechains")
+        logger.debug("Nodechains")
         self.nodechains = []
         for nc in range(len(reader.NDCHN_ISA_NDCHN_REC_NC_NOD_1)):
             nd1 = reader.NDCHN_ISA_NDCHN_REC_NC_NOD_1[nc]
             nd2 = reader.NDCHN_ISA_NDCHN_REC_NC_NOD_2[nc]
             ndm = reader.NDCHN_ISA_NDCHN_REC_NC_NOD_MID[nc]
             try:
                 node1 = self.nodes[abs(nd1) - 1]
@@ -507,15 +506,15 @@
                 self.nodechains.append(
                     NodeChain(nc + 1, nodes))
             except IndexError:
                 logger.warning('IndexError in nodes')
                 raise  # preserve the stack trace
 
         self.elements = []
-        logger.info("Elements")
+        logger.debug("Elements")
         for e in range(len(reader.ELEM_ISA_EL_NOD_PNTR)):
             ndkeys = []
             ndk = reader.ELEM_ISA_EL_NOD_PNTR[e]
 
             while ndk > 0:
                 ndkeys.append(reader.ELE_NOD_ISA_ND_KEY[ndk - 1])
                 ndk = reader.ELE_NOD_ISA_NXT_ND_PNTR[ndk - 1]
@@ -538,15 +537,15 @@
                          reader.ELEM_ISA_ELEM_REC_EL_RELUC_2[e]),
                         (reader.ELEM_ISA_ELEM_REC_EL_MAG_1[e],
                          reader.ELEM_ISA_ELEM_REC_EL_MAG_2[e]),
                         loss_dens,  # in W/m³
                         reader.BR_TEMP_COEF/100,
                         temperature)   # in 1/K
             )
-        logger.info("SuperElements")
+        logger.debug("SuperElements")
         self.superelements = []
         for se in range(len(reader.SUPEL_ISA_SE_NDCHN_PNTR)):
             nc_keys = []
             nc_ptr = reader.SUPEL_ISA_SE_NDCHN_PNTR[se]
 
             while nc_ptr > 0:
                 nc_keys.append(reader.SE_NDCHN_ISA_NC_KEY[nc_ptr - 1])
@@ -594,15 +593,15 @@
                              reader.SUPEL_ISA_SUPEL_REC_SE_VEL_SYS[se],
                              reader.SUPEL_ISA_SUPEL_REC_SE_VELO_1[se],
                              reader.SUPEL_ISA_SUPEL_REC_SE_VELO_2[se],
                              reader.SUPEL_ISA_SUPEL_REC_SE_CURD_RE[se],
                              reader.SUPEL_ISA_SUPEL_REC_SE_CURD_IM[se],
                              fillfactor, temp_coef, temperature))
 
-        logger.info("Subregions")
+        logger.debug("Subregions")
         self.subregions = []
         for sr in range(len(reader.SR_ISA_SR_SE_PNTR)):
             se_keys = []
             se_ptr = reader.SR_ISA_SR_SE_PNTR[sr]
 
             while se_ptr > 0:
                 se_keys.append(reader.SR_SE_ISA_SE_KEY[se_ptr - 1])
@@ -629,15 +628,15 @@
                           reader.SR_ISA_SR_REC_SR_NAME[sr].strip(),
                           reader.SR_ISA_SR_REC_SR_NTURNS[sr],
                           reader.SR_ISA_SR_REC_SR_CUR_DIR[sr],
                           reader.SR_ISA_SR_REC_SR_WB_KEY[sr] - 1,
                           superelements,
                           nodechains))
 
-        logger.info("Windings")
+        logger.debug("Windings")
         self.windings = []
         try:
             for wd in range(len(reader.WB_ISA_WB_SR_PNTR)):
                 sr_keys = []
                 sr_ptr = reader.WB_ISA_WB_SR_PNTR[wd]
 
                 while sr_ptr > 0:
@@ -685,30 +684,30 @@
             pass
         self.pos_el_fe_induction = np.asarray(reader.pos_el_fe_induction)
         try:
             self.beta_loss = np.asarray(reader.beta_loss)
             self.curr_loss = np.array([c/np.sqrt(2) for c in reader.curr_loss])
         except AttributeError:
             pass
-        logger.info(reader.el_fe_induction_1)
+        logger.debug(reader.el_fe_induction_1)
         if len(np.asarray(reader.el_fe_induction_1).shape) > 2:
             self.el_fe_induction_1 = np.asarray(
                 reader.el_fe_induction_1).T/1000
             self.el_fe_induction_2 = np.asarray(
                 reader.el_fe_induction_2).T/1000
             self.eddy_cu_vpot = np.asarray(reader.eddy_cu_vpot).T/1000
         else:
             try:
                 self.el_fe_induction_1 = np.asarray(
                     [e for e in reader.el_fe_induction_1 if e[0]]).T/1000
                 self.el_fe_induction_2 = np.asarray(
                     [e for e in reader.el_fe_induction_2 if e[0]]).T/1000
                 self.eddy_cu_vpot = np.asarray(
                     [e for e in reader.eddy_cu_vpot if e[0]]).T/1000
-                logger.info('El Fe Induction %s', np.asarray(
+                logger.debug('El Fe Induction %s', np.asarray(
                     reader.el_fe_induction_1).shape)
             except:
                 pass
 
         self.iron_loss_coefficients = getattr(
             reader, 'iron_loss_coefficients', [])
 
@@ -805,15 +804,15 @@
         '''Returns the scale factor
         Parameters
         ----------
         None
 
         Returns
         -------
-        scale_facor : int
+        scale_factor : int
         '''
         try:
             poles = 2*self.pole_pairs
         except:
             poles = 2
         try:
             poles_sim = self.poles_sim
```

### Comparing `femagtools-1.2.6/femagtools/jcf2msh.py` & `femagtools-1.2.7/femagtools/jcf2msh.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/jhb.py` & `femagtools-1.2.7/femagtools/jhb.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/job.py` & `femagtools-1.2.7/femagtools/job.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/losscoeffs.py` & `femagtools-1.2.7/femagtools/losscoeffs.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/machine/__init__.py` & `femagtools-1.2.7/femagtools/machine/__init__.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/machine/effloss.py` & `femagtools-1.2.7/femagtools/machine/effloss.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/machine/im.py` & `femagtools-1.2.7/femagtools/machine/im.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/machine/pm.py` & `femagtools-1.2.7/femagtools/machine/pm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/machine/sizing.py` & `femagtools-1.2.7/femagtools/machine/sizing.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/machine/sm.py` & `femagtools-1.2.7/femagtools/machine/sm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/machine/utils.py` & `femagtools-1.2.7/femagtools/machine/utils.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/magnet.py` & `femagtools-1.2.7/femagtools/magnet.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/mcv.py` & `femagtools-1.2.7/femagtools/mcv.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/me.py` & `femagtools-1.2.7/femagtools/me.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/model.py` & `femagtools-1.2.7/femagtools/model.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/moo/algorithm.py` & `femagtools-1.2.7/femagtools/moo/algorithm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/moo/population.py` & `femagtools-1.2.7/femagtools/moo/population.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/moo/problem.py` & `femagtools-1.2.7/femagtools/moo/problem.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/moproblem.py` & `femagtools-1.2.7/femagtools/moproblem.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/multiproc.py` & `femagtools-1.2.7/femagtools/multiproc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/mxw2msh.py` & `femagtools-1.2.7/femagtools/mxw2msh.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/nc.py` & `femagtools-1.2.7/femagtools/nc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/netlist.py` & `femagtools-1.2.7/femagtools/netlist.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/ntib.py` & `femagtools-1.2.7/femagtools/ntib.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/opt.py` & `femagtools-1.2.7/femagtools/opt.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/parstudy.py` & `femagtools-1.2.7/femagtools/parstudy.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/plot.py` & `femagtools-1.2.7/femagtools/plot.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/poc.py` & `femagtools-1.2.7/femagtools/poc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/FE-losses.mako` & `femagtools-1.2.7/femagtools/templates/FE-losses.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/asyn_motor.mako` & `femagtools-1.2.7/femagtools/templates/asyn_motor.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/basic_modpar.mako` & `femagtools-1.2.7/femagtools/templates/basic_modpar.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/calc_field_ts.mako` & `femagtools-1.2.7/femagtools/templates/calc_field_ts.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/cogg_calc.mako` & `femagtools-1.2.7/femagtools/templates/cogg_calc.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/com_motor_sim.mako` & `femagtools-1.2.7/femagtools/templates/com_motor_sim.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/cu_losses.mako` & `femagtools-1.2.7/femagtools/templates/cu_losses.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/ec-rotorbar.mako` & `femagtools-1.2.7/femagtools/templates/ec-rotorbar.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/fe-contr.mako` & `femagtools-1.2.7/femagtools/templates/fe-contr.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/gen_winding.mako` & `femagtools-1.2.7/femagtools/templates/gen_winding.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/inductances.mako` & `femagtools-1.2.7/femagtools/templates/inductances.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/ld_lq_fast.mako` & `femagtools-1.2.7/femagtools/templates/ld_lq_fast.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/leak_dist_wind.mako` & `femagtools-1.2.7/femagtools/templates/leak_dist_wind.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/leak_evol_wind.mako` & `femagtools-1.2.7/femagtools/templates/leak_evol_wind.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/magnet-data.mako` & `femagtools-1.2.7/femagtools/templates/magnet-data.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/magnetFC2.mako` & `femagtools-1.2.7/femagtools/templates/magnetFC2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/magnetIron.mako` & `femagtools-1.2.7/femagtools/templates/magnetIron.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/magnetIron2.mako` & `femagtools-1.2.7/femagtools/templates/magnetIron2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/magnetIron3.mako` & `femagtools-1.2.7/femagtools/templates/magnetIron3.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/magnetIron4.mako` & `femagtools-1.2.7/femagtools/templates/magnetIron4.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/magnetIron5.mako` & `femagtools-1.2.7/femagtools/templates/magnetIron5.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/magnetIronV.mako` & `femagtools-1.2.7/femagtools/templates/magnetIronV.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/magnetSector.mako` & `femagtools-1.2.7/femagtools/templates/magnetSector.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/magnetSectorLinear.mako` & `femagtools-1.2.7/femagtools/templates/magnetSectorLinear.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/magnetShell.mako` & `femagtools-1.2.7/femagtools/templates/magnetShell.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/magnetShell2.mako` & `femagtools-1.2.7/femagtools/templates/magnetShell2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/mesh-airgap.mako` & `femagtools-1.2.7/femagtools/templates/mesh-airgap.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/modal_analysis.mako` & `femagtools-1.2.7/femagtools/templates/modal_analysis.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/mult_cal_fast.mako` & `femagtools-1.2.7/femagtools/templates/mult_cal_fast.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/noloadflux-rot.mako` & `femagtools-1.2.7/femagtools/templates/noloadflux-rot.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/noloadflux.mako` & `femagtools-1.2.7/femagtools/templates/noloadflux.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/noloadfluxdc.mako` & `femagtools-1.2.7/femagtools/templates/noloadfluxdc.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/plots.mako` & `femagtools-1.2.7/femagtools/templates/plots.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/pm_sym_f_cur.mako` & `femagtools-1.2.7/femagtools/templates/pm_sym_f_cur.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/pm_sym_fast.mako` & `femagtools-1.2.7/femagtools/templates/pm_sym_fast.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/pm_sym_loss.mako` & `femagtools-1.2.7/femagtools/templates/pm_sym_loss.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/psd_psq_fast.mako` & `femagtools-1.2.7/femagtools/templates/psd_psq_fast.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/ring.mako` & `femagtools-1.2.7/femagtools/templates/ring.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/rot_hsm.mako` & `femagtools-1.2.7/femagtools/templates/rot_hsm.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/rotorAsyn.mako` & `femagtools-1.2.7/femagtools/templates/rotorAsyn.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/rotorKs2.mako` & `femagtools-1.2.7/femagtools/templates/rotorKs2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/rotor_msh.mako` & `femagtools-1.2.7/femagtools/templates/rotor_msh.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/rotor_winding.mako` & `femagtools-1.2.7/femagtools/templates/rotor_winding.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/shortcircuit.mako` & `femagtools-1.2.7/femagtools/templates/shortcircuit.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/srm.mako` & `femagtools-1.2.7/femagtools/templates/srm.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/stator1.mako` & `femagtools-1.2.7/femagtools/templates/stator1.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/stator2.mako` & `femagtools-1.2.7/femagtools/templates/stator2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/stator3Linear.mako` & `femagtools-1.2.7/femagtools/templates/stator3Linear.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/stator4.mako` & `femagtools-1.2.7/femagtools/templates/stator4.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/statorBG.mako` & `femagtools-1.2.7/femagtools/templates/statorBG.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/statorRing.mako` & `femagtools-1.2.7/femagtools/templates/statorRing.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/statorRotor3.mako` & `femagtools-1.2.7/femagtools/templates/statorRotor3.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/stator_msh.mako` & `femagtools-1.2.7/femagtools/templates/stator_msh.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/templates/torq_calc.mako` & `femagtools-1.2.7/femagtools/templates/torq_calc.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/tks.py` & `femagtools-1.2.7/femagtools/tks.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/ts.py` & `femagtools-1.2.7/femagtools/ts.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/vbf.py` & `femagtools-1.2.7/femagtools/vbf.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/vtu.py` & `femagtools-1.2.7/femagtools/vtu.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools/windings.py` & `femagtools-1.2.7/femagtools/windings.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/femagtools.egg-info/PKG-INFO` & `femagtools-1.2.7/femagtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femagtools
-Version: 1.2.6
+Version: 1.2.7
 Summary: Python API for FEMAG
 Author-email: Ronald Tanner <tar@semafor.ch>, Dapu Zhang <d.zhan@gtisoft.com>, Beat Holm <hob@semafor.ch>, Günther Amsler <amg@semafor.ch>, Nicolas Mauchle <mau@semafor.ch>
 License: Copyright (c) 2016-2023, Semafor Informatik & Energie AG, Basel
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions
```

### Comparing `femagtools-1.2.6/femagtools.egg-info/SOURCES.txt` & `femagtools-1.2.7/femagtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/pyproject.toml` & `femagtools-1.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/tests/test_airgap_induction.py` & `femagtools-1.2.7/tests/test_airgap_induction.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/tests/test_amela.py` & `femagtools-1.2.7/tests/test_amela.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/tests/test_asm.py` & `femagtools-1.2.7/tests/test_asm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/tests/test_bchreader.py` & `femagtools-1.2.7/tests/test_bchreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/tests/test_convert.py` & `femagtools-1.2.7/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/tests/test_effloss.py` & `femagtools-1.2.7/tests/test_effloss.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/tests/test_erg.py` & `femagtools-1.2.7/tests/test_erg.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/tests/test_femag.py` & `femagtools-1.2.7/tests/test_femag.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/tests/test_forcedens.py` & `femagtools-1.2.7/tests/test_forcedens.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/tests/test_fsl.py` & `femagtools-1.2.7/tests/test_fsl.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/tests/test_im.py` & `femagtools-1.2.7/tests/test_im.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/tests/test_isa7.py` & `femagtools-1.2.7/tests/test_isa7.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/tests/test_jhb.py` & `femagtools-1.2.7/tests/test_jhb.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/tests/test_job.py` & `femagtools-1.2.7/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/tests/test_losscoeffs.py` & `femagtools-1.2.7/tests/test_losscoeffs.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/tests/test_machine.py` & `femagtools-1.2.7/tests/test_machine.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/tests/test_magncurv.py` & `femagtools-1.2.7/tests/test_magncurv.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/tests/test_mcvreader.py` & `femagtools-1.2.7/tests/test_mcvreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/tests/test_mcvwriter.py` & `femagtools-1.2.7/tests/test_mcvwriter.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/tests/test_model.py` & `femagtools-1.2.7/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/tests/test_nc.py` & `femagtools-1.2.7/tests/test_nc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/tests/test_parident.py` & `femagtools-1.2.7/tests/test_parident.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/tests/test_parstudy.py` & `femagtools-1.2.7/tests/test_parstudy.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/tests/test_pocfile.py` & `femagtools-1.2.7/tests/test_pocfile.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/tests/test_sizing.py` & `femagtools-1.2.7/tests/test_sizing.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/tests/test_sm.py` & `femagtools-1.2.7/tests/test_sm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/tests/test_tksreader.py` & `femagtools-1.2.7/tests/test_tksreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/tests/test_ts.py` & `femagtools-1.2.7/tests/test_ts.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/tests/test_vbfreader.py` & `femagtools-1.2.7/tests/test_vbfreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/tests/test_vtu.py` & `femagtools-1.2.7/tests/test_vtu.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.6/tests/test_windings.py` & `femagtools-1.2.7/tests/test_windings.py`

 * *Files identical despite different names*

