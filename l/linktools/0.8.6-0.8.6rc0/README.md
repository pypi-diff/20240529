# Comparing `tmp/linktools-0.8.6.tar.gz` & `tmp/linktools-0.8.6rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktools-0.8.6.tar", last modified: Wed May 29 14:31:56 2024, max compression
+gzip compressed data, was "linktools-0.8.6rc0.tar", last modified: Wed May 15 15:42:03 2024, max compression
```

## Comparing `linktools-0.8.6.tar` & `linktools-0.8.6rc0.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:31:56.486642 linktools-0.8.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11895 2024-05-29 14:29:34.000000 linktools-0.8.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-29 14:29:34.000000 linktools-0.8.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    35452 2024-05-29 14:31:56.486642 linktools-0.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    33405 2024-05-29 14:29:34.000000 linktools-0.8.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-29 14:29:34.000000 linktools-0.8.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 14:31:56.486642 linktools-0.8.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     4278 2024-05-29 14:29:34.000000 linktools-0.8.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:31:56.466642 linktools-0.8.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:31:56.470642 linktools-0.8.6/src/linktools/
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21565 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/_environ.py
--rw-r--r--   0 runner    (1001) docker     (127)    20616 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/_url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:31:56.470642 linktools-0.8.6/src/linktools/android/
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/android/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23899 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/android/adb.py
--rw-r--r--   0 runner    (1001) docker     (127)    13360 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/android/struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:31:56.474642 linktools-0.8.6/src/linktools/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/assets/android-frida.json
--rw-r--r--   0 runner    (1001) docker     (127)    82987 2024-05-29 14:31:50.000000 linktools-0.8.6/src/linktools/assets/android-tools.apk
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-29 14:31:50.000000 linktools-0.8.6/src/linktools/assets/android-tools.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:31:56.466642 linktools-0.8.6/src/linktools/assets/containers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:31:56.474642 linktools-0.8.6/src/linktools/assets/containers/100-nginx/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/assets/containers/100-nginx/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/assets/containers/100-nginx/compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/assets/containers/100-nginx/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    47272 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/assets/containers/100-nginx/dnsapi.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/assets/containers/100-nginx/http.conf
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/assets/containers/100-nginx/https.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:31:56.474642 linktools-0.8.6/src/linktools/assets/containers/110-portainer/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/assets/containers/110-portainer/compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/assets/containers/110-portainer/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/assets/containers/110-portainer/nginx.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:31:56.474642 linktools-0.8.6/src/linktools/assets/containers/120-flare/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/assets/containers/120-flare/compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/assets/containers/120-flare/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/assets/containers/120-flare/nginx.conf
--rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/assets/fake_useragent.json
--rw-r--r--   0 runner    (1001) docker     (127)    44744 2024-05-29 14:29:40.000000 linktools-0.8.6/src/linktools/assets/frida.js
--rw-r--r--   0 runner    (1001) docker     (127)    24005 2024-05-29 14:29:40.000000 linktools-0.8.6/src/linktools/assets/frida.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:31:56.466642 linktools-0.8.6/src/linktools/assets/objection/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:31:56.474642 linktools-0.8.6/src/linktools/assets/objection/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/assets/objection/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15614 2024-05-29 14:31:56.000000 linktools-0.8.6/src/linktools/assets/tools.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:31:56.474642 linktools-0.8.6/src/linktools/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/cli/argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    31604 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/cli/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:31:56.474642 linktools-0.8.6/src/linktools/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/cli/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:31:56.478642 linktools-0.8.6/src/linktools/cli/commands/android/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/cli/commands/android/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2494 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/cli/commands/android/adb.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2140 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/cli/commands/android/agent.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15066 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/cli/commands/android/app.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2614 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/cli/commands/android/debug.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7405 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/cli/commands/android/frida.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/cli/commands/android/info.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4937 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/cli/commands/android/intent.py
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/cli/commands/android/objection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15517 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/cli/commands/android/pidcat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4383 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/cli/commands/android/top.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:31:56.478642 linktools-0.8.6/src/linktools/cli/commands/common/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/cli/commands/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/cli/commands/common/cert.py
--rw-r--r--   0 runner    (1001) docker     (127)    15318 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/cli/commands/common/cntr.py
--rw-r--r--   0 runner    (1001) docker     (127)     9255 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/cli/commands/common/env.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/cli/commands/common/grep.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4143 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/cli/commands/common/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:31:56.478642 linktools-0.8.6/src/linktools/cli/commands/ios/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/cli/commands/ios/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6351 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/cli/commands/ios/frida.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/cli/commands/ios/ipa.py
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/cli/commands/ios/objection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/cli/commands/ios/scp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/cli/commands/ios/sib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/cli/commands/ios/ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)    17530 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/cli/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:31:56.478642 linktools-0.8.6/src/linktools/container/
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16132 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/container/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    21050 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/container/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/container/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:31:56.482642 linktools-0.8.6/src/linktools/frida/
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/frida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/frida/android.py
--rw-r--r--   0 runner    (1001) docker     (127)    30766 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/frida/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/frida/ios.py
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/frida/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/frida/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:31:56.482642 linktools-0.8.6/src/linktools/ida/
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/ida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/ida/ida.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:31:56.482642 linktools-0.8.6/src/linktools/ios/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/ios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/ios/ipa.py
--rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/ios/sib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/ios/struct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-29 14:31:56.000000 linktools-0.8.6/src/linktools/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/reactor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:31:56.482642 linktools-0.8.6/src/linktools/references/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/references/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:31:56.482642 linktools-0.8.6/src/linktools/references/fake_useragent/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/references/fake_useragent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/references/fake_useragent/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/references/fake_useragent/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/references/fake_useragent/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/references/fake_useragent/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/references/fake_useragent/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/rich.py
--rw-r--r--   0 runner    (1001) docker     (127)    13556 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:31:56.482642 linktools-0.8.6/src/linktools/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/utils/_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/utils/_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/utils/_subprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19476 2024-05-29 14:29:34.000000 linktools-0.8.6/src/linktools/utils/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:31:56.482642 linktools-0.8.6/src/linktools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    35452 2024-05-29 14:31:56.000000 linktools-0.8.6/src/linktools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-29 14:31:56.000000 linktools-0.8.6/src/linktools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 14:31:56.000000 linktools-0.8.6/src/linktools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-29 14:31:56.000000 linktools-0.8.6/src/linktools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-29 14:31:56.000000 linktools-0.8.6/src/linktools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-29 14:31:56.000000 linktools-0.8.6/src/linktools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.391425 linktools-0.8.6rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11895 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    35455 2024-05-15 15:42:03.391425 linktools-0.8.6rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    33405 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 15:42:03.391425 linktools-0.8.6rc0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4278 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.367425 linktools-0.8.6rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.375425 linktools-0.8.6rc0/src/linktools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21680 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12625 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/_environ.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20344 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.375425 linktools-0.8.6rc0/src/linktools/android/
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/android/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23773 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/android/adb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13360 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/android/struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.375425 linktools-0.8.6rc0/src/linktools/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    82987 2024-05-15 15:41:57.000000 linktools-0.8.6rc0/src/linktools/assets/android-tools.apk
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-15 15:41:57.000000 linktools-0.8.6rc0/src/linktools/assets/android-tools.json
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/assets/chrome-driver.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.371425 linktools-0.8.6rc0/src/linktools/assets/containers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.379425 linktools-0.8.6rc0/src/linktools/assets/containers/100-nginx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/assets/containers/100-nginx/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/assets/containers/100-nginx/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/assets/containers/100-nginx/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47272 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/assets/containers/100-nginx/dnsapi.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/assets/containers/100-nginx/http.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/assets/containers/100-nginx/https.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.379425 linktools-0.8.6rc0/src/linktools/assets/containers/110-portainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/assets/containers/110-portainer/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/assets/containers/110-portainer/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/assets/containers/110-portainer/nginx.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.379425 linktools-0.8.6rc0/src/linktools/assets/containers/120-flare/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/assets/containers/120-flare/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/assets/containers/120-flare/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/assets/containers/120-flare/nginx.conf
+-rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/assets/fake_useragent.json
+-rw-r--r--   0 runner    (1001) docker     (127)    44744 2024-05-15 15:40:20.000000 linktools-0.8.6rc0/src/linktools/assets/frida.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24005 2024-05-15 15:40:21.000000 linktools-0.8.6rc0/src/linktools/assets/frida.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.371425 linktools-0.8.6rc0/src/linktools/assets/objection/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.379425 linktools-0.8.6rc0/src/linktools/assets/objection/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/assets/objection/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15614 2024-05-15 15:42:03.000000 linktools-0.8.6rc0/src/linktools/assets/tools.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.379425 linktools-0.8.6rc0/src/linktools/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31604 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.379425 linktools-0.8.6rc0/src/linktools/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.383425 linktools-0.8.6rc0/src/linktools/cli/commands/android/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/android/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2494 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/android/adb.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2140 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/android/agent.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15066 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/android/app.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2614 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/android/debug.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7405 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/android/frida.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/android/info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4937 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/android/intent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/android/objection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15517 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/android/pidcat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4383 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/android/top.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.383425 linktools-0.8.6rc0/src/linktools/cli/commands/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/common/cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15318 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/common/cntr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9255 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/common/env.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/common/grep.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4143 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/common/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.383425 linktools-0.8.6rc0/src/linktools/cli/commands/ios/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/ios/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6351 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/ios/frida.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/ios/ipa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/ios/objection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/ios/scp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/ios/sib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/ios/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17530 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.383425 linktools-0.8.6rc0/src/linktools/container/
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16132 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/container/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21050 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/container/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/container/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.387425 linktools-0.8.6rc0/src/linktools/frida/
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/frida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/frida/android.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30766 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/frida/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/frida/ios.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/frida/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/frida/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.387425 linktools-0.8.6rc0/src/linktools/ida/
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/ida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/ida/ida.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.387425 linktools-0.8.6rc0/src/linktools/ios/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/ios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/ios/ipa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/ios/sib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/ios/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-15 15:42:03.000000 linktools-0.8.6rc0/src/linktools/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/reactor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.387425 linktools-0.8.6rc0/src/linktools/references/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/references/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.387425 linktools-0.8.6rc0/src/linktools/references/fake_useragent/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/references/fake_useragent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/references/fake_useragent/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/references/fake_useragent/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/references/fake_useragent/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/references/fake_useragent/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/references/fake_useragent/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/rich.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13556 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.387425 linktools-0.8.6rc0/src/linktools/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/utils/_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/utils/_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/utils/_subprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19476 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/utils/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.387425 linktools-0.8.6rc0/src/linktools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    35455 2024-05-15 15:42:03.000000 linktools-0.8.6rc0/src/linktools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-15 15:42:03.000000 linktools-0.8.6rc0/src/linktools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 15:42:03.000000 linktools-0.8.6rc0/src/linktools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-15 15:42:03.000000 linktools-0.8.6rc0/src/linktools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-15 15:42:03.000000 linktools-0.8.6rc0/src/linktools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 15:42:03.000000 linktools-0.8.6rc0/src/linktools.egg-info/top_level.txt
```

### Comparing `linktools-0.8.6/LICENSE` & `linktools-0.8.6rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/PKG-INFO` & `linktools-0.8.6rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linktools
-Version: 0.8.6
+Version: 0.8.6rc0
 Summary: linktools toolkit
 Author-email: Hu Ji <669898595@qq.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/ice-black-tea/linktools
 Project-URL: Repository, https://github.com/ice-black-tea/linktools.git
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `linktools-0.8.6/README.md` & `linktools-0.8.6rc0/README.md`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/pyproject.toml` & `linktools-0.8.6rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/setup.py` & `linktools-0.8.6rc0/setup.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/__init__.py` & `linktools-0.8.6rc0/src/linktools/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/__main__.py` & `linktools-0.8.6rc0/src/linktools/__main__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/_config.py` & `linktools-0.8.6rc0/src/linktools/_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -253,31 +253,33 @@
 
 class Config:
     __lock__ = threading.RLock()
 
     def __init__(
             self,
             environ: "BaseEnviron",
-            data: ConfigDict,
+            config: ConfigDict,
             namespace: str = __missing__,
             prefix: str = __missing__,
+            share: bool = False
     ):
         """
         初始化配置对象
         :param environ: 环境对象
-        :param data: 配置相关数据
+        :param config: 配置相关数据
         :param namespace: 缓存对应的命名空间
         :param prefix: 环境变量前缀
+        :param share: 是否共享配置
         """
         self._environ = environ
