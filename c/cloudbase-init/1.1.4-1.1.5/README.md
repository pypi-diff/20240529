# Comparing `tmp/cloudbase-init-1.1.4.tar.gz` & `tmp/cloudbase-init-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudbase-init-1.1.4.tar", last modified: Tue Feb 14 16:16:27 2023, max compression
+gzip compressed data, was "cloudbase-init-1.1.5.tar", last modified: Wed May 29 10:23:44 2024, max compression
```

## Comparing `cloudbase-init-1.1.4.tar` & `cloudbase-init-1.1.5.tar`

### file list

```diff
@@ -1,349 +1,353 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.678978 cloudbase-init-1.1.4/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/.gitattributes
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/.testr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4268 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1667 2023-02-14 16:16:27.000000 cloudbase-init-1.1.4/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21711 2023-02-14 16:16:27.000000 cloudbase-init-1.1.4/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1859 2023-02-14 16:16:27.678978 cloudbase-init-1.1.4/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.622968 cloudbase-init-1.1.4/cloudbase_init.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1859 2023-02-14 16:16:27.000000 cloudbase-init-1.1.4/cloudbase_init.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13866 2023-02-14 16:16:27.000000 cloudbase-init-1.1.4/cloudbase_init.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-14 16:16:27.000000 cloudbase-init-1.1.4/cloudbase_init.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-02-14 16:16:27.000000 cloudbase-init-1.1.4/cloudbase_init.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-14 16:16:27.000000 cloudbase-init-1.1.4/cloudbase_init.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-14 16:16:27.000000 cloudbase-init-1.1.4/cloudbase_init.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-02-14 16:16:27.000000 cloudbase-init-1.1.4/cloudbase_init.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       14 2023-02-14 16:16:27.000000 cloudbase-init-1.1.4/cloudbase_init.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.622968 cloudbase-init-1.1.4/cloudbaseinit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.626969 cloudbase-init-1.1.4/cloudbaseinit/conf/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/conf/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1594 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/conf/azure.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1270 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/conf/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2818 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/conf/cloudconfig.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2408 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/conf/cloudstack.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15944 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/conf/default.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2323 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/conf/ec2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1419 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/conf/factory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1985 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/conf/gce.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2935 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/conf/maas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2233 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/conf/openstack.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1274 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/conf/opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1830 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/conf/ovf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1959 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/conf/packet.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1741 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/conf/vmwareguestinfo.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1737 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/constant.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2309 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9739 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/init.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.626969 cloudbase-init-1.1.4/cloudbaseinit/metadata/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/metadata/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1360 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/metadata/factory.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.630970 cloudbase-init-1.1.4/cloudbaseinit/metadata/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/metadata/services/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18904 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/metadata/services/azureservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10863 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/metadata/services/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3510 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/metadata/services/baseconfigdrive.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10964 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/metadata/services/baseopenstackservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9743 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/metadata/services/cloudstack.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1179 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/metadata/services/configdrive.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2744 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/metadata/services/ec2service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6666 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/metadata/services/gceservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2782 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/metadata/services/httpservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11586 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/metadata/services/maasservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11949 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/metadata/services/nocloudservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9556 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/metadata/services/opennebulaservice.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.630970 cloudbase-init-1.1.4/cloudbaseinit/metadata/services/osconfigdrive/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/metadata/services/osconfigdrive/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1006 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/metadata/services/osconfigdrive/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1128 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/metadata/services/osconfigdrive/factory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9820 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/metadata/services/osconfigdrive/windows.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4925 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/metadata/services/ovfservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4995 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/metadata/services/packet.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5113 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/metadata/services/vmwareguestinfoservice.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.630970 cloudbase-init-1.1.4/cloudbaseinit/models/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/models/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2857 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/models/network.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.630970 cloudbase-init-1.1.4/cloudbaseinit/osutils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/osutils/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7346 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/osutils/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      938 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/osutils/factory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      755 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/osutils/posix.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    70936 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/osutils/windows.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.634970 cloudbase-init-1.1.4/cloudbaseinit/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.634970 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1065 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3710 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/createuser.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3838 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/ephemeraldisk.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7296 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/execcmd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1479 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/fileexecutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1698 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/localscripts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1967 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/mtu.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12101 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/networkconfig.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2941 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/ntpclient.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1338 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/sethostname.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5629 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/setuserpassword.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2077 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/sshpublickeys.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1284 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/trim.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8554 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdata.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.638971 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      907 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1041 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/cloudboothook.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4200 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/cloudconfig.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.638971 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      879 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2164 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/factory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2811 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2925 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/runcmd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1361 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/set_hostname.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1672 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/set_ntp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1429 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/set_timezone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6907 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/users.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5650 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/write_files.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      978 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/factory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1889 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/heat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      871 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/multipartmixed.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1619 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/parthandler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1589 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/shellscript.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3426 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdatautils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2981 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/factory.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.642972 cloudbase-init-1.1.4/cloudbaseinit/plugins/windows/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/windows/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11345 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/windows/azureguestagent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2401 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/windows/bootconfig.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2637 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/windows/certificates.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1620 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/windows/createuser.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1249 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/windows/displayidletimeout.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1360 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/windows/extendvolumes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3841 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/windows/licensing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2676 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/windows/ntpclient.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3087 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/windows/pagefiles.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1826 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/windows/rdp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1866 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/windows/sanpolicy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1423 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/windows/updates.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5109 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/windows/winrmcertificateauth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6292 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/plugins/windows/winrmlistener.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1109 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/shell.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.642972 cloudbase-init-1.1.4/cloudbaseinit/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      935 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/fake.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.642972 cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8181 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/fake_json_response.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.646972 cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.646972 cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/osconfigdrive/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/osconfigdrive/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1815 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/osconfigdrive/test_factory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22143 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/osconfigdrive/test_windows.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37321 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/test_azureservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9597 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5627 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/test_baseconfigdrive.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22155 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/test_baseopenstackservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14179 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/test_cloudstack.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2846 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/test_configdrive.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4015 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/test_ec2service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7157 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/test_gceservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4933 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/test_httpservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17075 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/test_maasservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9767 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/test_nocloudservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11625 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/test_opennebulaservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7265 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/test_ovfservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9111 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/test_packet.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7557 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/test_vmwareguestinfoservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2184 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/test_factory.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.650973 cloudbase-init-1.1.4/cloudbaseinit/tests/osutils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/osutils/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2396 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/osutils/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1461 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/osutils/test_factory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   123856 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/osutils/test_windows.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.650973 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.654974 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5872 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/test_createuser.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12052 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/test_ephemeraldisk.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5842 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/test_execcmd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2940 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/test_fileexecutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2870 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/test_localscripts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3479 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/test_mtu.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17977 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/test_networkconfig.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5743 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/test_ntpclient.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2311 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/test_sethostname.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14041 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/test_setuserpassword.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4050 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/test_sshpublickeys.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1786 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/test_trim.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19380 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/test_userdata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4096 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/test_userdatautils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.654974 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/userdataplugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/userdataplugins/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.654974 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3143 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/test_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3744 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/test_runcmd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1476 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/test_set_hostname.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1525 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/test_set_ntp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2215 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/test_set_timezone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4897 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/test_users.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11703 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/test_write_files.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1221 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/userdataplugins/test_cloudboothook.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3232 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/userdataplugins/test_cloudconfig.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1037 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/userdataplugins/test_factory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3242 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/userdataplugins/test_heat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2172 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/userdataplugins/test_parthandler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3275 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/userdataplugins/test_shellscript.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5160 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/test_factory.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.658974 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/windows/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/windows/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10464 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/windows/test_azureguestagent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5050 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/windows/test_bootconfig.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5225 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/windows/test_certificates.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3256 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/windows/test_createuser.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2085 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/windows/test_displayidletimeout.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2594 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/windows/test_extendvolumes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6387 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/windows/test_licensing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4647 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/windows/test_ntpclient.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7479 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/windows/test_pagefiles.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4115 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/windows/test_rdp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3642 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/windows/test_sanpolicy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2469 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/windows/test_updates.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6830 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/windows/test_winrmcertificateauth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13303 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/windows/test_winrmlistener.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.658974 cloudbase-init-1.1.4/cloudbaseinit/tests/resources/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/resources/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/resources/cloud_config_userdata
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2128 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/test_exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17857 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/test_init.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4608 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/test_version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7172 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/testutils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.662975 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.662975 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/template_engine/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/template_engine/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1145 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/template_engine/test_base_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2178 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/template_engine/test_factory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3299 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/template_engine/test_jinja2_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1528 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/test_classloader.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1737 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/test_crypt.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3146 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/test_debiface.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8224 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/test_dhcp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2265 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/test_encoding.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3444 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/test_hostname.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2464 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/test_log.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4696 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/test_network.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4267 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/test_retry_decorator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1523 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/test_serialization.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.666976 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.666976 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/storage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/storage/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2533 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/storage/test_factory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10038 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/storage/test_vds_storage_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6877 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/storage/test_wsm_storage_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7077 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_bootconfig.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12460 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_disk.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9607 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_licensing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11742 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_netlbfo.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12535 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_network.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2125 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_powercfg.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2442 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_privilege.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3202 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_rdp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3617 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_security.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11739 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_timezone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2304 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_updates.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1747 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_vds.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6341 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_vfat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16995 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_winrmconfig.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2505 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_wmi_loader.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1606 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_ws2_32.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    36779 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_x509.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.666976 cloudbase-init-1.1.4/cloudbaseinit/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1308 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/classloader.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1351 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/crypt.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4325 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/debiface.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4776 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/dhcp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1393 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/encoding.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2255 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/hostname.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3479 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/log.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3478 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/network.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1113 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/network_team.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3936 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/retry_decorator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1296 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/serialization.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.670976 cloudbase-init-1.1.4/cloudbaseinit/utils/template_engine/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/template_engine/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2364 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/template_engine/base_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1470 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/template_engine/factory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1785 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/template_engine/jinja2_template.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.674977 cloudbase-init-1.1.4/cloudbaseinit/utils/windows/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/windows/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3408 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/windows/bootconfig.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11648 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/windows/cryptoapi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12734 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/windows/disk.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5602 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/windows/iphlpapi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2707 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/windows/kernel32.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6165 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/windows/licensing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8113 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/windows/netlbfo.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6197 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/windows/network.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1164 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/windows/powercfg.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1331 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/windows/privilege.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5795 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/windows/productkeys.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1741 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/windows/rdp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1720 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/windows/security.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.674977 cloudbase-init-1.1.4/cloudbaseinit/utils/windows/storage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/windows/storage/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1043 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/windows/storage/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1461 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/windows/storage/factory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6387 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/windows/storage/vds_storage_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3923 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/windows/storage/wsm_storage_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6967 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/windows/timezone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1581 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/windows/updates.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11577 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/windows/vds.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2418 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/windows/vfat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7631 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/windows/winrmconfig.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1422 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/windows/wmi_loader.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1708 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/windows/ws2_32.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21277 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/windows/x509.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      700 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/utils/x509constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2274 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/cloudbaseinit/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.674977 cloudbase-init-1.1.4/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7450 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/doc/Makefile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7006 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/doc/make.bat
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      345 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.674977 cloudbase-init-1.1.4/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9472 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/doc/source/config.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1689 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/doc/source/intro.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17040 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/doc/source/plugins.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18062 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/doc/source/services.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4960 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/doc/source/tutorial.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10439 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/doc/source/userdata.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.618968 cloudbase-init-1.1.4/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.674977 cloudbase-init-1.1.4/etc/cloudbase-init/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/etc/cloudbase-init/README.md
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/etc/cloudbase-init/cloudbase-init-config-generator.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.618968 cloudbase-init-1.1.4/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.678978 cloudbase-init-1.1.4/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/releasenotes/notes/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.678978 cloudbase-init-1.1.4/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.678978 cloudbase-init-1.1.4/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:27.678978 cloudbase-init-1.1.4/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9332 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      301 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      928 2023-02-14 16:16:27.678978 cloudbase-init-1.1.4/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1419 2023-02-14 16:16:03.000000 cloudbase-init-1.1.4/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.675096 cloudbase-init-1.1.5/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/.gitattributes
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.627096 cloudbase-init-1.1.5/.github/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.631096 cloudbase-init-1.1.5/.github/workflows/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3176 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/.github/workflows/cloudbase_init_tests.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/.readthedocs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/.testr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4442 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1822 2024-05-29 10:23:44.000000 cloudbase-init-1.1.5/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22600 2024-05-29 10:23:44.000000 cloudbase-init-1.1.5/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1910 2024-05-29 10:23:44.675096 cloudbase-init-1.1.5/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.631096 cloudbase-init-1.1.5/cloudbase_init.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1910 2024-05-29 10:23:44.000000 cloudbase-init-1.1.5/cloudbase_init.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13927 2024-05-29 10:23:44.000000 cloudbase-init-1.1.5/cloudbase_init.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-29 10:23:44.000000 cloudbase-init-1.1.5/cloudbase_init.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-05-29 10:23:44.000000 cloudbase-init-1.1.5/cloudbase_init.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-29 10:23:44.000000 cloudbase-init-1.1.5/cloudbase_init.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-05-29 10:23:44.000000 cloudbase-init-1.1.5/cloudbase_init.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2024-05-29 10:23:44.000000 cloudbase-init-1.1.5/cloudbase_init.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       14 2024-05-29 10:23:44.000000 cloudbase-init-1.1.5/cloudbase_init.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.635096 cloudbase-init-1.1.5/cloudbaseinit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.635096 cloudbase-init-1.1.5/cloudbaseinit/conf/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/conf/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1594 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/conf/azure.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1270 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/conf/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2818 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/conf/cloudconfig.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2408 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/conf/cloudstack.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15944 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/conf/default.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2323 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/conf/ec2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1419 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/conf/factory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1985 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/conf/gce.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2935 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/conf/maas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2233 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/conf/openstack.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1274 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/conf/opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1830 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/conf/ovf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1959 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/conf/packet.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1741 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/conf/vmwareguestinfo.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1737 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/constant.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2309 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9746 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/init.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.635096 cloudbase-init-1.1.5/cloudbaseinit/metadata/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/metadata/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1360 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/metadata/factory.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.639096 cloudbase-init-1.1.5/cloudbaseinit/metadata/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/metadata/services/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18904 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/metadata/services/azureservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10863 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/metadata/services/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3510 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/metadata/services/baseconfigdrive.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10964 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/metadata/services/baseopenstackservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9743 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/metadata/services/cloudstack.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1179 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/metadata/services/configdrive.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2744 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/metadata/services/ec2service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6666 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/metadata/services/gceservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2782 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/metadata/services/httpservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11586 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/metadata/services/maasservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20918 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/metadata/services/nocloudservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9556 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/metadata/services/opennebulaservice.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.639096 cloudbase-init-1.1.5/cloudbaseinit/metadata/services/osconfigdrive/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/metadata/services/osconfigdrive/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1006 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/metadata/services/osconfigdrive/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1128 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/metadata/services/osconfigdrive/factory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9833 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/metadata/services/osconfigdrive/windows.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4925 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/metadata/services/ovfservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4995 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/metadata/services/packet.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8145 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/metadata/services/vmwareguestinfoservice.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.639096 cloudbase-init-1.1.5/cloudbaseinit/models/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/models/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2857 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/models/network.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.639096 cloudbase-init-1.1.5/cloudbaseinit/osutils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/osutils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7346 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/osutils/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      938 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/osutils/factory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      755 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/osutils/posix.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    71147 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/osutils/windows.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.639096 cloudbase-init-1.1.5/cloudbaseinit/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.643096 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1065 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3710 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/createuser.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3838 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/ephemeraldisk.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7296 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/execcmd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1479 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/fileexecutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1698 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/localscripts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1967 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/mtu.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12101 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/networkconfig.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2941 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/ntpclient.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1338 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/sethostname.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5629 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/setuserpassword.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2077 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/sshpublickeys.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1284 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/trim.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8554 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdata.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.643096 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      907 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1041 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/cloudboothook.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4200 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/cloudconfig.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.643096 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      879 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2164 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/factory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2811 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2925 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/runcmd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1361 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/set_hostname.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1672 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/set_ntp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1429 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/set_timezone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6907 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/users.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5650 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/write_files.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      978 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/factory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1889 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/heat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      871 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/multipartmixed.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1619 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/parthandler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1589 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/shellscript.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3426 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdatautils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2981 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/factory.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.647096 cloudbase-init-1.1.5/cloudbaseinit/plugins/windows/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/windows/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11345 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/windows/azureguestagent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2401 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/windows/bootconfig.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2637 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/windows/certificates.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1620 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/windows/createuser.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1249 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/windows/displayidletimeout.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1360 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/windows/extendvolumes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3841 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/windows/licensing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2676 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/windows/ntpclient.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3087 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/windows/pagefiles.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1826 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/windows/rdp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1866 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/windows/sanpolicy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1423 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/windows/updates.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5109 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/windows/winrmcertificateauth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6292 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/plugins/windows/winrmlistener.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1109 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/shell.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.647096 cloudbase-init-1.1.5/cloudbaseinit/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      954 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      935 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/fake.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.647096 cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8181 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/fake_json_response.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.651096 cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.651096 cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/osconfigdrive/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/osconfigdrive/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1815 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/osconfigdrive/test_factory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22179 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/osconfigdrive/test_windows.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    37321 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/test_azureservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9597 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5627 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/test_baseconfigdrive.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22155 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/test_baseopenstackservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14179 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/test_cloudstack.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2846 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/test_configdrive.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4015 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/test_ec2service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7157 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/test_gceservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4933 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/test_httpservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17075 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/test_maasservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16354 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/test_nocloudservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11625 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/test_opennebulaservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7265 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/test_ovfservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9111 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/test_packet.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11488 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/test_vmwareguestinfoservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2184 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/test_factory.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.651096 cloudbase-init-1.1.5/cloudbaseinit/tests/osutils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/osutils/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2396 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/osutils/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1461 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/osutils/test_factory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   123992 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/osutils/test_windows.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.651096 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.655096 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5872 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/test_createuser.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12052 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/test_ephemeraldisk.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5842 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/test_execcmd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2940 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/test_fileexecutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2870 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/test_localscripts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3479 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/test_mtu.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17977 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/test_networkconfig.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5743 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/test_ntpclient.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2311 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/test_sethostname.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14041 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/test_setuserpassword.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4050 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/test_sshpublickeys.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1786 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/test_trim.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19380 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/test_userdata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4096 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/test_userdatautils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.655096 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/userdataplugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/userdataplugins/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.659096 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3143 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/test_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3744 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/test_runcmd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1476 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/test_set_hostname.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1525 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/test_set_ntp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2215 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/test_set_timezone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4897 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/test_users.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11703 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/test_write_files.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1221 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/userdataplugins/test_cloudboothook.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3232 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/userdataplugins/test_cloudconfig.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1037 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/userdataplugins/test_factory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3242 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/userdataplugins/test_heat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2172 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/userdataplugins/test_parthandler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3275 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/userdataplugins/test_shellscript.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5160 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/test_factory.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.659096 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/windows/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/windows/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10464 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/windows/test_azureguestagent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5050 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/windows/test_bootconfig.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5225 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/windows/test_certificates.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3256 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/windows/test_createuser.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2085 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/windows/test_displayidletimeout.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2594 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/windows/test_extendvolumes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6387 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/windows/test_licensing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4647 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/windows/test_ntpclient.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7479 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/windows/test_pagefiles.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4115 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/windows/test_rdp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3642 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/windows/test_sanpolicy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2469 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/windows/test_updates.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6830 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/windows/test_winrmcertificateauth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13303 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/windows/test_winrmlistener.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.659096 cloudbase-init-1.1.5/cloudbaseinit/tests/resources/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/resources/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/resources/cloud_config_userdata
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2128 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/test_exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18026 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/test_init.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4608 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/test_version.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7172 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/testutils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.663096 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.663096 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/template_engine/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/template_engine/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1145 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/template_engine/test_base_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2178 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/template_engine/test_factory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3299 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/template_engine/test_jinja2_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1528 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/test_classloader.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1737 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/test_crypt.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3146 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/test_debiface.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8224 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/test_dhcp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2265 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/test_encoding.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3444 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/test_hostname.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2464 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/test_log.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4696 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/test_network.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4267 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/test_retry_decorator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1523 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/test_serialization.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.667096 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.667096 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/storage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/storage/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2533 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/storage/test_factory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10038 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/storage/test_vds_storage_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6877 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/storage/test_wsm_storage_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7077 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_bootconfig.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12460 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_disk.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9607 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_licensing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11742 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_netlbfo.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12535 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_network.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2125 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_powercfg.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2442 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_privilege.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3202 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_rdp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3617 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_security.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11739 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_timezone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2304 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_updates.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1747 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_vds.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7126 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_vfat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16995 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_winrmconfig.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2505 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_wmi_loader.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1606 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_ws2_32.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    36779 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_x509.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.667096 cloudbase-init-1.1.5/cloudbaseinit/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1308 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/classloader.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1351 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/crypt.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4325 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/debiface.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4776 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/dhcp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1393 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/encoding.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2255 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/hostname.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3479 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/log.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3478 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/network.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1113 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/network_team.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3936 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/retry_decorator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1296 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/serialization.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.667096 cloudbase-init-1.1.5/cloudbaseinit/utils/template_engine/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/template_engine/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2364 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/template_engine/base_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1470 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/template_engine/factory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1785 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/template_engine/jinja2_template.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.671096 cloudbase-init-1.1.5/cloudbaseinit/utils/windows/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/windows/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3408 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/windows/bootconfig.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11797 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/windows/cryptoapi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12734 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/windows/disk.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5602 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/windows/iphlpapi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2707 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/windows/kernel32.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6165 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/windows/licensing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8113 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/windows/netlbfo.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6197 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/windows/network.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1164 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/windows/powercfg.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1331 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/windows/privilege.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5795 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/windows/productkeys.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1741 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/windows/rdp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1720 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/windows/security.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.671096 cloudbase-init-1.1.5/cloudbaseinit/utils/windows/storage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/windows/storage/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1043 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/windows/storage/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1461 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/windows/storage/factory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6387 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/windows/storage/vds_storage_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3923 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/windows/storage/wsm_storage_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6967 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/windows/timezone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1581 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/windows/updates.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11577 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/windows/vds.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2439 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/windows/vfat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7631 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/windows/winrmconfig.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1422 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/windows/wmi_loader.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1708 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/windows/ws2_32.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21279 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/windows/x509.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      700 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/utils/x509constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2274 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/cloudbaseinit/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.671096 cloudbase-init-1.1.5/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7450 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/doc/Makefile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7006 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/doc/make.bat
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      345 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.675096 cloudbase-init-1.1.5/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9472 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/doc/source/config.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1689 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/doc/source/intro.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17040 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/doc/source/plugins.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18424 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/doc/source/services.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4960 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/doc/source/tutorial.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10439 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/doc/source/userdata.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.627096 cloudbase-init-1.1.5/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.675096 cloudbase-init-1.1.5/etc/cloudbase-init/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/etc/cloudbase-init/README.md
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/etc/cloudbase-init/cloudbase-init-config-generator.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.627096 cloudbase-init-1.1.5/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.675096 cloudbase-init-1.1.5/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/releasenotes/notes/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.675096 cloudbase-init-1.1.5/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.675096 cloudbase-init-1.1.5/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:44.675096 cloudbase-init-1.1.5/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9332 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      968 2024-05-29 10:23:44.675096 cloudbase-init-1.1.5/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1477 2024-05-29 10:23:00.000000 cloudbase-init-1.1.5/tox.ini
```

### Comparing `cloudbase-init-1.1.4/.zuul.yaml` & `cloudbase-init-1.1.5/.zuul.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 - project:
     templates:
       - openstack-cover-jobs
       - build-openstack-docs-pti
