# Comparing `tmp/seatsio-76.6.0.tar.gz` & `tmp/seatsio-76.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seatsio-76.6.0.tar", last modified: Wed Apr 24 11:23:49 2024, max compression
+gzip compressed data, was "seatsio-76.7.0.tar", last modified: Wed May 29 09:22:48 2024, max compression
```

## Comparing `seatsio-76.6.0.tar` & `seatsio-76.7.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:49.213226 seatsio-76.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-24 11:23:44.000000 seatsio-76.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 11:23:44.000000 seatsio-76.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-04-24 11:23:49.213226 seatsio-76.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-04-24 11:23:44.000000 seatsio-76.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:49.205226 seatsio-76.6.0/seatsio/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:49.209226 seatsio-76.6.0/seatsio/charts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/charts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/charts/chartsClient.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/charts/chartsRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/domain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:49.209226 seatsio-76.6.0/seatsio/eventlog/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/eventlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/eventlog/eventLogClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:49.209226 seatsio-76.6.0/seatsio/events/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/changeBestAvailableObjectStatusRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/changeObjectStatusRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/channelProperties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/channelsClient.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/channelsRequests.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/createMultipleEventsRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/createSingleEventRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/eventProperties.py
--rw-r--r--   0 runner    (1001) docker     (127)    11568 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/eventsClient.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/extraDataRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/forSaleRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/objectProperties.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/overrideSeasonObjectStatusRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/statusChangeRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/updateEventRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:49.209226 seatsio-76.6.0/seatsio/holdtokens/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/holdtokens/HoldTokenClient.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/holdtokens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/httpClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:49.213226 seatsio-76.6.0/seatsio/pagination/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/pagination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/pagination/listableObjectsClient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/pagination/lister.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/pagination/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/pagination/pageFetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/pagination/pagedIterator.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/region.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:49.213226 seatsio-76.6.0/seatsio/reports/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:49.213226 seatsio-76.6.0/seatsio/reports/charts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/reports/charts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/reports/charts/chartReports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:49.213226 seatsio-76.6.0/seatsio/reports/events/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/reports/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/reports/events/eventReports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:49.213226 seatsio-76.6.0/seatsio/reports/usage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/reports/usage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/reports/usage/usageReports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:49.213226 seatsio-76.6.0/seatsio/seasons/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/seasons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/seasons/seasonsClient.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:49.213226 seatsio-76.6.0/seatsio/workspaces/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/workspaces/UpdateWorkspaceRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/workspaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/workspaces/createWorkspaceRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/workspaces/workspacesClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:49.209226 seatsio-76.6.0/seatsio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-04-24 11:23:49.000000 seatsio-76.6.0/seatsio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-24 11:23:49.000000 seatsio-76.6.0/seatsio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 11:23:49.000000 seatsio-76.6.0/seatsio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 11:23:49.000000 seatsio-76.6.0/seatsio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-24 11:23:49.000000 seatsio-76.6.0/seatsio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 11:23:49.213226 seatsio-76.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-24 11:23:46.000000 seatsio-76.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:22:48.419281 seatsio-76.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-29 09:22:40.000000 seatsio-76.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-29 09:22:40.000000 seatsio-76.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6928 2024-05-29 09:22:48.419281 seatsio-76.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-05-29 09:22:40.000000 seatsio-76.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:22:48.415281 seatsio-76.7.0/seatsio/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:22:48.415281 seatsio-76.7.0/seatsio/charts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/charts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/charts/chartsClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/charts/chartsRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15227 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/domain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:22:48.415281 seatsio-76.7.0/seatsio/eventlog/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/eventlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/eventlog/eventLogClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:22:48.419281 seatsio-76.7.0/seatsio/events/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/events/changeBestAvailableObjectStatusRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/events/changeObjectStatusRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/events/channelProperties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/events/channelsClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/events/channelsRequests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/events/createMultipleEventsRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/events/createSingleEventRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/events/eventProperties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11568 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/events/eventsClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/events/extraDataRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/events/forSaleRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/events/objectProperties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/events/overrideSeasonObjectStatusRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/events/statusChangeRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/events/updateEventRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:22:48.419281 seatsio-76.7.0/seatsio/holdtokens/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/holdtokens/HoldTokenClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/holdtokens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/httpClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:22:48.419281 seatsio-76.7.0/seatsio/pagination/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/pagination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/pagination/listableObjectsClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/pagination/lister.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/pagination/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/pagination/pageFetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/pagination/pagedIterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/region.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:22:48.419281 seatsio-76.7.0/seatsio/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:22:48.419281 seatsio-76.7.0/seatsio/reports/charts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/reports/charts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/reports/charts/chartReports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:22:48.419281 seatsio-76.7.0/seatsio/reports/events/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/reports/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/reports/events/eventReports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:22:48.419281 seatsio-76.7.0/seatsio/reports/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/reports/usage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/reports/usage/usageReports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:22:48.419281 seatsio-76.7.0/seatsio/seasons/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/seasons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/seasons/seasonsClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:22:48.419281 seatsio-76.7.0/seatsio/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/workspaces/UpdateWorkspaceRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/workspaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/workspaces/createWorkspaceRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-29 09:22:40.000000 seatsio-76.7.0/seatsio/workspaces/workspacesClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:22:48.415281 seatsio-76.7.0/seatsio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6928 2024-05-29 09:22:48.000000 seatsio-76.7.0/seatsio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-29 09:22:48.000000 seatsio-76.7.0/seatsio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 09:22:48.000000 seatsio-76.7.0/seatsio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-29 09:22:48.000000 seatsio-76.7.0/seatsio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-29 09:22:48.000000 seatsio-76.7.0/seatsio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 09:22:48.419281 seatsio-76.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-29 09:22:45.000000 seatsio-76.7.0/setup.py
```

### Comparing `seatsio-76.6.0/LICENSE` & `seatsio-76.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seatsio-76.6.0/PKG-INFO` & `seatsio-76.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seatsio
-Version: 76.6.0
+Version: 76.7.0
 Summary: The official Seats.io Python client library
 Home-page: https://github.com/seatsio/seatsio-python
 Author: The seats.io dev team
 Author-email: hello@seats.io
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -114,14 +114,22 @@
 import seatsio
 client = seatsio.Client(seatsio.Region.EU(), secret_key="my-workspace-secret-key")
 category_list = client.charts.list_categories(<chart key>)
 for category in category_list:
   print(category.label)
 ```
 
+### Updating a category
+
+```python
+import seatsio
+client = seatsio.Client(seatsio.Region.EU(), secret_key="my-workspace-secret-key")
+client.charts.update_category(chart_key=chart.key, category_key=1, label="Updated label", color="#bbbbbb", accessible=True)
+```
+
 ### Listing all charts
 
 ```python
 import seatsio
 client = seatsio.Client(seatsio.Region.EU(), secret_key="my-workspace-secret-key")
 charts = client.charts.list()
 for chart in charts:
```

### Comparing `seatsio-76.6.0/README.md` & `seatsio-76.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,22 @@
 import seatsio
 client = seatsio.Client(seatsio.Region.EU(), secret_key="my-workspace-secret-key")
 category_list = client.charts.list_categories(<chart key>)
 for category in category_list:
   print(category.label)
 ```
 
+### Updating a category
+
+```python
+import seatsio
+client = seatsio.Client(seatsio.Region.EU(), secret_key="my-workspace-secret-key")
+client.charts.update_category(chart_key=chart.key, category_key=1, label="Updated label", color="#bbbbbb", accessible=True)
+```
+
 ### Listing all charts
 
 ```python
 import seatsio
 client = seatsio.Client(seatsio.Region.EU(), secret_key="my-workspace-secret-key")
 charts = client.charts.list()
 for chart in charts:
```

### Comparing `seatsio-76.6.0/seatsio/charts/chartsClient.py` & `seatsio-76.7.0/seatsio/charts/chartsClient.py`

 * *Files 10% similar despite different names*

```diff
@@ -93,14 +93,20 @@
 
     def list_categories(self, chart_key):
         response = self.http_client.url("/charts/{chart_key}/categories",
                                         chart_key=chart_key) \
             .get()
         return Category.create_list(response["categories"])
 
+    def update_category(self, chart_key, category_key, label, color, accessible):
+        self.http_client.url("/charts/{chart_key}/categories/{category_key}",
+                             chart_key=chart_key,
+                             category_key=category_key) \
+            .post(UpdateCategoryRequest(label, color, accessible))
+
     def move_to_archive(self, chart_key):
         self.http_client.url("/charts/{key}/actions/move-to-archive", key=chart_key).post()
 
     def move_out_of_archive(self, chart_key):
         self.http_client.url("/charts/{key}/actions/move-out-of-archive", key=chart_key).post()
 
     def publish_draft_version(self, chart_key):
@@ -129,7 +135,16 @@
     def validate_published_version(self, key):
         response = self.http_client.url("/charts/{key}/version/published/actions/validate", key=key).post()
         return ChartValidation(json.loads(response.text))
 
     def validate_draft_version(self, key):
         response = self.http_client.url("/charts/{key}/version/draft/actions/validate", key=key).post()
         return ChartValidation(json.loads(response.text))
+
+class UpdateCategoryRequest:
+    def __init__(self, label, color, accessible):
+        if label:
+            self.label = label
+        if color:
+            self.color = color
+        if accessible:
+            self.accessible = accessible
```

### Comparing `seatsio-76.6.0/seatsio/client.py` & `seatsio-76.7.0/seatsio/client.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.6.0/seatsio/domain.py` & `seatsio-76.7.0/seatsio/domain.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         self.name = data.get("name")
         self.published_version_thumbnail_url = data.get("publishedVersionThumbnailUrl")
         self.draft_version_thumbnail_url = data.get("draftVersionThumbnailUrl")
         self.events = Event.create_list(data.get("events"))
         self.tags = data.get("tags")
         self.archived = data.get("archived")
         self.validation = data.get("validation")
