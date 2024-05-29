# Comparing `tmp/musicntwrk-2.3.6.tar.gz` & `tmp/musicntwrk-2.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musicntwrk-2.3.6.tar", last modified: Fri May 17 15:27:25 2024, max compression
+gzip compressed data, was "musicntwrk-2.3.7.tar", last modified: Wed May 29 21:35:28 2024, max compression
```

## Comparing `musicntwrk-2.3.6.tar` & `musicntwrk-2.3.7.tar`

### file list

```diff
@@ -1,186 +1,186 @@
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-17 15:27:25.665170 musicntwrk-2.3.6/
--rw-r--r--   0 marco      (502) staff       (20)     7568 2024-05-17 15:27:25.664958 musicntwrk-2.3.6/PKG-INFO
--rw-r--r--   0 marco      (502) staff       (20)     6849 2022-07-24 12:39:52.000000 musicntwrk-2.3.6/README.md
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-17 15:27:25.664463 musicntwrk-2.3.6/musicntwrk.egg-info/
--rw-r--r--   0 marco      (502) staff       (20)     7568 2024-05-17 15:27:25.000000 musicntwrk-2.3.6/musicntwrk.egg-info/PKG-INFO
--rw-r--r--   0 marco      (502) staff       (20)     4795 2024-05-17 15:27:25.000000 musicntwrk-2.3.6/musicntwrk.egg-info/SOURCES.txt
--rw-r--r--   0 marco      (502) staff       (20)        1 2024-05-17 15:27:25.000000 musicntwrk-2.3.6/musicntwrk.egg-info/dependency_links.txt
--rw-r--r--   0 marco      (502) staff       (20)      159 2024-05-17 15:27:25.000000 musicntwrk-2.3.6/musicntwrk.egg-info/requires.txt
--rw-r--r--   0 marco      (502) staff       (20)       11 2024-05-17 15:27:25.000000 musicntwrk-2.3.6/musicntwrk.egg-info/top_level.txt
--rw-r--r--   0 marco      (502) staff       (20)       97 2023-06-23 22:57:58.000000 musicntwrk-2.3.6/pyproject.toml
--rw-r--r--   0 marco      (502) staff       (20)       38 2024-05-17 15:27:25.665215 musicntwrk-2.3.6/setup.cfg
--rw-r--r--   0 marco      (502) staff       (20)     1508 2024-05-17 15:25:50.000000 musicntwrk-2.3.6/setup.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-17 15:27:25.636323 musicntwrk-2.3.6/src/
--rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/__init__.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-17 15:27:25.637502 musicntwrk-2.3.6/src/comptools/
--rw-r--r--   0 marco      (502) staff       (20)    39621 2021-05-31 23:27:25.000000 musicntwrk-2.3.6/src/comptools/MidiFile.py
--rw-r--r--   0 marco      (502) staff       (20)     1762 2024-03-14 00:36:27.000000 musicntwrk-2.3.6/src/comptools/displayNotes.py
--rw-r--r--   0 marco      (502) staff       (20)     2786 2021-09-23 16:53:48.000000 musicntwrk-2.3.6/src/comptools/genmidi.py
--rw-r--r--   0 marco      (502) staff       (20)     7771 2023-05-25 20:48:36.000000 musicntwrk-2.3.6/src/comptools/music.py
--rw-r--r--   0 marco      (502) staff       (20)     1888 2021-05-31 23:27:25.000000 musicntwrk-2.3.6/src/comptools/notation.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-17 15:27:25.640809 musicntwrk-2.3.6/src/data/
--rw-r--r--   0 marco      (502) staff       (20)      828 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/data/MIDImap.py
--rw-r--r--   0 marco      (502) staff       (20)     2559 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/data/MIDImidi.py
--rw-r--r--   0 marco      (502) staff       (20)      988 2023-05-25 21:55:41.000000 musicntwrk-2.3.6/src/data/MIDIscore.py
--rw-r--r--   0 marco      (502) staff       (20)     1275 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/data/WRITEscore.py
--rw-r--r--   0 marco      (502) staff       (20)     1013 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/data/WRITEscoreNoTime.py
--rw-r--r--   0 marco      (502) staff       (20)     2086 2023-01-08 21:25:29.000000 musicntwrk-2.3.6/src/data/WRITEscoreOps.py
--rw-r--r--   0 marco      (502) staff       (20)     3272 2021-10-26 23:20:31.000000 musicntwrk-2.3.6/src/data/WRITEscoreOpsMIDI.py
--rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/data/__init__.py
--rw-r--r--   0 marco      (502) staff       (20)     2926 2024-04-24 14:48:35.000000 musicntwrk-2.3.6/src/data/analyzeSound.py
--rw-r--r--   0 marco      (502) staff       (20)     3956 2024-04-24 14:48:49.000000 musicntwrk-2.3.6/src/data/analyzeTimbre.py
--rw-r--r--   0 marco      (502) staff       (20)   114667 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/data/ctcsound.py
--rw-r--r--   0 marco      (502) staff       (20)     3993 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/data/i_spectral.py
--rw-r--r--   0 marco      (502) staff       (20)     3275 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/data/i_spectral2.py
--rw-r--r--   0 marco      (502) staff       (20)     1921 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/data/i_spectral_pure.py
--rw-r--r--   0 marco      (502) staff       (20)     2597 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/data/i_spectral_pyo.py
--rw-r--r--   0 marco      (502) staff       (20)     6358 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/data/i_time_series.py
--rw-r--r--   0 marco      (502) staff       (20)     1270 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/data/r_1Ddata.py
--rw-r--r--   0 marco      (502) staff       (20)    10624 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/data/scaleMapping.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-17 15:27:25.644600 musicntwrk-2.3.6/src/harmony/
--rw-r--r--   0 marco      (502) staff       (20)       66 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/harmony/__init__.py
--rw-r--r--   0 marco      (502) staff       (20)     2035 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/harmony/applyOps.py
--rw-r--r--   0 marco      (502) staff       (20)     1256 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/harmony/changePoint.py
--rw-r--r--   0 marco      (502) staff       (20)     2640 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/harmony/chinese_postman.py
--rw-r--r--   0 marco      (502) staff       (20)     1703 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/harmony/enharmonicDictionary.py
--rw-r--r--   0 marco      (502) staff       (20)     1309 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/harmony/getRN.py
--rw-r--r--   0 marco      (502) staff       (20)     4137 2024-04-30 22:40:21.000000 musicntwrk-2.3.6/src/harmony/harmonicDesign.py
--rw-r--r--   0 marco      (502) staff       (20)     3055 2024-04-24 15:25:04.000000 musicntwrk-2.3.6/src/harmony/keySections.py
--rw-r--r--   0 marco      (502) staff       (20)     3022 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/harmony/lookupOps.py
--rw-r--r--   0 marco      (502) staff       (20)      884 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/harmony/lookupProgr.py
--rw-r--r--   0 marco      (502) staff       (20)     1265 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/harmony/lookupWrapper.py
--rw-r--r--   0 marco      (502) staff       (20)     2416 2023-08-02 08:26:29.000000 musicntwrk-2.3.6/src/harmony/networkHarmonyGen.py
--rw-r--r--   0 marco      (502) staff       (20)     2769 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/harmony/plotHarmonicTable.py
--rw-r--r--   0 marco      (502) staff       (20)     2784 2023-12-28 02:44:32.000000 musicntwrk-2.3.6/src/harmony/rhythmicDesign.py
--rw-r--r--   0 marco      (502) staff       (20)     4765 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/harmony/scoreAnalysis.py
--rw-r--r--   0 marco      (502) staff       (20)     1257 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/harmony/scoreDesign.py
--rw-r--r--   0 marco      (502) staff       (20)     2307 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/harmony/scoreFilter.py
--rw-r--r--   0 marco      (502) staff       (20)     2492 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/harmony/shortHands.py
--rw-r--r--   0 marco      (502) staff       (20)     2002 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/harmony/showAnalysis.py
--rw-r--r--   0 marco      (502) staff       (20)     4473 2023-08-02 08:24:19.000000 musicntwrk-2.3.6/src/harmony/spiralChordSpace.py
--rw-r--r--   0 marco      (502) staff       (20)     2921 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/harmony/tonalAnalysis.py
--rw-r--r--   0 marco      (502) staff       (20)     7685 2023-01-27 02:25:22.000000 musicntwrk-2.3.6/src/harmony/tonalHarmonyCalculator.py
--rw-r--r--   0 marco      (502) staff       (20)     4652 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/harmony/tonalHarmonyModels.py
--rw-r--r--   0 marco      (502) staff       (20)     1899 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/harmony/tonalPartition.py
--rw-r--r--   0 marco      (502) staff       (20)     2647 2024-04-24 21:17:23.000000 musicntwrk-2.3.6/src/harmony/tonnentz.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-17 15:27:25.646227 musicntwrk-2.3.6/src/ml_utils/
--rw-r--r--   0 marco      (502) staff       (20)       88 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/ml_utils/__init__.py
--rw-r--r--   0 marco      (502) staff       (20)     2695 2024-04-14 21:34:16.000000 musicntwrk-2.3.6/src/ml_utils/checkRun.py
--rw-r--r--   0 marco      (502) staff       (20)     1407 2024-04-14 21:35:54.000000 musicntwrk-2.3.6/src/ml_utils/modelDump.py
--rw-r--r--   0 marco      (502) staff       (20)     1479 2024-04-14 22:54:15.000000 musicntwrk-2.3.6/src/ml_utils/modelLoad.py
--rw-r--r--   0 marco      (502) staff       (20)     1513 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/ml_utils/multiModelPredictor.py
--rw-r--r--   0 marco      (502) staff       (20)     1432 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/ml_utils/prepareDataSet.py
--rw-r--r--   0 marco      (502) staff       (20)     2024 2024-04-15 02:03:11.000000 musicntwrk-2.3.6/src/ml_utils/readModels.py
--rw-r--r--   0 marco      (502) staff       (20)      814 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/ml_utils/scaleDataSet.py
--rw-r--r--   0 marco      (502) staff       (20)     3299 2024-04-14 22:01:21.000000 musicntwrk-2.3.6/src/ml_utils/trainCNNmodel.py
--rw-r--r--   0 marco      (502) staff       (20)     2260 2024-04-14 21:50:15.000000 musicntwrk-2.3.6/src/ml_utils/trainNNmodel.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-17 15:27:25.650581 musicntwrk-2.3.6/src/msctools/
--rw-r--r--   0 marco      (502) staff       (20)     9430 2024-05-17 02:06:40.000000 musicntwrk-2.3.6/src/msctools/base.py
--rw-r--r--   0 marco      (502) staff       (20)      597 2024-05-11 18:48:50.000000 musicntwrk-2.3.6/src/msctools/cfg.py
--rw-r--r--   0 marco      (502) staff       (20)     2248 2023-09-08 07:15:36.000000 musicntwrk-2.3.6/src/msctools/converters.py
--rw-r--r--   0 marco      (502) staff       (20)      336 2024-01-30 00:27:07.000000 musicntwrk-2.3.6/src/msctools/decorators.py
--rw-r--r--   0 marco      (502) staff       (20)     7080 2024-05-02 20:15:38.000000 musicntwrk-2.3.6/src/msctools/devices.py
--rw-r--r--   0 marco      (502) staff       (20)    78504 2024-01-20 15:29:09.000000 musicntwrk-2.3.6/src/msctools/dictionaries.py
--rw-r--r--   0 marco      (502) staff       (20)    48647 2023-11-09 23:14:46.000000 musicntwrk-2.3.6/src/msctools/dsp.py
--rw-r--r--   0 marco      (502) staff       (20)     5951 2024-05-02 20:33:09.000000 musicntwrk-2.3.6/src/msctools/envelopes.py
--rw-r--r--   0 marco      (502) staff       (20)     8785 2024-05-17 14:38:55.000000 musicntwrk-2.3.6/src/msctools/envelopes_thread.py
--rw-r--r--   0 marco      (502) staff       (20)    19624 2024-04-20 12:45:11.000000 musicntwrk-2.3.6/src/msctools/networks.py
--rw-r--r--   0 marco      (502) staff       (20)      865 2023-04-13 16:06:16.000000 musicntwrk-2.3.6/src/msctools/oscserver.py
--rw-r--r--   0 marco      (502) staff       (20)     2119 2024-05-11 15:37:48.000000 musicntwrk-2.3.6/src/msctools/osctools.py
--rw-r--r--   0 marco      (502) staff       (20)      472 2022-11-22 00:46:09.000000 musicntwrk-2.3.6/src/msctools/pan.py
--rw-r--r--   0 marco      (502) staff       (20)     4826 2024-05-02 20:19:05.000000 musicntwrk-2.3.6/src/msctools/players.py
--rw-r--r--   0 marco      (502) staff       (20)     8801 2024-05-17 14:50:52.000000 musicntwrk-2.3.6/src/msctools/players_thread.py
--rw-r--r--   0 marco      (502) staff       (20)     1648 2024-05-02 20:19:16.000000 musicntwrk-2.3.6/src/msctools/pyoPlayer.py
--rw-r--r--   0 marco      (502) staff       (20)    17002 2024-04-20 13:03:26.000000 musicntwrk-2.3.6/src/msctools/pyotools.py
--rw-r--r--   0 marco      (502) staff       (20)     1374 2024-05-02 20:19:32.000000 musicntwrk-2.3.6/src/msctools/session.py
--rw-r--r--   0 marco      (502) staff       (20)      680 2024-05-05 22:00:38.000000 musicntwrk-2.3.6/src/msctools/utils.py
--rw-r--r--   0 marco      (502) staff       (20)     5386 2023-04-13 16:05:54.000000 musicntwrk-2.3.6/src/msctools/videocapture.py
--rw-r--r--   0 marco      (502) staff       (20)    68822 2024-01-26 02:18:22.000000 musicntwrk-2.3.6/src/musicntwrk.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-17 15:27:25.654485 musicntwrk-2.3.6/src/networks/
--rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/networks/__init__.py
--rw-r--r--   0 marco      (502) staff       (20)     2580 2023-08-02 08:22:01.000000 musicntwrk-2.3.6/src/networks/analysisNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     2646 2023-08-02 08:22:01.000000 musicntwrk-2.3.6/src/networks/orchestralNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     2388 2023-04-04 23:24:43.000000 musicntwrk-2.3.6/src/networks/orchestralVector.py
--rw-r--r--   0 marco      (502) staff       (20)     1695 2024-04-24 21:12:18.000000 musicntwrk-2.3.6/src/networks/orchestralVectorColor.py
--rw-r--r--   0 marco      (502) staff       (20)     4853 2024-04-24 15:27:50.000000 musicntwrk-2.3.6/src/networks/pcsDictionary.py
--rw-r--r--   0 marco      (502) staff       (20)     5852 2023-08-02 08:22:01.000000 musicntwrk-2.3.6/src/networks/pcsEgoNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     4914 2023-08-02 08:22:01.000000 musicntwrk-2.3.6/src/networks/pcsNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     2966 2023-08-02 08:22:01.000000 musicntwrk-2.3.6/src/networks/rLeadNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     2470 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/networks/readScore.py
--rw-r--r--   0 marco      (502) staff       (20)     3085 2022-01-09 00:40:38.000000 musicntwrk-2.3.6/src/networks/rhythmDictionary.py
--rw-r--r--   0 marco      (502) staff       (20)     4322 2023-08-02 08:22:01.000000 musicntwrk-2.3.6/src/networks/rhythmNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     4053 2023-12-28 02:35:13.000000 musicntwrk-2.3.6/src/networks/rhythmPDictionary.py
--rw-r--r--   0 marco      (502) staff       (20)     2456 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/networks/scoreDictionary.py
--rw-r--r--   0 marco      (502) staff       (20)     1592 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/networks/scoreMIDIDictionary.py
--rw-r--r--   0 marco      (502) staff       (20)     5809 2023-08-02 08:22:01.000000 musicntwrk-2.3.6/src/networks/scoreNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     5791 2023-08-02 08:22:01.000000 musicntwrk-2.3.6/src/networks/scoreSubNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     3697 2023-08-02 08:22:01.000000 musicntwrk-2.3.6/src/networks/timbralNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     4102 2023-08-02 08:22:01.000000 musicntwrk-2.3.6/src/networks/vLeadNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     4789 2023-08-02 08:22:01.000000 musicntwrk-2.3.6/src/networks/vLeadNetworkByName.py
--rw-r--r--   0 marco      (502) staff       (20)     2936 2023-08-02 08:22:01.000000 musicntwrk-2.3.6/src/networks/vLeadNetworkByNameVec.py
--rw-r--r--   0 marco      (502) staff       (20)     2634 2023-08-02 08:22:01.000000 musicntwrk-2.3.6/src/networks/vLeadNetworkVec.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-17 15:27:25.656255 musicntwrk-2.3.6/src/plotting/
--rw-r--r--   0 marco      (502) staff       (20)     1066 2024-04-24 14:49:13.000000 musicntwrk-2.3.6/src/plotting/barplot.py
--rw-r--r--   0 marco      (502) staff       (20)    24919 2023-12-21 02:30:18.000000 musicntwrk-2.3.6/src/plotting/chordspace.py
--rw-r--r--   0 marco      (502) staff       (20)     7250 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/plotting/drawMultiLayerNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     2888 2023-07-05 22:49:56.000000 musicntwrk-2.3.6/src/plotting/drawNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     6340 2023-08-02 09:17:49.000000 musicntwrk-2.3.6/src/plotting/drawNetwork3D.py
--rw-r--r--   0 marco      (502) staff       (20)     2256 2021-11-23 20:31:22.000000 musicntwrk-2.3.6/src/plotting/drawNetworkViz.py
--rw-r--r--   0 marco      (502) staff       (20)     1246 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/plotting/drawNetworkX.py
--rw-r--r--   0 marco      (502) staff       (20)      895 2024-04-24 14:49:25.000000 musicntwrk-2.3.6/src/plotting/plotCC.py
--rw-r--r--   0 marco      (502) staff       (20)      716 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/plotting/plotCurveXY.py
--rw-r--r--   0 marco      (502) staff       (20)      711 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/plotting/plotCurveY.py
--rw-r--r--   0 marco      (502) staff       (20)     1680 2023-08-02 14:25:53.000000 musicntwrk-2.3.6/src/plotting/plotDegreeAnalysis.py
--rw-r--r--   0 marco      (502) staff       (20)     1869 2024-04-24 14:50:13.000000 musicntwrk-2.3.6/src/plotting/plotOpsHistogram.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-17 15:27:25.658276 musicntwrk-2.3.6/src/timbre/
--rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/timbre/__init__.py
--rw-r--r--   0 marco      (502) staff       (20)     1743 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/timbre/computeASCBW.py
--rw-r--r--   0 marco      (502) staff       (20)     1552 2023-04-04 23:13:40.000000 musicntwrk-2.3.6/src/timbre/computeCompMPS.py
--rw-r--r--   0 marco      (502) staff       (20)     1663 2023-04-04 23:14:32.000000 musicntwrk-2.3.6/src/timbre/computeMFCC.py
--rw-r--r--   0 marco      (502) staff       (20)     2653 2024-04-24 14:50:05.000000 musicntwrk-2.3.6/src/timbre/computeModifiedASCBW.py
--rw-r--r--   0 marco      (502) staff       (20)     1475 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/timbre/computePSCC.py
--rw-r--r--   0 marco      (502) staff       (20)     2263 2023-06-23 21:10:40.000000 musicntwrk-2.3.6/src/timbre/computeStandardizedMFCC.py
--rw-r--r--   0 marco      (502) staff       (20)     1769 2022-10-29 00:30:08.000000 musicntwrk-2.3.6/src/timbre/computeStandardizedMFPS.py
--rw-r--r--   0 marco      (502) staff       (20)     1926 2022-10-29 00:29:28.000000 musicntwrk-2.3.6/src/timbre/computeStandardizedPSCC.py
--rw-r--r--   0 marco      (502) staff       (20)     1194 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/timbre/mfccSoundDecay.py
--rw-r--r--   0 marco      (502) staff       (20)      848 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/timbre/mfccSoundDecayOptimal.py
--rw-r--r--   0 marco      (502) staff       (20)     1395 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/timbre/mfccSoundDecayPiecewise.py
--rw-r--r--   0 marco      (502) staff       (20)     2092 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/timbre/minimizeBKPT.py
--rw-r--r--   0 marco      (502) staff       (20)      974 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/timbre/normSoundDecay.py
--rw-r--r--   0 marco      (502) staff       (20)     1342 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/timbre/normSoundDecay2.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-17 15:27:25.664287 musicntwrk-2.3.6/src/utils/
--rw-r--r--   0 marco      (502) staff       (20)     1142 2023-05-25 21:57:17.000000 musicntwrk-2.3.6/src/utils/Remove.py
--rw-r--r--   0 marco      (502) staff       (20)     1962 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/utils/SegmentedLinearReg.py
--rw-r--r--   0 marco      (502) staff       (20)      884 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/utils/Sublists.py
--rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/utils/__init__.py
--rw-r--r--   0 marco      (502) staff       (20)     3121 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/utils/communications.py
--rw-r--r--   0 marco      (502) staff       (20)     9768 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/utils/diffusionEntropyAnalyis.py
--rw-r--r--   0 marco      (502) staff       (20)     5511 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/utils/diffusionEntropyAnalyisNew.py
--rw-r--r--   0 marco      (502) staff       (20)     1758 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/utils/entropyKLdiv.py
--rw-r--r--   0 marco      (502) staff       (20)     1005 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/utils/extractByString.py
--rw-r--r--   0 marco      (502) staff       (20)      830 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/utils/fetchWaves.py
--rw-r--r--   0 marco      (502) staff       (20)     1086 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/utils/findLengthMax.py
--rw-r--r--   0 marco      (502) staff       (20)      883 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/utils/flatten.py
--rw-r--r--   0 marco      (502) staff       (20)      591 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/utils/floatize.py
--rw-r--r--   0 marco      (502) staff       (20)     1669 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/utils/generalizedOpsHistogram.py
--rw-r--r--   0 marco      (502) staff       (20)     1541 2022-06-24 15:34:43.000000 musicntwrk-2.3.6/src/utils/generalizedOpsName.py
--rw-r--r--   0 marco      (502) staff       (20)      760 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/utils/init_list_of_objects.py
--rw-r--r--   0 marco      (502) staff       (20)     1700 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/utils/load_balancing.py
--rw-r--r--   0 marco      (502) staff       (20)     1398 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/utils/minimalDistance.py
--rw-r--r--   0 marco      (502) staff       (20)     1297 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/utils/minimalDistanceVec.py
--rw-r--r--   0 marco      (502) staff       (20)     1401 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/utils/minimalNoBijDistance.py
--rw-r--r--   0 marco      (502) staff       (20)     1053 2021-11-19 16:54:18.000000 musicntwrk-2.3.6/src/utils/opsCheckByName.py
--rw-r--r--   0 marco      (502) staff       (20)      827 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/utils/opsCheckByNameVec.py
--rw-r--r--   0 marco      (502) staff       (20)      878 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/utils/opsDistance.py
--rw-r--r--   0 marco      (502) staff       (20)     1653 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/utils/opsHistogram.py
--rw-r--r--   0 marco      (502) staff       (20)     1537 2021-11-12 22:37:18.000000 musicntwrk-2.3.6/src/utils/opsName.py
--rw-r--r--   0 marco      (502) staff       (20)     2413 2021-11-19 01:35:52.000000 musicntwrk-2.3.6/src/utils/opsNameFull.py
--rw-r--r--   0 marco      (502) staff       (20)     1638 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/utils/opsNameVec.py
--rw-r--r--   0 marco      (502) staff       (20)      721 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/utils/play_with_simpleaudio.py
--rw-r--r--   0 marco      (502) staff       (20)     4681 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/utils/powerFit.py
--rw-r--r--   0 marco      (502) staff       (20)     1384 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/utils/rhythmDistance.py
--rw-r--r--   0 marco      (502) staff       (20)     2605 2021-08-06 01:36:29.000000 musicntwrk-2.3.6/src/utils/scaleFreeFit.py
--rw-r--r--   0 marco      (502) staff       (20)     1130 2021-11-22 17:37:40.000000 musicntwrk-2.3.6/src/utils/score2vLead.py
--rw-r--r--   0 marco      (502) staff       (20)      730 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/utils/str2float.py
--rw-r--r--   0 marco      (502) staff       (20)      702 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/utils/str2frac.py
--rw-r--r--   0 marco      (502) staff       (20)      963 2021-06-25 20:55:30.000000 musicntwrk-2.3.6/src/utils/vectorDistance.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-29 21:35:28.321792 musicntwrk-2.3.7/
+-rw-r--r--   0 marco      (502) staff       (20)     7568 2024-05-29 21:35:28.315714 musicntwrk-2.3.7/PKG-INFO
+-rw-r--r--   0 marco      (502) staff       (20)     6849 2022-07-24 12:39:52.000000 musicntwrk-2.3.7/README.md
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-29 21:35:28.315258 musicntwrk-2.3.7/musicntwrk.egg-info/
+-rw-r--r--   0 marco      (502) staff       (20)     7568 2024-05-29 21:35:28.000000 musicntwrk-2.3.7/musicntwrk.egg-info/PKG-INFO
+-rw-r--r--   0 marco      (502) staff       (20)     4795 2024-05-29 21:35:28.000000 musicntwrk-2.3.7/musicntwrk.egg-info/SOURCES.txt
+-rw-r--r--   0 marco      (502) staff       (20)        1 2024-05-29 21:35:28.000000 musicntwrk-2.3.7/musicntwrk.egg-info/dependency_links.txt
+-rw-r--r--   0 marco      (502) staff       (20)      159 2024-05-29 21:35:28.000000 musicntwrk-2.3.7/musicntwrk.egg-info/requires.txt
+-rw-r--r--   0 marco      (502) staff       (20)       11 2024-05-29 21:35:28.000000 musicntwrk-2.3.7/musicntwrk.egg-info/top_level.txt
+-rw-r--r--   0 marco      (502) staff       (20)       97 2023-06-23 22:57:58.000000 musicntwrk-2.3.7/pyproject.toml
+-rw-r--r--   0 marco      (502) staff       (20)       38 2024-05-29 21:35:28.321953 musicntwrk-2.3.7/setup.cfg
+-rw-r--r--   0 marco      (502) staff       (20)     1508 2024-05-29 21:22:28.000000 musicntwrk-2.3.7/setup.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-29 21:35:28.292036 musicntwrk-2.3.7/src/
+-rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/__init__.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-29 21:35:28.293175 musicntwrk-2.3.7/src/comptools/
+-rw-r--r--   0 marco      (502) staff       (20)    39621 2021-05-31 23:27:25.000000 musicntwrk-2.3.7/src/comptools/MidiFile.py
+-rw-r--r--   0 marco      (502) staff       (20)     1762 2024-03-14 00:36:27.000000 musicntwrk-2.3.7/src/comptools/displayNotes.py
+-rw-r--r--   0 marco      (502) staff       (20)     2786 2021-09-23 16:53:48.000000 musicntwrk-2.3.7/src/comptools/genmidi.py
+-rw-r--r--   0 marco      (502) staff       (20)     7771 2023-05-25 20:48:36.000000 musicntwrk-2.3.7/src/comptools/music.py
+-rw-r--r--   0 marco      (502) staff       (20)     1888 2021-05-31 23:27:25.000000 musicntwrk-2.3.7/src/comptools/notation.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-29 21:35:28.295767 musicntwrk-2.3.7/src/data/
+-rw-r--r--   0 marco      (502) staff       (20)      828 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/data/MIDImap.py
+-rw-r--r--   0 marco      (502) staff       (20)     2559 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/data/MIDImidi.py
+-rw-r--r--   0 marco      (502) staff       (20)      988 2023-05-25 21:55:41.000000 musicntwrk-2.3.7/src/data/MIDIscore.py
+-rw-r--r--   0 marco      (502) staff       (20)     1275 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/data/WRITEscore.py
+-rw-r--r--   0 marco      (502) staff       (20)     1013 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/data/WRITEscoreNoTime.py
+-rw-r--r--   0 marco      (502) staff       (20)     2086 2023-01-08 21:25:29.000000 musicntwrk-2.3.7/src/data/WRITEscoreOps.py
+-rw-r--r--   0 marco      (502) staff       (20)     3272 2021-10-26 23:20:31.000000 musicntwrk-2.3.7/src/data/WRITEscoreOpsMIDI.py
+-rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/data/__init__.py
+-rw-r--r--   0 marco      (502) staff       (20)     2926 2024-04-24 14:48:35.000000 musicntwrk-2.3.7/src/data/analyzeSound.py
+-rw-r--r--   0 marco      (502) staff       (20)     3956 2024-04-24 14:48:49.000000 musicntwrk-2.3.7/src/data/analyzeTimbre.py
+-rw-r--r--   0 marco      (502) staff       (20)   114667 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/data/ctcsound.py
+-rw-r--r--   0 marco      (502) staff       (20)     3993 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/data/i_spectral.py
+-rw-r--r--   0 marco      (502) staff       (20)     3275 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/data/i_spectral2.py
+-rw-r--r--   0 marco      (502) staff       (20)     1921 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/data/i_spectral_pure.py
+-rw-r--r--   0 marco      (502) staff       (20)     2597 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/data/i_spectral_pyo.py
+-rw-r--r--   0 marco      (502) staff       (20)     6358 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/data/i_time_series.py
+-rw-r--r--   0 marco      (502) staff       (20)     1270 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/data/r_1Ddata.py
+-rw-r--r--   0 marco      (502) staff       (20)    10624 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/data/scaleMapping.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-29 21:35:28.298515 musicntwrk-2.3.7/src/harmony/
+-rw-r--r--   0 marco      (502) staff       (20)       66 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/harmony/__init__.py
+-rw-r--r--   0 marco      (502) staff       (20)     2035 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/harmony/applyOps.py
+-rw-r--r--   0 marco      (502) staff       (20)     1256 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/harmony/changePoint.py
+-rw-r--r--   0 marco      (502) staff       (20)     2640 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/harmony/chinese_postman.py
+-rw-r--r--   0 marco      (502) staff       (20)     1703 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/harmony/enharmonicDictionary.py
+-rw-r--r--   0 marco      (502) staff       (20)     1309 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/harmony/getRN.py
+-rw-r--r--   0 marco      (502) staff       (20)     4137 2024-04-30 22:40:21.000000 musicntwrk-2.3.7/src/harmony/harmonicDesign.py
+-rw-r--r--   0 marco      (502) staff       (20)     3055 2024-04-24 15:25:04.000000 musicntwrk-2.3.7/src/harmony/keySections.py
+-rw-r--r--   0 marco      (502) staff       (20)     3022 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/harmony/lookupOps.py
+-rw-r--r--   0 marco      (502) staff       (20)      884 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/harmony/lookupProgr.py
+-rw-r--r--   0 marco      (502) staff       (20)     1265 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/harmony/lookupWrapper.py
+-rw-r--r--   0 marco      (502) staff       (20)     2416 2023-08-02 08:26:29.000000 musicntwrk-2.3.7/src/harmony/networkHarmonyGen.py
+-rw-r--r--   0 marco      (502) staff       (20)     2769 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/harmony/plotHarmonicTable.py
+-rw-r--r--   0 marco      (502) staff       (20)     2784 2023-12-28 02:44:32.000000 musicntwrk-2.3.7/src/harmony/rhythmicDesign.py
+-rw-r--r--   0 marco      (502) staff       (20)     4765 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/harmony/scoreAnalysis.py
+-rw-r--r--   0 marco      (502) staff       (20)     1257 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/harmony/scoreDesign.py
+-rw-r--r--   0 marco      (502) staff       (20)     2307 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/harmony/scoreFilter.py
+-rw-r--r--   0 marco      (502) staff       (20)     2492 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/harmony/shortHands.py
+-rw-r--r--   0 marco      (502) staff       (20)     2002 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/harmony/showAnalysis.py
+-rw-r--r--   0 marco      (502) staff       (20)     4473 2023-08-02 08:24:19.000000 musicntwrk-2.3.7/src/harmony/spiralChordSpace.py
+-rw-r--r--   0 marco      (502) staff       (20)     2921 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/harmony/tonalAnalysis.py
+-rw-r--r--   0 marco      (502) staff       (20)     7685 2023-01-27 02:25:22.000000 musicntwrk-2.3.7/src/harmony/tonalHarmonyCalculator.py
+-rw-r--r--   0 marco      (502) staff       (20)     4652 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/harmony/tonalHarmonyModels.py
+-rw-r--r--   0 marco      (502) staff       (20)     1899 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/harmony/tonalPartition.py
+-rw-r--r--   0 marco      (502) staff       (20)     2647 2024-04-24 21:17:23.000000 musicntwrk-2.3.7/src/harmony/tonnentz.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-29 21:35:28.299596 musicntwrk-2.3.7/src/ml_utils/
+-rw-r--r--   0 marco      (502) staff       (20)       88 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/ml_utils/__init__.py
+-rw-r--r--   0 marco      (502) staff       (20)     2695 2024-04-14 21:34:16.000000 musicntwrk-2.3.7/src/ml_utils/checkRun.py
+-rw-r--r--   0 marco      (502) staff       (20)     1407 2024-04-14 21:35:54.000000 musicntwrk-2.3.7/src/ml_utils/modelDump.py
+-rw-r--r--   0 marco      (502) staff       (20)     1479 2024-04-14 22:54:15.000000 musicntwrk-2.3.7/src/ml_utils/modelLoad.py
+-rw-r--r--   0 marco      (502) staff       (20)     1513 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/ml_utils/multiModelPredictor.py
+-rw-r--r--   0 marco      (502) staff       (20)     1432 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/ml_utils/prepareDataSet.py
+-rw-r--r--   0 marco      (502) staff       (20)     2024 2024-04-15 02:03:11.000000 musicntwrk-2.3.7/src/ml_utils/readModels.py
+-rw-r--r--   0 marco      (502) staff       (20)      814 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/ml_utils/scaleDataSet.py
+-rw-r--r--   0 marco      (502) staff       (20)     3299 2024-04-14 22:01:21.000000 musicntwrk-2.3.7/src/ml_utils/trainCNNmodel.py
+-rw-r--r--   0 marco      (502) staff       (20)     2260 2024-04-14 21:50:15.000000 musicntwrk-2.3.7/src/ml_utils/trainNNmodel.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-29 21:35:28.302843 musicntwrk-2.3.7/src/msctools/
+-rw-r--r--   0 marco      (502) staff       (20)     9913 2024-05-29 17:54:42.000000 musicntwrk-2.3.7/src/msctools/base.py
+-rw-r--r--   0 marco      (502) staff       (20)      597 2024-05-11 18:48:50.000000 musicntwrk-2.3.7/src/msctools/cfg.py
+-rw-r--r--   0 marco      (502) staff       (20)     2248 2023-09-08 07:15:36.000000 musicntwrk-2.3.7/src/msctools/converters.py
+-rw-r--r--   0 marco      (502) staff       (20)      336 2024-01-30 00:27:07.000000 musicntwrk-2.3.7/src/msctools/decorators.py
+-rw-r--r--   0 marco      (502) staff       (20)     7080 2024-05-02 20:15:38.000000 musicntwrk-2.3.7/src/msctools/devices.py
+-rw-r--r--   0 marco      (502) staff       (20)    78504 2024-01-20 15:29:09.000000 musicntwrk-2.3.7/src/msctools/dictionaries.py
+-rw-r--r--   0 marco      (502) staff       (20)    48647 2023-11-09 23:14:46.000000 musicntwrk-2.3.7/src/msctools/dsp.py
+-rw-r--r--   0 marco      (502) staff       (20)     5951 2024-05-02 20:33:09.000000 musicntwrk-2.3.7/src/msctools/envelopes.py
+-rw-r--r--   0 marco      (502) staff       (20)     8785 2024-05-17 14:38:55.000000 musicntwrk-2.3.7/src/msctools/envelopes_thread.py
+-rw-r--r--   0 marco      (502) staff       (20)    19624 2024-04-20 12:45:11.000000 musicntwrk-2.3.7/src/msctools/networks.py
+-rw-r--r--   0 marco      (502) staff       (20)      865 2023-04-13 16:06:16.000000 musicntwrk-2.3.7/src/msctools/oscserver.py
+-rw-r--r--   0 marco      (502) staff       (20)     2119 2024-05-11 15:37:48.000000 musicntwrk-2.3.7/src/msctools/osctools.py
+-rw-r--r--   0 marco      (502) staff       (20)      472 2022-11-22 00:46:09.000000 musicntwrk-2.3.7/src/msctools/pan.py
+-rw-r--r--   0 marco      (502) staff       (20)     4826 2024-05-02 20:19:05.000000 musicntwrk-2.3.7/src/msctools/players.py
+-rw-r--r--   0 marco      (502) staff       (20)     8801 2024-05-17 14:50:52.000000 musicntwrk-2.3.7/src/msctools/players_thread.py
+-rw-r--r--   0 marco      (502) staff       (20)     1648 2024-05-02 20:19:16.000000 musicntwrk-2.3.7/src/msctools/pyoPlayer.py
+-rw-r--r--   0 marco      (502) staff       (20)    17002 2024-04-20 13:03:26.000000 musicntwrk-2.3.7/src/msctools/pyotools.py
+-rw-r--r--   0 marco      (502) staff       (20)     1374 2024-05-02 20:19:32.000000 musicntwrk-2.3.7/src/msctools/session.py
+-rw-r--r--   0 marco      (502) staff       (20)      680 2024-05-05 22:00:38.000000 musicntwrk-2.3.7/src/msctools/utils.py
+-rw-r--r--   0 marco      (502) staff       (20)     5386 2023-04-13 16:05:54.000000 musicntwrk-2.3.7/src/msctools/videocapture.py
+-rw-r--r--   0 marco      (502) staff       (20)    68822 2024-01-26 02:18:22.000000 musicntwrk-2.3.7/src/musicntwrk.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-29 21:35:28.306362 musicntwrk-2.3.7/src/networks/
+-rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/networks/__init__.py
+-rw-r--r--   0 marco      (502) staff       (20)     2580 2023-08-02 08:22:01.000000 musicntwrk-2.3.7/src/networks/analysisNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     2646 2023-08-02 08:22:01.000000 musicntwrk-2.3.7/src/networks/orchestralNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     2388 2023-04-04 23:24:43.000000 musicntwrk-2.3.7/src/networks/orchestralVector.py
+-rw-r--r--   0 marco      (502) staff       (20)     1695 2024-04-24 21:12:18.000000 musicntwrk-2.3.7/src/networks/orchestralVectorColor.py
+-rw-r--r--   0 marco      (502) staff       (20)     4853 2024-04-24 15:27:50.000000 musicntwrk-2.3.7/src/networks/pcsDictionary.py
+-rw-r--r--   0 marco      (502) staff       (20)     5852 2023-08-02 08:22:01.000000 musicntwrk-2.3.7/src/networks/pcsEgoNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     4914 2023-08-02 08:22:01.000000 musicntwrk-2.3.7/src/networks/pcsNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     2966 2023-08-02 08:22:01.000000 musicntwrk-2.3.7/src/networks/rLeadNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     2470 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/networks/readScore.py
+-rw-r--r--   0 marco      (502) staff       (20)     3085 2022-01-09 00:40:38.000000 musicntwrk-2.3.7/src/networks/rhythmDictionary.py
+-rw-r--r--   0 marco      (502) staff       (20)     4322 2023-08-02 08:22:01.000000 musicntwrk-2.3.7/src/networks/rhythmNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     4053 2023-12-28 02:35:13.000000 musicntwrk-2.3.7/src/networks/rhythmPDictionary.py
+-rw-r--r--   0 marco      (502) staff       (20)     2456 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/networks/scoreDictionary.py
+-rw-r--r--   0 marco      (502) staff       (20)     1592 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/networks/scoreMIDIDictionary.py
+-rw-r--r--   0 marco      (502) staff       (20)     5809 2023-08-02 08:22:01.000000 musicntwrk-2.3.7/src/networks/scoreNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     5791 2023-08-02 08:22:01.000000 musicntwrk-2.3.7/src/networks/scoreSubNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     3697 2023-08-02 08:22:01.000000 musicntwrk-2.3.7/src/networks/timbralNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     4102 2023-08-02 08:22:01.000000 musicntwrk-2.3.7/src/networks/vLeadNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     4789 2023-08-02 08:22:01.000000 musicntwrk-2.3.7/src/networks/vLeadNetworkByName.py
+-rw-r--r--   0 marco      (502) staff       (20)     2936 2023-08-02 08:22:01.000000 musicntwrk-2.3.7/src/networks/vLeadNetworkByNameVec.py
+-rw-r--r--   0 marco      (502) staff       (20)     2634 2023-08-02 08:22:01.000000 musicntwrk-2.3.7/src/networks/vLeadNetworkVec.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-29 21:35:28.308165 musicntwrk-2.3.7/src/plotting/
+-rw-r--r--   0 marco      (502) staff       (20)     1066 2024-04-24 14:49:13.000000 musicntwrk-2.3.7/src/plotting/barplot.py
+-rw-r--r--   0 marco      (502) staff       (20)    24919 2023-12-21 02:30:18.000000 musicntwrk-2.3.7/src/plotting/chordspace.py
+-rw-r--r--   0 marco      (502) staff       (20)     7250 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/plotting/drawMultiLayerNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     2888 2023-07-05 22:49:56.000000 musicntwrk-2.3.7/src/plotting/drawNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     6340 2023-08-02 09:17:49.000000 musicntwrk-2.3.7/src/plotting/drawNetwork3D.py
+-rw-r--r--   0 marco      (502) staff       (20)     2256 2021-11-23 20:31:22.000000 musicntwrk-2.3.7/src/plotting/drawNetworkViz.py
+-rw-r--r--   0 marco      (502) staff       (20)     1246 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/plotting/drawNetworkX.py
+-rw-r--r--   0 marco      (502) staff       (20)      895 2024-04-24 14:49:25.000000 musicntwrk-2.3.7/src/plotting/plotCC.py
+-rw-r--r--   0 marco      (502) staff       (20)      716 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/plotting/plotCurveXY.py
+-rw-r--r--   0 marco      (502) staff       (20)      711 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/plotting/plotCurveY.py
+-rw-r--r--   0 marco      (502) staff       (20)     1680 2023-08-02 14:25:53.000000 musicntwrk-2.3.7/src/plotting/plotDegreeAnalysis.py
+-rw-r--r--   0 marco      (502) staff       (20)     1869 2024-04-24 14:50:13.000000 musicntwrk-2.3.7/src/plotting/plotOpsHistogram.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-29 21:35:28.310145 musicntwrk-2.3.7/src/timbre/
+-rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/timbre/__init__.py
+-rw-r--r--   0 marco      (502) staff       (20)     1743 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/timbre/computeASCBW.py
+-rw-r--r--   0 marco      (502) staff       (20)     1552 2023-04-04 23:13:40.000000 musicntwrk-2.3.7/src/timbre/computeCompMPS.py
+-rw-r--r--   0 marco      (502) staff       (20)     1663 2023-04-04 23:14:32.000000 musicntwrk-2.3.7/src/timbre/computeMFCC.py
+-rw-r--r--   0 marco      (502) staff       (20)     2653 2024-04-24 14:50:05.000000 musicntwrk-2.3.7/src/timbre/computeModifiedASCBW.py
+-rw-r--r--   0 marco      (502) staff       (20)     1475 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/timbre/computePSCC.py
+-rw-r--r--   0 marco      (502) staff       (20)     2263 2023-06-23 21:10:40.000000 musicntwrk-2.3.7/src/timbre/computeStandardizedMFCC.py
+-rw-r--r--   0 marco      (502) staff       (20)     1769 2022-10-29 00:30:08.000000 musicntwrk-2.3.7/src/timbre/computeStandardizedMFPS.py
+-rw-r--r--   0 marco      (502) staff       (20)     1926 2022-10-29 00:29:28.000000 musicntwrk-2.3.7/src/timbre/computeStandardizedPSCC.py
+-rw-r--r--   0 marco      (502) staff       (20)     1194 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/timbre/mfccSoundDecay.py
+-rw-r--r--   0 marco      (502) staff       (20)      848 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/timbre/mfccSoundDecayOptimal.py
+-rw-r--r--   0 marco      (502) staff       (20)     1395 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/timbre/mfccSoundDecayPiecewise.py
+-rw-r--r--   0 marco      (502) staff       (20)     2092 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/timbre/minimizeBKPT.py
+-rw-r--r--   0 marco      (502) staff       (20)      974 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/timbre/normSoundDecay.py
+-rw-r--r--   0 marco      (502) staff       (20)     1342 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/timbre/normSoundDecay2.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-29 21:35:28.315065 musicntwrk-2.3.7/src/utils/
+-rw-r--r--   0 marco      (502) staff       (20)     1142 2023-05-25 21:57:17.000000 musicntwrk-2.3.7/src/utils/Remove.py
+-rw-r--r--   0 marco      (502) staff       (20)     1962 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/utils/SegmentedLinearReg.py
+-rw-r--r--   0 marco      (502) staff       (20)      884 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/utils/Sublists.py
+-rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/utils/__init__.py
+-rw-r--r--   0 marco      (502) staff       (20)     3121 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/utils/communications.py
+-rw-r--r--   0 marco      (502) staff       (20)     9768 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/utils/diffusionEntropyAnalyis.py
+-rw-r--r--   0 marco      (502) staff       (20)     5511 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/utils/diffusionEntropyAnalyisNew.py
+-rw-r--r--   0 marco      (502) staff       (20)     1758 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/utils/entropyKLdiv.py
+-rw-r--r--   0 marco      (502) staff       (20)     1005 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/utils/extractByString.py
+-rw-r--r--   0 marco      (502) staff       (20)      830 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/utils/fetchWaves.py
+-rw-r--r--   0 marco      (502) staff       (20)     1086 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/utils/findLengthMax.py
+-rw-r--r--   0 marco      (502) staff       (20)      883 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/utils/flatten.py
+-rw-r--r--   0 marco      (502) staff       (20)      591 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/utils/floatize.py
+-rw-r--r--   0 marco      (502) staff       (20)     1669 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/utils/generalizedOpsHistogram.py
+-rw-r--r--   0 marco      (502) staff       (20)     1541 2022-06-24 15:34:43.000000 musicntwrk-2.3.7/src/utils/generalizedOpsName.py
+-rw-r--r--   0 marco      (502) staff       (20)      760 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/utils/init_list_of_objects.py
+-rw-r--r--   0 marco      (502) staff       (20)     1700 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/utils/load_balancing.py
+-rw-r--r--   0 marco      (502) staff       (20)     1398 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/utils/minimalDistance.py
+-rw-r--r--   0 marco      (502) staff       (20)     1297 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/utils/minimalDistanceVec.py
+-rw-r--r--   0 marco      (502) staff       (20)     1401 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/utils/minimalNoBijDistance.py
+-rw-r--r--   0 marco      (502) staff       (20)     1053 2021-11-19 16:54:18.000000 musicntwrk-2.3.7/src/utils/opsCheckByName.py
+-rw-r--r--   0 marco      (502) staff       (20)      827 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/utils/opsCheckByNameVec.py
+-rw-r--r--   0 marco      (502) staff       (20)      878 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/utils/opsDistance.py
+-rw-r--r--   0 marco      (502) staff       (20)     1653 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/utils/opsHistogram.py
+-rw-r--r--   0 marco      (502) staff       (20)     1537 2021-11-12 22:37:18.000000 musicntwrk-2.3.7/src/utils/opsName.py
+-rw-r--r--   0 marco      (502) staff       (20)     2413 2021-11-19 01:35:52.000000 musicntwrk-2.3.7/src/utils/opsNameFull.py
+-rw-r--r--   0 marco      (502) staff       (20)     1638 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/utils/opsNameVec.py
+-rw-r--r--   0 marco      (502) staff       (20)      721 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/utils/play_with_simpleaudio.py
+-rw-r--r--   0 marco      (502) staff       (20)     4681 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/utils/powerFit.py
+-rw-r--r--   0 marco      (502) staff       (20)     1384 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/utils/rhythmDistance.py
+-rw-r--r--   0 marco      (502) staff       (20)     2605 2021-08-06 01:36:29.000000 musicntwrk-2.3.7/src/utils/scaleFreeFit.py
+-rw-r--r--   0 marco      (502) staff       (20)     1130 2021-11-22 17:37:40.000000 musicntwrk-2.3.7/src/utils/score2vLead.py
+-rw-r--r--   0 marco      (502) staff       (20)      730 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/utils/str2float.py
+-rw-r--r--   0 marco      (502) staff       (20)      702 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/utils/str2frac.py
+-rw-r--r--   0 marco      (502) staff       (20)      963 2021-06-25 20:55:30.000000 musicntwrk-2.3.7/src/utils/vectorDistance.py
```

### Comparing `musicntwrk-2.3.6/PKG-INFO` & `musicntwrk-2.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicntwrk
-Version: 2.3.6
+Version: 2.3.7
 Summary: music as data, data as music
 Home-page: https://www.musicntwrk.com
 Author: Marco Buongiorno Nardelli
 Author-email: mbn@unt.edu
 Platform: OS independent
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: musicntwrk Version: 2.3.6 Summary: music as data,
+Metadata-Version: 2.1 Name: musicntwrk Version: 2.3.7 Summary: music as data,
 data as music Home-page: https://www.musicntwrk.com Author: Marco Buongiorno
 Nardelli Author-email: mbn@unt.edu Platform: OS independent Description-
 Content-Type: text/markdown Requires-Dist: numpy Requires-Dist: scipy Requires-
 Dist: pandas Requires-Dist: python-louvain Requires-Dist: networkx Requires-
 Dist: music21 Requires-Dist: librosa Requires-Dist: numba Requires-Dist: pyo
 Requires-Dist: matplotlib Requires-Dist: tensorflow Requires-Dist: powerlaw
 Requires-Dist: vpython Requires-Dist: wget Requires-Dist: PySimpleGUI Requires-
