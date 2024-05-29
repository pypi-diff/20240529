# Comparing `tmp/nkululeko-0.85.2.tar.gz` & `tmp/nkululeko-0.86.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkululeko-0.85.2.tar", last modified: Tue May 21 10:52:10 2024, max compression
+gzip compressed data, was "nkululeko-0.86.0.tar", last modified: Wed May 29 08:17:01 2024, max compression
```

## Comparing `nkululeko-0.85.2.tar` & `nkululeko-0.86.0.tar`

### file list

```diff
@@ -1,227 +1,226 @@
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.644683 nkululeko-0.85.2/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17943 2024-05-21 10:51:45.000000 nkululeko-0.85.2/CHANGELOG.md
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.85.2/LICENSE
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    36671 2024-05-21 10:52:10.644683 nkululeko-0.85.2/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17457 2024-04-24 09:02:29.000000 nkululeko-0.85.2/README.md
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.632683 nkululeko-0.85.2/data/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.632683 nkululeko-0.85.2/data/aesdd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1513 2023-10-04 08:46:04.000000 nkululeko-0.85.2/data/aesdd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.632683 nkululeko-0.85.2/data/androids/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-30 12:19:59.000000 nkululeko-0.85.2/data/androids/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.632683 nkululeko-0.85.2/data/androids_orig/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-20 18:21:45.000000 nkululeko-0.85.2/data/androids_orig/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.632683 nkululeko-0.85.2/data/androids_test/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-09-19 12:01:52.000000 nkululeko-0.85.2/data/androids_test/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.632683 nkululeko-0.85.2/data/ased/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1566 2023-09-19 09:19:58.000000 nkululeko-0.85.2/data/ased/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.632683 nkululeko-0.85.2/data/asvp-esd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1889 2023-09-06 07:54:15.000000 nkululeko-0.85.2/data/asvp-esd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.632683 nkululeko-0.85.2/data/baved/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1899 2023-09-12 12:11:50.000000 nkululeko-0.85.2/data/baved/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.632683 nkululeko-0.85.2/data/cafe/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1520 2023-09-11 09:21:27.000000 nkululeko-0.85.2/data/cafe/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.632683 nkululeko-0.85.2/data/clac/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1202 2023-10-04 08:46:04.000000 nkululeko-0.85.2/data/clac/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.632683 nkululeko-0.85.2/data/cmu-mosei/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1805 2023-10-20 09:59:16.000000 nkululeko-0.85.2/data/cmu-mosei/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.632683 nkululeko-0.85.2/data/demos/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2058 2023-09-19 09:19:58.000000 nkululeko-0.85.2/data/demos/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.632683 nkululeko-0.85.2/data/ekorpus/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1641 2023-09-12 12:11:50.000000 nkululeko-0.85.2/data/ekorpus/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.632683 nkululeko-0.85.2/data/emns/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2073 2023-09-19 09:19:58.000000 nkululeko-0.85.2/data/emns/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.632683 nkululeko-0.85.2/data/emofilm/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1305 2023-08-23 12:21:27.000000 nkululeko-0.85.2/data/emofilm/convert_to_16k.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1736 2023-08-23 06:49:28.000000 nkululeko-0.85.2/data/emofilm/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.632683 nkululeko-0.85.2/data/emorynlp/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1686 2023-09-20 08:48:00.000000 nkululeko-0.85.2/data/emorynlp/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.632683 nkululeko-0.85.2/data/emov-db/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1777 2023-12-19 12:05:21.000000 nkululeko-0.85.2/data/emov-db/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.632683 nkululeko-0.85.2/data/emovo/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1595 2023-09-19 09:19:58.000000 nkululeko-0.85.2/data/emovo/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.632683 nkululeko-0.85.2/data/emozionalmente/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9348 2023-08-23 06:49:28.000000 nkululeko-0.85.2/data/emozionalmente/create.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.632683 nkululeko-0.85.2/data/enterface/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2429 2023-09-19 09:19:58.000000 nkululeko-0.85.2/data/enterface/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.636683 nkululeko-0.85.2/data/esd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1534 2023-09-11 09:21:27.000000 nkululeko-0.85.2/data/esd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.636683 nkululeko-0.85.2/data/gerparas/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3023 2023-10-06 16:05:03.000000 nkululeko-0.85.2/data/gerparas/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.636683 nkululeko-0.85.2/data/iemocap/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3041 2023-10-04 08:46:04.000000 nkululeko-0.85.2/data/iemocap/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.636683 nkululeko-0.85.2/data/jl/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2022 2023-10-04 08:46:04.000000 nkululeko-0.85.2/data/jl/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.636683 nkululeko-0.85.2/data/jtes/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1727 2023-10-04 08:46:04.000000 nkululeko-0.85.2/data/jtes/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.636683 nkululeko-0.85.2/data/meld/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3694 2023-09-19 09:19:58.000000 nkululeko-0.85.2/data/meld/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.636683 nkululeko-0.85.2/data/mesd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2053 2023-09-19 09:19:58.000000 nkululeko-0.85.2/data/mesd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.636683 nkululeko-0.85.2/data/mess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1529 2023-09-19 09:19:58.000000 nkululeko-0.85.2/data/mess/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.636683 nkululeko-0.85.2/data/mlendsnd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1714 2023-12-19 12:05:21.000000 nkululeko-0.85.2/data/mlendsnd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.636683 nkululeko-0.85.2/data/msp-improv/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2328 2023-08-23 06:49:28.000000 nkululeko-0.85.2/data/msp-improv/process_database2.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.636683 nkululeko-0.85.2/data/msp-podcast/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-08-23 06:49:28.000000 nkululeko-0.85.2/data/msp-podcast/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.636683 nkululeko-0.85.2/data/oreau2/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1557 2023-09-19 09:19:58.000000 nkululeko-0.85.2/data/oreau2/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.636683 nkululeko-0.85.2/data/portuguese/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3892 2023-09-12 12:11:50.000000 nkululeko-0.85.2/data/portuguese/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.636683 nkululeko-0.85.2/data/ravdess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3612 2024-04-22 09:09:10.000000 nkululeko-0.85.2/data/ravdess/process_database.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3144 2023-10-06 16:05:03.000000 nkululeko-0.85.2/data/ravdess/process_database_speaker.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.636683 nkululeko-0.85.2/data/savee/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1680 2023-09-19 09:19:58.000000 nkululeko-0.85.2/data/savee/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.636683 nkululeko-0.85.2/data/shemo/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1624 2023-09-19 09:19:58.000000 nkululeko-0.85.2/data/shemo/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.636683 nkululeko-0.85.2/data/subesco/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2991 2023-09-19 09:19:58.000000 nkululeko-0.85.2/data/subesco/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.636683 nkululeko-0.85.2/data/tess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1472 2023-09-11 09:21:27.000000 nkululeko-0.85.2/data/tess/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.636683 nkululeko-0.85.2/data/thorsten-emotional/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1142 2023-09-06 07:54:15.000000 nkululeko-0.85.2/data/thorsten-emotional/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.636683 nkululeko-0.85.2/data/urdu/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1803 2023-09-19 09:19:58.000000 nkululeko-0.85.2/data/urdu/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.636683 nkululeko-0.85.2/data/vivae/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1209 2023-09-12 12:11:50.000000 nkululeko-0.85.2/data/vivae/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.632683 nkululeko-0.85.2/docs/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.636683 nkululeko-0.85.2/docs/source/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3070 2024-04-22 09:09:10.000000 nkululeko-0.85.2/docs/source/conf.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.632683 nkululeko-0.85.2/meta/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.636683 nkululeko-0.85.2/meta/demos/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      617 2021-10-28 13:49:53.000000 nkululeko-0.85.2/meta/demos/demo_best_model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1252 2022-12-07 09:32:42.000000 nkululeko-0.85.2/meta/demos/my_experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2022-12-15 16:06:58.000000 nkululeko-0.85.2/meta/demos/my_experiment_local.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      681 2021-10-28 13:49:53.000000 nkululeko-0.85.2/meta/demos/plot_faster_anim.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.640684 nkululeko-0.85.2/nkululeko/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-08-31 11:56:33.000000 nkululeko-0.85.2/nkululeko/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3194 2024-02-29 11:07:44.000000 nkululeko-0.85.2/nkululeko/aug_train.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3051 2024-02-29 11:04:02.000000 nkululeko-0.85.2/nkululeko/augment.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.640684 nkululeko-0.85.2/nkululeko/augmenting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:16:55.000000 nkululeko-0.85.2/nkululeko/augmenting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2905 2023-12-29 16:48:37.000000 nkululeko-0.85.2/nkululeko/augmenting/augmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2669 2023-12-29 16:49:20.000000 nkululeko-0.85.2/nkululeko/augmenting/randomsplicer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1791 2023-09-07 11:33:33.000000 nkululeko-0.85.2/nkululeko/augmenting/randomsplicing.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3542 2024-05-13 11:40:51.000000 nkululeko-0.85.2/nkululeko/augmenting/resampler.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.640684 nkululeko-0.85.2/nkululeko/autopredict/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:02.000000 nkululeko-0.85.2/nkululeko/autopredict/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2023-12-19 11:16:15.000000 nkululeko-0.85.2/nkululeko/autopredict/ap_age.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.85.2/nkululeko/autopredict/ap_arousal.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1039 2023-12-19 11:16:15.000000 nkululeko-0.85.2/nkululeko/autopredict/ap_dominance.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1008 2023-12-19 11:16:15.000000 nkululeko-0.85.2/nkululeko/autopredict/ap_gender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1104 2023-12-19 11:16:16.000000 nkululeko-0.85.2/nkululeko/autopredict/ap_mos.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1137 2023-12-19 11:16:15.000000 nkululeko-0.85.2/nkululeko/autopredict/ap_pesq.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1185 2023-12-19 11:16:16.000000 nkululeko-0.85.2/nkululeko/autopredict/ap_sdr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1107 2023-12-19 11:16:15.000000 nkululeko-0.85.2/nkululeko/autopredict/ap_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1184 2023-12-19 11:16:15.000000 nkululeko-0.85.2/nkululeko/autopredict/ap_stoi.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.85.2/nkululeko/autopredict/ap_valence.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5048 2024-04-22 09:09:10.000000 nkululeko-0.85.2/nkululeko/autopredict/estimate_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      969 2023-09-07 11:39:39.000000 nkululeko-0.85.2/nkululeko/cacheddataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       39 2024-05-21 10:50:54.000000 nkululeko-0.85.2/nkululeko/constants.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.640684 nkululeko-0.85.2/nkululeko/data/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:06.000000 nkululeko-0.85.2/nkululeko/data/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    27650 2024-04-22 09:10:47.000000 nkululeko-0.85.2/nkululeko/data/dataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3933 2024-05-21 10:44:53.000000 nkululeko-0.85.2/nkululeko/data/dataset_csv.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3232 2024-05-03 09:55:35.000000 nkululeko-0.85.2/nkululeko/demo.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2025 2024-02-29 21:51:15.000000 nkululeko-0.85.2/nkululeko/demo_feats.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4757 2024-05-03 09:56:14.000000 nkululeko-0.85.2/nkululeko/demo_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    30722 2024-05-21 10:44:53.000000 nkululeko-0.85.2/nkululeko/experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2609 2024-04-30 15:24:17.000000 nkululeko-0.85.2/nkululeko/explore.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4632 2023-12-19 11:16:14.000000 nkululeko-0.85.2/nkululeko/export.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.640684 nkululeko-0.85.2/nkululeko/feat_extract/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:10.000000 nkululeko-0.85.2/nkululeko/feat_extract/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3113 2024-04-23 09:16:18.000000 nkululeko-0.85.2/nkululeko/feat_extract/feats_agender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3424 2024-04-29 13:37:24.000000 nkululeko-0.85.2/nkululeko/feat_extract/feats_agender_agender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12722 2024-05-03 14:41:56.000000 nkululeko-0.85.2/nkululeko/feat_extract/feats_analyser.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3162 2024-04-23 09:16:18.000000 nkululeko-0.85.2/nkululeko/feat_extract/feats_auddim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3187 2024-04-23 09:16:18.000000 nkululeko-0.85.2/nkululeko/feat_extract/feats_audmodel.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3489 2024-04-23 09:16:18.000000 nkululeko-0.85.2/nkululeko/feat_extract/feats_clap.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5196 2024-04-24 17:12:28.000000 nkululeko-0.85.2/nkululeko/feat_extract/feats_hubert.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1622 2024-04-23 09:55:16.000000 nkululeko-0.85.2/nkululeko/feat_extract/feats_import.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2021 2023-12-19 11:16:16.000000 nkululeko-0.85.2/nkululeko/feat_extract/feats_mld.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4174 2024-04-23 10:17:00.000000 nkululeko-0.85.2/nkululeko/feat_extract/feats_mos.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3978 2024-04-24 10:46:37.000000 nkululeko-0.85.2/nkululeko/feat_extract/feats_opensmile.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4980 2024-04-23 09:16:18.000000 nkululeko-0.85.2/nkululeko/feat_extract/feats_oxbow.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3105 2024-04-23 09:16:18.000000 nkululeko-0.85.2/nkululeko/feat_extract/feats_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.85.2/nkululeko/feat_extract/feats_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3670 2024-04-23 09:59:48.000000 nkululeko-0.85.2/nkululeko/feat_extract/feats_spectra.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4803 2023-10-06 16:05:03.000000 nkululeko-0.85.2/nkululeko/feat_extract/feats_spkrec.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4617 2024-04-29 13:37:24.000000 nkululeko-0.85.2/nkululeko/feat_extract/feats_squim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3228 2024-04-30 09:31:46.000000 nkululeko-0.85.2/nkululeko/feat_extract/feats_trill.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5268 2024-04-29 13:37:24.000000 nkululeko-0.85.2/nkululeko/feat_extract/feats_wav2vec2.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4703 2024-04-24 17:06:22.000000 nkululeko-0.85.2/nkululeko/feat_extract/feats_wavlm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4533 2024-05-15 15:09:05.000000 nkululeko-0.85.2/nkululeko/feat_extract/feats_whisper.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1448 2024-04-23 09:16:18.000000 nkululeko-0.85.2/nkululeko/feat_extract/featureset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21304 2024-04-15 13:57:11.000000 nkululeko-0.85.2/nkululeko/feat_extract/feinberg_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3976 2024-04-23 11:13:33.000000 nkululeko-0.85.2/nkululeko/feature_extractor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3474 2023-12-19 11:16:14.000000 nkululeko-0.85.2/nkululeko/file_checker.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7222 2023-12-19 11:16:14.000000 nkululeko-0.85.2/nkululeko/filter_data.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      525 2024-05-03 12:01:14.000000 nkululeko-0.85.2/nkululeko/glob_conf.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.640684 nkululeko-0.85.2/nkululeko/losses/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:16.000000 nkululeko-0.85.2/nkululeko/losses/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      976 2023-09-07 11:37:43.000000 nkululeko-0.85.2/nkululeko/losses/loss_ccc.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1309 2023-09-26 13:42:48.000000 nkululeko-0.85.2/nkululeko/losses/loss_softf1loss.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10452 2024-05-17 12:04:16.000000 nkululeko-0.85.2/nkululeko/modelrunner.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.644683 nkululeko-0.85.2/nkululeko/models/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:20.000000 nkululeko-0.85.2/nkululeko/models/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5091 2024-05-15 15:09:05.000000 nkululeko-0.85.2/nkululeko/models/finetune_model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11639 2024-05-15 15:09:05.000000 nkululeko-0.85.2/nkululeko/models/model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2024-05-03 14:26:57.000000 nkululeko-0.85.2/nkululeko/models/model_bayes.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9954 2024-05-03 14:27:45.000000 nkululeko-0.85.2/nkululeko/models/model_cnn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      649 2024-05-03 14:28:01.000000 nkululeko-0.85.2/nkululeko/models/model_gmm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      599 2024-05-03 14:28:22.000000 nkululeko-0.85.2/nkululeko/models/model_knn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      610 2024-05-03 14:28:14.000000 nkululeko-0.85.2/nkululeko/models/model_knn_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      422 2024-05-03 14:28:34.000000 nkululeko-0.85.2/nkululeko/models/model_lin_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9854 2024-05-03 14:29:13.000000 nkululeko-0.85.2/nkululeko/models/model_mlp.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10204 2024-05-03 14:28:58.000000 nkululeko-0.85.2/nkululeko/models/model_mlp_regression.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      940 2024-05-03 14:29:24.000000 nkululeko-0.85.2/nkululeko/models/model_svm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      725 2024-05-03 14:29:39.000000 nkululeko-0.85.2/nkululeko/models/model_svr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      417 2024-05-03 14:30:08.000000 nkululeko-0.85.2/nkululeko/models/model_tree.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      428 2024-05-03 14:29:56.000000 nkululeko-0.85.2/nkululeko/models/model_tree_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    15098 2024-05-17 14:22:45.000000 nkululeko-0.85.2/nkululeko/models/model_tuned.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      447 2024-05-03 14:33:39.000000 nkululeko-0.85.2/nkululeko/models/model_xgb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      418 2024-05-03 14:34:29.000000 nkululeko-0.85.2/nkululeko/models/model_xgr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5634 2024-04-23 14:42:13.000000 nkululeko-0.85.2/nkululeko/multidb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3725 2024-04-26 06:05:26.000000 nkululeko-0.85.2/nkululeko/nkuluflag.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1968 2024-04-23 12:35:01.000000 nkululeko-0.85.2/nkululeko/nkululeko.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    23276 2024-04-29 13:37:24.000000 nkululeko-0.85.2/nkululeko/plots.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2409 2024-04-22 09:09:10.000000 nkululeko-0.85.2/nkululeko/predict.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.644683 nkululeko-0.85.2/nkululeko/reporting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-10-13 10:14:37.000000 nkululeko-0.85.2/nkululeko/reporting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      648 2023-10-02 13:54:57.000000 nkululeko-0.85.2/nkululeko/reporting/defines.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1886 2023-12-19 13:13:44.000000 nkululeko-0.85.2/nkululeko/reporting/latex_writer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1060 2023-12-19 11:16:16.000000 nkululeko-0.85.2/nkululeko/reporting/report.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      533 2023-09-26 14:51:22.000000 nkululeko-0.85.2/nkululeko/reporting/report_item.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12841 2024-04-25 13:02:38.000000 nkululeko-0.85.2/nkululeko/reporting/reporter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      742 2024-04-16 12:21:39.000000 nkululeko-0.85.2/nkululeko/reporting/result.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3354 2024-05-13 11:40:51.000000 nkululeko-0.85.2/nkululeko/resample.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7624 2024-04-22 09:09:10.000000 nkululeko-0.85.2/nkululeko/runmanager.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4101 2024-01-31 12:20:11.000000 nkululeko-0.85.2/nkululeko/scaler.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4835 2024-02-29 11:06:43.000000 nkululeko-0.85.2/nkululeko/segment.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.644683 nkululeko-0.85.2/nkululeko/segmenting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:24.000000 nkululeko-0.85.2/nkululeko/segmenting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1947 2023-09-07 11:39:09.000000 nkululeko-0.85.2/nkululeko/segmenting/seg_inaspeechsegmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3301 2023-12-19 11:16:15.000000 nkululeko-0.85.2/nkululeko/segmenting/seg_silero.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10047 2023-09-26 13:42:49.000000 nkululeko-0.85.2/nkululeko/syllable_nuclei.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1677 2024-04-26 06:04:30.000000 nkululeko-0.85.2/nkululeko/test.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3237 2024-04-25 14:01:11.000000 nkululeko-0.85.2/nkululeko/test_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8465 2024-05-15 15:09:05.000000 nkululeko-0.85.2/nkululeko/test_pretrain.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.644683 nkululeko-0.85.2/nkululeko/utils/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:28.000000 nkululeko-0.85.2/nkululeko/utils/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4021 2023-09-20 08:48:00.000000 nkululeko-0.85.2/nkululeko/utils/files.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.85.2/nkululeko/utils/stats.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    13816 2024-05-13 11:40:51.000000 nkululeko-0.85.2/nkululeko/utils/util.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.644683 nkululeko-0.85.2/nkululeko.egg-info/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    36671 2024-05-21 10:52:10.000000 nkululeko-0.85.2/nkululeko.egg-info/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5167 2024-05-21 10:52:10.000000 nkululeko-0.85.2/nkululeko.egg-info/SOURCES.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2024-05-21 10:52:10.000000 nkululeko-0.85.2/nkululeko.egg-info/dependency_links.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      298 2024-05-21 10:52:10.000000 nkululeko-0.85.2/nkululeko.egg-info/requires.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2024-05-21 10:52:10.000000 nkululeko-0.85.2/nkululeko.egg-info/top_level.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.85.2/pyproject.toml
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1001 2024-05-21 10:52:10.644683 nkululeko-0.85.2/setup.cfg
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.85.2/setup.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.632683 nkululeko-0.85.2/venv/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-21 10:52:10.644683 nkululeko-0.85.2/venv/bin/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1200 2023-12-29 19:06:16.000000 nkululeko-0.85.2/venv/bin/activate_this.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.957785 nkululeko-0.86.0/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18124 2024-05-28 14:50:25.000000 nkululeko-0.86.0/CHANGELOG.md
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.86.0/LICENSE
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    36852 2024-05-29 08:17:01.953784 nkululeko-0.86.0/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17457 2024-04-24 09:02:29.000000 nkululeko-0.86.0/README.md
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.941784 nkululeko-0.86.0/data/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/aesdd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1513 2023-10-04 08:46:04.000000 nkululeko-0.86.0/data/aesdd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/androids/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-30 12:19:59.000000 nkululeko-0.86.0/data/androids/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/androids_orig/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-20 18:21:45.000000 nkululeko-0.86.0/data/androids_orig/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/androids_test/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-09-19 12:01:52.000000 nkululeko-0.86.0/data/androids_test/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/ased/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1566 2023-09-19 09:19:58.000000 nkululeko-0.86.0/data/ased/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/asvp-esd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1889 2023-09-06 07:54:15.000000 nkululeko-0.86.0/data/asvp-esd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/baved/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1899 2023-09-12 12:11:50.000000 nkululeko-0.86.0/data/baved/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/cafe/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1520 2023-09-11 09:21:27.000000 nkululeko-0.86.0/data/cafe/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/clac/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1202 2023-10-04 08:46:04.000000 nkululeko-0.86.0/data/clac/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/cmu-mosei/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1805 2023-10-20 09:59:16.000000 nkululeko-0.86.0/data/cmu-mosei/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/demos/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2058 2023-09-19 09:19:58.000000 nkululeko-0.86.0/data/demos/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/ekorpus/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1641 2023-09-12 12:11:50.000000 nkululeko-0.86.0/data/ekorpus/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/emns/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2073 2023-09-19 09:19:58.000000 nkululeko-0.86.0/data/emns/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/emofilm/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1305 2023-08-23 12:21:27.000000 nkululeko-0.86.0/data/emofilm/convert_to_16k.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1736 2023-08-23 06:49:28.000000 nkululeko-0.86.0/data/emofilm/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/emorynlp/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1686 2023-09-20 08:48:00.000000 nkululeko-0.86.0/data/emorynlp/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/emov-db/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1777 2023-12-19 12:05:21.000000 nkululeko-0.86.0/data/emov-db/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/emovo/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1595 2023-09-19 09:19:58.000000 nkululeko-0.86.0/data/emovo/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/emozionalmente/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9348 2023-08-23 06:49:28.000000 nkululeko-0.86.0/data/emozionalmente/create.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/enterface/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2429 2023-09-19 09:19:58.000000 nkululeko-0.86.0/data/enterface/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/esd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1534 2023-09-11 09:21:27.000000 nkululeko-0.86.0/data/esd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/gerparas/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3023 2023-10-06 16:05:03.000000 nkululeko-0.86.0/data/gerparas/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/iemocap/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3041 2023-10-04 08:46:04.000000 nkululeko-0.86.0/data/iemocap/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/jl/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2022 2023-10-04 08:46:04.000000 nkululeko-0.86.0/data/jl/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/jtes/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1727 2023-10-04 08:46:04.000000 nkululeko-0.86.0/data/jtes/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/meld/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3694 2023-09-19 09:19:58.000000 nkululeko-0.86.0/data/meld/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/mesd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2053 2023-09-19 09:19:58.000000 nkululeko-0.86.0/data/mesd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/mess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1529 2023-09-19 09:19:58.000000 nkululeko-0.86.0/data/mess/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/mlendsnd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1714 2023-12-19 12:05:21.000000 nkululeko-0.86.0/data/mlendsnd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/msp-improv/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2328 2023-08-23 06:49:28.000000 nkululeko-0.86.0/data/msp-improv/process_database2.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/msp-podcast/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-08-23 06:49:28.000000 nkululeko-0.86.0/data/msp-podcast/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/oreau2/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1557 2023-09-19 09:19:58.000000 nkululeko-0.86.0/data/oreau2/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/portuguese/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3892 2023-09-12 12:11:50.000000 nkululeko-0.86.0/data/portuguese/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/ravdess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3612 2024-04-22 09:09:10.000000 nkululeko-0.86.0/data/ravdess/process_database.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3144 2023-10-06 16:05:03.000000 nkululeko-0.86.0/data/ravdess/process_database_speaker.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/savee/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1680 2023-09-19 09:19:58.000000 nkululeko-0.86.0/data/savee/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/shemo/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1624 2023-09-19 09:19:58.000000 nkululeko-0.86.0/data/shemo/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/subesco/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2991 2023-09-19 09:19:58.000000 nkululeko-0.86.0/data/subesco/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/tess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1472 2023-09-11 09:21:27.000000 nkululeko-0.86.0/data/tess/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/thorsten-emotional/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1142 2023-09-06 07:54:15.000000 nkululeko-0.86.0/data/thorsten-emotional/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/urdu/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1803 2023-09-19 09:19:58.000000 nkululeko-0.86.0/data/urdu/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/data/vivae/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1209 2023-09-12 12:11:50.000000 nkululeko-0.86.0/data/vivae/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.941784 nkululeko-0.86.0/docs/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/docs/source/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3070 2024-04-22 09:09:10.000000 nkululeko-0.86.0/docs/source/conf.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.941784 nkululeko-0.86.0/meta/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/meta/demos/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      617 2021-10-28 13:49:53.000000 nkululeko-0.86.0/meta/demos/demo_best_model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1252 2022-12-07 09:32:42.000000 nkululeko-0.86.0/meta/demos/my_experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2022-12-15 16:06:58.000000 nkululeko-0.86.0/meta/demos/my_experiment_local.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      681 2021-10-28 13:49:53.000000 nkululeko-0.86.0/meta/demos/plot_faster_anim.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.949784 nkululeko-0.86.0/nkululeko/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-08-31 11:56:33.000000 nkululeko-0.86.0/nkululeko/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3194 2024-02-29 11:07:44.000000 nkululeko-0.86.0/nkululeko/aug_train.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3051 2024-02-29 11:04:02.000000 nkululeko-0.86.0/nkululeko/augment.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.949784 nkululeko-0.86.0/nkululeko/augmenting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:16:55.000000 nkululeko-0.86.0/nkululeko/augmenting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2905 2023-12-29 16:48:37.000000 nkululeko-0.86.0/nkululeko/augmenting/augmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2669 2023-12-29 16:49:20.000000 nkululeko-0.86.0/nkululeko/augmenting/randomsplicer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1791 2023-09-07 11:33:33.000000 nkululeko-0.86.0/nkululeko/augmenting/randomsplicing.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3542 2024-05-13 11:40:51.000000 nkululeko-0.86.0/nkululeko/augmenting/resampler.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.949784 nkululeko-0.86.0/nkululeko/autopredict/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:02.000000 nkululeko-0.86.0/nkululeko/autopredict/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2023-12-19 11:16:15.000000 nkululeko-0.86.0/nkululeko/autopredict/ap_age.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.86.0/nkululeko/autopredict/ap_arousal.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1039 2023-12-19 11:16:15.000000 nkululeko-0.86.0/nkululeko/autopredict/ap_dominance.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1008 2023-12-19 11:16:15.000000 nkululeko-0.86.0/nkululeko/autopredict/ap_gender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1104 2023-12-19 11:16:16.000000 nkululeko-0.86.0/nkululeko/autopredict/ap_mos.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1137 2023-12-19 11:16:15.000000 nkululeko-0.86.0/nkululeko/autopredict/ap_pesq.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1185 2023-12-19 11:16:16.000000 nkululeko-0.86.0/nkululeko/autopredict/ap_sdr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1107 2023-12-19 11:16:15.000000 nkululeko-0.86.0/nkululeko/autopredict/ap_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1184 2023-12-19 11:16:15.000000 nkululeko-0.86.0/nkululeko/autopredict/ap_stoi.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.86.0/nkululeko/autopredict/ap_valence.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5048 2024-04-22 09:09:10.000000 nkululeko-0.86.0/nkululeko/autopredict/estimate_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      969 2023-09-07 11:39:39.000000 nkululeko-0.86.0/nkululeko/cacheddataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       39 2024-05-28 14:50:51.000000 nkululeko-0.86.0/nkululeko/constants.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.949784 nkululeko-0.86.0/nkululeko/data/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:06.000000 nkululeko-0.86.0/nkululeko/data/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    27650 2024-04-22 09:10:47.000000 nkululeko-0.86.0/nkululeko/data/dataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3933 2024-05-21 10:44:53.000000 nkululeko-0.86.0/nkululeko/data/dataset_csv.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3232 2024-05-03 09:55:35.000000 nkululeko-0.86.0/nkululeko/demo.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2025 2024-02-29 21:51:15.000000 nkululeko-0.86.0/nkululeko/demo_feats.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4757 2024-05-03 09:56:14.000000 nkululeko-0.86.0/nkululeko/demo_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    30962 2024-05-29 08:14:47.000000 nkululeko-0.86.0/nkululeko/experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2609 2024-04-30 15:24:17.000000 nkululeko-0.86.0/nkululeko/explore.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4632 2023-12-19 11:16:14.000000 nkululeko-0.86.0/nkululeko/export.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.953784 nkululeko-0.86.0/nkululeko/feat_extract/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:10.000000 nkululeko-0.86.0/nkululeko/feat_extract/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3113 2024-04-23 09:16:18.000000 nkululeko-0.86.0/nkululeko/feat_extract/feats_agender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3424 2024-04-29 13:37:24.000000 nkululeko-0.86.0/nkululeko/feat_extract/feats_agender_agender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12722 2024-05-03 14:41:56.000000 nkululeko-0.86.0/nkululeko/feat_extract/feats_analyser.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3162 2024-04-23 09:16:18.000000 nkululeko-0.86.0/nkululeko/feat_extract/feats_auddim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3187 2024-04-23 09:16:18.000000 nkululeko-0.86.0/nkululeko/feat_extract/feats_audmodel.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3489 2024-04-23 09:16:18.000000 nkululeko-0.86.0/nkululeko/feat_extract/feats_clap.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5196 2024-04-24 17:12:28.000000 nkululeko-0.86.0/nkululeko/feat_extract/feats_hubert.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1622 2024-04-23 09:55:16.000000 nkululeko-0.86.0/nkululeko/feat_extract/feats_import.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2021 2023-12-19 11:16:16.000000 nkululeko-0.86.0/nkululeko/feat_extract/feats_mld.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4174 2024-04-23 10:17:00.000000 nkululeko-0.86.0/nkululeko/feat_extract/feats_mos.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4028 2024-05-29 07:55:31.000000 nkululeko-0.86.0/nkululeko/feat_extract/feats_opensmile.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4980 2024-04-23 09:16:18.000000 nkululeko-0.86.0/nkululeko/feat_extract/feats_oxbow.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3105 2024-04-23 09:16:18.000000 nkululeko-0.86.0/nkululeko/feat_extract/feats_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.86.0/nkululeko/feat_extract/feats_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3670 2024-04-23 09:59:48.000000 nkululeko-0.86.0/nkululeko/feat_extract/feats_spectra.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4803 2023-10-06 16:05:03.000000 nkululeko-0.86.0/nkululeko/feat_extract/feats_spkrec.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4617 2024-04-29 13:37:24.000000 nkululeko-0.86.0/nkululeko/feat_extract/feats_squim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3228 2024-04-30 09:31:46.000000 nkululeko-0.86.0/nkululeko/feat_extract/feats_trill.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5268 2024-04-29 13:37:24.000000 nkululeko-0.86.0/nkululeko/feat_extract/feats_wav2vec2.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4703 2024-04-24 17:06:22.000000 nkululeko-0.86.0/nkululeko/feat_extract/feats_wavlm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4533 2024-05-15 15:09:05.000000 nkululeko-0.86.0/nkululeko/feat_extract/feats_whisper.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1541 2024-05-29 07:58:33.000000 nkululeko-0.86.0/nkululeko/feat_extract/featureset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21304 2024-04-15 13:57:11.000000 nkululeko-0.86.0/nkululeko/feat_extract/feinberg_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3976 2024-04-23 11:13:33.000000 nkululeko-0.86.0/nkululeko/feature_extractor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3474 2023-12-19 11:16:14.000000 nkululeko-0.86.0/nkululeko/file_checker.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7222 2023-12-19 11:16:14.000000 nkululeko-0.86.0/nkululeko/filter_data.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      525 2024-05-03 12:01:14.000000 nkululeko-0.86.0/nkululeko/glob_conf.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.953784 nkululeko-0.86.0/nkululeko/losses/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:16.000000 nkululeko-0.86.0/nkululeko/losses/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      976 2023-09-07 11:37:43.000000 nkululeko-0.86.0/nkululeko/losses/loss_ccc.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1309 2023-09-26 13:42:48.000000 nkululeko-0.86.0/nkululeko/losses/loss_softf1loss.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10452 2024-05-17 12:04:16.000000 nkululeko-0.86.0/nkululeko/modelrunner.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.953784 nkululeko-0.86.0/nkululeko/models/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:20.000000 nkululeko-0.86.0/nkululeko/models/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11639 2024-05-15 15:09:05.000000 nkululeko-0.86.0/nkululeko/models/model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2024-05-03 14:26:57.000000 nkululeko-0.86.0/nkululeko/models/model_bayes.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9954 2024-05-03 14:27:45.000000 nkululeko-0.86.0/nkululeko/models/model_cnn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      649 2024-05-03 14:28:01.000000 nkululeko-0.86.0/nkululeko/models/model_gmm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      599 2024-05-03 14:28:22.000000 nkululeko-0.86.0/nkululeko/models/model_knn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      610 2024-05-03 14:28:14.000000 nkululeko-0.86.0/nkululeko/models/model_knn_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      422 2024-05-03 14:28:34.000000 nkululeko-0.86.0/nkululeko/models/model_lin_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9854 2024-05-03 14:29:13.000000 nkululeko-0.86.0/nkululeko/models/model_mlp.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10204 2024-05-03 14:28:58.000000 nkululeko-0.86.0/nkululeko/models/model_mlp_regression.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      940 2024-05-03 14:29:24.000000 nkululeko-0.86.0/nkululeko/models/model_svm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      725 2024-05-03 14:29:39.000000 nkululeko-0.86.0/nkululeko/models/model_svr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      417 2024-05-03 14:30:08.000000 nkululeko-0.86.0/nkululeko/models/model_tree.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      428 2024-05-03 14:29:56.000000 nkululeko-0.86.0/nkululeko/models/model_tree_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18049 2024-05-28 14:48:26.000000 nkululeko-0.86.0/nkululeko/models/model_tuned.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      447 2024-05-03 14:33:39.000000 nkululeko-0.86.0/nkululeko/models/model_xgb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      418 2024-05-03 14:34:29.000000 nkululeko-0.86.0/nkululeko/models/model_xgr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5634 2024-04-23 14:42:13.000000 nkululeko-0.86.0/nkululeko/multidb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3725 2024-04-26 06:05:26.000000 nkululeko-0.86.0/nkululeko/nkuluflag.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1968 2024-04-23 12:35:01.000000 nkululeko-0.86.0/nkululeko/nkululeko.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    23276 2024-04-29 13:37:24.000000 nkululeko-0.86.0/nkululeko/plots.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2409 2024-04-22 09:09:10.000000 nkululeko-0.86.0/nkululeko/predict.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.953784 nkululeko-0.86.0/nkululeko/reporting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-10-13 10:14:37.000000 nkululeko-0.86.0/nkululeko/reporting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      648 2023-10-02 13:54:57.000000 nkululeko-0.86.0/nkululeko/reporting/defines.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1886 2023-12-19 13:13:44.000000 nkululeko-0.86.0/nkululeko/reporting/latex_writer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1060 2023-12-19 11:16:16.000000 nkululeko-0.86.0/nkululeko/reporting/report.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      533 2023-09-26 14:51:22.000000 nkululeko-0.86.0/nkululeko/reporting/report_item.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12841 2024-04-25 13:02:38.000000 nkululeko-0.86.0/nkululeko/reporting/reporter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      742 2024-04-16 12:21:39.000000 nkululeko-0.86.0/nkululeko/reporting/result.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3354 2024-05-13 11:40:51.000000 nkululeko-0.86.0/nkululeko/resample.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7624 2024-04-22 09:09:10.000000 nkululeko-0.86.0/nkululeko/runmanager.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4101 2024-01-31 12:20:11.000000 nkululeko-0.86.0/nkululeko/scaler.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4835 2024-02-29 11:06:43.000000 nkululeko-0.86.0/nkululeko/segment.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.953784 nkululeko-0.86.0/nkululeko/segmenting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:24.000000 nkululeko-0.86.0/nkululeko/segmenting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1947 2023-09-07 11:39:09.000000 nkululeko-0.86.0/nkululeko/segmenting/seg_inaspeechsegmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3301 2023-12-19 11:16:15.000000 nkululeko-0.86.0/nkululeko/segmenting/seg_silero.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10047 2023-09-26 13:42:49.000000 nkululeko-0.86.0/nkululeko/syllable_nuclei.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1677 2024-04-26 06:04:30.000000 nkululeko-0.86.0/nkululeko/test.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3237 2024-04-25 14:01:11.000000 nkululeko-0.86.0/nkululeko/test_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8465 2024-05-15 15:09:05.000000 nkululeko-0.86.0/nkululeko/test_pretrain.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.953784 nkululeko-0.86.0/nkululeko/utils/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:28.000000 nkululeko-0.86.0/nkululeko/utils/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4021 2023-09-20 08:48:00.000000 nkululeko-0.86.0/nkululeko/utils/files.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.86.0/nkululeko/utils/stats.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    13816 2024-05-13 11:40:51.000000 nkululeko-0.86.0/nkululeko/utils/util.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.953784 nkululeko-0.86.0/nkululeko.egg-info/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    36852 2024-05-29 08:17:01.000000 nkululeko-0.86.0/nkululeko.egg-info/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5132 2024-05-29 08:17:01.000000 nkululeko-0.86.0/nkululeko.egg-info/SOURCES.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2024-05-29 08:17:01.000000 nkululeko-0.86.0/nkululeko.egg-info/dependency_links.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      298 2024-05-29 08:17:01.000000 nkululeko-0.86.0/nkululeko.egg-info/requires.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2024-05-29 08:17:01.000000 nkululeko-0.86.0/nkululeko.egg-info/top_level.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.86.0/pyproject.toml
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1001 2024-05-29 08:17:01.957785 nkululeko-0.86.0/setup.cfg
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.86.0/setup.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.945784 nkululeko-0.86.0/venv/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 08:17:01.953784 nkululeko-0.86.0/venv/bin/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1200 2023-12-29 19:06:16.000000 nkululeko-0.86.0/venv/bin/activate_this.py
```

### Comparing `nkululeko-0.85.2/CHANGELOG.md` & `nkululeko-0.86.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+Version 0.86.0
+--------------
+* added regression to finetuning
+* added other transformer models to finetuning
+* added output the train/dev features sets actually used by the model
+
 Version 0.85.2
 --------------
 * added data, and automatic task label detection
 
 Version 0.85.1
 --------------
 * fixed bug in model_finetuned that label_num was constant 2