-        self._data = data
+        self._config = config if share else pickle.loads(pickle.dumps(config))
         self._namespace = namespace if namespace != __missing__ else "MAIN"
         self._prefix = prefix.upper() if prefix != __missing__ else ""
         self._reload = None
-        self._cache_data = dict()
+        self._cache = dict()
         self._cache_path = self._environ.get_data_path(f"{self._environ.name}.cfg", create_parent=True)
         self.load_cache()
 
     @property
     def reload(self) -> bool:
         """
         是否重新加载配置
@@ -318,57 +320,57 @@
         last_error = __missing__
         try:
             env_key = f"{self._prefix}{key}"
             if env_key in os.environ:
                 value = os.environ.get(env_key)
                 return self.cast(value, type=type)
 
-            if key in self._cache_data:
-                value = self._cache_data.get(key)
-                prop = self._data.get(key, None)
+            if key in self._cache:
+                value = self._cache.get(key)
+                prop = self._config.get(key, None)
                 if self.reload:
                     if isinstance(prop, ConfigProperty) and prop.reloadable:
                         with self.__lock__:
-                            value = self._cache_data[key] = prop.load(self, key, type=type, cache=value)
+                            value = self._cache[key] = prop.load(self, key, type=type, cache=value)
                             return value
                     if isinstance(default, ConfigProperty) and default.reloadable:
                         with self.__lock__:
-                            value = self._cache_data[key] = default.load(self, key, type=type, cache=value)
+                            value = self._cache[key] = default.load(self, key, type=type, cache=value)
                             return value
                 return self.cast(value, type=type)
 
-            if key in self._data:
-                value = self._data.get(key)
+            if key in self._config:
+                value = self._config.get(key)
                 if isinstance(value, ConfigProperty):
                     with self.__lock__:
-                        value = self._cache_data[key] = value.load(self, key, type=type)
+                        value = self._cache[key] = value.load(self, key, type=type)
                         return value
                 return self.cast(value, type=type)
 
         except Exception as e:
             last_error = e
 
         if default == __missing__:
             if last_error != __missing__:
                 raise last_error
             raise ConfigError(f"Not found environment variable \"{self._prefix}{key}\" or config \"{key}\"")
 
         if isinstance(default, ConfigProperty):
             with self.__lock__:
-                value = self._cache_data[key] = default.load(self, key, type=type)
+                value = self._cache[key] = default.load(self, key, type=type)
             return value
 
         return default
 
     def keys(self) -> Generator[str, None, None]:
         """
         遍历配置名，默认不遍历内置配置
         """
-        keys = set(self._data.keys())
-        keys.update(self._cache_data.keys())
+        keys = set(self._config.keys())
+        keys.update(self._cache.keys())
         for key in os.environ.keys():
             if key.startswith(self._prefix):
                 keys.add(key[len(self._prefix):])
         for key in sorted(keys):
             yield key
 
     def items(self) -> Generator[Tuple[str, Any], None, None]:
@@ -378,45 +380,45 @@
         for key in self.keys():
             yield key, self.get(key)
 
     def set(self, key: str, value: Any) -> None:
         """
         更新配置
         """
-        self._data[key] = value
+        self._config[key] = value
 
     def set_default(self, key: str, value: Any) -> Any:
         """
         设置默认配置
         """
-        return self._data.setdefault(key, value)
+        return self._config.setdefault(key, value)
 
     def update(self, **kwargs) -> None:
         """
         更新配置
         """
-        self._data.update(**kwargs)
+        self._config.update(**kwargs)
 
     def update_defaults(self, **kwargs) -> None:
         """
         更新默认配置
         """
         for key, value in kwargs.items():
-            self._data.setdefault(key, value)
+            self._config.setdefault(key, value)
 
     def update_from_file(self, path: str, load: Callable[[IO[Any]], Mapping] = None) -> bool:
         """
         加载配置文件，按照扩展名来匹配相应的加载规则
         """
         if load is not None:
-            return self._data.update_from_file(path, load=load)
+            return self._config.update_from_file(path, load=load)
         if path.endswith(".py"):
-            return self._data.update_from_pyfile(path)
+            return self._config.update_from_pyfile(path)
         elif path.endswith(".json"):
-            return self._data.update_from_file(path, load=json.load)
+            return self._config.update_from_file(path, load=json.load)
         self._environ.logger.debug(f"Unsupported config file: {path}")
         return False
 
     def update_from_dir(self, path: str, recursion: bool = False) -> bool:
         """
         加载配置文件目录，按照扩展名来匹配相应的加载规则
         """
@@ -448,45 +450,45 @@
 
     def load_cache(self) -> None:
         """
         从缓存中加载配置
         """
         parser = ConfigCacheParser(self)
         with self.__lock__:
-            self._cache_data.clear()
-            self._cache_data.update(parser.items())
+            self._cache.clear()
+            self._cache.update(parser.items())
 
     def save_cache(self, **kwargs: Any) -> None:
         """
         保存配置到缓存
         :param kwargs: 需要保存的配置
         """
         parser = ConfigCacheParser(self)
         with self.__lock__:
             for key, value in kwargs.items():
-                self._cache_data[key] = value
+                self._cache[key] = value
                 parser.set(key, self.cast(value, type=str))
         parser.dump()
 
     def remove_cache(self, *keys: str) -> None:
         """
         删除缓存
         :param keys: 需要删除的缓存键
         """
         parser = ConfigCacheParser(self)
         with self.__lock__:
             for key in keys:
-                self._cache_data.pop(key, None)
+                self._cache.pop(key, None)
                 parser.remove(key)
         parser.dump()
 
     def __contains__(self, key) -> bool:
         return f"{self._prefix}{key}" in os.environ or \
-            key in self._data or \
-            key in self._cache_data
+            key in self._config or \
+            key in self._cache
 
     def __getitem__(self, key: str) -> Any:
         return self.get(key)
 
     def __setitem__(self, key: str, value: Any):
         self.set(key, value)
 
@@ -652,11 +654,12 @@
             self,
             config: "Config",
             namespace: str = __missing__,
             prefix: str = __missing__,
     ):
         super().__init__(
             config._environ,
-            config._data,
+            config._config,
             namespace=namespace if namespace != __missing__ else config._namespace,
-            prefix=prefix if prefix != __missing__ else config._prefix
+            prefix=prefix if prefix != __missing__ else config._prefix,
+            share=True
         )
```

### Comparing `linktools-0.8.6/src/linktools/_environ.py` & `linktools-0.8.6rc0/src/linktools/_environ.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,16 +28,17 @@
 """
 import abc
 import json
 import logging
 import os
 import pathlib
 import shutil