-      - openstack-python3-zed-jobs
+      - openstack-python3-jobs
       - build-release-notes-jobs-python3
     post:
       jobs:
         - cbsl-init-upload-git-mirror
 
 - job:
     name: cbsl-init-upload-git-mirror
     parent: upload-git-mirror
     description: Mirrors x/cloudbase-init to cloudbase/cloudbase-init
     vars:
       git_mirror_repository: cloudbase/cloudbase-init
     secrets:
       - name: git_mirror_credentials
-        secret: cbsl-init-github-secret
+        secret: cbsl-init-github-secret-v2
         pass-to-parent: true
 
 - secret:
-    name: cbsl-init-github-secret
+    name: cbsl-init-github-secret-v2
     data:
       user: git
       host: github.com
-      host_key: github.com ssh-rsa AAAAB3NzaC1yc2EAAAABIwAAAQEAq2A7hRGmdnm9tUDbO9IDSwBK6TbQa+PXYPCPy6rbTrTtw7PHkccKrpp0yVhp5HdEIcKr6pLlVDBfOLX9QUsyCOV0wzfjIJNlGEYsdlLJizHhbn2mUjvSAHQqZETYP81eFzLQNnPHt4EVVUh7VfDESU84KezmD5QlWpXLmvU31/yMf+Se8xhHTvKSCZIFImWwoG6mbUoWf9nzpIoaSjB+weqqUUmpaaasXVal72J+UX2B+2RPW3RcT0eOzQgqlJL3RKrTJvdsjE3JEAvGq3lGHSZXy28G3skua2SmVi/w4yCE6gbODqnTWlg7+wC604ydGXA8VJiS5ap43JXiUFFAaQ==
+      host_key: github.com ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQCj7ndNxQowgcQnjshcLrqPEiiphnt+VTTvDP6mHBL9j1aNUkY4Ue1gvwnGLVlOhGeYrnZaMgRK6+PKCUXaDbC7qtbW8gIkhL7aGCsOr/C56SJMy/BCZfxd1nWzAOxSDPgVsmerOBYfNqltV9/hWCqBywINIR+5dIg6JTJ72pcEpEjcYgXkE2YEFXV1JHnsKgbLWNlhScqb2UmyRkQyytRLtL+38TGxkxCflmO+5Z8CSSNY7GidjMIZ7Q4zMjA2n1nGrlTDkzwDCsw+wqFPGQA179cnfGWOWRVruj16z6XyvxvjJwbz0wQZ75XK5tKSb7FNyeIEs4TT4jk+S4dhPeAUC5y+bDYirYgM4GC7uEnztnZyaVWQ7B381AK4Qdrwt51ZqExKbQpTUNn+EjqoTwvqNj4kqx5QUCI0ThS/YkOxJCXmPUWZbhjpCg56i+2aB6CmK2JGhn57K5mj0MNdBXA4/WnwH6XoPWJzK5Nyu2zB3nAZp+S5hpQs+p1vN1/wsjk=
       ssh_key: !encrypted/pkcs1-oaep
         - URxcngnyX5brhRdwST+52sruiMTD5TW5ZLYU/Kr3uDlhbCAiZl+1lRvRStHkRw4nEwBat
           lpWrdJzrcfS7iqmdAZ/XkTXRnzY3nmH6+fASJ0XN1gcTuVKCveYg+4dmtd1BBUmGqwi+S
           9AMBXuUBayK6Wnyr160NC8isX2k7DLYnszX1QtPM+/gYTr+jM4cJOK7HUxIJQpqj7jwjF
           yY3nr1Nn881rvpbgqx9t0JOMW9eCxZBFQ86bZ75GWRan7jQmxc9M9tiDcHYKP7/Dy9i8+
           2V0LjPvQla4UYM3nu+9F3CIXvrsWrd3zAPWX0c93rAcq07vBAGhAU6rqW2X93n9ZV6wqA
           QDqIdLO6OWRaSq2fEb+/4ZTMSGRzFmarWTpYoQElkKWVCbiKJuKPxQPZfcqY0acEIvbZU
