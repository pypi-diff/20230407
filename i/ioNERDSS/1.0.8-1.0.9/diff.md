# Comparing `tmp/ioNERDSS-1.0.8.tar.gz` & `tmp/ioNERDSS-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ioNERDSS-1.0.8.tar", last modified: Tue Apr  4 18:42:35 2023, max compression
+gzip compressed data, was "ioNERDSS-1.0.9.tar", last modified: Tue Apr  4 18:53:59 2023, max compression
```

## Comparing `ioNERDSS-1.0.8.tar` & `ioNERDSS-1.0.9.tar`

### file list

```diff
@@ -1,188 +1,188 @@
-drwxr-xr-x   0 guosikao   (501) staff       (20)        0 2023-04-04 18:42:35.347130 ioNERDSS-1.0.8/
--rw-r--r--   0 guosikao   (501) staff       (20)     1055 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/LICENCE
--rw-r--r--   0 guosikao   (501) staff       (20)      664 2023-04-04 18:42:35.346982 ioNERDSS-1.0.8/PKG-INFO
--rw-r--r--   0 guosikao   (501) staff       (20)       83 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/README.md
-drwxr-xr-x   0 guosikao   (501) staff       (20)        0 2023-04-04 18:42:35.311689 ioNERDSS-1.0.8/ioNERDSS/
--rw-r--r--   0 guosikao   (501) staff       (20)       24 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/__init__.py
-drwxr-xr-x   0 guosikao   (501) staff       (20)        0 2023-04-04 18:42:35.344007 ioNERDSS-1.0.8/ioNERDSS/functions/
--rw-r--r--   0 guosikao   (501) staff       (20)     1852 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/COM_leg_list_gen.py
--rw-r--r--   0 guosikao   (501) staff       (20)      547 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/PDB_bind_df_gen.py
--rw-r--r--   0 guosikao   (501) staff       (20)     1451 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/PDB_binding_info_df.py
--rw-r--r--   0 guosikao   (501) staff       (20)      954 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/PDB_complex_df_gen.py
--rw-r--r--   0 guosikao   (501) staff       (20)       88 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/PDB_dis_cal.py
--rw-r--r--   0 guosikao   (501) staff       (20)     1922 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/PDB_dis_df_gen.py
--rw-r--r--   0 guosikao   (501) staff       (20)      374 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/PDB_find_bond.py
--rw-r--r--   0 guosikao   (501) staff       (20)      779 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/PDB_find_complex.py
--rw-r--r--   0 guosikao   (501) staff       (20)      837 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/PDB_find_complex_df.py
--rw-r--r--   0 guosikao   (501) staff       (20)      843 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/PDB_new_pdb.py
--rw-r--r--   0 guosikao   (501) staff       (20)     1005 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/PDB_pdb_to_df.py
--rw-r--r--   0 guosikao   (501) staff       (20)      958 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/RESTART_complex_df_gen.py
--rw-r--r--   0 guosikao   (501) staff       (20)      841 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/RESTART_find_complex_df.py
--rw-r--r--   0 guosikao   (501) staff       (20)      855 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/RESTART_new_pdb.py
--rw-r--r--   0 guosikao   (501) staff       (20)      616 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/RESTART_pdb_to_df.py
--rw-r--r--   0 guosikao   (501) staff       (20)      792 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/RESTART_read_restart.py
--rw-r--r--   0 guosikao   (501) staff       (20)      877 2023-04-04 18:40:12.000000 ioNERDSS-1.0.8/ioNERDSS/functions/__init__.py
--rw-r--r--   0 guosikao   (501) staff       (20)     1203 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/angle_cal.py
--rw-r--r--   0 guosikao   (501) staff       (20)     6030 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/associate_prob_asymmetric.py
--rw-r--r--   0 guosikao   (501) staff       (20)     5003 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/associate_prob_symmetric.py
--rw-r--r--   0 guosikao   (501) staff       (20)     1954 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/complex_lifetime.py
--rw-r--r--   0 guosikao   (501) staff       (20)      177 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/cube_face.py
--rw-r--r--   0 guosikao   (501) staff       (20)      337 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/cube_face_COM_coord.py
--rw-r--r--   0 guosikao   (501) staff       (20)      373 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/cube_face_COM_leg_coord.py
--rw-r--r--   0 guosikao   (501) staff       (20)      842 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/cube_face_COM_leg_list_gen.py
--rw-r--r--   0 guosikao   (501) staff       (20)      774 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/cube_face_COM_list_gen.py
--rw-r--r--   0 guosikao   (501) staff       (20)      444 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/cube_face_input_coord.py
--rw-r--r--   0 guosikao   (501) staff       (20)      361 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/cube_face_leg_reduce.py
--rw-r--r--   0 guosikao   (501) staff       (20)      632 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/cube_face_leg_reduce_coord_gen.py
--rw-r--r--   0 guosikao   (501) staff       (20)      492 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/cube_face_vert_coord.py
--rw-r--r--   0 guosikao   (501) staff       (20)     8918 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/cube_face_write.py
--rw-r--r--   0 guosikao   (501) staff       (20)      177 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/cube_vert.py
--rw-r--r--   0 guosikao   (501) staff       (20)      288 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/cube_vert_COM_leg.py
--rw-r--r--   0 guosikao   (501) staff       (20)      909 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/cube_vert_COM_leg_gen.py
--rw-r--r--   0 guosikao   (501) staff       (20)      487 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/cube_vert_coord.py
--rw-r--r--   0 guosikao   (501) staff       (20)      484 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/cube_vert_input_coord.py
--rw-r--r--   0 guosikao   (501) staff       (20)      293 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/cube_vert_leg_reduce.py
--rw-r--r--   0 guosikao   (501) staff       (20)      522 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/cube_vert_leg_reduce_coor_gen.py
--rw-r--r--   0 guosikao   (501) staff       (20)      667 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/cube_vert_norm_input.py
--rw-r--r--   0 guosikao   (501) staff       (20)     5393 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/cube_vert_write.py
--rw-r--r--   0 guosikao   (501) staff       (20)     6169 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/dissociate_prob_asymmetric.py
--rw-r--r--   0 guosikao   (501) staff       (20)     5142 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/dissociate_prob_symmetric.py
--rw-r--r--   0 guosikao   (501) staff       (20)     1343 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/distance.py
--rw-r--r--   0 guosikao   (501) staff       (20)      177 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/dode_face.py
--rw-r--r--   0 guosikao   (501) staff       (20)     1107 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/dode_face_COM_coor.py
--rw-r--r--   0 guosikao   (501) staff       (20)      511 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/dode_face_COM_leg_coor.py
--rw-r--r--   0 guosikao   (501) staff       (20)     1656 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/dode_face_COM_leg_list_gen.py
--rw-r--r--   0 guosikao   (501) staff       (20)     1521 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/dode_face_COM_list_gen.py
--rw-r--r--   0 guosikao   (501) staff       (20)      977 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/dode_face_dodecahedron_coord.py
--rw-r--r--   0 guosikao   (501) staff       (20)      460 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/dode_face_input_coord.py
--rw-r--r--   0 guosikao   (501) staff       (20)      454 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/dode_face_leg_reduce.py
--rw-r--r--   0 guosikao   (501) staff       (20)      650 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/dode_face_leg_reduce_coor_gen.py
--rw-r--r--   0 guosikao   (501) staff       (20)    12313 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/dode_face_write.py
--rw-r--r--   0 guosikao   (501) staff       (20)      177 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/dode_vert.py
--rw-r--r--   0 guosikao   (501) staff       (20)      288 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/dode_vert_COM_leg.py
--rw-r--r--   0 guosikao   (501) staff       (20)     2053 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/dode_vert_COM_leg_gen.py
--rw-r--r--   0 guosikao   (501) staff       (20)      837 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/dode_vert_coord.py
--rw-r--r--   0 guosikao   (501) staff       (20)      489 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/dode_vert_input_coord.py
--rw-r--r--   0 guosikao   (501) staff       (20)      293 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/dode_vert_leg_reduce.py
--rw-r--r--   0 guosikao   (501) staff       (20)      522 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/dode_vert_leg_reduce_coor_gen.py
--rw-r--r--   0 guosikao   (501) staff       (20)      667 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/dode_vert_norm_input.py
--rw-r--r--   0 guosikao   (501) staff       (20)     5409 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/dode_vert_write.py
--rw-r--r--   0 guosikao   (501) staff       (20)      382 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/fitSphere.py
--rw-r--r--   0 guosikao   (501) staff       (20)     3716 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/free_energy.py
--rw-r--r--   0 guosikao   (501) staff       (20)     2904 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/growth_prob.py
-drwxr-xr-x   0 guosikao   (501) staff       (20)        0 2023-04-04 18:42:35.346718 ioNERDSS-1.0.8/ioNERDSS/functions/hist/
--rw-r--r--   0 guosikao   (501) staff       (20)      855 2023-04-04 18:40:12.000000 ioNERDSS-1.0.8/ioNERDSS/functions/hist/__init__.py
--rw-r--r--   0 guosikao   (501) staff       (20)     3558 2023-04-04 18:40:12.000000 ioNERDSS-1.0.8/ioNERDSS/functions/hist/hist_3d_time.py
--rw-r--r--   0 guosikao   (501) staff       (20)      724 2023-04-04 18:40:12.000000 ioNERDSS-1.0.8/ioNERDSS/functions/hist/hist_temp.py
--rw-r--r--   0 guosikao   (501) staff       (20)     4365 2023-04-04 18:40:12.000000 ioNERDSS-1.0.8/ioNERDSS/functions/hist/hist_time_heatmap.py
--rw-r--r--   0 guosikao   (501) staff       (20)     4830 2023-04-04 18:40:12.000000 ioNERDSS-1.0.8/ioNERDSS/functions/hist/hist_time_heatmap_fraction.py
--rw-r--r--   0 guosikao   (501) staff       (20)     4666 2023-04-04 18:40:12.000000 ioNERDSS-1.0.8/ioNERDSS/functions/hist/hist_time_heatmap_mono_count.py
--rw-r--r--   0 guosikao   (501) staff       (20)     3636 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/hist.py
--rw-r--r--   0 guosikao   (501) staff       (20)      177 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/icos_face.py
--rw-r--r--   0 guosikao   (501) staff       (20)      668 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/icos_face_COM_coord.py
--rw-r--r--   0 guosikao   (501) staff       (20)      327 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/icos_face_COM_leg_coord.py
--rw-r--r--   0 guosikao   (501) staff       (20)     1664 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/icos_face_COM_list_gen.py
--rw-r--r--   0 guosikao   (501) staff       (20)      395 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/icos_face_input_coord.py
--rw-r--r--   0 guosikao   (501) staff       (20)      369 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/icos_face_leg_reduce.py
--rw-r--r--   0 guosikao   (501) staff       (20)      508 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/icos_face_leg_reduce_coord_gen.py
--rw-r--r--   0 guosikao   (501) staff       (20)      642 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/icos_face_vert_coord.py
--rw-r--r--   0 guosikao   (501) staff       (20)     6212 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/icos_face_write.py
--rw-r--r--   0 guosikao   (501) staff       (20)      323 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/icos_vert.py
--rw-r--r--   0 guosikao   (501) staff       (20)      432 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/icos_vert_COM_leg.py
--rw-r--r--   0 guosikao   (501) staff       (20)     1529 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/icos_vert_COM_leg_gen.py
--rw-r--r--   0 guosikao   (501) staff       (20)      947 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/icos_vert_center_coor.py
--rw-r--r--   0 guosikao   (501) staff       (20)      518 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/icos_vert_check_dis.py
--rw-r--r--   0 guosikao   (501) staff       (20)      637 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/icos_vert_coord.py
--rw-r--r--   0 guosikao   (501) staff       (20)      589 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/icos_vert_input_coord.py
--rw-r--r--   0 guosikao   (501) staff       (20)      293 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/icos_vert_leg_reduce.py
--rw-r--r--   0 guosikao   (501) staff       (20)      522 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/icos_vert_leg_reduce_coor_gen.py
--rw-r--r--   0 guosikao   (501) staff       (20)      680 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/icos_vert_norm_input.py
--rw-r--r--   0 guosikao   (501) staff       (20)    11139 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/icos_vert_write.py
--rw-r--r--   0 guosikao   (501) staff       (20)     1447 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/locate_position_PDB.py
--rw-r--r--   0 guosikao   (501) staff       (20)      982 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/locate_position_restart.py
--rw-r--r--   0 guosikao   (501) staff       (20)     1861 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/max_complex.py
--rw-r--r--   0 guosikao   (501) staff       (20)     2746 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/mean_complex.py
--rw-r--r--   0 guosikao   (501) staff       (20)      206 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/mid_pt.py
--rw-r--r--   0 guosikao   (501) staff       (20)     6176 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/multi_3D_hist.py
--rw-r--r--   0 guosikao   (501) staff       (20)     6641 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/multi_heatmap.py
--rw-r--r--   0 guosikao   (501) staff       (20)     5526 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/multi_hist.py
--rw-r--r--   0 guosikao   (501) staff       (20)    13602 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/multi_hist_stacked.py
--rw-r--r--   0 guosikao   (501) staff       (20)     1831 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/multi_hist_to_csv.py
--rw-r--r--   0 guosikao   (501) staff       (20)      281 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/multi_hist_to_df.py
--rw-r--r--   0 guosikao   (501) staff       (20)     2888 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/multi_max_complex.py
--rw-r--r--   0 guosikao   (501) staff       (20)     3206 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/multi_mean_complex.py
--rw-r--r--   0 guosikao   (501) staff       (20)      177 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/octa_face.py
--rw-r--r--   0 guosikao   (501) staff       (20)      668 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/octa_face_COM_coord.py
--rw-r--r--   0 guosikao   (501) staff       (20)      327 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/octa_face_COM_leg_coord.py
--rw-r--r--   0 guosikao   (501) staff       (20)      887 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/octa_face_COM_leg_list_gen.py
--rw-r--r--   0 guosikao   (501) staff       (20)      802 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/octa_face_COM_list_gen.py
--rw-r--r--   0 guosikao   (501) staff       (20)      395 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/octa_face_input_coord.py
--rw-r--r--   0 guosikao   (501) staff       (20)      364 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/octa_face_leg_reduce.py
--rw-r--r--   0 guosikao   (501) staff       (20)      585 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/octa_face_leg_reduce_coord_gen.py
--rw-r--r--   0 guosikao   (501) staff       (20)      430 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/octa_face_vert_coord.py
--rw-r--r--   0 guosikao   (501) staff       (20)     6189 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/octa_face_write.py
--rw-r--r--   0 guosikao   (501) staff       (20)      177 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/octa_vert.py
--rw-r--r--   0 guosikao   (501) staff       (20)      345 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/octa_vert_COM_leg.py
--rw-r--r--   0 guosikao   (501) staff       (20)      785 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/octa_vert_COM_leg_gen.py
--rw-r--r--   0 guosikao   (501) staff       (20)      425 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/octa_vert_coord.py
--rw-r--r--   0 guosikao   (501) staff       (20)      533 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/octa_vert_input_coord.py
--rw-r--r--   0 guosikao   (501) staff       (20)      293 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/octa_vert_leg_reduce.py
--rw-r--r--   0 guosikao   (501) staff       (20)      522 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/octa_vert_leg_reduce_coor_gen.py
--rw-r--r--   0 guosikao   (501) staff       (20)     7784 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/octa_vert_write.py
--rw-r--r--   0 guosikao   (501) staff       (20)     2306 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/read_cluster_lifetime.py
--rw-r--r--   0 guosikao   (501) staff       (20)     1230 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/read_file.py
--rw-r--r--   0 guosikao   (501) staff       (20)     1096 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/read_multi_hist.py
--rw-r--r--   0 guosikao   (501) staff       (20)     1839 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/read_transition_matrix.py
--rw-r--r--   0 guosikao   (501) staff       (20)    27617 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_UI.py
--rw-r--r--   0 guosikao   (501) staff       (20)     3054 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_angles.py
--rw-r--r--   0 guosikao   (501) staff       (20)     1288 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_calculate_phi.py
--rw-r--r--   0 guosikao   (501) staff       (20)     3534 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_chain_int.py
--rw-r--r--   0 guosikao   (501) staff       (20)      529 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_data_check.py
--rw-r--r--   0 guosikao   (501) staff       (20)       82 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_mag.py
--rw-r--r--   0 guosikao   (501) staff       (20)     2439 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_norm_check.py
--rw-r--r--   0 guosikao   (501) staff       (20)      521 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_norm_input.py
--rw-r--r--   0 guosikao   (501) staff       (20)      739 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_separate_COM.py
--rw-r--r--   0 guosikao   (501) staff       (20)     2507 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_separate_angle.py
--rw-r--r--   0 guosikao   (501) staff       (20)     1755 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_separate_filter.py
--rw-r--r--   0 guosikao   (501) staff       (20)     9215 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_separate_read.py
--rw-r--r--   0 guosikao   (501) staff       (20)     6523 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_separate_sigma.py
--rw-r--r--   0 guosikao   (501) staff       (20)     4607 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_separate_write.py
--rw-r--r--   0 guosikao   (501) staff       (20)     1795 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_show_3D.py
--rw-r--r--   0 guosikao   (501) staff       (20)     2109 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_show_PDB.py
--rw-r--r--   0 guosikao   (501) staff       (20)      335 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_triangle_correction.py
--rw-r--r--   0 guosikao   (501) staff       (20)      329 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_unit.py
--rw-r--r--   0 guosikao   (501) staff       (20)     2437 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/single_hist_to_csv.py
--rw-r--r--   0 guosikao   (501) staff       (20)      285 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/single_hist_to_df.py
--rw-r--r--   0 guosikao   (501) staff       (20)      862 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/single_locate_position_restart.py
--rw-r--r--   0 guosikao   (501) staff       (20)     1213 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/single_restart_to_df.py
--rw-r--r--   0 guosikao   (501) staff       (20)     6505 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/sphere_regularization_index.py
--rw-r--r--   0 guosikao   (501) staff       (20)      177 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/tetr_face.py
--rw-r--r--   0 guosikao   (501) staff       (20)      680 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/tetr_face_COM_coord.py
--rw-r--r--   0 guosikao   (501) staff       (20)      327 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/tetr_face_COM_leg_coord.py
--rw-r--r--   0 guosikao   (501) staff       (20)      555 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/tetr_face_COM_leg_list_gen.py
--rw-r--r--   0 guosikao   (501) staff       (20)      503 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/tetr_face_COM_list_gen.py
--rw-r--r--   0 guosikao   (501) staff       (20)      421 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/tetr_face_coord.py
--rw-r--r--   0 guosikao   (501) staff       (20)      395 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/tetr_face_input_coord.py
--rw-r--r--   0 guosikao   (501) staff       (20)      363 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/tetr_face_leg_reduce.py
--rw-r--r--   0 guosikao   (501) staff       (20)      585 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/tetr_face_leg_reduce_coord_gen.py
--rw-r--r--   0 guosikao   (501) staff       (20)     6208 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/tetr_face_write.py
--rw-r--r--   0 guosikao   (501) staff       (20)      177 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/tetr_vert.py
--rw-r--r--   0 guosikao   (501) staff       (20)      288 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/tetr_vert_COM_leg.py
--rw-r--r--   0 guosikao   (501) staff       (20)      541 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/tetr_vert_COM_leg_gen.py
--rw-r--r--   0 guosikao   (501) staff       (20)      421 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/tetr_vert_coord.py
--rw-r--r--   0 guosikao   (501) staff       (20)      484 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/tetr_vert_input_coord.py
--rw-r--r--   0 guosikao   (501) staff       (20)      293 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/tetr_vert_leg_reduce.py
--rw-r--r--   0 guosikao   (501) staff       (20)      588 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/tetr_vert_leg_reduce_coor_gen.py
--rw-r--r--   0 guosikao   (501) staff       (20)      667 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/tetr_vert_norm_input.py
--rw-r--r--   0 guosikao   (501) staff       (20)     5380 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/tetr_vert_write.py
--rw-r--r--   0 guosikao   (501) staff       (20)      984 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/traj_track.py
--rw-r--r--   0 guosikao   (501) staff       (20)     1385 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/xyz_to_csv.py
--rw-r--r--   0 guosikao   (501) staff       (20)      416 2023-04-01 07:11:37.000000 ioNERDSS-1.0.8/ioNERDSS/functions/xyz_to_df.py
-drwxr-xr-x   0 guosikao   (501) staff       (20)        0 2023-04-04 18:42:35.312364 ioNERDSS-1.0.8/ioNERDSS.egg-info/
--rw-r--r--   0 guosikao   (501) staff       (20)      664 2023-04-04 18:42:35.000000 ioNERDSS-1.0.8/ioNERDSS.egg-info/PKG-INFO
--rw-r--r--   0 guosikao   (501) staff       (20)     7330 2023-04-04 18:42:35.000000 ioNERDSS-1.0.8/ioNERDSS.egg-info/SOURCES.txt
--rw-r--r--   0 guosikao   (501) staff       (20)        1 2023-04-04 18:42:35.000000 ioNERDSS-1.0.8/ioNERDSS.egg-info/dependency_links.txt
--rw-r--r--   0 guosikao   (501) staff       (20)       24 2023-04-04 18:42:35.000000 ioNERDSS-1.0.8/ioNERDSS.egg-info/requires.txt
--rw-r--r--   0 guosikao   (501) staff       (20)        9 2023-04-04 18:42:35.000000 ioNERDSS-1.0.8/ioNERDSS.egg-info/top_level.txt
--rw-r--r--   0 guosikao   (501) staff       (20)       38 2023-04-04 18:42:35.347170 ioNERDSS-1.0.8/setup.cfg
--rw-r--r--   0 guosikao   (501) staff       (20)      848 2023-04-04 18:42:26.000000 ioNERDSS-1.0.8/setup.py
+drwxr-xr-x   0 guosikao   (501) staff       (20)        0 2023-04-04 18:53:59.740414 ioNERDSS-1.0.9/
+-rw-r--r--   0 guosikao   (501) staff       (20)     1055 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/LICENCE
+-rw-r--r--   0 guosikao   (501) staff       (20)      664 2023-04-04 18:53:59.740246 ioNERDSS-1.0.9/PKG-INFO
+-rw-r--r--   0 guosikao   (501) staff       (20)       83 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/README.md
+drwxr-xr-x   0 guosikao   (501) staff       (20)        0 2023-04-04 18:53:59.708207 ioNERDSS-1.0.9/ioNERDSS/
+-rw-r--r--   0 guosikao   (501) staff       (20)       23 2023-04-04 18:53:37.000000 ioNERDSS-1.0.9/ioNERDSS/__init__.py
+drwxr-xr-x   0 guosikao   (501) staff       (20)        0 2023-04-04 18:53:59.739012 ioNERDSS-1.0.9/ioNERDSS/functions/
+-rw-r--r--   0 guosikao   (501) staff       (20)     1852 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/COM_leg_list_gen.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      547 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/PDB_bind_df_gen.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     1451 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/PDB_binding_info_df.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      954 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/PDB_complex_df_gen.py
+-rw-r--r--   0 guosikao   (501) staff       (20)       88 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/PDB_dis_cal.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     1922 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/PDB_dis_df_gen.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      374 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/PDB_find_bond.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      779 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/PDB_find_complex.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      837 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/PDB_find_complex_df.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      843 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/PDB_new_pdb.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     1005 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/PDB_pdb_to_df.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      958 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/RESTART_complex_df_gen.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      841 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/RESTART_find_complex_df.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      855 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/RESTART_new_pdb.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      616 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/RESTART_pdb_to_df.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      792 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/RESTART_read_restart.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      881 2023-04-04 18:53:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/__init__.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     1203 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/angle_cal.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     6030 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/associate_prob_asymmetric.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     5003 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/associate_prob_symmetric.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     1954 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/complex_lifetime.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      177 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/cube_face.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      337 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/cube_face_COM_coord.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      373 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/cube_face_COM_leg_coord.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      842 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/cube_face_COM_leg_list_gen.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      774 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/cube_face_COM_list_gen.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      444 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/cube_face_input_coord.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      361 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/cube_face_leg_reduce.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      632 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/cube_face_leg_reduce_coord_gen.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      492 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/cube_face_vert_coord.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     8918 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/cube_face_write.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      177 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/cube_vert.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      288 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/cube_vert_COM_leg.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      909 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/cube_vert_COM_leg_gen.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      487 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/cube_vert_coord.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      484 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/cube_vert_input_coord.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      293 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/cube_vert_leg_reduce.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      522 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/cube_vert_leg_reduce_coor_gen.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      667 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/cube_vert_norm_input.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     5393 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/cube_vert_write.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     6169 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/dissociate_prob_asymmetric.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     5142 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/dissociate_prob_symmetric.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     1343 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/distance.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      177 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/dode_face.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     1107 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/dode_face_COM_coor.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      511 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/dode_face_COM_leg_coor.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     1656 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/dode_face_COM_leg_list_gen.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     1521 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/dode_face_COM_list_gen.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      977 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/dode_face_dodecahedron_coord.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      460 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/dode_face_input_coord.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      454 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/dode_face_leg_reduce.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      650 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/dode_face_leg_reduce_coor_gen.py
+-rw-r--r--   0 guosikao   (501) staff       (20)    12313 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/dode_face_write.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      177 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/dode_vert.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      288 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/dode_vert_COM_leg.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     2053 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/dode_vert_COM_leg_gen.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      837 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/dode_vert_coord.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      489 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/dode_vert_input_coord.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      293 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/dode_vert_leg_reduce.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      522 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/dode_vert_leg_reduce_coor_gen.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      667 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/dode_vert_norm_input.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     5409 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/dode_vert_write.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      382 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/fitSphere.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     3716 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/free_energy.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     2904 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/growth_prob.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     3634 2023-04-04 18:53:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/hist.py
+drwxr-xr-x   0 guosikao   (501) staff       (20)        0 2023-04-04 18:53:59.739982 ioNERDSS-1.0.9/ioNERDSS/functions/hist_dir/
+-rw-r--r--   0 guosikao   (501) staff       (20)      855 2023-04-04 18:53:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/hist_dir/__init__.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     3558 2023-04-04 18:53:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/hist_dir/hist_3d_time.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      724 2023-04-04 18:53:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/hist_dir/hist_temp.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     4365 2023-04-04 18:53:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/hist_dir/hist_time_heatmap.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     4830 2023-04-04 18:53:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/hist_dir/hist_time_heatmap_fraction.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     4666 2023-04-04 18:53:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/hist_dir/hist_time_heatmap_mono_count.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     1230 2023-04-04 18:53:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/hist_dir/read_file.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      177 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/icos_face.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      668 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/icos_face_COM_coord.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      327 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/icos_face_COM_leg_coord.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     1664 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/icos_face_COM_list_gen.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      395 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/icos_face_input_coord.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      369 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/icos_face_leg_reduce.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      508 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/icos_face_leg_reduce_coord_gen.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      642 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/icos_face_vert_coord.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     6212 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/icos_face_write.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      323 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/icos_vert.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      432 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/icos_vert_COM_leg.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     1529 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/icos_vert_COM_leg_gen.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      947 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/icos_vert_center_coor.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      518 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/icos_vert_check_dis.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      637 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/icos_vert_coord.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      589 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/icos_vert_input_coord.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      293 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/icos_vert_leg_reduce.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      522 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/icos_vert_leg_reduce_coor_gen.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      680 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/icos_vert_norm_input.py
+-rw-r--r--   0 guosikao   (501) staff       (20)    11139 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/icos_vert_write.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     1447 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/locate_position_PDB.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      982 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/locate_position_restart.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     1870 2023-04-04 18:53:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/max_complex.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     2755 2023-04-04 18:53:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/mean_complex.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      206 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/mid_pt.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     6176 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/multi_3D_hist.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     6641 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/multi_heatmap.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     5526 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/multi_hist.py
+-rw-r--r--   0 guosikao   (501) staff       (20)    13602 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/multi_hist_stacked.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     1831 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/multi_hist_to_csv.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      281 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/multi_hist_to_df.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     2892 2023-04-04 18:53:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/multi_max_complex.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     3210 2023-04-04 18:53:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/multi_mean_complex.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      177 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/octa_face.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      668 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/octa_face_COM_coord.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      327 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/octa_face_COM_leg_coord.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      887 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/octa_face_COM_leg_list_gen.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      802 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/octa_face_COM_list_gen.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      395 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/octa_face_input_coord.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      364 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/octa_face_leg_reduce.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      585 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/octa_face_leg_reduce_coord_gen.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      430 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/octa_face_vert_coord.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     6189 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/octa_face_write.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      177 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/octa_vert.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      345 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/octa_vert_COM_leg.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      785 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/octa_vert_COM_leg_gen.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      425 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/octa_vert_coord.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      533 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/octa_vert_input_coord.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      293 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/octa_vert_leg_reduce.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      522 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/octa_vert_leg_reduce_coor_gen.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     7784 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/octa_vert_write.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     2306 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/read_cluster_lifetime.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     1096 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/read_multi_hist.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     1839 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/read_transition_matrix.py
+-rw-r--r--   0 guosikao   (501) staff       (20)    27617 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_UI.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     3054 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_angles.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     1288 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_calculate_phi.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     3534 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_chain_int.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      529 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_data_check.py
+-rw-r--r--   0 guosikao   (501) staff       (20)       82 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_mag.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     2439 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_norm_check.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      521 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_norm_input.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      739 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_separate_COM.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     2507 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_separate_angle.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     1755 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_separate_filter.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     9215 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_separate_read.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     6523 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_separate_sigma.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     4607 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_separate_write.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     1795 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_show_3D.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     2109 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_show_PDB.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      335 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_triangle_correction.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      329 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_unit.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     2437 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/single_hist_to_csv.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      285 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/single_hist_to_df.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      862 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/single_locate_position_restart.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     1213 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/single_restart_to_df.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     6509 2023-04-04 18:53:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/sphere_regularization_index.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      177 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/tetr_face.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      680 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/tetr_face_COM_coord.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      327 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/tetr_face_COM_leg_coord.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      555 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/tetr_face_COM_leg_list_gen.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      503 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/tetr_face_COM_list_gen.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      421 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/tetr_face_coord.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      395 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/tetr_face_input_coord.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      363 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/tetr_face_leg_reduce.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      585 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/tetr_face_leg_reduce_coord_gen.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     6208 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/tetr_face_write.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      177 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/tetr_vert.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      288 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/tetr_vert_COM_leg.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      541 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/tetr_vert_COM_leg_gen.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      421 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/tetr_vert_coord.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      484 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/tetr_vert_input_coord.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      293 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/tetr_vert_leg_reduce.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      588 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/tetr_vert_leg_reduce_coor_gen.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      667 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/tetr_vert_norm_input.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     5380 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/tetr_vert_write.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      984 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/traj_track.py
+-rw-r--r--   0 guosikao   (501) staff       (20)     1385 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/xyz_to_csv.py
+-rw-r--r--   0 guosikao   (501) staff       (20)      416 2023-04-01 07:11:37.000000 ioNERDSS-1.0.9/ioNERDSS/functions/xyz_to_df.py
+drwxr-xr-x   0 guosikao   (501) staff       (20)        0 2023-04-04 18:53:59.708884 ioNERDSS-1.0.9/ioNERDSS.egg-info/
+-rw-r--r--   0 guosikao   (501) staff       (20)      664 2023-04-04 18:53:59.000000 ioNERDSS-1.0.9/ioNERDSS.egg-info/PKG-INFO
+-rw-r--r--   0 guosikao   (501) staff       (20)     7363 2023-04-04 18:53:59.000000 ioNERDSS-1.0.9/ioNERDSS.egg-info/SOURCES.txt
+-rw-r--r--   0 guosikao   (501) staff       (20)        1 2023-04-04 18:53:59.000000 ioNERDSS-1.0.9/ioNERDSS.egg-info/dependency_links.txt
+-rw-r--r--   0 guosikao   (501) staff       (20)       24 2023-04-04 18:53:59.000000 ioNERDSS-1.0.9/ioNERDSS.egg-info/requires.txt
+-rw-r--r--   0 guosikao   (501) staff       (20)        9 2023-04-04 18:53:59.000000 ioNERDSS-1.0.9/ioNERDSS.egg-info/top_level.txt
+-rw-r--r--   0 guosikao   (501) staff       (20)       38 2023-04-04 18:53:59.740450 ioNERDSS-1.0.9/setup.cfg
+-rw-r--r--   0 guosikao   (501) staff       (20)      848 2023-04-04 18:53:51.000000 ioNERDSS-1.0.9/setup.py
```

### Comparing `ioNERDSS-1.0.8/LICENCE` & `ioNERDSS-1.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/PKG-INFO` & `ioNERDSS-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ioNERDSS
-Version: 1.0.8
+Version: 1.0.9
 Summary: Package for analysing NERDSS inputs and outputs.
 Home-page: 
 Author: Zixiu (Hugh) Liu
 Author-email: zliu140@jhu.edu
 License: MIT
 Keywords: NERDSS Simulation,Analysis Tools
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/COM_leg_list_gen.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/COM_leg_list_gen.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/PDB_bind_df_gen.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/PDB_bind_df_gen.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/PDB_binding_info_df.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/PDB_binding_info_df.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/PDB_complex_df_gen.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/PDB_complex_df_gen.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/PDB_dis_df_gen.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/PDB_dis_df_gen.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/PDB_find_complex.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/PDB_find_complex.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/PDB_find_complex_df.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/PDB_find_complex_df.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/PDB_new_pdb.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/PDB_new_pdb.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/PDB_pdb_to_df.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/PDB_pdb_to_df.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/RESTART_complex_df_gen.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/RESTART_complex_df_gen.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/RESTART_find_complex_df.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/RESTART_find_complex_df.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/RESTART_new_pdb.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/RESTART_new_pdb.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/RESTART_pdb_to_df.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/RESTART_pdb_to_df.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/RESTART_read_restart.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/RESTART_read_restart.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/__init__.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .hist import *
+from .hist_dir import *
 
 
 import os
 import importlib
 
 # Get the directory of the current __init__.py file
 current_directory = os.path.dirname(__file__)
