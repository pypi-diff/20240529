# Comparing `tmp/aliyun-python-sdk-ddoscoo-1.0.5.tar.gz` & `tmp/aliyun-python-sdk-ddoscoo-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-ddoscoo-1.0.5.tar", last modified: Thu Jun 30 09:47:07 2022, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-ddoscoo-1.0.6.tar", last modified: Wed May 29 02:38:17 2024, max compression
```

## Comparing `aliyun-python-sdk-ddoscoo-1.0.5.tar` & `aliyun-python-sdk-ddoscoo-1.0.6.tar`

### file list

```diff
@@ -1,180 +1,195 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-30 09:47:07.000000 aliyun-python-sdk-ddoscoo-1.0.5/
--rw-r--r--   0 root         (0) root         (0)      575 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1557 2022-06-30 09:47:07.000000 aliyun-python-sdk-ddoscoo-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      535 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-30 09:47:07.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyun_python_sdk_ddoscoo.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1557 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyun_python_sdk_ddoscoo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11186 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyun_python_sdk_ddoscoo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyun_python_sdk_ddoscoo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyun_python_sdk_ddoscoo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyun_python_sdk_ddoscoo.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-30 09:47:07.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/
--rw-r--r--   0 root         (0) root         (0)       21 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1088 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-30 09:47:07.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-30 09:47:07.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/
--rw-r--r--   0 root         (0) root         (0)     1849 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/AddAutoCcBlacklistRequest.py
--rw-r--r--   0 root         (0) root         (0)     1849 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/AddAutoCcWhitelistRequest.py
--rw-r--r--   0 root         (0) root         (0)     2316 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/AssociateWebCertRequest.py
--rw-r--r--   0 root         (0) root         (0)     1835 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/AttachSceneDefenseObjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     1831 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ConfigL7RsPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1465 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ConfigLayer4RemarkRequest.py
--rw-r--r--   0 root         (0) root         (0)     1648 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ConfigLayer4RuleBakModeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1473 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ConfigLayer4RulePolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1650 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ConfigNetworkRegionBlockRequest.py
--rw-r--r--   0 root         (0) root         (0)     1483 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ConfigNetworkRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1634 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ConfigUdpReflectRequest.py
--rw-r--r--   0 root         (0) root         (0)     1849 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ConfigWebCCTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2186 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ConfigWebIpSetRequest.py
--rw-r--r--   0 root         (0) root         (0)     1867 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/CreateAsyncTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2979 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/CreateDomainResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1483 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/CreateNetworkRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2359 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/CreatePortRequest.py
--rw-r--r--   0 root         (0) root         (0)     1976 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/CreateSceneDefensePolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2185 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/CreateSchedulerRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2411 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/CreateTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2765 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/CreateWebCCRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2629 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/CreateWebRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1664 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DeleteAsyncTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1662 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DeleteAutoCcBlacklistRequest.py
--rw-r--r--   0 root         (0) root         (0)     1662 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DeleteAutoCcWhitelistRequest.py
--rw-r--r--   0 root         (0) root         (0)     1451 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DeleteDomainResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1475 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DeleteNetworkRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2359 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DeletePortRequest.py
--rw-r--r--   0 root         (0) root         (0)     1471 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DeleteSceneDefensePolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1682 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DeleteSchedulerRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2374 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DeleteTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1817 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DeleteWebCCRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1943 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DeleteWebCacheCustomRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1947 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DeleteWebPreciseAccessRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1658 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DeleteWebRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1875 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeAsyncTasksRequest.py
--rw-r--r--   0 root         (0) root         (0)     1650 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeAttackAnalysisMaxQpsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2028 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeAutoCcBlacklistRequest.py
--rw-r--r--   0 root         (0) root         (0)     1666 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeAutoCcListCountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2028 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeAutoCcWhitelistRequest.py
--rw-r--r--   0 root         (0) root         (0)     1664 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeBackSourceCidrRequest.py
--rw-r--r--   0 root         (0) root         (0)     1567 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeBlackholeStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1780 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeBlockStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1658 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeCertsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1752 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeCnameReusesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2502 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDDoSEventsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2201 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDDosAllEventListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1795 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDDosEventAreaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1807 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDDosEventAttackTypeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1793 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDDosEventIspRequest.py
--rw-r--r--   0 root         (0) root         (0)     1634 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDDosEventMaxRequest.py
--rw-r--r--   0 root         (0) root         (0)     1954 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDDosEventSrcIpRequest.py
--rw-r--r--   0 root         (0) root         (0)     1525 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDefenseCountStatisticsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2424 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDefenseRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2408 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDomainAttackEventsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2026 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDomainOverviewRequest.py
--rw-r--r--   0 root         (0) root         (0)     2199 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDomainQPSListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2034 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDomainQpsWithCacheRequest.py
--rw-r--r--   0 root         (0) root         (0)     2345 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDomainResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2040 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDomainStatusCodeCountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2398 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDomainStatusCodeListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1869 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDomainTopAttackListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2048 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDomainViewSourceCountriesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2048 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDomainViewSourceProvincesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2191 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDomainViewTopCostTimeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2181 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDomainViewTopUrlRequest.py
--rw-r--r--   0 root         (0) root         (0)     1772 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDomainsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1491 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeElasticBandwidthSpecRequest.py
--rw-r--r--   0 root         (0) root         (0)     1493 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeHealthCheckListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1497 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeHealthCheckStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1567 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeInstanceDetailsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1955 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeInstanceIdsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1563 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeInstanceSpecsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1573 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeInstanceStatisticsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1678 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeInstanceStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     3889 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1945 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeL7RsPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1477 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeLayer4RulePolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1519 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeLogStoreExistStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1487 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeNetworkRegionBlockRequest.py
--rw-r--r--   0 root         (0) root         (0)     1505 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeNetworkRuleAttributesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2275 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeNetworkRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2621 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeOpEntitiesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2142 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribePortAttackMaxFlowRequest.py
--rw-r--r--   0 root         (0) root         (0)     1569 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribePortAutoCcStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2291 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribePortConnsCountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2470 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribePortConnsListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2313 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribePortFlowListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2132 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribePortMaxConnsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2265 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribePortRequest.py
--rw-r--r--   0 root         (0) root         (0)     2154 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribePortViewSourceCountriesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2144 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribePortViewSourceIspsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2154 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribePortViewSourceProvincesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1698 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeSceneDefenseObjectsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1867 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeSceneDefensePoliciesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2062 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeSchedulerRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1507 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeSlsAuthStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1511 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeSlsLogstoreInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1507 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeSlsOpenStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1664 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeStsGrantStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2398 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeSystemLogRequest.py
--rw-r--r--   0 root         (0) root         (0)     2072 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeTagKeysRequest.py
--rw-r--r--   0 root         (0) root         (0)     2600 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1471 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeUdpReflectRequest.py
--rw-r--r--   0 root         (0) root         (0)     1513 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeUnBlackholeCountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1505 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeUnBlockCountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1907 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeWebAccessLogDispatchStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1525 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeWebAccessLogEmptyCountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1684 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeWebAccessLogStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1535 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeWebAccessModeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1768 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeWebAreaBlockConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2040 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeWebCCRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1760 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeWebCacheConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1766 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeWebCcProtectSwitchRequest.py
--rw-r--r--   0 root         (0) root         (0)     1509 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeWebCustomPortsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1770 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeWebInstanceRelationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1770 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeWebPreciseAccessRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2715 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeWebRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1835 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DetachSceneDefenseObjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     1473 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DisableSceneDefensePolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1682 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DisableWebAccessLogConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1656 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DisableWebCCRequest.py
--rw-r--r--   0 root         (0) root         (0)     1664 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DisableWebCCRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1475 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/EmptyAutoCcBlacklistRequest.py
--rw-r--r--   0 root         (0) root         (0)     1475 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/EmptyAutoCcWhitelistRequest.py
--rw-r--r--   0 root         (0) root         (0)     1497 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/EmptySlsLogstoreRequest.py
--rw-r--r--   0 root         (0) root         (0)     1471 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/EnableSceneDefensePolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1680 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/EnableWebAccessLogConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1654 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/EnableWebCCRequest.py
--rw-r--r--   0 root         (0) root         (0)     1662 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/EnableWebCCRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1698 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyBlackholeStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2052 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyBlockStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1994 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyCnameReuseRequest.py
--rw-r--r--   0 root         (0) root         (0)     2979 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyDomainResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1708 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyElasticBandWidthRequest.py
--rw-r--r--   0 root         (0) root         (0)     1648 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyFullLogTtlRequest.py
--rw-r--r--   0 root         (0) root         (0)     2104 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyHealthCheckConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1835 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyHttp2EnableRequest.py
--rw-r--r--   0 root         (0) root         (0)     1642 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyInstanceRemarkRequest.py
--rw-r--r--   0 root         (0) root         (0)     2080 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyNetworkRuleAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1801 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyPortAutoCcStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2359 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyPortRequest.py
--rw-r--r--   0 root         (0) root         (0)     2155 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifySceneDefensePolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2185 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifySchedulerRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1829 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyTlsConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1843 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyWebAIProtectModeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1847 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyWebAIProtectSwitchRequest.py
--rw-r--r--   0 root         (0) root         (0)     1642 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyWebAccessModeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1917 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyWebAreaBlockRequest.py
--rw-r--r--   0 root         (0) root         (0)     1847 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyWebAreaBlockSwitchRequest.py
--rw-r--r--   0 root         (0) root         (0)     2765 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyWebCCRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1841 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyWebCacheCustomRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1823 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyWebCacheModeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1841 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyWebCacheSwitchRequest.py
--rw-r--r--   0 root         (0) root         (0)     1839 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyWebIpSetSwitchRequest.py
--rw-r--r--   0 root         (0) root         (0)     2020 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyWebPreciseAccessRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1855 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyWebPreciseAccessSwitchRequest.py
--rw-r--r--   0 root         (0) root         (0)     2751 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyWebRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1465 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ReleaseInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1833 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/SwitchSchedulerRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2022-06-30 09:47:07.000000 aliyun-python-sdk-ddoscoo-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2472 2022-06-30 09:47:06.000000 aliyun-python-sdk-ddoscoo-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)      575 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1557 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      535 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyun_python_sdk_ddoscoo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1557 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyun_python_sdk_ddoscoo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12177 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyun_python_sdk_ddoscoo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyun_python_sdk_ddoscoo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyun_python_sdk_ddoscoo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyun_python_sdk_ddoscoo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/
+-rw-r--r--   0 root         (0) root         (0)     1859 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/AddAutoCcBlacklistRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1859 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/AddAutoCcWhitelistRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2725 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/AssociateWebCertRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/AttachSceneDefenseObjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2052 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ConfigL7RsPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ConfigLayer4RealLimitRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1475 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ConfigLayer4RemarkRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ConfigLayer4RuleBakModeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1483 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ConfigLayer4RulePolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ConfigNetworkRegionBlockRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1493 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ConfigNetworkRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ConfigUdpReflectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1859 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ConfigWebCCTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2196 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ConfigWebIpSetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1877 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/CreateAsyncTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2905 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/CreateDomainResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1493 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/CreateNetworkRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2369 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/CreatePortRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1986 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/CreateSceneDefensePolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/CreateSchedulerRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2421 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/CreateTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2775 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/CreateWebCCRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2639 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/CreateWebRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DeleteAsyncTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1672 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DeleteAutoCcBlacklistRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1672 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DeleteAutoCcWhitelistRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1461 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DeleteDomainResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1485 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DeleteNetworkRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2369 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DeletePortRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1481 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DeleteSceneDefensePolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1692 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DeleteSchedulerRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2384 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DeleteTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1827 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DeleteWebCCRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1953 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DeleteWebCacheCustomRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1957 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DeleteWebPreciseAccessRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DeleteWebRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1885 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeAsyncTasksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeAttackAnalysisMaxQpsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeAutoCcBlacklistRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeAutoCcListCountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeAutoCcWhitelistRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1859 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeBackSourceCidrRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeBlackholeStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1790 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeBlockStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeCertsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeCnameReusesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2512 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDDoSEventsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2211 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDDosAllEventListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1805 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDDosEventAreaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1817 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDDosEventAttackTypeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1803 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDDosEventIspRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDDosEventMaxRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDDosEventSrcIpRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDefenseCountStatisticsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2434 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDefenseRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2418 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDomainAttackEventsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2036 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDomainOverviewRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2209 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDomainQPSListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2355 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDomainResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDomainSecurityProfileRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2050 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDomainStatusCodeCountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2408 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDomainStatusCodeListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1879 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDomainTopAttackListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDomainViewSourceCountriesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDomainViewSourceProvincesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2201 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDomainViewTopCostTimeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2191 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDomainViewTopUrlRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDomainsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1501 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeElasticBandwidthSpecRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1795 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeElasticQpsRecordRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2129 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeElasticQpsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1672 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeHeadersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1503 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeHealthCheckListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1507 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeHealthCheckStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeInstanceDetailsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeInstanceExtRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1965 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeInstanceIdsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1573 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeInstanceSpecsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1583 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeInstanceStatisticsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1688 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeInstanceStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3899 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1955 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeL7RsPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeLayer4RulePolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1529 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeLogStoreExistStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeNetworkRegionBlockRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1515 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeNetworkRuleAttributesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2285 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeNetworkRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2631 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeOpEntitiesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribePortAttackMaxFlowRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1579 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribePortAutoCcStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1970 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribePortCcAttackTopIPRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2301 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribePortConnsCountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2480 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribePortConnsListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2323 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribePortFlowListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2142 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribePortMaxConnsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2275 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribePortRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2164 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribePortViewSourceCountriesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2154 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribePortViewSourceIspsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2164 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribePortViewSourceProvincesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeSceneDefenseObjectsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1877 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeSceneDefensePoliciesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2072 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeSchedulerRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2280 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeSlaEventListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeSlsAuthStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1521 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeSlsLogstoreInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeSlsOpenStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeStsGrantStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2408 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeSystemLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2082 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeTagKeysRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2610 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2154 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeTotalAttackMaxFlowRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1481 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeUdpReflectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1523 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeUnBlackholeCountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1515 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeUnBlockCountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeWebAccessLogDispatchStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeWebAccessLogEmptyCountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1694 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeWebAccessLogStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1545 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeWebAccessModeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1778 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeWebAreaBlockConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2050 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeWebCCRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1770 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeWebCacheConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1776 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeWebCcProtectSwitchRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1519 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeWebCustomPortsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1780 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeWebInstanceRelationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1780 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeWebPreciseAccessRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2332 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeWebReportTopIpRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2725 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeWebRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DetachSceneDefenseObjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1483 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DisableSceneDefensePolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1692 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DisableWebAccessLogConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DisableWebCCRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DisableWebCCRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1485 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/EmptyAutoCcBlacklistRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1485 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/EmptyAutoCcWhitelistRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1507 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/EmptySlsLogstoreRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1481 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/EnableSceneDefensePolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1690 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/EnableWebAccessLogConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/EnableWebCCRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1672 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/EnableWebCCRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyBizBandWidthModeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyBlackholeStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyBlockStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyCnameReuseRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2905 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyDomainResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1718 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyElasticBandWidthRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1897 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyElasticBizBandWidthRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1843 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyElasticBizQpsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyFullLogTtlRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1877 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyHeadersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyHealthCheckConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyHttp2EnableRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyInstanceRemarkRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2090 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyNetworkRuleAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1622 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyOcspStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyPortAutoCcStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2369 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyPortRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyQpsModeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2165 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifySceneDefensePolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifySchedulerRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1839 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyTlsConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1853 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyWebAIProtectModeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1857 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyWebAIProtectSwitchRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyWebAccessModeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1927 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyWebAreaBlockRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1857 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyWebAreaBlockSwitchRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2775 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyWebCCRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyWebCacheCustomRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyWebCacheModeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyWebCacheSwitchRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyWebIpSetSwitchRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2030 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyWebPreciseAccessRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1865 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyWebPreciseAccessSwitchRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2761 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyWebRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1475 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ReleaseInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1843 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/SwitchSchedulerRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2472 2024-05-29 02:38:16.000000 aliyun-python-sdk-ddoscoo-1.0.6/setup.py
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/LICENSE` & `aliyun-python-sdk-ddoscoo-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/PKG-INFO` & `aliyun-python-sdk-ddoscoo-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-ddoscoo
-Version: 1.0.5
+Version: 1.0.6
 Summary: The ddoscoo module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-ddoscoo
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/README.rst` & `aliyun-python-sdk-ddoscoo-1.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyun_python_sdk_ddoscoo.egg-info/PKG-INFO` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyun_python_sdk_ddoscoo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-ddoscoo
-Version: 1.0.5
+Version: 1.0.6
 Summary: The ddoscoo module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-ddoscoo
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyun_python_sdk_ddoscoo.egg-info/SOURCES.txt` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyun_python_sdk_ddoscoo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 aliyunsdkddoscoo/endpoint.py
 aliyunsdkddoscoo/request/__init__.py
 aliyunsdkddoscoo/request/v20200101/AddAutoCcBlacklistRequest.py
 aliyunsdkddoscoo/request/v20200101/AddAutoCcWhitelistRequest.py
 aliyunsdkddoscoo/request/v20200101/AssociateWebCertRequest.py
 aliyunsdkddoscoo/request/v20200101/AttachSceneDefenseObjectRequest.py
 aliyunsdkddoscoo/request/v20200101/ConfigL7RsPolicyRequest.py