```

### Comparing `cloudbase-init-1.1.4/AUTHORS` & `cloudbase-init-1.1.5/AUTHORS`

 * *Files 12% similar despite different names*

```diff
@@ -16,26 +16,30 @@
 Ionut Hulub <ihulub@cloudbasesolutions.com>
 James Penick <penick@yahoo-inc.com>
 Jeremy Stanley <fungi@yuggoth.org>
 Jose Dillet <jdillet@vmware.com>
 Kevin_Zheng <zhengzhenyu@huawei.com>
 Kris Lindgren <klindgren@godaddy.com>
 Lucian Petrut <lpetrut@cloudbasesolutions.com>
+Lukas Kranz <lukas.kranz@bearingpoint.com>
+Luqman Aden <me@luqman.ca>
 Madalin <mbivolan@cloudbasesolutions.com>
 Mathieu Gagné <mgagne@iweb.com>
 Noboru Iwamatsu <n_iwamatsu@jp.fujitsu.com>
 Ondřej Nový <ondrej.novy@firma.seznam.cz>
 Paul Stone <s7oneyuk@gmail.com>
 Paula Madalina Crismaru <pcrismaru@cloudbasesolutions.com>
 Peng Yong <ppyy@pubyun.com>
 Robert Tingirica <rtingirica@cloudbasesolutions.com>
 Rui Lopes <rgl@ruilopes.com>
 Sean McGinnis <sean.mcginnis@gmail.com>
 Stefan Caraiman <scaraiman@cloudbasesolutions.com>
+Takashi Kajinami <kajinamit@oss.nttdata.com>
 Tingirica Robert <rtingirica@cloudbasesolutions.com>
 Vieri <15050873171@163.com>