```

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/angle_cal.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/angle_cal.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/associate_prob_asymmetric.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/associate_prob_asymmetric.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/associate_prob_symmetric.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/associate_prob_symmetric.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/complex_lifetime.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/complex_lifetime.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/cube_face_COM_leg_list_gen.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/cube_face_COM_leg_list_gen.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/cube_face_COM_list_gen.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/cube_face_COM_list_gen.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/cube_face_leg_reduce_coord_gen.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/cube_face_leg_reduce_coord_gen.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/cube_face_write.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/cube_face_write.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/cube_vert_COM_leg_gen.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/cube_vert_COM_leg_gen.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/cube_vert_leg_reduce_coor_gen.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/cube_vert_leg_reduce_coor_gen.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/cube_vert_norm_input.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/cube_vert_norm_input.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/cube_vert_write.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/cube_vert_write.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/dissociate_prob_asymmetric.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/dissociate_prob_asymmetric.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/dissociate_prob_symmetric.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/dissociate_prob_symmetric.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/distance.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/distance.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/dode_face_COM_coor.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/dode_face_COM_coor.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/dode_face_COM_leg_list_gen.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/dode_face_COM_leg_list_gen.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/dode_face_COM_list_gen.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/dode_face_COM_list_gen.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/dode_face_dodecahedron_coord.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/dode_face_dodecahedron_coord.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/dode_face_leg_reduce_coor_gen.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/dode_face_leg_reduce_coor_gen.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/dode_face_write.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/dode_face_write.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/dode_vert_COM_leg_gen.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/dode_vert_COM_leg_gen.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/dode_vert_coord.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/dode_vert_coord.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/dode_vert_leg_reduce_coor_gen.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/dode_vert_leg_reduce_coor_gen.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/dode_vert_norm_input.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/dode_vert_norm_input.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/dode_vert_write.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/dode_vert_write.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/free_energy.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/free_energy.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/growth_prob.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/growth_prob.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/hist/__init__.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/hist_dir/__init__.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/hist/hist_3d_time.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/hist_dir/hist_3d_time.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/hist/hist_temp.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/hist_dir/hist_temp.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/hist/hist_time_heatmap.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/hist_dir/hist_time_heatmap.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/hist/hist_time_heatmap_fraction.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/hist_dir/hist_time_heatmap_fraction.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/hist/hist_time_heatmap_mono_count.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/hist_dir/hist_time_heatmap_mono_count.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/hist.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/hist.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import matplotlib.pyplot as plt
-from .read_file import read_file
+from hist_dir import read_file
 
 
 def hist(FileName: str, FileNum: int, InitialTime: float, FinalTime: float, SpeciesName: str,
          BarSize: int = 1, ShowFig: bool = True, SaveFig: bool = False):
     file_name_head = FileName.split('.')[0]
     file_name_tail = FileName.split('.')[1]
     count_list = []
```

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/icos_face_COM_coord.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/icos_face_COM_coord.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/icos_face_COM_list_gen.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/icos_face_COM_list_gen.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/icos_face_vert_coord.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/icos_face_vert_coord.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/icos_face_write.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/icos_face_write.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/icos_vert_COM_leg_gen.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/icos_vert_COM_leg_gen.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/icos_vert_center_coor.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/icos_vert_center_coor.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/icos_vert_check_dis.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/icos_vert_check_dis.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/icos_vert_coord.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/icos_vert_coord.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/icos_vert_input_coord.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/icos_vert_input_coord.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/icos_vert_leg_reduce_coor_gen.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/icos_vert_leg_reduce_coor_gen.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/icos_vert_norm_input.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/icos_vert_norm_input.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/icos_vert_write.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/icos_vert_write.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/locate_position_PDB.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/locate_position_PDB.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/locate_position_restart.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/locate_position_restart.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/max_complex.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/max_complex.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import matplotlib.pyplot as plt
-from .read_file import read_file
+from .hist_dir.read_file import read_file
 
 
 def max_complex(FileName: str, FileNum: int, InitialTime: float, FinalTime: float,
                 SpeciesName: str, ShowFig: bool = True, SaveFig: bool = False):
     file_name_head = FileName.split('.')[0]
     file_name_tail = FileName.split('.')[1]
     time_list = []