```

### Comparing `musicntwrk-2.3.6/README.md` & `musicntwrk-2.3.7/README.md`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/musicntwrk.egg-info/PKG-INFO` & `musicntwrk-2.3.7/musicntwrk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicntwrk
-Version: 2.3.6
+Version: 2.3.7
 Summary: music as data, data as music
 Home-page: https://www.musicntwrk.com
 Author: Marco Buongiorno Nardelli
 Author-email: mbn@unt.edu
 Platform: OS independent
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: musicntwrk Version: 2.3.6 Summary: music as data,
+Metadata-Version: 2.1 Name: musicntwrk Version: 2.3.7 Summary: music as data,
 data as music Home-page: https://www.musicntwrk.com Author: Marco Buongiorno
 Nardelli Author-email: mbn@unt.edu Platform: OS independent Description-
 Content-Type: text/markdown Requires-Dist: numpy Requires-Dist: scipy Requires-
 Dist: pandas Requires-Dist: python-louvain Requires-Dist: networkx Requires-
 Dist: music21 Requires-Dist: librosa Requires-Dist: numba Requires-Dist: pyo
 Requires-Dist: matplotlib Requires-Dist: tensorflow Requires-Dist: powerlaw
 Requires-Dist: vpython Requires-Dist: wget Requires-Dist: PySimpleGUI Requires-
```