```

### Comparing `nkululeko-0.85.2/LICENSE` & `nkululeko-0.86.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/PKG-INFO` & `nkululeko-0.86.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.85.2
+Version: 0.86.0
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -329,14 +329,20 @@
    year = {2022},
 }
 ```
 
 Changelog
 =========
 
+Version 0.86.0
+--------------
+* added regression to finetuning
+* added other transformer models to finetuning
+* added output the train/dev features sets actually used by the model
+
 Version 0.85.2
 --------------
 * added data, and automatic task label detection
 
 Version 0.85.1
 --------------
 * fixed bug in model_finetuned that label_num was constant 2
```

### Comparing `nkululeko-0.85.2/README.md` & `nkululeko-0.86.0/README.md`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/aesdd/process_database.py` & `nkululeko-0.86.0/data/aesdd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/androids/process_database.py` & `nkululeko-0.86.0/data/androids/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/androids_orig/process_database.py` & `nkululeko-0.86.0/data/androids_orig/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/androids_test/process_database.py` & `nkululeko-0.86.0/data/androids_test/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/ased/process_database.py` & `nkululeko-0.86.0/data/ased/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/asvp-esd/process_database.py` & `nkululeko-0.86.0/data/asvp-esd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/baved/process_database.py` & `nkululeko-0.86.0/data/baved/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/cafe/process_database.py` & `nkululeko-0.86.0/data/cafe/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/clac/process_database.py` & `nkululeko-0.86.0/data/clac/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/cmu-mosei/process_database.py` & `nkululeko-0.86.0/data/cmu-mosei/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/demos/process_database.py` & `nkululeko-0.86.0/data/demos/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/ekorpus/process_database.py` & `nkululeko-0.86.0/data/ekorpus/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/emns/process_database.py` & `nkululeko-0.86.0/data/emns/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/emofilm/convert_to_16k.py` & `nkululeko-0.86.0/data/emofilm/convert_to_16k.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/emofilm/process_database.py` & `nkululeko-0.86.0/data/emofilm/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/emorynlp/process_database.py` & `nkululeko-0.86.0/data/emorynlp/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/emov-db/process_database.py` & `nkululeko-0.86.0/data/emov-db/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/emovo/process_database.py` & `nkululeko-0.86.0/data/emovo/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/emozionalmente/create.py` & `nkululeko-0.86.0/data/emozionalmente/create.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/enterface/process_database.py` & `nkululeko-0.86.0/data/enterface/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/esd/process_database.py` & `nkululeko-0.86.0/data/esd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/gerparas/process_database.py` & `nkululeko-0.86.0/data/gerparas/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/iemocap/process_database.py` & `nkululeko-0.86.0/data/iemocap/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/jl/process_database.py` & `nkululeko-0.86.0/data/jl/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/jtes/process_database.py` & `nkululeko-0.86.0/data/jtes/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/meld/process_database.py` & `nkululeko-0.86.0/data/meld/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/mesd/process_database.py` & `nkululeko-0.86.0/data/mesd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/mess/process_database.py` & `nkululeko-0.86.0/data/mess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/mlendsnd/process_database.py` & `nkululeko-0.86.0/data/mlendsnd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/msp-improv/process_database2.py` & `nkululeko-0.86.0/data/msp-improv/process_database2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/msp-podcast/process_database.py` & `nkululeko-0.86.0/data/msp-podcast/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/oreau2/process_database.py` & `nkululeko-0.86.0/data/oreau2/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/portuguese/process_database.py` & `nkululeko-0.86.0/data/portuguese/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/ravdess/process_database.py` & `nkululeko-0.86.0/data/ravdess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/ravdess/process_database_speaker.py` & `nkululeko-0.86.0/data/ravdess/process_database_speaker.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/savee/process_database.py` & `nkululeko-0.86.0/data/savee/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/shemo/process_database.py` & `nkululeko-0.86.0/data/shemo/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/subesco/process_database.py` & `nkululeko-0.86.0/data/subesco/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/tess/process_database.py` & `nkululeko-0.86.0/data/tess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/thorsten-emotional/process_database.py` & `nkululeko-0.86.0/data/thorsten-emotional/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/urdu/process_database.py` & `nkululeko-0.86.0/data/urdu/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/data/vivae/process_database.py` & `nkululeko-0.86.0/data/vivae/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/docs/source/conf.py` & `nkululeko-0.86.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/meta/demos/demo_best_model.py` & `nkululeko-0.86.0/meta/demos/demo_best_model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/meta/demos/my_experiment.py` & `nkululeko-0.86.0/meta/demos/my_experiment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/meta/demos/my_experiment_local.py` & `nkululeko-0.86.0/meta/demos/my_experiment_local.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/meta/demos/plot_faster_anim.py` & `nkululeko-0.86.0/meta/demos/plot_faster_anim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/aug_train.py` & `nkululeko-0.86.0/nkululeko/aug_train.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/augment.py` & `nkululeko-0.86.0/nkululeko/augment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/augmenting/augmenter.py` & `nkululeko-0.86.0/nkululeko/augmenting/augmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/augmenting/randomsplicer.py` & `nkululeko-0.86.0/nkululeko/augmenting/randomsplicer.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/augmenting/randomsplicing.py` & `nkululeko-0.86.0/nkululeko/augmenting/randomsplicing.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/augmenting/resampler.py` & `nkululeko-0.86.0/nkululeko/augmenting/resampler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/autopredict/ap_age.py` & `nkululeko-0.86.0/nkululeko/autopredict/ap_age.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/autopredict/ap_arousal.py` & `nkululeko-0.86.0/nkululeko/autopredict/ap_arousal.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/autopredict/ap_dominance.py` & `nkululeko-0.86.0/nkululeko/autopredict/ap_dominance.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/autopredict/ap_gender.py` & `nkululeko-0.86.0/nkululeko/autopredict/ap_gender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/autopredict/ap_mos.py` & `nkululeko-0.86.0/nkululeko/autopredict/ap_mos.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/autopredict/ap_pesq.py` & `nkululeko-0.86.0/nkululeko/autopredict/ap_pesq.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/autopredict/ap_sdr.py` & `nkululeko-0.86.0/nkululeko/autopredict/ap_sdr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/autopredict/ap_snr.py` & `nkululeko-0.86.0/nkululeko/autopredict/ap_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/autopredict/ap_stoi.py` & `nkululeko-0.86.0/nkululeko/autopredict/ap_stoi.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/autopredict/ap_valence.py` & `nkululeko-0.86.0/nkululeko/autopredict/ap_valence.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/autopredict/estimate_snr.py` & `nkululeko-0.86.0/nkululeko/autopredict/estimate_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/cacheddataset.py` & `nkululeko-0.86.0/nkululeko/cacheddataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/data/dataset.py` & `nkululeko-0.86.0/nkululeko/data/dataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/data/dataset_csv.py` & `nkululeko-0.86.0/nkululeko/data/dataset_csv.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/demo.py` & `nkululeko-0.86.0/nkululeko/demo.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/demo_feats.py` & `nkululeko-0.86.0/nkululeko/demo_feats.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/demo_predictor.py` & `nkululeko-0.86.0/nkululeko/demo_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/experiment.py` & `nkululeko-0.86.0/nkululeko/experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,23 +26,22 @@
 from nkululeko.runmanager import Runmanager
 from nkululeko.scaler import Scaler
 from nkululeko.test_predictor import TestPredictor
 from nkululeko.utils.util import Util
 
 
 class Experiment:
-    """Main class specifying an experiment"""
+    """Main class specifying an experiment."""
 
     def __init__(self, config_obj):
-        """
-        Parameters
-        ----------
-        config_obj : a config parser object that sets the experiment parameters and being set as a global object.
-        """
+        """Constructor.
 
+        Args:
+            - config_obj : a config parser object that sets the experiment parameters and being set as a global object.
+        """
         self.set_globals(config_obj)
         self.name = glob_conf.config["EXP"]["name"]
         self.root = os.path.join(glob_conf.config["EXP"]["root"], "")
         self.data_dir = os.path.join(self.root, self.name)
         audeer.mkdir(self.data_dir)  # create the experiment directory
         self.util = Util("experiment")
         glob_conf.set_util(self.util)
@@ -105,23 +104,21 @@
         self.target = self.util.config_val("DATA", "target", "emotion")
         glob_conf.set_target(self.target)
         # print target via debug
         self.util.debug(f"target: {self.target}")
         # print keys/column
         dbs = ",".join(list(self.datasets.keys()))
         labels = self.util.config_val("DATA", "labels", False)
-        auto_labels = list(
-            next(iter(self.datasets.values())).df[self.target].unique()
-        )
+        auto_labels = list(next(iter(self.datasets.values())).df[self.target].unique())
         if labels:
             self.labels = ast.literal_eval(labels)
             self.util.debug(f"Target labels (from config): {labels}")
         else:
             self.labels = auto_labels