+aliyunsdkddoscoo/request/v20200101/ConfigLayer4RealLimitRequest.py
 aliyunsdkddoscoo/request/v20200101/ConfigLayer4RemarkRequest.py
 aliyunsdkddoscoo/request/v20200101/ConfigLayer4RuleBakModeRequest.py
 aliyunsdkddoscoo/request/v20200101/ConfigLayer4RulePolicyRequest.py
 aliyunsdkddoscoo/request/v20200101/ConfigNetworkRegionBlockRequest.py
 aliyunsdkddoscoo/request/v20200101/ConfigNetworkRulesRequest.py
 aliyunsdkddoscoo/request/v20200101/ConfigUdpReflectRequest.py
 aliyunsdkddoscoo/request/v20200101/ConfigWebCCTemplateRequest.py
@@ -64,99 +65,113 @@
 aliyunsdkddoscoo/request/v20200101/DescribeDDosEventMaxRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeDDosEventSrcIpRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeDefenseCountStatisticsRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeDefenseRecordsRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeDomainAttackEventsRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeDomainOverviewRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeDomainQPSListRequest.py
-aliyunsdkddoscoo/request/v20200101/DescribeDomainQpsWithCacheRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeDomainResourceRequest.py
+aliyunsdkddoscoo/request/v20200101/DescribeDomainSecurityProfileRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeDomainStatusCodeCountRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeDomainStatusCodeListRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeDomainTopAttackListRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeDomainViewSourceCountriesRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeDomainViewSourceProvincesRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeDomainViewTopCostTimeRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeDomainViewTopUrlRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeDomainsRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeElasticBandwidthSpecRequest.py
+aliyunsdkddoscoo/request/v20200101/DescribeElasticQpsRecordRequest.py
+aliyunsdkddoscoo/request/v20200101/DescribeElasticQpsRequest.py
+aliyunsdkddoscoo/request/v20200101/DescribeHeadersRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeHealthCheckListRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeHealthCheckStatusRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeInstanceDetailsRequest.py
+aliyunsdkddoscoo/request/v20200101/DescribeInstanceExtRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeInstanceIdsRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeInstanceSpecsRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeInstanceStatisticsRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeInstanceStatusRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeInstancesRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeL7RsPolicyRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeLayer4RulePolicyRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeLogStoreExistStatusRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeNetworkRegionBlockRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeNetworkRuleAttributesRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeNetworkRulesRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeOpEntitiesRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribePortAttackMaxFlowRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribePortAutoCcStatusRequest.py
+aliyunsdkddoscoo/request/v20200101/DescribePortCcAttackTopIPRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribePortConnsCountRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribePortConnsListRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribePortFlowListRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribePortMaxConnsRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribePortRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribePortViewSourceCountriesRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribePortViewSourceIspsRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribePortViewSourceProvincesRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeSceneDefenseObjectsRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeSceneDefensePoliciesRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeSchedulerRulesRequest.py
+aliyunsdkddoscoo/request/v20200101/DescribeSlaEventListRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeSlsAuthStatusRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeSlsLogstoreInfoRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeSlsOpenStatusRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeStsGrantStatusRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeSystemLogRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeTagKeysRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeTagResourcesRequest.py
+aliyunsdkddoscoo/request/v20200101/DescribeTotalAttackMaxFlowRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeUdpReflectRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeUnBlackholeCountRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeUnBlockCountRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeWebAccessLogDispatchStatusRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeWebAccessLogEmptyCountRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeWebAccessLogStatusRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeWebAccessModeRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeWebAreaBlockConfigsRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeWebCCRulesRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeWebCacheConfigsRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeWebCcProtectSwitchRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeWebCustomPortsRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeWebInstanceRelationsRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeWebPreciseAccessRuleRequest.py
+aliyunsdkddoscoo/request/v20200101/DescribeWebReportTopIpRequest.py
 aliyunsdkddoscoo/request/v20200101/DescribeWebRulesRequest.py
 aliyunsdkddoscoo/request/v20200101/DetachSceneDefenseObjectRequest.py
 aliyunsdkddoscoo/request/v20200101/DisableSceneDefensePolicyRequest.py
 aliyunsdkddoscoo/request/v20200101/DisableWebAccessLogConfigRequest.py
 aliyunsdkddoscoo/request/v20200101/DisableWebCCRequest.py
 aliyunsdkddoscoo/request/v20200101/DisableWebCCRuleRequest.py
 aliyunsdkddoscoo/request/v20200101/EmptyAutoCcBlacklistRequest.py
 aliyunsdkddoscoo/request/v20200101/EmptyAutoCcWhitelistRequest.py
 aliyunsdkddoscoo/request/v20200101/EmptySlsLogstoreRequest.py
 aliyunsdkddoscoo/request/v20200101/EnableSceneDefensePolicyRequest.py
 aliyunsdkddoscoo/request/v20200101/EnableWebAccessLogConfigRequest.py
 aliyunsdkddoscoo/request/v20200101/EnableWebCCRequest.py
 aliyunsdkddoscoo/request/v20200101/EnableWebCCRuleRequest.py