+Zhongcheng Lao <zhongchengl@vmware.com>
 alexpilotti <ap@pilotti.it>
 avladu <avladu@cloudbasesolutions.com>
 liyubo <MrCocoaCat@aliyun.com>
 sunjiazz <sunjia@inspur.com>
 trobert2 <rtingirica@cloudbasesolutions.com>
 yoerg <xrepiv+ubuntuone@gmail.com>
```

### Comparing `cloudbase-init-1.1.4/ChangeLog` & `cloudbase-init-1.1.5/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,33 @@
 CHANGES
 =======
 
+1.1.5
+-----
+
+* Add official support for Python 3.11
+* github\_actions: show tox logs
+* Add network config support to VMware guest info service
+* Use MSFT\_NetAdapter to rename adapter
+* docs: update network config v1 document url
+* Support alternate 'public-keys' format for NoCloud service
+* readthedocs: add configuration file
+* Replace the old UPPER\_CONSTRAINTS\_FILE env
+* winrmlistener: use sha2 instead of insecure sha1
+* requirements: add missing pytz package
+* github\_actions: add windows and functional testing
+* python 3.11: run tests on github and opendev
+* replace unittest.mock.\_get\_target with mock one
+* use instance\_id as string for plugin sections
+* github\_mirror: update ssh secret name
+* github\_mirror: update ssh-rsa public key
+* github\_actions: run python tox on commit / pull
+* Accept drives with vFAT label 'cidata' as a configdrive
+* Bump version to 1.1.5
+
 1.1.4
 -----
 
 * bsdtar: check if tool path exists
 * tox: fix py3 / docs gates
 * crypto: replaced openssl with cryptography module
 * cloudconfig: fix type in key name no\_create\_home
```

### Comparing `cloudbase-init-1.1.4/LICENSE` & `cloudbase-init-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/PKG-INFO` & `cloudbase-init-1.1.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cloudbase-init
-Version: 1.1.4
+Version: 1.1.5
 Summary: Portable cloud initialization service
 Home-page: http://www.cloudbase.it/
 Author: Cloudbase Solutions Srl
 Author-email: apilotti@cloudbasesolutions.com
 License: UNKNOWN
 Description: Portable Multi-Cloud Initialization Service
         ===========================================
@@ -47,7 +47,8 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
```

### Comparing `cloudbase-init-1.1.4/README.rst` & `cloudbase-init-1.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbase_init.egg-info/PKG-INFO` & `cloudbase-init-1.1.5/cloudbase_init.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cloudbase-init
-Version: 1.1.4
+Version: 1.1.5
 Summary: Portable cloud initialization service
 Home-page: http://www.cloudbase.it/
 Author: Cloudbase Solutions Srl
 Author-email: apilotti@cloudbasesolutions.com
 License: UNKNOWN
 Description: Portable Multi-Cloud Initialization Service
         ===========================================
@@ -47,7 +47,8 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
```

### Comparing `cloudbase-init-1.1.4/cloudbase_init.egg-info/SOURCES.txt` & `cloudbase-init-1.1.5/cloudbase_init.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 .coveragerc
 .gitattributes
+.readthedocs.yaml
 .stestr.conf
 .testr.conf
 .zuul.yaml
 AUTHORS
 ChangeLog
 LICENSE
 README.rst
 requirements.txt
 setup.cfg
 setup.py
 test-requirements.txt
 tox.ini
+.github/workflows/cloudbase_init_tests.yml
 cloudbase_init.egg-info/PKG-INFO
 cloudbase_init.egg-info/SOURCES.txt
 cloudbase_init.egg-info/dependency_links.txt
 cloudbase_init.egg-info/entry_points.txt
 cloudbase_init.egg-info/not-zip-safe
 cloudbase_init.egg-info/pbr.json
 cloudbase_init.egg-info/requires.txt
```

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/conf/__init__.py` & `cloudbase-init-1.1.5/cloudbaseinit/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/conf/azure.py` & `cloudbase-init-1.1.5/cloudbaseinit/conf/azure.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/conf/base.py` & `cloudbase-init-1.1.5/cloudbaseinit/conf/base.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/conf/cloudconfig.py` & `cloudbase-init-1.1.5/cloudbaseinit/conf/cloudconfig.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/conf/cloudstack.py` & `cloudbase-init-1.1.5/cloudbaseinit/conf/cloudstack.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/conf/default.py` & `cloudbase-init-1.1.5/cloudbaseinit/conf/default.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/conf/ec2.py` & `cloudbase-init-1.1.5/cloudbaseinit/conf/ec2.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/conf/factory.py` & `cloudbase-init-1.1.5/cloudbaseinit/conf/factory.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/conf/gce.py` & `cloudbase-init-1.1.5/cloudbaseinit/conf/gce.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/conf/maas.py` & `cloudbase-init-1.1.5/cloudbaseinit/conf/maas.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/conf/openstack.py` & `cloudbase-init-1.1.5/cloudbaseinit/conf/openstack.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/conf/opts.py` & `cloudbase-init-1.1.5/cloudbaseinit/conf/opts.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/conf/ovf.py` & `cloudbase-init-1.1.5/cloudbaseinit/conf/ovf.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/conf/packet.py` & `cloudbase-init-1.1.5/cloudbaseinit/conf/packet.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/conf/vmwareguestinfo.py` & `cloudbase-init-1.1.5/cloudbaseinit/conf/vmwareguestinfo.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/constant.py` & `cloudbase-init-1.1.5/cloudbaseinit/constant.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/exception.py` & `cloudbase-init-1.1.5/cloudbaseinit/exception.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/init.py` & `cloudbase-init-1.1.5/cloudbaseinit/init.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 class InitManager(object):
     _PLUGINS_CONFIG_SECTION = 'Plugins'
 
     def _get_plugins_section(self, instance_id):
         if not instance_id:
             return self._PLUGINS_CONFIG_SECTION
         else:
-            return instance_id + "/" + self._PLUGINS_CONFIG_SECTION
+            return ("%s/%s" % (instance_id, self._PLUGINS_CONFIG_SECTION))
 
     def _get_plugin_status(self, osutils, instance_id, plugin_name):
         return osutils.get_config_value(plugin_name,
                                         self._get_plugins_section(instance_id))
 
     def _set_plugin_status(self, osutils, instance_id, plugin_name, status):
         osutils.set_config_value(plugin_name, status,
```

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/metadata/factory.py` & `cloudbase-init-1.1.5/cloudbaseinit/metadata/factory.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/metadata/services/azureservice.py` & `cloudbase-init-1.1.5/cloudbaseinit/metadata/services/azureservice.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/metadata/services/base.py` & `cloudbase-init-1.1.5/cloudbaseinit/metadata/services/base.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/metadata/services/baseconfigdrive.py` & `cloudbase-init-1.1.5/cloudbaseinit/metadata/services/baseconfigdrive.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/metadata/services/baseopenstackservice.py` & `cloudbase-init-1.1.5/cloudbaseinit/metadata/services/baseopenstackservice.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/metadata/services/cloudstack.py` & `cloudbase-init-1.1.5/cloudbaseinit/metadata/services/cloudstack.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/metadata/services/configdrive.py` & `cloudbase-init-1.1.5/cloudbaseinit/metadata/services/configdrive.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/metadata/services/ec2service.py` & `cloudbase-init-1.1.5/cloudbaseinit/metadata/services/ec2service.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/metadata/services/gceservice.py` & `cloudbase-init-1.1.5/cloudbaseinit/metadata/services/gceservice.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/metadata/services/httpservice.py` & `cloudbase-init-1.1.5/cloudbaseinit/metadata/services/httpservice.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/metadata/services/maasservice.py` & `cloudbase-init-1.1.5/cloudbaseinit/metadata/services/maasservice.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/metadata/services/opennebulaservice.py` & `cloudbase-init-1.1.5/cloudbaseinit/metadata/services/opennebulaservice.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/metadata/services/osconfigdrive/base.py` & `cloudbase-init-1.1.5/cloudbaseinit/metadata/services/osconfigdrive/base.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/metadata/services/osconfigdrive/factory.py` & `cloudbase-init-1.1.5/cloudbaseinit/metadata/services/osconfigdrive/factory.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/metadata/services/osconfigdrive/windows.py` & `cloudbase-init-1.1.5/cloudbaseinit/metadata/services/osconfigdrive/windows.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,15 @@
 
     def _get_config_drive_from_raw_hdd(self, drive_label, metadata_file):
         disks = map(disk.Disk, self._osutils.get_physical_disks())
         return self._extract_iso_from_devices(disks)
 
     def _get_config_drive_from_vfat(self, drive_label, metadata_file):
         for drive_path in self._osutils.get_physical_disks():
-            if vfat.is_vfat_drive(self._osutils, drive_path):
+            if vfat.is_vfat_drive(self._osutils, drive_path, drive_label):
                 LOG.info('Config Drive found on disk %r', drive_path)
                 vfat.copy_from_vfat_drive(self._osutils, drive_path,
                                           self.target_path)
                 return True
         return False
 
     def _get_config_drive_from_partition(self, drive_label, metadata_file):