-        self.util.debug(f"Target labels (from database): {auto_labels}")
+            self.util.debug(f"Target labels (from database): {auto_labels}")
         glob_conf.set_labels(self.labels)
         self.util.debug(f"loaded databases {dbs}")
 
     def _import_csv(self, storage):
         # df = pd.read_csv(storage, header=0, index_col=[0,1,2])
         # df.index.set_levels(pd.to_timedelta(df.index.levels[1]), level=1)
         # df.index.set_levels(pd.to_timedelta(df.index.levels[2]), level=2)
@@ -156,16 +153,15 @@
                 if data.got_age:
                     self.got_age = True
                 if data.got_speaker:
                     self.got_speaker = True
                 data.split()
                 data.prepare_labels()
                 self.df_test = pd.concat(
-                    [self.df_test, self.util.make_segmented_index(
-                        data.df_test)]
+                    [self.df_test, self.util.make_segmented_index(data.df_test)]
                 )
                 self.df_test.is_labeled = data.is_labeled
             self.df_test.got_gender = self.got_gender
             self.df_test.got_speaker = self.got_speaker
             # self.util.set_config_val('FEATS', 'needs_features_extraction', 'True')
             # self.util.set_config_val('FEATS', 'no_reuse', 'True')
             self.df_test["class_label"] = self.df_test[self.target]
