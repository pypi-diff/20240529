# Comparing `tmp/dub-0.0.5.tar.gz` & `tmp/dub-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dub-0.0.5.tar", last modified: Tue May 21 19:07:05 2024, max compression
+gzip compressed data, was "dub-0.0.6.tar", last modified: Wed May 29 17:13:44 2024, max compression
```

## Comparing `dub-0.0.5.tar` & `dub-0.0.6.tar`

### file list

```diff
@@ -1,109 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:07:05.686021 dub-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    17862 2024-05-21 19:07:05.686021 dub-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12238 2024-05-21 19:06:57.000000 dub-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 19:07:05.686021 dub-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-21 19:06:57.000000 dub-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:07:05.666021 dub-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:07:05.670021 dub-0.0.5/src/dub/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:07:05.674021 dub-0.0.5/src/dub/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    76952 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)    91883 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/clicks.py
--rw-r--r--   0 runner    (1001) docker     (127)    51298 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/domains.py
--rw-r--r--   0 runner    (1001) docker     (127)    68151 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/links.py
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/metatags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:07:05.674021 dub-0.0.5/src/dub/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:07:05.674021 dub-0.0.5/src/dub/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/components/clicksbycities.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/components/clicksbycountry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/components/countrycode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/components/domainschema.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/components/httpmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    41946 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/components/linkgeotargeting.py
--rw-r--r--   0 runner    (1001) docker     (127)    50145 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/components/linkschema.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/components/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/components/tagschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/components/workspaceschema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:07:05.678021 dub-0.0.5/src/dub/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/errors/badrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/errors/conflict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/errors/forbidden.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/errors/internalservererror.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/errors/inviteexpired.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/errors/notfound.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/errors/ratelimitexceeded.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/errors/sdkerror.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/errors/unauthorized.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/errors/unprocessableentity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:07:05.678021 dub-0.0.5/src/dub/models/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/internal/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:07:05.682021 dub-0.0.5/src/dub/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/adddomain.py
--rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/bulkcreatelinks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/createlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/createtag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/createworkspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/deletedomain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/deletelink.py
--rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getbrowsersbyclicks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getbrowsersbyclicksdeprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getcitiesbyclicks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getcitiesbyclicksdeprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getclickscount.py
--rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getclickscountdeprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getcountriesbyclicks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getcountriesbyclicksdeprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     5798 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getdevicesbyclicks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getdevicesbyclicksdeprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getlinkinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getlinks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getlinkscount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getmetatags.py
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getosbyclicks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getosbyclicksdeprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getqrcode.py
--rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getreferersbyclicks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getreferersbyclicksdeprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/gettags.py
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/gettimeseriesbyclicks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/gettimeseriesbyclicksdeprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/gettoplinksbyclicks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/gettoplinksbyclicksdeprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/gettopurlsbyclicks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/gettopurlsbyclicksdeprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getworkspace.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getworkspaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/listdomains.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/setprimarydomain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/trackcustomer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/tracklead.py
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/tracksale.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/transferdomain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/updatedomain.py
--rw-r--r--   0 runner    (1001) docker     (127)     8566 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/updatelink.py
--rw-r--r--   0 runner    (1001) docker     (127)     8095 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/upsertlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/qr_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    17342 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    24875 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/track.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:07:05.686021 dub-0.0.5/src/dub/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32651 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24355 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/workspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:07:05.674021 dub-0.0.5/src/dub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17862 2024-05-21 19:07:05.000000 dub-0.0.5/src/dub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-21 19:07:05.000000 dub-0.0.5/src/dub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:07:05.000000 dub-0.0.5/src/dub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-21 19:07:05.000000 dub-0.0.5/src/dub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-21 19:07:05.000000 dub-0.0.5/src/dub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:13:44.638980 dub-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-29 17:13:29.000000 dub-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14630 2024-05-29 17:13:44.638980 dub-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-05-29 17:13:29.000000 dub-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 17:13:44.638980 dub-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-29 17:13:29.000000 dub-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:13:44.622979 dub-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:13:44.626979 dub-0.0.6/src/dub/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:13:44.626979 dub-0.0.6/src/dub/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9076 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52378 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/domains.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69591 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/metatags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:13:44.626979 dub-0.0.6/src/dub/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:13:44.634980 dub-0.0.6/src/dub/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/clicksbrowsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/clickscities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/clickscount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/clickscountries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/clicksdevices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/clicksos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/clicksreferers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/clickstimeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/clickstoplinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/clickstopurls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/countrycode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/domainschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/httpmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/leadsbrowsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/leadscities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/leadscount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/leadscountries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/leadsdevices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/leadsos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/leadsreferers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/leadstimeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/leadstoplinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/leadstopurls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41946 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/linkgeotargeting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50627 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/linkschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/salesbrowsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/salescities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/salescount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/salescountries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/salesdevices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/salesos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/salesreferers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/salestimeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/salestoplinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/salestopurls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/tagschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/workspaceschema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:13:44.634980 dub-0.0.6/src/dub/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/errors/badrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/errors/conflict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/errors/forbidden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/errors/internalservererror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/errors/inviteexpired.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/errors/notfound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/errors/ratelimitexceeded.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/errors/sdkerror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/errors/unauthorized.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/errors/unprocessableentity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:13:44.634980 dub-0.0.6/src/dub/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/internal/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:13:44.638980 dub-0.0.6/src/dub/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/adddomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8107 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/bulkcreatelinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8159 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/createlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/createtag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/createworkspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/deletedomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/deletelink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/getlinkinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/getlinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/getlinkscount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/getmetatags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/getqrcode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/gettags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/getworkspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/getworkspaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/listdomains.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10285 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/retrieveanalytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/setprimarydomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/trackcustomer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/tracklead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/tracksale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/transferdomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/updatedomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8671 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/updatelink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8200 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/upsertlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8384 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/qr_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17702 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25415 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/track.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:13:44.638980 dub-0.0.6/src/dub/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32701 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24895 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:13:44.626979 dub-0.0.6/src/dub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14630 2024-05-29 17:13:44.000000 dub-0.0.6/src/dub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-29 17:13:44.000000 dub-0.0.6/src/dub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 17:13:44.000000 dub-0.0.6/src/dub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-29 17:13:44.000000 dub-0.0.6/src/dub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-29 17:13:44.000000 dub-0.0.6/src/dub.egg-info/top_level.txt
```

### Comparing `dub-0.0.5/PKG-INFO` & `dub-0.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dub
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/dubinc/dub-python.git
 Author: Speakeasy
 License: UNKNOWN
 Description: # dub
         
         <div align="left">
@@ -41,14 +41,15 @@
         from dub.models import operations
         
         s = dub.Dub(
             token="DUB_API_KEY",
             workspace_id='<value>',
         )
         
+        
         res = s.links.create(request=operations.CreateLinkRequestBody(
             url='https://google/com',
             external_id='123456',
             tag_ids=[
                 'clux0rgak00011...',
             ],
         ))
@@ -66,14 +67,15 @@
         from dub.models import operations
         
         s = dub.Dub(
             token="DUB_API_KEY",
             workspace_id='<value>',
         )
         
+        
         res = s.links.upsert(request=operations.UpsertLinkRequestBody(
             url='https://google/com',
             external_id='123456',
             tag_ids=[
                 'clux0rgak00011...',
             ],
         ))