```

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/metadata/services/ovfservice.py` & `cloudbase-init-1.1.5/cloudbaseinit/metadata/services/ovfservice.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/metadata/services/packet.py` & `cloudbase-init-1.1.5/cloudbaseinit/metadata/services/packet.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/metadata/services/vmwareguestinfoservice.py` & `cloudbase-init-1.1.5/cloudbaseinit/metadata/services/vmwareguestinfoservice.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,23 +10,26 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import base64
+import collections
+import copy
 import gzip
 import io
 import os
 
 from oslo_log import log as oslo_logging
 
 from cloudbaseinit import conf as cloudbaseinit_conf
 from cloudbaseinit import exception
 from cloudbaseinit.metadata.services import base
+from cloudbaseinit.metadata.services import nocloudservice
 from cloudbaseinit.osutils import factory as osutils_factory
 from cloudbaseinit.utils import serialization
 
 CONF = cloudbaseinit_conf.CONF
 LOG = oslo_logging.getLogger(__name__)
 
 
@@ -110,24 +113,24 @@
 
         if not os.path.exists(self._rpc_tool_path):
             LOG.info("%s does not exist. "
                      "Please provide a valid value for VMware rpctool path."
                      % self._rpc_tool_path)
             return False
 
-        self._meta_data = serialization.parse_json_yaml(
-            self._get_guest_data('metadata'))
+        metadata = self._get_guest_data('metadata')
+        self._meta_data = serialization.parse_json_yaml(metadata) \
+            if metadata else {}
         if not isinstance(self._meta_data, dict):
             LOG.warning("Instance metadata is not a dictionary.")
             self._meta_data = {}
 
         self._user_data = self._get_guest_data('userdata')
 
-        if self._meta_data or self._user_data:
-            return True
+        return True if self._meta_data or self._user_data else None
 
     def _get_data(self, path):
         pass
 
     def get_instance_id(self):
         return self._meta_data.get('instance-id')
 
@@ -147,7 +150,92 @@
         return list(set((key.strip() for key in public_keys)))
 
     def get_admin_username(self):
         return self._meta_data.get('admin-username')
 
     def get_admin_password(self):
         return self._meta_data.get('admin-password')
+
+    def get_network_details_v2(self):
+        """Return a `NetworkDetailsV2` object."""
+        network = self._process_network_config(self._meta_data)
+        if not network:
+            LOG.info("V2 network metadata not found")
+            return
+
+        return nocloudservice.NoCloudNetworkConfigParser.parse(network)
+
+    def _decode(self, key, enc_type, data):
+        """Returns the decoded string value of data
+
+        _decode returns the decoded string value of data
+        key is a string used to identify the data being decoded in log messages
+        """
+        LOG.debug("Getting encoded data for key=%s, enc=%s", key, enc_type)
+
+        if enc_type in ["gzip+base64", "gz+b64"]:
+            LOG.debug("Decoding %s format %s", enc_type, key)
+            raw_data = self._decode_data(data, True, True)
+        elif enc_type in ["base64", "b64"]:
+            LOG.debug("Decoding %s format %s", enc_type, key)
+            raw_data = self._b64d(data)
+        else:
+            LOG.debug("Plain-text data %s", key)
+            raw_data = data
+
+        if isinstance(raw_data, str):
+            return raw_data
+
+        return raw_data.decode('utf-8')
+
+    @staticmethod
+    def _load_json_or_yaml(data):
+        """Load a JSON or YAML string into a dictionary
+
+        load first attempts to unmarshal the provided data as JSON, and if
+        that fails then attempts to unmarshal the data as YAML. If data is
+        None then a new dictionary is returned.
+        """
+        if not data:
+            return {}
+        # If data is already a dictionary, here will return it directly.
+        if isinstance(data, dict):
+            return data
+
+        return serialization.parse_json_yaml(data)
+
+    @staticmethod
+    def _b64d(source):
+        # Base64 decode some data, accepting bytes or unicode/str, and
+        # returning str/unicode if the result is utf-8 compatible,
+        # otherwise returning bytes.
+        decoded = base64.b64decode(source)
+        try:
+            return decoded.decode("utf-8")
+        except UnicodeDecodeError:
+            return decoded
+
+    def _process_network_config(self, data):
+        """Loads and parse the optional network configuration."""
+        if not data:
+            return {}
+
+        network = None
+        if "network" in data:
+            network = data["network"]
+
+        network_enc = None
+        if "network.encoding" in data:
+            network_enc = data["network.encoding"]
+
+        if not network:
+            return {}
+
+        if isinstance(network, collections.abc.Mapping):
+            network = copy.deepcopy(network)
+        else:
+            LOG.debug("network data to be decoded %s", network)
+            dec_net = self._decode("metadata.network", network_enc, network)
+            network = self._load_json_or_yaml(dec_net)
+
+        LOG.debug("network data %s", network)
+        return {"network": network}
```

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/models/network.py` & `cloudbase-init-1.1.5/cloudbaseinit/models/network.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/osutils/base.py` & `cloudbase-init-1.1.5/cloudbaseinit/osutils/base.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/osutils/factory.py` & `cloudbase-init-1.1.5/cloudbaseinit/osutils/factory.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/osutils/posix.py` & `cloudbase-init-1.1.5/cloudbaseinit/osutils/posix.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/osutils/windows.py` & `cloudbase-init-1.1.5/cloudbaseinit/osutils/windows.py`

 * *Files 0% similar despite different names*

```diff
@@ -854,26 +854,33 @@
             (out, err, ret_val) = self.execute_process(args, shell=False)
             if ret_val:
                 raise exception.CloudbaseInitException(
                     'Setting MTU for interface "%(name)s" with '
                     'value "%(mtu)s" failed' % {'name': name, 'mtu': mtu})
 
     def rename_network_adapter(self, old_name, new_name):
-        base_dir = self._get_system_dir()
-        netsh_path = os.path.join(base_dir, 'netsh.exe')
-
-        args = [netsh_path, "interface", "set", "interface",
-                'name=%s' % old_name, 'newname=%s' % new_name]
-        (out, err, ret_val) = self.execute_process(args, shell=False)
-        if ret_val:
+        net_adapter = self._get_network_msft_adapter(old_name)
+        try:
+            net_adapter.rename(new_name)
+            self._get_network_msft_adapter(new_name)
+        except Exception:
             raise exception.CloudbaseInitException(
                 'Renaming interface "%(old_name)s" to "%(new_name)s" '
                 'failed' % {'old_name': old_name, 'new_name': new_name})
 
     @staticmethod
+    def _get_network_msft_adapter(name):
+        conn = wmi.WMI(moniker='//./root/standardcimv2')
+        query = conn.MSFT_NetAdapter(Name=name)
+        if not len(query):
+            raise exception.CloudbaseInitException(
+                "MSFT network adapter not found: %s" % name)
+        return query[0]
+
+    @staticmethod
     def _get_network_adapter(name):
         conn = wmi.WMI(moniker='//./root/cimv2')
         query = conn.Win32_NetworkAdapter(NetConnectionID=name)
         if not len(query):
             raise exception.CloudbaseInitException(
                 "Network adapter not found: %s" % name)
         return query[0]
```

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/base.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/base.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/constants.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/constants.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/createuser.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/createuser.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/ephemeraldisk.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/ephemeraldisk.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/execcmd.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/execcmd.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/fileexecutils.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/fileexecutils.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/localscripts.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/localscripts.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/mtu.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/mtu.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/networkconfig.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/networkconfig.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/ntpclient.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/ntpclient.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/sethostname.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/sethostname.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/setuserpassword.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/setuserpassword.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/sshpublickeys.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/sshpublickeys.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/trim.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/trim.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdata.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdata.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/base.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/base.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/cloudboothook.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/cloudboothook.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/cloudconfig.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/cloudconfig.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/base.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/base.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/factory.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/factory.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/groups.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/groups.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/runcmd.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/runcmd.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/set_hostname.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/set_hostname.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/set_ntp.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/set_ntp.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/set_timezone.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/set_timezone.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/users.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/users.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/write_files.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/cloudconfigplugins/write_files.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/factory.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/factory.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/heat.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/heat.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/multipartmixed.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/multipartmixed.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/parthandler.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/parthandler.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdataplugins/shellscript.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdataplugins/shellscript.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/common/userdatautils.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/common/userdatautils.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/factory.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/factory.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/windows/azureguestagent.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/windows/azureguestagent.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/windows/bootconfig.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/windows/bootconfig.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/windows/certificates.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/windows/certificates.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/windows/createuser.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/windows/createuser.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/windows/displayidletimeout.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/windows/displayidletimeout.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/windows/extendvolumes.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/windows/extendvolumes.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/windows/licensing.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/windows/licensing.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/windows/ntpclient.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/windows/ntpclient.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/windows/pagefiles.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/windows/pagefiles.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/windows/rdp.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/windows/rdp.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/windows/sanpolicy.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/windows/sanpolicy.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/windows/updates.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/windows/updates.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/windows/winrmcertificateauth.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/windows/winrmcertificateauth.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/plugins/windows/winrmlistener.py` & `cloudbase-init-1.1.5/cloudbaseinit/plugins/windows/winrmlistener.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/shell.py` & `cloudbase-init-1.1.5/cloudbaseinit/shell.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/fake.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/fake.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/fake_json_response.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/fake_json_response.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/osconfigdrive/test_factory.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/osconfigdrive/test_factory.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/osconfigdrive/test_windows.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/osconfigdrive/test_windows.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,16 +325,16 @@
             response = self._config_manager._get_config_drive_from_vfat(
                 self._fake_label, self._fake_metadata_file)
 
         self.assertTrue(response)
         self.osutils.get_physical_disks.assert_called_once_with()
 
         expected_is_vfat_calls = [
-            mock.call(self.osutils, mock.sentinel.drive1),
-            mock.call(self.osutils, mock.sentinel.drive2),
+            mock.call(self.osutils, mock.sentinel.drive1, self._fake_label),
+            mock.call(self.osutils, mock.sentinel.drive2, self._fake_label),
         ]
         self.assertEqual(expected_is_vfat_calls, mock_is_vfat_drive.mock_calls)
         mock_copy_from_vfat_drive.assert_called_once_with(
             self.osutils,
             mock.sentinel.drive2,
             self._config_manager.target_path)
```

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/test_azureservice.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/test_azureservice.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/test_base.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/test_base.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/test_baseconfigdrive.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/test_baseconfigdrive.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/test_baseopenstackservice.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/test_baseopenstackservice.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/test_cloudstack.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/test_cloudstack.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/test_configdrive.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/test_configdrive.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/test_ec2service.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/test_ec2service.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/test_gceservice.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/test_gceservice.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/test_httpservice.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/test_httpservice.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/test_maasservice.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/test_maasservice.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/test_opennebulaservice.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/test_opennebulaservice.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/test_ovfservice.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/test_ovfservice.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/test_packet.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/test_packet.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/services/test_vmwareguestinfoservice.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/services/test_vmwareguestinfoservice.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,27 +13,100 @@
 #    under the License.
 
 import importlib
 import unittest
 
 import ddt
 