@@ -258,25 +254,23 @@
                 train_cats = self.df_train["class_label"].unique()
 
             else:
                 if self.df_test.is_labeled:
                     test_cats = self.df_test[self.target].unique()
                 else:
                     # if there is no target, copy a dummy label
-                    self.df_test = self._add_random_target(
-                        self.df_test).astype("str")
+                    self.df_test = self._add_random_target(self.df_test).astype("str")
                 train_cats = self.df_train[self.target].unique()
                 # print(f"df_train: {pd.DataFrame(self.df_train[self.target])}")
                 # print(f"train_cats with target {self.target}: {train_cats}")
             if self.df_test.is_labeled:
                 if type(test_cats) == np.ndarray:
                     self.util.debug(f"Categories test (nd.array): {test_cats}")
                 else:
-                    self.util.debug(
-                        f"Categories test (list): {list(test_cats)}")
+                    self.util.debug(f"Categories test (list): {list(test_cats)}")
             if type(train_cats) == np.ndarray:
                 self.util.debug(f"Categories train (nd.array): {train_cats}")
             else:
                 self.util.debug(f"Categories train (list): {list(train_cats)}")
 
             # encode the labels as numbers
             self.label_encoder = LabelEncoder()
@@ -291,16 +285,15 @@
             self.util.debug(
                 f"{self.df_test.speaker.nunique()} speakers in test and"
                 f" {self.df_train.speaker.nunique()} speakers in train"
             )
 
         target_factor = self.util.config_val("DATA", "target_divide_by", False)
         if target_factor:
-            self.df_test[self.target] = self.df_test[self.target] / \
-                float(target_factor)
+            self.df_test[self.target] = self.df_test[self.target] / float(target_factor)
             self.df_train[self.target] = self.df_train[self.target] / float(
                 target_factor
             )
             if not self.util.exp_is_classification():
                 self.df_test["class_label"] = self.df_test["class_label"] / float(
                     target_factor
                 )
@@ -315,24 +308,22 @@
             a[i] = random.choice(labels)
         df[self.target] = a
         return df
 
     def plot_distribution(self, df_labels):
         """Plot the distribution of samples and speaker per target class and biological sex"""
         plot = Plots()
-        sample_selection = self.util.config_val(
-            "EXPL", "sample_selection", "all")
+        sample_selection = self.util.config_val("EXPL", "sample_selection", "all")
         plot.plot_distributions(df_labels)
         if self.got_speaker:
             plot.plot_distributions_speaker(df_labels)
 
     def extract_test_feats(self):
         self.feats_test = pd.DataFrame()
-        feats_name = "_".join(ast.literal_eval(
-            glob_conf.config["DATA"]["tests"]))
+        feats_name = "_".join(ast.literal_eval(glob_conf.config["DATA"]["tests"]))
         feats_types = self.util.config_val_list("FEATS", "type", ["os"])
         self.feature_extractor = FeatureExtractor(
             self.df_test, feats_types, feats_name, "test"
         )
         self.feats_test = self.feature_extractor.extract()
         self.util.debug(f"Test features shape:{self.feats_test.shape}")
 