+import sys
 import time
-from typing import TYPE_CHECKING, TypeVar, Type, Any
+from typing import TYPE_CHECKING, TypeVar, Type, Any, Dict
 
 from . import utils, metadata
 from .decorator import cached_property, cached_classproperty
 
 if TYPE_CHECKING:
     from ._config import ConfigDict, Config
     from ._tools import Tools, Tool
@@ -92,15 +93,15 @@
         return utils.get_machine()
 
     @property
     def debug(self) -> bool:
         """
         debug模式
         """
-        return self.get_config("DEBUG", type=bool)
+        return self.get_config("DEBUG", type=bool, default=False)
 
     @debug.setter
     def debug(self, value: bool) -> None:
         """
         debug模式
         """
         self.set_config("DEBUG", value)
@@ -243,26 +244,39 @@
     def get_logger(self, name: str = None) -> logging.Logger:
         """
         获取模块名作为前缀的logger
         """
         name = f"{self.name}.{name}" if name else self.name
         return self._log_manager.getLogger(name)
 
+    @cached_classproperty
+    def _default_config(self) -> "ConfigDict":
+        from ._config import ConfigDict
+
+        config = ConfigDict()
+
+        config.update({
+            "TOOL_SHELL": {
+                "absolute_path": utils.get_shell_path(),
+            },
+            "TOOL_PYTHON": {
+                "absolute_path": sys.executable,
+            }
+        })
+
+        return config
+
     def _create_config(self) -> "Config":