+from cloudbaseinit.utils import serialization
+
 try:
     import unittest.mock as mock
 except ImportError:
     import mock
 
 from cloudbaseinit import conf as cloudbaseinit_conf
 from cloudbaseinit import exception
+from cloudbaseinit.models import network as network_model
 from cloudbaseinit.tests import testutils
 
 
 CONF = cloudbaseinit_conf.CONF
 BASE_MODULE_PATH = 'cloudbaseinit.metadata.services.vmwareguestinfoservice'
 MODULE_PATH = BASE_MODULE_PATH + '.VMwareGuestInfoService'
+NETWORK_CONFIG_TEST_DATA_V1 = """
+network:
+  version: 1
+  config:
+  - type: physical
+    name: eth0
+    mac_address: "00:50:56:a1:8e:43"
+    subnets:
+    - type: static
+      address: 172.26.0.37
+      netmask: 255.255.255.240
+      gateway: 172.26.0.33
+      dns_nameservers:
+      - 10.20.145.1
+      - 10.20.145.2
+"""
+NETWORK_CONFIG_TEST_DATA_V2 = """
+network:
+  version: 2
+  ethernets:
+    eth0:
+      match:
+        macaddress: "00:50:56:a1:8e:43"
+      set-name: "eth0"
+      addresses:
+      - 172.26.0.37/28
+      gateway4: 172.26.0.33
+      nameservers:
+        addresses:
+        - 10.20.145.1
+        - 10.20.145.2
+"""
+EXPECTED_NETWORK_LINK = network_model.Link(
+    id="eth0",
+    name="eth0",
+    type=network_model.LINK_TYPE_PHYSICAL,
+    enabled=True,
+    mac_address="00:50:56:a1:8e:43",
+    mtu=None,
+    bond=None,
+    vlan_link=None,
+    vlan_id=None)
+EXPECTED_NETWORK_NETWORK = network_model.Network(
+    link="eth0",
+    address_cidr="172.26.0.37/28",
+    dns_nameservers=["10.20.145.1", "10.20.145.2"],
+    routes=[network_model.Route(
+        network_cidr="0.0.0.0/0",
+        gateway="172.26.0.33")]
+)
+EXPECTED_NETWORK_NAME_SERVER = network_model.NameServerService(
+    addresses=['10.20.145.1', '10.20.145.2'],
+    search=None)
+EXPECTED_NETWORK_DETAILS_V1 = network_model.NetworkDetailsV2(
+    links=[EXPECTED_NETWORK_LINK],
+    networks=[EXPECTED_NETWORK_NETWORK],
+    services=[]
+)
+EXPECTED_NETWORK_DETAILS_V2 = network_model.NetworkDetailsV2(
+    links=[EXPECTED_NETWORK_LINK],
+    networks=[EXPECTED_NETWORK_NETWORK],
+    services=[EXPECTED_NETWORK_NAME_SERVER]
+)
+NETWORK_CONFIG_TEST_DATA_V2_GZIPB64 = """
+network: |
+    H4sIAHWT3mUCA22OSQrDMAxF9zmFyD6uPGRAtzGJaLqIC5ZJ6e3roYVSCgJJ/389dHKU2z0QmI7TzjFwEuo
+    A8oKlAxw+rXsby7L6bYssQtAj0phrIq9pYXK2rynhNAR/cE4UShPfVyyNNICejTKTQmXni1mqePWJH/7p6M
+    u01Sk44XjmZz+f/AArEpVBpd2o9B/NdC+Zoo9N7AAAAA==
+network.encoding: gzip+base64
+"""
 
 
 class FakeException(Exception):
     pass
 
 
 @ddt.ddt
@@ -86,55 +159,69 @@
         self._test_load_no_rpc_tool(expected_output, 'fake_path')
 
     @mock.patch('os.path.exists')
     @mock.patch('cloudbaseinit.utils.serialization.parse_json_yaml')
     @mock.patch(MODULE_PATH + "._get_guest_data")
     def _test_load_meta_data(self, mock_get_guestinfo, mock_parse,
                              mock_os_path_exists, parse_return=None,
-                             get_guest_data_result=None, exception=False,
+                             get_guest_data_results=None, exception=False,
                              expected_result=None, meta_data_return=False):
 
         mock_os_path_exists.return_value = True
         mock_parse.return_value = parse_return
 
         if not exception:
-            mock_get_guestinfo.return_value = get_guest_data_result
+            mock_get_guestinfo.side_effect = get_guest_data_results
             result = self._service.load()
             self.assertEqual(result, expected_result)
-            mock_get_guestinfo.assert_called_with('userdata')
-            mock_parse.assert_called_once_with(get_guest_data_result)
+            self.assertEqual(mock_get_guestinfo.call_args_list[0].args,
+                             ('metadata',))
+            self.assertEqual(mock_get_guestinfo.call_args_list[1].args,
+                             ('userdata',))
+            if get_guest_data_results and len(get_guest_data_results) > 1 \
+                    and get_guest_data_results[0]:
+                mock_parse.assert_called_once_with(get_guest_data_results[0])
             self.assertEqual(mock_get_guestinfo.call_count, 2)
             self.assertEqual(self._service._meta_data, meta_data_return)
-            self.assertEqual(self._service._user_data, get_guest_data_result)
+            self.assertEqual(self._service._user_data,
+                             get_guest_data_results[1])
         else:
             mock_get_guestinfo.side_effect = FakeException("Fake")
             self.assertRaises(FakeException, self._service.load)
 
     def test_load_no_meta_data(self):