@@ -341,16 +332,15 @@
 
         They will be stored on disk and need to be removed manually.
 
         The string FEATS.feats_type is read from the config, defaults to os.
 
         """
         df_train, df_test = self.df_train, self.df_test
-        feats_name = "_".join(ast.literal_eval(
-            glob_conf.config["DATA"]["databases"]))
+        feats_name = "_".join(ast.literal_eval(glob_conf.config["DATA"]["databases"]))
         self.feats_test, self.feats_train = pd.DataFrame(), pd.DataFrame()
         feats_types = self.util.config_val_list("FEATS", "type", [])
         # for some models no features are needed
         if len(feats_types) == 0:
             self.util.debug("no feature extractor specified.")
             self.feats_train, self.feats_test = pd.DataFrame(), pd.DataFrame()
             return
@@ -376,28 +366,30 @@
             ]
             self.util.warn(f"new train labels shape: {self.df_train.shape[0]}")
         if self.feats_test.shape[0] < self.df_test.shape[0]:
             self.util.warn(
                 f"test feats ({self.feats_test.shape[0]}) != test labels"
                 f" ({self.df_test.shape[0]})"
             )
-            self.df_test = self.df_test[self.df_test.index.isin(
-                self.feats_test.index)]
-            self.util.warn(f"mew test labels shape: {self.df_test.shape[0]}")
+            self.df_test = self.df_test[self.df_test.index.isin(self.feats_test.index)]
+            self.util.warn(f"new test labels shape: {self.df_test.shape[0]}")
 
         self._check_scale()
+        # store = self.util.get_path("store")
+        # store_format = self.util.config_val("FEATS", "store_format", "pkl")
+        # storage = f"{store}test_feats.{store_format}"
+        # self.util.write_store(self.feats_test, storage, store_format)
+        # storage = f"{store}train_feats.{store_format}"
+        # self.util.write_store(self.feats_train, storage, store_format)
 
     def augment(self):
-        """
-        Augment the selected samples
-        """
+        """Augment the selected samples."""
         from nkululeko.augmenting.augmenter import Augmenter
 
-        sample_selection = self.util.config_val(
-            "AUGMENT", "sample_selection", "all")
+        sample_selection = self.util.config_val("AUGMENT", "sample_selection", "all")
         if sample_selection == "all":
             df = pd.concat([self.df_train, self.df_test])
         elif sample_selection == "train":
             df = self.df_train
         elif sample_selection == "test":
             df = self.df_test
         else:
@@ -484,16 +476,15 @@
 
     def random_splice(self):
         """
         Random-splice the selected samples
         """
         from nkululeko.augmenting.randomsplicer import Randomsplicer
 
-        sample_selection = self.util.config_val(
-            "AUGMENT", "sample_selection", "all")
+        sample_selection = self.util.config_val("AUGMENT", "sample_selection", "all")
         if sample_selection == "all":
             df = pd.concat([self.df_train, self.df_test])
         elif sample_selection == "train":
             df = self.df_train
         elif sample_selection == "test":
             df = self.df_test
         else:
@@ -506,16 +497,15 @@
         return df_ret
 
     def analyse_features(self, needs_feats):
         """Do a feature exploration."""
         plot_feats = eval(
             self.util.config_val("EXPL", "feature_distributions", "False")
         )
-        sample_selection = self.util.config_val(
-            "EXPL", "sample_selection", "all")
+        sample_selection = self.util.config_val("EXPL", "sample_selection", "all")
         # get the data labels
         if sample_selection == "all":
             df_labels = pd.concat([self.df_train, self.df_test])
             self.util.copy_flags(self.df_train, df_labels)
         elif sample_selection == "train":
             df_labels = self.df_train
             self.util.copy_flags(self.df_train, df_labels)
@@ -570,30 +560,31 @@
         if scatter_var:
             scatters = ast.literal_eval(glob_conf.config["EXPL"]["scatter"])
             scat_targets = ast.literal_eval(scatter_target)
             plots = Plots()
             for scat_target in scat_targets:
                 if self.util.is_categorical(df_labels[scat_target]):
                     for scatter in scatters:
-                        plots.scatter_plot(
-                            df_feats, df_labels, scat_target, scatter)
+                        plots.scatter_plot(df_feats, df_labels, scat_target, scatter)
                 else:
                     self.util.debug(
                         f"{self.name}: binning continuous variable to categories"
                     )
                     cat_vals = self.util.continuous_to_categorical(
                         df_labels[scat_target]
                     )
                     df_labels[f"{scat_target}_bins"] = cat_vals.values
                     for scatter in scatters:
                         plots.scatter_plot(
                             df_feats, df_labels, f"{scat_target}_bins", scatter
                         )
 
     def _check_scale(self):
+        self.util.save_to_store(self.feats_train, "feats_train")
+        self.util.save_to_store(self.feats_test, "feats_test")
         scale_feats = self.util.config_val("FEATS", "scale", False)
         # print the scale
         self.util.debug(f"scaler: {scale_feats}")
         if scale_feats:
             self.scaler_feats = Scaler(
                 self.df_train,
                 self.df_test,
@@ -660,16 +651,15 @@
         best = self.get_best_report(self.reports)
         # if not best.is_classification:
         #     best.continuous_to_categorical()
         truths = best.truths
         preds = best.preds
         speakers = self.df_test.speaker.values
         print(f"{len(truths)} {len(preds)} {len(speakers) }")
-        df = pd.DataFrame(
-            data={"truth": truths, "pred": preds, "speaker": speakers})
+        df = pd.DataFrame(data={"truth": truths, "pred": preds, "speaker": speakers})
         plot_name = "result_combined_per_speaker"
         self.util.debug(
             f"plotting speaker combination ({function}) confusion matrix to"
             f" {plot_name}"
         )
         best.plot_per_speaker(df, plot_name, function)
```

### Comparing `nkululeko-0.85.2/nkululeko/explore.py` & `nkululeko-0.86.0/nkululeko/explore.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/export.py` & `nkululeko-0.86.0/nkululeko/export.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/feat_extract/feats_agender.py` & `nkululeko-0.86.0/nkululeko/feat_extract/feats_agender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/feat_extract/feats_agender_agender.py` & `nkululeko-0.86.0/nkululeko/feat_extract/feats_agender_agender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/feat_extract/feats_analyser.py` & `nkululeko-0.86.0/nkululeko/feat_extract/feats_analyser.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/feat_extract/feats_auddim.py` & `nkululeko-0.86.0/nkululeko/feat_extract/feats_auddim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/feat_extract/feats_audmodel.py` & `nkululeko-0.86.0/nkululeko/feat_extract/feats_audmodel.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/feat_extract/feats_clap.py` & `nkululeko-0.86.0/nkululeko/feat_extract/feats_clap.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/feat_extract/feats_hubert.py` & `nkululeko-0.86.0/nkululeko/feat_extract/feats_hubert.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/feat_extract/feats_import.py` & `nkululeko-0.86.0/nkululeko/feat_extract/feats_import.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/feat_extract/feats_mld.py` & `nkululeko-0.86.0/nkululeko/feat_extract/feats_mld.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/feat_extract/feats_mos.py` & `nkululeko-0.86.0/nkululeko/feat_extract/feats_mos.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/feat_extract/feats_opensmile.py` & `nkululeko-0.86.0/nkululeko/feat_extract/feats_opensmile.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,32 +61,32 @@
         smile = opensmile.Smile(
             feature_set=self.feature_set,
             feature_level=opensmile.FeatureLevel.Functionals,
         )
         feats = smile.process_signal(signal, sr)
         return feats.to_numpy()
 
-    def filter(self):
-        # use only the features that are indexed in the target dataframes
-        self.df = self.df[self.df.index.isin(self.data_df.index)]
-        try:
-            # use only some features
-            selected_features = ast.literal_eval(
-                glob_conf.config["FEATS"]["os.features"]
-            )
-            self.util.debug(f"selecting features from opensmile: {selected_features}")
-            sel_feats_df = pd.DataFrame()
-            hit = False
-            for feat in selected_features:
-                try:
-                    sel_feats_df[feat] = self.df[feat]
-                    hit = True
-                except KeyError:
-                    pass
-            if hit:
-                self.df = sel_feats_df
-                self.util.debug(
-                    "new feats shape after selecting opensmile features:"
-                    f" {self.df.shape}"
-                )
-        except KeyError:
-            pass
+    # def filter(self):
+    #     # use only the features that are indexed in the target dataframes
+    #     self.df = self.df[self.df.index.isin(self.data_df.index)]
+    #     try:
+    #         # use only some features
+    #         selected_features = ast.literal_eval(
+    #             glob_conf.config["FEATS"]["os.features"]
+    #         )
+    #         self.util.debug(f"selecting features from opensmile: {selected_features}")
+    #         sel_feats_df = pd.DataFrame()
+    #         hit = False
+    #         for feat in selected_features:
+    #             try:
+    #                 sel_feats_df[feat] = self.df[feat]
+    #                 hit = True
+    #             except KeyError:
+    #                 pass
+    #         if hit:
+    #             self.df = sel_feats_df
+    #             self.util.debug(
+    #                 "new feats shape after selecting opensmile features:"
+    #                 f" {self.df.shape}"
+    #             )
+    #     except KeyError:
+    #         pass
```

### Comparing `nkululeko-0.85.2/nkululeko/feat_extract/feats_oxbow.py` & `nkululeko-0.86.0/nkululeko/feat_extract/feats_oxbow.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/feat_extract/feats_praat.py` & `nkululeko-0.86.0/nkululeko/feat_extract/feats_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/feat_extract/feats_snr.py` & `nkululeko-0.86.0/nkululeko/feat_extract/feats_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/feat_extract/feats_spectra.py` & `nkululeko-0.86.0/nkululeko/feat_extract/feats_spectra.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/feat_extract/feats_spkrec.py` & `nkululeko-0.86.0/nkululeko/feat_extract/feats_spkrec.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/feat_extract/feats_squim.py` & `nkululeko-0.86.0/nkululeko/feat_extract/feats_squim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/feat_extract/feats_trill.py` & `nkululeko-0.86.0/nkululeko/feat_extract/feats_trill.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/feat_extract/feats_wav2vec2.py` & `nkululeko-0.86.0/nkululeko/feat_extract/feats_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/feat_extract/feats_wavlm.py` & `nkululeko-0.86.0/nkululeko/feat_extract/feats_wavlm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/feat_extract/feats_whisper.py` & `nkululeko-0.86.0/nkululeko/feat_extract/feats_whisper.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/feat_extract/featureset.py` & `nkululeko-0.86.0/nkululeko/feat_extract/featureset.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,35 +11,35 @@
     # (and indexed with the data from the sets)
     data_df = None  # dataframe to get audio paths
 
     def __init__(self, name, data_df, feats_type):
         self.name = name
         self.data_df = data_df
         self.util = Util("featureset")
-        self.feats_types = feats_type
+        self.feats_type = feats_type
 
     def extract(self):
         pass
 
     def filter(self):
         # use only the features that are indexed in the target dataframes
         self.df = self.df[self.df.index.isin(self.data_df.index)]
         try:
             # use only some features
-            selected_features = ast.literal_eval(
-                glob_conf.config["FEATS"]["features"])
+            selected_features = ast.literal_eval(glob_conf.config["FEATS"]["features"])
             self.util.debug(f"selecting features: {selected_features}")
             sel_feats_df = pd.DataFrame()
             hit = False
             for feat in selected_features:
                 try:
                     sel_feats_df[feat] = self.df[feat]
                     hit = True
                 except KeyError:
+                    self.util.warn(f"non existent feature in {self.feats_type}: {feat}")
                     pass
             if hit:
                 self.df = sel_feats_df
                 self.util.debug(
-                    f"new feats shape after selecting features: {self.df.shape}"
+                    f"new feats shape after selecting features for {self.feats_type}: {self.df.shape}"
                 )
         except KeyError:
             pass
```

### Comparing `nkululeko-0.85.2/nkululeko/feat_extract/feinberg_praat.py` & `nkululeko-0.86.0/nkululeko/feat_extract/feinberg_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/feature_extractor.py` & `nkululeko-0.86.0/nkululeko/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/file_checker.py` & `nkululeko-0.86.0/nkululeko/file_checker.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/filter_data.py` & `nkululeko-0.86.0/nkululeko/filter_data.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/glob_conf.py` & `nkululeko-0.86.0/nkululeko/glob_conf.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/losses/loss_ccc.py` & `nkululeko-0.86.0/nkululeko/losses/loss_ccc.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/losses/loss_softf1loss.py` & `nkululeko-0.86.0/nkululeko/losses/loss_softf1loss.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/modelrunner.py` & `nkululeko-0.86.0/nkululeko/modelrunner.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/models/model.py` & `nkululeko-0.86.0/nkululeko/models/model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/models/model_cnn.py` & `nkululeko-0.86.0/nkululeko/models/model_cnn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/models/model_gmm.py` & `nkululeko-0.86.0/nkululeko/models/model_gmm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/models/model_knn.py` & `nkululeko-0.86.0/nkululeko/models/model_knn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/models/model_knn_reg.py` & `nkululeko-0.86.0/nkululeko/models/model_knn_reg.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/models/model_mlp.py` & `nkululeko-0.86.0/nkululeko/models/model_mlp.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/models/model_mlp_regression.py` & `nkululeko-0.86.0/nkululeko/models/model_mlp_regression.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/models/model_svm.py` & `nkululeko-0.86.0/nkululeko/models/model_svm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/models/model_svr.py` & `nkululeko-0.86.0/nkululeko/models/model_svr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/models/model_tuned.py` & `nkululeko-0.86.0/nkululeko/models/model_tuned.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Code based on @jwagner.
-"""
+"""Code based on @jwagner."""
 
 import dataclasses
 import json
 import os
 import pickle
 import typing
 