+aliyunsdkddoscoo/request/v20200101/ModifyBizBandWidthModeRequest.py
 aliyunsdkddoscoo/request/v20200101/ModifyBlackholeStatusRequest.py
 aliyunsdkddoscoo/request/v20200101/ModifyBlockStatusRequest.py
 aliyunsdkddoscoo/request/v20200101/ModifyCnameReuseRequest.py
 aliyunsdkddoscoo/request/v20200101/ModifyDomainResourceRequest.py
 aliyunsdkddoscoo/request/v20200101/ModifyElasticBandWidthRequest.py
+aliyunsdkddoscoo/request/v20200101/ModifyElasticBizBandWidthRequest.py
+aliyunsdkddoscoo/request/v20200101/ModifyElasticBizQpsRequest.py
 aliyunsdkddoscoo/request/v20200101/ModifyFullLogTtlRequest.py
+aliyunsdkddoscoo/request/v20200101/ModifyHeadersRequest.py
 aliyunsdkddoscoo/request/v20200101/ModifyHealthCheckConfigRequest.py
 aliyunsdkddoscoo/request/v20200101/ModifyHttp2EnableRequest.py
 aliyunsdkddoscoo/request/v20200101/ModifyInstanceRemarkRequest.py
 aliyunsdkddoscoo/request/v20200101/ModifyNetworkRuleAttributeRequest.py
+aliyunsdkddoscoo/request/v20200101/ModifyOcspStatusRequest.py
 aliyunsdkddoscoo/request/v20200101/ModifyPortAutoCcStatusRequest.py
 aliyunsdkddoscoo/request/v20200101/ModifyPortRequest.py
+aliyunsdkddoscoo/request/v20200101/ModifyQpsModeRequest.py
 aliyunsdkddoscoo/request/v20200101/ModifySceneDefensePolicyRequest.py
 aliyunsdkddoscoo/request/v20200101/ModifySchedulerRuleRequest.py
 aliyunsdkddoscoo/request/v20200101/ModifyTlsConfigRequest.py
 aliyunsdkddoscoo/request/v20200101/ModifyWebAIProtectModeRequest.py
 aliyunsdkddoscoo/request/v20200101/ModifyWebAIProtectSwitchRequest.py
 aliyunsdkddoscoo/request/v20200101/ModifyWebAccessModeRequest.py
 aliyunsdkddoscoo/request/v20200101/ModifyWebAreaBlockRequest.py
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/endpoint.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/AddAutoCcBlacklistRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/AddAutoCcBlacklistRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class AddAutoCcBlacklistRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'AddAutoCcBlacklist')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'AddAutoCcBlacklist','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/AddAutoCcWhitelistRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/AddAutoCcWhitelistRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class AddAutoCcWhitelistRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'AddAutoCcWhitelist')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'AddAutoCcWhitelist','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/AssociateWebCertRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyCnameReuseRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,48 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class AssociateWebCertRequest(RpcRequest):
+class ModifyCnameReuseRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'AssociateWebCert')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyCnameReuse','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_Cert(self): # String
-		return self.get_query_params().get('Cert')
+	def get_Cname(self): # String
+		return self.get_query_params().get('Cname')
 
-	def set_Cert(self, Cert):  # String
-		self.add_query_param('Cert', Cert)
-	def get_CertId(self): # Integer
-		return self.get_query_params().get('CertId')
-
-	def set_CertId(self, CertId):  # Integer
-		self.add_query_param('CertId', CertId)
+	def set_Cname(self, Cname):  # String
+		self.add_query_param('Cname', Cname)
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
-	def get_Key(self): # String
-		return self.get_query_params().get('Key')
-
-	def set_Key(self, Key):  # String
-		self.add_query_param('Key', Key)
-	def get_CertName(self): # String
-		return self.get_query_params().get('CertName')
+	def get_Enable(self): # Integer
+		return self.get_query_params().get('Enable')
 
-	def set_CertName(self, CertName):  # String
-		self.add_query_param('CertName', CertName)
+	def set_Enable(self, Enable):  # Integer
+		self.add_query_param('Enable', Enable)
 	def get_Domain(self): # String
 		return self.get_query_params().get('Domain')
 
 	def set_Domain(self, Domain):  # String
 		self.add_query_param('Domain', Domain)
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/AttachSceneDefenseObjectRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/AttachSceneDefenseObjectRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class AttachSceneDefenseObjectRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'AttachSceneDefenseObject')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'AttachSceneDefenseObject','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ConfigL7RsPolicyRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyWebPreciseAccessSwitchRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class ConfigL7RsPolicyRequest(RpcRequest):
+class ModifyWebPreciseAccessSwitchRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ConfigL7RsPolicy')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyWebPreciseAccessSwitch','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -37,12 +37,12 @@
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
 	def get_Domain(self): # String
 		return self.get_query_params().get('Domain')
 
 	def set_Domain(self, Domain):  # String
 		self.add_query_param('Domain', Domain)
-	def get_Policy(self): # String
-		return self.get_query_params().get('Policy')
+	def get_Config(self): # String
+		return self.get_query_params().get('Config')
 
-	def set_Policy(self, Policy):  # String
-		self.add_query_param('Policy', Policy)
+	def set_Config(self, Config):  # String
+		self.add_query_param('Config', Config)
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ConfigLayer4RemarkRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ConfigLayer4RemarkRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class ConfigLayer4RemarkRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ConfigLayer4Remark')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ConfigLayer4Remark','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ConfigLayer4RuleBakModeRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ConfigLayer4RuleBakModeRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class ConfigLayer4RuleBakModeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ConfigLayer4RuleBakMode')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ConfigLayer4RuleBakMode','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ConfigLayer4RulePolicyRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ConfigLayer4RulePolicyRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class ConfigLayer4RulePolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ConfigLayer4RulePolicy')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ConfigLayer4RulePolicy','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ConfigNetworkRegionBlockRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ConfigNetworkRegionBlockRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class ConfigNetworkRegionBlockRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ConfigNetworkRegionBlock')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ConfigNetworkRegionBlock','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ConfigNetworkRulesRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ConfigNetworkRulesRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class ConfigNetworkRulesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ConfigNetworkRules')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ConfigNetworkRules','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ConfigUdpReflectRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ConfigUdpReflectRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class ConfigUdpReflectRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ConfigUdpReflect')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ConfigUdpReflect','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ConfigWebCCTemplateRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ConfigWebCCTemplateRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class ConfigWebCCTemplateRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ConfigWebCCTemplate')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ConfigWebCCTemplate','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ConfigWebIpSetRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ConfigWebIpSetRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class ConfigWebIpSetRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ConfigWebIpSet')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ConfigWebIpSet','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/CreateAsyncTaskRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/CreateAsyncTaskRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class CreateAsyncTaskRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'CreateAsyncTask')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'CreateAsyncTask','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/CreateDomainResourceRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyDomainResourceRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class CreateDomainResourceRequest(RpcRequest):
+class ModifyDomainResourceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'CreateDomainResource')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyDomainResource','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -49,22 +49,22 @@
 			self.add_query_param('RealServers.' + str(depth1 + 1), RealServers[depth1])
 	def get_InstanceIdss(self): # RepeatList
 		return self.get_query_params().get('InstanceIds')
 
 	def set_InstanceIdss(self, InstanceIds):  # RepeatList
 		for depth1 in range(len(InstanceIds)):
 			self.add_query_param('InstanceIds.' + str(depth1 + 1), InstanceIds[depth1])