-        self._test_load_meta_data(meta_data_return={})
+        self._test_load_meta_data(meta_data_return={},
+                                  expected_result=True,
+                                  get_guest_data_results=[None,
+                                                          "fake userdata"])
 
     def test_load_no_user_data(self):
         parse_return = {"fake": "metadata"}
         self._test_load_meta_data(parse_return=parse_return,
                                   expected_result=True,
+                                  get_guest_data_results=["fake metadata",
+                                                          None],
                                   meta_data_return=parse_return)
 
     def test_load_fail(self):
         self._test_load_meta_data(parse_return={"fake": "metadata"},
                                   exception=True)
 
     def test_load(self):
         parse_return = {"fake": "metadata"}
         self._test_load_meta_data(parse_return=parse_return,
-                                  get_guest_data_result="fake userdata",
+                                  get_guest_data_results=["fake metadata",
+                                                          "fake userdata"],
                                   expected_result=True,
                                   meta_data_return=parse_return)
 
     def test_load_no_dict_metadata(self):
         self._test_load_meta_data(parse_return="not_a_dict",
+                                  get_guest_data_results=["fake metadata",
+                                                          None],
                                   expected_result=None, meta_data_return={})
 
     @ddt.data((None, []),
               ('', []),
               (b'', []),
               (b'ssh1', [b"ssh1"]),
               ('ssh1', ["ssh1"]),
@@ -177,13 +264,36 @@
 
         data = self._service._get_guest_data(data_key)
 
         self.assertEqual(data, decoded_data)
         mock_decode_data.assert_called_once_with(data_key_ret,
                                                  is_base64, is_gzip)
 
+    @ddt.data(({}, None),
+              (serialization.parse_json_yaml(NETWORK_CONFIG_TEST_DATA_V1),
+               EXPECTED_NETWORK_DETAILS_V1),
+              (serialization.parse_json_yaml(NETWORK_CONFIG_TEST_DATA_V2),
+               EXPECTED_NETWORK_DETAILS_V2))
+    @ddt.unpack
+    def test_get_network_details(self, network_data, expected_return_value):
+        self._service._meta_data = network_data
+
+        network_v2 = self._service.get_network_details_v2()
+        self.assertEqual(network_v2, expected_return_value)
+
+    @mock.patch(MODULE_PATH + "._get_guest_data")
+    @mock.patch('os.path.exists')
+    def test_get_network_details_v2_b64(self, mock_os_path_exists,
+                                        mock_get_guest_data):
+        mock_os_path_exists.return_value = True
+        mock_get_guest_data.return_value = NETWORK_CONFIG_TEST_DATA_V2_GZIPB64
+
+        self._service.load()
+        network_v2 = self._service.get_network_details_v2()
+        self.assertEqual(network_v2, EXPECTED_NETWORK_DETAILS_V2)
+
     @mock.patch(MODULE_PATH + "._get_guestinfo_value")
     def test_get_guest_data_fail(self, mock_get_guestinfo_value):
 
         mock_get_guestinfo_value.return_value = "no encoding"
         self.assertRaises(exception.CloudbaseInitException,
                           self._service._get_guest_data, 'fake_key')
```

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/metadata/test_factory.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/metadata/test_factory.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/osutils/test_base.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/osutils/test_base.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/osutils/test_factory.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/osutils/test_factory.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/osutils/test_windows.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/osutils/test_windows.py`

 * *Files 1% similar despite different names*

```diff
@@ -835,36 +835,41 @@
     def test_set_static_network_config_ipv4(self):
         self._test_set_static_network_config(ipv6=False)
 
     def test_set_static_network_config_ipv6(self):
         self._test_set_static_network_config(ipv6=True)
 
     @mock.patch('cloudbaseinit.osutils.windows.WindowsUtils'
-                '.execute_process')
-    @mock.patch('cloudbaseinit.osutils.windows.WindowsUtils'
-                '._get_system_dir')
-    def _test_rename_network_adapter(self, should_fail, mock_get_system_dir,
-                                     mock_execute_process):
-        base_dir = "fake path"
+                '._get_network_msft_adapter')
+    def _test_rename_network_adapter(self, rename_exception,
+                                     mock_get_network_adapter):
         old_name = "fake_old"
         new_name = "fake_new"
-        mock_get_system_dir.return_value = base_dir
-        ret_val = 1 if should_fail else 0
-        mock_execute_process.return_value = (None, None, ret_val)
 
-        if should_fail:
+        adapter = mock.Mock()
+        adapter.Name = mock.sentinel.old_name
+        mock_get_network_adapter.return_value = adapter
+        get_network_adapter_called = 1
+        if rename_exception:
+            adapter.rename.side_effect = Exception("fake exception")
             with self.assertRaises(exception.CloudbaseInitException):
                 self._winutils.rename_network_adapter(old_name, new_name)
         else:
+            get_network_adapter_called = 2
             self._winutils.rename_network_adapter(old_name, new_name)
 
-        mock_get_system_dir.assert_called_once_with()
-        args = [os.path.join(base_dir, "netsh.exe"), "interface", "set",
-                "interface", 'name=%s' % old_name, 'newname=%s' % new_name]
-        mock_execute_process.assert_called_once_with(args, shell=False)
+        adapter.rename.assert_called()
+
+        self.assertEqual(mock_get_network_adapter.call_count,
+                         get_network_adapter_called)
+        self.assertEqual(mock_get_network_adapter.call_args_list[0].args,
+                         (old_name,))
+        if not exception:
+            self.assertEqual(mock_get_network_adapter.call_args_list[1].args,
+                             (new_name,))
 
     def _test_get_config_key_name(self, section):
         response = self._winutils._get_config_key_name(section)
         if section:
             self.assertEqual(self._winutils._config_key + section + '\\',
                              response)
         else:
```

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/test_createuser.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/test_createuser.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/test_ephemeraldisk.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/test_ephemeraldisk.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/test_execcmd.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/test_execcmd.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/test_fileexecutils.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/test_fileexecutils.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/test_localscripts.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/test_localscripts.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/test_mtu.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/test_mtu.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/test_networkconfig.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/test_networkconfig.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/test_ntpclient.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/test_ntpclient.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/test_sethostname.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/test_sethostname.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/test_setuserpassword.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/test_setuserpassword.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/test_sshpublickeys.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/test_sshpublickeys.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/test_trim.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/test_trim.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/test_userdata.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/test_userdata.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/test_userdatautils.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/test_userdatautils.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/test_groups.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/test_groups.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/test_runcmd.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/test_runcmd.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/test_set_hostname.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/test_set_hostname.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/test_set_ntp.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/test_set_ntp.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/test_set_timezone.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/test_set_timezone.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/test_users.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/test_users.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/test_write_files.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/userdataplugins/cloudconfigplugins/test_write_files.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/userdataplugins/test_cloudboothook.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/userdataplugins/test_cloudboothook.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/userdataplugins/test_cloudconfig.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/userdataplugins/test_cloudconfig.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/userdataplugins/test_factory.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/userdataplugins/test_factory.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/userdataplugins/test_heat.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/userdataplugins/test_heat.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/userdataplugins/test_parthandler.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/userdataplugins/test_parthandler.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/common/userdataplugins/test_shellscript.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/common/userdataplugins/test_shellscript.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/test_factory.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/test_factory.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/windows/test_azureguestagent.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/windows/test_azureguestagent.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/windows/test_bootconfig.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/windows/test_bootconfig.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/windows/test_certificates.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/windows/test_certificates.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/windows/test_createuser.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/windows/test_createuser.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/windows/test_displayidletimeout.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/windows/test_displayidletimeout.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/windows/test_extendvolumes.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/windows/test_extendvolumes.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/windows/test_licensing.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/windows/test_licensing.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/windows/test_ntpclient.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/windows/test_ntpclient.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/windows/test_pagefiles.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/windows/test_pagefiles.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/windows/test_rdp.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/windows/test_rdp.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/windows/test_sanpolicy.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/windows/test_sanpolicy.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/windows/test_updates.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/windows/test_updates.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/windows/test_winrmcertificateauth.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/windows/test_winrmcertificateauth.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/plugins/windows/test_winrmlistener.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/plugins/windows/test_winrmlistener.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/resources/cloud_config_userdata` & `cloudbase-init-1.1.5/cloudbaseinit/tests/resources/cloud_config_userdata`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/test_exception.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/test_init.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/test_init.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,22 +56,26 @@
         self._module_patcher.stop()
 
     def _test_get_plugin_section(self, instance_id):
         response = self._init._get_plugins_section(instance_id=instance_id)
         if not instance_id:
             self.assertEqual(self._init._PLUGINS_CONFIG_SECTION, response)
         else:
-            self.assertEqual(
-                instance_id + "/" + self._init._PLUGINS_CONFIG_SECTION,
-                response)
+            expected_response = (
+                "%s/%s" % (instance_id, self._init._PLUGINS_CONFIG_SECTION))
+            self.assertEqual(expected_response, response)
 
     def test_get_plugin_section_id(self):
         fake_id = "100"
         self._test_get_plugin_section(instance_id=fake_id)
 
+    def test_get_plugin_section_id_int(self):
+        fake_id = 100
+        self._test_get_plugin_section(instance_id=fake_id)
+
     def test_get_plugin_section_no_id(self):
         self._test_get_plugin_section(instance_id=None)
 
     @mock.patch('cloudbaseinit.init.InitManager._get_plugins_section')
     def test_get_plugin_status(self, mock_get_plugins_section):
         self.osutils.get_config_value.return_value = 1
         response = self._init._get_plugin_status(self.osutils, 'fake id',
```

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/test_version.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/testutils.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/testutils.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/template_engine/test_base_template.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/template_engine/test_base_template.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/template_engine/test_factory.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/template_engine/test_factory.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/template_engine/test_jinja2_template.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/template_engine/test_jinja2_template.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/test_classloader.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/test_classloader.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/test_crypt.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/test_crypt.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/test_debiface.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/test_debiface.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/test_dhcp.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/test_dhcp.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/test_encoding.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/test_encoding.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/test_hostname.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/test_hostname.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/test_log.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/test_log.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/test_network.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/test_network.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/test_retry_decorator.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/test_retry_decorator.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/test_serialization.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/test_serialization.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/storage/test_factory.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/storage/test_factory.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/storage/test_vds_storage_manager.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/storage/test_vds_storage_manager.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/storage/test_wsm_storage_manager.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/storage/test_wsm_storage_manager.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_bootconfig.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_bootconfig.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_disk.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_disk.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_licensing.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_licensing.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_netlbfo.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_netlbfo.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_network.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_network.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_powercfg.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_powercfg.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_privilege.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_privilege.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_rdp.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_rdp.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_security.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_security.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_timezone.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_timezone.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_updates.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_updates.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_vds.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_vds.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_vfat.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_vfat.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,25 +27,27 @@
 CONF = vfat.CONF
 
 
 class TestVfat(unittest.TestCase):
 
     def _test_is_vfat_drive(self, execute_process_value,
                             expected_logging,
-                            expected_response):
+                            expected_response,
+                            drive_label='config-2'):
 
         mock_osutils = mock.Mock()
         mock_osutils.execute_process.return_value = execute_process_value
 
         with testutils.LogSnatcher('cloudbaseinit.utils.windows.'
                                    'vfat') as snatcher:
             with testutils.ConfPatcher('mtools_path', 'mtools_path'):
 
                 response = vfat.is_vfat_drive(mock_osutils,
-                                              mock.sentinel.drive)
+                                              mock.sentinel.drive,
+                                              drive_label)
 
                 mdir = os.path.join(CONF.mtools_path, "mlabel.exe")
                 mock_osutils.execute_process.assert_called_once_with(
                     [mdir, "-i", mock.sentinel.drive, "-s"],
                     shell=False)
 
         self.assertEqual(expected_logging, snatcher.output)
@@ -101,14 +103,28 @@
         execute_process_value = (mock_out, None, 0)
         expected_response = True
 
         self._test_is_vfat_drive(execute_process_value=execute_process_value,
                                  expected_logging=expected_logging,
                                  expected_response=expected_response)
 
+    def test_is_vfat_drive_works_alternate_drive_label(self):
+        mock_out = b"Volume label is CIDATA    \r\n"
+        expected_logging = [
+            "Obtained label information for drive %r: %r"
+            % (mock.sentinel.drive, mock_out)
+        ]
+        execute_process_value = (mock_out, None, 0)
+        expected_response = True
+
+        self._test_is_vfat_drive(execute_process_value=execute_process_value,
+                                 expected_logging=expected_logging,
+                                 expected_response=expected_response,
+                                 drive_label='cidata')
+
     def test_is_vfat_drive_with_wrong_label(self):
         mock_out = b"Not volu label  \r\n"
         expected_logging = [
             "Obtained label information for drive %r: %r"
             % (mock.sentinel.drive, mock_out)
         ]
         execute_process_value = (mock_out, None, 0)