@@ -23,43 +21,63 @@
 import nkululeko.glob_conf as glob_conf
 from nkululeko.models.model import Model as BaseModel
 from nkululeko.reporting.reporter import Reporter
 
 
 class TunedModel(BaseModel):
 
-    is_classifier = True
-
     def __init__(self, df_train, df_test, feats_train, feats_test):
         """Constructor taking the configuration and all dataframes."""
         super().__init__(df_train, df_test, feats_train, feats_test)
         super().set_model_type("finetuned")
         self.name = "finetuned_wav2vec2"
         self.target = glob_conf.config["DATA"]["target"]
         labels = glob_conf.labels
         self.class_num = len(labels)
-        device = self.util.config_val("MODEL", "device", "cpu")
-        self.batch_size = int(self.util.config_val("MODEL", "batch_size", "8"))
-        if device != "cpu":
-            self.util.debug(f"running on device {device}")
+        device = self.util.config_val("MODEL", "device", False)
+        if not device:
+            self.device = "cuda" if torch.cuda.is_available() else "cpu"
+        else:
+            self.device = device
+        if self.device != "cpu":
             os.environ["CUDA_DEVICE_ORDER"] = "PCI_BUS_ID"
-            os.environ["CUDA_VISIBLE_DEVICES"] = device
+            os.environ["CUDA_VISIBLE_DEVICES"] = self.device
+        self.util.debug(f"running on device {self.device}")
+        self.is_classifier = self.util.exp_is_classification()
+        if self.is_classifier:
+            self.measure = "uar"
+        else:
+            self.measure = self.util.config_val("MODEL", "measure", "ccc")
+        self.util.debug(f"evaluation metrics: {self.measure}")
+        self.batch_size = int(self.util.config_val("MODEL", "batch_size", "8"))
+        self.util.debug(f"batch size: {self.batch_size}")
+        self.learning_rate = float(
+            self.util.config_val("MODEL", "learning_rate", 0.0001)
+        )
         self.df_train, self.df_test = df_train, df_test
         self.epoch_num = int(self.util.config_val("EXP", "epochs", 1))
-
+        drop = self.util.config_val("MODEL", "drop", False)
+        self.drop = 0.1
+        if drop:
+            self.drop = float(drop)
+        self.util.debug(f"init: training with dropout: {self.drop}")
         self._init_model()
 
     def _init_model(self):
         model_path = "facebook/wav2vec2-large-robust-ft-swbd-300h"
+        pretrained_model = self.util.config_val("MODEL", "pretrained_model", model_path)
         self.num_layers = None
         self.sampling_rate = 16000
         self.max_duration_sec = 8.0
         self.accumulation_steps = 4
-        # create dataset
 
+        # print finetuning information via debug
+        self.util.debug(f"Finetuning from model: {pretrained_model}")
+
+        # create dataset
         dataset = {}
         target_name = glob_conf.target
         data_sources = {
             "train": pd.DataFrame(self.df_train[target_name]),
             "dev": pd.DataFrame(self.df_test[target_name]),
         }
 
@@ -72,30 +90,40 @@
             df.end = df.end.dt.total_seconds()
             ds = datasets.Dataset.from_pandas(df)
             dataset[split] = ds
 
         self.dataset = datasets.DatasetDict(dataset)
 
         # load pre-trained model
-        le = glob_conf.label_encoder
-        mapping = dict(zip(le.classes_, range(len(le.classes_))))
-        target_mapping = {k: int(v) for k, v in mapping.items()}
-        target_mapping_reverse = {value: key for key, value in target_mapping.items()}
-
-        self.config = transformers.AutoConfig.from_pretrained(
-            model_path,
-            num_labels=len(target_mapping),
-            label2id=target_mapping,
-            id2label=target_mapping_reverse,
-            finetuning_task=target_name,
-        )
+        if self.is_classifier:
+            le = glob_conf.label_encoder
+            mapping = dict(zip(le.classes_, range(len(le.classes_))))
+            target_mapping = {k: int(v) for k, v in mapping.items()}
+            target_mapping_reverse = {
+                value: key for key, value in target_mapping.items()
+            }
+            self.config = transformers.AutoConfig.from_pretrained(
+                model_path,
+                num_labels=len(target_mapping),
+                label2id=target_mapping,
+                id2label=target_mapping_reverse,
+                finetuning_task=target_name,
+            )
+        else:
+            self.config = transformers.AutoConfig.from_pretrained(
+                model_path,
+                num_labels=1,
+                finetuning_task=target_name,
+            )
         if self.num_layers is not None:
             self.config.num_hidden_layers = self.num_layers
+        self.config.final_dropout = self.drop
         setattr(self.config, "sampling_rate", self.sampling_rate)
         setattr(self.config, "data", self.util.get_data_name())
+        setattr(self.config, "is_classifier", self.is_classifier)
 
         vocab_dict = {}
         with open("vocab.json", "w") as vocab_file:
             json.dump(vocab_dict, vocab_file)
         tokenizer = transformers.Wav2Vec2CTCTokenizer("./vocab.json")
         tokenizer.save_pretrained(".")
 
@@ -109,15 +137,15 @@
         self.processor = transformers.Wav2Vec2Processor(
             feature_extractor=feature_extractor,
             tokenizer=tokenizer,
         )
         assert self.processor.feature_extractor.sampling_rate == self.sampling_rate
 
         self.model = Model.from_pretrained(
-            model_path,
+            pretrained_model,
             config=self.config,
         )
         self.model.freeze_feature_extractor()
         self.model.train()
         self.model_initialized = True
 
     def set_model_type(self, type):
@@ -166,32 +194,43 @@
         )
         batch = self.processor.pad(
             input_values,
             padding=True,
             return_tensors="pt",
         )
 
-        batch["labels"] = torch.tensor(targets)
+        batch["labels"] = torch.Tensor(targets)
 
         return batch
 
     def compute_metrics(self, p: transformers.EvalPrediction):
 
         metrics = {
             "UAR": audmetric.unweighted_average_recall,
             "ACC": audmetric.accuracy,
         }
+        metrics_reg = {
+            "PCC": audmetric.pearson_cc,
+            "CCC": audmetric.concordance_cc,
+            "MSE": audmetric.mean_squared_error,
+            "MAE": audmetric.mean_absolute_error,
+        }
 
         # truth = p.label_ids[:, 0].astype(int)
         truth = p.label_ids
         preds = p.predictions
         preds = np.argmax(preds, axis=1)
         scores = {}
-        for name, metric in metrics.items():
-            scores[f"{name}"] = metric(truth, preds)
+        if self.is_classifier:
+            for name, metric in metrics.items():
+                scores[f"{name}"] = metric(truth, preds)
+        else:
+            for name, metric in metrics_reg.items():
+                scores[f"{name}"] = metric(truth, preds)
+
         return scores
 
     def train(self):
         """Train the model."""
         model_root = self.util.get_path("model_dir")
         log_root = os.path.join(self.util.get_exp_dir(), "log")
         audeer.mkdir(log_root)
@@ -199,31 +238,32 @@
         conf_file = os.path.join(self.torch_root, "config.json")
         if os.path.isfile(conf_file):
             self.util.debug(f"reusing finetuned model: {conf_file}")
             self.load(self.run, self.epoch_num)
             return
         targets = pd.DataFrame(self.dataset["train"]["targets"])
         counts = targets[0].value_counts().sort_index()
-        train_weights = 1 / counts
-        train_weights /= train_weights.sum()
-        self.util.debug("train weights: {train_weights}")
-        criterion = torch.nn.CrossEntropyLoss(
-            weight=torch.Tensor(train_weights).to("cuda"),
-        )
-        # criterion = torch.nn.CrossEntropyLoss()
 
-        class Trainer(transformers.Trainer):
+        if self.is_classifier:
+            train_weights = 1 / counts
+            train_weights /= train_weights.sum()
+            self.util.debug(f"train weights: {train_weights}")
+            criterion = torch.nn.CrossEntropyLoss(
+                weight=torch.Tensor(train_weights).to("cuda"),
+            )
+        else:
+            criterion = ConcordanceCorCoeff()
 
+        class Trainer(transformers.Trainer):
             def compute_loss(
                 self,
                 model,
                 inputs,
                 return_outputs=False,
             ):
-
                 targets = inputs.pop("labels").squeeze()
                 targets = targets.type(torch.long)
 
                 outputs = model(**inputs)
                 logits = outputs[0].squeeze()
 
                 loss = criterion(logits, targets)
@@ -232,31 +272,33 @@
 
         num_steps = (
             len(self.dataset["train"])
             // (self.batch_size * self.accumulation_steps)
             // 5
         )
         num_steps = max(1, num_steps)