-        from ._config import Config, ConfigDict
+        from ._config import Config
 
         return Config(
             self,
-            ConfigDict(
-                DEBUG=False,
-                SHOW_LOG_LEVEL=True,
-                SHOW_LOG_TIME=False,
-            ),
+            self._default_config,
             namespace="MAIN",
-            prefix=f"{self.name.upper()}_"
+            prefix=f"{self.name.upper()}_",
         )
 
     @cached_property
     def config(self) -> "Config":
         """
         环境相关配置
         """
@@ -299,31 +313,41 @@
 
     def _create_tools(self) -> "Tools":
         from ._tools import Tools
         from ._config import ConfigDict
 
         config = ConfigDict()
 
-        template_path = environ.get_path("template", "tools.yml")
-        data_path = environ.get_data_path("tools", "tools.json")
-        asset_path = environ.get_asset_path("tools.json")
-
-        if os.path.exists(data_path):
-            config.update_from_file(data_path, json.load)
-        elif metadata.__release__ or not os.path.exists(template_path):
-            config.update_from_file(asset_path, json.load)
+        yaml_path = environ.get_path("template", "tools.yml")
+        if metadata.__release__ or not os.path.exists(yaml_path):
+            config.update_from_file(
+                environ.get_asset_path("tools.json"),
+                json.load
+            )
         else:
             import yaml