@@ -101,37 +103,15 @@
         
         ### [qr_codes](https://github.com/dubinc/dub-python/blob/master/docs/sdks/qrcodes/README.md)
         
         * [get](https://github.com/dubinc/dub-python/blob/master/docs/sdks/qrcodes/README.md#get) - Retrieve a QR code
         
         ### [analytics](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md)
         
-        * [~~timeseries~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#timeseries) - Retrieve timeseries click analytics :warning: **Deprecated** Use `timeseries` instead.
-        * [~~country~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#country) - Retrieve top countries by clicks :warning: **Deprecated** Use `countries` instead.
-        * [~~city~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#city) - Retrieve top cities by clicks :warning: **Deprecated** Use `cities` instead.
-        * [~~device~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#device) - Retrieve top devices by clicks :warning: **Deprecated** Use `devices` instead.
-        * [~~browser~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#browser) - Retrieve top browsers by clicks :warning: **Deprecated** Use `browsers` instead.
-        * [~~os~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#os) - Retrieve top OS by clicks :warning: **Deprecated** Use `os` instead.
-        * [~~referer~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#referer) - Retrieve top referers by clicks :warning: **Deprecated** Use `referers` instead.
-        * [~~top_links~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#top_links) - Retrieve top links by clicks :warning: **Deprecated** Use `top_links` instead.
-        * [~~top_urls~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#top_urls) - Retrieve top URLs by clicks :warning: **Deprecated** Use `top_urls` instead.
-        
-        ### [analytics.clicks](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md)
-        
-        * [count](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#count) - Retrieve the total clicks count
-        * [timeseries](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#timeseries) - Retrieve timeseries click analytics
-        * [countries](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#countries) - Retrieve top countries by clicks
-        * [cities](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#cities) - Retrieve top cities by clicks
-        * [devices](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#devices) - Retrieve top devices by clicks
-        * [browsers](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#browsers) - Retrieve top browsers by clicks
-        * [os](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#os) - Retrieve top OS by clicks
-        * [referers](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#referers) - Retrieve top referers by clicks
-        * [top_links](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#top_links) - Retrieve top links by clicks
-        * [top_urls](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#top_urls) - Retrieve top URLs by clicks
-        * [~~get_clicks_count_deprecated~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#get_clicks_count_deprecated) - Retrieve the total clicks count :warning: **Deprecated** Use `count` instead.
+        * [retrieve](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#retrieve) - Retrieve analytics for a link, a domain, or the authenticated workspace.
         
         ### [workspaces](https://github.com/dubinc/dub-python/blob/master/docs/sdks/workspaces/README.md)
         
         * [list](https://github.com/dubinc/dub-python/blob/master/docs/sdks/workspaces/README.md#list) - Retrieve a list of workspaces
         * [create](https://github.com/dubinc/dub-python/blob/master/docs/sdks/workspaces/README.md#create) - Create a workspace
         * [get](https://github.com/dubinc/dub-python/blob/master/docs/sdks/workspaces/README.md#get) - Retrieve a workspace
         
@@ -188,14 +168,15 @@
             token="DUB_API_KEY",
             workspace_id='<value>',
         )
         
         res = None
         try:
             res = s.links.list(request=operations.GetLinksRequest())
+        
         except errors.BadRequest as e:
             # handle exception
             raise(e)
         except errors.Unauthorized as e:
             # handle exception
             raise(e)
         except errors.Forbidden as e:
@@ -249,14 +230,15 @@
         
         s = dub.Dub(
             server_idx=0,
             token="DUB_API_KEY",
             workspace_id='<value>',
         )
         
+        
         res = s.links.list(request=operations.GetLinksRequest())
         
         if res.link_schemas is not None:
             # handle response
             pass
         
         ```
@@ -271,14 +253,15 @@
         
         s = dub.Dub(
             server_url="https://api.dub.co",
             token="DUB_API_KEY",
             workspace_id='<value>',
         )
         
+        
         res = s.links.list(request=operations.GetLinksRequest())
         
         if res.link_schemas is not None:
             # handle response
             pass
         
         ```
@@ -317,14 +300,15 @@
         from dub.models import operations
         
         s = dub.Dub(
             token="DUB_API_KEY",
             workspace_id='<value>',
         )
         
+        
         res = s.links.list(request=operations.GetLinksRequest())
         
         if res.link_schemas is not None:
             # handle response
             pass
         
         ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dub Version: 0.0.5 Summary: Python Client SDK
+Metadata-Version: 2.1 Name: dub Version: 0.0.6 Summary: Python Client SDK
 Generated by Speakeasy Home-page: https://github.com/dubinc/dub-python.git
 Author: Speakeasy License: UNKNOWN Description: # dub
 _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
 _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
 ## ð **Welcome to your new SDK!** ð It has been generated successfully
 based on your OpenAPI spec. However, it is not yet ready for production use.
@@ -36,82 +36,41 @@
 Update a link * [create_many](https://github.com/dubinc/dub-python/blob/master/
 docs/sdks/links/README.md#create_many) - Bulk create links * [upsert](https://
 github.com/dubinc/dub-python/blob/master/docs/sdks/links/README.md#upsert) -
 Upsert a link ### [qr_codes](https://github.com/dubinc/dub-python/blob/master/
 docs/sdks/qrcodes/README.md) * [get](https://github.com/dubinc/dub-python/blob/
 master/docs/sdks/qrcodes/README.md#get) - Retrieve a QR code ### [analytics]
 (https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/
-README.md) * [~~timeseries~~](https://github.com/dubinc/dub-python/blob/master/
-docs/sdks/analytics/README.md#timeseries) - Retrieve timeseries click analytics
-:warning: **Deprecated** Use `timeseries` instead. * [~~country~~](https://
-github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#country)
-- Retrieve top countries by clicks :warning: **Deprecated** Use `countries`
-instead. * [~~city~~](https://github.com/dubinc/dub-python/blob/master/docs/
-sdks/analytics/README.md#city) - Retrieve top cities by clicks :warning:
-**Deprecated** Use `cities` instead. * [~~device~~](https://github.com/dubinc/
-dub-python/blob/master/docs/sdks/analytics/README.md#device) - Retrieve top
-devices by clicks :warning: **Deprecated** Use `devices` instead. *
-[~~browser~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
-analytics/README.md#browser) - Retrieve top browsers by clicks :warning:
-**Deprecated** Use `browsers` instead. * [~~os~~](https://github.com/dubinc/
-dub-python/blob/master/docs/sdks/analytics/README.md#os) - Retrieve top OS by
-clicks :warning: **Deprecated** Use `os` instead. * [~~referer~~](https://
-github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#referer)
-- Retrieve top referers by clicks :warning: **Deprecated** Use `referers`
-instead. * [~~top_links~~](https://github.com/dubinc/dub-python/blob/master/
-docs/sdks/analytics/README.md#top_links) - Retrieve top links by clicks :
-warning: **Deprecated** Use `top_links` instead. * [~~top_urls~~](https://
-github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/
-README.md#top_urls) - Retrieve top URLs by clicks :warning: **Deprecated** Use
-`top_urls` instead. ### [analytics.clicks](https://github.com/dubinc/dub-
-python/blob/master/docs/sdks/clicks/README.md) * [count](https://github.com/
-dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#count) - Retrieve the
-total clicks count * [timeseries](https://github.com/dubinc/dub-python/blob/
-master/docs/sdks/clicks/README.md#timeseries) - Retrieve timeseries click
-analytics * [countries](https://github.com/dubinc/dub-python/blob/master/docs/
-sdks/clicks/README.md#countries) - Retrieve top countries by clicks * [cities]
-(https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/
-README.md#cities) - Retrieve top cities by clicks * [devices](https://
-github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#devices) -
-Retrieve top devices by clicks * [browsers](https://github.com/dubinc/dub-
-python/blob/master/docs/sdks/clicks/README.md#browsers) - Retrieve top browsers
-by clicks * [os](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
-clicks/README.md#os) - Retrieve top OS by clicks * [referers](https://
-github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#referers) -
-Retrieve top referers by clicks * [top_links](https://github.com/dubinc/dub-
-python/blob/master/docs/sdks/clicks/README.md#top_links) - Retrieve top links
-by clicks * [top_urls](https://github.com/dubinc/dub-python/blob/master/docs/
-sdks/clicks/README.md#top_urls) - Retrieve top URLs by clicks *
-[~~get_clicks_count_deprecated~~](https://github.com/dubinc/dub-python/blob/
-master/docs/sdks/clicks/README.md#get_clicks_count_deprecated) - Retrieve the
-total clicks count :warning: **Deprecated** Use `count` instead. ###
-[workspaces](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
-workspaces/README.md) * [list](https://github.com/dubinc/dub-python/blob/
-master/docs/sdks/workspaces/README.md#list) - Retrieve a list of workspaces *
-[create](https://github.com/dubinc/dub-python/blob/master/docs/sdks/workspaces/
-README.md#create) - Create a workspace * [get](https://github.com/dubinc/dub-
-python/blob/master/docs/sdks/workspaces/README.md#get) - Retrieve a workspace
-### [tags](https://github.com/dubinc/dub-python/blob/master/docs/sdks/tags/
-README.md) * [list](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
-tags/README.md#list) - Retrieve a list of tags * [create](https://github.com/
-dubinc/dub-python/blob/master/docs/sdks/tags/README.md#create) - Create a new
-tag ### [domains](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
-domains/README.md) * [list](https://github.com/dubinc/dub-python/blob/master/
-docs/sdks/domains/README.md#list) - Retrieve a list of domains * [add](https://
-github.com/dubinc/dub-python/blob/master/docs/sdks/domains/README.md#add) - Add
-a domain * [delete](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
-domains/README.md#delete) - Delete a domain * [update](https://github.com/
-dubinc/dub-python/blob/master/docs/sdks/domains/README.md#update) - Update a
-domain * [set_primary](https://github.com/dubinc/dub-python/blob/master/docs/
-sdks/domains/README.md#set_primary) - Set a domain as primary * [transfer]
-(https://github.com/dubinc/dub-python/blob/master/docs/sdks/domains/
-README.md#transfer) - Transfer a domain ### [track](https://github.com/dubinc/
-dub-python/blob/master/docs/sdks/track/README.md) * [lead](https://github.com/
-dubinc/dub-python/blob/master/docs/sdks/track/README.md#lead) - Track a lead *
-[sale](https://github.com/dubinc/dub-python/blob/master/docs/sdks/track/
+README.md) * [retrieve](https://github.com/dubinc/dub-python/blob/master/docs/
+sdks/analytics/README.md#retrieve) - Retrieve analytics for a link, a domain,
+or the authenticated workspace. ### [workspaces](https://github.com/dubinc/dub-
+python/blob/master/docs/sdks/workspaces/README.md) * [list](https://github.com/
+dubinc/dub-python/blob/master/docs/sdks/workspaces/README.md#list) - Retrieve a
+list of workspaces * [create](https://github.com/dubinc/dub-python/blob/master/
+docs/sdks/workspaces/README.md#create) - Create a workspace * [get](https://
+github.com/dubinc/dub-python/blob/master/docs/sdks/workspaces/README.md#get) -
+Retrieve a workspace ### [tags](https://github.com/dubinc/dub-python/blob/
+master/docs/sdks/tags/README.md) * [list](https://github.com/dubinc/dub-python/
+blob/master/docs/sdks/tags/README.md#list) - Retrieve a list of tags * [create]
+(https://github.com/dubinc/dub-python/blob/master/docs/sdks/tags/
+README.md#create) - Create a new tag ### [domains](https://github.com/dubinc/
+dub-python/blob/master/docs/sdks/domains/README.md) * [list](https://
+github.com/dubinc/dub-python/blob/master/docs/sdks/domains/README.md#list) -
+Retrieve a list of domains * [add](https://github.com/dubinc/dub-python/blob/
+master/docs/sdks/domains/README.md#add) - Add a domain * [delete](https://
+github.com/dubinc/dub-python/blob/master/docs/sdks/domains/README.md#delete) -
+Delete a domain * [update](https://github.com/dubinc/dub-python/blob/master/
+docs/sdks/domains/README.md#update) - Update a domain * [set_primary](https://
+github.com/dubinc/dub-python/blob/master/docs/sdks/domains/
+README.md#set_primary) - Set a domain as primary * [transfer](https://
+github.com/dubinc/dub-python/blob/master/docs/sdks/domains/README.md#transfer)
+- Transfer a domain ### [track](https://github.com/dubinc/dub-python/blob/
+master/docs/sdks/track/README.md) * [lead](https://github.com/dubinc/dub-
+python/blob/master/docs/sdks/track/README.md#lead) - Track a lead * [sale]
+(https://github.com/dubinc/dub-python/blob/master/docs/sdks/track/
 README.md#sale) - Track a sale * [customer](https://github.com/dubinc/dub-
 python/blob/master/docs/sdks/track/README.md#customer) - Track a customer ###
 [metatags](https://github.com/dubinc/dub-python/blob/master/docs/sdks/metatags/
 README.md) * [get](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
 metatags/README.md#get) - Retrieve the metatags for a URL ## Error Handling
 Handling errors in this SDK should largely match your expectations. All
 operations return a response object or raise an error. If Error objects are
```

### Comparing `dub-0.0.5/README.md` & `dub-0.0.6/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 from dub.models import operations
 
 s = dub.Dub(
     token="DUB_API_KEY",
     workspace_id='<value>',
 )
 
+
 res = s.links.create(request=operations.CreateLinkRequestBody(
     url='https://google/com',
     external_id='123456',
     tag_ids=[
         'clux0rgak00011...',
     ],
 ))
@@ -59,14 +60,15 @@
 from dub.models import operations
 
 s = dub.Dub(
     token="DUB_API_KEY",
     workspace_id='<value>',
 )
 
+
 res = s.links.upsert(request=operations.UpsertLinkRequestBody(
     url='https://google/com',
     external_id='123456',
     tag_ids=[
         'clux0rgak00011...',
     ],
 ))
@@ -94,37 +96,15 @@
 
 ### [qr_codes](docs/sdks/qrcodes/README.md)
 
 * [get](docs/sdks/qrcodes/README.md#get) - Retrieve a QR code
 
 ### [analytics](docs/sdks/analytics/README.md)
 
-* [~~timeseries~~](docs/sdks/analytics/README.md#timeseries) - Retrieve timeseries click analytics :warning: **Deprecated** Use `timeseries` instead.
-* [~~country~~](docs/sdks/analytics/README.md#country) - Retrieve top countries by clicks :warning: **Deprecated** Use `countries` instead.
-* [~~city~~](docs/sdks/analytics/README.md#city) - Retrieve top cities by clicks :warning: **Deprecated** Use `cities` instead.
-* [~~device~~](docs/sdks/analytics/README.md#device) - Retrieve top devices by clicks :warning: **Deprecated** Use `devices` instead.
-* [~~browser~~](docs/sdks/analytics/README.md#browser) - Retrieve top browsers by clicks :warning: **Deprecated** Use `browsers` instead.
-* [~~os~~](docs/sdks/analytics/README.md#os) - Retrieve top OS by clicks :warning: **Deprecated** Use `os` instead.
-* [~~referer~~](docs/sdks/analytics/README.md#referer) - Retrieve top referers by clicks :warning: **Deprecated** Use `referers` instead.
-* [~~top_links~~](docs/sdks/analytics/README.md#top_links) - Retrieve top links by clicks :warning: **Deprecated** Use `top_links` instead.
-* [~~top_urls~~](docs/sdks/analytics/README.md#top_urls) - Retrieve top URLs by clicks :warning: **Deprecated** Use `top_urls` instead.
-
-### [analytics.clicks](docs/sdks/clicks/README.md)
-
-* [count](docs/sdks/clicks/README.md#count) - Retrieve the total clicks count
-* [timeseries](docs/sdks/clicks/README.md#timeseries) - Retrieve timeseries click analytics
-* [countries](docs/sdks/clicks/README.md#countries) - Retrieve top countries by clicks
-* [cities](docs/sdks/clicks/README.md#cities) - Retrieve top cities by clicks
-* [devices](docs/sdks/clicks/README.md#devices) - Retrieve top devices by clicks
-* [browsers](docs/sdks/clicks/README.md#browsers) - Retrieve top browsers by clicks
-* [os](docs/sdks/clicks/README.md#os) - Retrieve top OS by clicks
-* [referers](docs/sdks/clicks/README.md#referers) - Retrieve top referers by clicks
-* [top_links](docs/sdks/clicks/README.md#top_links) - Retrieve top links by clicks
-* [top_urls](docs/sdks/clicks/README.md#top_urls) - Retrieve top URLs by clicks
-* [~~get_clicks_count_deprecated~~](docs/sdks/clicks/README.md#get_clicks_count_deprecated) - Retrieve the total clicks count :warning: **Deprecated** Use `count` instead.
+* [retrieve](docs/sdks/analytics/README.md#retrieve) - Retrieve analytics for a link, a domain, or the authenticated workspace.
 
 ### [workspaces](docs/sdks/workspaces/README.md)
 
 * [list](docs/sdks/workspaces/README.md#list) - Retrieve a list of workspaces
 * [create](docs/sdks/workspaces/README.md#create) - Create a workspace
 * [get](docs/sdks/workspaces/README.md#get) - Retrieve a workspace
 
@@ -181,14 +161,15 @@
     token="DUB_API_KEY",
     workspace_id='<value>',
 )
 
 res = None
 try:
     res = s.links.list(request=operations.GetLinksRequest())
+
 except errors.BadRequest as e:
     # handle exception
     raise(e)
 except errors.Unauthorized as e:
     # handle exception
     raise(e)
 except errors.Forbidden as e:
@@ -242,14 +223,15 @@
 
 s = dub.Dub(
     server_idx=0,
     token="DUB_API_KEY",
     workspace_id='<value>',
 )
 
+
 res = s.links.list(request=operations.GetLinksRequest())
 
 if res.link_schemas is not None:
     # handle response
     pass
 
 ```
@@ -264,14 +246,15 @@
 
 s = dub.Dub(
     server_url="https://api.dub.co",
     token="DUB_API_KEY",
     workspace_id='<value>',
 )
 
+
 res = s.links.list(request=operations.GetLinksRequest())
 
 if res.link_schemas is not None:
     # handle response
     pass
 
 ```
@@ -310,14 +293,15 @@
 from dub.models import operations
 
 s = dub.Dub(
     token="DUB_API_KEY",
     workspace_id='<value>',
 )
 
+
 res = s.links.list(request=operations.GetLinksRequest())
 
 if res.link_schemas is not None:
     # handle response
     pass
 
 ```
```

#### html2text {}

```diff
@@ -26,51 +26,23 @@
 Create a new link * [count](docs/sdks/links/README.md#count) - Retrieve the
 number of links * [get](docs/sdks/links/README.md#get) - Retrieve a link *
 [delete](docs/sdks/links/README.md#delete) - Delete a link * [update](docs/
 sdks/links/README.md#update) - Update a link * [create_many](docs/sdks/links/
 README.md#create_many) - Bulk create links * [upsert](docs/sdks/links/
 README.md#upsert) - Upsert a link ### [qr_codes](docs/sdks/qrcodes/README.md) *
 [get](docs/sdks/qrcodes/README.md#get) - Retrieve a QR code ### [analytics]
-(docs/sdks/analytics/README.md) * [~~timeseries~~](docs/sdks/analytics/
-README.md#timeseries) - Retrieve timeseries click analytics :warning:
-**Deprecated** Use `timeseries` instead. * [~~country~~](docs/sdks/analytics/
-README.md#country) - Retrieve top countries by clicks :warning: **Deprecated**
-Use `countries` instead. * [~~city~~](docs/sdks/analytics/README.md#city) -
-Retrieve top cities by clicks :warning: **Deprecated** Use `cities` instead. *
-[~~device~~](docs/sdks/analytics/README.md#device) - Retrieve top devices by
-clicks :warning: **Deprecated** Use `devices` instead. * [~~browser~~](docs/
-sdks/analytics/README.md#browser) - Retrieve top browsers by clicks :warning:
-**Deprecated** Use `browsers` instead. * [~~os~~](docs/sdks/analytics/
-README.md#os) - Retrieve top OS by clicks :warning: **Deprecated** Use `os`
-instead. * [~~referer~~](docs/sdks/analytics/README.md#referer) - Retrieve top
-referers by clicks :warning: **Deprecated** Use `referers` instead. *
-[~~top_links~~](docs/sdks/analytics/README.md#top_links) - Retrieve top links
-by clicks :warning: **Deprecated** Use `top_links` instead. * [~~top_urls~~]
-(docs/sdks/analytics/README.md#top_urls) - Retrieve top URLs by clicks :
-warning: **Deprecated** Use `top_urls` instead. ### [analytics.clicks](docs/
-sdks/clicks/README.md) * [count](docs/sdks/clicks/README.md#count) - Retrieve
-the total clicks count * [timeseries](docs/sdks/clicks/README.md#timeseries) -
-Retrieve timeseries click analytics * [countries](docs/sdks/clicks/
-README.md#countries) - Retrieve top countries by clicks * [cities](docs/sdks/
-clicks/README.md#cities) - Retrieve top cities by clicks * [devices](docs/sdks/
-clicks/README.md#devices) - Retrieve top devices by clicks * [browsers](docs/
-sdks/clicks/README.md#browsers) - Retrieve top browsers by clicks * [os](docs/
-sdks/clicks/README.md#os) - Retrieve top OS by clicks * [referers](docs/sdks/
-clicks/README.md#referers) - Retrieve top referers by clicks * [top_links]
-(docs/sdks/clicks/README.md#top_links) - Retrieve top links by clicks *
-[top_urls](docs/sdks/clicks/README.md#top_urls) - Retrieve top URLs by clicks *
-[~~get_clicks_count_deprecated~~](docs/sdks/clicks/
-README.md#get_clicks_count_deprecated) - Retrieve the total clicks count :
-warning: **Deprecated** Use `count` instead. ### [workspaces](docs/sdks/
-workspaces/README.md) * [list](docs/sdks/workspaces/README.md#list) - Retrieve
-a list of workspaces * [create](docs/sdks/workspaces/README.md#create) - Create
-a workspace * [get](docs/sdks/workspaces/README.md#get) - Retrieve a workspace
-### [tags](docs/sdks/tags/README.md) * [list](docs/sdks/tags/README.md#list) -
-Retrieve a list of tags * [create](docs/sdks/tags/README.md#create) - Create a
-new tag ### [domains](docs/sdks/domains/README.md) * [list](docs/sdks/domains/
+(docs/sdks/analytics/README.md) * [retrieve](docs/sdks/analytics/
+README.md#retrieve) - Retrieve analytics for a link, a domain, or the
+authenticated workspace. ### [workspaces](docs/sdks/workspaces/README.md) *
+[list](docs/sdks/workspaces/README.md#list) - Retrieve a list of workspaces *
+[create](docs/sdks/workspaces/README.md#create) - Create a workspace * [get]
+(docs/sdks/workspaces/README.md#get) - Retrieve a workspace ### [tags](docs/
+sdks/tags/README.md) * [list](docs/sdks/tags/README.md#list) - Retrieve a list
+of tags * [create](docs/sdks/tags/README.md#create) - Create a new tag ###
+[domains](docs/sdks/domains/README.md) * [list](docs/sdks/domains/
 README.md#list) - Retrieve a list of domains * [add](docs/sdks/domains/
 README.md#add) - Add a domain * [delete](docs/sdks/domains/README.md#delete) -
 Delete a domain * [update](docs/sdks/domains/README.md#update) - Update a
 domain * [set_primary](docs/sdks/domains/README.md#set_primary) - Set a domain
 as primary * [transfer](docs/sdks/domains/README.md#transfer) - Transfer a
 domain ### [track](docs/sdks/track/README.md) * [lead](docs/sdks/track/
 README.md#lead) - Track a lead * [sale](docs/sdks/track/README.md#sale) - Track
```

### Comparing `dub-0.0.5/setup.py` & `dub-0.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='dub',
-    version='0.0.5',
+    version='0.0.6',
     author='Speakeasy',
     description='Python Client SDK Generated by Speakeasy',
     url='https://github.com/dubinc/dub-python.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `dub-0.0.5/src/dub/_hooks/registration.py` & `dub-0.0.6/src/dub/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.5/src/dub/_hooks/sdkhooks.py` & `dub-0.0.6/src/dub/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.5/src/dub/_hooks/types.py` & `dub-0.0.6/src/dub/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.5/src/dub/analytics.py` & `dub-0.0.6/src/dub/links.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,37 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
-from .clicks import Clicks
 from .sdkconfiguration import SDKConfiguration
 from dub import utils
 from dub._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from dub.models import components, errors, operations
 from typing import List, Optional
 
-class Analytics:
-    clicks: Clicks
+class Links:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
-        self._init_sdks()
-    
-    def _init_sdks(self):
-        self.clicks = Clicks(self.sdk_configuration)
         
     
     
-    def timeseries(self, request: operations.GetTimeseriesByClicksDeprecatedRequest) -> operations.GetTimeseriesByClicksDeprecatedResponse:
-        r"""Retrieve timeseries click analytics
-        Retrieve timeseries click analytics for a link, a domain, or the authenticated workspace over a period of time.
-
-        Deprecated method: This method is deprecated. Use dub.analytics.clicks.timeseries instead.. Use timeseries instead.
+    def list(self, request: operations.GetLinksRequest) -> operations.GetLinksResponse:
+        r"""Retrieve a list of links
+        Retrieve a list of links for the authenticated workspace. The list will be paginated and the provided query parameters allow filtering the returned links.
         """
-        hook_ctx = HookContext(operation_id='getTimeseriesByClicksDeprecated', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.GetTimeseriesByClicksDeprecatedGlobals(
+        hook_ctx = HookContext(operation_id='getLinks', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        _globals = operations.GetLinksGlobals(
             workspace_id=self.sdk_configuration.globals.workspace_id,
             project_slug=self.sdk_configuration.globals.project_slug,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/analytics/timeseries', request, _globals)
+        url = utils.generate_url(base_url, '/links', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
@@ -64,134 +56,135 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetTimeseriesByClicksDeprecatedResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
+        res = operations.GetLinksResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetTimeseriesByClicksDeprecatedResponseBody]])
-                res.response_bodies = out
+                out = utils.unmarshal_json(http_res.text, Optional[List[components.LinkSchema]])
+                res.link_schemas = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequest)
+                out = utils.unmarshal_json(http_res.text, errors.BadRequest, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Unauthorized)
+                out = utils.unmarshal_json(http_res.text, errors.Unauthorized, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 403:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Forbidden)
+                out = utils.unmarshal_json(http_res.text, errors.Forbidden, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 404:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.NotFound)
+                out = utils.unmarshal_json(http_res.text, errors.NotFound, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 409:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Conflict)
+                out = utils.unmarshal_json(http_res.text, errors.Conflict, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 410:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InviteExpired)
+                out = utils.unmarshal_json(http_res.text, errors.InviteExpired, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 422:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity)
+                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 429:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded)
+                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 500:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InternalServerError)
+                out = utils.unmarshal_json(http_res.text, errors.InternalServerError, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def country(self, request: operations.GetCountriesByClicksDeprecatedRequest) -> operations.GetCountriesByClicksDeprecatedResponse:
-        r"""Retrieve top countries by clicks
-        Retrieve the top countries by number of clicks for a link, a domain, or the authenticated workspace.
-
-        Deprecated method: This method is deprecated. Use dub.analytics.clicks.countries instead.. Use countries instead.
+    def create(self, request: Optional[operations.CreateLinkRequestBody] = None) -> operations.CreateLinkResponse:
+        r"""Create a new link
+        Create a new link for the authenticated workspace.
         """
-        hook_ctx = HookContext(operation_id='getCountriesByClicksDeprecated', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.GetCountriesByClicksDeprecatedGlobals(
+        hook_ctx = HookContext(operation_id='createLink', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        _globals = operations.CreateLinkGlobals(
             workspace_id=self.sdk_configuration.globals.workspace_id,
             project_slug=self.sdk_configuration.globals.project_slug,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/analytics/country', request, _globals)
+        url = utils.generate_url(base_url, '/links', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
+        req_content_type, data, form = utils.serialize_request_body(request, Optional[operations.CreateLinkRequestBody], "request", False, True, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
@@ -202,120 +195,118 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetCountriesByClicksDeprecatedResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
+        res = operations.CreateLinkResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[components.ClicksByCountry]])
-                res.clicks_by_countries = out
+                out = utils.unmarshal_json(http_res.text, Optional[components.LinkSchema])
+                res.link_schema = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequest)
+                out = utils.unmarshal_json(http_res.text, errors.BadRequest, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Unauthorized)
+                out = utils.unmarshal_json(http_res.text, errors.Unauthorized, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 403:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Forbidden)
+                out = utils.unmarshal_json(http_res.text, errors.Forbidden, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 404:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.NotFound)
+                out = utils.unmarshal_json(http_res.text, errors.NotFound, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 409:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Conflict)
+                out = utils.unmarshal_json(http_res.text, errors.Conflict, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 410:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InviteExpired)
+                out = utils.unmarshal_json(http_res.text, errors.InviteExpired, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 422:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity)
+                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 429:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded)
+                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 500:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InternalServerError)
+                out = utils.unmarshal_json(http_res.text, errors.InternalServerError, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def city(self, request: operations.GetCitiesByClicksDeprecatedRequest) -> operations.GetCitiesByClicksDeprecatedResponse:
-        r"""Retrieve top cities by clicks
-        Retrieve the top countries by number of clicks for a link, a domain, or the authenticated workspace.
-
-        Deprecated method: This method is deprecated. Use dub.analytics.clicks.cities instead.. Use cities instead.
+    def count(self, request: operations.GetLinksCountRequest) -> operations.GetLinksCountResponse:
+        r"""Retrieve the number of links
+        Retrieve the number of links for the authenticated workspace. The provided query parameters allow filtering the returned links.
         """
-        hook_ctx = HookContext(operation_id='getCitiesByClicksDeprecated', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.GetCitiesByClicksDeprecatedGlobals(
+        hook_ctx = HookContext(operation_id='getLinksCount', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        _globals = operations.GetLinksCountGlobals(
             workspace_id=self.sdk_configuration.globals.workspace_id,
             project_slug=self.sdk_configuration.globals.project_slug,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/analytics/city', request, _globals)
+        url = utils.generate_url(base_url, '/links/count', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
@@ -340,258 +331,125 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetCitiesByClicksDeprecatedResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
+        res = operations.GetLinksCountResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[components.ClicksByCities]])
-                res.clicks_by_cities = out
+                out = utils.unmarshal_json(http_res.text, Optional[float])
+                res.number = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequest)
+                out = utils.unmarshal_json(http_res.text, errors.BadRequest, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Unauthorized)
+                out = utils.unmarshal_json(http_res.text, errors.Unauthorized, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 403:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Forbidden)
+                out = utils.unmarshal_json(http_res.text, errors.Forbidden, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 404:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.NotFound)
+                out = utils.unmarshal_json(http_res.text, errors.NotFound, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 409:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Conflict)
+                out = utils.unmarshal_json(http_res.text, errors.Conflict, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 410:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InviteExpired)
+                out = utils.unmarshal_json(http_res.text, errors.InviteExpired, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 422:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity)
+                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 429:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded)
+                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 500:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InternalServerError)
+                out = utils.unmarshal_json(http_res.text, errors.InternalServerError, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def device(self, request: operations.GetDevicesByClicksDeprecatedRequest) -> operations.GetDevicesByClicksDeprecatedResponse:
-        r"""Retrieve top devices by clicks
-        Retrieve the top devices by number of clicks for a link, a domain, or the authenticated workspace.
-
-        Deprecated method: This method is deprecated. Use dub.analytics.clicks.devices instead.. Use devices instead.
+    def get(self, domain: Optional[str] = None, key: Optional[str] = None, link_id: Optional[str] = None, external_id: Optional[str] = None) -> operations.GetLinkInfoResponse:
+        r"""Retrieve a link
+        Retrieve the info for a link.
         """
-        hook_ctx = HookContext(operation_id='getDevicesByClicksDeprecated', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.GetDevicesByClicksDeprecatedGlobals(
-            workspace_id=self.sdk_configuration.globals.workspace_id,
-            project_slug=self.sdk_configuration.globals.project_slug,
+        hook_ctx = HookContext(operation_id='getLinkInfo', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.GetLinkInfoRequest(
+            domain=domain,
+            key=key,
+            link_id=link_id,
+            external_id=external_id,
         )
         
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
-        
-        url = utils.generate_url(base_url, '/analytics/device', request, _globals)
-        
-        if callable(self.sdk_configuration.security):
-            headers, query_params = utils.get_security(self.sdk_configuration.security())
-        else:
-            headers, query_params = utils.get_security(self.sdk_configuration.security)
-        
-        headers = { **utils.get_headers(request, _globals), **headers }
-        query_params = { **utils.get_query_params(request, _globals), **query_params }
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
-        client = self.sdk_configuration.client
-        
-        try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
-            http_res = client.send(req)
-        except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
-
-        if utils.match_status_codes(['400','401','403','404','409','410','422','429','4XX','500','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
-                raise e
-            if result is not None:
-                http_res = result
-        else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
-        
-        
-        res = operations.GetDevicesByClicksDeprecatedResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
-        
-        if http_res.status_code == 200:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetDevicesByClicksDeprecatedResponseBody]])
-                res.response_bodies = out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 400:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequest)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 401:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Unauthorized)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 403:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Forbidden)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 404:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.NotFound)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 409:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Conflict)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 410:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InviteExpired)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 422:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 429:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 500:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InternalServerError)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        else:
-            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
-
-        return res
-
-    
-    
-    def browser(self, request: operations.GetBrowsersByClicksDeprecatedRequest) -> operations.GetBrowsersByClicksDeprecatedResponse:
-        r"""Retrieve top browsers by clicks
-        Retrieve the top browsers by number of clicks for a link, a domain, or the authenticated workspace.
-
-        Deprecated method: This method is deprecated. Use dub.analytics.clicks.browsers instead.. Use browsers instead.
-        """
-        hook_ctx = HookContext(operation_id='getBrowsersByClicksDeprecated', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.GetBrowsersByClicksDeprecatedGlobals(
+        _globals = operations.GetLinkInfoGlobals(
             workspace_id=self.sdk_configuration.globals.workspace_id,
             project_slug=self.sdk_configuration.globals.project_slug,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/analytics/browser', request, _globals)
+        url = utils.generate_url(base_url, '/links/info', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
@@ -616,134 +474,136 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetBrowsersByClicksDeprecatedResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
+        res = operations.GetLinkInfoResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetBrowsersByClicksDeprecatedResponseBody]])
-                res.response_bodies = out
+                out = utils.unmarshal_json(http_res.text, Optional[components.LinkSchema])
+                res.link_schema = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequest)
+                out = utils.unmarshal_json(http_res.text, errors.BadRequest, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Unauthorized)
+                out = utils.unmarshal_json(http_res.text, errors.Unauthorized, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 403:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Forbidden)
+                out = utils.unmarshal_json(http_res.text, errors.Forbidden, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 404:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.NotFound)
+                out = utils.unmarshal_json(http_res.text, errors.NotFound, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 409:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Conflict)
+                out = utils.unmarshal_json(http_res.text, errors.Conflict, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 410:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InviteExpired)
+                out = utils.unmarshal_json(http_res.text, errors.InviteExpired, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 422:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity)
+                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 429:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded)
+                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 500:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InternalServerError)
+                out = utils.unmarshal_json(http_res.text, errors.InternalServerError, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def os(self, request: operations.GetOSByClicksDeprecatedRequest) -> operations.GetOSByClicksDeprecatedResponse:
-        r"""Retrieve top OS by clicks
-        Retrieve the top OS by number of clicks for a link, a domain, or the authenticated workspace.
-
-        Deprecated method: This method is deprecated. Use dub.analytics.clicks.os instead.. Use os instead.
+    def delete(self, link_id: str) -> operations.DeleteLinkResponse:
+        r"""Delete a link
+        Delete a link for the authenticated workspace.
         """
-        hook_ctx = HookContext(operation_id='getOSByClicksDeprecated', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.GetOSByClicksDeprecatedGlobals(
+        hook_ctx = HookContext(operation_id='deleteLink', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.DeleteLinkRequest(
+            link_id=link_id,
+        )
+        
+        _globals = operations.DeleteLinkGlobals(
             workspace_id=self.sdk_configuration.globals.workspace_id,
             project_slug=self.sdk_configuration.globals.project_slug,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/analytics/os', request, _globals)
+        url = utils.generate_url(base_url, '/links/{linkId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
@@ -754,134 +614,140 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetOSByClicksDeprecatedResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
+        res = operations.DeleteLinkResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetOSByClicksDeprecatedResponseBody]])
-                res.response_bodies = out
+                out = utils.unmarshal_json(http_res.text, Optional[operations.DeleteLinkResponseBody])
+                res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequest)
+                out = utils.unmarshal_json(http_res.text, errors.BadRequest, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Unauthorized)
+                out = utils.unmarshal_json(http_res.text, errors.Unauthorized, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 403:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Forbidden)
+                out = utils.unmarshal_json(http_res.text, errors.Forbidden, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 404:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.NotFound)
+                out = utils.unmarshal_json(http_res.text, errors.NotFound, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 409:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Conflict)
+                out = utils.unmarshal_json(http_res.text, errors.Conflict, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 410:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InviteExpired)
+                out = utils.unmarshal_json(http_res.text, errors.InviteExpired, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 422:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity)
+                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 429:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded)
+                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 500:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InternalServerError)
+                out = utils.unmarshal_json(http_res.text, errors.InternalServerError, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def referer(self, request: operations.GetReferersByClicksDeprecatedRequest) -> operations.GetReferersByClicksDeprecatedResponse:
-        r"""Retrieve top referers by clicks
-        Retrieve the top referers by number of clicks for a link, a domain, or the authenticated workspace.
-
-        Deprecated method: This method is deprecated. Use dub.analytics.clicks.referers instead.. Use referers instead.
+    def update(self, link_id: str, request_body: Optional[operations.UpdateLinkRequestBody] = None) -> operations.UpdateLinkResponse:
+        r"""Update a link
+        Update a link for the authenticated workspace. If there's no change, returns it as it is.
         """
-        hook_ctx = HookContext(operation_id='getReferersByClicksDeprecated', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.GetReferersByClicksDeprecatedGlobals(
+        hook_ctx = HookContext(operation_id='updateLink', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.UpdateLinkRequest(
+            link_id=link_id,
+            request_body=request_body,
+        )
+        
+        _globals = operations.UpdateLinkGlobals(
             workspace_id=self.sdk_configuration.globals.workspace_id,
             project_slug=self.sdk_configuration.globals.project_slug,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/analytics/referer', request, _globals)
+        url = utils.generate_url(base_url, '/links/{linkId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
+        req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateLinkRequest, "request_body", False, True, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = client.prepare_request(requests_http.Request('PATCH', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
@@ -892,134 +758,135 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetReferersByClicksDeprecatedResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
+        res = operations.UpdateLinkResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetReferersByClicksDeprecatedResponseBody]])
-                res.response_bodies = out
+                out = utils.unmarshal_json(http_res.text, Optional[components.LinkSchema])
+                res.link_schema = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequest)
+                out = utils.unmarshal_json(http_res.text, errors.BadRequest, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Unauthorized)
+                out = utils.unmarshal_json(http_res.text, errors.Unauthorized, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 403:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Forbidden)
+                out = utils.unmarshal_json(http_res.text, errors.Forbidden, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 404:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.NotFound)
+                out = utils.unmarshal_json(http_res.text, errors.NotFound, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 409:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Conflict)
+                out = utils.unmarshal_json(http_res.text, errors.Conflict, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 410:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InviteExpired)
+                out = utils.unmarshal_json(http_res.text, errors.InviteExpired, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 422:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity)
+                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 429:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded)
+                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 500:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InternalServerError)
+                out = utils.unmarshal_json(http_res.text, errors.InternalServerError, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def top_links(self, request: operations.GetTopLinksByClicksDeprecatedRequest) -> operations.GetTopLinksByClicksDeprecatedResponse:
-        r"""Retrieve top links by clicks
-        Retrieve the top links by number of clicks for a domain or the authenticated workspace.
-
-        Deprecated method: This method is deprecated. Use dub.analytics.clicks.topLinks instead.. Use top_links instead.
+    def create_many(self, request: Optional[List[operations.RequestBody]] = None) -> operations.BulkCreateLinksResponse:
+        r"""Bulk create links
+        Bulk create up to 100 links for the authenticated workspace.
         """
-        hook_ctx = HookContext(operation_id='getTopLinksByClicksDeprecated', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.GetTopLinksByClicksDeprecatedGlobals(
+        hook_ctx = HookContext(operation_id='bulkCreateLinks', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        _globals = operations.BulkCreateLinksGlobals(
             workspace_id=self.sdk_configuration.globals.workspace_id,
             project_slug=self.sdk_configuration.globals.project_slug,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/analytics/top_links', request, _globals)
+        url = utils.generate_url(base_url, '/links/bulk', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
+        req_content_type, data, form = utils.serialize_request_body(request, Optional[List[operations.RequestBody]], "request", False, True, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
@@ -1030,134 +897,135 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetTopLinksByClicksDeprecatedResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
+        res = operations.BulkCreateLinksResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetTopLinksByClicksDeprecatedResponseBody]])
-                res.response_bodies = out
+                out = utils.unmarshal_json(http_res.text, Optional[List[components.LinkSchema]])
+                res.link_schemas = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequest)
+                out = utils.unmarshal_json(http_res.text, errors.BadRequest, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Unauthorized)
+                out = utils.unmarshal_json(http_res.text, errors.Unauthorized, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 403:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Forbidden)
+                out = utils.unmarshal_json(http_res.text, errors.Forbidden, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 404:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.NotFound)
+                out = utils.unmarshal_json(http_res.text, errors.NotFound, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 409:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Conflict)
+                out = utils.unmarshal_json(http_res.text, errors.Conflict, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 410:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InviteExpired)
+                out = utils.unmarshal_json(http_res.text, errors.InviteExpired, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 422:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity)
+                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 429:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded)
+                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 500:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InternalServerError)
+                out = utils.unmarshal_json(http_res.text, errors.InternalServerError, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def top_urls(self, request: operations.GetTopURLsByClicksDeprecatedRequest) -> operations.GetTopURLsByClicksDeprecatedResponse:
-        r"""Retrieve top URLs by clicks
-        Retrieve the top URLs by number of clicks for a given short link.
-
-        Deprecated method: This method is deprecated. Use dub.analytics.clicks.topUrls instead.. Use top_urls instead.
+    def upsert(self, request: Optional[operations.UpsertLinkRequestBody] = None) -> operations.UpsertLinkResponse:
+        r"""Upsert a link
+        Upsert a link for the authenticated workspace by its URL. If a link with the same URL already exists, return it (or update it if there are any changes). Otherwise, a new link will be created.
         """
-        hook_ctx = HookContext(operation_id='getTopURLsByClicksDeprecated', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.GetTopURLsByClicksDeprecatedGlobals(
+        hook_ctx = HookContext(operation_id='upsertLink', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        _globals = operations.UpsertLinkGlobals(
             workspace_id=self.sdk_configuration.globals.workspace_id,
             project_slug=self.sdk_configuration.globals.project_slug,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/analytics/top_urls', request, _globals)
+        url = utils.generate_url(base_url, '/links/upsert', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
+        req_content_type, data, form = utils.serialize_request_body(request, Optional[operations.UpsertLinkRequestBody], "request", False, True, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
@@ -1168,94 +1036,94 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetTopURLsByClicksDeprecatedResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
+        res = operations.UpsertLinkResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetTopURLsByClicksDeprecatedResponseBody]])
-                res.response_bodies = out
+                out = utils.unmarshal_json(http_res.text, Optional[components.LinkSchema])
+                res.link_schema = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequest)
+                out = utils.unmarshal_json(http_res.text, errors.BadRequest, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Unauthorized)
+                out = utils.unmarshal_json(http_res.text, errors.Unauthorized, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 403:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Forbidden)
+                out = utils.unmarshal_json(http_res.text, errors.Forbidden, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 404:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.NotFound)
+                out = utils.unmarshal_json(http_res.text, errors.NotFound, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 409:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Conflict)
+                out = utils.unmarshal_json(http_res.text, errors.Conflict, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 410:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InviteExpired)
+                out = utils.unmarshal_json(http_res.text, errors.InviteExpired, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 422:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity)
+                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 429:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded)
+                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 500:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InternalServerError)
+                out = utils.unmarshal_json(http_res.text, errors.InternalServerError, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
```

### Comparing `dub-0.0.5/src/dub/clicks.py` & `dub-0.0.6/src/dub/domains.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,171 +3,38 @@
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from dub import utils
 from dub._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from dub.models import components, errors, operations
 from typing import List, Optional
 
-class Clicks:
+class Domains:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def count(self, request: operations.GetClicksCountRequest) -> operations.GetClicksCountResponse:
-        r"""Retrieve the total clicks count
-        Retrieve the total number of clicks for a link, a domain, or the authenticated workspace.
+    def list(self) -> operations.ListDomainsResponse:
+        r"""Retrieve a list of domains
+        Retrieve a list of domains associated with the authenticated workspace.
         """
-        hook_ctx = HookContext(operation_id='getClicksCount', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.GetClicksCountGlobals(
-            workspace_id=self.sdk_configuration.globals.workspace_id,
-            project_slug=self.sdk_configuration.globals.project_slug,
+        hook_ctx = HookContext(operation_id='listDomains', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.ListDomainsRequest(
         )
         
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
-        
-        url = utils.generate_url(base_url, '/analytics/clicks/count', request, _globals)
-        
-        if callable(self.sdk_configuration.security):
-            headers, query_params = utils.get_security(self.sdk_configuration.security())
-        else:
-            headers, query_params = utils.get_security(self.sdk_configuration.security)
-        
-        headers = { **utils.get_headers(request, _globals), **headers }
-        query_params = { **utils.get_query_params(request, _globals), **query_params }
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
-        client = self.sdk_configuration.client
-        
-        try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
-            http_res = client.send(req)
-        except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
-
-        if utils.match_status_codes(['400','401','403','404','409','410','422','429','4XX','500','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
-                raise e
-            if result is not None:
-                http_res = result
-        else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
-        
-        
-        res = operations.GetClicksCountResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
-        
-        if http_res.status_code == 200:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[float])
-                res.number = out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 400:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequest)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 401:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Unauthorized)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 403:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Forbidden)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 404:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.NotFound)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 409:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Conflict)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 410:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InviteExpired)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 422:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 429:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 500:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InternalServerError)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        else:
-            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
-
-        return res
-
-    
-    
-    def timeseries(self, request: operations.GetTimeseriesByClicksRequest) -> operations.GetTimeseriesByClicksResponse:
-        r"""Retrieve timeseries click analytics
-        Retrieve timeseries click analytics for a link, a domain, or the authenticated workspace over a period of time.
-        """
-        hook_ctx = HookContext(operation_id='getTimeseriesByClicks', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.GetTimeseriesByClicksGlobals(
+        _globals = operations.ListDomainsGlobals(
             workspace_id=self.sdk_configuration.globals.workspace_id,
             project_slug=self.sdk_configuration.globals.project_slug,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/analytics/clicks/timeseries', request, _globals)
+        url = utils.generate_url(base_url, '/domains', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
@@ -192,132 +59,135 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetTimeseriesByClicksResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
+        res = operations.ListDomainsResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[operations.ResponseBody]])
-                res.response_bodies = out
+                out = utils.unmarshal_json(http_res.text, Optional[List[components.DomainSchema]])
+                res.domain_schemas = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequest)
+                out = utils.unmarshal_json(http_res.text, errors.BadRequest, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Unauthorized)
+                out = utils.unmarshal_json(http_res.text, errors.Unauthorized, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 403:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Forbidden)
+                out = utils.unmarshal_json(http_res.text, errors.Forbidden, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 404:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.NotFound)
+                out = utils.unmarshal_json(http_res.text, errors.NotFound, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 409:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Conflict)
+                out = utils.unmarshal_json(http_res.text, errors.Conflict, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 410:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InviteExpired)
+                out = utils.unmarshal_json(http_res.text, errors.InviteExpired, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 422:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity)
+                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 429:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded)
+                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 500:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InternalServerError)
+                out = utils.unmarshal_json(http_res.text, errors.InternalServerError, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def countries(self, request: operations.GetCountriesByClicksRequest) -> operations.GetCountriesByClicksResponse:
-        r"""Retrieve top countries by clicks
-        Retrieve the top countries by number of clicks for a link, a domain, or the authenticated workspace.
+    def add(self, request: Optional[operations.AddDomainRequestBody] = None) -> operations.AddDomainResponse:
+        r"""Add a domain
+        Add a domain to the authenticated workspace.
         """
-        hook_ctx = HookContext(operation_id='getCountriesByClicks', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.GetCountriesByClicksGlobals(
+        hook_ctx = HookContext(operation_id='addDomain', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        _globals = operations.AddDomainGlobals(
             workspace_id=self.sdk_configuration.globals.workspace_id,
             project_slug=self.sdk_configuration.globals.project_slug,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/analytics/clicks/countries', request, _globals)
+        url = utils.generate_url(base_url, '/domains', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
+        req_content_type, data, form = utils.serialize_request_body(request, Optional[operations.AddDomainRequestBody], "request", False, True, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
@@ -328,268 +198,136 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetCountriesByClicksResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
+        res = operations.AddDomainResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
-        if http_res.status_code == 200:
+        if http_res.status_code == 201:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[components.ClicksByCountry]])
-                res.clicks_by_countries = out
+                out = utils.unmarshal_json(http_res.text, Optional[components.DomainSchema])
+                res.domain_schema = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequest)
+                out = utils.unmarshal_json(http_res.text, errors.BadRequest, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Unauthorized)
+                out = utils.unmarshal_json(http_res.text, errors.Unauthorized, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 403:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Forbidden)
+                out = utils.unmarshal_json(http_res.text, errors.Forbidden, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 404:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.NotFound)
+                out = utils.unmarshal_json(http_res.text, errors.NotFound, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 409:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Conflict)
+                out = utils.unmarshal_json(http_res.text, errors.Conflict, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 410:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InviteExpired)
+                out = utils.unmarshal_json(http_res.text, errors.InviteExpired, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 422:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity)
+                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 429:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded)
+                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 500:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InternalServerError)
+                out = utils.unmarshal_json(http_res.text, errors.InternalServerError, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def cities(self, request: operations.GetCitiesByClicksRequest) -> operations.GetCitiesByClicksResponse:
-        r"""Retrieve top cities by clicks
-        Retrieve the top countries by number of clicks for a link, a domain, or the authenticated workspace.
+    def delete(self, slug: str) -> operations.DeleteDomainResponse:
+        r"""Delete a domain
+        Delete a domain from a workspace. It cannot be undone. This will also delete all the links associated with the domain.
         """
-        hook_ctx = HookContext(operation_id='getCitiesByClicks', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.GetCitiesByClicksGlobals(
-            workspace_id=self.sdk_configuration.globals.workspace_id,
-            project_slug=self.sdk_configuration.globals.project_slug,
+        hook_ctx = HookContext(operation_id='deleteDomain', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.DeleteDomainRequest(
+            slug=slug,
         )
         
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
-        
-        url = utils.generate_url(base_url, '/analytics/clicks/cities', request, _globals)
-        
-        if callable(self.sdk_configuration.security):
-            headers, query_params = utils.get_security(self.sdk_configuration.security())
-        else:
-            headers, query_params = utils.get_security(self.sdk_configuration.security)
-        
-        headers = { **utils.get_headers(request, _globals), **headers }
-        query_params = { **utils.get_query_params(request, _globals), **query_params }
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
-        client = self.sdk_configuration.client
-        
-        try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
-            http_res = client.send(req)
-        except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
-
-        if utils.match_status_codes(['400','401','403','404','409','410','422','429','4XX','500','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
-                raise e
-            if result is not None:
-                http_res = result
-        else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
-        
-        
-        res = operations.GetCitiesByClicksResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
-        
-        if http_res.status_code == 200:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[components.ClicksByCities]])
-                res.clicks_by_cities = out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 400:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequest)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 401:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Unauthorized)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 403:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Forbidden)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 404:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.NotFound)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 409:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Conflict)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 410:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InviteExpired)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 422:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 429:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 500:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InternalServerError)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        else:
-            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
-
-        return res
-
-    
-    
-    def devices(self, request: operations.GetDevicesByClicksRequest) -> operations.GetDevicesByClicksResponse:
-        r"""Retrieve top devices by clicks
-        Retrieve the top devices by number of clicks for a link, a domain, or the authenticated workspace.
-        """
-        hook_ctx = HookContext(operation_id='getDevicesByClicks', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.GetDevicesByClicksGlobals(
+        _globals = operations.DeleteDomainGlobals(
             workspace_id=self.sdk_configuration.globals.workspace_id,
             project_slug=self.sdk_configuration.globals.project_slug,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/analytics/clicks/devices', request, _globals)
+        url = utils.generate_url(base_url, '/domains/{slug}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
@@ -600,268 +338,140 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetDevicesByClicksResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
+        res = operations.DeleteDomainResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetDevicesByClicksResponseBody]])
-                res.response_bodies = out
+                out = utils.unmarshal_json(http_res.text, Optional[operations.DeleteDomainResponseBody])
+                res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequest)
+                out = utils.unmarshal_json(http_res.text, errors.BadRequest, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Unauthorized)
+                out = utils.unmarshal_json(http_res.text, errors.Unauthorized, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 403:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Forbidden)
+                out = utils.unmarshal_json(http_res.text, errors.Forbidden, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 404:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.NotFound)
+                out = utils.unmarshal_json(http_res.text, errors.NotFound, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 409:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Conflict)
+                out = utils.unmarshal_json(http_res.text, errors.Conflict, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 410:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InviteExpired)
+                out = utils.unmarshal_json(http_res.text, errors.InviteExpired, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 422:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity)
+                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 429:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded)
+                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 500:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InternalServerError)
+                out = utils.unmarshal_json(http_res.text, errors.InternalServerError, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def browsers(self, request: operations.GetBrowsersByClicksRequest) -> operations.GetBrowsersByClicksResponse:
-        r"""Retrieve top browsers by clicks
-        Retrieve the top browsers by number of clicks for a link, a domain, or the authenticated workspace.
+    def update(self, slug: str, request_body: Optional[operations.UpdateDomainRequestBody] = None) -> operations.UpdateDomainResponse:
+        r"""Update a domain
+        Update a domain for the authenticated workspace.
         """
-        hook_ctx = HookContext(operation_id='getBrowsersByClicks', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.GetBrowsersByClicksGlobals(
-            workspace_id=self.sdk_configuration.globals.workspace_id,
-            project_slug=self.sdk_configuration.globals.project_slug,
+        hook_ctx = HookContext(operation_id='updateDomain', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.UpdateDomainRequest(
+            slug=slug,
+            request_body=request_body,
         )
         
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
-        
-        url = utils.generate_url(base_url, '/analytics/clicks/browsers', request, _globals)
-        
-        if callable(self.sdk_configuration.security):
-            headers, query_params = utils.get_security(self.sdk_configuration.security())
-        else:
-            headers, query_params = utils.get_security(self.sdk_configuration.security)
-        
-        headers = { **utils.get_headers(request, _globals), **headers }
-        query_params = { **utils.get_query_params(request, _globals), **query_params }
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
-        client = self.sdk_configuration.client
-        
-        try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
-            http_res = client.send(req)
-        except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
-
-        if utils.match_status_codes(['400','401','403','404','409','410','422','429','4XX','500','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
-                raise e
-            if result is not None:
-                http_res = result
-        else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
-        
-        
-        res = operations.GetBrowsersByClicksResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
-        
-        if http_res.status_code == 200:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetBrowsersByClicksResponseBody]])
-                res.response_bodies = out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 400:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequest)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 401:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Unauthorized)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 403:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Forbidden)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 404:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.NotFound)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 409:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Conflict)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 410:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InviteExpired)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 422:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 429:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 500:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InternalServerError)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        else:
-            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
-
-        return res
-
-    
-    
-    def os(self, request: operations.GetOSByClicksRequest) -> operations.GetOSByClicksResponse:
-        r"""Retrieve top OS by clicks
-        Retrieve the top OS by number of clicks for a link, a domain, or the authenticated workspace.
-        """
-        hook_ctx = HookContext(operation_id='getOSByClicks', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.GetOSByClicksGlobals(
+        _globals = operations.UpdateDomainGlobals(
             workspace_id=self.sdk_configuration.globals.workspace_id,
             project_slug=self.sdk_configuration.globals.project_slug,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/analytics/clicks/os', request, _globals)
+        url = utils.generate_url(base_url, '/domains/{slug}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
+        req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateDomainRequest, "request_body", False, True, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = client.prepare_request(requests_http.Request('PATCH', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
@@ -872,268 +482,136 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetOSByClicksResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
+        res = operations.UpdateDomainResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetOSByClicksResponseBody]])
-                res.response_bodies = out
+                out = utils.unmarshal_json(http_res.text, Optional[components.DomainSchema])
+                res.domain_schema = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequest)
+                out = utils.unmarshal_json(http_res.text, errors.BadRequest, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Unauthorized)
+                out = utils.unmarshal_json(http_res.text, errors.Unauthorized, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 403:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Forbidden)
+                out = utils.unmarshal_json(http_res.text, errors.Forbidden, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 404:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.NotFound)
+                out = utils.unmarshal_json(http_res.text, errors.NotFound, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 409:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Conflict)
+                out = utils.unmarshal_json(http_res.text, errors.Conflict, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 410:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InviteExpired)
+                out = utils.unmarshal_json(http_res.text, errors.InviteExpired, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 422:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity)
+                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 429:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded)
+                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 500:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InternalServerError)
+                out = utils.unmarshal_json(http_res.text, errors.InternalServerError, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def referers(self, request: operations.GetReferersByClicksRequest) -> operations.GetReferersByClicksResponse:
-        r"""Retrieve top referers by clicks
-        Retrieve the top referers by number of clicks for a link, a domain, or the authenticated workspace.
+    def set_primary(self, slug: str) -> operations.SetPrimaryDomainResponse:
+        r"""Set a domain as primary
+        Set a domain as primary for the authenticated workspace.
         """
-        hook_ctx = HookContext(operation_id='getReferersByClicks', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.GetReferersByClicksGlobals(
-            workspace_id=self.sdk_configuration.globals.workspace_id,
-            project_slug=self.sdk_configuration.globals.project_slug,
+        hook_ctx = HookContext(operation_id='setPrimaryDomain', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.SetPrimaryDomainRequest(
+            slug=slug,
         )
         
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
-        
-        url = utils.generate_url(base_url, '/analytics/clicks/referers', request, _globals)
-        
-        if callable(self.sdk_configuration.security):
-            headers, query_params = utils.get_security(self.sdk_configuration.security())
-        else:
-            headers, query_params = utils.get_security(self.sdk_configuration.security)
-        
-        headers = { **utils.get_headers(request, _globals), **headers }
-        query_params = { **utils.get_query_params(request, _globals), **query_params }
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
-        client = self.sdk_configuration.client
-        
-        try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
-            http_res = client.send(req)
-        except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
-
-        if utils.match_status_codes(['400','401','403','404','409','410','422','429','4XX','500','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
-                raise e
-            if result is not None:
-                http_res = result
-        else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
-        
-        
-        res = operations.GetReferersByClicksResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
-        
-        if http_res.status_code == 200:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetReferersByClicksResponseBody]])
-                res.response_bodies = out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 400:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequest)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 401:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Unauthorized)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 403:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Forbidden)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 404:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.NotFound)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 409:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Conflict)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 410:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InviteExpired)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 422:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 429:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 500:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InternalServerError)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        else:
-            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
-
-        return res
-
-    
-    
-    def top_links(self, request: operations.GetTopLinksByClicksRequest) -> operations.GetTopLinksByClicksResponse:
-        r"""Retrieve top links by clicks
-        Retrieve the top links by number of clicks for a domain or the authenticated workspace.
-        """
-        hook_ctx = HookContext(operation_id='getTopLinksByClicks', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.GetTopLinksByClicksGlobals(
+        _globals = operations.SetPrimaryDomainGlobals(
             workspace_id=self.sdk_configuration.globals.workspace_id,
             project_slug=self.sdk_configuration.globals.project_slug,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/analytics/clicks/top_links', request, _globals)
+        url = utils.generate_url(base_url, '/domains/{slug}/primary', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
@@ -1144,270 +622,140 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetTopLinksByClicksResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
+        res = operations.SetPrimaryDomainResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetTopLinksByClicksResponseBody]])
-                res.response_bodies = out
+                out = utils.unmarshal_json(http_res.text, Optional[components.DomainSchema])
+                res.domain_schema = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequest)
+                out = utils.unmarshal_json(http_res.text, errors.BadRequest, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Unauthorized)
+                out = utils.unmarshal_json(http_res.text, errors.Unauthorized, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 403:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Forbidden)
+                out = utils.unmarshal_json(http_res.text, errors.Forbidden, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 404:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.NotFound)
+                out = utils.unmarshal_json(http_res.text, errors.NotFound, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 409:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Conflict)
+                out = utils.unmarshal_json(http_res.text, errors.Conflict, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 410:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InviteExpired)
+                out = utils.unmarshal_json(http_res.text, errors.InviteExpired, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 422:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity)
+                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 429:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded)
+                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 500:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InternalServerError)
+                out = utils.unmarshal_json(http_res.text, errors.InternalServerError, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def top_urls(self, request: operations.GetTopURLsByClicksRequest) -> operations.GetTopURLsByClicksResponse:
-        r"""Retrieve top URLs by clicks
-        Retrieve the top URLs by number of clicks for a given short link.
+    def transfer(self, slug: str, request_body: Optional[operations.TransferDomainRequestBody] = None) -> operations.TransferDomainResponse:
+        r"""Transfer a domain
+        Transfer a domain to another workspace within the authenticated account.
         """
-        hook_ctx = HookContext(operation_id='getTopURLsByClicks', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.GetTopURLsByClicksGlobals(
-            workspace_id=self.sdk_configuration.globals.workspace_id,
-            project_slug=self.sdk_configuration.globals.project_slug,
+        hook_ctx = HookContext(operation_id='transferDomain', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.TransferDomainRequest(
+            slug=slug,
+            request_body=request_body,
         )
         
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
-        
-        url = utils.generate_url(base_url, '/analytics/clicks/top_urls', request, _globals)
-        
-        if callable(self.sdk_configuration.security):
-            headers, query_params = utils.get_security(self.sdk_configuration.security())
-        else:
-            headers, query_params = utils.get_security(self.sdk_configuration.security)
-        
-        headers = { **utils.get_headers(request, _globals), **headers }
-        query_params = { **utils.get_query_params(request, _globals), **query_params }
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
-        client = self.sdk_configuration.client
-        
-        try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
-            http_res = client.send(req)
-        except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
-
-        if utils.match_status_codes(['400','401','403','404','409','410','422','429','4XX','500','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
-                raise e
-            if result is not None:
-                http_res = result
-        else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
-        
-        
-        res = operations.GetTopURLsByClicksResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
-        
-        if http_res.status_code == 200:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetTopURLsByClicksResponseBody]])
-                res.response_bodies = out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 400:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequest)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 401:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Unauthorized)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 403:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Forbidden)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 404:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.NotFound)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 409:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Conflict)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 410:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InviteExpired)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 422:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 429:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 500:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InternalServerError)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        else:
-            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
-
-        return res
-
-    
-    
-    def get_clicks_count_deprecated(self, request: operations.GetClicksCountDeprecatedRequest) -> operations.GetClicksCountDeprecatedResponse:
-        r"""Retrieve the total clicks count
-        Retrieve the total number of clicks for a link, a domain, or the authenticated workspace.
-
-        Deprecated method: This method is deprecated. Use dub.analytics.clicks.count instead.. Use count instead.
-        """
-        hook_ctx = HookContext(operation_id='getClicksCountDeprecated', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.GetClicksCountDeprecatedGlobals(
+        _globals = operations.TransferDomainGlobals(
             workspace_id=self.sdk_configuration.globals.workspace_id,
             project_slug=self.sdk_configuration.globals.project_slug,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/analytics/clicks', request, _globals)
+        url = utils.generate_url(base_url, '/domains/{slug}/transfer', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
+        req_content_type, data, form = utils.serialize_request_body(request, operations.TransferDomainRequest, "request_body", False, True, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
@@ -1418,94 +766,94 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetClicksCountDeprecatedResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
+        res = operations.TransferDomainResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[float])
-                res.number = out
+                out = utils.unmarshal_json(http_res.text, Optional[components.DomainSchema])
+                res.domain_schema = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequest)
+                out = utils.unmarshal_json(http_res.text, errors.BadRequest, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Unauthorized)
+                out = utils.unmarshal_json(http_res.text, errors.Unauthorized, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 403:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Forbidden)
+                out = utils.unmarshal_json(http_res.text, errors.Forbidden, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 404:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.NotFound)
+                out = utils.unmarshal_json(http_res.text, errors.NotFound, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 409:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Conflict)
+                out = utils.unmarshal_json(http_res.text, errors.Conflict, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 410:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InviteExpired)
+                out = utils.unmarshal_json(http_res.text, errors.InviteExpired, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 422:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity)
+                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 429:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded)
+                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 500:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InternalServerError)
+                out = utils.unmarshal_json(http_res.text, errors.InternalServerError, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
```

### Comparing `dub-0.0.5/src/dub/metatags.py` & `dub-0.0.6/src/dub/metatags.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.5/src/dub/models/components/clicksbycities.py` & `dub-0.0.6/src/dub/models/components/clickscities.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from dub import utils
 from enum import Enum
 
 
-class ClicksByCitiesCountry(str, Enum):
+class ClicksCitiesCountry(str, Enum):
     r"""The 2-letter country code of the city: https://d.to/geo"""
     AF = 'AF'
     AL = 'AL'
     DZ = 'DZ'
     AS = 'AS'
     AD = 'AD'
     AO = 'AO'
@@ -259,16 +259,16 @@
     SX = 'SX'
     SS = 'SS'
     XK = 'XK'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ClicksByCities:
+class ClicksCities:
     city: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('city') }})
     r"""The name of the city"""
-    country: ClicksByCitiesCountry = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('country') }})
+    country: ClicksCitiesCountry = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('country') }})
     r"""The 2-letter country code of the city: https://d.to/geo"""
     clicks: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('clicks') }})
     r"""The number of clicks from this city"""
```

### Comparing `dub-0.0.5/src/dub/models/components/clicksbycountry.py` & `dub-0.0.6/src/dub/models/components/clickscountries.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,14 +259,14 @@
     SX = 'SX'
     SS = 'SS'
     XK = 'XK'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ClicksByCountry:
+class ClicksCountries:
     country: Country = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('country') }})
     r"""The 2-letter country code: https://d.to/geo"""
     clicks: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('clicks') }})
     r"""The number of clicks from this country"""
```

### Comparing `dub-0.0.5/src/dub/models/components/countrycode.py` & `dub-0.0.6/src/dub/models/components/countrycode.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.5/src/dub/models/components/domainschema.py` & `dub-0.0.6/src/dub/models/components/domainschema.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.5/src/dub/models/components/httpmetadata.py` & `dub-0.0.6/src/dub/models/components/httpmetadata.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.5/src/dub/models/components/linkgeotargeting.py` & `dub-0.0.6/src/dub/models/components/linkgeotargeting.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.5/src/dub/models/components/linkschema.py` & `dub-0.0.6/src/dub/models/components/linkschema.py`

 * *Files 0% similar despite different names*

```diff
@@ -343,9 +343,13 @@
     r"""Whether the short link uses Custom Social Media Cards feature."""
     rewrite: Optional[bool] = dataclasses.field(default=False, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rewrite'), 'exclude': lambda f: f is None }})
     r"""Whether the short link uses link cloaking."""
     public_stats: Optional[bool] = dataclasses.field(default=False, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('publicStats'), 'exclude': lambda f: f is None }})
     r"""Whether the short link's stats are publicly accessible."""
     clicks: Optional[float] = dataclasses.field(default=0, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('clicks'), 'exclude': lambda f: f is None }})
     r"""The number of clicks on the short link."""
+    leads: Optional[float] = dataclasses.field(default=0, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leads'), 'exclude': lambda f: f is None }})
+    r"""[BETA]: The number of leads the short links has generated."""
+    sales: Optional[float] = dataclasses.field(default=0, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sales'), 'exclude': lambda f: f is None }})
+    r"""[BETA]: The number of sales the short links has generated."""
```

### Comparing `dub-0.0.5/src/dub/models/components/tagschema.py` & `dub-0.0.6/src/dub/models/components/tagschema.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.5/src/dub/models/components/workspaceschema.py` & `dub-0.0.6/src/dub/models/components/workspaceschema.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.5/src/dub/models/errors/__init__.py` & `dub-0.0.6/src/dub/models/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.5/src/dub/models/errors/badrequest.py` & `dub-0.0.6/src/dub/models/errors/badrequest.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.5/src/dub/models/errors/conflict.py` & `dub-0.0.6/src/dub/models/errors/conflict.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.5/src/dub/models/errors/forbidden.py` & `dub-0.0.6/src/dub/models/errors/forbidden.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.5/src/dub/models/errors/internalservererror.py` & `dub-0.0.6/src/dub/models/errors/internalservererror.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.5/src/dub/models/errors/inviteexpired.py` & `dub-0.0.6/src/dub/models/errors/inviteexpired.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.5/src/dub/models/errors/notfound.py` & `dub-0.0.6/src/dub/models/errors/notfound.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.5/src/dub/models/errors/ratelimitexceeded.py` & `dub-0.0.6/src/dub/models/errors/ratelimitexceeded.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.5/src/dub/models/errors/sdkerror.py` & `dub-0.0.6/src/dub/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.5/src/dub/models/errors/unauthorized.py` & `dub-0.0.6/src/dub/models/errors/unauthorized.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.5/src/dub/models/errors/unprocessableentity.py` & `dub-0.0.6/src/dub/models/errors/unprocessableentity.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.5/src/dub/models/internal/globals.py` & `dub-0.0.6/src/dub/models/internal/globals.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.5/src/dub/models/operations/adddomain.py` & `dub-0.0.6/src/dub/models/operations/adddomain.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     r"""Prevent search engines from indexing the domain. Defaults to `false`."""
     placeholder: Optional[str] = dataclasses.field(default='https://dub.co/help/article/what-is-dub', metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('placeholder'), 'exclude': lambda f: f is AddDomainRequestBody.UNSET }})
     r"""Provide context to your teammates in the link creation modal by showing them an example of a link to be shortened."""
     
 
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class AddDomainResponse:
-    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
+    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field(metadata={'dataclasses_json': { 'exclude': lambda f: True }})
     domain_schema: Optional[components_domainschema.DomainSchema] = dataclasses.field(default=None)
     r"""The domain was added."""
```

### Comparing `dub-0.0.5/src/dub/models/operations/bulkcreatelinks.py` & `dub-0.0.6/src/dub/models/operations/bulkcreatelinks.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,15 @@
     r"""The Android destination URL for the short link for Android device targeting."""
     geo: Optional[components_linkgeotargeting.LinkGeoTargeting] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('geo'), 'exclude': lambda f: f is RequestBody.UNSET }})
     r"""Geo targeting information for the short link in JSON format `{[COUNTRY]: https://example.com }`."""
     
 
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class BulkCreateLinksResponse:
-    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
+    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field(metadata={'dataclasses_json': { 'exclude': lambda f: True }})
     link_schemas: Optional[List[components_linkschema.LinkSchema]] = dataclasses.field(default=None)
     r"""The created links"""
```

### Comparing `dub-0.0.5/src/dub/models/operations/createlink.py` & `dub-0.0.6/src/dub/models/operations/createlink.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,15 @@
     r"""The Android destination URL for the short link for Android device targeting."""
     geo: Optional[components_linkgeotargeting.LinkGeoTargeting] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('geo'), 'exclude': lambda f: f is CreateLinkRequestBody.UNSET }})
     r"""Geo targeting information for the short link in JSON format `{[COUNTRY]: https://example.com }`."""
     
 
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CreateLinkResponse:
-    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
+    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field(metadata={'dataclasses_json': { 'exclude': lambda f: True }})
     link_schema: Optional[components_linkschema.LinkSchema] = dataclasses.field(default=None)
     r"""The created link"""
```

### Comparing `dub-0.0.5/src/dub/models/operations/createtag.py` & `dub-0.0.6/src/dub/models/operations/createtag.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     r"""The name of the tag to create."""
     color: Optional[Color] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('color'), 'exclude': lambda f: f is None }})
     r"""The color of the tag. If not provided, a random color will be used from the list: red, yellow, green, blue, purple, pink, brown."""
     
 
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CreateTagResponse:
-    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
+    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field(metadata={'dataclasses_json': { 'exclude': lambda f: True }})
     tag_schema: Optional[components_tagschema.TagSchema] = dataclasses.field(default=None)
     r"""The created tag"""
```

### Comparing `dub-0.0.5/src/dub/models/operations/createworkspace.py` & `dub-0.0.6/src/dub/models/operations/createworkspace.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
     slug: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('slug') }})
     domain: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('domain'), 'exclude': lambda f: f is None }})
     
 
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CreateWorkspaceResponse:
-    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
+    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field(metadata={'dataclasses_json': { 'exclude': lambda f: True }})
     workspace_schema: Optional[components_workspaceschema.WorkspaceSchema] = dataclasses.field(default=None)
     r"""The created workspace"""
```

### Comparing `dub-0.0.5/src/dub/models/operations/deletedomain.py` & `dub-0.0.6/src/dub/models/operations/deletedomain.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     r"""The domain was deleted."""
     slug: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('slug') }})
     r"""The domain name."""
     
 
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DeleteDomainResponse:
-    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
+    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field(metadata={'dataclasses_json': { 'exclude': lambda f: True }})
     object: Optional[DeleteDomainResponseBody] = dataclasses.field(default=None)
     r"""The domain was deleted."""
```

### Comparing `dub-0.0.5/src/dub/models/operations/deletelink.py` & `dub-0.0.6/src/dub/models/operations/deletelink.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     r"""The deleted link"""
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     r"""The ID of the link."""
     
 
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DeleteLinkResponse:
-    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
+    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field(metadata={'dataclasses_json': { 'exclude': lambda f: True }})
     object: Optional[DeleteLinkResponseBody] = dataclasses.field(default=None)
     r"""The deleted link"""
```

### Comparing `dub-0.0.5/src/dub/models/operations/getlinkinfo.py` & `dub-0.0.6/src/dub/models/operations/getlinkinfo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ...models.components import httpmetadata as components_httpmetadata
 from ...models.components import linkschema as components_linkschema
+from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetLinkInfoGlobals:
     workspace_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'workspaceId', 'style': 'form', 'explode': True }})
     project_slug: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'projectSlug', 'style': 'form', 'explode': True }})
@@ -25,14 +26,15 @@
     r"""The unique ID of the short link."""
     external_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'externalId', 'style': 'form', 'explode': True }})
     r"""This is the ID of the link in the your database. Must be prefixed with `ext_` when passed as a query parameter."""
     
 
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetLinkInfoResponse:
-    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
+    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field(metadata={'dataclasses_json': { 'exclude': lambda f: True }})
     link_schema: Optional[components_linkschema.LinkSchema] = dataclasses.field(default=None)
     r"""The retrieved link"""
```

### Comparing `dub-0.0.5/src/dub/models/operations/getlinks.py` & `dub-0.0.6/src/dub/models/operations/getlinks.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ...models.components import httpmetadata as components_httpmetadata
 from ...models.components import linkschema as components_linkschema
+from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import List, Optional, Union
 
 
 @dataclasses.dataclass
 class GetLinksGlobals:
     workspace_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'workspaceId', 'style': 'form', 'explode': True }})
@@ -50,14 +51,15 @@
     r"""The field to sort the links by. The default is `createdAt`, and sort order is always descending."""
     page: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
     r"""The page number for pagination (each page contains 100 links)."""
     
 
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetLinksResponse:
-    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
+    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field(metadata={'dataclasses_json': { 'exclude': lambda f: True }})
     link_schemas: Optional[List[components_linkschema.LinkSchema]] = dataclasses.field(default=None)
     r"""A list of links"""
```

### Comparing `dub-0.0.5/src/dub/models/operations/getlinkscount.py` & `dub-0.0.6/src/dub/models/operations/getlinkscount.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ...models.components import httpmetadata as components_httpmetadata
+from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import List, Optional, Union
 
 
 @dataclasses.dataclass
 class GetLinksCountGlobals:
     workspace_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'workspaceId', 'style': 'form', 'explode': True }})
@@ -50,14 +51,15 @@
     r"""Whether to include tags in the response. Defaults to `false` if not provided."""
     group_by: Optional[GroupBy] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'groupBy', 'style': 'form', 'explode': True }})
     r"""The field to group the links by."""
     
 
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetLinksCountResponse:
-    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
+    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field(metadata={'dataclasses_json': { 'exclude': lambda f: True }})
     number: Optional[float] = dataclasses.field(default=None)
     r"""A list of links"""
```

### Comparing `dub-0.0.5/src/dub/models/operations/getmetatags.py` & `dub-0.0.6/src/dub/models/operations/getmetatags.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     r"""The meta description tag for the URL."""
     image: Optional[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('image') }})
     r"""The OpenGraph image for the URL."""
     
 
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetMetatagsResponse:
-    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
+    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field(metadata={'dataclasses_json': { 'exclude': lambda f: True }})
     object: Optional[GetMetatagsResponseBody] = dataclasses.field(default=None)
     r"""The retrieved metatags"""
```

### Comparing `dub-0.0.5/src/dub/models/operations/getqrcode.py` & `dub-0.0.6/src/dub/models/operations/getqrcode.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ...models.components import httpmetadata as components_httpmetadata
+from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 
 
 class Level(str, Enum):
     r"""The level of error correction to use for the QR code. Defaults to `L` if not provided."""
     L = 'L'
@@ -29,14 +30,15 @@
     r"""The background color of the QR code in hex format. Defaults to `#ffffff` if not provided."""
     include_margin: Optional[bool] = dataclasses.field(default=True, metadata={'query_param': { 'field_name': 'includeMargin', 'style': 'form', 'explode': True }})
     r"""Whether to include a margin around the QR code. Defaults to `false` if not provided."""
     
 
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetQRCodeResponse:
-    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
+    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field(metadata={'dataclasses_json': { 'exclude': lambda f: True }})
     res: Optional[str] = dataclasses.field(default=None)
     r"""The QR code"""
```

### Comparing `dub-0.0.5/src/dub/models/operations/gettags.py` & `dub-0.0.6/src/dub/models/operations/gettags.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ...models.components import httpmetadata as components_httpmetadata
 from ...models.components import tagschema as components_tagschema
+from dataclasses_json import Undefined, dataclass_json
 from typing import List, Optional
 
 
 @dataclasses.dataclass
 class GetTagsGlobals:
     workspace_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'workspaceId', 'style': 'form', 'explode': True }})
     project_slug: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'projectSlug', 'style': 'form', 'explode': True }})
@@ -17,14 +18,15 @@
 
 
 @dataclasses.dataclass
 class GetTagsRequest:
     pass
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetTagsResponse:
-    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
+    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field(metadata={'dataclasses_json': { 'exclude': lambda f: True }})
     tag_schemas: Optional[List[components_tagschema.TagSchema]] = dataclasses.field(default=None)
     r"""A list of tags"""
```

### Comparing `dub-0.0.5/src/dub/models/operations/getworkspace.py` & `dub-0.0.6/src/dub/models/operations/getworkspace.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ...models.components import httpmetadata as components_httpmetadata
 from ...models.components import workspaceschema as components_workspaceschema
+from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetWorkspaceRequest:
     id_or_slug: str = dataclasses.field(metadata={'path_param': { 'field_name': 'idOrSlug', 'style': 'simple', 'explode': False }})
     r"""The ID or slug of the workspace."""
     
 
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetWorkspaceResponse:
-    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
+    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field(metadata={'dataclasses_json': { 'exclude': lambda f: True }})
     workspace_schema: Optional[components_workspaceschema.WorkspaceSchema] = dataclasses.field(default=None)
     r"""The retrieved workspace"""
```

### Comparing `dub-0.0.5/src/dub/models/operations/listdomains.py` & `dub-0.0.6/src/dub/models/operations/listdomains.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ...models.components import domainschema as components_domainschema
 from ...models.components import httpmetadata as components_httpmetadata
+from dataclasses_json import Undefined, dataclass_json
 from typing import List, Optional
 
 
 @dataclasses.dataclass
 class ListDomainsGlobals:
     workspace_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'workspaceId', 'style': 'form', 'explode': True }})
     project_slug: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'projectSlug', 'style': 'form', 'explode': True }})
@@ -17,14 +18,15 @@
 
 
 @dataclasses.dataclass
 class ListDomainsRequest:
     pass
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ListDomainsResponse:
-    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
+    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field(metadata={'dataclasses_json': { 'exclude': lambda f: True }})
     domain_schemas: Optional[List[components_domainschema.DomainSchema]] = dataclasses.field(default=None)
     r"""The domains were retrieved."""
```

### Comparing `dub-0.0.5/src/dub/models/operations/setprimarydomain.py` & `dub-0.0.6/src/dub/models/operations/setprimarydomain.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ...models.components import domainschema as components_domainschema
 from ...models.components import httpmetadata as components_httpmetadata
+from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclasses.dataclass
 class SetPrimaryDomainGlobals:
     workspace_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'workspaceId', 'style': 'form', 'explode': True }})
     project_slug: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'projectSlug', 'style': 'form', 'explode': True }})