-	def get_ProxyTypess(self): # RepeatList
+	def get_ProxyTypes(self): # Array
 		return self.get_query_params().get('ProxyTypes')
 
-	def set_ProxyTypess(self, ProxyTypes):  # RepeatList
-		for depth1 in range(len(ProxyTypes)):
-			if ProxyTypes[depth1].get('ProxyPorts') is not None:
-				for depth2 in range(len(ProxyTypes[depth1].get('ProxyPorts'))):
-					self.add_query_param('ProxyTypes.' + str(depth1 + 1) + '.ProxyPorts.' + str(depth2 + 1), ProxyTypes[depth1].get('ProxyPorts')[depth2])
-			if ProxyTypes[depth1].get('ProxyType') is not None:
-				self.add_query_param('ProxyTypes.' + str(depth1 + 1) + '.ProxyType', ProxyTypes[depth1].get('ProxyType'))
+	def set_ProxyTypes(self, ProxyTypes):  # Array
+		for index1, value1 in enumerate(ProxyTypes):
+			if value1.get('ProxyPorts') is not None:
+				for index2, value2 in enumerate(value1.get('ProxyPorts')):
+					self.add_query_param('ProxyTypes.' + str(index1 + 1) + '.ProxyPorts.' + str(index2 + 1), value2)
+			if value1.get('ProxyType') is not None:
+				self.add_query_param('ProxyTypes.' + str(index1 + 1) + '.ProxyType', value1.get('ProxyType'))
 	def get_Domain(self): # String
 		return self.get_query_params().get('Domain')
 
 	def set_Domain(self, Domain):  # String
 		self.add_query_param('Domain', Domain)
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/CreateNetworkRulesRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/CreateNetworkRulesRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class CreateNetworkRulesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'CreateNetworkRules')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'CreateNetworkRules','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/CreatePortRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/CreatePortRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class CreatePortRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'CreatePort')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'CreatePort','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/CreateSceneDefensePolicyRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/CreateSceneDefensePolicyRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class CreateSceneDefensePolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'CreateSceneDefensePolicy')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'CreateSceneDefensePolicy','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/CreateSchedulerRuleRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/CreateSchedulerRuleRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class CreateSchedulerRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'CreateSchedulerRule')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'CreateSchedulerRule','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/CreateTagResourcesRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/CreateTagResourcesRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class CreateTagResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'CreateTagResources')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'CreateTagResources','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/CreateWebCCRuleRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/CreateWebCCRuleRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class CreateWebCCRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'CreateWebCCRule')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'CreateWebCCRule','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/CreateWebRuleRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/CreateWebRuleRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class CreateWebRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'CreateWebRule')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'CreateWebRule','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DeleteAsyncTaskRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DeleteAsyncTaskRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DeleteAsyncTaskRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DeleteAsyncTask')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DeleteAsyncTask','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DeleteAutoCcBlacklistRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DeleteAutoCcBlacklistRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DeleteAutoCcBlacklistRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DeleteAutoCcBlacklist')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DeleteAutoCcBlacklist','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DeleteAutoCcWhitelistRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DeleteAutoCcWhitelistRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DeleteAutoCcWhitelistRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DeleteAutoCcWhitelist')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DeleteAutoCcWhitelist','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DeleteDomainResourceRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DeleteDomainResourceRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DeleteDomainResourceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DeleteDomainResource')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DeleteDomainResource','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DeleteNetworkRuleRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DeleteNetworkRuleRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DeleteNetworkRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DeleteNetworkRule')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DeleteNetworkRule','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DeletePortRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DeletePortRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DeletePortRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DeletePort')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DeletePort','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DeleteSceneDefensePolicyRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/EnableSceneDefensePolicyRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class DeleteSceneDefensePolicyRequest(RpcRequest):
+class EnableSceneDefensePolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DeleteSceneDefensePolicy')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'EnableSceneDefensePolicy','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DeleteSchedulerRuleRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DeleteSchedulerRuleRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DeleteSchedulerRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DeleteSchedulerRule')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DeleteSchedulerRule','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DeleteTagResourcesRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DeleteTagResourcesRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DeleteTagResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DeleteTagResources')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DeleteTagResources','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DeleteWebCCRuleRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DeleteWebCCRuleRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DeleteWebCCRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DeleteWebCCRule')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DeleteWebCCRule','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DeleteWebCacheCustomRuleRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DeleteWebPreciseAccessRuleRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class DeleteWebCacheCustomRuleRequest(RpcRequest):
+class DeleteWebPreciseAccessRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DeleteWebCacheCustomRule')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DeleteWebPreciseAccessRule','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DeleteWebPreciseAccessRuleRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DeleteWebCacheCustomRuleRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class DeleteWebPreciseAccessRuleRequest(RpcRequest):
+class DeleteWebCacheCustomRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DeleteWebPreciseAccessRule')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DeleteWebCacheCustomRule','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DeleteWebRuleRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DeleteWebRuleRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DeleteWebRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DeleteWebRule')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DeleteWebRule','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeAsyncTasksRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeAsyncTasksRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeAsyncTasksRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeAsyncTasks')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeAsyncTasks','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeAttackAnalysisMaxQpsRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeAttackAnalysisMaxQpsRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeAttackAnalysisMaxQpsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeAttackAnalysisMaxQps')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeAttackAnalysisMaxQps','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeAutoCcBlacklistRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeAutoCcBlacklistRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeAutoCcBlacklistRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeAutoCcBlacklist')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeAutoCcBlacklist','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeAutoCcListCountRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeAutoCcListCountRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeAutoCcListCountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeAutoCcListCount')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeAutoCcListCount','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeAutoCcWhitelistRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeAutoCcWhitelistRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeAutoCcWhitelistRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeAutoCcWhitelist')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeAutoCcWhitelist','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeBackSourceCidrRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DisableWebCCRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,28 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class DescribeBackSourceCidrRequest(RpcRequest):
+class DisableWebCCRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeBackSourceCidr')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DisableWebCC','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_Line(self): # String
-		return self.get_query_params().get('Line')
-
-	def set_Line(self, Line):  # String
-		self.add_query_param('Line', Line)
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
+	def get_Domain(self): # String
+		return self.get_query_params().get('Domain')
+
+	def set_Domain(self, Domain):  # String
+		self.add_query_param('Domain', Domain)
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeBlackholeStatusRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeBlackholeStatusRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeBlackholeStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeBlackholeStatus')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeBlackholeStatus','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeBlockStatusRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeBlockStatusRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeBlockStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeBlockStatus')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeBlockStatus','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeCertsRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeCertsRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeCertsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeCerts')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeCerts','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeCnameReusesRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeWebCcProtectSwitchRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class DescribeCnameReusesRequest(RpcRequest):
+class DescribeWebCcProtectSwitchRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeCnameReuses')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeWebCcProtectSwitch','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDDoSEventsRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDDoSEventsRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeDDoSEventsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDDoSEvents')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDDoSEvents','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDDosAllEventListRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDDosAllEventListRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeDDosAllEventListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDDosAllEventList')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDDosAllEventList','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDDosEventAreaRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDDosEventAreaRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeDDosEventAreaRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDDosEventArea')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDDosEventArea','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDDosEventAttackTypeRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDDosEventAttackTypeRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeDDosEventAttackTypeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDDosEventAttackType')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDDosEventAttackType','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDDosEventIspRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDDosEventIspRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeDDosEventIspRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDDosEventIsp')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDDosEventIsp','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDDosEventMaxRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDDosEventMaxRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeDDosEventMaxRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDDosEventMax')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDDosEventMax','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDDosEventSrcIpRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDDosEventSrcIpRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeDDosEventSrcIpRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDDosEventSrcIp')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDDosEventSrcIp','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDefenseCountStatisticsRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeWebCustomPortsRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class DescribeDefenseCountStatisticsRequest(RpcRequest):
+class DescribeWebCustomPortsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDefenseCountStatistics')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeWebCustomPorts','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDefenseRecordsRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDefenseRecordsRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeDefenseRecordsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDefenseRecords')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDefenseRecords','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDomainAttackEventsRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDomainAttackEventsRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeDomainAttackEventsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDomainAttackEvents')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDomainAttackEvents','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDomainOverviewRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDomainOverviewRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeDomainOverviewRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDomainOverview')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDomainOverview','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDomainQPSListRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDomainQPSListRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeDomainQPSListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDomainQPSList')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDomainQPSList','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDomainQpsWithCacheRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDomainStatusCodeCountRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,38 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class DescribeDomainQpsWithCacheRequest(RpcRequest):
+class DescribeDomainStatusCodeCountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDomainQpsWithCache')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDomainStatusCodeCount','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_EndTime(self): # Long
-		return self.get_query_params().get('EndTime')
-
-	def set_EndTime(self, EndTime):  # Long
-		self.add_query_param('EndTime', EndTime)
 	def get_StartTime(self): # Long
 		return self.get_query_params().get('StartTime')
 
 	def set_StartTime(self, StartTime):  # Long
 		self.add_query_param('StartTime', StartTime)
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
+	def get_EndTime(self): # Long
+		return self.get_query_params().get('EndTime')
+
+	def set_EndTime(self, EndTime):  # Long
+		self.add_query_param('EndTime', EndTime)
 	def get_Domain(self): # String
 		return self.get_query_params().get('Domain')
 
 	def set_Domain(self, Domain):  # String
 		self.add_query_param('Domain', Domain)
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDomainResourceRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDomainResourceRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeDomainResourceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDomainResource')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDomainResource','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDomainStatusCodeCountRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDomainViewSourceCountriesRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,38 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class DescribeDomainStatusCodeCountRequest(RpcRequest):
+class DescribeDomainViewSourceCountriesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDomainStatusCodeCount')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDomainViewSourceCountries','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_EndTime(self): # Long
+		return self.get_query_params().get('EndTime')
+
+	def set_EndTime(self, EndTime):  # Long
+		self.add_query_param('EndTime', EndTime)
 	def get_StartTime(self): # Long
 		return self.get_query_params().get('StartTime')
 
 	def set_StartTime(self, StartTime):  # Long
 		self.add_query_param('StartTime', StartTime)
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
-	def get_EndTime(self): # Long
-		return self.get_query_params().get('EndTime')
-
-	def set_EndTime(self, EndTime):  # Long
-		self.add_query_param('EndTime', EndTime)
 	def get_Domain(self): # String
 		return self.get_query_params().get('Domain')
 
 	def set_Domain(self, Domain):  # String
 		self.add_query_param('Domain', Domain)
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDomainStatusCodeListRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDomainStatusCodeListRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeDomainStatusCodeListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDomainStatusCodeList')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDomainStatusCodeList','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDomainTopAttackListRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDomainTopAttackListRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeDomainTopAttackListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDomainTopAttackList')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDomainTopAttackList','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDomainViewSourceCountriesRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDomainViewSourceProvincesRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class DescribeDomainViewSourceCountriesRequest(RpcRequest):
+class DescribeDomainViewSourceProvincesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDomainViewSourceCountries')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDomainViewSourceProvinces','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDomainViewSourceProvincesRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyTlsConfigRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,38 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class DescribeDomainViewSourceProvincesRequest(RpcRequest):
+class ModifyTlsConfigRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDomainViewSourceProvinces')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyTlsConfig','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_EndTime(self): # Long
-		return self.get_query_params().get('EndTime')
-
-	def set_EndTime(self, EndTime):  # Long
-		self.add_query_param('EndTime', EndTime)
-	def get_StartTime(self): # Long
-		return self.get_query_params().get('StartTime')
-
-	def set_StartTime(self, StartTime):  # Long
-		self.add_query_param('StartTime', StartTime)
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
 	def get_Domain(self): # String
 		return self.get_query_params().get('Domain')
 
 	def set_Domain(self, Domain):  # String
 		self.add_query_param('Domain', Domain)
