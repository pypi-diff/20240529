# Comparing `tmp/canlib-1.25.393.tar.gz` & `tmp/canlib-1.26.487.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\build\Data\240218~2\pycanlib\DEFAUL~2\src\dist\.tmp-9ldunt6r\canlib-1.25.393.tar", last modified: Sun Feb 18 20:34:48 2024, max compression
+gzip compressed data, was "D:\build\Data\240522~2\pycanlib\DEFAUL~2\src\dist\.tmp-w0g8aavn\canlib-1.26.487.tar", last modified: Wed May 22 19:55:17 2024, max compression
```

## Comparing `canlib-1.25.393.tar` & `canlib-1.26.487.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxrwxrwx   0        0        0        0 2024-02-18 20:34:48.000000 canlib-1.25.393/
--rw-rw-rw-   0        0        0     1068 2024-02-18 20:32:40.000000 canlib-1.25.393/LICENSE
--rw-rw-rw-   0        0        0       59 2024-02-18 20:32:40.000000 canlib-1.25.393/MANIFEST.in
--rw-rw-rw-   0        0        0     7536 2024-02-18 20:34:48.000000 canlib-1.25.393/PKG-INFO
--rw-rw-rw-   0        0        0     6792 2024-02-18 20:32:40.000000 canlib-1.25.393/README.rst
--rw-rw-rw-   0        0        0    25831 2024-02-18 20:32:42.000000 canlib-1.25.393/Relnotes.rst
-drwxrwxrwx   0        0        0        0 2024-02-18 20:34:48.000000 canlib-1.25.393/canlib/
--rw-rw-rw-   0        0        0      385 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/__about__.py
--rw-rw-rw-   0        0        0      221 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/__init__.py
--rw-rw-rw-   0        0        0       26 2024-02-18 20:32:42.000000 canlib-1.25.393/canlib/__version__.py
-drwxrwxrwx   0        0        0        0 2024-02-18 20:34:48.000000 canlib-1.25.393/canlib/canlib/
--rw-rw-rw-   0        0        0     2477 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/canlib/__init__.py
--rw-rw-rw-   0        0        0      725 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/canlib/_channel.py
--rw-rw-rw-   0        0        0    22718 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/canlib/busparams.py
--rw-rw-rw-   0        0        0    60559 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/canlib/channel.py
--rw-rw-rw-   0        0        0    18151 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/canlib/channeldata.py
--rw-rw-rw-   0        0        0    10771 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/canlib/constants.py
--rw-rw-rw-   0        0        0     9455 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/canlib/dll.py
--rw-rw-rw-   0        0        0    30453 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/canlib/enums.py
--rw-rw-rw-   0        0        0     6531 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/canlib/envvar.py
--rw-rw-rw-   0        0        0     5906 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/canlib/exceptions.py
--rw-rw-rw-   0        0        0    15796 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/canlib/iocontrol.py
--rw-rw-rw-   0        0        0    22000 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/canlib/iopin.py
--rw-rw-rw-   0        0        0     6796 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/canlib/objbuf.py
--rw-rw-rw-   0        0        0     3305 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/canlib/structures.py
--rw-rw-rw-   0        0        0     2935 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/canlib/timedomain.py
--rw-rw-rw-   0        0        0     4932 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/canlib/txe.py
--rw-rw-rw-   0        0        0    15687 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/canlib/wrapper.py
--rw-rw-rw-   0        0        0      360 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/cenum.py
--rw-rw-rw-   0        0        0     7805 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/deprecation.py
--rw-rw-rw-   0        0        0    16036 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/device.py
--rw-rw-rw-   0        0        0     8974 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/dllLoader.py
--rw-rw-rw-   0        0        0     7583 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/ean.py
--rw-rw-rw-   0        0        0      760 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/exceptions.py
--rw-rw-rw-   0        0        0     4003 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/frame.py
--rw-rw-rw-   0        0        0     8738 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/futureapi.py
--rw-rw-rw-   0        0        0     5226 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/j1939.py
--rw-rw-rw-   0        0        0    12275 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvDevice.py
--rw-rw-rw-   0        0        0    25506 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvMemoConfig.py
--rw-rw-rw-   0        0        0      115 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvMessage.py
--rw-rw-rw-   0        0        0      247 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvaMemoLibXml.py
-drwxrwxrwx   0        0        0        0 2024-02-18 20:34:48.000000 canlib-1.25.393/canlib/kvadblib/
--rw-rw-rw-   0        0        0     1517 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvadblib/__init__.py
--rw-rw-rw-   0        0        0     3498 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvadblib/attribute.py
--rw-rw-rw-   0        0        0     8276 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvadblib/attributedef.py
--rw-rw-rw-   0        0        0     1189 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvadblib/bound_message.py
--rw-rw-rw-   0        0        0     2099 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvadblib/bound_signal.py
--rw-rw-rw-   0        0        0       11 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvadblib/constants.py
--rw-rw-rw-   0        0        0    18943 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvadblib/dbc.py
--rw-rw-rw-   0        0        0    11330 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvadblib/dll.py
--rw-rw-rw-   0        0        0     2611 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvadblib/enums.py
--rw-rw-rw-   0        0        0     3130 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvadblib/exceptions.py
--rw-rw-rw-   0        0        0     3530 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvadblib/framebox.py
--rw-rw-rw-   0        0        0    12525 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvadblib/message.py
--rw-rw-rw-   0        0        0     4207 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvadblib/node.py
--rw-rw-rw-   0        0        0    15148 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvadblib/signal.py
--rw-rw-rw-   0        0        0     2326 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvadblib/wrapper.py
-drwxrwxrwx   0        0        0        0 2024-02-18 20:34:48.000000 canlib-1.25.393/canlib/kvamemolibxml/
--rw-rw-rw-   0        0        0     1441 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvamemolibxml/__init__.py
--rw-rw-rw-   0        0        0     4778 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvamemolibxml/configuration.py
--rw-rw-rw-   0        0        0       85 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvamemolibxml/constants.py
--rw-rw-rw-   0        0        0     1587 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvamemolibxml/dll.py
--rw-rw-rw-   0        0        0     3864 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvamemolibxml/enums.py
--rw-rw-rw-   0        0        0     1995 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvamemolibxml/exceptions.py
--rw-rw-rw-   0        0        0     7078 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvamemolibxml/wrapper.py
-drwxrwxrwx   0        0        0        0 2024-02-18 20:34:48.000000 canlib-1.25.393/canlib/kvlclib/
--rw-rw-rw-   0        0        0      761 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvlclib/__init__.py
--rw-rw-rw-   0        0        0     2182 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvlclib/constants.py
--rw-rw-rw-   0        0        0    11729 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvlclib/converter.py
--rw-rw-rw-   0        0        0     4464 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvlclib/deprecated.py
--rw-rw-rw-   0        0        0     3277 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvlclib/dll.py
--rw-rw-rw-   0        0        0     3242 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvlclib/enums.py
--rw-rw-rw-   0        0        0     2333 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvlclib/exceptions.py
--rw-rw-rw-   0        0        0     4745 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvlclib/properties.py
--rw-rw-rw-   0        0        0     3696 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvlclib/readerformat.py
--rw-rw-rw-   0        0        0      766 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvlclib/wrapper.py
--rw-rw-rw-   0        0        0     4390 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvlclib/writerformat.py
-drwxrwxrwx   0        0        0        0 2024-02-18 20:34:48.000000 canlib-1.25.393/canlib/kvmlib/
--rw-rw-rw-   0        0        0     1579 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvmlib/__init__.py
--rw-rw-rw-   0        0        0     2123 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvmlib/constants.py
--rw-rw-rw-   0        0        0    15889 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvmlib/deprecated.py
--rw-rw-rw-   0        0        0     5307 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvmlib/dll.py
--rw-rw-rw-   0        0        0     3429 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvmlib/enums.py
--rw-rw-rw-   0        0        0    16016 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvmlib/events.py
--rw-rw-rw-   0        0        0     2607 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvmlib/exceptions.py
--rw-rw-rw-   0        0        0     6624 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvmlib/kme.py
--rw-rw-rw-   0        0        0     3196 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvmlib/kmf.py
--rw-rw-rw-   0        0        0     3501 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvmlib/log.py
--rw-rw-rw-   0        0        0     4657 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvmlib/logfile.py
--rw-rw-rw-   0        0        0    10133 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvmlib/memorator.py
--rw-rw-rw-   0        0        0      396 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvmlib/messages.py
--rw-rw-rw-   0        0        0      547 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvmlib/wrapper.py
-drwxrwxrwx   0        0        0        0 2024-02-18 20:34:48.000000 canlib-1.25.393/canlib/kvrlib/
--rw-rw-rw-   0        0        0     2506 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvrlib/__init__.py
--rw-rw-rw-   0        0        0     1886 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvrlib/address.py
--rw-rw-rw-   0        0        0     4565 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvrlib/constants.py
--rw-rw-rw-   0        0        0    14748 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvrlib/discovery.py
--rw-rw-rw-   0        0        0     6340 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvrlib/dll.py
--rw-rw-rw-   0        0        0     6646 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvrlib/enums.py
--rw-rw-rw-   0        0        0     1971 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvrlib/exceptions.py
--rw-rw-rw-   0        0        0     7016 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvrlib/infoset.py
--rw-rw-rw-   0        0        0    23169 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvrlib/remotedevice.py
--rw-rw-rw-   0        0        0      923 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvrlib/service.py
--rw-rw-rw-   0        0        0     5172 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvrlib/structures.py
--rw-rw-rw-   0        0        0    13293 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/kvrlib/wrapper.py
-drwxrwxrwx   0        0        0        0 2024-02-18 20:34:48.000000 canlib-1.25.393/canlib/linlib/
--rw-rw-rw-   0        0        0      538 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/linlib/__init__.py
--rw-rw-rw-   0        0        0    15071 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/linlib/channel.py
--rw-rw-rw-   0        0        0     3148 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/linlib/dll.py
--rw-rw-rw-   0        0        0     3799 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/linlib/enums.py
--rw-rw-rw-   0        0        0     2928 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/linlib/exceptions.py
--rw-rw-rw-   0        0        0     2721 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/linlib/structures.py
--rw-rw-rw-   0        0        0     4607 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/linlib/wrapper.py
--rw-rw-rw-   0        0        0     3509 2024-02-18 20:32:40.000000 canlib-1.25.393/canlib/versionnumber.py
-drwxrwxrwx   0        0        0        0 2024-02-18 20:34:48.000000 canlib-1.25.393/canlib.egg-info/
--rw-rw-rw-   0        0        0     7536 2024-02-18 20:34:48.000000 canlib-1.25.393/canlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2882 2024-02-18 20:34:48.000000 canlib-1.25.393/canlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-18 20:34:48.000000 canlib-1.25.393/canlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      129 2024-02-18 20:34:48.000000 canlib-1.25.393/canlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-02-18 20:34:48.000000 canlib-1.25.393/canlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-18 20:34:48.000000 canlib-1.25.393/setup.cfg
--rw-rw-rw-   0        0        0     2381 2024-02-18 20:32:40.000000 canlib-1.25.393/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-18 20:34:48.000000 canlib-1.25.393/tests/
--rw-rw-rw-   0        0        0     6044 2024-02-18 20:32:40.000000 canlib-1.25.393/tests/test_Frame.py
--rw-rw-rw-   0        0        0     7525 2024-02-18 20:32:40.000000 canlib-1.25.393/tests/test_bound_signal.py
--rw-rw-rw-   0        0        0     2374 2024-02-18 20:32:40.000000 canlib-1.25.393/tests/test_device.py
--rw-rw-rw-   0        0        0     1730 2024-02-18 20:32:40.000000 canlib-1.25.393/tests/test_ean.py
--rw-rw-rw-   0        0        0      641 2024-02-18 20:32:40.000000 canlib-1.25.393/tests/test_kvDevice.py
--rw-rw-rw-   0        0        0     2237 2024-02-18 20:32:40.000000 canlib-1.25.393/tests/test_versionnumber.py
+drwxrwxrwx   0        0        0        0 2024-05-22 19:55:17.000000 canlib-1.26.487/
+-rw-rw-rw-   0        0        0     1068 2024-05-22 19:53:07.000000 canlib-1.26.487/LICENSE
+-rw-rw-rw-   0        0        0       59 2024-05-22 19:53:07.000000 canlib-1.26.487/MANIFEST.in
+-rw-rw-rw-   0        0        0     7536 2024-05-22 19:55:17.000000 canlib-1.26.487/PKG-INFO
+-rw-rw-rw-   0        0        0     6792 2024-05-22 19:53:07.000000 canlib-1.26.487/README.rst
+-rw-rw-rw-   0        0        0    26003 2024-05-22 19:53:10.000000 canlib-1.26.487/Relnotes.rst
+drwxrwxrwx   0        0        0        0 2024-05-22 19:55:17.000000 canlib-1.26.487/canlib/
+-rw-rw-rw-   0        0        0      385 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/__about__.py
+-rw-rw-rw-   0        0        0      221 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/__init__.py
+-rw-rw-rw-   0        0        0       26 2024-05-22 19:53:09.000000 canlib-1.26.487/canlib/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 19:55:17.000000 canlib-1.26.487/canlib/canlib/
+-rw-rw-rw-   0        0        0     2477 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/canlib/__init__.py
+-rw-rw-rw-   0        0        0      725 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/canlib/_channel.py
+-rw-rw-rw-   0        0        0    22718 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/canlib/busparams.py
+-rw-rw-rw-   0        0        0    60559 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/canlib/channel.py
+-rw-rw-rw-   0        0        0    18151 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/canlib/channeldata.py
+-rw-rw-rw-   0        0        0    10771 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/canlib/constants.py
+-rw-rw-rw-   0        0        0     9455 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/canlib/dll.py
+-rw-rw-rw-   0        0        0    30560 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/canlib/enums.py
+-rw-rw-rw-   0        0        0     6531 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/canlib/envvar.py
+-rw-rw-rw-   0        0        0     5906 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/canlib/exceptions.py
+-rw-rw-rw-   0        0        0    15796 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/canlib/iocontrol.py
+-rw-rw-rw-   0        0        0    22000 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/canlib/iopin.py
+-rw-rw-rw-   0        0        0     6796 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/canlib/objbuf.py
+-rw-rw-rw-   0        0        0     3305 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/canlib/structures.py
+-rw-rw-rw-   0        0        0     2935 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/canlib/timedomain.py
+-rw-rw-rw-   0        0        0     4932 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/canlib/txe.py
+-rw-rw-rw-   0        0        0    15687 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/canlib/wrapper.py
+-rw-rw-rw-   0        0        0      360 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/cenum.py
+-rw-rw-rw-   0        0        0     7805 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/deprecation.py
+-rw-rw-rw-   0        0        0    16036 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/device.py
+-rw-rw-rw-   0        0        0     8974 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/dllLoader.py
+-rw-rw-rw-   0        0        0     7583 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/ean.py
+-rw-rw-rw-   0        0        0      760 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/exceptions.py
+-rw-rw-rw-   0        0        0     4003 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/frame.py
+-rw-rw-rw-   0        0        0     8738 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/futureapi.py
+-rw-rw-rw-   0        0        0     5226 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/j1939.py
+-rw-rw-rw-   0        0        0    12275 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvDevice.py
+-rw-rw-rw-   0        0        0    25506 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvMemoConfig.py
+-rw-rw-rw-   0        0        0      115 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvMessage.py
+-rw-rw-rw-   0        0        0      247 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvaMemoLibXml.py
+drwxrwxrwx   0        0        0        0 2024-05-22 19:55:17.000000 canlib-1.26.487/canlib/kvadblib/
+-rw-rw-rw-   0        0        0     1517 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvadblib/__init__.py
+-rw-rw-rw-   0        0        0     3498 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvadblib/attribute.py
+-rw-rw-rw-   0        0        0     8276 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvadblib/attributedef.py
+-rw-rw-rw-   0        0        0     1189 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvadblib/bound_message.py
+-rw-rw-rw-   0        0        0     2099 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvadblib/bound_signal.py
+-rw-rw-rw-   0        0        0       11 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvadblib/constants.py
+-rw-rw-rw-   0        0        0    18943 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvadblib/dbc.py
+-rw-rw-rw-   0        0        0    11330 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvadblib/dll.py
+-rw-rw-rw-   0        0        0     2611 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvadblib/enums.py
+-rw-rw-rw-   0        0        0     3130 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvadblib/exceptions.py
+-rw-rw-rw-   0        0        0     3530 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvadblib/framebox.py
+-rw-rw-rw-   0        0        0    12525 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvadblib/message.py
+-rw-rw-rw-   0        0        0     4207 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvadblib/node.py
+-rw-rw-rw-   0        0        0    15148 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvadblib/signal.py
+-rw-rw-rw-   0        0        0     2326 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvadblib/wrapper.py
+drwxrwxrwx   0        0        0        0 2024-05-22 19:55:17.000000 canlib-1.26.487/canlib/kvamemolibxml/
+-rw-rw-rw-   0        0        0     1441 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvamemolibxml/__init__.py
+-rw-rw-rw-   0        0        0     4778 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvamemolibxml/configuration.py
+-rw-rw-rw-   0        0        0       85 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvamemolibxml/constants.py
+-rw-rw-rw-   0        0        0     1587 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvamemolibxml/dll.py
+-rw-rw-rw-   0        0        0     3864 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvamemolibxml/enums.py
+-rw-rw-rw-   0        0        0     1995 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvamemolibxml/exceptions.py
+-rw-rw-rw-   0        0        0     7078 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvamemolibxml/wrapper.py
+drwxrwxrwx   0        0        0        0 2024-05-22 19:55:17.000000 canlib-1.26.487/canlib/kvlclib/
+-rw-rw-rw-   0        0        0      761 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvlclib/__init__.py
+-rw-rw-rw-   0        0        0     2182 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvlclib/constants.py
+-rw-rw-rw-   0        0        0    11729 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvlclib/converter.py
+-rw-rw-rw-   0        0        0     4464 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvlclib/deprecated.py
+-rw-rw-rw-   0        0        0     3277 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvlclib/dll.py
+-rw-rw-rw-   0        0        0     3242 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvlclib/enums.py
+-rw-rw-rw-   0        0        0     2333 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvlclib/exceptions.py
+-rw-rw-rw-   0        0        0     4745 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvlclib/properties.py
+-rw-rw-rw-   0        0        0     3696 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvlclib/readerformat.py
+-rw-rw-rw-   0        0        0      766 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvlclib/wrapper.py
+-rw-rw-rw-   0        0        0     4390 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvlclib/writerformat.py
+drwxrwxrwx   0        0        0        0 2024-05-22 19:55:17.000000 canlib-1.26.487/canlib/kvmlib/
+-rw-rw-rw-   0        0        0     1579 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvmlib/__init__.py
+-rw-rw-rw-   0        0        0     2123 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvmlib/constants.py
+-rw-rw-rw-   0        0        0    15889 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvmlib/deprecated.py
+-rw-rw-rw-   0        0        0     5307 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvmlib/dll.py
+-rw-rw-rw-   0        0        0     3429 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvmlib/enums.py
+-rw-rw-rw-   0        0        0    16016 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvmlib/events.py
+-rw-rw-rw-   0        0        0     2607 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvmlib/exceptions.py
+-rw-rw-rw-   0        0        0     6624 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvmlib/kme.py
+-rw-rw-rw-   0        0        0     3196 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvmlib/kmf.py
+-rw-rw-rw-   0        0        0     3501 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvmlib/log.py
+-rw-rw-rw-   0        0        0     4657 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvmlib/logfile.py
+-rw-rw-rw-   0        0        0    10133 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvmlib/memorator.py
+-rw-rw-rw-   0        0        0      396 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvmlib/messages.py
+-rw-rw-rw-   0        0        0      547 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvmlib/wrapper.py
+drwxrwxrwx   0        0        0        0 2024-05-22 19:55:17.000000 canlib-1.26.487/canlib/kvrlib/
+-rw-rw-rw-   0        0        0     2506 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvrlib/__init__.py
+-rw-rw-rw-   0        0        0     1886 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvrlib/address.py
+-rw-rw-rw-   0        0        0     4565 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvrlib/constants.py
+-rw-rw-rw-   0        0        0    14748 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvrlib/discovery.py
+-rw-rw-rw-   0        0        0     6340 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvrlib/dll.py
+-rw-rw-rw-   0        0        0     6646 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvrlib/enums.py
+-rw-rw-rw-   0        0        0     1971 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvrlib/exceptions.py
+-rw-rw-rw-   0        0        0     7016 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvrlib/infoset.py
+-rw-rw-rw-   0        0        0    23169 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvrlib/remotedevice.py
+-rw-rw-rw-   0        0        0      923 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvrlib/service.py
+-rw-rw-rw-   0        0        0     5172 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvrlib/structures.py
+-rw-rw-rw-   0        0        0    13293 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/kvrlib/wrapper.py
+drwxrwxrwx   0        0        0        0 2024-05-22 19:55:17.000000 canlib-1.26.487/canlib/linlib/
+-rw-rw-rw-   0        0        0      538 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/linlib/__init__.py
+-rw-rw-rw-   0        0        0    15071 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/linlib/channel.py
+-rw-rw-rw-   0        0        0     3148 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/linlib/dll.py
+-rw-rw-rw-   0        0        0     3799 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/linlib/enums.py
+-rw-rw-rw-   0        0        0     2928 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/linlib/exceptions.py
+-rw-rw-rw-   0        0        0     2721 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/linlib/structures.py
+-rw-rw-rw-   0        0        0     4607 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/linlib/wrapper.py
+-rw-rw-rw-   0        0        0     3509 2024-05-22 19:53:07.000000 canlib-1.26.487/canlib/versionnumber.py
+drwxrwxrwx   0        0        0        0 2024-05-22 19:55:17.000000 canlib-1.26.487/canlib.egg-info/
+-rw-rw-rw-   0        0        0     7536 2024-05-22 19:55:17.000000 canlib-1.26.487/canlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2882 2024-05-22 19:55:17.000000 canlib-1.26.487/canlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 19:55:17.000000 canlib-1.26.487/canlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      129 2024-05-22 19:55:17.000000 canlib-1.26.487/canlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-22 19:55:17.000000 canlib-1.26.487/canlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 19:55:17.000000 canlib-1.26.487/setup.cfg
+-rw-rw-rw-   0        0        0     2381 2024-05-22 19:53:07.000000 canlib-1.26.487/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 19:55:17.000000 canlib-1.26.487/tests/
+-rw-rw-rw-   0        0        0     6044 2024-05-22 19:53:07.000000 canlib-1.26.487/tests/test_Frame.py
+-rw-rw-rw-   0        0        0     7525 2024-05-22 19:53:07.000000 canlib-1.26.487/tests/test_bound_signal.py
+-rw-rw-rw-   0        0        0     2374 2024-05-22 19:53:07.000000 canlib-1.26.487/tests/test_device.py
+-rw-rw-rw-   0        0        0     1730 2024-05-22 19:53:07.000000 canlib-1.26.487/tests/test_ean.py
+-rw-rw-rw-   0        0        0      641 2024-05-22 19:53:07.000000 canlib-1.26.487/tests/test_kvDevice.py
+-rw-rw-rw-   0        0        0     2237 2024-05-22 19:53:07.000000 canlib-1.26.487/tests/test_versionnumber.py
```

### Comparing `canlib-1.25.393/LICENSE` & `canlib-1.26.487/LICENSE`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/PKG-INFO` & `canlib-1.26.487/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canlib
-Version: 1.25.393
+Version: 1.26.487
 Summary: Python wrapper for Kvaser CANlib
 Home-page: https://github.com/Kvaser/pycanlib
 Author: Kvaser AB
 Author-email: support@kvaser.com
 License: MIT
 Keywords: development
 Classifier: Development Status :: 4 - Beta
```