-            config.update_from_file(template_path, yaml.safe_load)
+            config.update_from_file(
+                yaml_path,
+                yaml.safe_load
+            )
 
         tools = Tools(self, config)
 
-        os.environ["PATH"] = os.pathsep.join(
-            tools.env_path + os.environ["PATH"].split(os.pathsep)
-        )
+        # set environment variable
+        index = 0
+        dir_names = os.environ["PATH"].split(os.pathsep)
+        for tool in Tools(self, config):
+            if tool.executable:
+                # dirname(executable[0]) -> environ["PATH"]
+                dir_name = tool.dirname
+                if dir_name and dir_name not in dir_names:
+                    # insert to head
+                    dir_names.insert(index, tool.dirname)
+                    index += 1
+        os.environ["PATH"] = os.pathsep.join(dir_names)
 
         return tools
 
     @cached_property
     def tools(self) -> "Tools":
         """
         工具集
@@ -367,26 +391,32 @@
     def description(self) -> str:
         return metadata.__description__
 
     @cached_property
     def root_path(self) -> str:
         return os.path.dirname(__file__)
 
-    def get_asset_path(self, *paths: str) -> str:
-        return self.get_path("assets", *paths)
-
     def _create_config(self):
         config = super()._create_config()
 
         # 初始化下载相关参数
         config.set(
             "DEFAULT_USER_AGENT",
             "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) "
             "AppleWebKit/537.36 (KHTML, like Gecko) "
             "Chrome/123.0.0.0 "
             "Safari/537.36"
         )
 
+        # 导入configs文件夹中所有配置文件
+        config.update_from_file(
+            self.get_asset_path("android-tools.json"),
+            load=json.load
+        )
+
         return config
 
+    def get_asset_path(self, *paths: str) -> str:
+        return self.get_path("assets", *paths)
+
 
 environ = Environ()
```

### Comparing `linktools-0.8.6/src/linktools/_tools.py` & `linktools-0.8.6rc0/src/linktools/_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -475,23 +475,38 @@
 
     def __init__(self, environ: "BaseEnviron", config: Dict[str, Dict]):
         self.environ = environ
         self.logger = environ.get_logger("tools")
         self.config = environ.wrap_config(prefix="")
         self.all = self._parse_items(config)
 
-    @property
-    def env_path(self) -> List[str]:
-        paths = []
-        for tool in self:
-            if tool.executable:
-                path = tool.dirname
-                if path and path not in paths:
-                    paths.append(path)
-        return paths
+    def _parse_items(self, config: Dict[str, Dict]) -> Dict[str, Tool]:
+        result = {
+            "shell": Tool(self, "shell", {
+                "cmdline": None,
+                "absolute_path": utils.get_shell_path(),
+            }),
+            "python": Tool(self, "python", {
+                "cmdline": None,
+                "absolute_path": sys.executable,
+            }),
+        }
+
+        for key, value in config.items():
+            if not isinstance(value, dict):
+                warnings.warn(f"dict was expected, got {type(value)}, ignored.")
+                continue
+            name = value.get("name", None)
+            if name is None:
+                if key.startswith("TOOL_"):
+                    key = key[len("TOOL_"):]
+                name = value["name"] = key.lower()
+            result[name] = Tool(self, name, value)
+
+        return result
 
     def keys(self) -> Generator[str, None, None]:
         for k, v in self.all.items():
             if v.supported:
                 yield k
 
     def values(self) -> Generator[Tool, None, None]:
@@ -518,32 +533,7 @@
         return tool
 
     def __getattr__(self, item: str) -> Tool:
         return self[item]
 
     def __setitem__(self, key: str, value: Tool):
         self.all[key] = value
-
-    def _parse_items(self, config: Dict[str, Dict]) -> Dict[str, Tool]:
-        result = {
-            "shell": Tool(self, "shell", {
-                "cmdline": None,
-                "absolute_path": utils.get_shell_path(),
-            }),
-            "python": Tool(self, "python", {
-                "cmdline": None,
-                "absolute_path": sys.executable,
-            }),
-        }
-
-        for key, value in config.items():
-            if not isinstance(value, dict):
-                warnings.warn(f"dict was expected, got {type(value)}, ignored.")
-                continue
-            name = value.get("name", None)
-            if name is None:
-                if key.startswith("TOOL_"):
-                    key = key[len("TOOL_"):]
-                name = value["name"] = key.lower()
-            result[name] = Tool(self, name, value)
-
-        return result
```

### Comparing `linktools-0.8.6/src/linktools/_url.py` & `linktools-0.8.6rc0/src/linktools/_url.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/android/__init__.py` & `linktools-0.8.6rc0/src/linktools/android/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/android/adb.py` & `linktools-0.8.6rc0/src/linktools/android/adb.py`

 * *Files 2% similar despite different names*

```diff
@@ -412,30 +412,28 @@
         :return: 是否存在
         """
         args = ["[", "-a", path, "]", "&&", "echo", "-n", "1"]
         out = self.shell(*args, **kwargs)
         return utils.bool(utils.int(out, default=0), default=False)
 
     @cached_classproperty