+	def get_Config(self): # String
+		return self.get_query_params().get('Config')
+
+	def set_Config(self, Config):  # String
+		self.add_query_param('Config', Config)
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDomainViewTopCostTimeRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDomainViewTopCostTimeRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeDomainViewTopCostTimeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDomainViewTopCostTime')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDomainViewTopCostTime','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDomainViewTopUrlRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDomainViewTopUrlRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeDomainViewTopUrlRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDomainViewTopUrl')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDomainViewTopUrl','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeDomainsRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDomainsRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeDomainsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDomains')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDomains','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeElasticBandwidthSpecRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeElasticBandwidthSpecRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeElasticBandwidthSpecRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeElasticBandwidthSpec')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeElasticBandwidthSpec','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeHealthCheckListRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeHealthCheckListRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeHealthCheckListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeHealthCheckList')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeHealthCheckList','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeHealthCheckStatusRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeHealthCheckStatusRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeHealthCheckStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeHealthCheckStatus')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeHealthCheckStatus','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeInstanceDetailsRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeInstanceStatisticsRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class DescribeInstanceDetailsRequest(RpcRequest):
+class DescribeInstanceStatisticsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeInstanceDetails')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeInstanceStatistics','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeInstanceIdsRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeInstanceIdsRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeInstanceIdsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeInstanceIds')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeInstanceIds','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeInstanceSpecsRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeInstanceSpecsRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeInstanceSpecsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeInstanceSpecs')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeInstanceSpecs','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeInstanceStatisticsRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribePortAutoCcStatusRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class DescribeInstanceStatisticsRequest(RpcRequest):
+class DescribePortAutoCcStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeInstanceStatistics')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribePortAutoCcStatus','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeInstanceStatusRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeInstanceStatusRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeInstanceStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeInstanceStatus')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeInstanceStatus','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeInstancesRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeInstancesRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeInstancesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeInstances')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeInstances','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeL7RsPolicyRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeL7RsPolicyRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeL7RsPolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeL7RsPolicy')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeL7RsPolicy','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeLayer4RulePolicyRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeLayer4RulePolicyRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeLayer4RulePolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeLayer4RulePolicy')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeLayer4RulePolicy','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeLogStoreExistStatusRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyFullLogTtlRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,23 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class DescribeLogStoreExistStatusRequest(RpcRequest):
+class ModifyFullLogTtlRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeLogStoreExistStatus')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyFullLogTtl','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_Ttl(self): # Integer
+		return self.get_query_params().get('Ttl')
+
+	def set_Ttl(self, Ttl):  # Integer
+		self.add_query_param('Ttl', Ttl)
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeNetworkRegionBlockRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeUdpReflectRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class DescribeNetworkRegionBlockRequest(RpcRequest):
+class DescribeUdpReflectRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeNetworkRegionBlock')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeUdpReflect','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeNetworkRuleAttributesRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeNetworkRuleAttributesRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeNetworkRuleAttributesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeNetworkRuleAttributes')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeNetworkRuleAttributes','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeNetworkRulesRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeNetworkRulesRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeNetworkRulesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeNetworkRules')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeNetworkRules','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeOpEntitiesRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeOpEntitiesRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeOpEntitiesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeOpEntities')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeOpEntities','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribePortAttackMaxFlowRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribePortViewSourceProvincesRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class DescribePortAttackMaxFlowRequest(RpcRequest):
+class DescribePortViewSourceProvincesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribePortAttackMaxFlow')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribePortViewSourceProvinces','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribePortAutoCcStatusRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeNetworkRegionBlockRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,24 +16,23 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class DescribePortAutoCcStatusRequest(RpcRequest):
+class DescribeNetworkRegionBlockRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribePortAutoCcStatus')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeNetworkRegionBlock','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_InstanceIdss(self): # RepeatList
-		return self.get_query_params().get('InstanceIds')
+	def get_InstanceId(self): # String
+		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceIdss(self, InstanceIds):  # RepeatList
-		for depth1 in range(len(InstanceIds)):
-			self.add_query_param('InstanceIds.' + str(depth1 + 1), InstanceIds[depth1])
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribePortConnsCountRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribePortConnsCountRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribePortConnsCountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribePortConnsCount')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribePortConnsCount','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribePortConnsListRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribePortConnsListRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribePortConnsListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribePortConnsList')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribePortConnsList','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribePortFlowListRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribePortFlowListRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribePortFlowListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribePortFlowList')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribePortFlowList','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribePortMaxConnsRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribePortViewSourceCountriesRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class DescribePortMaxConnsRequest(RpcRequest):
+class DescribePortViewSourceCountriesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribePortMaxConns')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribePortViewSourceCountries','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribePortRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribePortRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribePortRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribePort')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribePort','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribePortViewSourceCountriesRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeTotalAttackMaxFlowRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,39 +16,39 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class DescribePortViewSourceCountriesRequest(RpcRequest):
+class DescribeTotalAttackMaxFlowRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribePortViewSourceCountries')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeTotalAttackMaxFlow','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_EndTime(self): # Long
-		return self.get_query_params().get('EndTime')
-
-	def set_EndTime(self, EndTime):  # Long
-		self.add_query_param('EndTime', EndTime)
 	def get_StartTime(self): # Long
 		return self.get_query_params().get('StartTime')
 
 	def set_StartTime(self, StartTime):  # Long
 		self.add_query_param('StartTime', StartTime)
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
+	def get_EndTime(self): # Long
+		return self.get_query_params().get('EndTime')
+
+	def set_EndTime(self, EndTime):  # Long
+		self.add_query_param('EndTime', EndTime)
 	def get_InstanceIdss(self): # RepeatList
 		return self.get_query_params().get('InstanceIds')
 
 	def set_InstanceIdss(self, InstanceIds):  # RepeatList
 		for depth1 in range(len(InstanceIds)):
 			self.add_query_param('InstanceIds.' + str(depth1 + 1), InstanceIds[depth1])
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribePortViewSourceIspsRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribePortAttackMaxFlowRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class DescribePortViewSourceIspsRequest(RpcRequest):
+class DescribePortAttackMaxFlowRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribePortViewSourceIsps')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribePortAttackMaxFlow','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribePortViewSourceProvincesRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyWebPreciseAccessRuleRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,39 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class DescribePortViewSourceProvincesRequest(RpcRequest):
+class ModifyWebPreciseAccessRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribePortViewSourceProvinces')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyWebPreciseAccessRule','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_EndTime(self): # Long
-		return self.get_query_params().get('EndTime')
+	def get_Expires(self): # Integer
+		return self.get_query_params().get('Expires')
 
-	def set_EndTime(self, EndTime):  # Long
-		self.add_query_param('EndTime', EndTime)
-	def get_StartTime(self): # Long
-		return self.get_query_params().get('StartTime')
+	def set_Expires(self, Expires):  # Integer
+		self.add_query_param('Expires', Expires)
+	def get_Rules(self): # String
+		return self.get_query_params().get('Rules')
 
-	def set_StartTime(self, StartTime):  # Long
-		self.add_query_param('StartTime', StartTime)
+	def set_Rules(self, Rules):  # String
+		self.add_query_param('Rules', Rules)
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
-	def get_InstanceIdss(self): # RepeatList
-		return self.get_query_params().get('InstanceIds')
+	def get_Domain(self): # String
+		return self.get_query_params().get('Domain')
 