@@ -20,14 +21,15 @@
 class SetPrimaryDomainRequest:
     slug: str = dataclasses.field(metadata={'path_param': { 'field_name': 'slug', 'style': 'simple', 'explode': False }})
     r"""The domain name."""
     
 
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SetPrimaryDomainResponse:
-    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
+    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field(metadata={'dataclasses_json': { 'exclude': lambda f: True }})
     domain_schema: Optional[components_domainschema.DomainSchema] = dataclasses.field(default=None)
     r"""The domain was set as primary"""
```

### Comparing `dub-0.0.5/src/dub/models/operations/trackcustomer.py` & `dub-0.0.6/src/dub/models/operations/trackcustomer.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,22 +7,21 @@
 from dub import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TrackCustomerRequestBody:
-    UNSET='__SPEAKEASY_UNSET__'
     customer_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerId') }})
     r"""This is the unique identifier for the customer in the client's app. This is used to track the customer's journey."""
-    customer_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerName'), 'exclude': lambda f: f is TrackCustomerRequestBody.UNSET }})
+    customer_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerName'), 'exclude': lambda f: f is None }})
     r"""Name of the customer in the client's app."""
-    customer_email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerEmail'), 'exclude': lambda f: f is TrackCustomerRequestBody.UNSET }})
+    customer_email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerEmail'), 'exclude': lambda f: f is None }})
     r"""Email of the customer in the client's app."""