### Comparing `canlib-1.25.393/README.rst` & `canlib-1.26.487/README.rst`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/Relnotes.rst` & `canlib-1.26.487/Relnotes.rst`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 ===========================================================================
 This is the release notes for the pycanlib module.
 
 .. contents::
     :depth: 2
 
 
+New Features and Fixed Problems in V1.26.487  (22-MAY-2024)
+===========================================================================
+* Added new enums to canlib.
+
+
 New Features and Fixed Problems in V1.25.393  (18-FEB-2024)
 ===========================================================================
 * Minor changes.
 
 
 New Features and Fixed Problems in V1.24.935  (13-SEP-2023)
 ===========================================================================
```

### Comparing `canlib-1.25.393/canlib/canlib/__init__.py` & `canlib-1.26.487/canlib/canlib/__init__.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/canlib/_channel.py` & `canlib-1.26.487/canlib/canlib/_channel.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/canlib/busparams.py` & `canlib-1.26.487/canlib/canlib/busparams.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/canlib/channel.py` & `canlib-1.26.487/canlib/canlib/channel.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/canlib/channeldata.py` & `canlib-1.26.487/canlib/canlib/channeldata.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/canlib/constants.py` & `canlib-1.26.487/canlib/canlib/constants.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/canlib/dll.py` & `canlib-1.26.487/canlib/canlib/dll.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/canlib/enums.py` & `canlib-1.26.487/canlib/canlib/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -524,14 +524,15 @@
     T_1041 = 16  #: TJA1041
     T_1041_OPTO = 17  #: TJA1041 with optical isolation
     RS485 = 18  #: RS485 (i.e. J1708)
     LIN = 19
     KONE = 20
     CANFD = 22
     CANFD_LIN = 24  #: HYBRID CAN-FD/LIN