-        # print(num_steps)
+
+        metrics_for_best_model = self.measure.upper()
 
         training_args = transformers.TrainingArguments(
             output_dir=model_root,
             logging_dir=log_root,
             per_device_train_batch_size=self.batch_size,
             per_device_eval_batch_size=self.batch_size,
             gradient_accumulation_steps=self.accumulation_steps,
             evaluation_strategy="steps",
             num_train_epochs=self.epoch_num,
-            fp16=True,
+            fp16=self.device == "cuda",
             save_steps=num_steps,
             eval_steps=num_steps,
             logging_steps=num_steps,
-            learning_rate=1e-4,
+            logging_strategy="epoch",
+            learning_rate=self.learning_rate,
             save_total_limit=2,
-            metric_for_best_model="UAR",
+            metric_for_best_model=metrics_for_best_model,
             greater_is_better=True,
             load_best_model_at_end=True,
             remove_unused_columns=False,
             report_to="none",
         )
 
         trainer = Trainer(
@@ -267,14 +309,15 @@
             train_dataset=self.dataset["train"],
             eval_dataset=self.dataset["dev"],
             tokenizer=self.processor.feature_extractor,
             callbacks=[transformers.integrations.TensorBoardCallback()],
         )
         trainer.train()
         trainer.save_model(self.torch_root)
+        self.util.debug(f"saved best model to {self.torch_root}")
         self.load(self.run, self.epoch)
 
     def get_predictions(self):
         results = []
         for (file, start, end), _ in audeer.progress_bar(
             self.df_test.iterrows(),
             total=len(self.df_test),
@@ -301,15 +344,15 @@
             self.epoch_num,
         )
         return report
 
     def predict_sample(self, signal):
         """Predict one sample"""
         prediction = {}
-        if self.util.exp_is_classification():
+        if self.is_classifier:
             # get the class probabilities
             predictions = self.model.predict(signal)
             # pred = self.clf.predict(features)
             for i in range(len(self.labels)):
                 cat = self.labels[i]
                 prediction[cat] = predictions[i]
         else:
@@ -333,19 +376,30 @@
         with open(path, "rb") as handle:
             self.clf = pickle.load(handle)
 
 
 @dataclasses.dataclass
 class ModelOutput(transformers.file_utils.ModelOutput):
 
-    logits_cat: torch.FloatTensor = None
+    logits: torch.FloatTensor = None
     hidden_states: typing.Tuple[torch.FloatTensor] = None
     cnn_features: torch.FloatTensor = None
 
 
+@dataclasses.dataclass
+class ModelOutputReg(transformers.file_utils.ModelOutput):
+
+    logits: torch.FloatTensor
+    hidden_states: typing.Tuple[torch.FloatTensor] = None
+    attentions: typing.Tuple[torch.FloatTensor] = None
+    logits_framewise: torch.FloatTensor = None
+    hidden_states_framewise: torch.FloatTensor = None
+    cnn_features: torch.FloatTensor = None
+
+
 class ModelHead(torch.nn.Module):
 
     def __init__(self, config):
 
         super().__init__()
 
         self.dense = torch.nn.Linear(config.hidden_size, config.hidden_size)
@@ -364,18 +418,22 @@
         return x
 
 
 class Model(Wav2Vec2PreTrainedModel):
 
     def __init__(self, config):
 
+        if not hasattr(config, "add_adapter"):
+            setattr(config, "add_adapter", False)
+
         super().__init__(config)
 
         self.wav2vec2 = Wav2Vec2Model(config)
-        self.cat = ModelHead(config)
+        self.head = ModelHead(config)
+        self.is_classifier = config.is_classifier
         self.init_weights()
 
     def freeze_feature_extractor(self):
         self.wav2vec2.feature_extractor._freeze_parameters()
 
     def pooling(
         self,
@@ -403,77 +461,80 @@
     def forward(
         self,
         input_values,
         attention_mask=None,
         labels=None,
         return_hidden=False,
     ):
-
         outputs = self.wav2vec2(
             input_values,
             attention_mask=attention_mask,
         )
-
         cnn_features = outputs.extract_features
         hidden_states_framewise = outputs.last_hidden_state
         hidden_states = self.pooling(
             hidden_states_framewise,
             attention_mask,
         )
-        logits_cat = self.cat(hidden_states)
-
+        logits = self.head(hidden_states)
         if not self.training:
-            logits_cat = torch.softmax(logits_cat, dim=1)
+            logits = torch.softmax(logits, dim=1)
 
         if return_hidden:
-
             # make time last axis
             cnn_features = torch.transpose(cnn_features, 1, 2)
-
-            return ModelOutput(
-                logits_cat=logits_cat,
-                hidden_states=hidden_states,
-                cnn_features=cnn_features,
-            )
-
+            if self.is_classifier:
+                return ModelOutput(
+                    logits=logits,
+                    hidden_states=hidden_states,
+                    cnn_features=cnn_features,
+                )
+            else:
+                return ModelOutputReg(
+                    logits=logits,
+                    hidden_states=hidden_states,
+                    cnn_features=cnn_features,
+                )
         else:
-
-            return ModelOutput(
-                logits_cat=logits_cat,
-            )
+            if self.is_classifier:
+                return ModelOutput(
+                    logits=logits,
+                )
+            else:
+                return ModelOutputReg(
+                    logits=logits,
+                )
 
     def predict(self, signal):
         result = self(torch.from_numpy(signal))
         result = result[0].detach().numpy()[0]
         return result
 
 
-class ModelWithPreProcessing(Model):
+class ConcordanceCorCoeff(torch.nn.Module):
 
-    def __init__(self, config):
-        super().__init__(config)
-
-    def forward(
-        self,
-        input_values,
-    ):
-        # Wav2Vec2FeatureExtractor.zero_mean_unit_var_norm():
-        # normed_slice = (vector - vector[:length].mean()) / np.sqrt(vector[:length].var() + 1e-7)
-
-        mean = input_values.mean()
-
-        # var = input_values.var()
-        # raises: onnxruntime.capi.onnxruntime_pybind11_state.NotImplemented: [ONNXRuntimeError] : 9 : NOT_IMPLEMENTED : Could not find an implementation for the node ReduceProd_3:ReduceProd(11)
-
-        var = torch.square(input_values - mean).mean()
-        input_values = (input_values - mean) / torch.sqrt(var + 1e-7)
-
-        output = super().forward(
-            input_values,
-            return_hidden=True,
-        )
+    def __init__(self):
+        super().__init__()
+        self.mean = torch.mean
+        self.var = torch.var
+        self.sum = torch.sum
+        self.sqrt = torch.sqrt
+        self.std = torch.std
+
+    def forward(self, prediction, ground_truth):
+        ground_truth = ground_truth.float()
+        mean_gt = self.mean(ground_truth, 0)
+        mean_pred = self.mean(prediction, 0)
+        var_gt = self.var(ground_truth, 0)
+        var_pred = self.var(prediction, 0)
+        v_pred = prediction - mean_pred
+        v_gt = ground_truth - mean_gt
+        cor = self.sum(v_pred * v_gt) / (
+            self.sqrt(self.sum(v_pred**2)) * self.sqrt(self.sum(v_gt**2))
+        )
+        sd_gt = self.std(ground_truth)
+        sd_pred = self.std(prediction)
+        numerator = 2 * cor * sd_gt * sd_pred
+        denominator = var_gt + var_pred + (mean_gt - mean_pred) ** 2
+        ccc = numerator / denominator
 
-        return (
-            output.hidden_states,
-            output.logits_cat,
-            output.cnn_features,
-        )
+        return 1 - ccc
```

### Comparing `nkululeko-0.85.2/nkululeko/multidb.py` & `nkululeko-0.86.0/nkululeko/multidb.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/nkuluflag.py` & `nkululeko-0.86.0/nkululeko/nkuluflag.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/nkululeko.py` & `nkululeko-0.86.0/nkululeko/nkululeko.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/plots.py` & `nkululeko-0.86.0/nkululeko/plots.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/predict.py` & `nkululeko-0.86.0/nkululeko/predict.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/reporting/defines.py` & `nkululeko-0.86.0/nkululeko/reporting/defines.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/reporting/latex_writer.py` & `nkululeko-0.86.0/nkululeko/reporting/latex_writer.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/reporting/report.py` & `nkululeko-0.86.0/nkululeko/reporting/report.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/reporting/report_item.py` & `nkululeko-0.86.0/nkululeko/reporting/report_item.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/reporting/reporter.py` & `nkululeko-0.86.0/nkululeko/reporting/reporter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/reporting/result.py` & `nkululeko-0.86.0/nkululeko/reporting/result.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/resample.py` & `nkululeko-0.86.0/nkululeko/resample.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/runmanager.py` & `nkululeko-0.86.0/nkululeko/runmanager.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/scaler.py` & `nkululeko-0.86.0/nkululeko/scaler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/segment.py` & `nkululeko-0.86.0/nkululeko/segment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/segmenting/seg_inaspeechsegmenter.py` & `nkululeko-0.86.0/nkululeko/segmenting/seg_inaspeechsegmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/segmenting/seg_silero.py` & `nkululeko-0.86.0/nkululeko/segmenting/seg_silero.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/syllable_nuclei.py` & `nkululeko-0.86.0/nkululeko/syllable_nuclei.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/test.py` & `nkululeko-0.86.0/nkululeko/test.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/test_predictor.py` & `nkululeko-0.86.0/nkululeko/test_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/test_pretrain.py` & `nkululeko-0.86.0/nkululeko/test_pretrain.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/utils/files.py` & `nkululeko-0.86.0/nkululeko/utils/files.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/utils/stats.py` & `nkululeko-0.86.0/nkululeko/utils/stats.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko/utils/util.py` & `nkululeko-0.86.0/nkululeko/utils/util.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/nkululeko.egg-info/PKG-INFO` & `nkululeko-0.86.0/nkululeko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.85.2
+Version: 0.86.0
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -329,14 +329,20 @@
    year = {2022},
 }
 ```
 
 Changelog
 =========
 
+Version 0.86.0
+--------------
+* added regression to finetuning
+* added other transformer models to finetuning
+* added output the train/dev features sets actually used by the model
+
 Version 0.85.2
 --------------
 * added data, and automatic task label detection
 
 Version 0.85.1
 --------------
 * fixed bug in model_finetuned that label_num was constant 2
```

### Comparing `nkululeko-0.85.2/nkululeko.egg-info/SOURCES.txt` & `nkululeko-0.86.0/nkululeko.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,14 @@
 nkululeko/feat_extract/feats_whisper.py
 nkululeko/feat_extract/featureset.py
 nkululeko/feat_extract/feinberg_praat.py
 nkululeko/losses/__init__.py
 nkululeko/losses/loss_ccc.py
 nkululeko/losses/loss_softf1loss.py
 nkululeko/models/__init__.py
-nkululeko/models/finetune_model.py
 nkululeko/models/model.py
 nkululeko/models/model_bayes.py
 nkululeko/models/model_cnn.py
 nkululeko/models/model_gmm.py
 nkululeko/models/model_knn.py
 nkululeko/models/model_knn_reg.py
 nkululeko/models/model_lin_reg.py
```

### Comparing `nkululeko-0.85.2/setup.cfg` & `nkululeko-0.86.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `nkululeko-0.85.2/venv/bin/activate_this.py` & `nkululeko-0.86.0/venv/bin/activate_this.py`

 * *Files identical despite different names*