-	def set_InstanceIdss(self, InstanceIds):  # RepeatList
-		for depth1 in range(len(InstanceIds)):
-			self.add_query_param('InstanceIds.' + str(depth1 + 1), InstanceIds[depth1])
+	def set_Domain(self, Domain):  # String
+		self.add_query_param('Domain', Domain)
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeSceneDefenseObjectsRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeSceneDefenseObjectsRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeSceneDefenseObjectsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeSceneDefenseObjects')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeSceneDefenseObjects','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeSceneDefensePoliciesRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeSceneDefensePoliciesRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeSceneDefensePoliciesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeSceneDefensePolicies')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeSceneDefensePolicies','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeSchedulerRulesRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeSchedulerRulesRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeSchedulerRulesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeSchedulerRules')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeSchedulerRules','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeSlsAuthStatusRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/EmptySlsLogstoreRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class DescribeSlsAuthStatusRequest(RpcRequest):
+class EmptySlsLogstoreRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeSlsAuthStatus')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'EmptySlsLogstore','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeSlsLogstoreInfoRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeSlsLogstoreInfoRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeSlsLogstoreInfoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeSlsLogstoreInfo')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeSlsLogstoreInfo','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeSlsOpenStatusRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeSlsOpenStatusRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeSlsOpenStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeSlsOpenStatus')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeSlsOpenStatus','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeStsGrantStatusRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeStsGrantStatusRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeStsGrantStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeStsGrantStatus')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeStsGrantStatus','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeSystemLogRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeSystemLogRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeSystemLogRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeSystemLog')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeSystemLog','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeTagKeysRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeTagKeysRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeTagKeysRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeTagKeys')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeTagKeys','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeTagResourcesRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeTagResourcesRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeTagResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeTagResources')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeTagResources','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeUdpReflectRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/EmptyAutoCcBlacklistRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class DescribeUdpReflectRequest(RpcRequest):
+class EmptyAutoCcBlacklistRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeUdpReflect')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'EmptyAutoCcBlacklist','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeUnBlackholeCountRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeUnBlackholeCountRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeUnBlackholeCountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeUnBlackholeCount')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeUnBlackholeCount','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeUnBlockCountRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeUnBlockCountRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeUnBlockCountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeUnBlockCount')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeUnBlockCount','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeWebAccessLogDispatchStatusRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeWebAccessLogDispatchStatusRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeWebAccessLogDispatchStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeWebAccessLogDispatchStatus')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeWebAccessLogDispatchStatus','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeWebAccessLogEmptyCountRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeWebAccessLogEmptyCountRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeWebAccessLogEmptyCountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeWebAccessLogEmptyCount')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeWebAccessLogEmptyCount','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeWebAccessLogStatusRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeWebAccessLogStatusRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeWebAccessLogStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeWebAccessLogStatus')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeWebAccessLogStatus','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeWebAccessModeRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeWebAccessModeRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeWebAccessModeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeWebAccessMode')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeWebAccessMode','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeWebAreaBlockConfigsRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeWebAreaBlockConfigsRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeWebAreaBlockConfigsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeWebAreaBlockConfigs')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeWebAreaBlockConfigs','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeWebCCRulesRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeWebCCRulesRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeWebCCRulesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeWebCCRules')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeWebCCRules','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeWebCacheConfigsRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeWebCacheConfigsRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeWebCacheConfigsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeWebCacheConfigs')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeWebCacheConfigs','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeWebCcProtectSwitchRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeHeadersRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,29 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class DescribeWebCcProtectSwitchRequest(RpcRequest):
+class DescribeHeadersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeWebCcProtectSwitch')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeHeaders','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_Domainss(self): # RepeatList
-		return self.get_query_params().get('Domains')
-
-	def set_Domainss(self, Domains):  # RepeatList
-		for depth1 in range(len(Domains)):
-			self.add_query_param('Domains.' + str(depth1 + 1), Domains[depth1])
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
+	def get_Domain(self): # String
+		return self.get_query_params().get('Domain')
+
+	def set_Domain(self, Domain):  # String
+		self.add_query_param('Domain', Domain)
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeWebCustomPortsRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeLogStoreExistStatusRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class DescribeWebCustomPortsRequest(RpcRequest):
+class DescribeLogStoreExistStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeWebCustomPorts')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeLogStoreExistStatus','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeWebInstanceRelationsRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeWebPreciseAccessRuleRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class DescribeWebInstanceRelationsRequest(RpcRequest):
+class DescribeWebPreciseAccessRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeWebInstanceRelations')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeWebPreciseAccessRule','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeWebPreciseAccessRuleRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeDefenseCountStatisticsRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,29 +16,23 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class DescribeWebPreciseAccessRuleRequest(RpcRequest):
+class DescribeDefenseCountStatisticsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeWebPreciseAccessRule')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeDefenseCountStatistics','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_Domainss(self): # RepeatList
-		return self.get_query_params().get('Domains')
-
-	def set_Domainss(self, Domains):  # RepeatList
-		for depth1 in range(len(Domains)):
-			self.add_query_param('Domains.' + str(depth1 + 1), Domains[depth1])
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DescribeWebRulesRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeWebRulesRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DescribeWebRulesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeWebRules')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeWebRules','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DetachSceneDefenseObjectRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DetachSceneDefenseObjectRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DetachSceneDefenseObjectRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DetachSceneDefenseObject')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DetachSceneDefenseObject','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DisableSceneDefensePolicyRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DisableSceneDefensePolicyRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class DisableSceneDefensePolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DisableSceneDefensePolicy')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DisableSceneDefensePolicy','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DisableWebAccessLogConfigRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/EnableWebCCRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class DisableWebAccessLogConfigRequest(RpcRequest):
+class EnableWebCCRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DisableWebAccessLogConfig')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'EnableWebCC','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DisableWebCCRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyWebCacheSwitchRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,28 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class DisableWebCCRequest(RpcRequest):
+class ModifyWebCacheSwitchRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DisableWebCC')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyWebCacheSwitch','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
+	def get_Enable(self): # Integer
+		return self.get_query_params().get('Enable')
+
+	def set_Enable(self, Enable):  # Integer
+		self.add_query_param('Enable', Enable)
 	def get_Domain(self): # String
 		return self.get_query_params().get('Domain')
 
 	def set_Domain(self, Domain):  # String
 		self.add_query_param('Domain', Domain)
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/DisableWebCCRuleRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/EnableWebCCRuleRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class DisableWebCCRuleRequest(RpcRequest):
+class EnableWebCCRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DisableWebCCRule')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'EnableWebCCRule','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/EmptyAutoCcBlacklistRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ReleaseInstanceRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class EmptyAutoCcBlacklistRequest(RpcRequest):
+class ReleaseInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'EmptyAutoCcBlacklist')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ReleaseInstance','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/EmptyAutoCcWhitelistRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/EmptyAutoCcWhitelistRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class EmptyAutoCcWhitelistRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'EmptyAutoCcWhitelist')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'EmptyAutoCcWhitelist','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/EmptySlsLogstoreRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyWebIpSetSwitchRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,23 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class EmptySlsLogstoreRequest(RpcRequest):
+class ModifyWebIpSetSwitchRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'EmptySlsLogstore')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyWebIpSetSwitch','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
+	def get_Domain(self): # String
+		return self.get_query_params().get('Domain')
+
+	def set_Domain(self, Domain):  # String
+		self.add_query_param('Domain', Domain)
+	def get_Config(self): # String
+		return self.get_query_params().get('Config')
+
+	def set_Config(self, Config):  # String
+		self.add_query_param('Config', Config)
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/EnableSceneDefensePolicyRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DeleteSceneDefensePolicyRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class EnableSceneDefensePolicyRequest(RpcRequest):
+class DeleteSceneDefensePolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'EnableSceneDefensePolicy')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DeleteSceneDefensePolicy','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/EnableWebAccessLogConfigRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/EnableWebAccessLogConfigRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class EnableWebAccessLogConfigRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'EnableWebAccessLogConfig')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'EnableWebAccessLogConfig','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/EnableWebCCRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyWebCacheModeRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,25 +16,30 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class EnableWebCCRequest(RpcRequest):
+class ModifyWebCacheModeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'EnableWebCC')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyWebCacheMode','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_Mode(self): # String
+		return self.get_query_params().get('Mode')
+
+	def set_Mode(self, Mode):  # String
+		self.add_query_param('Mode', Mode)
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
 	def get_Domain(self): # String
 		return self.get_query_params().get('Domain')
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/EnableWebCCRuleRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeCnameReusesRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,28 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class EnableWebCCRuleRequest(RpcRequest):
+class DescribeCnameReusesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'EnableWebCCRule')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeCnameReuses','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_Domainss(self): # RepeatList
+		return self.get_query_params().get('Domains')
+
+	def set_Domainss(self, Domains):  # RepeatList
+		for depth1 in range(len(Domains)):
+			self.add_query_param('Domains.' + str(depth1 + 1), Domains[depth1])
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
-	def get_Domain(self): # String
-		return self.get_query_params().get('Domain')
-
-	def set_Domain(self, Domain):  # String
-		self.add_query_param('Domain', Domain)
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyBlackholeStatusRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyBlackholeStatusRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class ModifyBlackholeStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyBlackholeStatus')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyBlackholeStatus','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyBlockStatusRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyBlockStatusRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class ModifyBlockStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyBlockStatus')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyBlockStatus','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyCnameReuseRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyHttp2EnableRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,30 +16,25 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class ModifyCnameReuseRequest(RpcRequest):
+class ModifyHttp2EnableRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyCnameReuse')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyHttp2Enable','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_Cname(self): # String
-		return self.get_query_params().get('Cname')
-
-	def set_Cname(self, Cname):  # String
-		self.add_query_param('Cname', Cname)
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
 	def get_Enable(self): # Integer
 		return self.get_query_params().get('Enable')
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyDomainResourceRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/CreateDomainResourceRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class ModifyDomainResourceRequest(RpcRequest):
+class CreateDomainResourceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyDomainResource')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'CreateDomainResource','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -43,28 +43,28 @@
 		self.add_query_param('RsType', RsType)
 	def get_RealServerss(self): # RepeatList
 		return self.get_query_params().get('RealServers')
 
 	def set_RealServerss(self, RealServers):  # RepeatList
 		for depth1 in range(len(RealServers)):
 			self.add_query_param('RealServers.' + str(depth1 + 1), RealServers[depth1])