-    customer_avatar: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerAvatar'), 'exclude': lambda f: f is TrackCustomerRequestBody.UNSET }})
+    customer_avatar: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerAvatar'), 'exclude': lambda f: f is None }})
     r"""Avatar of the customer in the client's app."""
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
@@ -32,14 +31,15 @@
     customer_name: Optional[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerName') }})
     customer_email: Optional[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerEmail') }})
     customer_avatar: Optional[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerAvatar') }})
     
 
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TrackCustomerResponse:
-    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
+    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field(metadata={'dataclasses_json': { 'exclude': lambda f: True }})
     object: Optional[TrackCustomerResponseBody] = dataclasses.field(default=None)
     r"""A customer was tracked."""
```

### Comparing `dub-0.0.5/src/dub/models/operations/tracklead.py` & `dub-0.0.6/src/dub/models/operations/tracklead.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,28 +7,27 @@
 from dub import utils
 from typing import Any, Dict, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TrackLeadRequestBody:
-    UNSET='__SPEAKEASY_UNSET__'
     click_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('clickId') }})
     r"""The ID of the click in th Dub. You can read this value from `dclid` cookie."""
     event_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventName') }})
     r"""The name of the event to track."""
     customer_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerId') }})
     r"""This is the unique identifier for the customer in the client's app. This is used to track the customer's journey."""