```

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/mean_complex.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/mean_complex.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import matplotlib.pyplot as plt
-from .read_file import read_file
+from .hist_dir.read_file import read_file
 
 
 def mean_complex(FileName: str, FileNum: int, InitialTime: float, FinalTime: float,
                  SpeciesName: str, ExcludeSize: int = 0, ShowFig: bool = True, SaveFig: bool = False):
     file_name_head = FileName.split('.')[0]
     file_name_tail = FileName.split('.')[1]
     time_list = []
```

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/multi_3D_hist.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/multi_3D_hist.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/multi_heatmap.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/multi_heatmap.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/multi_hist.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/multi_hist.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/multi_hist_stacked.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/multi_hist_stacked.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/multi_hist_to_csv.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/multi_hist_to_csv.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/multi_max_complex.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/multi_max_complex.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import matplotlib.pyplot as plt
-from .hist import hist
+from .hist_dir import hist
 from .read_multi_hist import read_multi_hist
 from .multi_hist import multi_hist
 
 
 def multi_max_complex(FileName: str, FileNum: int, InitialTime: float, FinalTime: float,
                       SpeciesList: list, SpeciesName: str, ShowFig: bool = True, SaveFig: bool = False):
     file_name_head = FileName.split('.')[0]
```

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/multi_mean_complex.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/multi_mean_complex.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import matplotlib.pyplot as plt
-from .hist import hist
+from .hist_dir import hist
 from .read_multi_hist import read_multi_hist
 from .multi_hist import multi_hist
 
 
 def multi_mean_complex(FileName: str, FileNum: int, InitialTime: float, FinalTime: float,
                        SpeciesList: list, SpeciesName: str, ExcludeSize: int = 0, ShowFig: bool = True, SaveFig: bool = False):
```

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/octa_face_COM_coord.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/octa_face_COM_coord.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/octa_face_COM_leg_list_gen.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/octa_face_COM_leg_list_gen.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/octa_face_COM_list_gen.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/octa_face_COM_list_gen.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/octa_face_leg_reduce_coord_gen.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/octa_face_leg_reduce_coord_gen.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/octa_face_write.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/octa_face_write.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/octa_vert_COM_leg_gen.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/octa_vert_COM_leg_gen.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/octa_vert_input_coord.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/octa_vert_input_coord.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/octa_vert_leg_reduce_coor_gen.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/octa_vert_leg_reduce_coor_gen.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/octa_vert_write.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/octa_vert_write.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/read_cluster_lifetime.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/read_cluster_lifetime.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/read_file.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/hist_dir/read_file.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/read_multi_hist.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/read_multi_hist.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/read_transition_matrix.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/read_transition_matrix.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_UI.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_UI.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_angles.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_angles.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_calculate_phi.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_calculate_phi.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_chain_int.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_chain_int.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_data_check.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_data_check.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_norm_check.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_norm_check.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_norm_input.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_norm_input.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_separate_COM.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_separate_COM.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_separate_angle.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_separate_angle.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_separate_filter.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_separate_filter.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_separate_read.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_separate_read.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_separate_sigma.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_separate_sigma.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_separate_write.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_separate_write.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_show_3D.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_show_3D.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/real_PDB_show_PDB.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/real_PDB_show_PDB.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/single_hist_to_csv.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/single_hist_to_csv.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/single_locate_position_restart.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/single_locate_position_restart.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/single_restart_to_df.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/single_restart_to_df.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/sphere_regularization_index.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/sphere_regularization_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import warnings
-from .hist import hist
+from .hist_dir import hist
 from .fitSphere import fitSphere
 from .single_restart_to_df import single_restart_to_df
 
 
 def sphere_regularization_index(FileNameHist: str, SpeciesName: str, LitNum: int, TimeStep: float,
                                 ComplexNum: int, Radius: float):
     warnings.simplefilter("ignore")