+        self.venue_type = data.get("venueType")
 
 
 class ChartValidation:
 
     def __init__(self, data):
         self.errors = data.get("errors")
         self.warnings = data.get("warnings")
```

### Comparing `seatsio-76.6.0/seatsio/events/changeBestAvailableObjectStatusRequest.py` & `seatsio-76.7.0/seatsio/events/changeBestAvailableObjectStatusRequest.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.6.0/seatsio/events/changeObjectStatusRequest.py` & `seatsio-76.7.0/seatsio/events/changeObjectStatusRequest.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.6.0/seatsio/events/channelsClient.py` & `seatsio-76.7.0/seatsio/events/channelsClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.6.0/seatsio/events/channelsRequests.py` & `seatsio-76.7.0/seatsio/events/channelsRequests.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.6.0/seatsio/events/createSingleEventRequest.py` & `seatsio-76.7.0/seatsio/events/createSingleEventRequest.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.6.0/seatsio/events/eventProperties.py` & `seatsio-76.7.0/seatsio/events/eventProperties.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.6.0/seatsio/events/eventsClient.py` & `seatsio-76.7.0/seatsio/events/eventsClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.6.0/seatsio/events/statusChangeRequest.py` & `seatsio-76.7.0/seatsio/events/statusChangeRequest.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.6.0/seatsio/events/updateEventRequest.py` & `seatsio-76.7.0/seatsio/events/updateEventRequest.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.6.0/seatsio/exceptions.py` & `seatsio-76.7.0/seatsio/exceptions.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.6.0/seatsio/holdtokens/HoldTokenClient.py` & `seatsio-76.7.0/seatsio/holdtokens/HoldTokenClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.6.0/seatsio/httpClient.py` & `seatsio-76.7.0/seatsio/httpClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.6.0/seatsio/pagination/listableObjectsClient.py` & `seatsio-76.7.0/seatsio/pagination/listableObjectsClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.6.0/seatsio/pagination/lister.py` & `seatsio-76.7.0/seatsio/pagination/lister.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.6.0/seatsio/pagination/page.py` & `seatsio-76.7.0/seatsio/pagination/page.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.6.0/seatsio/pagination/pageFetcher.py` & `seatsio-76.7.0/seatsio/pagination/pageFetcher.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.6.0/seatsio/pagination/pagedIterator.py` & `seatsio-76.7.0/seatsio/pagination/pagedIterator.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.6.0/seatsio/reports/charts/chartReports.py` & `seatsio-76.7.0/seatsio/reports/charts/chartReports.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.6.0/seatsio/reports/events/eventReports.py` & `seatsio-76.7.0/seatsio/reports/events/eventReports.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.6.0/seatsio/reports/usage/usageReports.py` & `seatsio-76.7.0/seatsio/reports/usage/usageReports.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.6.0/seatsio/seasons/seasonsClient.py` & `seatsio-76.7.0/seatsio/seasons/seasonsClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.6.0/seatsio/workspaces/workspacesClient.py` & `seatsio-76.7.0/seatsio/workspaces/workspacesClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.6.0/seatsio.egg-info/PKG-INFO` & `seatsio-76.7.0/seatsio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seatsio
-Version: 76.6.0
+Version: 76.7.0
 Summary: The official Seats.io Python client library
 Home-page: https://github.com/seatsio/seatsio-python
 Author: The seats.io dev team
 Author-email: hello@seats.io
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -114,14 +114,22 @@
 import seatsio
 client = seatsio.Client(seatsio.Region.EU(), secret_key="my-workspace-secret-key")
 category_list = client.charts.list_categories(<chart key>)
 for category in category_list:
   print(category.label)
 ```
 
+### Updating a category
+
+```python
+import seatsio
+client = seatsio.Client(seatsio.Region.EU(), secret_key="my-workspace-secret-key")
+client.charts.update_category(chart_key=chart.key, category_key=1, label="Updated label", color="#bbbbbb", accessible=True)
+```
+
 ### Listing all charts
 
 ```python
 import seatsio
 client = seatsio.Client(seatsio.Region.EU(), secret_key="my-workspace-secret-key")
 charts = client.charts.list()
 for chart in charts:
```

### Comparing `seatsio-76.6.0/seatsio.egg-info/SOURCES.txt` & `seatsio-76.7.0/seatsio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seatsio-76.6.0/setup.py` & `seatsio-76.7.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name='seatsio',
-    version='v76.6.0',
+    version='v76.7.0',
     description='The official Seats.io Python client library',
     author='The seats.io dev team',
     author_email='hello@seats.io',
     url='https://github.com/seatsio/seatsio-python',
     license="MIT",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
 
     packages=find_packages(),
     install_requires=[
-        "requests==2.31",
+        "requests==2.32.0",
         "munch==4.0",
         "jsonpickle>=1.0, <1.4",
         "future==1.0.0",
         "six==1.16",
     ],
     tests_require=[
         "parameterized==0.9.0"
```