+    CANFD_SIC = 26  #: CAN-FD SIC transceiver
     LINX_LIN = 64
     LINX_J1708 = 66
     LINX_K = 68
     LINX_SWC = 70
     LINX_LS = 72
 
 
@@ -619,18 +620,19 @@
     USBCAN_KLINE = 68  #: USBcan Pro HS/K-Line.
     ETHERCAN = 70  #: Kvaser Ethercan.
     USBCAN_LIGHT = 72  #: Kvaser USBcan Light.
     USBCAN_PRO2 = 74  #: Kvaser USBcan Pro 5xHS and variants.
     PCIE_V2 = 76  #: Kvaser PCIEcan 4xHS and variants.
     MEMORATOR_PRO2 = 78  #: Kvaser Memorator Pro 5xHS and variants.
     LEAF2 = 80  #: Kvaser Leaf Pro HS v2 and variants.
-    MEMORATOR_V2 = 82  #: Kvaser Memorator (2nd generation)
+    MEMORATOR_V2 = 82  #: Kvaser Memorator (2nd generation).
     CANLINHYBRID = 84  #: Kvaser Hybrid CAN/LIN.
-    DINRAIL = 86  #: Kvaser DIN Rail SE400S and variants
-    U100 = 88  #: Kvaser U100 and variants
+    DINRAIL = 86  #: Kvaser DIN Rail SE400S and variants.
+    U100 = 88  #: Kvaser U100 and variants.
+    LEAF_V3 = 90 #: Kvaser Kvaser Leaf v3 and variants.
 
     # Obsolete
     CANPARI = 3  #: CANpari (obsolete).
     USBCAN = 11  #: USBcan (obsolete).
     SIMULATED = 44  #: Simulated CAN bus for Kvaser Creator (obsolete).
     ACQUISITOR = 46  #: Kvaser Acquisitor (obsolete).
     IRIS = 58  #: Obsolete name, use `BLACKBIRD` instead.