```

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/tetr_face_COM_coord.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/tetr_face_COM_coord.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/tetr_face_COM_leg_list_gen.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/tetr_face_COM_leg_list_gen.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/tetr_face_leg_reduce_coord_gen.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/tetr_face_leg_reduce_coord_gen.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/tetr_face_write.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/tetr_face_write.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/tetr_vert_COM_leg_gen.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/tetr_vert_COM_leg_gen.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/tetr_vert_leg_reduce_coor_gen.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/tetr_vert_leg_reduce_coor_gen.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/tetr_vert_norm_input.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/tetr_vert_norm_input.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/tetr_vert_write.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/tetr_vert_write.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/traj_track.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/traj_track.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS/functions/xyz_to_csv.py` & `ioNERDSS-1.0.9/ioNERDSS/functions/xyz_to_csv.py`

 * *Files identical despite different names*

### Comparing `ioNERDSS-1.0.8/ioNERDSS.egg-info/PKG-INFO` & `ioNERDSS-1.0.9/ioNERDSS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ioNERDSS
-Version: 1.0.8
+Version: 1.0.9
 Summary: Package for analysing NERDSS inputs and outputs.
 Home-page: 
 Author: Zixiu (Hugh) Liu
 Author-email: zliu140@jhu.edu
 License: MIT
 Keywords: NERDSS Simulation,Analysis Tools
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ioNERDSS-1.0.8/ioNERDSS.egg-info/SOURCES.txt` & `ioNERDSS-1.0.9/ioNERDSS.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,14 @@
 ioNERDSS/functions/octa_vert_COM_leg_gen.py
 ioNERDSS/functions/octa_vert_coord.py
 ioNERDSS/functions/octa_vert_input_coord.py
 ioNERDSS/functions/octa_vert_leg_reduce.py
 ioNERDSS/functions/octa_vert_leg_reduce_coor_gen.py
 ioNERDSS/functions/octa_vert_write.py
 ioNERDSS/functions/read_cluster_lifetime.py