-    def _agent_info(self) -> dict:
-        agent_path = environ.get_asset_path("android-tools.json")
-        agent_data = json.loads(utils.read_file(agent_path, text=True))
-        agent_info = agent_data["ANDROID_TOOL_BRIDGE_APK"]
+    def agent_info(self) -> dict:
+        agent_info = environ.get_config("ANDROID_TOOL_BRIDGE_APK", type=dict)
         agent_info["start_flag"] = f"__start_flag_{agent_info['md5']}__"
         agent_info["end_flag"] = f"__end_flag_{agent_info['md5']}__"
         return agent_info
 
     @cached_property
-    def _agent_path(self) -> str:
+    def agent_path(self) -> str:
         """
         初始化agent
         :return: agent路径
         """
-        apk_name = self._agent_info["name"]
-        apk_md5 = self._agent_info["md5"]
+        apk_name = self.agent_info["name"]
+        apk_md5 = self.agent_info["md5"]
 
         apk_path = environ.get_asset_path(apk_name)
         target_dir = self.get_storage_path("apk", apk_md5)
         target_path = self.get_storage_path("apk", apk_md5, apk_name)
 
         # check apk path
         if not self.is_file_exist(target_path):
@@ -449,21 +447,21 @@
     def make_agent_args(self, *args: [str], flag: bool = False) -> [str]:
         """
         生成agent参数
         :param args: 参数
         :param flag: 是否添加flag
         :return: 参数列表
         """