```

### Comparing `canlib-1.25.393/canlib/canlib/envvar.py` & `canlib-1.26.487/canlib/canlib/envvar.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/canlib/exceptions.py` & `canlib-1.26.487/canlib/canlib/exceptions.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/canlib/iocontrol.py` & `canlib-1.26.487/canlib/canlib/iocontrol.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/canlib/iopin.py` & `canlib-1.26.487/canlib/canlib/iopin.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/canlib/objbuf.py` & `canlib-1.26.487/canlib/canlib/objbuf.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/canlib/structures.py` & `canlib-1.26.487/canlib/canlib/structures.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/canlib/timedomain.py` & `canlib-1.26.487/canlib/canlib/timedomain.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/canlib/txe.py` & `canlib-1.26.487/canlib/canlib/txe.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/canlib/wrapper.py` & `canlib-1.26.487/canlib/canlib/wrapper.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/deprecation.py` & `canlib-1.26.487/canlib/deprecation.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/device.py` & `canlib-1.26.487/canlib/device.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/dllLoader.py` & `canlib-1.26.487/canlib/dllLoader.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/ean.py` & `canlib-1.26.487/canlib/ean.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/exceptions.py` & `canlib-1.26.487/canlib/exceptions.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/frame.py` & `canlib-1.26.487/canlib/frame.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/futureapi.py` & `canlib-1.26.487/canlib/futureapi.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/j1939.py` & `canlib-1.26.487/canlib/j1939.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvDevice.py` & `canlib-1.26.487/canlib/kvDevice.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvMemoConfig.py` & `canlib-1.26.487/canlib/kvMemoConfig.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvadblib/__init__.py` & `canlib-1.26.487/canlib/kvadblib/__init__.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvadblib/attribute.py` & `canlib-1.26.487/canlib/kvadblib/attribute.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvadblib/attributedef.py` & `canlib-1.26.487/canlib/kvadblib/attributedef.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvadblib/bound_message.py` & `canlib-1.26.487/canlib/kvadblib/bound_message.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvadblib/bound_signal.py` & `canlib-1.26.487/canlib/kvadblib/bound_signal.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvadblib/dbc.py` & `canlib-1.26.487/canlib/kvadblib/dbc.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvadblib/dll.py` & `canlib-1.26.487/canlib/kvadblib/dll.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvadblib/enums.py` & `canlib-1.26.487/canlib/kvadblib/enums.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvadblib/exceptions.py` & `canlib-1.26.487/canlib/kvadblib/exceptions.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvadblib/framebox.py` & `canlib-1.26.487/canlib/kvadblib/framebox.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvadblib/message.py` & `canlib-1.26.487/canlib/kvadblib/message.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvadblib/node.py` & `canlib-1.26.487/canlib/kvadblib/node.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvadblib/signal.py` & `canlib-1.26.487/canlib/kvadblib/signal.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvadblib/wrapper.py` & `canlib-1.26.487/canlib/kvadblib/wrapper.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvamemolibxml/__init__.py` & `canlib-1.26.487/canlib/kvamemolibxml/__init__.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvamemolibxml/configuration.py` & `canlib-1.26.487/canlib/kvamemolibxml/configuration.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvamemolibxml/dll.py` & `canlib-1.26.487/canlib/kvamemolibxml/dll.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvamemolibxml/enums.py` & `canlib-1.26.487/canlib/kvamemolibxml/enums.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvamemolibxml/exceptions.py` & `canlib-1.26.487/canlib/kvamemolibxml/exceptions.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvamemolibxml/wrapper.py` & `canlib-1.26.487/canlib/kvamemolibxml/wrapper.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvlclib/__init__.py` & `canlib-1.26.487/canlib/kvlclib/__init__.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvlclib/constants.py` & `canlib-1.26.487/canlib/kvlclib/constants.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvlclib/converter.py` & `canlib-1.26.487/canlib/kvlclib/converter.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvlclib/deprecated.py` & `canlib-1.26.487/canlib/kvlclib/deprecated.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvlclib/dll.py` & `canlib-1.26.487/canlib/kvlclib/dll.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvlclib/enums.py` & `canlib-1.26.487/canlib/kvlclib/enums.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvlclib/exceptions.py` & `canlib-1.26.487/canlib/kvlclib/exceptions.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvlclib/properties.py` & `canlib-1.26.487/canlib/kvlclib/properties.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvlclib/readerformat.py` & `canlib-1.26.487/canlib/kvlclib/readerformat.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvlclib/wrapper.py` & `canlib-1.26.487/canlib/kvlclib/wrapper.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvlclib/writerformat.py` & `canlib-1.26.487/canlib/kvlclib/writerformat.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvmlib/__init__.py` & `canlib-1.26.487/canlib/kvmlib/__init__.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvmlib/constants.py` & `canlib-1.26.487/canlib/kvmlib/constants.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvmlib/deprecated.py` & `canlib-1.26.487/canlib/kvmlib/deprecated.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvmlib/dll.py` & `canlib-1.26.487/canlib/kvmlib/dll.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvmlib/enums.py` & `canlib-1.26.487/canlib/kvmlib/enums.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvmlib/events.py` & `canlib-1.26.487/canlib/kvmlib/events.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvmlib/exceptions.py` & `canlib-1.26.487/canlib/kvmlib/exceptions.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvmlib/kme.py` & `canlib-1.26.487/canlib/kvmlib/kme.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvmlib/kmf.py` & `canlib-1.26.487/canlib/kvmlib/kmf.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvmlib/log.py` & `canlib-1.26.487/canlib/kvmlib/log.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvmlib/logfile.py` & `canlib-1.26.487/canlib/kvmlib/logfile.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvmlib/memorator.py` & `canlib-1.26.487/canlib/kvmlib/memorator.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvmlib/wrapper.py` & `canlib-1.26.487/canlib/kvmlib/wrapper.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvrlib/__init__.py` & `canlib-1.26.487/canlib/kvrlib/__init__.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvrlib/address.py` & `canlib-1.26.487/canlib/kvrlib/address.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvrlib/constants.py` & `canlib-1.26.487/canlib/kvrlib/constants.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvrlib/discovery.py` & `canlib-1.26.487/canlib/kvrlib/discovery.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvrlib/dll.py` & `canlib-1.26.487/canlib/kvrlib/dll.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvrlib/enums.py` & `canlib-1.26.487/canlib/kvrlib/enums.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvrlib/exceptions.py` & `canlib-1.26.487/canlib/kvrlib/exceptions.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvrlib/infoset.py` & `canlib-1.26.487/canlib/kvrlib/infoset.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvrlib/remotedevice.py` & `canlib-1.26.487/canlib/kvrlib/remotedevice.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvrlib/service.py` & `canlib-1.26.487/canlib/kvrlib/service.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvrlib/structures.py` & `canlib-1.26.487/canlib/kvrlib/structures.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/kvrlib/wrapper.py` & `canlib-1.26.487/canlib/kvrlib/wrapper.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/linlib/__init__.py` & `canlib-1.26.487/canlib/linlib/__init__.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/linlib/channel.py` & `canlib-1.26.487/canlib/linlib/channel.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/linlib/dll.py` & `canlib-1.26.487/canlib/linlib/dll.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/linlib/enums.py` & `canlib-1.26.487/canlib/linlib/enums.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/linlib/exceptions.py` & `canlib-1.26.487/canlib/linlib/exceptions.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/linlib/structures.py` & `canlib-1.26.487/canlib/linlib/structures.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/linlib/wrapper.py` & `canlib-1.26.487/canlib/linlib/wrapper.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib/versionnumber.py` & `canlib-1.26.487/canlib/versionnumber.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/canlib.egg-info/PKG-INFO` & `canlib-1.26.487/canlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canlib
-Version: 1.25.393
+Version: 1.26.487
 Summary: Python wrapper for Kvaser CANlib
 Home-page: https://github.com/Kvaser/pycanlib
 Author: Kvaser AB
 Author-email: support@kvaser.com
 License: MIT
 Keywords: development
 Classifier: Development Status :: 4 - Beta
```

### Comparing `canlib-1.25.393/canlib.egg-info/SOURCES.txt` & `canlib-1.26.487/canlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/setup.py` & `canlib-1.26.487/setup.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/tests/test_Frame.py` & `canlib-1.26.487/tests/test_Frame.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/tests/test_bound_signal.py` & `canlib-1.26.487/tests/test_bound_signal.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/tests/test_device.py` & `canlib-1.26.487/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/tests/test_ean.py` & `canlib-1.26.487/tests/test_ean.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/tests/test_kvDevice.py` & `canlib-1.26.487/tests/test_kvDevice.py`

 * *Files identical despite different names*

### Comparing `canlib-1.25.393/tests/test_versionnumber.py` & `canlib-1.26.487/tests/test_versionnumber.py`

 * *Files identical despite different names*