-	def get_ProxyTypess(self): # RepeatList
-		return self.get_query_params().get('ProxyTypes')
-
-	def set_ProxyTypess(self, ProxyTypes):  # RepeatList
-		for depth1 in range(len(ProxyTypes)):
-			if ProxyTypes[depth1].get('ProxyPorts') is not None:
-				for depth2 in range(len(ProxyTypes[depth1].get('ProxyPorts'))):
-					self.add_query_param('ProxyTypes.' + str(depth1 + 1) + '.ProxyPorts.' + str(depth2 + 1), ProxyTypes[depth1].get('ProxyPorts')[depth2])
-			if ProxyTypes[depth1].get('ProxyType') is not None:
-				self.add_query_param('ProxyTypes.' + str(depth1 + 1) + '.ProxyType', ProxyTypes[depth1].get('ProxyType'))
 	def get_InstanceIdss(self): # RepeatList
 		return self.get_query_params().get('InstanceIds')
 
 	def set_InstanceIdss(self, InstanceIds):  # RepeatList
 		for depth1 in range(len(InstanceIds)):
 			self.add_query_param('InstanceIds.' + str(depth1 + 1), InstanceIds[depth1])
+	def get_ProxyTypes(self): # Array
+		return self.get_query_params().get('ProxyTypes')
+
+	def set_ProxyTypes(self, ProxyTypes):  # Array
+		for index1, value1 in enumerate(ProxyTypes):
+			if value1.get('ProxyPorts') is not None:
+				for index2, value2 in enumerate(value1.get('ProxyPorts')):
+					self.add_query_param('ProxyTypes.' + str(index1 + 1) + '.ProxyPorts.' + str(index2 + 1), value2)
+			if value1.get('ProxyType') is not None:
+				self.add_query_param('ProxyTypes.' + str(index1 + 1) + '.ProxyType', value1.get('ProxyType'))
 	def get_Domain(self): # String
 		return self.get_query_params().get('Domain')
 
 	def set_Domain(self, Domain):  # String
 		self.add_query_param('Domain', Domain)
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyElasticBandWidthRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyElasticBandWidthRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class ModifyElasticBandWidthRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyElasticBandWidth')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyElasticBandWidth','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyFullLogTtlRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeWebInstanceRelationsRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,28 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class ModifyFullLogTtlRequest(RpcRequest):
+class DescribeWebInstanceRelationsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyFullLogTtl')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeWebInstanceRelations','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_Ttl(self): # Integer
-		return self.get_query_params().get('Ttl')
+	def get_Domainss(self): # RepeatList
+		return self.get_query_params().get('Domains')
 
-	def set_Ttl(self, Ttl):  # Integer
-		self.add_query_param('Ttl', Ttl)
+	def set_Domainss(self, Domains):  # RepeatList
+		for depth1 in range(len(Domains)):
+			self.add_query_param('Domains.' + str(depth1 + 1), Domains[depth1])
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyHealthCheckConfigRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyNetworkRuleAttributeRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,30 +16,25 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class ModifyHealthCheckConfigRequest(RpcRequest):
+class ModifyNetworkRuleAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyHealthCheckConfig')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyNetworkRuleAttribute','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_HealthCheck(self): # String
-		return self.get_query_params().get('HealthCheck')
-
-	def set_HealthCheck(self, HealthCheck):  # String
-		self.add_query_param('HealthCheck', HealthCheck)
 	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
 	def set_InstanceId(self, InstanceId):  # String
 		self.add_query_param('InstanceId', InstanceId)
 	def get_FrontendPort(self): # Integer
 		return self.get_query_params().get('FrontendPort')
@@ -47,7 +42,12 @@
 	def set_FrontendPort(self, FrontendPort):  # Integer
 		self.add_query_param('FrontendPort', FrontendPort)
 	def get_ForwardProtocol(self): # String
 		return self.get_query_params().get('ForwardProtocol')
 
 	def set_ForwardProtocol(self, ForwardProtocol):  # String
 		self.add_query_param('ForwardProtocol', ForwardProtocol)
+	def get_Config(self): # String
+		return self.get_query_params().get('Config')
+
+	def set_Config(self, Config):  # String
+		self.add_query_param('Config', Config)
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyHttp2EnableRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyWebAreaBlockSwitchRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,33 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class ModifyHttp2EnableRequest(RpcRequest):
+class ModifyWebAreaBlockSwitchRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyHttp2Enable')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyWebAreaBlockSwitch','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
-	def get_Enable(self): # Integer
-		return self.get_query_params().get('Enable')
-
-	def set_Enable(self, Enable):  # Integer
-		self.add_query_param('Enable', Enable)
 	def get_Domain(self): # String
 		return self.get_query_params().get('Domain')
 
 	def set_Domain(self, Domain):  # String
 		self.add_query_param('Domain', Domain)
+	def get_Config(self): # String
+		return self.get_query_params().get('Config')
+
+	def set_Config(self, Config):  # String
+		self.add_query_param('Config', Config)
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyInstanceRemarkRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyInstanceRemarkRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class ModifyInstanceRemarkRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyInstanceRemark')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyInstanceRemark','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyNetworkRuleAttributeRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ConfigLayer4RealLimitRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,38 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class ModifyNetworkRuleAttributeRequest(RpcRequest):
+class ConfigLayer4RealLimitRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyNetworkRuleAttribute')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ConfigLayer4RealLimit','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_LimitValue(self): # Long
+		return self.get_query_params().get('LimitValue')
+
+	def set_LimitValue(self, LimitValue):  # Long
+		self.add_query_param('LimitValue', LimitValue)
 	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
 	def set_InstanceId(self, InstanceId):  # String
 		self.add_query_param('InstanceId', InstanceId)
-	def get_FrontendPort(self): # Integer
-		return self.get_query_params().get('FrontendPort')
-
-	def set_FrontendPort(self, FrontendPort):  # Integer
-		self.add_query_param('FrontendPort', FrontendPort)
-	def get_ForwardProtocol(self): # String
-		return self.get_query_params().get('ForwardProtocol')
-
-	def set_ForwardProtocol(self, ForwardProtocol):  # String
-		self.add_query_param('ForwardProtocol', ForwardProtocol)
-	def get_Config(self): # String
-		return self.get_query_params().get('Config')
-
-	def set_Config(self, Config):  # String
-		self.add_query_param('Config', Config)
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyPortAutoCcStatusRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyPortAutoCcStatusRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class ModifyPortAutoCcStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyPortAutoCcStatus')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyPortAutoCcStatus','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyPortRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyPortRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class ModifyPortRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyPort')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyPort','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifySceneDefensePolicyRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifySceneDefensePolicyRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class ModifySceneDefensePolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifySceneDefensePolicy')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifySceneDefensePolicy','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifySchedulerRuleRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifySchedulerRuleRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class ModifySchedulerRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifySchedulerRule')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifySchedulerRule','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyTlsConfigRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyWebAIProtectSwitchRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class ModifyTlsConfigRequest(RpcRequest):
+class ModifyWebAIProtectSwitchRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyTlsConfig')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyWebAIProtectSwitch','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyWebAIProtectModeRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyWebAIProtectModeRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class ModifyWebAIProtectModeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyWebAIProtectMode')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyWebAIProtectMode','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyWebAIProtectSwitchRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyWebAreaBlockRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,33 +16,34 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class ModifyWebAIProtectSwitchRequest(RpcRequest):
+class ModifyWebAreaBlockRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyWebAIProtectSwitch')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyWebAreaBlock','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_Regionss(self): # RepeatList
+		return self.get_query_params().get('Regions')
+
+	def set_Regionss(self, Regions):  # RepeatList
+		for depth1 in range(len(Regions)):
+			self.add_query_param('Regions.' + str(depth1 + 1), Regions[depth1])
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
 	def get_Domain(self): # String
 		return self.get_query_params().get('Domain')
 
 	def set_Domain(self, Domain):  # String
 		self.add_query_param('Domain', Domain)
-	def get_Config(self): # String
-		return self.get_query_params().get('Config')
-
-	def set_Config(self, Config):  # String
-		self.add_query_param('Config', Config)
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyWebAccessModeRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyWebAccessModeRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class ModifyWebAccessModeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyWebAccessMode')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyWebAccessMode','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyWebAreaBlockRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DisableWebCCRuleRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,31 +16,25 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class ModifyWebAreaBlockRequest(RpcRequest):
+class DisableWebCCRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyWebAreaBlock')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DisableWebCCRule','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_Regionss(self): # RepeatList
-		return self.get_query_params().get('Regions')
-
-	def set_Regionss(self, Regions):  # RepeatList
-		for depth1 in range(len(Regions)):
-			self.add_query_param('Regions.' + str(depth1 + 1), Regions[depth1])
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
 	def get_Domain(self): # String
 		return self.get_query_params().get('Domain')
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyWebAreaBlockSwitchRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DisableWebAccessLogConfigRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class ModifyWebAreaBlockSwitchRequest(RpcRequest):
+class DisableWebAccessLogConfigRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyWebAreaBlockSwitch')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DisableWebAccessLogConfig','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -37,12 +37,7 @@
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
 	def get_Domain(self): # String
 		return self.get_query_params().get('Domain')
 
 	def set_Domain(self, Domain):  # String
 		self.add_query_param('Domain', Domain)