### Comparing `musicntwrk-2.3.6/musicntwrk.egg-info/SOURCES.txt` & `musicntwrk-2.3.7/musicntwrk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/setup.py` & `musicntwrk-2.3.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
 with open(path.join(this_directory, 'README.md')) as f:
 	long_description = f.read()
 
 
 setup(name='musicntwrk',
 
-	version='2.3.6',
+	version='2.3.7',
 
 	description='music as data, data as music',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	author='Marco Buongiorno Nardelli',
 	author_email='mbn@unt.edu',
 	platforms='OS independent',
```

### Comparing `musicntwrk-2.3.6/src/comptools/MidiFile.py` & `musicntwrk-2.3.7/src/comptools/MidiFile.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/comptools/displayNotes.py` & `musicntwrk-2.3.7/src/comptools/displayNotes.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/comptools/genmidi.py` & `musicntwrk-2.3.7/src/comptools/genmidi.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/comptools/music.py` & `musicntwrk-2.3.7/src/comptools/music.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/comptools/notation.py` & `musicntwrk-2.3.7/src/comptools/notation.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/data/MIDImap.py` & `musicntwrk-2.3.7/src/data/MIDImap.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/data/MIDImidi.py` & `musicntwrk-2.3.7/src/data/MIDImidi.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/data/MIDIscore.py` & `musicntwrk-2.3.7/src/data/MIDIscore.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/data/WRITEscore.py` & `musicntwrk-2.3.7/src/data/WRITEscore.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/data/WRITEscoreNoTime.py` & `musicntwrk-2.3.7/src/data/WRITEscoreNoTime.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/data/WRITEscoreOps.py` & `musicntwrk-2.3.7/src/data/WRITEscoreOps.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/data/WRITEscoreOpsMIDI.py` & `musicntwrk-2.3.7/src/data/WRITEscoreOpsMIDI.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/data/analyzeSound.py` & `musicntwrk-2.3.7/src/data/analyzeSound.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/data/analyzeTimbre.py` & `musicntwrk-2.3.7/src/data/analyzeTimbre.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/data/ctcsound.py` & `musicntwrk-2.3.7/src/data/ctcsound.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/data/i_spectral.py` & `musicntwrk-2.3.7/src/data/i_spectral.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/data/i_spectral2.py` & `musicntwrk-2.3.7/src/data/i_spectral2.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/data/i_spectral_pure.py` & `musicntwrk-2.3.7/src/data/i_spectral_pure.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/data/i_spectral_pyo.py` & `musicntwrk-2.3.7/src/data/i_spectral_pyo.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/data/i_time_series.py` & `musicntwrk-2.3.7/src/data/i_time_series.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/data/r_1Ddata.py` & `musicntwrk-2.3.7/src/data/r_1Ddata.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/data/scaleMapping.py` & `musicntwrk-2.3.7/src/data/scaleMapping.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/harmony/applyOps.py` & `musicntwrk-2.3.7/src/harmony/applyOps.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/harmony/changePoint.py` & `musicntwrk-2.3.7/src/harmony/changePoint.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/harmony/chinese_postman.py` & `musicntwrk-2.3.7/src/harmony/chinese_postman.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/harmony/enharmonicDictionary.py` & `musicntwrk-2.3.7/src/harmony/enharmonicDictionary.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/harmony/getRN.py` & `musicntwrk-2.3.7/src/harmony/getRN.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/harmony/harmonicDesign.py` & `musicntwrk-2.3.7/src/harmony/harmonicDesign.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/harmony/keySections.py` & `musicntwrk-2.3.7/src/harmony/keySections.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/harmony/lookupOps.py` & `musicntwrk-2.3.7/src/harmony/lookupOps.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/harmony/lookupProgr.py` & `musicntwrk-2.3.7/src/harmony/lookupProgr.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/harmony/lookupWrapper.py` & `musicntwrk-2.3.7/src/harmony/lookupWrapper.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/harmony/networkHarmonyGen.py` & `musicntwrk-2.3.7/src/harmony/networkHarmonyGen.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/harmony/plotHarmonicTable.py` & `musicntwrk-2.3.7/src/harmony/plotHarmonicTable.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/harmony/rhythmicDesign.py` & `musicntwrk-2.3.7/src/harmony/rhythmicDesign.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/harmony/scoreAnalysis.py` & `musicntwrk-2.3.7/src/harmony/scoreAnalysis.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/harmony/scoreDesign.py` & `musicntwrk-2.3.7/src/harmony/scoreDesign.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/harmony/scoreFilter.py` & `musicntwrk-2.3.7/src/harmony/scoreFilter.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/harmony/shortHands.py` & `musicntwrk-2.3.7/src/harmony/shortHands.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/harmony/showAnalysis.py` & `musicntwrk-2.3.7/src/harmony/showAnalysis.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/harmony/spiralChordSpace.py` & `musicntwrk-2.3.7/src/harmony/spiralChordSpace.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/harmony/tonalAnalysis.py` & `musicntwrk-2.3.7/src/harmony/tonalAnalysis.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/harmony/tonalHarmonyCalculator.py` & `musicntwrk-2.3.7/src/harmony/tonalHarmonyCalculator.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/harmony/tonalHarmonyModels.py` & `musicntwrk-2.3.7/src/harmony/tonalHarmonyModels.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/harmony/tonalPartition.py` & `musicntwrk-2.3.7/src/harmony/tonalPartition.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/harmony/tonnentz.py` & `musicntwrk-2.3.7/src/harmony/tonnentz.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/ml_utils/checkRun.py` & `musicntwrk-2.3.7/src/ml_utils/checkRun.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/ml_utils/modelDump.py` & `musicntwrk-2.3.7/src/ml_utils/modelDump.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/ml_utils/modelLoad.py` & `musicntwrk-2.3.7/src/ml_utils/modelLoad.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/ml_utils/multiModelPredictor.py` & `musicntwrk-2.3.7/src/ml_utils/multiModelPredictor.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/ml_utils/prepareDataSet.py` & `musicntwrk-2.3.7/src/ml_utils/prepareDataSet.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/ml_utils/readModels.py` & `musicntwrk-2.3.7/src/ml_utils/readModels.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/ml_utils/scaleDataSet.py` & `musicntwrk-2.3.7/src/ml_utils/scaleDataSet.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/ml_utils/trainCNNmodel.py` & `musicntwrk-2.3.7/src/ml_utils/trainCNNmodel.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/ml_utils/trainNNmodel.py` & `musicntwrk-2.3.7/src/ml_utils/trainNNmodel.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/msctools/base.py` & `musicntwrk-2.3.7/src/msctools/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,26 +188,43 @@
 			client("/live/clip/set/warping",[self.n,self.c,1],self.host,self.port).send()
 			
 	def dur(self):
 		client("/live/clip/get/file_path",[self.n,self.c],self.host,self.port).send()
 		time.sleep(cfg.TICK)
 		fil = cfg.data[2]
 		sr, wav = wavfile.read(fil)
-		nsamples = wav.size/wav.shape[1]
+		try:
+			nsamples = wav.size/wav.shape[1]
+		except:
+			nsamples = wav.size
 		return(nsamples/sr)
 
+	def length(self):
+		client("/live/clip/get/length",[self.n,self.c],self.host,self.port).send()
+		time.sleep(cfg.TICK)
+		return(cfg.data[2])
+
+
 	def gain(self,gain=db2value(0.0),mode='set'):
 		if mode == 'setdb':
 			client("/live/clip/set/gain",[self.n,self.c,db4value(gain)],self.host,self.port).send()
 		if mode == 'set':
 			client("/live/clip/set/gain",[self.n,self.c,gain],self.host,self.port).send()
 		if mode == 'get':
 			client("/live/clip/get/gain",[self.n,self.c],self.host,self.port).send()
 			time.sleep(cfg.TICK)
 			return(value2db(cfg.data[1]))
+
+	def pitch(self,pitch=0,mode='set'):
+		if mode == 'set':
+			client("/live/clip/set/pitch_coarse",[self.n,self.c,pitch],self.host,self.port).send()
+		if mode == 'get':
+			client("/live/clip/get/pitch_coarse",[self.n,self.c],self.host,self.port).send()
+			time.sleep(cfg.TICK)
+			return(cfg.data[1])
 	
 class ClipSlot:
 	
 	def __init__(self,track,clip_slot,controls=None,host=cfg.HOST,port=cfg.PORT):
 		self.n = track
 		self.c = clip_slot
 		self.port = port
```

### Comparing `musicntwrk-2.3.6/src/msctools/cfg.py` & `musicntwrk-2.3.7/src/msctools/cfg.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/msctools/converters.py` & `musicntwrk-2.3.7/src/msctools/converters.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/msctools/devices.py` & `musicntwrk-2.3.7/src/msctools/devices.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/msctools/dictionaries.py` & `musicntwrk-2.3.7/src/msctools/dictionaries.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/msctools/dsp.py` & `musicntwrk-2.3.7/src/msctools/dsp.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/msctools/envelopes.py` & `musicntwrk-2.3.7/src/msctools/envelopes.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/msctools/envelopes_thread.py` & `musicntwrk-2.3.7/src/msctools/envelopes_thread.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/msctools/networks.py` & `musicntwrk-2.3.7/src/msctools/networks.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/msctools/oscserver.py` & `musicntwrk-2.3.7/src/msctools/oscserver.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/msctools/osctools.py` & `musicntwrk-2.3.7/src/msctools/osctools.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/msctools/players.py` & `musicntwrk-2.3.7/src/msctools/players.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/msctools/players_thread.py` & `musicntwrk-2.3.7/src/msctools/players_thread.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/msctools/pyoPlayer.py` & `musicntwrk-2.3.7/src/msctools/pyoPlayer.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/msctools/pyotools.py` & `musicntwrk-2.3.7/src/msctools/pyotools.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/msctools/session.py` & `musicntwrk-2.3.7/src/msctools/session.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/msctools/utils.py` & `musicntwrk-2.3.7/src/msctools/utils.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/msctools/videocapture.py` & `musicntwrk-2.3.7/src/msctools/videocapture.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/musicntwrk.py` & `musicntwrk-2.3.7/src/musicntwrk.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/networks/analysisNetwork.py` & `musicntwrk-2.3.7/src/networks/analysisNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/networks/orchestralNetwork.py` & `musicntwrk-2.3.7/src/networks/orchestralNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/networks/orchestralVector.py` & `musicntwrk-2.3.7/src/networks/orchestralVector.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/networks/orchestralVectorColor.py` & `musicntwrk-2.3.7/src/networks/orchestralVectorColor.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/networks/pcsDictionary.py` & `musicntwrk-2.3.7/src/networks/pcsDictionary.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/networks/pcsEgoNetwork.py` & `musicntwrk-2.3.7/src/networks/pcsEgoNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/networks/pcsNetwork.py` & `musicntwrk-2.3.7/src/networks/pcsNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/networks/rLeadNetwork.py` & `musicntwrk-2.3.7/src/networks/rLeadNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/networks/readScore.py` & `musicntwrk-2.3.7/src/networks/readScore.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/networks/rhythmDictionary.py` & `musicntwrk-2.3.7/src/networks/rhythmDictionary.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/networks/rhythmNetwork.py` & `musicntwrk-2.3.7/src/networks/rhythmNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/networks/rhythmPDictionary.py` & `musicntwrk-2.3.7/src/networks/rhythmPDictionary.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/networks/scoreDictionary.py` & `musicntwrk-2.3.7/src/networks/scoreDictionary.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/networks/scoreMIDIDictionary.py` & `musicntwrk-2.3.7/src/networks/scoreMIDIDictionary.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/networks/scoreNetwork.py` & `musicntwrk-2.3.7/src/networks/scoreNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/networks/scoreSubNetwork.py` & `musicntwrk-2.3.7/src/networks/scoreSubNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/networks/timbralNetwork.py` & `musicntwrk-2.3.7/src/networks/timbralNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/networks/vLeadNetwork.py` & `musicntwrk-2.3.7/src/networks/vLeadNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/networks/vLeadNetworkByName.py` & `musicntwrk-2.3.7/src/networks/vLeadNetworkByName.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/networks/vLeadNetworkByNameVec.py` & `musicntwrk-2.3.7/src/networks/vLeadNetworkByNameVec.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/networks/vLeadNetworkVec.py` & `musicntwrk-2.3.7/src/networks/vLeadNetworkVec.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/plotting/barplot.py` & `musicntwrk-2.3.7/src/plotting/barplot.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/plotting/chordspace.py` & `musicntwrk-2.3.7/src/plotting/chordspace.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/plotting/drawMultiLayerNetwork.py` & `musicntwrk-2.3.7/src/plotting/drawMultiLayerNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/plotting/drawNetwork.py` & `musicntwrk-2.3.7/src/plotting/drawNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/plotting/drawNetwork3D.py` & `musicntwrk-2.3.7/src/plotting/drawNetwork3D.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/plotting/drawNetworkViz.py` & `musicntwrk-2.3.7/src/plotting/drawNetworkViz.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/plotting/drawNetworkX.py` & `musicntwrk-2.3.7/src/plotting/drawNetworkX.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/plotting/plotCC.py` & `musicntwrk-2.3.7/src/plotting/plotCC.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/plotting/plotCurveXY.py` & `musicntwrk-2.3.7/src/plotting/plotCurveXY.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/plotting/plotCurveY.py` & `musicntwrk-2.3.7/src/plotting/plotCurveY.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/plotting/plotDegreeAnalysis.py` & `musicntwrk-2.3.7/src/plotting/plotDegreeAnalysis.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/plotting/plotOpsHistogram.py` & `musicntwrk-2.3.7/src/plotting/plotOpsHistogram.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/timbre/computeASCBW.py` & `musicntwrk-2.3.7/src/timbre/computeASCBW.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/timbre/computeCompMPS.py` & `musicntwrk-2.3.7/src/timbre/computeCompMPS.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/timbre/computeMFCC.py` & `musicntwrk-2.3.7/src/timbre/computeMFCC.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/timbre/computeModifiedASCBW.py` & `musicntwrk-2.3.7/src/timbre/computeModifiedASCBW.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/timbre/computePSCC.py` & `musicntwrk-2.3.7/src/timbre/computePSCC.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/timbre/computeStandardizedMFCC.py` & `musicntwrk-2.3.7/src/timbre/computeStandardizedMFCC.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/timbre/computeStandardizedMFPS.py` & `musicntwrk-2.3.7/src/timbre/computeStandardizedMFPS.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/timbre/computeStandardizedPSCC.py` & `musicntwrk-2.3.7/src/timbre/computeStandardizedPSCC.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/timbre/mfccSoundDecay.py` & `musicntwrk-2.3.7/src/timbre/mfccSoundDecay.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/timbre/mfccSoundDecayOptimal.py` & `musicntwrk-2.3.7/src/timbre/mfccSoundDecayOptimal.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/timbre/mfccSoundDecayPiecewise.py` & `musicntwrk-2.3.7/src/timbre/mfccSoundDecayPiecewise.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/timbre/minimizeBKPT.py` & `musicntwrk-2.3.7/src/timbre/minimizeBKPT.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/timbre/normSoundDecay.py` & `musicntwrk-2.3.7/src/timbre/normSoundDecay.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/timbre/normSoundDecay2.py` & `musicntwrk-2.3.7/src/timbre/normSoundDecay2.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/Remove.py` & `musicntwrk-2.3.7/src/utils/Remove.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/SegmentedLinearReg.py` & `musicntwrk-2.3.7/src/utils/SegmentedLinearReg.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/Sublists.py` & `musicntwrk-2.3.7/src/utils/Sublists.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/communications.py` & `musicntwrk-2.3.7/src/utils/communications.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/diffusionEntropyAnalyis.py` & `musicntwrk-2.3.7/src/utils/diffusionEntropyAnalyis.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/diffusionEntropyAnalyisNew.py` & `musicntwrk-2.3.7/src/utils/diffusionEntropyAnalyisNew.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/entropyKLdiv.py` & `musicntwrk-2.3.7/src/utils/entropyKLdiv.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/extractByString.py` & `musicntwrk-2.3.7/src/utils/extractByString.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/fetchWaves.py` & `musicntwrk-2.3.7/src/utils/fetchWaves.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/findLengthMax.py` & `musicntwrk-2.3.7/src/utils/findLengthMax.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/flatten.py` & `musicntwrk-2.3.7/src/utils/flatten.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/floatize.py` & `musicntwrk-2.3.7/src/utils/floatize.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/generalizedOpsHistogram.py` & `musicntwrk-2.3.7/src/utils/generalizedOpsHistogram.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/generalizedOpsName.py` & `musicntwrk-2.3.7/src/utils/generalizedOpsName.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/init_list_of_objects.py` & `musicntwrk-2.3.7/src/utils/init_list_of_objects.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/load_balancing.py` & `musicntwrk-2.3.7/src/utils/load_balancing.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/minimalDistance.py` & `musicntwrk-2.3.7/src/utils/minimalDistance.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/minimalDistanceVec.py` & `musicntwrk-2.3.7/src/utils/minimalDistanceVec.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/minimalNoBijDistance.py` & `musicntwrk-2.3.7/src/utils/minimalNoBijDistance.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/opsCheckByName.py` & `musicntwrk-2.3.7/src/utils/opsCheckByName.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/opsCheckByNameVec.py` & `musicntwrk-2.3.7/src/utils/opsCheckByNameVec.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/opsDistance.py` & `musicntwrk-2.3.7/src/utils/opsDistance.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/opsHistogram.py` & `musicntwrk-2.3.7/src/utils/opsHistogram.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/opsName.py` & `musicntwrk-2.3.7/src/utils/opsName.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/opsNameFull.py` & `musicntwrk-2.3.7/src/utils/opsNameFull.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/opsNameVec.py` & `musicntwrk-2.3.7/src/utils/opsNameVec.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/play_with_simpleaudio.py` & `musicntwrk-2.3.7/src/utils/play_with_simpleaudio.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/powerFit.py` & `musicntwrk-2.3.7/src/utils/powerFit.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/rhythmDistance.py` & `musicntwrk-2.3.7/src/utils/rhythmDistance.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/scaleFreeFit.py` & `musicntwrk-2.3.7/src/utils/scaleFreeFit.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/score2vLead.py` & `musicntwrk-2.3.7/src/utils/score2vLead.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/str2float.py` & `musicntwrk-2.3.7/src/utils/str2float.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/str2frac.py` & `musicntwrk-2.3.7/src/utils/str2frac.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.6/src/utils/vectorDistance.py` & `musicntwrk-2.3.7/src/utils/vectorDistance.py`

 * *Files identical despite different names*