-    customer_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerName'), 'exclude': lambda f: f is TrackLeadRequestBody.UNSET }})
+    customer_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerName'), 'exclude': lambda f: f is None }})
     r"""Name of the customer in the client's app."""
-    customer_email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerEmail'), 'exclude': lambda f: f is TrackLeadRequestBody.UNSET }})
+    customer_email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerEmail'), 'exclude': lambda f: f is None }})
     r"""Email of the customer in the client's app."""
-    customer_avatar: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerAvatar'), 'exclude': lambda f: f is TrackLeadRequestBody.UNSET }})
+    customer_avatar: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerAvatar'), 'exclude': lambda f: f is None }})
     r"""Avatar of the customer in the client's app."""
-    metadata: Optional[Dict[str, Any]] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is TrackLeadRequestBody.UNSET }})
+    metadata: Optional[Dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     r"""Additional metadata to be stored with the lead event"""
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
@@ -36,19 +35,20 @@
     r"""A lead was tracked."""
     click_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('clickId') }})
     event_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventName') }})
     customer_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerId') }})
     customer_name: Optional[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerName') }})
     customer_email: Optional[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerEmail') }})
     customer_avatar: Optional[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerAvatar') }})
-    metadata: Optional[Dict[str, Any]] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata') }})
+    metadata: Optional[Dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     
 
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TrackLeadResponse:
-    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
+    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field(metadata={'dataclasses_json': { 'exclude': lambda f: True }})
     object: Optional[TrackLeadResponseBody] = dataclasses.field(default=None)
     r"""A lead was tracked."""
```

### Comparing `dub-0.0.5/src/dub/models/operations/tracksale.py` & `dub-0.0.6/src/dub/models/operations/tracksale.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     invoice_id: Optional[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoiceId') }})
     currency: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency') }})
     metadata: Optional[Dict[str, Any]] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata') }})
     
 
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TrackSaleResponse:
-    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
+    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field(metadata={'dataclasses_json': { 'exclude': lambda f: True }})
     object: Optional[TrackSaleResponseBody] = dataclasses.field(default=None)
     r"""A sale was tracked."""
```

### Comparing `dub-0.0.5/src/dub/models/operations/transferdomain.py` & `dub-0.0.6/src/dub/models/operations/transferdomain.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     slug: str = dataclasses.field(metadata={'path_param': { 'field_name': 'slug', 'style': 'simple', 'explode': False }})
     r"""The domain name."""
     request_body: Optional[TransferDomainRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TransferDomainResponse:
-    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
+    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field(metadata={'dataclasses_json': { 'exclude': lambda f: True }})
     domain_schema: Optional[components_domainschema.DomainSchema] = dataclasses.field(default=None)
     r"""The domain transfer initiated"""
```

### Comparing `dub-0.0.5/src/dub/models/operations/updatedomain.py` & `dub-0.0.6/src/dub/models/operations/updatedomain.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     slug: str = dataclasses.field(metadata={'path_param': { 'field_name': 'slug', 'style': 'simple', 'explode': False }})
     r"""The domain name."""
     request_body: Optional[UpdateDomainRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class UpdateDomainResponse:
-    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
+    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field(metadata={'dataclasses_json': { 'exclude': lambda f: True }})
     domain_schema: Optional[components_domainschema.DomainSchema] = dataclasses.field(default=None)
     r"""The domain was updated."""
```

### Comparing `dub-0.0.5/src/dub/models/operations/updatelink.py` & `dub-0.0.6/src/dub/models/operations/updatelink.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,15 @@
     link_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'linkId', 'style': 'simple', 'explode': False }})
     r"""The id of the link to update. You may use either `linkId` (obtained via `/links/info` endpoint) or `externalId` prefixed with `ext_`."""
     request_body: Optional[UpdateLinkRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class UpdateLinkResponse:
-    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
+    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field(metadata={'dataclasses_json': { 'exclude': lambda f: True }})
     link_schema: Optional[components_linkschema.LinkSchema] = dataclasses.field(default=None)
     r"""The updated link"""
```

### Comparing `dub-0.0.5/src/dub/models/operations/upsertlink.py` & `dub-0.0.6/src/dub/models/operations/upsertlink.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,15 @@
     r"""The Android destination URL for the short link for Android device targeting."""
     geo: Optional[components_linkgeotargeting.LinkGeoTargeting] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('geo'), 'exclude': lambda f: f is UpsertLinkRequestBody.UNSET }})
     r"""Geo targeting information for the short link in JSON format `{[COUNTRY]: https://example.com }`."""
     
 
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class UpsertLinkResponse:
-    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
+    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field(metadata={'dataclasses_json': { 'exclude': lambda f: True }})
     link_schema: Optional[components_linkschema.LinkSchema] = dataclasses.field(default=None)
     r"""The upserted link"""
```

### Comparing `dub-0.0.5/src/dub/qr_codes.py` & `dub-0.0.6/src/dub/qr_codes.py`

 * *Files 16% similar despite different names*

```diff
@@ -61,81 +61,81 @@
                 res.res = http_res.text
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequest)
+                out = utils.unmarshal_json(http_res.text, errors.BadRequest, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Unauthorized)
+                out = utils.unmarshal_json(http_res.text, errors.Unauthorized, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 403:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Forbidden)
+                out = utils.unmarshal_json(http_res.text, errors.Forbidden, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 404:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.NotFound)
+                out = utils.unmarshal_json(http_res.text, errors.NotFound, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 409:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Conflict)
+                out = utils.unmarshal_json(http_res.text, errors.Conflict, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 410:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InviteExpired)
+                out = utils.unmarshal_json(http_res.text, errors.InviteExpired, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 422:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity)
+                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 429:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded)
+                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 500:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InternalServerError)
+                out = utils.unmarshal_json(http_res.text, errors.InternalServerError, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
```

### Comparing `dub-0.0.5/src/dub/sdk.py` & `dub-0.0.6/src/dub/sdk.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.5/src/dub/sdkconfiguration.py` & `dub-0.0.6/src/dub/sdkconfiguration.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,17 +21,17 @@
     client: requests_http.Session
     globals: internal.Globals
     security: Union[components.Security,Callable[[], components.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = '0.0.1'
-    sdk_version: str = '0.0.5'
-    gen_version: str = '2.333.3'
-    user_agent: str = 'speakeasy-sdk/python 0.0.5 2.333.3 0.0.1 dub'
+    sdk_version: str = '0.0.6'
+    gen_version: str = '2.338.1'
+    user_agent: str = 'speakeasy-sdk/python 0.0.6 2.338.1 0.0.1 dub'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `dub-0.0.5/src/dub/tags.py` & `dub-0.0.6/src/dub/tags.py`

 * *Files 7% similar despite different names*

```diff
@@ -72,81 +72,81 @@
                 res.tag_schemas = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequest)
+                out = utils.unmarshal_json(http_res.text, errors.BadRequest, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Unauthorized)
+                out = utils.unmarshal_json(http_res.text, errors.Unauthorized, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 403:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Forbidden)
+                out = utils.unmarshal_json(http_res.text, errors.Forbidden, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 404:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.NotFound)
+                out = utils.unmarshal_json(http_res.text, errors.NotFound, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 409:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Conflict)
+                out = utils.unmarshal_json(http_res.text, errors.Conflict, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 410:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InviteExpired)
+                out = utils.unmarshal_json(http_res.text, errors.InviteExpired, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 422:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity)
+                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 429:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded)
+                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 500:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InternalServerError)
+                out = utils.unmarshal_json(http_res.text, errors.InternalServerError, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
@@ -216,81 +216,81 @@
                 res.tag_schema = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequest)
+                out = utils.unmarshal_json(http_res.text, errors.BadRequest, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Unauthorized)
+                out = utils.unmarshal_json(http_res.text, errors.Unauthorized, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 403:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Forbidden)
+                out = utils.unmarshal_json(http_res.text, errors.Forbidden, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 404:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.NotFound)
+                out = utils.unmarshal_json(http_res.text, errors.NotFound, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 409:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Conflict)
+                out = utils.unmarshal_json(http_res.text, errors.Conflict, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 410:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InviteExpired)
+                out = utils.unmarshal_json(http_res.text, errors.InviteExpired, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 422:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity)
+                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 429:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded)
+                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 500:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InternalServerError)
+                out = utils.unmarshal_json(http_res.text, errors.InternalServerError, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
```

### Comparing `dub-0.0.5/src/dub/track.py` & `dub-0.0.6/src/dub/workspaces.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,44 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from dub import utils
 from dub._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from dub.models import components, errors, operations
-from typing import Optional
+from typing import List, Optional
 
-class Track:
+class Workspaces:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def lead(self, request: Optional[operations.TrackLeadRequestBody] = None) -> operations.TrackLeadResponse:
-        r"""Track a lead
-        Track a lead for a short link.
+    def list(self) -> operations.GetWorkspacesResponse:
+        r"""Retrieve a list of workspaces
+        Retrieve a list of workspaces for the authenticated user.
         """
-        hook_ctx = HookContext(operation_id='trackLead', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='getWorkspaces', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/track/lead'
+        url = base_url + '/workspaces'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        req_content_type, data, form = utils.serialize_request_body(request, Optional[operations.TrackLeadRequestBody], "request", False, True, 'json')
-        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
@@ -52,120 +49,120 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.TrackLeadResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
+        res = operations.GetWorkspacesResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[operations.TrackLeadResponseBody])
-                res.object = out
+                out = utils.unmarshal_json(http_res.text, Optional[List[components.WorkspaceSchema]])
+                res.workspace_schemas = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequest)
+                out = utils.unmarshal_json(http_res.text, errors.BadRequest, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Unauthorized)
+                out = utils.unmarshal_json(http_res.text, errors.Unauthorized, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 403:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Forbidden)
+                out = utils.unmarshal_json(http_res.text, errors.Forbidden, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 404:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.NotFound)
+                out = utils.unmarshal_json(http_res.text, errors.NotFound, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 409:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Conflict)
+                out = utils.unmarshal_json(http_res.text, errors.Conflict, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 410:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InviteExpired)
+                out = utils.unmarshal_json(http_res.text, errors.InviteExpired, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 422:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity)
+                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 429:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded)
+                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 500:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InternalServerError)
+                out = utils.unmarshal_json(http_res.text, errors.InternalServerError, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def sale(self, request: Optional[operations.TrackSaleRequestBody] = None) -> operations.TrackSaleResponse:
-        r"""Track a sale
-        Track a sale for a short link.
+    def create(self, request: Optional[operations.CreateWorkspaceRequestBody] = None) -> operations.CreateWorkspaceResponse:
+        r"""Create a workspace
+        Create a new workspace for the authenticated user.
         """
-        hook_ctx = HookContext(operation_id='trackSale', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='createWorkspace', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/track/sale'
+        url = base_url + '/workspaces'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        req_content_type, data, form = utils.serialize_request_body(request, Optional[operations.TrackSaleRequestBody], "request", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, Optional[operations.CreateWorkspaceRequestBody], "request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
@@ -184,128 +181,129 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.TrackSaleResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
+        res = operations.CreateWorkspaceResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[operations.TrackSaleResponseBody])
-                res.object = out
+                out = utils.unmarshal_json(http_res.text, Optional[components.WorkspaceSchema])
+                res.workspace_schema = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequest)
+                out = utils.unmarshal_json(http_res.text, errors.BadRequest, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Unauthorized)
+                out = utils.unmarshal_json(http_res.text, errors.Unauthorized, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 403:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Forbidden)
+                out = utils.unmarshal_json(http_res.text, errors.Forbidden, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 404:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.NotFound)
+                out = utils.unmarshal_json(http_res.text, errors.NotFound, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 409:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Conflict)
+                out = utils.unmarshal_json(http_res.text, errors.Conflict, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 410:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InviteExpired)
+                out = utils.unmarshal_json(http_res.text, errors.InviteExpired, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 422:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity)
+                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 429:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded)
+                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 500:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InternalServerError)
+                out = utils.unmarshal_json(http_res.text, errors.InternalServerError, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def customer(self, request: Optional[operations.TrackCustomerRequestBody] = None) -> operations.TrackCustomerResponse:
-        r"""Track a customer
-        Track a customer for an authenticated workspace.
+    def get(self, id_or_slug: str) -> operations.GetWorkspaceResponse:
+        r"""Retrieve a workspace
+        Retrieve a workspace for the authenticated user.
         """
-        hook_ctx = HookContext(operation_id='trackCustomer', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='getWorkspace', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.GetWorkspaceRequest(
+            id_or_slug=id_or_slug,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/track/customer'
+        url = utils.generate_url(base_url, '/workspaces/{idOrSlug}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        req_content_type, data, form = utils.serialize_request_body(request, Optional[operations.TrackCustomerRequestBody], "request", False, True, 'json')
-        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
@@ -316,94 +314,94 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.TrackCustomerResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
+        res = operations.GetWorkspaceResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[operations.TrackCustomerResponseBody])
-                res.object = out
+                out = utils.unmarshal_json(http_res.text, Optional[components.WorkspaceSchema])
+                res.workspace_schema = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequest)
+                out = utils.unmarshal_json(http_res.text, errors.BadRequest, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Unauthorized)
+                out = utils.unmarshal_json(http_res.text, errors.Unauthorized, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 403:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Forbidden)
+                out = utils.unmarshal_json(http_res.text, errors.Forbidden, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 404:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.NotFound)
+                out = utils.unmarshal_json(http_res.text, errors.NotFound, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 409:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Conflict)
+                out = utils.unmarshal_json(http_res.text, errors.Conflict, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 410:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InviteExpired)
+                out = utils.unmarshal_json(http_res.text, errors.InviteExpired, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 422:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity)
+                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 429:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded)
+                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 500:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InternalServerError)
+                out = utils.unmarshal_json(http_res.text, errors.InternalServerError, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
```

### Comparing `dub-0.0.5/src/dub/utils/retries.py` & `dub-0.0.6/src/dub/utils/retries.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.5/src/dub/utils/utils.py` & `dub-0.0.6/src/dub/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -814,19 +814,19 @@
             return ",".join(items)
     else:
         return f"{_val_to_string(obj)}"
 
     return ""
 
 
-def unmarshal_json(data, typ, decoder=None):
+def unmarshal_json(data, typ, decoder=None, infer_missing=False):
     unmarshal = make_dataclass("Unmarshal", [("res", typ)], bases=(DataClassJsonMixin,))
     json_dict = json.loads(data)
     try:
-        out = unmarshal.from_dict({"res": json_dict})
+        out = unmarshal.from_dict({"res": json_dict}, infer_missing=infer_missing)
     except AttributeError as attr_err:
         raise AttributeError(
             f"unable to unmarshal {data} as {typ} - {attr_err}"
         ) from attr_err
 
     return out.res if decoder is None else decoder(out.res)
```

### Comparing `dub-0.0.5/src/dub/workspaces.py` & `dub-0.0.6/src/dub/track.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from dub import utils
 from dub._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from dub.models import components, errors, operations
-from typing import List, Optional
+from typing import Optional
 
-class Workspaces:
+class Track:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def list(self) -> operations.GetWorkspacesResponse:
-        r"""Retrieve a list of workspaces
-        Retrieve a list of workspaces for the authenticated user.
+    def lead(self, request: Optional[operations.TrackLeadRequestBody] = None) -> operations.TrackLeadResponse:
+        r"""Track a lead
+        Track a lead for a short link.
         """
-        hook_ctx = HookContext(operation_id='getWorkspaces', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='trackLead', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/workspaces'
+        url = base_url + '/track/lead'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        req_content_type, data, form = utils.serialize_request_body(request, Optional[operations.TrackLeadRequestBody], "request", False, True, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
@@ -49,120 +52,120 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetWorkspacesResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
+        res = operations.TrackLeadResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[components.WorkspaceSchema]])
-                res.workspace_schemas = out
+                out = utils.unmarshal_json(http_res.text, Optional[operations.TrackLeadResponseBody])
+                res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequest)
+                out = utils.unmarshal_json(http_res.text, errors.BadRequest, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Unauthorized)
+                out = utils.unmarshal_json(http_res.text, errors.Unauthorized, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 403:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Forbidden)
+                out = utils.unmarshal_json(http_res.text, errors.Forbidden, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 404:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.NotFound)
+                out = utils.unmarshal_json(http_res.text, errors.NotFound, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 409:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Conflict)
+                out = utils.unmarshal_json(http_res.text, errors.Conflict, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 410:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InviteExpired)
+                out = utils.unmarshal_json(http_res.text, errors.InviteExpired, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 422:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity)
+                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 429:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded)
+                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 500:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InternalServerError)
+                out = utils.unmarshal_json(http_res.text, errors.InternalServerError, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def create(self, request: Optional[operations.CreateWorkspaceRequestBody] = None) -> operations.CreateWorkspaceResponse:
-        r"""Create a workspace
-        Create a new workspace for the authenticated user.
+    def sale(self, request: Optional[operations.TrackSaleRequestBody] = None) -> operations.TrackSaleResponse:
+        r"""Track a sale
+        Track a sale for a short link.
         """
-        hook_ctx = HookContext(operation_id='createWorkspace', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='trackSale', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/workspaces'
+        url = base_url + '/track/sale'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        req_content_type, data, form = utils.serialize_request_body(request, Optional[operations.CreateWorkspaceRequestBody], "request", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, Optional[operations.TrackSaleRequestBody], "request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
@@ -181,129 +184,128 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.CreateWorkspaceResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
+        res = operations.TrackSaleResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.WorkspaceSchema])
-                res.workspace_schema = out
+                out = utils.unmarshal_json(http_res.text, Optional[operations.TrackSaleResponseBody])
+                res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequest)
+                out = utils.unmarshal_json(http_res.text, errors.BadRequest, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Unauthorized)
+                out = utils.unmarshal_json(http_res.text, errors.Unauthorized, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 403:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Forbidden)
+                out = utils.unmarshal_json(http_res.text, errors.Forbidden, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 404:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.NotFound)
+                out = utils.unmarshal_json(http_res.text, errors.NotFound, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 409:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Conflict)
+                out = utils.unmarshal_json(http_res.text, errors.Conflict, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 410:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InviteExpired)
+                out = utils.unmarshal_json(http_res.text, errors.InviteExpired, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 422:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity)
+                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 429:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded)
+                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 500:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InternalServerError)
+                out = utils.unmarshal_json(http_res.text, errors.InternalServerError, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def get(self, id_or_slug: str) -> operations.GetWorkspaceResponse:
-        r"""Retrieve a workspace
-        Retrieve a workspace for the authenticated user.
+    def customer(self, request: Optional[operations.TrackCustomerRequestBody] = None) -> operations.TrackCustomerResponse:
+        r"""Track a customer
+        Track a customer for an authenticated workspace.
         """
-        hook_ctx = HookContext(operation_id='getWorkspace', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.GetWorkspaceRequest(
-            id_or_slug=id_or_slug,
-        )
-        
+        hook_ctx = HookContext(operation_id='trackCustomer', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/workspaces/{idOrSlug}', request)
+        url = base_url + '/track/customer'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        req_content_type, data, form = utils.serialize_request_body(request, Optional[operations.TrackCustomerRequestBody], "request", False, True, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
@@ -314,94 +316,94 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetWorkspaceResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
+        res = operations.TrackCustomerResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.WorkspaceSchema])
-                res.workspace_schema = out
+                out = utils.unmarshal_json(http_res.text, Optional[operations.TrackCustomerResponseBody])
+                res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequest)
+                out = utils.unmarshal_json(http_res.text, errors.BadRequest, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Unauthorized)
+                out = utils.unmarshal_json(http_res.text, errors.Unauthorized, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 403:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Forbidden)
+                out = utils.unmarshal_json(http_res.text, errors.Forbidden, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 404:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.NotFound)
+                out = utils.unmarshal_json(http_res.text, errors.NotFound, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 409:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.Conflict)
+                out = utils.unmarshal_json(http_res.text, errors.Conflict, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 410:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InviteExpired)
+                out = utils.unmarshal_json(http_res.text, errors.InviteExpired, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 422:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity)
+                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 429:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded)
+                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 500:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.InternalServerError)
+                out = utils.unmarshal_json(http_res.text, errors.InternalServerError, infer_missing=True)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
```

### Comparing `dub-0.0.5/src/dub.egg-info/PKG-INFO` & `dub-0.0.6/src/dub.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dub
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/dubinc/dub-python.git
 Author: Speakeasy
 License: UNKNOWN
 Description: # dub
         
         <div align="left">