-ioNERDSS/functions/read_file.py
 ioNERDSS/functions/read_multi_hist.py
 ioNERDSS/functions/read_transition_matrix.py
 ioNERDSS/functions/real_PDB_UI.py
 ioNERDSS/functions/real_PDB_angles.py
 ioNERDSS/functions/real_PDB_calculate_phi.py
 ioNERDSS/functions/real_PDB_chain_int.py
 ioNERDSS/functions/real_PDB_data_check.py
@@ -169,13 +168,14 @@
 ioNERDSS/functions/tetr_vert_leg_reduce.py
 ioNERDSS/functions/tetr_vert_leg_reduce_coor_gen.py
 ioNERDSS/functions/tetr_vert_norm_input.py
 ioNERDSS/functions/tetr_vert_write.py
 ioNERDSS/functions/traj_track.py
 ioNERDSS/functions/xyz_to_csv.py
 ioNERDSS/functions/xyz_to_df.py
-ioNERDSS/functions/hist/__init__.py
-ioNERDSS/functions/hist/hist_3d_time.py
-ioNERDSS/functions/hist/hist_temp.py
-ioNERDSS/functions/hist/hist_time_heatmap.py
-ioNERDSS/functions/hist/hist_time_heatmap_fraction.py
-ioNERDSS/functions/hist/hist_time_heatmap_mono_count.py
+ioNERDSS/functions/hist_dir/__init__.py
+ioNERDSS/functions/hist_dir/hist_3d_time.py
+ioNERDSS/functions/hist_dir/hist_temp.py
+ioNERDSS/functions/hist_dir/hist_time_heatmap.py
+ioNERDSS/functions/hist_dir/hist_time_heatmap_fraction.py
+ioNERDSS/functions/hist_dir/hist_time_heatmap_mono_count.py
+ioNERDSS/functions/hist_dir/read_file.py
```

### Comparing `ioNERDSS-1.0.8/setup.py` & `ioNERDSS-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='ioNERDSS',
-    version='1.0.8',
+    version='1.0.9',
     description='Package for analysing NERDSS inputs and outputs.',
     long_description='A python package for analysing inputs and outputs for NERDSS simulator, including generating input files for Platonic solids and output visualization, etc.',
     url='',
     author='Zixiu (Hugh) Liu',
     author_email='zliu140@jhu.edu',
     license='MIT',
     classifiers=classifiers,
```