@@ -139,15 +155,16 @@
         mock_osutils.execute_process.assert_called_once_with(
             [mcopy, "-s", "-n", "-i", mock.sentinel.drive, "::/", "."],
             shell=False)
 
     def test_is_vfat_drive_mtools_not_given(self):
         with self.assertRaises(exception.CloudbaseInitException) as cm:
             vfat.is_vfat_drive(mock.sentinel.osutils,
-                               mock.sentinel.target_path)
+                               mock.sentinel.target_path,
+                               mock.sentinel.drive_label)
         expected_message = ('"mtools_path" needs to be provided in order '
                             'to access VFAT drives')
         self.assertEqual(expected_message, str(cm.exception.args[0]))
 
     def test_copy_from_vfat_drive_mtools_not_given(self):
         with self.assertRaises(exception.CloudbaseInitException) as cm:
             vfat.copy_from_vfat_drive(mock.sentinel.osutils,
```

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_winrmconfig.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_winrmconfig.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_wmi_loader.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_wmi_loader.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_ws2_32.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_ws2_32.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/tests/utils/windows/test_x509.py` & `cloudbase-init-1.1.5/cloudbaseinit/tests/utils/windows/test_x509.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/classloader.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/classloader.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/crypt.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/debiface.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/debiface.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/dhcp.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/dhcp.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/encoding.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/hostname.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/hostname.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/log.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/log.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/network.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/network.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/network_team.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/network_team.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/retry_decorator.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/retry_decorator.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/serialization.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/template_engine/base_template.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/template_engine/base_template.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/template_engine/factory.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/template_engine/factory.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/template_engine/jinja2_template.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/template_engine/jinja2_template.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/windows/bootconfig.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/windows/bootconfig.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/windows/cryptoapi.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/windows/cryptoapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,16 +133,18 @@
 PROV_RSA_FULL = 1
 X509_ASN_ENCODING = 1
 CERT_FIND_ANY = 0
 CERT_FIND_SHA1_HASH = 0x10000
 CERT_KEY_PROV_INFO_PROP_ID = 2
 CERT_KEY_CONTEXT_PROP_ID = 5
 
+# https://learn.microsoft.com/en-us/windows/win32/api/wincrypt/ns-wincrypt-crypt_algorithm_identifier
 szOID_PKIX_KP_SERVER_AUTH = b"1.3.6.1.5.5.7.3.1"
 szOID_RSA_SHA1RSA = b"1.2.840.113549.1.1.5"
+szOID_RSA_SHA256RSA = b"1.2.840.113549.1.1.11"
 
 advapi32 = windll.advapi32
 crypt32 = windll.crypt32
 kernel32 = windll.kernel32
 
 advapi32.CryptAcquireContextW.restype = wintypes.BOOL
 advapi32.CryptAcquireContextW.argtypes = [wintypes.HANDLE, wintypes.LPCWSTR,
```

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/windows/disk.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/windows/disk.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/windows/iphlpapi.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/windows/iphlpapi.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/windows/kernel32.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/windows/kernel32.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/windows/licensing.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/windows/licensing.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/windows/netlbfo.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/windows/netlbfo.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/windows/network.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/windows/network.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/windows/powercfg.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/windows/powercfg.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/windows/privilege.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/windows/privilege.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/windows/productkeys.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/windows/productkeys.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/windows/rdp.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/windows/rdp.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/windows/security.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/windows/security.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/windows/storage/base.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/windows/storage/base.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/windows/storage/factory.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/windows/storage/factory.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/windows/storage/vds_storage_manager.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/windows/storage/vds_storage_manager.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/windows/storage/wsm_storage_manager.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/windows/storage/wsm_storage_manager.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/windows/timezone.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/windows/timezone.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/windows/updates.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/windows/updates.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/windows/vds.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/windows/vds.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/windows/vfat.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/windows/vfat.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,27 +18,26 @@
 from oslo_log import log as oslo_logging
 
 from cloudbaseinit import conf as cloudbaseinit_conf
 from cloudbaseinit import exception
 
 
 CONF = cloudbaseinit_conf.CONF
-CONFIG_DRIVE_LABELS = ['config-2', 'CONFIG-2']
 LOG = oslo_logging.getLogger(__name__)
 VOLUME_LABEL_REGEX = re.compile("Volume label is (.*?)$")
 
 
 def _check_mtools_path():
     if not CONF.mtools_path:
         raise exception.CloudbaseInitException(
             '"mtools_path" needs to be provided in order '
             'to access VFAT drives')
 
 
-def is_vfat_drive(osutils, drive_path):
+def is_vfat_drive(osutils, drive_path, drive_label):
     """Check if the given drive contains a VFAT filesystem."""
     _check_mtools_path()
     mlabel = os.path.join(CONF.mtools_path, "mlabel.exe")
     args = [mlabel, "-i", drive_path, "-s"]
 
     out, err, exit_code = osutils.execute_process(args, shell=False)
     if exit_code:
@@ -46,15 +45,16 @@
                   drive_path)
         LOG.debug("mlabel failed with error %r", err)
         return False
 
     LOG.debug("Obtained label information for drive %r: %r", drive_path, out)
     out = out.decode().strip()
     match = VOLUME_LABEL_REGEX.search(out)
-    return match.group(1) in CONFIG_DRIVE_LABELS if match else False
+    drive_labels = [drive_label.lower(), drive_label.upper()]
+    return match.group(1) in drive_labels if match else False
 
 
 def copy_from_vfat_drive(osutils, drive_path, target_path):
     """Copy everything from the given VFAT drive into the given target."""
     _check_mtools_path()
     cwd = os.getcwd()
     try:
```

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/windows/winrmconfig.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/windows/winrmconfig.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/windows/wmi_loader.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/windows/wmi_loader.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/windows/ws2_32.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/windows/ws2_32.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/windows/x509.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/windows/x509.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
 
             if machine_keyset:
                 key_prov_info.dwFlags = cryptoapi.CRYPT_MACHINE_KEYSET
             else:
                 key_prov_info.dwFlags = 0
 
             sign_alg = cryptoapi.CRYPT_ALGORITHM_IDENTIFIER()
-            sign_alg.pszObjId = cryptoapi.szOID_RSA_SHA1RSA
+            sign_alg.pszObjId = cryptoapi.szOID_RSA_SHA256RSA
 
             start_time = cryptoapi.SYSTEMTIME()
             cryptoapi.GetSystemTime(ctypes.byref(start_time))
 
             end_time = self._add_system_time_interval(
                 start_time, X509_END_DATE_INTERVAL)
```

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/utils/x509constants.py` & `cloudbase-init-1.1.5/cloudbaseinit/utils/x509constants.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/cloudbaseinit/version.py` & `cloudbase-init-1.1.5/cloudbaseinit/version.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/doc/Makefile` & `cloudbase-init-1.1.5/doc/Makefile`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/doc/make.bat` & `cloudbase-init-1.1.5/doc/make.bat`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/doc/source/conf.py` & `cloudbase-init-1.1.5/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/doc/source/index.rst` & `cloudbase-init-1.1.5/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/doc/source/intro.rst` & `cloudbase-init-1.1.5/doc/source/intro.rst`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/doc/source/plugins.rst` & `cloudbase-init-1.1.5/doc/source/plugins.rst`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/doc/source/services.rst` & `cloudbase-init-1.1.5/doc/source/services.rst`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 
 Capabilities:
 
     * instance id
     * hostname
     * public keys
     * static network configuration (Debian and `network config v1
-      <https://cloudinit.readthedocs.io/en/latest/topics/network-config-format-v1.html>`_
+      <https://cloudinit.readthedocs.io/en/22.4.2/topics/network-config-format-v1.html>`__
       formats)
     * user data
 
 Config options for `config_drive` section:
 
     * raw_hdd (bool: True)
     * cdrom (bool: True)
@@ -514,14 +514,28 @@
     instance-id: cloud-vm
     local-hostname: cloud-vm
     admin-username: cloud-username
     admin-password: Passw0rd
     public-keys-data: |
       ssh-key 1
       ssh-key 2
+    network:
+      version: 2
+      ethernets:
+        id0:
+          match:
+            macaddress: "00:50:56:a1:8e:43"
+          set-name: "eth0"
+          addresses:
+          - 172.26.0.37/28
+          gateway4: 172.26.0.33
+          nameservers:
+            addresses:
+            - 10.20.145.1
+            - 10.20.145.2
 
 This metadata content needs to be set as string in the guestinfo
 dictionary, thus needs to be converted to base64 (it is recommended to
 gzip it too).
 To convert to gzip+base64 format:
 
 .. code-block:: bash
@@ -544,14 +558,15 @@
 
 
 Capabilities:
 
     * instance id
     * hostname
     * public keys
+    * static network configuration
     * admin user name
     * admin user password
     * user data
 
 Config options for `vmwareguestinfo` section:
 
     * vmware_rpctool_path (string: "%ProgramFiles%/VMware/VMware Tools/rpctool.exe")
```

### Comparing `cloudbase-init-1.1.4/doc/source/tutorial.rst` & `cloudbase-init-1.1.5/doc/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/doc/source/userdata.rst` & `cloudbase-init-1.1.5/doc/source/userdata.rst`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/releasenotes/source/conf.py` & `cloudbase-init-1.1.5/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/setup.cfg` & `cloudbase-init-1.1.5/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cloudbase-init
-version = 1.1.4
+version = 1.1.5
 summary = Portable cloud initialization service
 description-file = 
 	README.rst
 author = Cloudbase Solutions Srl
 author-email = apilotti@cloudbasesolutions.com
 home-page = http://www.cloudbase.it/
 classifier = 
@@ -14,14 +14,15 @@
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [files]
 packages = 
 	cloudbaseinit
 
 [global]
 setup-hooks =
```

### Comparing `cloudbase-init-1.1.4/setup.py` & `cloudbase-init-1.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/test-requirements.txt` & `cloudbase-init-1.1.5/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `cloudbase-init-1.1.4/tox.ini` & `cloudbase-init-1.1.5/tox.ini`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 envlist = py3,pep8
 skipsdist = True
 
 [testenv]
 usedevelop = True
 setenv = VIRTUAL_ENV={envdir}
 deps =
-  -c{env:UPPER_CONSTRAINTS_FILE:https://opendev.org/openstack/requirements/raw/branch/master/upper-constraints.txt}
+  -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
   -r{toxinidir}/test-requirements.txt
   -r{toxinidir}/requirements.txt
 commands = stestr run --slowest {posargs}
 
 [testenv:pep8]
 commands = flake8 {posargs}
 
@@ -27,14 +27,15 @@
   coverage xml -o cover/coverage.xml
 
 [testenv:venv]
 commands = {posargs}
 
 [testenv:docs]
 deps =
+  -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
   -r{toxinidir}/doc/requirements.txt
   -egit+https://github.com/openstack/cloudbase-init\#egg=cloudbase-init
 commands =
   sphinx-build -a -E -W -d doc/build/doctrees -b html doc/source doc/build/html
 
 [testenv:releasenotes]
 deps = {[testenv:docs]deps}
```