@@ -41,14 +41,15 @@
         from dub.models import operations
         
         s = dub.Dub(
             token="DUB_API_KEY",
             workspace_id='<value>',
         )
         
+        
         res = s.links.create(request=operations.CreateLinkRequestBody(
             url='https://google/com',
             external_id='123456',
             tag_ids=[
                 'clux0rgak00011...',
             ],
         ))
@@ -66,14 +67,15 @@
         from dub.models import operations
         
         s = dub.Dub(
             token="DUB_API_KEY",
             workspace_id='<value>',
         )
         
+        
         res = s.links.upsert(request=operations.UpsertLinkRequestBody(
             url='https://google/com',
             external_id='123456',
             tag_ids=[
                 'clux0rgak00011...',
             ],
         ))
@@ -101,37 +103,15 @@
         
         ### [qr_codes](https://github.com/dubinc/dub-python/blob/master/docs/sdks/qrcodes/README.md)
         
         * [get](https://github.com/dubinc/dub-python/blob/master/docs/sdks/qrcodes/README.md#get) - Retrieve a QR code
         
         ### [analytics](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md)
         
-        * [~~timeseries~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#timeseries) - Retrieve timeseries click analytics :warning: **Deprecated** Use `timeseries` instead.
-        * [~~country~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#country) - Retrieve top countries by clicks :warning: **Deprecated** Use `countries` instead.
-        * [~~city~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#city) - Retrieve top cities by clicks :warning: **Deprecated** Use `cities` instead.
-        * [~~device~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#device) - Retrieve top devices by clicks :warning: **Deprecated** Use `devices` instead.
-        * [~~browser~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#browser) - Retrieve top browsers by clicks :warning: **Deprecated** Use `browsers` instead.
-        * [~~os~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#os) - Retrieve top OS by clicks :warning: **Deprecated** Use `os` instead.
-        * [~~referer~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#referer) - Retrieve top referers by clicks :warning: **Deprecated** Use `referers` instead.
-        * [~~top_links~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#top_links) - Retrieve top links by clicks :warning: **Deprecated** Use `top_links` instead.
-        * [~~top_urls~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#top_urls) - Retrieve top URLs by clicks :warning: **Deprecated** Use `top_urls` instead.
-        
-        ### [analytics.clicks](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md)
-        
-        * [count](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#count) - Retrieve the total clicks count
-        * [timeseries](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#timeseries) - Retrieve timeseries click analytics
-        * [countries](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#countries) - Retrieve top countries by clicks
-        * [cities](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#cities) - Retrieve top cities by clicks
-        * [devices](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#devices) - Retrieve top devices by clicks
-        * [browsers](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#browsers) - Retrieve top browsers by clicks
-        * [os](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#os) - Retrieve top OS by clicks
-        * [referers](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#referers) - Retrieve top referers by clicks
-        * [top_links](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#top_links) - Retrieve top links by clicks
-        * [top_urls](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#top_urls) - Retrieve top URLs by clicks
-        * [~~get_clicks_count_deprecated~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#get_clicks_count_deprecated) - Retrieve the total clicks count :warning: **Deprecated** Use `count` instead.
+        * [retrieve](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#retrieve) - Retrieve analytics for a link, a domain, or the authenticated workspace.
         
         ### [workspaces](https://github.com/dubinc/dub-python/blob/master/docs/sdks/workspaces/README.md)
         
         * [list](https://github.com/dubinc/dub-python/blob/master/docs/sdks/workspaces/README.md#list) - Retrieve a list of workspaces
         * [create](https://github.com/dubinc/dub-python/blob/master/docs/sdks/workspaces/README.md#create) - Create a workspace
         * [get](https://github.com/dubinc/dub-python/blob/master/docs/sdks/workspaces/README.md#get) - Retrieve a workspace
         
@@ -188,14 +168,15 @@
             token="DUB_API_KEY",
             workspace_id='<value>',
         )
         
         res = None
         try:
             res = s.links.list(request=operations.GetLinksRequest())
+        
         except errors.BadRequest as e:
             # handle exception
             raise(e)
         except errors.Unauthorized as e:
             # handle exception
             raise(e)
         except errors.Forbidden as e:
@@ -249,14 +230,15 @@
         
         s = dub.Dub(
             server_idx=0,
             token="DUB_API_KEY",
             workspace_id='<value>',
         )
         
+        
         res = s.links.list(request=operations.GetLinksRequest())
         
         if res.link_schemas is not None:
             # handle response
             pass
         
         ```
@@ -271,14 +253,15 @@
         
         s = dub.Dub(
             server_url="https://api.dub.co",
             token="DUB_API_KEY",
             workspace_id='<value>',
         )
         
+        
         res = s.links.list(request=operations.GetLinksRequest())
         
         if res.link_schemas is not None:
             # handle response
             pass
         
         ```
@@ -317,14 +300,15 @@
         from dub.models import operations
         
         s = dub.Dub(
             token="DUB_API_KEY",
             workspace_id='<value>',
         )
         
+        
         res = s.links.list(request=operations.GetLinksRequest())
         
         if res.link_schemas is not None:
             # handle response
             pass
         
         ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dub Version: 0.0.5 Summary: Python Client SDK
+Metadata-Version: 2.1 Name: dub Version: 0.0.6 Summary: Python Client SDK
 Generated by Speakeasy Home-page: https://github.com/dubinc/dub-python.git
 Author: Speakeasy License: UNKNOWN Description: # dub
 _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
 _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
 ## ð **Welcome to your new SDK!** ð It has been generated successfully
 based on your OpenAPI spec. However, it is not yet ready for production use.
@@ -36,82 +36,41 @@
 Update a link * [create_many](https://github.com/dubinc/dub-python/blob/master/
 docs/sdks/links/README.md#create_many) - Bulk create links * [upsert](https://
 github.com/dubinc/dub-python/blob/master/docs/sdks/links/README.md#upsert) -
 Upsert a link ### [qr_codes](https://github.com/dubinc/dub-python/blob/master/
 docs/sdks/qrcodes/README.md) * [get](https://github.com/dubinc/dub-python/blob/
 master/docs/sdks/qrcodes/README.md#get) - Retrieve a QR code ### [analytics]
 (https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/
-README.md) * [~~timeseries~~](https://github.com/dubinc/dub-python/blob/master/
-docs/sdks/analytics/README.md#timeseries) - Retrieve timeseries click analytics
-:warning: **Deprecated** Use `timeseries` instead. * [~~country~~](https://
-github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#country)
-- Retrieve top countries by clicks :warning: **Deprecated** Use `countries`
-instead. * [~~city~~](https://github.com/dubinc/dub-python/blob/master/docs/
-sdks/analytics/README.md#city) - Retrieve top cities by clicks :warning:
-**Deprecated** Use `cities` instead. * [~~device~~](https://github.com/dubinc/
-dub-python/blob/master/docs/sdks/analytics/README.md#device) - Retrieve top
-devices by clicks :warning: **Deprecated** Use `devices` instead. *
-[~~browser~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
-analytics/README.md#browser) - Retrieve top browsers by clicks :warning:
-**Deprecated** Use `browsers` instead. * [~~os~~](https://github.com/dubinc/
-dub-python/blob/master/docs/sdks/analytics/README.md#os) - Retrieve top OS by
-clicks :warning: **Deprecated** Use `os` instead. * [~~referer~~](https://
-github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#referer)
-- Retrieve top referers by clicks :warning: **Deprecated** Use `referers`
-instead. * [~~top_links~~](https://github.com/dubinc/dub-python/blob/master/
-docs/sdks/analytics/README.md#top_links) - Retrieve top links by clicks :
-warning: **Deprecated** Use `top_links` instead. * [~~top_urls~~](https://
-github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/
-README.md#top_urls) - Retrieve top URLs by clicks :warning: **Deprecated** Use
-`top_urls` instead. ### [analytics.clicks](https://github.com/dubinc/dub-
-python/blob/master/docs/sdks/clicks/README.md) * [count](https://github.com/
-dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#count) - Retrieve the
-total clicks count * [timeseries](https://github.com/dubinc/dub-python/blob/
-master/docs/sdks/clicks/README.md#timeseries) - Retrieve timeseries click
-analytics * [countries](https://github.com/dubinc/dub-python/blob/master/docs/
-sdks/clicks/README.md#countries) - Retrieve top countries by clicks * [cities]
-(https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/
-README.md#cities) - Retrieve top cities by clicks * [devices](https://
-github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#devices) -
-Retrieve top devices by clicks * [browsers](https://github.com/dubinc/dub-
-python/blob/master/docs/sdks/clicks/README.md#browsers) - Retrieve top browsers
-by clicks * [os](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
-clicks/README.md#os) - Retrieve top OS by clicks * [referers](https://
-github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#referers) -
-Retrieve top referers by clicks * [top_links](https://github.com/dubinc/dub-
-python/blob/master/docs/sdks/clicks/README.md#top_links) - Retrieve top links
-by clicks * [top_urls](https://github.com/dubinc/dub-python/blob/master/docs/
-sdks/clicks/README.md#top_urls) - Retrieve top URLs by clicks *
-[~~get_clicks_count_deprecated~~](https://github.com/dubinc/dub-python/blob/
-master/docs/sdks/clicks/README.md#get_clicks_count_deprecated) - Retrieve the
-total clicks count :warning: **Deprecated** Use `count` instead. ###
-[workspaces](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
-workspaces/README.md) * [list](https://github.com/dubinc/dub-python/blob/
-master/docs/sdks/workspaces/README.md#list) - Retrieve a list of workspaces *
-[create](https://github.com/dubinc/dub-python/blob/master/docs/sdks/workspaces/
-README.md#create) - Create a workspace * [get](https://github.com/dubinc/dub-
-python/blob/master/docs/sdks/workspaces/README.md#get) - Retrieve a workspace
-### [tags](https://github.com/dubinc/dub-python/blob/master/docs/sdks/tags/
-README.md) * [list](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
-tags/README.md#list) - Retrieve a list of tags * [create](https://github.com/
-dubinc/dub-python/blob/master/docs/sdks/tags/README.md#create) - Create a new
-tag ### [domains](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
-domains/README.md) * [list](https://github.com/dubinc/dub-python/blob/master/
-docs/sdks/domains/README.md#list) - Retrieve a list of domains * [add](https://
-github.com/dubinc/dub-python/blob/master/docs/sdks/domains/README.md#add) - Add
-a domain * [delete](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
-domains/README.md#delete) - Delete a domain * [update](https://github.com/
-dubinc/dub-python/blob/master/docs/sdks/domains/README.md#update) - Update a
-domain * [set_primary](https://github.com/dubinc/dub-python/blob/master/docs/
-sdks/domains/README.md#set_primary) - Set a domain as primary * [transfer]
-(https://github.com/dubinc/dub-python/blob/master/docs/sdks/domains/
-README.md#transfer) - Transfer a domain ### [track](https://github.com/dubinc/
-dub-python/blob/master/docs/sdks/track/README.md) * [lead](https://github.com/
-dubinc/dub-python/blob/master/docs/sdks/track/README.md#lead) - Track a lead *
-[sale](https://github.com/dubinc/dub-python/blob/master/docs/sdks/track/
+README.md) * [retrieve](https://github.com/dubinc/dub-python/blob/master/docs/
+sdks/analytics/README.md#retrieve) - Retrieve analytics for a link, a domain,
+or the authenticated workspace. ### [workspaces](https://github.com/dubinc/dub-
+python/blob/master/docs/sdks/workspaces/README.md) * [list](https://github.com/
+dubinc/dub-python/blob/master/docs/sdks/workspaces/README.md#list) - Retrieve a
+list of workspaces * [create](https://github.com/dubinc/dub-python/blob/master/
+docs/sdks/workspaces/README.md#create) - Create a workspace * [get](https://
+github.com/dubinc/dub-python/blob/master/docs/sdks/workspaces/README.md#get) -
+Retrieve a workspace ### [tags](https://github.com/dubinc/dub-python/blob/
+master/docs/sdks/tags/README.md) * [list](https://github.com/dubinc/dub-python/
+blob/master/docs/sdks/tags/README.md#list) - Retrieve a list of tags * [create]
+(https://github.com/dubinc/dub-python/blob/master/docs/sdks/tags/
+README.md#create) - Create a new tag ### [domains](https://github.com/dubinc/
+dub-python/blob/master/docs/sdks/domains/README.md) * [list](https://
+github.com/dubinc/dub-python/blob/master/docs/sdks/domains/README.md#list) -
+Retrieve a list of domains * [add](https://github.com/dubinc/dub-python/blob/
+master/docs/sdks/domains/README.md#add) - Add a domain * [delete](https://
+github.com/dubinc/dub-python/blob/master/docs/sdks/domains/README.md#delete) -
+Delete a domain * [update](https://github.com/dubinc/dub-python/blob/master/
+docs/sdks/domains/README.md#update) - Update a domain * [set_primary](https://
+github.com/dubinc/dub-python/blob/master/docs/sdks/domains/
+README.md#set_primary) - Set a domain as primary * [transfer](https://
+github.com/dubinc/dub-python/blob/master/docs/sdks/domains/README.md#transfer)
+- Transfer a domain ### [track](https://github.com/dubinc/dub-python/blob/
+master/docs/sdks/track/README.md) * [lead](https://github.com/dubinc/dub-
+python/blob/master/docs/sdks/track/README.md#lead) - Track a lead * [sale]
+(https://github.com/dubinc/dub-python/blob/master/docs/sdks/track/
 README.md#sale) - Track a sale * [customer](https://github.com/dubinc/dub-
 python/blob/master/docs/sdks/track/README.md#customer) - Track a customer ###
 [metatags](https://github.com/dubinc/dub-python/blob/master/docs/sdks/metatags/
 README.md) * [get](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
 metatags/README.md#get) - Retrieve the metatags for a URL ## Error Handling
 Handling errors in this SDK should largely match your expectations. All
 operations return a response object or raise an error. If Error objects are
```

### Comparing `dub-0.0.5/src/dub.egg-info/SOURCES.txt` & `dub-0.0.6/src/dub.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+LICENSE
 README.md
 setup.py
 src/dub/__init__.py
 src/dub/analytics.py
-src/dub/clicks.py
 src/dub/domains.py
 src/dub/links.py
 src/dub/metatags.py
 src/dub/qr_codes.py
 src/dub/sdk.py
 src/dub/sdkconfiguration.py
 src/dub/tags.py
@@ -19,21 +19,49 @@
 src/dub.egg-info/top_level.txt
 src/dub/_hooks/__init__.py
 src/dub/_hooks/registration.py
 src/dub/_hooks/sdkhooks.py
 src/dub/_hooks/types.py
 src/dub/models/__init__.py
 src/dub/models/components/__init__.py
-src/dub/models/components/clicksbycities.py
-src/dub/models/components/clicksbycountry.py
+src/dub/models/components/clicksbrowsers.py
+src/dub/models/components/clickscities.py
+src/dub/models/components/clickscount.py
+src/dub/models/components/clickscountries.py
+src/dub/models/components/clicksdevices.py
+src/dub/models/components/clicksos.py
+src/dub/models/components/clicksreferers.py
+src/dub/models/components/clickstimeseries.py
+src/dub/models/components/clickstoplinks.py
+src/dub/models/components/clickstopurls.py
 src/dub/models/components/countrycode.py
 src/dub/models/components/domainschema.py
 src/dub/models/components/httpmetadata.py
+src/dub/models/components/leadsbrowsers.py
+src/dub/models/components/leadscities.py
+src/dub/models/components/leadscount.py
+src/dub/models/components/leadscountries.py
+src/dub/models/components/leadsdevices.py
+src/dub/models/components/leadsos.py
+src/dub/models/components/leadsreferers.py
+src/dub/models/components/leadstimeseries.py
+src/dub/models/components/leadstoplinks.py
+src/dub/models/components/leadstopurls.py
 src/dub/models/components/linkgeotargeting.py
 src/dub/models/components/linkschema.py
+src/dub/models/components/salesbrowsers.py
+src/dub/models/components/salescities.py
+src/dub/models/components/salescount.py
+src/dub/models/components/salescountries.py
+src/dub/models/components/salesdevices.py
+src/dub/models/components/salesos.py
+src/dub/models/components/salesreferers.py
+src/dub/models/components/salestimeseries.py
+src/dub/models/components/salestoplinks.py
+src/dub/models/components/salestopurls.py
 src/dub/models/components/security.py
 src/dub/models/components/tagschema.py
 src/dub/models/components/workspaceschema.py
 src/dub/models/errors/__init__.py
 src/dub/models/errors/badrequest.py
 src/dub/models/errors/conflict.py
 src/dub/models/errors/forbidden.py
@@ -50,43 +78,24 @@
 src/dub/models/operations/adddomain.py
 src/dub/models/operations/bulkcreatelinks.py
 src/dub/models/operations/createlink.py
 src/dub/models/operations/createtag.py
 src/dub/models/operations/createworkspace.py
 src/dub/models/operations/deletedomain.py
 src/dub/models/operations/deletelink.py
-src/dub/models/operations/getbrowsersbyclicks.py
-src/dub/models/operations/getbrowsersbyclicksdeprecated.py
-src/dub/models/operations/getcitiesbyclicks.py
-src/dub/models/operations/getcitiesbyclicksdeprecated.py
-src/dub/models/operations/getclickscount.py
-src/dub/models/operations/getclickscountdeprecated.py
-src/dub/models/operations/getcountriesbyclicks.py
-src/dub/models/operations/getcountriesbyclicksdeprecated.py
-src/dub/models/operations/getdevicesbyclicks.py
-src/dub/models/operations/getdevicesbyclicksdeprecated.py
 src/dub/models/operations/getlinkinfo.py
 src/dub/models/operations/getlinks.py
 src/dub/models/operations/getlinkscount.py
 src/dub/models/operations/getmetatags.py
-src/dub/models/operations/getosbyclicks.py
-src/dub/models/operations/getosbyclicksdeprecated.py
 src/dub/models/operations/getqrcode.py
-src/dub/models/operations/getreferersbyclicks.py
-src/dub/models/operations/getreferersbyclicksdeprecated.py
 src/dub/models/operations/gettags.py
-src/dub/models/operations/gettimeseriesbyclicks.py
-src/dub/models/operations/gettimeseriesbyclicksdeprecated.py
-src/dub/models/operations/gettoplinksbyclicks.py
-src/dub/models/operations/gettoplinksbyclicksdeprecated.py
-src/dub/models/operations/gettopurlsbyclicks.py
-src/dub/models/operations/gettopurlsbyclicksdeprecated.py
 src/dub/models/operations/getworkspace.py
 src/dub/models/operations/getworkspaces.py
 src/dub/models/operations/listdomains.py
+src/dub/models/operations/retrieveanalytics.py
 src/dub/models/operations/setprimarydomain.py
 src/dub/models/operations/trackcustomer.py
 src/dub/models/operations/tracklead.py
 src/dub/models/operations/tracksale.py
 src/dub/models/operations/transferdomain.py
 src/dub/models/operations/updatedomain.py
 src/dub/models/operations/updatelink.py
```