-        agent_info = self._agent_info
+        agent_info = self.agent_info
         start_flag = agent_info["start_flag"]
         end_flag = agent_info["end_flag"]
         main_class = agent_info["main"]
 
         agent_args = [
-            "CLASSPATH=%s" % self._agent_path,
+            "CLASSPATH=%s" % self.agent_path,
             "app_process", "/", main_class,
         ]
 
         if flag:
             agent_args.extend([
                 "--start-flag", start_flag,
                 "--end-flag", end_flag
@@ -476,15 +474,15 @@
     @utils.timeoutable
     def call_agent(self, *args: [str], **kwargs) -> str:
         """
         调用辅助apk功能
         :param args: 参数
         :return: 输出结果
         """
-        agent_info = self._agent_info
+        agent_info = self.agent_info
         start_flag = agent_info["start_flag"]
         end_flag = agent_info["end_flag"]
 
         # call apk
         result = self.shell(
             *self.make_agent_args(*args, flag=True),
             **kwargs
```

### Comparing `linktools-0.8.6/src/linktools/android/struct.py` & `linktools-0.8.6rc0/src/linktools/android/struct.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/assets/containers/100-nginx/Dockerfile` & `linktools-0.8.6rc0/src/linktools/assets/containers/100-nginx/Dockerfile`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/assets/containers/100-nginx/container.py` & `linktools-0.8.6rc0/src/linktools/assets/containers/100-nginx/container.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/assets/containers/100-nginx/dnsapi.txt` & `linktools-0.8.6rc0/src/linktools/assets/containers/100-nginx/dnsapi.txt`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/assets/containers/110-portainer/container.py` & `linktools-0.8.6rc0/src/linktools/assets/containers/110-portainer/container.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/assets/containers/120-flare/compose.yml` & `linktools-0.8.6rc0/src/linktools/assets/containers/120-flare/compose.yml`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/assets/containers/120-flare/container.py` & `linktools-0.8.6rc0/src/linktools/assets/containers/120-flare/container.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/assets/containers/120-flare/nginx.conf` & `linktools-0.8.6rc0/src/linktools/assets/containers/120-flare/nginx.conf`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/assets/fake_useragent.json` & `linktools-0.8.6rc0/src/linktools/assets/fake_useragent.json`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/assets/frida.js` & `linktools-0.8.6rc0/src/linktools/assets/frida.js`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/assets/frida.min.js` & `linktools-0.8.6rc0/src/linktools/assets/frida.min.js`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/assets/objection/plugins/__init__.py` & `linktools-0.8.6rc0/src/linktools/assets/objection/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/assets/tools.json` & `linktools-0.8.6rc0/src/linktools/assets/tools.json`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/cli/__init__.py` & `linktools-0.8.6rc0/src/linktools/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/cli/argparse.py` & `linktools-0.8.6rc0/src/linktools/cli/argparse.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/cli/command.py` & `linktools-0.8.6rc0/src/linktools/cli/command.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/cli/commands/android/adb.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/android/adb.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/cli/commands/android/agent.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/android/agent.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/cli/commands/android/app.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/android/app.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/cli/commands/android/debug.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/android/debug.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/cli/commands/android/frida.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/android/frida.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/cli/commands/android/info.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/android/info.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/cli/commands/android/intent.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/android/intent.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/cli/commands/android/objection.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/android/objection.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/cli/commands/android/pidcat.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/android/pidcat.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/cli/commands/android/top.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/android/top.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/cli/commands/common/cert.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/common/cert.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/cli/commands/common/cntr.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/common/cntr.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/cli/commands/common/env.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/common/env.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/cli/commands/common/grep.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/common/grep.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/cli/commands/common/tools.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/common/tools.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/cli/commands/ios/frida.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/ios/frida.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/cli/commands/ios/ipa.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/ios/ipa.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/cli/commands/ios/objection.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/ios/objection.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/cli/commands/ios/scp.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/ios/scp.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/cli/commands/ios/sib.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/ios/sib.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/cli/commands/ios/ssh.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/ios/ssh.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/cli/device.py` & `linktools-0.8.6rc0/src/linktools/cli/device.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/container/__init__.py` & `linktools-0.8.6rc0/src/linktools/container/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/container/container.py` & `linktools-0.8.6rc0/src/linktools/container/container.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/container/manager.py` & `linktools-0.8.6rc0/src/linktools/container/manager.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/container/repository.py` & `linktools-0.8.6rc0/src/linktools/container/repository.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/decorator.py` & `linktools-0.8.6rc0/src/linktools/decorator.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/device.py` & `linktools-0.8.6rc0/src/linktools/device.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/frida/__init__.py` & `linktools-0.8.6rc0/src/linktools/frida/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/frida/android.py` & `linktools-0.8.6rc0/src/linktools/frida/android.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,27 +4,25 @@
 # Author    : HuJi <jihu.hj@alibaba-inc.com>
 # Datetime  : 2022/2/25 6:45 PM
 # User      : huji
 # Product   : PyCharm
 # Project   : link
 
 import fnmatch
-import json
 import lzma
 import os
 import shutil
-from typing import Optional, Dict, List
+from typing import Optional, Dict
 
 import frida
 
 from .server import FridaServer
 from .. import environ, utils
 from .._url import DownloadHttpError
 from ..android import Device
-from ..decorator import cached_classproperty
 from ..reactor import Stoppable
 
 _logger = environ.get_logger("frida.server.android")
 
 
 class AndroidFridaServer(FridaServer):
     """
@@ -94,25 +92,19 @@
                         self._device.sudo("kill", "-9", process.pid, ignore_errors=True)
         finally:
             # 把转发端口给移除了，不然会一直占用这个端口
             if self._forward is not None:
                 self._forward.stop()
                 self._forward = None
 
-    @cached_classproperty
-    def _server_info(self) -> "List[Dict[str, str]]":
-        server_path = environ.get_asset_path("android-frida.json")
-        server_data = json.loads(utils.read_file(server_path, text=True))
-        return server_data["ANDROID_TOOL_FRIDA_SERVER"]
-
     @classmethod
     def _get_executables(cls, abi: str, version: str):
         result = []
-        for config in cls._server_info:
-            config = dict(config)
+        configs = environ.get_config("ANDROID_TOOL_FRIDA_SERVER", type=list)
+        for config in configs:
             config.update(version=version, abi=abi)
             min_version = config.get("min_version", "0.0.0")
             max_version = config.get("max_version", "99999.0.0")
             if utils.parse_version(min_version) <= utils.parse_version(version) <= utils.parse_version(max_version):
                 result.append(cls.Executable(config))
         return result
```

### Comparing `linktools-0.8.6/src/linktools/frida/app.py` & `linktools-0.8.6rc0/src/linktools/frida/app.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/frida/ios.py` & `linktools-0.8.6rc0/src/linktools/frida/ios.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/frida/script.py` & `linktools-0.8.6rc0/src/linktools/frida/script.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/frida/server.py` & `linktools-0.8.6rc0/src/linktools/frida/server.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/ida/__init__.py` & `linktools-0.8.6rc0/src/linktools/ida/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/ida/ida.py` & `linktools-0.8.6rc0/src/linktools/ida/ida.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/ios/ipa.py` & `linktools-0.8.6rc0/src/linktools/ios/ipa.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/ios/sib.py` & `linktools-0.8.6rc0/src/linktools/ios/sib.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/ios/struct.py` & `linktools-0.8.6rc0/src/linktools/ios/struct.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/metadata.py` & `linktools-0.8.6rc0/src/linktools/metadata.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,16 +32,16 @@
     __eq__ = lambda l, r: \
         l is r or type(l) is type(r)
     __repr__ = lambda _: "__missing__"
 
 
 __name__ = "linktools"
 __release__ = True
-__version__ = "0.8.6"
+__version__ = "0.8.6rc0"
 __missing__ = __MissingType()
 __description__ = f"""\
     ___       __   __              __
    / (_)___  / /__/ /_____  ____  / /____
-  / / / __ \\/ //_/ __/ __ \\/ __ \\/ / ___/  linktools toolkit (v0.8.6)
+  / / / __ \\/ //_/ __/ __ \\/ __ \\/ / ___/  linktools toolkit (v0.8.6rc0)
  / / / / / / ,< / /_/ /_/ / /_/ / (__  )   by: Hu Ji <669898595@qq.com>
 /_/_/_/ /_/_/|_|\\__/\\____/\\____/_/____/
 """
```

### Comparing `linktools-0.8.6/src/linktools/reactor.py` & `linktools-0.8.6rc0/src/linktools/reactor.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/references/fake_useragent/fake.py` & `linktools-0.8.6rc0/src/linktools/references/fake_useragent/fake.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/references/fake_useragent/utils.py` & `linktools-0.8.6rc0/src/linktools/references/fake_useragent/utils.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/rich.py` & `linktools-0.8.6rc0/src/linktools/rich.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,16 +53,16 @@
 
 
 class LogHandler(RichHandler):
 
     def __init__(self, environ: "BaseEnviron"):
         super().__init__(
             show_path=False,
-            show_level=environ.get_config("SHOW_LOG_LEVEL", type=bool),
-            show_time=environ.get_config("SHOW_LOG_TIME", type=bool),
+            show_level=environ.get_config("SHOW_LOG_LEVEL", type=bool, default=True),
+            show_time=environ.get_config("SHOW_LOG_TIME", type=bool, default=False),
             omit_repeated_times=False,
             log_time_format=self.make_time_text
             # markup=True,
             # highlighter=NullHighlighter()
         )
 
         self._styles = {
```

### Comparing `linktools-0.8.6/src/linktools/ssh.py` & `linktools-0.8.6rc0/src/linktools/ssh.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/utils/__init__.py` & `linktools-0.8.6rc0/src/linktools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/utils/_port.py` & `linktools-0.8.6rc0/src/linktools/utils/_port.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/utils/_proxy.py` & `linktools-0.8.6rc0/src/linktools/utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/utils/_subprocess.py` & `linktools-0.8.6rc0/src/linktools/utils/_subprocess.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools/utils/_utils.py` & `linktools-0.8.6rc0/src/linktools/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools.egg-info/PKG-INFO` & `linktools-0.8.6rc0/src/linktools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linktools
-Version: 0.8.6
+Version: 0.8.6rc0
 Summary: linktools toolkit
 Author-email: Hu Ji <669898595@qq.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/ice-black-tea/linktools
 Project-URL: Repository, https://github.com/ice-black-tea/linktools.git
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `linktools-0.8.6/src/linktools.egg-info/SOURCES.txt` & `linktools-0.8.6rc0/src/linktools.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 src/linktools.egg-info/dependency_links.txt
 src/linktools.egg-info/entry_points.txt
 src/linktools.egg-info/requires.txt
 src/linktools.egg-info/top_level.txt
 src/linktools/android/__init__.py
 src/linktools/android/adb.py
 src/linktools/android/struct.py
-src/linktools/assets/android-frida.json
 src/linktools/assets/android-tools.apk
 src/linktools/assets/android-tools.json
+src/linktools/assets/chrome-driver.json
 src/linktools/assets/fake_useragent.json
 src/linktools/assets/frida.js
 src/linktools/assets/frida.min.js
 src/linktools/assets/tools.json
 src/linktools/assets/containers/100-nginx/Dockerfile
 src/linktools/assets/containers/100-nginx/compose.yml
 src/linktools/assets/containers/100-nginx/container.py
```

### Comparing `linktools-0.8.6/src/linktools.egg-info/entry_points.txt` & `linktools-0.8.6rc0/src/linktools.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `linktools-0.8.6/src/linktools.egg-info/requires.txt` & `linktools-0.8.6rc0/src/linktools.egg-info/requires.txt`

 * *Files identical despite different names*