-	def get_Config(self): # String
-		return self.get_query_params().get('Config')
-
-	def set_Config(self, Config):  # String
-		self.add_query_param('Config', Config)
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyWebCCRuleRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyWebCCRuleRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class ModifyWebCCRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyWebCCRule')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyWebCCRule','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyWebCacheCustomRuleRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyWebCacheCustomRuleRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class ModifyWebCacheCustomRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyWebCacheCustomRule')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyWebCacheCustomRule','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyWebCacheModeRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyHeadersRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,30 +16,30 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class ModifyWebCacheModeRequest(RpcRequest):
+class ModifyHeadersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyWebCacheMode')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyHeaders','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_Mode(self): # String
-		return self.get_query_params().get('Mode')
+	def get_CustomHeaders(self): # String
+		return self.get_query_params().get('CustomHeaders')
 
-	def set_Mode(self, Mode):  # String
-		self.add_query_param('Mode', Mode)
+	def set_CustomHeaders(self, CustomHeaders):  # String
+		self.add_query_param('CustomHeaders', CustomHeaders)
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
 	def get_Domain(self): # String
 		return self.get_query_params().get('Domain')
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyWebCacheSwitchRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyOcspStatusRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,30 +16,25 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class ModifyWebCacheSwitchRequest(RpcRequest):
+class ModifyOcspStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyWebCacheSwitch')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyOcspStatus','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_ResourceGroupId(self): # String
-		return self.get_query_params().get('ResourceGroupId')
-
-	def set_ResourceGroupId(self, ResourceGroupId):  # String
-		self.add_query_param('ResourceGroupId', ResourceGroupId)
 	def get_Enable(self): # Integer
 		return self.get_query_params().get('Enable')
 
 	def set_Enable(self, Enable):  # Integer
 		self.add_query_param('Enable', Enable)
 	def get_Domain(self): # String
 		return self.get_query_params().get('Domain')
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyWebIpSetSwitchRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeBackSourceCidrRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,33 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class ModifyWebIpSetSwitchRequest(RpcRequest):
+class DescribeBackSourceCidrRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyWebIpSetSwitch')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeBackSourceCidr','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_Line(self): # String
+		return self.get_query_params().get('Line')
+
+	def set_Line(self, Line):  # String
+		self.add_query_param('Line', Line)
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
-	def get_Domain(self): # String
-		return self.get_query_params().get('Domain')
-
-	def set_Domain(self, Domain):  # String
-		self.add_query_param('Domain', Domain)
-	def get_Config(self): # String
-		return self.get_query_params().get('Config')
+	def get_IpVersion(self): # String
+		return self.get_query_params().get('IpVersion')
 
-	def set_Config(self, Config):  # String
-		self.add_query_param('Config', Config)
+	def set_IpVersion(self, IpVersion):  # String
+		self.add_query_param('IpVersion', IpVersion)
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyWebPreciseAccessRuleRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ModifyWebRuleRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,38 +16,55 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class ModifyWebPreciseAccessRuleRequest(RpcRequest):
+class ModifyWebRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyWebPreciseAccessRule')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyWebRule','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_Expires(self): # Integer
-		return self.get_query_params().get('Expires')
+	def get_HttpsExt(self): # String
+		return self.get_query_params().get('HttpsExt')
 
-	def set_Expires(self, Expires):  # Integer
-		self.add_query_param('Expires', Expires)
-	def get_Rules(self): # String
-		return self.get_query_params().get('Rules')
-
-	def set_Rules(self, Rules):  # String
-		self.add_query_param('Rules', Rules)
+	def set_HttpsExt(self, HttpsExt):  # String
+		self.add_query_param('HttpsExt', HttpsExt)
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
+	def get_RsType(self): # Integer
+		return self.get_query_params().get('RsType')
+
+	def set_RsType(self, RsType):  # Integer
+		self.add_query_param('RsType', RsType)
+	def get_RealServerss(self): # RepeatList
+		return self.get_query_params().get('RealServers')
+
+	def set_RealServerss(self, RealServers):  # RepeatList
+		for depth1 in range(len(RealServers)):
+			self.add_query_param('RealServers.' + str(depth1 + 1), RealServers[depth1])
+	def get_ProxyTypes(self): # String
+		return self.get_query_params().get('ProxyTypes')
+
+	def set_ProxyTypes(self, ProxyTypes):  # String
+		self.add_query_param('ProxyTypes', ProxyTypes)
+	def get_InstanceIdss(self): # RepeatList
+		return self.get_query_params().get('InstanceIds')
+
+	def set_InstanceIdss(self, InstanceIds):  # RepeatList
+		for depth1 in range(len(InstanceIds)):
+			self.add_query_param('InstanceIds.' + str(depth1 + 1), InstanceIds[depth1])
 	def get_Domain(self): # String
 		return self.get_query_params().get('Domain')
 
 	def set_Domain(self, Domain):  # String
 		self.add_query_param('Domain', Domain)
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyWebPreciseAccessSwitchRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribePortCcAttackTopIPRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,33 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class ModifyWebPreciseAccessSwitchRequest(RpcRequest):
+class DescribePortCcAttackTopIPRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyWebPreciseAccessSwitch')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribePortCcAttackTopIP','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_ResourceGroupId(self): # String
-		return self.get_query_params().get('ResourceGroupId')
+	def get_StartTimestamp(self): # Long
+		return self.get_query_params().get('StartTimestamp')
 
-	def set_ResourceGroupId(self, ResourceGroupId):  # String
-		self.add_query_param('ResourceGroupId', ResourceGroupId)
-	def get_Domain(self): # String
-		return self.get_query_params().get('Domain')
+	def set_StartTimestamp(self, StartTimestamp):  # Long
+		self.add_query_param('StartTimestamp', StartTimestamp)
+	def get_Limit(self): # Long
+		return self.get_query_params().get('Limit')
 
-	def set_Domain(self, Domain):  # String
-		self.add_query_param('Domain', Domain)
-	def get_Config(self): # String
-		return self.get_query_params().get('Config')
+	def set_Limit(self, Limit):  # Long
+		self.add_query_param('Limit', Limit)
+	def get_Ip(self): # String
+		return self.get_query_params().get('Ip')
 
-	def set_Config(self, Config):  # String
-		self.add_query_param('Config', Config)
+	def set_Ip(self, Ip):  # String
+		self.add_query_param('Ip', Ip)
+	def get_Port(self): # String
+		return self.get_query_params().get('Port')
+
+	def set_Port(self, Port):  # String
+		self.add_query_param('Port', Port)
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ModifyWebRuleRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/ConfigL7RsPolicyRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,55 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class ModifyWebRuleRequest(RpcRequest):
+class ConfigL7RsPolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ModifyWebRule')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ConfigL7RsPolicy','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_HttpsExt(self): # String
-		return self.get_query_params().get('HttpsExt')
+	def get_UpstreamRetry(self): # Integer
+		return self.get_query_params().get('UpstreamRetry')
 
-	def set_HttpsExt(self, HttpsExt):  # String
-		self.add_query_param('HttpsExt', HttpsExt)
+	def set_UpstreamRetry(self, UpstreamRetry):  # Integer
+		self.add_query_param('UpstreamRetry', UpstreamRetry)
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
-	def get_RsType(self): # Integer
-		return self.get_query_params().get('RsType')
-
-	def set_RsType(self, RsType):  # Integer
-		self.add_query_param('RsType', RsType)
-	def get_RealServerss(self): # RepeatList
-		return self.get_query_params().get('RealServers')
-
-	def set_RealServerss(self, RealServers):  # RepeatList
-		for depth1 in range(len(RealServers)):
-			self.add_query_param('RealServers.' + str(depth1 + 1), RealServers[depth1])
-	def get_ProxyTypes(self): # String
-		return self.get_query_params().get('ProxyTypes')
-
-	def set_ProxyTypes(self, ProxyTypes):  # String
-		self.add_query_param('ProxyTypes', ProxyTypes)
-	def get_InstanceIdss(self): # RepeatList
-		return self.get_query_params().get('InstanceIds')
-
-	def set_InstanceIdss(self, InstanceIds):  # RepeatList
-		for depth1 in range(len(InstanceIds)):
-			self.add_query_param('InstanceIds.' + str(depth1 + 1), InstanceIds[depth1])
 	def get_Domain(self): # String
 		return self.get_query_params().get('Domain')
 
 	def set_Domain(self, Domain):  # String
 		self.add_query_param('Domain', Domain)
+	def get_Policy(self): # String
+		return self.get_query_params().get('Policy')
+
+	def set_Policy(self, Policy):  # String
+		self.add_query_param('Policy', Policy)
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/ReleaseInstanceRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/DescribeInstanceDetailsRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,23 +16,24 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
-class ReleaseInstanceRequest(RpcRequest):
+class DescribeInstanceDetailsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'ReleaseInstance')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'DescribeInstanceDetails','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_InstanceId(self): # String
-		return self.get_query_params().get('InstanceId')
+	def get_InstanceIdss(self): # RepeatList
+		return self.get_query_params().get('InstanceIds')
 
-	def set_InstanceId(self, InstanceId):  # String
-		self.add_query_param('InstanceId', InstanceId)
+	def set_InstanceIdss(self, InstanceIds):  # RepeatList
+		for depth1 in range(len(InstanceIds)):
+			self.add_query_param('InstanceIds.' + str(depth1 + 1), InstanceIds[depth1])
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/aliyunsdkddoscoo/request/v20200101/SwitchSchedulerRuleRequest.py` & `aliyun-python-sdk-ddoscoo-1.0.6/aliyunsdkddoscoo/request/v20200101/SwitchSchedulerRuleRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkddoscoo.endpoint import endpoint_data
 
 class SwitchSchedulerRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'SwitchSchedulerRule')
+		RpcRequest.__init__(self, 'ddoscoo', '2020-01-01', 'SwitchSchedulerRule','ddoscoo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-ddoscoo-1.0.5/setup.py` & `aliyun-python-sdk-ddoscoo-1.0.6/setup.py`

 * *Files identical despite different names*

