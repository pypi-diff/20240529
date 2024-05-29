# Comparing `tmp/carthage-0.32.tar.gz` & `tmp/carthage-0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carthage-0.32.tar", last modified: Mon Apr 15 21:08:26 2024, max compression
+gzip compressed data, was "carthage-0.33.tar", last modified: Wed May 29 14:02:06 2024, max compression
```

## Comparing `carthage-0.32.tar` & `carthage-0.33.tar`

### file list

```diff
@@ -1,232 +1,234 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.754113 carthage-0.32/
--rw-r--r--   0 runner    (1001) docker     (127)    42976 2024-04-15 21:08:21.000000 carthage-0.32/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-15 21:08:21.000000 carthage-0.32/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-15 21:08:26.754113 carthage-0.32/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-15 21:08:21.000000 carthage-0.32/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.726113 carthage-0.32/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1248 2024-04-15 21:08:21.000000 carthage-0.32/bin/btrfs-rmrf
--rwxr-xr-x   0 runner    (1001) docker     (127)     2758 2024-04-15 21:08:21.000000 carthage-0.32/bin/carthage
--rwxr-xr-x   0 runner    (1001) docker     (127)     1109 2024-04-15 21:08:21.000000 carthage-0.32/bin/carthage-console
--rwxr-xr-x   0 runner    (1001) docker     (127)     8449 2024-04-15 21:08:21.000000 carthage-0.32/bin/carthage-runner
--rwxr-xr-x   0 runner    (1001) docker     (127)     2359 2024-04-15 21:08:21.000000 carthage-0.32/bin/carthage-vault-tool
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.730113 carthage-0.32/carthage/
--rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-04-15 21:08:21.000000 carthage-0.32/carthage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28784 2024-04-15 21:08:21.000000 carthage-0.32/carthage/ansible.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-15 21:08:21.000000 carthage-0.32/carthage/become_privileged.py
--rw-r--r--   0 runner    (1001) docker     (127)     9396 2024-04-15 21:08:21.000000 carthage-0.32/carthage/carthage_deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-15 21:08:21.000000 carthage-0.32/carthage/carthage_plugin.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7461 2024-04-15 21:08:21.000000 carthage-0.32/carthage/cloud_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.734113 carthage-0.32/carthage/config/
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-15 21:08:21.000000 carthage-0.32/carthage/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-15 21:08:21.000000 carthage-0.32/carthage/config/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-04-15 21:08:21.000000 carthage-0.32/carthage/config/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     8720 2024-04-15 21:08:21.000000 carthage-0.32/carthage/config/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-15 21:08:21.000000 carthage-0.32/carthage/config/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-04-15 21:08:21.000000 carthage-0.32/carthage/console.py
--rw-r--r--   0 runner    (1001) docker     (127)    13899 2024-04-15 21:08:21.000000 carthage-0.32/carthage/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-04-15 21:08:21.000000 carthage-0.32/carthage/debian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.734113 carthage-0.32/carthage/dependency_injection/
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-15 21:08:21.000000 carthage-0.32/carthage/dependency_injection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    68732 2024-04-15 21:08:21.000000 carthage-0.32/carthage/dependency_injection/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13754 2024-04-15 21:08:21.000000 carthage-0.32/carthage/dependency_injection/introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)    37395 2024-04-15 21:08:21.000000 carthage-0.32/carthage/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-04-15 21:08:21.000000 carthage-0.32/carthage/deployment_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     8247 2024-04-15 21:08:21.000000 carthage-0.32/carthage/dns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.734113 carthage-0.32/carthage/entanglement/
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-15 21:08:21.000000 carthage-0.32/carthage/entanglement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10564 2024-04-15 21:08:21.000000 carthage-0.32/carthage/entanglement/instrumentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-15 21:08:21.000000 carthage-0.32/carthage/entanglement/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-04-15 21:08:21.000000 carthage-0.32/carthage/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.734113 carthage-0.32/carthage/extra_packages/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-15 21:08:21.000000 carthage-0.32/carthage/extra_packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-15 21:08:21.000000 carthage-0.32/carthage/extra_packages/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-04-15 21:08:21.000000 carthage-0.32/carthage/extra_packages/repo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.734113 carthage-0.32/carthage/extra_packages/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-15 21:08:21.000000 carthage-0.32/carthage/extra_packages/resources/reprepro_distributions
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-15 21:08:21.000000 carthage-0.32/carthage/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    22296 2024-04-15 21:08:21.000000 carthage-0.32/carthage/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    18480 2024-04-15 21:08:21.000000 carthage-0.32/carthage/kvstore.py
--rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-04-15 21:08:21.000000 carthage-0.32/carthage/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    42053 2024-04-15 21:08:21.000000 carthage-0.32/carthage/machine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.738113 carthage-0.32/carthage/modeling/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-15 21:08:21.000000 carthage-0.32/carthage/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-15 21:08:21.000000 carthage-0.32/carthage/modeling/ansible.py
--rw-r--r--   0 runner    (1001) docker     (127)    25507 2024-04-15 21:08:21.000000 carthage-0.32/carthage/modeling/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15601 2024-04-15 21:08:21.000000 carthage-0.32/carthage/modeling/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-15 21:08:21.000000 carthage-0.32/carthage/modeling/example.py
--rw-r--r--   0 runner    (1001) docker     (127)    33276 2024-04-15 21:08:21.000000 carthage-0.32/carthage/modeling/implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-04-15 21:08:21.000000 carthage-0.32/carthage/modeling/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.738113 carthage-0.32/carthage/network/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-15 21:08:21.000000 carthage-0.32/carthage/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44037 2024-04-15 21:08:21.000000 carthage-0.32/carthage/network/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-04-15 21:08:21.000000 carthage-0.32/carthage/network/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-15 21:08:21.000000 carthage-0.32/carthage/network/links.py
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-04-15 21:08:21.000000 carthage-0.32/carthage/network/mac.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-15 21:08:21.000000 carthage-0.32/carthage/network/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-15 21:08:21.000000 carthage-0.32/carthage/network/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-04-15 21:08:21.000000 carthage-0.32/carthage/oci.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-15 21:08:21.000000 carthage-0.32/carthage/pki.py
--rw-r--r--   0 runner    (1001) docker     (127)    10742 2024-04-15 21:08:21.000000 carthage-0.32/carthage/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.738113 carthage-0.32/carthage/podman/
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-15 21:08:21.000000 carthage-0.32/carthage/podman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33518 2024-04-15 21:08:21.000000 carthage-0.32/carthage/podman/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-15 21:08:21.000000 carthage-0.32/carthage/podman/carthage_plugin.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-04-15 21:08:21.000000 carthage-0.32/carthage/podman/modeling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-15 21:08:21.000000 carthage-0.32/carthage/ports.py
--rw-r--r--   0 runner    (1001) docker     (127)     7452 2024-04-15 21:08:21.000000 carthage-0.32/carthage/pytest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-04-15 21:08:21.000000 carthage-0.32/carthage/pytest_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.738113 carthage-0.32/carthage/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/80-net-setup-link.rules
--rwxr-xr-x   0 runner    (1001) docker     (127)      658 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/ansible-chroot-helper
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.722113 carthage-0.32/carthage/resources/fai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.738113 carthage-0.32/carthage/resources/fai/class/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/class/DEFAULT.var
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.738113 carthage-0.32/carthage/resources/fai/debconf/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/debconf/IPMI
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/debconf/SERIAL
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.738113 carthage-0.32/carthage/resources/fai/disk_config/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/disk_config/DEFAULT
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/disk_config/LVM
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.718113 carthage-0.32/carthage/resources/fai/files/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.722113 carthage-0.32/carthage/resources/fai/files/etc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.718113 carthage-0.32/carthage/resources/fai/files/etc/cloud/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.718113 carthage-0.32/carthage/resources/fai/files/etc/cloud/cloud.cfg.d/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.738113 carthage-0.32/carthage/resources/fai/files/etc/cloud/cloud.cfg.d/20_use_netplan.cfg/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/files/etc/cloud/cloud.cfg.d/20_use_netplan.cfg/CLOUD_INIT
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.742113 carthage-0.32/carthage/resources/fai/files/etc/cloud/ds-identify.cfg/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/files/etc/cloud/ds-identify.cfg/CLOUD_INIT
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.722113 carthage-0.32/carthage/resources/fai/files/etc/pam.d/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.742113 carthage-0.32/carthage/resources/fai/files/etc/pam.d/su/
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/files/etc/pam.d/su/OPENROOT
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.742113 carthage-0.32/carthage/resources/fai/files/etc/resolv.conf/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/files/etc/resolv.conf/DEFAULT
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.742113 carthage-0.32/carthage/resources/fai/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)       76 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/hooks/extrbase.CONTAINER2VM
--rwxr-xr-x   0 runner    (1001) docker     (127)       72 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/hooks/repository.DEFAULT
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.742113 carthage-0.32/carthage/resources/fai/package_config/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/package_config/CLOUD_INIT
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/package_config/DEFAULT
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/package_config/GROW
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/package_config/IPMI
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/package_config/LVM
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.722113 carthage-0.32/carthage/resources/fai/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.742113 carthage-0.32/carthage/resources/fai/scripts/CLOUD_INIT/
--rwxr-xr-x   0 runner    (1001) docker     (127)      251 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/scripts/CLOUD_INIT/10-setup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.742113 carthage-0.32/carthage/resources/fai/scripts/GRUB_EFI/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2208 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/scripts/GRUB_EFI/10-setup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.742113 carthage-0.32/carthage/resources/fai/scripts/OPENROOT/
--rwxr-xr-x   0 runner    (1001) docker     (127)       37 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/scripts/OPENROOT/10-setup
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/scripts/OPENROOT/20-setup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.742113 carthage-0.32/carthage/resources/fai/scripts/SERIAL/
--rwxr-xr-x   0 runner    (1001) docker     (127)       90 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/scripts/SERIAL/20-SERIAL
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/hadron-xorg-modes
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/runner_console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.746113 carthage-0.32/carthage/resources/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/bond-netdev.mako
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/bond-network.mako
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/bridge-netdev.mako
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/bridge-network.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/default-network.mako
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/gre-netdev.mako
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/gre-network.mako
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/network-base.mako
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/physical-link.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.746113 carthage-0.32/carthage/resources/templates/skeletons/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.746113 carthage-0.32/carthage/resources/templates/skeletons/layout/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/skeletons/layout/carthage_plugin.py.mako
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/skeletons/layout/carthage_plugin.yml.mako
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/skeletons/layout/layout.py.mako
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/skeletons/prototype.mako
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/vlan-netdev.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/vlan-network.mako
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/vm-config.mako
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/vm-console.mako
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/xfrm-netdev.mako
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/test_ansible.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-15 21:08:21.000000 carthage-0.32/carthage/runner_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    33781 2024-04-15 21:08:21.000000 carthage-0.32/carthage/setup_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-15 21:08:21.000000 carthage-0.32/carthage/sh.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-15 21:08:21.000000 carthage-0.32/carthage/skeleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     8886 2024-04-15 21:08:21.000000 carthage-0.32/carthage/sonic.py
--rw-r--r--   0 runner    (1001) docker     (127)    10924 2024-04-15 21:08:21.000000 carthage-0.32/carthage/ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-15 21:08:21.000000 carthage-0.32/carthage/system_dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-04-15 21:08:21.000000 carthage-0.32/carthage/systemd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-15 21:08:21.000000 carthage-0.32/carthage/tb_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-04-15 21:08:21.000000 carthage-0.32/carthage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.746113 carthage-0.32/carthage/vault/
--rw-r--r--   0 runner    (1001) docker     (127)     9201 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vault/carthage_plugin.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11757 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.750113 carthage-0.32/carthage/vmware/
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/carthage_plugin.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/config_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/convenience.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/datacenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/datastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    11979 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17559 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/vm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.754113 carthage-0.32/carthage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-15 21:08:26.000000 carthage-0.32/carthage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-15 21:08:26.000000 carthage-0.32/carthage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 21:08:26.000000 carthage-0.32/carthage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-15 21:08:26.000000 carthage-0.32/carthage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 21:08:26.000000 carthage-0.32/carthage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-15 21:08:21.000000 carthage-0.32/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 21:08:26.754113 carthage-0.32/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.754113 carthage-0.32/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-15 21:08:21.000000 carthage-0.32/tests/carthage_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-15 21:08:21.000000 carthage-0.32/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-15 21:08:21.000000 carthage-0.32/tests/inner_conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-15 21:08:21.000000 carthage-0.32/tests/inner_plugin_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-15 21:08:21.000000 carthage-0.32/tests/machine_mock.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-15 21:08:21.000000 carthage-0.32/tests/override-config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.754113 carthage-0.32/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-15 21:08:21.000000 carthage-0.32/tests/resources/base_test.tar.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.754113 carthage-0.32/tests/resources/dynamic_container/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-15 21:08:21.000000 carthage-0.32/tests/resources/dynamic_container/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 21:08:21.000000 carthage-0.32/tests/resources/inventory.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-15 21:08:21.000000 carthage-0.32/tests/resources/local_playbook.yml
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-15 21:08:21.000000 carthage-0.32/tests/resources/test_ansible.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.722113 carthage-0.32/tests/resources/test_ansible_role/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.754113 carthage-0.32/tests/resources/test_ansible_role/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-15 21:08:21.000000 carthage-0.32/tests/resources/test_ansible_role/tasks/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-15 21:08:21.000000 carthage-0.32/tests/resources/test_playbook.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.754113 carthage-0.32/tests/resources/true_container/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 21:08:21.000000 carthage-0.32/tests/resources/true_container/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-15 21:08:21.000000 carthage-0.32/tests/template-2.expected
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.754113 carthage-0.32/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-15 21:08:21.000000 carthage-0.32/tests/templates/template-2.mako
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-15 21:08:21.000000 carthage-0.32/tests/templates/test.mako
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-15 21:08:21.000000 carthage-0.32/tests/templates/test_hash.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_ansible.py
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_become.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_carthage_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    20584 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_dependency_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (127)    14915 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_modeling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_pki.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.754113 carthage-0.32/tests/test_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_plugin/carthage_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_plugin/carthage_plugin.yml
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)    11982 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_podman.py
--rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_setup_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_vm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_vmware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.700496 carthage-0.33/
+-rw-r--r--   0 runner    (1001) docker     (127)    42976 2024-05-29 14:02:02.000000 carthage-0.33/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-29 14:02:02.000000 carthage-0.33/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-29 14:02:06.700496 carthage-0.33/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-29 14:02:02.000000 carthage-0.33/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.672496 carthage-0.33/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1248 2024-05-29 14:02:02.000000 carthage-0.33/bin/btrfs-rmrf
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2758 2024-05-29 14:02:02.000000 carthage-0.33/bin/carthage
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1109 2024-05-29 14:02:02.000000 carthage-0.33/bin/carthage-console
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8449 2024-05-29 14:02:02.000000 carthage-0.33/bin/carthage-runner
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2359 2024-05-29 14:02:02.000000 carthage-0.33/bin/carthage-vault-tool
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.680496 carthage-0.33/carthage/
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-05-29 14:02:02.000000 carthage-0.33/carthage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29787 2024-05-29 14:02:02.000000 carthage-0.33/carthage/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-29 14:02:02.000000 carthage-0.33/carthage/become_privileged.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9396 2024-05-29 14:02:02.000000 carthage-0.33/carthage/carthage_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-29 14:02:02.000000 carthage-0.33/carthage/carthage_plugin.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-05-29 14:02:02.000000 carthage-0.33/carthage/cloud_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.680496 carthage-0.33/carthage/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-29 14:02:02.000000 carthage-0.33/carthage/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-29 14:02:02.000000 carthage-0.33/carthage/config/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-05-29 14:02:02.000000 carthage-0.33/carthage/config/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8720 2024-05-29 14:02:02.000000 carthage-0.33/carthage/config/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-05-29 14:02:02.000000 carthage-0.33/carthage/config/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-05-29 14:02:02.000000 carthage-0.33/carthage/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14349 2024-05-29 14:02:02.000000 carthage-0.33/carthage/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-29 14:02:02.000000 carthage-0.33/carthage/debian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.680496 carthage-0.33/carthage/dependency_injection/
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-29 14:02:02.000000 carthage-0.33/carthage/dependency_injection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68933 2024-05-29 14:02:02.000000 carthage-0.33/carthage/dependency_injection/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15045 2024-05-29 14:02:02.000000 carthage-0.33/carthage/dependency_injection/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37902 2024-05-29 14:02:02.000000 carthage-0.33/carthage/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-29 14:02:02.000000 carthage-0.33/carthage/deployment_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8271 2024-05-29 14:02:02.000000 carthage-0.33/carthage/dns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.680496 carthage-0.33/carthage/entanglement/
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-29 14:02:02.000000 carthage-0.33/carthage/entanglement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10564 2024-05-29 14:02:02.000000 carthage-0.33/carthage/entanglement/instrumentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-29 14:02:02.000000 carthage-0.33/carthage/entanglement/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-05-29 14:02:02.000000 carthage-0.33/carthage/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.680496 carthage-0.33/carthage/extra_packages/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-29 14:02:02.000000 carthage-0.33/carthage/extra_packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-29 14:02:02.000000 carthage-0.33/carthage/extra_packages/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-05-29 14:02:02.000000 carthage-0.33/carthage/extra_packages/repo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.680496 carthage-0.33/carthage/extra_packages/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-29 14:02:02.000000 carthage-0.33/carthage/extra_packages/resources/reprepro_distributions
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-05-29 14:02:02.000000 carthage-0.33/carthage/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22296 2024-05-29 14:02:02.000000 carthage-0.33/carthage/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18480 2024-05-29 14:02:02.000000 carthage-0.33/carthage/kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-05-29 14:02:02.000000 carthage-0.33/carthage/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43123 2024-05-29 14:02:02.000000 carthage-0.33/carthage/machine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.684496 carthage-0.33/carthage/modeling/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-29 14:02:02.000000 carthage-0.33/carthage/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-29 14:02:02.000000 carthage-0.33/carthage/modeling/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25507 2024-05-29 14:02:02.000000 carthage-0.33/carthage/modeling/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15600 2024-05-29 14:02:02.000000 carthage-0.33/carthage/modeling/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-29 14:02:02.000000 carthage-0.33/carthage/modeling/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33806 2024-05-29 14:02:02.000000 carthage-0.33/carthage/modeling/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-29 14:02:02.000000 carthage-0.33/carthage/modeling/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.684496 carthage-0.33/carthage/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-29 14:02:02.000000 carthage-0.33/carthage/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44077 2024-05-29 14:02:02.000000 carthage-0.33/carthage/network/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-05-29 14:02:02.000000 carthage-0.33/carthage/network/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-29 14:02:02.000000 carthage-0.33/carthage/network/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-05-29 14:02:02.000000 carthage-0.33/carthage/network/mac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-29 14:02:02.000000 carthage-0.33/carthage/network/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-29 14:02:02.000000 carthage-0.33/carthage/network/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-05-29 14:02:02.000000 carthage-0.33/carthage/oci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-29 14:02:02.000000 carthage-0.33/carthage/pki.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11770 2024-05-29 14:02:02.000000 carthage-0.33/carthage/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.684496 carthage-0.33/carthage/podman/
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-29 14:02:02.000000 carthage-0.33/carthage/podman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36379 2024-05-29 14:02:02.000000 carthage-0.33/carthage/podman/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-29 14:02:02.000000 carthage-0.33/carthage/podman/carthage_plugin.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    14984 2024-05-29 14:02:02.000000 carthage-0.33/carthage/podman/container_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8251 2024-05-29 14:02:02.000000 carthage-0.33/carthage/podman/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-29 14:02:02.000000 carthage-0.33/carthage/ports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7452 2024-05-29 14:02:02.000000 carthage-0.33/carthage/pytest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-29 14:02:02.000000 carthage-0.33/carthage/pytest_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.684496 carthage-0.33/carthage/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/80-net-setup-link.rules
+-rwxr-xr-x   0 runner    (1001) docker     (127)      658 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/ansible-chroot-helper
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.672496 carthage-0.33/carthage/resources/fai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.684496 carthage-0.33/carthage/resources/fai/class/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/fai/class/DEFAULT.var
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.684496 carthage-0.33/carthage/resources/fai/debconf/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/fai/debconf/IPMI
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/fai/debconf/SERIAL
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.688496 carthage-0.33/carthage/resources/fai/disk_config/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/fai/disk_config/DEFAULT
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/fai/disk_config/LVM
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.668496 carthage-0.33/carthage/resources/fai/files/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.668496 carthage-0.33/carthage/resources/fai/files/etc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.668496 carthage-0.33/carthage/resources/fai/files/etc/cloud/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.668496 carthage-0.33/carthage/resources/fai/files/etc/cloud/cloud.cfg.d/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.688496 carthage-0.33/carthage/resources/fai/files/etc/cloud/cloud.cfg.d/20_use_netplan.cfg/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/fai/files/etc/cloud/cloud.cfg.d/20_use_netplan.cfg/CLOUD_INIT
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.688496 carthage-0.33/carthage/resources/fai/files/etc/cloud/ds-identify.cfg/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/fai/files/etc/cloud/ds-identify.cfg/CLOUD_INIT
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.668496 carthage-0.33/carthage/resources/fai/files/etc/pam.d/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.688496 carthage-0.33/carthage/resources/fai/files/etc/pam.d/su/
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/fai/files/etc/pam.d/su/OPENROOT
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.688496 carthage-0.33/carthage/resources/fai/files/etc/resolv.conf/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/fai/files/etc/resolv.conf/DEFAULT
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.688496 carthage-0.33/carthage/resources/fai/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       76 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/fai/hooks/extrbase.CONTAINER2VM
+-rwxr-xr-x   0 runner    (1001) docker     (127)       72 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/fai/hooks/repository.DEFAULT
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.688496 carthage-0.33/carthage/resources/fai/package_config/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/fai/package_config/CLOUD_INIT
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/fai/package_config/DEFAULT
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/fai/package_config/GROW
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/fai/package_config/IPMI
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/fai/package_config/LVM
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.672496 carthage-0.33/carthage/resources/fai/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.688496 carthage-0.33/carthage/resources/fai/scripts/CLOUD_INIT/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      251 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/fai/scripts/CLOUD_INIT/10-setup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.688496 carthage-0.33/carthage/resources/fai/scripts/GRUB_EFI/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2208 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/fai/scripts/GRUB_EFI/10-setup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.688496 carthage-0.33/carthage/resources/fai/scripts/OPENROOT/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       37 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/fai/scripts/OPENROOT/10-setup
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/fai/scripts/OPENROOT/20-setup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.688496 carthage-0.33/carthage/resources/fai/scripts/SERIAL/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       90 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/fai/scripts/SERIAL/20-SERIAL
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/hadron-xorg-modes
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/runner_console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.692496 carthage-0.33/carthage/resources/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/templates/bond-netdev.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/templates/bond-network.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/templates/bridge-netdev.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/templates/bridge-network.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/templates/default-network.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/templates/gre-netdev.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/templates/gre-network.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/templates/network-base.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/templates/physical-link.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.692496 carthage-0.33/carthage/resources/templates/skeletons/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.692496 carthage-0.33/carthage/resources/templates/skeletons/layout/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/templates/skeletons/layout/carthage_plugin.py.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/templates/skeletons/layout/carthage_plugin.yml.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/templates/skeletons/layout/layout.py.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/templates/skeletons/prototype.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/templates/vlan-netdev.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/templates/vlan-network.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/templates/vm-config.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/templates/vm-console.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/templates/xfrm-netdev.mako
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-29 14:02:02.000000 carthage-0.33/carthage/resources/test_ansible.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-29 14:02:02.000000 carthage-0.33/carthage/runner_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34275 2024-05-29 14:02:02.000000 carthage-0.33/carthage/setup_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-29 14:02:02.000000 carthage-0.33/carthage/sh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-29 14:02:02.000000 carthage-0.33/carthage/skeleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8886 2024-05-29 14:02:02.000000 carthage-0.33/carthage/sonic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11429 2024-05-29 14:02:02.000000 carthage-0.33/carthage/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-29 14:02:02.000000 carthage-0.33/carthage/system_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-29 14:02:02.000000 carthage-0.33/carthage/systemd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-29 14:02:02.000000 carthage-0.33/carthage/tb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-05-29 14:02:02.000000 carthage-0.33/carthage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.692496 carthage-0.33/carthage/vault/
+-rw-r--r--   0 runner    (1001) docker     (127)     9201 2024-05-29 14:02:02.000000 carthage-0.33/carthage/vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-29 14:02:02.000000 carthage-0.33/carthage/vault/carthage_plugin.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11757 2024-05-29 14:02:02.000000 carthage-0.33/carthage/vm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.696496 carthage-0.33/carthage/vmware/
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-29 14:02:02.000000 carthage-0.33/carthage/vmware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-05-29 14:02:02.000000 carthage-0.33/carthage/vmware/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-29 14:02:02.000000 carthage-0.33/carthage/vmware/carthage_plugin.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-29 14:02:02.000000 carthage-0.33/carthage/vmware/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-29 14:02:02.000000 carthage-0.33/carthage/vmware/config_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-29 14:02:02.000000 carthage-0.33/carthage/vmware/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-29 14:02:02.000000 carthage-0.33/carthage/vmware/convenience.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-29 14:02:02.000000 carthage-0.33/carthage/vmware/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-29 14:02:02.000000 carthage-0.33/carthage/vmware/datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-05-29 14:02:02.000000 carthage-0.33/carthage/vmware/datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-29 14:02:02.000000 carthage-0.33/carthage/vmware/folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-29 14:02:02.000000 carthage-0.33/carthage/vmware/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-29 14:02:02.000000 carthage-0.33/carthage/vmware/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12246 2024-05-29 14:02:02.000000 carthage-0.33/carthage/vmware/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-05-29 14:02:02.000000 carthage-0.33/carthage/vmware/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-29 14:02:02.000000 carthage-0.33/carthage/vmware/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17559 2024-05-29 14:02:02.000000 carthage-0.33/carthage/vmware/vm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.700496 carthage-0.33/carthage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-29 14:02:06.000000 carthage-0.33/carthage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-05-29 14:02:06.000000 carthage-0.33/carthage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 14:02:06.000000 carthage-0.33/carthage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-29 14:02:06.000000 carthage-0.33/carthage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 14:02:06.000000 carthage-0.33/carthage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-29 14:02:02.000000 carthage-0.33/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 14:02:06.700496 carthage-0.33/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.700496 carthage-0.33/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-29 14:02:02.000000 carthage-0.33/tests/carthage_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-29 14:02:02.000000 carthage-0.33/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-29 14:02:02.000000 carthage-0.33/tests/inner_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-29 14:02:02.000000 carthage-0.33/tests/inner_plugin_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-29 14:02:02.000000 carthage-0.33/tests/machine_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-29 14:02:02.000000 carthage-0.33/tests/override-config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-29 14:02:02.000000 carthage-0.33/tests/podman_remote_host.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.700496 carthage-0.33/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-29 14:02:02.000000 carthage-0.33/tests/resources/base_test.tar.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.700496 carthage-0.33/tests/resources/dynamic_container/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-29 14:02:02.000000 carthage-0.33/tests/resources/dynamic_container/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 14:02:02.000000 carthage-0.33/tests/resources/inventory.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-29 14:02:02.000000 carthage-0.33/tests/resources/local_playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-29 14:02:02.000000 carthage-0.33/tests/resources/test_ansible.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.672496 carthage-0.33/tests/resources/test_ansible_role/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.700496 carthage-0.33/tests/resources/test_ansible_role/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-29 14:02:02.000000 carthage-0.33/tests/resources/test_ansible_role/tasks/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-29 14:02:02.000000 carthage-0.33/tests/resources/test_playbook.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.700496 carthage-0.33/tests/resources/true_container/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-29 14:02:02.000000 carthage-0.33/tests/resources/true_container/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-29 14:02:02.000000 carthage-0.33/tests/template-2.expected
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.700496 carthage-0.33/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-29 14:02:02.000000 carthage-0.33/tests/templates/template-2.mako
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-29 14:02:02.000000 carthage-0.33/tests/templates/test.mako
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-29 14:02:02.000000 carthage-0.33/tests/templates/test_hash.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-05-29 14:02:02.000000 carthage-0.33/tests/test_ansible.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-05-29 14:02:02.000000 carthage-0.33/tests/test_become.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-29 14:02:02.000000 carthage-0.33/tests/test_carthage_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-29 14:02:02.000000 carthage-0.33/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-29 14:02:02.000000 carthage-0.33/tests/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20827 2024-05-29 14:02:02.000000 carthage-0.33/tests/test_dependency_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-05-29 14:02:02.000000 carthage-0.33/tests/test_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-29 14:02:02.000000 carthage-0.33/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-29 14:02:02.000000 carthage-0.33/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-05-29 14:02:02.000000 carthage-0.33/tests/test_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14915 2024-05-29 14:02:02.000000 carthage-0.33/tests/test_modeling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-29 14:02:02.000000 carthage-0.33/tests/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-29 14:02:02.000000 carthage-0.33/tests/test_pki.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:02:06.700496 carthage-0.33/tests/test_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-29 14:02:02.000000 carthage-0.33/tests/test_plugin/carthage_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-29 14:02:02.000000 carthage-0.33/tests/test_plugin/carthage_plugin.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-29 14:02:02.000000 carthage-0.33/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14121 2024-05-29 14:02:02.000000 carthage-0.33/tests/test_podman.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-05-29 14:02:02.000000 carthage-0.33/tests/test_setup_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-29 14:02:02.000000 carthage-0.33/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-05-29 14:02:02.000000 carthage-0.33/tests/test_vm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-29 14:02:02.000000 carthage-0.33/tests/test_vmware.py
```

### Comparing `carthage-0.32/LICENSE` & `carthage-0.33/LICENSE`

 * *Files identical despite different names*

### Comparing `carthage-0.32/PKG-INFO` & `carthage-0.33/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carthage
-Version: 0.32
+Version: 0.33
 Summary: A powerful Infrastructure as Code (IAC) framework
 Author-email: Sam Hartman <sam.hartman@hadronindustries.com>
 License: LGPL-3
 Project-URL: Homepage, https://github.com/hadron/carthage
 Project-URL: Documentation, https://carthage.readthedocs.io
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `carthage-0.32/README.rst` & `carthage-0.33/README.rst`

 * *Files identical despite different names*

### Comparing `carthage-0.32/bin/btrfs-rmrf` & `carthage-0.33/bin/btrfs-rmrf`

 * *Files identical despite different names*

### Comparing `carthage-0.32/bin/carthage` & `carthage-0.33/bin/carthage`

 * *Files identical despite different names*

### Comparing `carthage-0.32/bin/carthage-console` & `carthage-0.33/bin/carthage-console`

 * *Files identical despite different names*

### Comparing `carthage-0.32/bin/carthage-runner` & `carthage-0.33/bin/carthage-runner`

 * *Files identical despite different names*

### Comparing `carthage-0.32/bin/carthage-vault-tool` & `carthage-0.33/bin/carthage-vault-tool`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/__init__.py` & `carthage-0.33/carthage/__init__.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/ansible.py` & `carthage-0.33/carthage/ansible.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from abc import ABC, abstractmethod
 from pathlib import Path
 
 from .dependency_injection import *
 from . import sh, Machine, machine
 from .container import Container
 from .config import ConfigLayout
-from .ssh import SshKey
+from .ssh import SshKey, SshAgent
 from .utils import validate_shell_safe
 from types import SimpleNamespace
 from .network import access_ssh_origin
 from . import setup_tasks
 from .plugins import CarthagePlugin
 import logging
 
@@ -166,14 +166,20 @@
                     pass
             if 'ansible_ssh_common_args' not in var_dict:
                 try:
                     if ssh_options := m.ssh_options:
                         var_dict['ansible_ssh_common_args'] = " ".join(ssh_options)
                 except Exception:
                     pass
+            if 'ansible_user' not in var_dict:
+                try:
+                    if m.ssh_login_user != 'root':
+                        var_dict['ansible_user'] = m.ssh_login_user
+                except Exception:
+                    pass
             hosts_dict[machine_name] = var_dict
             groups = []
             for p in self.group_plugins:
                 try:
                     groups += await self.ainjector(p.groups_for, m)
                 except BaseException:
                     logger.exception(f"Error determining groups for {machine_name} from group plugin {p.name}")
@@ -482,23 +488,26 @@
                                log=log,
                                origin=dependency_quote(origin))
 
 __all__ += ['run_play']
 
 
 @inject(ssh_key=InjectionKey(SshKey, _optional=True),
+        ssh_agent=InjectionKey(SshAgent, _optional=True),
         config=ConfigLayout)
 @contextlib.contextmanager
 def write_config(config_dir, inventory,
                  *, ssh_key, log,
                  config, origin,
                  inventory_overrides,
+                 ssh_agent,
                  ansible_config):
     private_key = ""
     if ssh_key:
+        ssh_agent = ssh_key.agent
         private_key = f"private_key_file = {ssh_key.key_path}"
     if not log:
         stdout_str = "stdout_callback = json"
     else:
         stdout_str = ""
     with tempfile.TemporaryDirectory(
             dir=config_dir,
@@ -543,15 +552,15 @@
         # ssh section
         f.write('''
 [ssh_connection]
 pipelining=True
 ''')
         if origin is None or isinstance(origin, NetworkNamespaceOrigin):
             f.write(f'''\
-ssh_args = -o ControlMaster=auto -o ControlPersist=60s -oUserKnownHostsFile={config.state_dir}/ssh_known_hosts {config.global_ssh_options}
+ssh_args = -F{ssh_agent.ssh_config} -o ControlMaster=auto -o ControlPersist=60s -oUserKnownHostsFile={config.state_dir}/ssh_known_hosts {config.global_ssh_options}
 ''')
         else:
             f.write(f'''\
 ssh_args = -o ControlMaster=auto -o ControlPersist=60s -oStrictHostKeyChecking=no
 ''')
 
         f.flush()
@@ -722,7 +731,29 @@
         add_provider(ansible_log, ansible_log_for_model, allow_multiple=True)
 
     Sets up a per-model ansible log in *stamp_path*/ansible.log.
     '''
     return f'{model.stamp_path}/ansible.log'
 
 __all__ += ['ansible_log_for_model']
+
+class AnsibleIpAddressMixin(Machine):
+
+    '''Normally, ansible inventory is generated at generation time,
+    which may be before cloud services have determined the IP address
+    of machines.  This Mixin will look at ip_address at runtime to set
+
+    In a     :class:`carthage.modeling.MachineModel`, use this as follows::
+
+        class server(MachineModel):
+            machine_mixins = (AnsibleIpAddressMixin,)
+
+
+        '''
+
+    @property
+    def ansible_inventory_overrides(self):
+        return {
+            'ansible_host':self.ip_address,
+            }
+
+__all__ += ['AnsibleIpAddressMixin']
```

### Comparing `carthage-0.32/carthage/become_privileged.py` & `carthage-0.33/carthage/become_privileged.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,17 +2,21 @@
 # Carthage is free software; you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License version 3
 # as published by the Free Software Foundation. It is distributed
 # WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the file
 # LICENSE for details.
 
+import os
 import typing
+import carthage.machine
 from . import machine, sh
 from .utils import memoproperty
+from .ssh import SshAgent
+
 __all__ = []
 
 #: List of sftp-server locations
 sftp_server_locations = (
     '/usr/lib/sftp-server',
     '/usr/libexec/openssh/sftp-server',
     )
@@ -45,23 +49,45 @@
             _user = self.runas_user
         return await super().run_command(
             *self.become_privileged_command(_user),
             *args,
             _user=self.ssh_login_user)
         
     async def sshfs_process_factory(self, user):
-        if not self.become_privileged(user):
-            return await super().sshfs_process_factory(user=user)
-        sftp_command_list = self.become_privileged_command(user) + [
-            '/bin/sh', '-c',
-            f"'for sftp in {' '.join(sftp_server_locations)} ; do test -x $sftp && exec $sftp; done'"]
-        sftp_command = " ".join(sftp_command_list)
-        return sh.sshfs(
-            '-o' 'ssh_command=' + " ".join(
-                str(self.ssh).split()[:-1]),
-            '-osftp_server='+sftp_command,
-            f'{machine.ssh_user_addr(self)}:/',
-            self.sshfs_path,
-            '-f',
-            )
-
+        become_privileged_command = self.become_privileged_command(user)
+        if not become_privileged_command:
+            return await super().sshfs_process_factory(user)
+        return await sshfs_sftp_finder(
+            self,
+            become_privileged_command=become_privileged_command,
+            sshfs_path=self.sshfs_path,
+            prefix="")
+    
 __all__ += ['BecomePrivilegedMixin']
+
+async def sshfs_sftp_finder(
+        machine:                            machine.Machine,
+                            become_privileged_command: list,
+        sshfs_path: str,
+        prefix:str = ""):
+    '''Like :class:`Machine`.  Does not use the sftp subsystem,
+    but instead tries to find an sftp server.  Also, mostly for
+    podman's convenienc in running an sftp server with unshare,
+    supports a prefix argument.
+
+    :param prefix: Command inserted between the become_privileged_command and sftp invocation.  Can be used to enter the right namespace.
+
+    '''
+    agent = await machine.ainjector.get_instance_async(SshAgent)
+    sftp_command_list = become_privileged_command + [
+        '/bin/sh', '-c',
+        f"'for sftp in {' '.join(sftp_server_locations)} ; do test -x $sftp && exec {prefix} $sftp; done'"]
+    sftp_command = " ".join(sftp_command_list)
+    return sh.sshfs(
+        '-o' 'ssh_command=' + " ".join(
+                str(machine.ssh).split()[:-1]),
+        '-osftp_server='+sftp_command,
+        f'{carthage.machine.ssh_user_addr(machine)}:/',
+        sshfs_path,
+        '-f',
+        _env=agent.agent_environ)
+
```

### Comparing `carthage-0.32/carthage/carthage_deployment.py` & `carthage-0.33/carthage/carthage_deployment.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/carthage_plugin.yml` & `carthage-0.33/carthage/carthage_plugin.yml`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     pypi: pyyaml
   - deb: python3-mako
     pypi: mako
   - deb: python3-lmdb
     pypi: lmdb
   - deb: python3-netifaces
     pypi: netifaces
+  - deb: git
   - deb: socat
   - deb: systemd-container
   - deb: libvirt-clients
   - deb: fai-setup-storage
   - deb: sshfs
   - deb: bridge-utils
   - deb: qemu-utils
```

### Comparing `carthage-0.32/carthage/cloud_init.py` & `carthage-0.33/carthage/cloud_init.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021, Hadron Industries, Inc.
+# Copyright (C) 2021, 2024, Hadron Industries, Inc.
 # Carthage is free software; you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License version 3
 # as published by the Free Software Foundation. It is distributed
 # WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the file
 # LICENSE for details.
 
@@ -29,15 +29,14 @@
         'disable_root': False})
 
     network_configuration: dict = dataclasses.field(default_factory=lambda: {})
 
     __all__ += ['CloudInitConfig']
 
 
-@inject_autokwargs(model=AbstractMachineModel)
 class CloudInitPlugin(Injectable):
 
     async def apply(self, config: CloudInitConfig):
         "Apply changes to the given :class:`CloudInitConfig`.  This is typically overridden so the plugin actually does something."
         pass
 
     @classmethod
@@ -127,14 +126,15 @@
         os.rename(output_tmp, output)
 
     return output
 
 __all__ += ['generate_cloud_init_cidata']
 
 
+@inject_autokwargs(model=AbstractMachineModel)
 class NetworkPlugin(CloudInitPlugin):
 
     name = "network"
 
     async def apply(self, config: CloudInitConfig):
         ethernets = config.network_configuration.setdefault('ethernets', {})
         for l in self.model.network_links.values():
@@ -170,16 +170,18 @@
 
     async def apply(self, config: CloudInitConfig):
         authorized_keys_file = Path(self.authorized_keys.path)
         authorized_keys = list(filter(
             lambda k: k and (not k[0] == '#'),
             authorized_keys_file.read_text().split("\n")))
         config.meta_data['public_ssh_keys'] = authorized_keys
+        config.user_data['ssh_authorized_keys'] = authorized_keys
 
 
+@inject_autokwargs(model=AbstractMachineModel)
 class HostnamePlugin(CloudInitPlugin):
 
     name = "hostname"
 
     async def apply(self, config: CloudInitConfig):
         config.user_data['hostname'] = self.model.name
 
@@ -199,14 +201,23 @@
             content = f.read()
         write_files.append(dict(
             path="/root/.ssh/authorized_keys",
             content=content,
             permissions='0644',
             owner='root:root'))
 
+class DisableRootPlugin(CloudInitPlugin):
+
+    name ='disable_root'
+
+    async def apply(self, config):
+        config.user_data['disable_root'] = True
+
+__all__ += ['DisableRootPlugin']
+
 
 @inject(injector=Injector)
 def enable_cloud_init_plugins(injector):
     injector.add_provider(AuthorizedKeysPlugin, allow_multiple=True)
     injector.add_provider(NetworkPlugin, allow_multiple=True)
     injector.add_provider(HostnamePlugin, allow_multiple=True)
```

### Comparing `carthage-0.32/carthage/config/__init__.py` & `carthage-0.33/carthage/config/__init__.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/config/base.py` & `carthage-0.33/carthage/config/base.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/config/layout.py` & `carthage-0.33/carthage/config/layout.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/config/schema.py` & `carthage-0.33/carthage/config/schema.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/config/types.py` & `carthage-0.33/carthage/config/types.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/console.py` & `carthage-0.33/carthage/console.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 
 import asyncio
 import argparse
 import code
 import collections.abc
 import concurrent.futures
+import functools
 import shlex
 import re
 import time
 import pkg_resources
 import os.path
 import readline
 import rlcompleter
@@ -154,28 +155,28 @@
         for k in self.completed_keys:
             print(f'[{k}]: {self.history[k]}')
         self.completed_keys.clear()
         return super().raw_input(*args, **kwargs)
 
     def displayhook(self, obj):
 
-        def future_callback(f):
+        def future_callback(num, f):
             del self.history[num]
             try:
                 self.history[num] = f.result()
                 self.completed_keys.append(num)
             except Exception as e:
                 print(f'[{num}]-> exception')
                 traceback.print_exc()
 
         if isinstance(obj, collections.abc.Coroutine):
             self.history_num += 1
             num = self.history_num
             future = asyncio.run_coroutine_threadsafe(obj, loop=self.loop)
-            future.add_done_callback(future_callback)
+            future.add_done_callback(functools.partial(future_callback, num))
             print(f'[{num}]: async {obj.__name__}')
             self.history[num] = future
             self.loop.call_soon_threadsafe(CarthageConsole.noop)
         else:
             self.orig_displayhook(obj)
 
     async def enable_console_commands(self, ainjector):
```

### Comparing `carthage-0.32/carthage/container.py` & `carthage-0.33/carthage/container.py`

 * *Files 3% similar despite different names*

```diff
@@ -298,14 +298,26 @@
         # know if your shell commands succeed or not.
         if not self.running:
             raise RuntimeError("Container not running")
 
         return sh.nsenter.bake("-t" + self.container_leader, "-C", "-m", "-n", "-u", "-i", "-p",
                                _env=self._environment())
 
+    def run_command(self, *args, _bg=True,
+                          _bg_exc=False, _user=None,
+                          **kwargs):
+        if _user is None:
+            _user = self.runas_user
+        if _user != 'root':
+            raise NotImplementedError('Not currently supported for runas_user to be different than root')
+        if self.running:
+            return self.shell(*args, **kwargs)
+        else:
+            return self.container_command(*args, _bg=_bg, _bg_exc=_bg_exc, **kwargs)
+        
     def _environment(self, networking=False):
         env = os.environ.copy()
         env['DEBIAN_FRONTEND'] = 'noninteractive'
         if networking:
             env['SYSTEMD_NSPAWN_API_VFS_WRITABLE'] = 'network'
         return env
 
@@ -337,10 +349,9 @@
     def _apply_to_container_customization(self, customization):
         '''A method indicating that this object can have :class:`~carthage.machine.ContainerCustomizations` applied.  Provides a mechanism for adapting the customization if needed to a particular container-like machine.  Not needed for this class.
         '''
         return
 
     def _apply_to_filesystem_customization(self, customization):
         customization.path = self.volume.path
-        customization.run_command = self.container_command
 
 __all__ = ['container_volume', 'container_image', 'Container']
```

### Comparing `carthage-0.32/carthage/debian.py` & `carthage-0.33/carthage/debian.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/dependency_injection/__init__.py` & `carthage-0.33/carthage/dependency_injection/__init__.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/dependency_injection/base.py` & `carthage-0.33/carthage/dependency_injection/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -918,14 +918,17 @@
 
     def __new__(cls, target_, *, require_type=False, **constraints):
         assert (cls is InjectionKey) or set(constraints) - \
             cls.POSSIBLE_PARAMETERS, "You cannot subclass InjectionKey with empty constraints"
         if require_type and not isinstance(target_, type):
             raise TypeError(
                 'Only types can be used as implicit injection keys; if this is intended then construct the injection key explicitly')
+        for k in constraints:
+            if k.startswith('_') and k not in cls.POSSIBLE_PARAMETERS:
+                raise TypeError(f'{k} is not an InjectionKey parameter')
         if isinstance(target_, InjectionKey):
             # mostly so you can take an existing injection key and mark it optional
             new_constraints = dict(target_.constraints)
             new_constraints.update(constraints)
             constraints = new_constraints
             target_ = target_.target
         if (not constraints):
@@ -974,15 +977,15 @@
     def __eq__(self, other):
         if not isinstance(other, type(self)):
             return False
         if self.target != other.target:
             return False
         if len(self.constraints) != len(other.constraints):
             return False
-        if all(map(lambda k: self.constraints[k] == other.constraints[k], self.constraints.keys())):
+        if all(map(lambda k: k in other.constraints and self.constraints[k] == other.constraints[k], self.constraints.keys())):
             return True
         return False
 
     def supplementary_injection_keys(self, p):
         if (isinstance(p, type) and issubclass(p, Injectable)) or \
            isinstance(p, Injectable):
             yield from p.supplementary_injection_keys(self)
```

### Comparing `carthage-0.32/carthage/dependency_injection/introspection.py` & `carthage-0.33/carthage/dependency_injection/introspection.py`

 * *Files 4% similar despite different names*

```diff
@@ -190,15 +190,26 @@
     def __enter__(self):
         for ctx in self.provider.instantiation_contexts:
             # We only care about the first one
             assert not self.dependencies_waiting
             self.dependencies_waiting = ctx.dependencies_waiting
             break
         self.provider.instantiation_contexts.add(self)
-        return super().__enter__()
+        res =  super().__enter__()
+        loop_detect = set()
+        cur = self
+        while cur:
+            try:
+                loop_tuple = cur.key, cur.injector, cur.key.ready is False
+                if loop_tuple in loop_detect:
+                    raise RuntimeError('injection loop detected: '+repr(self))
+                loop_detect.add(loop_tuple)
+            except AttributeError: pass
+            cur = cur.parent
+        return res
 
     @property
     def description(self):
         desc = f'Instantiating {self.key} using {self.injector}'
         if self.injector is not self.triggering_injector:
             desc += f' for {self.triggering_injector}'
         return desc
@@ -389,8 +400,33 @@
             visit(get_dependencies_for(inner_val, dependency.injector), inner_val, cycle=cycle|{inner_val})
             
     visit(get_dependencies_for(obj, injector),
           obj, {obj})
 
 __all__ += ['calculate_reverse_dependencies']
 
+def instantiation_leaves():
+    '''Start from :data:`instantiation_roots` and chase down all the
+    dependencies.  Return all contexts that do not have any
+    dependencies waiting that have not already been seen.
+    '''
+    to_consider = list(instantiation_roots)
+    ids_seen = set()
+    leaves = set()
+    while to_consider:
+        to_consider_next = set()
+        for context in to_consider:
+            has_dependencies = False
+            ids_seen.add(id(context))
+            for dependency in context.dependencies_waiting.values():
+                if id(dependency) in ids_seen:
+                    continue
+                to_consider_next.add(dependency)
+                has_dependencies = True
+            if not has_dependencies:
+                leaves.add(context)
+        to_consider = to_consider_next
+    return leaves
+
+__all__ += ['instantiation_leaves']
+
 from . import base
```

### Comparing `carthage-0.32/carthage/deployment.py` & `carthage-0.33/carthage/deployment.py`

 * *Files 1% similar despite different names*

```diff
@@ -559,87 +559,96 @@
     await do_recurse(stop_at=ainjector)
     if futures:
         await asyncio.gather(*futures)
     return results
 
 __all__ += ['find_deployables']
 
-async def find_deployable(deployable: Deployable):
+async def find_deployable(deployable: Deployable, required:bool = False):
     '''
     Ideally, :meth:`Deployable.find` would return non-falsy if an object exists and falsy if it does not exist.  Unfortunately, some of the Carthage plugins do not follow this pattern.  This method:
 
     * Returns whatever find returns if it is non-falsy (I.E. objects exists)
 
     * Returns true if find returns falsy (typically None) and *deployable.mob* exists and is not None
 
     * Returns False otherwise
 
+    :param required: if true, raise if the object is not found
     '''
     result = await deployable.find()
     if bool(result): return result
     try:
         if deployable.mob is not None: return True
     except AttributeError: pass
+    if required:
+        raise LookupError(f'Failed to find {deployable}')
     return False
 
 __all__ += ['find_deployable']
 
 @inject(ainjector=AsyncInjector)
 async def find_orphan_deployables(
         deployables:list[Deployable] = None,
         *,
         ainjector):
     '''Find any orphans in a set of Deployables. An orphan is a
     deployable that used to be deployed by a layout, but is no longer
     deployed.
-    Not all :class:`DeploymentFinders` are able to find orphans, so some orphaned objects might not be recognized.
+    Not all :class:`DeployableFinders` are able to find orphans, so some orphaned objects might not be recognized.
 
     :param deployments: If slpecified, this should be the result of :func:`find_deployments` with recurse set to True. If None, then find_deployments will be called with recursive and readonly set to True.
 
     '''
     if deployables is None:
         deployables = await ainjector(find_deployables, readonly=True, recurse=True)
     else:
         deployables = list(deployables)
-    #handle dynamic_dependencies
-    dynamic_dependencies: list[Deployable] = []
-    this_round = deployables
-    while this_round:
-        for d in this_round:
-            if not hasattr(d, 'dynamic_dependencies'):
-                continue
-            with instantiation_not_ready():
-                for dynamic in await d.dynamic_dependencies():
-                    if isinstance(dynamic, InjectionKey):
-                        dynamic = await d.ainjector.get_instance_async(dynamic)
-                    dynamic_dependencies.append(dynamic)
-        this_round = []
-        for d in dynamic_dependencies:
-            if d not in deployables:
-                if not is_obj_ready(d):
-                    d.readonly = DryRun
-                deployables.append(d)
-                this_round.append(d)
-    deployables = [ d for d in deployables
-                    if await ainjector(find_deployable, d)]
-    res = ainjector.filter_instantiate(DeployableFinder, ['name'])
-    finders = [x[1] for x in res]
-    orphans = []
-    for finder in finders:
-        orphans.extend(await ainjector(finder.find_orphans, deployables))
-        for d in orphans:
-            d.readonly = DryRun
-    async def orphan_filter(o):
-        if await ainjector(find_deployable, o):
-            return True
-        else:
-            logger.debug(f'{o} is not an orphan because it does not exist')
-            return False
-    orphans =  [o for o in orphans if await orphan_filter(o)]
-    return orphans
+    try:
+        #handle dynamic_dependencies
+        dynamic_dependencies: list[Deployable] = []
+        set_as_readonly:list[Deployable] = []
+        this_round = deployables
+        while this_round:
+            for d in this_round:
+                if not hasattr(d, 'dynamic_dependencies'):
+                    continue
+                with instantiation_not_ready():
+                    for dynamic in await d.dynamic_dependencies():
+                        if isinstance(dynamic, InjectionKey):
+                            dynamic = await d.ainjector.get_instance_async(dynamic)
+                        dynamic_dependencies.append(dynamic)
+            this_round = []
+            for d in dynamic_dependencies:
+                if d not in deployables:
+                    if not d.readonly and not is_obj_ready(d):
+                        d.readonly = DryRun
+                        set_as_readonly.append(d)
+                    deployables.append(d)
+                    this_round.append(d)
+        deployables = [ d for d in deployables
+                        if await ainjector(find_deployable, d)]
+        res = ainjector.filter_instantiate(DeployableFinder, ['name'])
+        finders = [x[1] for x in res]
+        orphans = []
+        for finder in finders:
+            orphans.extend(await ainjector(finder.find_orphans, deployables))
+            for d in orphans:
+                d.readonly = DryRun
+        async def orphan_filter(o):
+            if await ainjector(find_deployable, o):
+                return True
+            else:
+                logger.debug(f'{o} is not an orphan because it does not exist')
+                return False
+        orphans =  [o for o in orphans if await orphan_filter(o)]
+        return orphans
+    finally:
+        for d in set_as_readonly:
+            d.readonly = False
 
 __all__ += ['find_orphan_deployables']
 
 def clear_dry_run_marker(deployables):
     for d in deployables:
         if d.readonly is DryRun:
             d.readonly = False
```

### Comparing `carthage-0.32/carthage/deployment_commands.py` & `carthage-0.33/carthage/deployment_commands.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/dns.py` & `carthage-0.33/carthage/dns.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,14 +175,15 @@
             public_name="www.foo.com", public_records=[('CNAME', 'foo.com')])
 
     '''
     if public_name:
         public_head, sep, public_domain = public_name.partition('.')
         public_zone = await ainjector.get_instance_async(InjectionKey(DnsZone, name=public_domain, addressing='public', _optional=True))
     else: public_zone = None
+    private_zone = None
     if private_name:
         private_head, sep, private_domain = private_name.partition('.')
         private_zone = await ainjector.get_instance_async(InjectionKey(DnsZone, name=private_domain, addressing='private', _optional=True))
         if  (not private_zone):
             private_zone = await ainjector.get_instance_async(InjectionKey(DnsZone, name=private_domain, _optional=True))
     futures = []
     if public_records and public_zone:
```

### Comparing `carthage-0.32/carthage/entanglement/__init__.py` & `carthage-0.33/carthage/entanglement/__init__.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/entanglement/instrumentation.py` & `carthage-0.33/carthage/entanglement/instrumentation.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/entanglement/server.py` & `carthage-0.33/carthage/entanglement/server.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/event.py` & `carthage-0.33/carthage/event.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/extra_packages/plugin.py` & `carthage-0.33/carthage/extra_packages/plugin.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/extra_packages/repo.py` & `carthage-0.33/carthage/extra_packages/repo.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/files.py` & `carthage-0.33/carthage/files.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,25 +95,27 @@
         path = injector(repo_path)
         return path.exists()
     checkout_repo.repo_path = repo_path
     return checkout_repo
 
 
 @inject(injector=Injector)
-def checkout_git_repo(url, repo, *, foreground=False, injector):
+def checkout_git_repo(url, repo, *, injector, foreground=False, branch=None):
     if foreground:
         options = dict(_fg=True)
     else: options = dict(_bg=True, _bg_exc=False)
     config = injector(ConfigLayout)
     path = Path(config.checkout_dir) / repo
     os.makedirs(config.checkout_dir, exist_ok=True)
     if path.exists():
         return sh.git("pull", "--rebase",
                       _cwd=path,
                       **options)
     else:
+        branchargs = ['--branch', branch] if branch else []
         return sh.git("clone",
                       url, str(path),
+                      *branchargs,
                       **options)
 
 
 __all__ += ['git_checkout_task', 'checkout_git_repo']
```

### Comparing `carthage-0.32/carthage/image.py` & `carthage-0.33/carthage/image.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/kvstore.py` & `carthage-0.33/carthage/kvstore.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/local.py` & `carthage-0.33/carthage/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-# Copyright (C) 2021, 2022, 2023, Hadron Industries, Inc.
+# Copyright (C) 2021, 2022, 2023, 2024, Hadron Industries, Inc.
 # Carthage is free software; you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License version 3
 # as published by the Free Software Foundation. It is distributed
 # WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the file
 # LICENSE for details.
 
 import contextlib
 from ipaddress import IPv4Address
 from pathlib import Path
+import os
 from .machine import Machine
 from .dependency_injection import *
 from . import sh
 from .utils import memoproperty, when_needed
 from .setup_tasks import SetupTaskMixin
 from .network import NetworkLink, BridgeNetwork, match_link
 
@@ -24,15 +25,22 @@
 When testing whether a :class:`Machine` is local, test for ``isinstance(machine, LocalMachineMixin)``
 
     '''
 
     ip_address = "127.0.0.1"
 
     @contextlib.asynccontextmanager
-    async def filesystem_access(self):
+    async def filesystem_access(self, user=None):
+        if user is None:
+            user = self.runas_user
+        if user != os.getlogin():
+            async with super().filesystem_access(user=user) as path:
+                yield path
+                return
+            
         yield Path("/")
 
     async def stop_machine(self):
         raise NotImplementedError("Stopping localhost may be more dramatic than desired")
 
     @property
     def shell(self):
```

### Comparing `carthage-0.32/carthage/machine.py` & `carthage-0.33/carthage/machine.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,16 +109,20 @@
             return self.model.ssh_options + jump_host_options
         return jump_host_options
 
     @memoproperty
     def ssh_jump_host(self):
         '''
         An :class:`SshMixin` or string to use as a jump host.
+        Also supports a :class:`AbstractMachineModel` with a :attr:`machine` attribute.
         '''
-        return self.injector.get_instance(InjectionKey(ssh_jump_host, _ready=False, _optional=True))
+        jump_host =  self.injector.get_instance(InjectionKey(ssh_jump_host, _ready=False, _optional=True))
+        if isinstance(jump_host, AbstractMachineModel) and hasattr(jump_host, 'machine'):
+            jump_host = jump_host.machine
+        return jump_host
 
     @memoproperty
     def ssh_login_user(self):
         '''
         The ssh user to log in as. Defaults to root, can be set either on the machine or the model.
         '''
         try:
@@ -168,16 +172,16 @@
             if ssh_key.key_path:
                 key_options = ("-i", ssh_key.key_path,)
             else:
                 key_options = ('',)
         else:
             ssh_agent = self.injector.get_instance(carthage.ssh.SshAgent)
             key_options = tuple()
-        options = self.ssh_options + ('-oUserKnownHostsFile=' +
-                                      os.path.join(self.config_layout.state_dir, 'ssh_known_hosts'),)
+        options = self.ssh_options + ('-F' +
+                                      str(ssh_agent.ssh_config),)
         if ssh_origin_container is not None:
             ip_address = self.ip_address
             ssh_origin_container.done_future().add_done_callback(self.ssh_recompute)
             return self.injector(access_ssh_origin).bake(
                 "/usr/bin/ssh",
                 *key_options,
                 *options,
@@ -212,19 +216,21 @@
         '''
         return RsyncPath(self, p)
 
     #: The command run remotely by :meth:`ssh_online`
     ssh_online_command = 'date'
 
     async def ssh_online(self):
-        logger.debug(f'Waiting for {self.name} to be ssh_online')
         online = False
         last_error = None
         await self.ainjector.get_instance_async(InjectionKey(carthage.ssh.SshKey, _optional=True)) #Instantiate in case it is async
         await self.ainjector.get_instance_async(carthage.ssh.SshAgent)
+        if self.ssh_jump_host:
+            await self.ssh_jump_host.ssh_online()
+        logger.debug(f'Waiting for {self.name} to be ssh_online')
         for i in range(self.ssh_online_retries):
             try:
                 await self.ssh(self.ssh_online_command,
                                _bg=True, _bg_exc=False,
                                _timeout=self.ssh_online_timeout)
             except (sh.TimeoutException, sh.ErrorReturnCode) as e:
                 last_error = e
@@ -232,15 +238,19 @@
                 continue
             online = True
             last_error = None
             self._ssh_online_required = False
             logger.debug(f'{self.name} is ssh_online')
             break
         if not online:
-            raise TimeoutError("{} not online".format(self.ip_address)) from last_error
+            if isinstance(last_error, sh.TimeoutException):
+                raise TimeoutError("{} not online".format(self._address)) from last_error
+            else:
+                raise TimeoutError(f'{self.ip_address} not online: {last_error}') from last_error
+            
 
     def ssh_recompute(self, *args):
         try:
             del self.__dict__['ssh']
         except KeyError:
             pass
         self._ssh_online_required = True
@@ -591,15 +601,14 @@
         return await meth()
 
     def _apply_to_filesystem_customization(self, customization):
         '''
         Adapts the customization to this type of machine.  Overridden in machines that can customize a filesystem without booting.
         '''
         customization.customization_context = customization._machine_context()
-        customization.run_command = self.run_command
 
     def run_command(self,
                         *args,
                         _bg=True,
                         _bg_exc=False,
                     _user=None):
         '''
@@ -612,30 +621,33 @@
 This handles quoting and  makes sure each argument is a separate argument on the eventual shell;
 it works like :meth:`carthage.container.Container.container_command` and is used to give a consistent interface by :meth:`run_command`.
 '''
         if _user is None:
             _user = self.runas_user
         if _user != self.ssh_login_user:
             raise ValueError(f'{self.__class__.__qualname__} Does not support runas_user different than ssh_login_user; consider BecomePrivilegedMixin or another privilege management solution.')
+        args = [str(a) if isinstance(a,Path) else a for a in args]
         return self.ssh(
             shlex.join(args),
             _bg=_bg, _bg_exc=_bg_exc)
 
         
     async def sshfs_process_factory(self, user):
         if user != self.ssh_login_user:
             raise ValueError(f'{self.__class__.__qualname__} cannot set up filesystem access when runas_user != ssh_login_user')
+        agent = await self.ainjector.get_instance_async(SshAgent)
         return sh.sshfs(
             '-o' 'ssh_command=' + " ".join(
                 str(self.ssh).split()[:-1]),
             f'{ssh_user_addr(self)}:/',
             self.sshfs_path,
             '-f',
             _bg=True,
-            _bg_exc=False)
+            _bg_exc=False,
+            _env = agent.agent_environ)
 
     @contextlib.asynccontextmanager
     async def filesystem_access(self, user=None):
 
         '''
         An asynchronous context manager that makes the filesystem of the *Machine* available on a local path.
 
@@ -689,16 +701,21 @@
                     with contextlib.suppress(OSError):
                         os.rmdir(dir)
 
 
 @inject_autokwargs(config_layout=ConfigLayout)
 class BaseCustomization(SetupTaskMixin, AsyncInjectable):
 
+    runas_user = None #: The user to run as
+
     def __init__(self, apply_to: Machine,
                  stamp=None, **kwargs):
+        # Copy in the runas_user before replacing the customization with a machine
+        if self.runas_user is None:
+            self.runas_user = apply_to.runas_user
         if isinstance(apply_to, BaseCustomization):
             apply_to = apply_to.host
         self.host = apply_to
         if not getattr(self, 'description', None):
             self.description = self.__class__.__name__
         self.stamp_stem = stamp or self.__class__.__name__
         super().__init__(**kwargs)
@@ -754,29 +771,36 @@
 
     async def apply(self):
         ''' Run setup tasks against host'''
         return await self.ainjector(self.run_setup_tasks, context=self.customization_context)
 
     def __getattr__(self, a):
         if a in ('ssh', 'ip_address', 'start_machine', 'stop_machine',
-                 "filesystem_access",
+                 'filesystem_access',
                  'model',
                  'name', 'ansible_inventory_name',
                  'machine_running', 'running',
                  'name', 'full_name',
                  'apply_customization'):
             return getattr(self.host, a)
         raise AttributeError(f"'{self!r}' has no attribute '{a}'")
 
     def __repr__(self):
         return f"<{self.__class__.__name__} description:\"{self.description}\" for {self.host.name}>"
 
     #: A description of the customization for inclusion in task logging
     description = ""
 
+    def run_command(self, *args, _user=None, **kwargs):
+        if _user is None:
+            _user = self.runas_user
+            return self.host.run_command(
+                *args, _user=_user,
+                **kwargs)
+        
 
 class MachineCustomization(BaseCustomization):
 
     '''A customization class for running customizations on running machines.'''
 
     @property
     def customization_context(self):
@@ -813,15 +837,15 @@
 
     def __init__(self, apply_to, **kwargs):
         super().__init__(apply_to, **kwargs)
         self.host._apply_to_filesystem_customization(self)
 
     @contextlib.asynccontextmanager
     async def _machine_context(self):
-        async with self.host.machine_running(), self.host.filesystem_access() as path:
+        async with self.host.machine_running(), self.host.filesystem_access(user=self.runas_user) as path:
             self.path = path
             yield
             return
 
 
 class CustomizationInspectorProxy:
 
@@ -904,15 +928,15 @@
     '''
     return CustomizationWrapper(customization=c,
                                 order=order,
                                 before=before)
 
 
 @inject_autokwargs(ssh_key=InjectionKey(SshKey, _ready=True))
-class BareMetalMachine(Machine, SetupTaskMixin):
+class BareMetalMachine(Machine, SetupTaskMixin, AsyncInjectable):
 
     '''Represents physical hardware that Carthage cannot start or stop
     '''
 
     running = False
 
     async def start_machine(self):
```

### Comparing `carthage-0.32/carthage/modeling/__init__.py` & `carthage-0.33/carthage/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/modeling/ansible.py` & `carthage-0.33/carthage/modeling/ansible.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/modeling/base.py` & `carthage-0.33/carthage/modeling/base.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/modeling/decorators.py` & `carthage-0.33/carthage/modeling/decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,15 +282,15 @@
     '''Indicate a set of keys that should be propagated up
     in a container::
 
         class foo(ModelingContainer):
             @propagate_key(InjectionKey(Baz, target = 42))
             class ourbaz(Baz): ...
 
-    When *foo* is included ain a container, then the *Baz* injection
+    When *foo* is included in a container, then the *Baz* injection
     key will be propagated up to dependencies provided by that
     container.  Since the key was not marked globally unique,
     constraints from *foo.our_key()* will be added to it as it is
     propagated.
 
     *keys* are also provided by the contained class as if :func:`provides` or :func:`globally_unique` were called.
```

### Comparing `carthage-0.32/carthage/modeling/example.py` & `carthage-0.33/carthage/modeling/example.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/modeling/implementation.py` & `carthage-0.33/carthage/modeling/implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021, 2022, 2023, Hadron Industries, Inc.
+# Copyright (C) 2021, 2022, 2023, 2024, Hadron Industries, Inc.
 # Carthage is free software; you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License version 3
 # as published by the Free Software Foundation. It is distributed
 # WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the file
 # LICENSE for details.
 
@@ -119,42 +119,14 @@
                 v = functools.partial(v,  cls, self)
             self.initial[k] = v
         self.parent_context = thread_local.current_context
         self.context_imported = False
         self.to_inject = dict()
 
 
-    def keys_for(self, name, state):
-        # returns key, (value, options)
-        def val(k):
-            value = state.value
-            if state.flags & NSFlags.dependency_quote:
-                return dependency_quote(value)
-            else:
-                return value
-
-        options = state.injection_options
-        state.extra_keys.sort(key=lambda k:k.globally_unique, reverse=True)
-        if state.flags & NSFlags.inject_by_name:
-            name_key = InjectionKey(name)
-            # If name_key is in extra_keys, use that, so we avoid
-            # differing in _globally_unique or _ready
-            if name_key not in state.extra_keys:
-                yield InjectionKey(name), (val(InjectionKey(name)), options)
-        if isinstance(state.value, type) and (state.flags & NSFlags.inject_by_class):
-            for b in state.value.__mro__:
-                if b in self.classes_to_inject:
-                    try:
-                        class_key = state.value.default_class_injection_key()
-                    except AttributeError:
-                        class_key = InjectionKey(b)
-                    class_key = InjectionKey(b, **class_key.constraints)
-                    yield class_key, (val(class_key), options)
-        for k in state.extra_keys:
-            yield k, (val(k), options)
 
     def __getitem__(self, k):
         # Normally when we set an item we drop it from initial
         # but there are some cases where we want a value for getitem different than the value that ends up in the eventual class
         # the obvious case is injector_access from the instantiate flag.
         # so initial actually takes precidence over our actual values.
         try:
@@ -202,15 +174,15 @@
                 pass
         if k.startswith('_'):
             if k == "__qualname__":
                 self.import_context()
             return state.value
         transclusion_keys = None
         if state.transclusion_key: transclusion_keys = {state.transclusion_key}
-        for k, info in self.keys_for(name=k, state=state):
+        for k, info in keys_for(name=k, state=state, classes_to_inject=self.classes_to_inject):
             self.to_inject[k] = info
             if transclusion_keys: transclusion_keys.add(k)
         if transclusion_keys:
             self.transclusions[state.transclusion_key] = frozenset(transclusion_keys)
         return state.value
 
     def __delitem__(self, k):
@@ -276,14 +248,46 @@
                 res = parent.to_inject[key][0]
                 if isinstance(res, dependency_quote):
                     res = res.value
                 return res
             parent = parent.parent_context
         raise KeyError
 
+def keys_for(name, state, classes_to_inject):
+    '''
+    Returns the set of keys for a given state item.
+    '''
+    # returns key, (value, options)
+    def val(k):
+        value = state.value
+        if state.flags & NSFlags.dependency_quote:
+            return dependency_quote(value)
+        else:
+            return value
+
+    options = state.injection_options
+    state.extra_keys.sort(key=lambda k:k.globally_unique, reverse=True)
+    if state.flags & NSFlags.inject_by_name:
+        name_key = InjectionKey(name)
+        # If name_key is in extra_keys, use that, so we avoid
+        # differing in _globally_unique or _ready
+        if name_key not in state.extra_keys:
+            yield InjectionKey(name), (val(InjectionKey(name)), options)
+    if isinstance(state.value, type) and (state.flags & NSFlags.inject_by_class):
+        for b in state.value.__mro__:
+            if b in classes_to_inject:
+                try:
+                    class_key = state.value.default_class_injection_key()
+                except AttributeError:
+                    class_key = InjectionKey(b)
+                class_key = InjectionKey(b, **class_key.constraints)
+                yield class_key, (val(class_key), options)
+    for k in state.extra_keys:
+        yield k, (val(k), options)
+
 def check_already_provided(metaclass_proxy, v):
     if not hasattr(metaclass_proxy, '__namespace__'):
         return None
     namespace = metaclass_proxy.__namespace__
     for k in getattr(v, '__provides_dependencies_for__', []):
         try:
             namespace.get_injected(k)
@@ -564,15 +568,15 @@
                 if set(outer_constraints) & set(k_inner.constraints):
                     return
                 k_new = InjectionKey(k_inner.target, **outer_constraints, **k_inner.constraints)
             else:
                 if not do_global: return
                 k_new = k_inner  # globally unique
             # Must be after we have chosen a globally unique key if there is one.
-            if k_new not in ns.to_inject and k_inner not in inner_key_map:
+            if k_new not in to_inject and k_inner not in inner_key_map:
                 inner_key_map[k_inner] = k_new
             if isinstance(v, decorators.injector_access):
                 # Normally injector_access will not actually get a key
                 # in __initial_injections__, but there are important
                 # cases where that happens, like the machine entry on
                 # MachineModel.  In general this situation will come
                 # up if some modeling type wishes to propagate
@@ -583,57 +587,64 @@
             # by adding the outer key's constraints to
             # v.injectable_key and use that as the new injectable key,
             # preserving the inner target key.  That generally works
             # so long as the injectable_key is not masked by a key
             # already in the outer injector or by an overlapping
             # constraint.  Also, It just moves the recursion around.
             v = injector_xref(outer_key, k_inner)
-            if k_new not in ns.to_inject:
-                ns.to_inject[k_new] = (v, options)
-                ns.to_propagate.add(k_new)
+            if k_new not in to_inject:
+                to_inject[k_new] = (v, options)
+                outer_to_propagate.add(k_new)
 
         if not isinstance(state.value, ModelingContainer):
             return
         inner_key_map = {}
         val = state.value
+        if isinstance(ns, ModelingNamespace):
+            ns = ModelingNamespaceProxy(ns.cls, ns)
         outer_key = None
+        to_inject = ns.__initial_injections__
+        outer_to_propagate = ns.__container_propagations__
         to_propagate = val.__container_propagations__
         outer_keys = []
         if hasattr(val, '__provides_dependencies_for__'):
             for outer_key in sorted(
                     val.__provides_dependencies_for__,
                     key=lambda k: k.globally_unique,
                     reverse=True):
-                if outer_key not in ns.to_propagate: continue
+                if outer_key not in outer_to_propagate: continue
                 if  len(outer_key.constraints) > 0:
                     outer_keys.append(outer_key)
         if to_propagate and not outer_keys:
             warnings.warn("Cannot propagate because no outer key with constraints found", stacklevel=3)
             return
         for k_inner in to_propagate:
             if k_inner not in val.__initial_injections__:
                 warnings.warn(f'Cannot propagate {k_inner} because it is not provided by {val}')
                 continue
             v, options = val.__initial_injections__[k_inner]
             do_global = True
             for outer_key in outer_keys:
                 propagate_provider(outer_key, k_inner, v, options, do_global)
                 do_global = False
-        map_transclusions(ns.transclusions, val, inner_key_map)
+        map_transclusions(ns.__transclusions__, val, inner_key_map)
 
     def _propagate_filter(target_cls, ns, k, state):
+        if isinstance(ns, ModelingNamespace):
+            ns = ModelingNamespaceProxy(ns.cls, ns)
         if hasattr(state.value, '__container_propagation_keys__'):
             propagation_keys = set(state.value.__container_propagation_keys__)
         else: propagation_keys = set()
-        keys_for = set((x[0] for x in ns.keys_for(name=k, state=state)))
-        propagation_keys &= keys_for
+        value_keys = set((x[0] for x in keys_for(name=k, state=state, classes_to_inject=set())))
+        propagation_keys &= value_keys
         # ModelingContainers must propagate even if they have no explicit keys
         if (not propagation_keys ) and isinstance(state.value, ModelingContainer):
-            propagation_keys = keys_for
-        ns.to_propagate |= propagation_keys
+            propagation_keys = value_keys
+        if propagation_keys: 
+            ns.__container_propagations__  |= propagation_keys
         
     # propagate_filter must come before integrate_containment so that
     # integrate_containment can check whether outer_keys are in
     # ns.to_propagate. However, filters are processed in reversed
     # order.
     namespace_filters = [_integrate_containment, _propagate_filter]
 
@@ -668,49 +679,49 @@
 
     @modelmethod
     def include_container(cls, obj,
                           *, close=True,
                           allow_multiple=False,
                           dynamic_name=None,
                           **kwargs):
-        if not hasattr(cls, '__namespace__'):
-            raise TypeError('include_container can only be called within a class body')
-        ns = cls.__namespace__
+        if dynamic_name and not hasattr(cls, '__namespace__'):
+            raise TypeError('include_container can only be called within a class body if dynamic_name is used')
         def handle_function(func):
             params = set(inspect.signature(func).parameters.keys())
             open_params = params - set(kwargs.keys())
             for k in open_params:
-                if k not in ns:
+                if not hasattr(cls, k):
                     raise AttributeError(f'{k} not found in enclosing class')
-                kwargs[k] = ns[k]
+                kwargs[k] = getattr(cls, k)
             return func(**kwargs)
         if not hasattr(obj, '__provides_dependencies_for__') and callable(obj):
             obj = handle_function(obj)
         if (not hasattr(obj, '__provides_dependencies_for__')) and not dynamic_name:
             raise TypeError(f'{obj} is not a modeling container class')
         state = NsEntry(obj)
         if dynamic_name:
             # This is gross, but it's not clear how to support
             # decorators ourselves
             if (not close) or allow_multiple:
                 raise TypeError('If using dynamic_name, use decorators to adjust close and allow_multiple')
-            ns[fixup_dynamic_name(dynamic_name)] = obj
+            setattr(cls, fixup_dynamic_name(dynamic_name), obj)
             return
         # Since we're not able to use ns.__setitem__, do the injection key stuff ourself.
         if not close:
             state.flags &= ~NSFlags.close
         if allow_multiple:
             state.flags |= NSFlags.allow_multiple
+        state.flags &= ~NSFlags.inject_by_name
         state.extra_keys = obj.__provides_dependencies_for__
         options = state.injection_options
-        for k in obj.__provides_dependencies_for__:
-            if k not in ns.to_inject:
-                ns.to_inject[k] = (obj, options)
-        ModelingContainer._propagate_filter(cls, ns, obj.__name__, state)
-        ModelingContainer._integrate_containment(cls, ns, obj.__name__, state)
+        for k, _ in keys_for(name="", state=state, classes_to_inject=set()):
+            if k not in cls.__initial_injections__:
+                cls.__initial_injections__[k] = (obj, options)
+        ModelingContainer._propagate_filter(cls, cls, obj.__name__, state)
+        ModelingContainer._integrate_containment(cls, cls, obj.__name__, state)
 
 
 
 __all__ += ['ModelingContainer']
 
 
 def adjust_bases_for_tasks(bases: tuple[type], namespace: dict) -> tuple[type]:
```

### Comparing `carthage-0.32/carthage/modeling/utils.py` & `carthage-0.33/carthage/modeling/utils.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/network/__init__.py` & `carthage-0.33/carthage/network/__init__.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/network/base.py` & `carthage-0.33/carthage/network/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,14 +175,15 @@
         pool.assignment_loop(self.network_links)
         
     async def access_by(self, cls: TechnologySpecificNetwork, ready=None):
         '''Request a view of *self* using *cls* as a technology-specific lens.
 
         :return: The instance of *cls* for accessing this network
         '''
+        await self.async_become_ready()
         assert issubclass(cls, TechnologySpecificNetwork), \
             "Must request access by a subclass of TechnologySpecificNetwork"
         instance = None
         if (cls not in self.ainjector) and self.vlan_id is not None:
             try:
                 instance = await self.ainjector.get_instance_async(InjectionKey(cls, vlan_id=self.vlan_id, _ready=ready))
                 self.ainjector.add_provider(instance)
```

### Comparing `carthage-0.32/carthage/network/config.py` & `carthage-0.33/carthage/network/config.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/network/links.py` & `carthage-0.33/carthage/network/links.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/network/mac.py` & `carthage-0.33/carthage/network/mac.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/network/namespace.py` & `carthage-0.33/carthage/network/namespace.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/network/switch.py` & `carthage-0.33/carthage/network/switch.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/oci.py` & `carthage-0.33/carthage/oci.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,48 @@
-# Copyright (C)  2022, Hadron Industries, Inc.
+# Copyright (C)  2022, 2024, Hadron Industries, Inc.
 # Carthage is free software; you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License version 3
 # as published by the Free Software Foundation. It is distributed
 # WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the file
 # LICENSE for details.
 
 from __future__ import annotations
 import dataclasses
 from carthage.dependency_injection import *
 from .setup_tasks import setup_task, SetupTaskMixin
 from .utils import memoproperty
 from .config.types import ConfigPath
 import carthage.machine
+import carthage.network
 
 
 __all__ = []
 
 #: This key provides a string whose result is the container image name to pull  or an image ID that is locally available.  Examples include ``docker.io/library/debian:latest`` or ``debian:unstable``
 oci_container_image = InjectionKey('oci/container_image')
 
 __all__ += ['oci_container_image']
 
+#: If provided this NetworkConfig will be used instead of
+#InjectionKey(NetworkConfig) within containers.  That typically means
+#that after resolve_networking, the container's injector will provide
+#InjectionKey(NetworkConfig) with whatever was provided by this key.  Note that MachineModel does not respect this key.  So it will be respected when containers are used directly or for pods and pod models.
+oci_container_network_config = InjectionKey(carthage.network.NetworkConfig, role='container')
+
+__all__ += ['oci_container_network_config']
+
 
 @inject_autokwargs(
-    oci_read_only=InjectionKey('oci_read_only', _optional=NotPresent)
+    readonly=InjectionKey('oci_read_only', _optional=NotPresent)
 )
 class OciManaged(SetupTaskMixin, AsyncInjectable):
 
     #:Should this object be treated as read only
-    oci_read_only = False
+    readonly = False
 
     async def find(self):
         '''Returns falsy if the object does not exist.  Ideally returns the creation time in unix time, otherwise returns True if the creation time cannot be determined.
         '''
         raise NotImplementedError
 
     @setup_task("Construct Object", order=400)
@@ -42,29 +51,32 @@
         # check_completed runs first and so we do not need to call, but
         # for an explicit call we need to call find ourselves.
         if not hasattr(self, '_find_result'):
             self._find_result = await self.find()
         if self._find_result:
             return  # find was successful
         del self._find_result
-        if self.oci_read_only:
+        if self.readonly:
             raise RuntimeError(f'{self} is read only but does not exist')
 
         await self.do_create()
         self._find_result = await self.find()
         return self._find_result
 
     @find_or_create.check_completed()
     async def find_or_create(self):
         self._find_result = await self.find()
         return self._find_result
 
     async def do_create(self):
         raise NotImplementedError
 
+    async def dynamic_dependencies(self):
+        return []
+
     def __repr__(self):
         res = f'<{self.__class__.__name__} '
         try: res += f'name:{self.name} '
         except Exception: pass
         try:
             if self.id:
                 res += f'id: {self.id} '
@@ -190,15 +202,15 @@
             self.name = name
         if id:
             self.id = id
         if not (self.name or self.id):
             raise TypeError('Either name or id is mandatory')
         super().__init__(**kwargs)
         if self.id:
-            self.oci_read_only = True
+            self.readonly = True
 
     @memoproperty
     def exposed_ports(self):
         '''Return a sequence of :class:`OciExposedPort` for any container ports that should be exposed.
 
         By default, instantiate all *OciExposedPort* instances in the injector.
         '''
```

### Comparing `carthage-0.32/carthage/pki.py` & `carthage-0.33/carthage/pki.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/plugins.py` & `carthage-0.33/carthage/plugins.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021, 2022, 2023, Hadron Industries, Inc.
+# Copyright (C) 2021, 2022, 2023, 2024, Hadron Industries, Inc.
 # Carthage is free software; you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License version 3
 # as published by the Free Software Foundation. It is distributed
 # WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the file
 # LICENSE for details.
 
@@ -11,14 +11,15 @@
 import logging
 import types
 import typing
 import sys
 import yaml
 from pathlib import Path
 from importlib.util import spec_from_file_location, module_from_spec, find_spec
+from typing import Union
 from urllib.parse import urlparse
 from .dependency_injection import *
 from .config import ConfigLayout
 from .files import checkout_git_repo
 
 
 logger = logging.getLogger('carthage.plugins')
@@ -62,78 +63,110 @@
 
     # Yes this fails for zips and similar.
     # If we care, we'd need to go to a lot of trouble to unpack things,
     # because we do need to make directories available for things like ansible
     # plays.
     def resource_path(self, resource):
         return self._get_resource(resource)
+plugin_spec = Union[str, dict, Path]
 
+def _parse_plugin_spec(spec: plugin_spec):
+    if isinstance(spec, dict):
+        return spec
+    if hasattr(spec, '__fspath__'):
+        return dict(type='path', path=spec.resolve())
+    assert isinstance(spec, str)
+    if ':' in spec:
+        prefix = spec.partition(':')[0]
+        if prefix in ('https', 'git+ssh'):
+            return dict(type='git', url=spec)
+        raise NotImplementedError(f'unrecognized plugin specification: {spec}')
+    if '/' in spec or spec == '.' or spec == '..':
+        return dict(type='path', path=Path(spec).resolve())
+    return dict(type='module', name=spec)
 
 @inject(injector=Injector)
-def load_plugin(spec: str,
+def load_plugin(spec: plugin_spec,
                 *, injector,
                 ignore_import_errors=False):
+
     '''
     Load a plugin from a plugin specification:
 
     * A path name to a directory containing a ``carthage_plugin.yml``
 
     * A python package name
 
     * A ``https`` URL to a Git repository
 
     * A ``git+ssh`` URL to a git repository
 
     :param ignore_import_errors:  If True, succeed and register the plugin even if the python code raises.  This is intended to allow the plugin to be loaded so its metadata can be examined to determine dependencies.  Obviously the plugin is unlikely to be functional in such a state.
     '''
-    if ':' in str(spec):
-        spec = handle_plugin_url(str(spec), injector)
-    if hasattr(spec, "__fspath__") or '/' in spec or spec == '.' or spec == '..':
-        path = Path(spec).resolve()
-        metadata_path = path / "carthage_plugin.yml"
-        if not metadata_path.exists():
-            raise FileNotFoundError(f'{metadata_path} not found')
-        metadata = yaml.safe_load(metadata_path.read_text())
-        if 'resource_dir' not in metadata:
-            metadata['resource_dir'] = path
-        if 'name' not in metadata:
-            raise ValueError(f'metadata must contain a name when loading plugin from path')
-        # Stop early if already loaded
-        try:
-            injector.get_instance(InjectionKey(CarthagePlugin, name=metadata['name']))
-            logger.debug(f'Plugin {metadata["name"]} already loaded')
-            return
-        except KeyError:
-            pass
-        _handle_plugin_config(injector, metadata, metadata_path, ignore_import_errors=ignore_import_errors)
-        try:
-            python_path = metadata['python']
-            python_path = str(path.joinpath(python_path))
-            if python_path not in sys.path:
-                sys.path.insert(0, python_path)
-        except KeyError:
-            pass
-        if 'package' in metadata:
-            module_spec = find_spec(metadata['package'])
+
+    spec = _parse_plugin_spec(spec)
+
+    if spec['type'] == 'module':
+        module_spec = find_spec(spec['name'])
+        return handle_module_spec(module_spec=module_spec, injector=injector, ignore_import_errors=ignore_import_errors, metadata=None)
+
+    elif spec['type'] == 'path':
+        return handle_path_url(spec['path'], injector, ignore_import_errors=ignore_import_errors)
+
+    elif spec['type'] == 'git':
+        path = handle_git_url(spec, injector)
+        return handle_path_url(path, injector, ignore_import_errors=ignore_import_errors)
+
+    else:
+        raise ValueError(f'unrecognized plugin type in {spec}')
+
+def handle_path_url(spec: dict, injector, ignore_import_errors):
+    path = Path(spec).resolve()
+    metadata_path = path / "carthage_plugin.yml"
+    if not metadata_path.exists():
+        raise FileNotFoundError(f'{metadata_path} not found')
+    metadata = yaml.safe_load(metadata_path.read_text())
+    if 'resource_dir' not in metadata:
+        metadata['resource_dir'] = path
+    if 'name' not in metadata:
+        raise ValueError(f'metadata must contain a name when loading plugin from path')
+    # Stop early if already loaded
+    try:
+        injector.get_instance(InjectionKey(CarthagePlugin, name=metadata['name']))
+        logger.debug(f'Plugin {metadata["name"]} already loaded')
+        return
+    except KeyError:
+        pass
+    _handle_plugin_config(injector, metadata, metadata_path, ignore_import_errors=ignore_import_errors)
+    try:
+        python_path = metadata['python']
+        python_path = str(path.joinpath(python_path))
+        if python_path not in sys.path:
+            sys.path.insert(0, python_path)
+    except KeyError:
+        pass
+    if 'package' in metadata:
+        module_spec = find_spec(metadata['package'])
+    else:
+        package_path = path.joinpath("carthage_plugin.py")
+        name = metadata['name']
+        if '.' not in name:
+            name = "carthage.carthage_plugins." + name
+            _setup_carthage_plugins_module()
+        if package_path.exists():
+            module_spec = spec_from_file_location(
+                name, location=package_path,
+                submodule_search_locations=[str(path / "python")]
+            )
         else:
-            package_path = path.joinpath("carthage_plugin.py")
-            name = metadata['name']
-            if '.' not in name:
-                name = "carthage.carthage_plugins." + name
-                _setup_carthage_plugins_module()
-            if package_path.exists():
-                module_spec = spec_from_file_location(
-                    name, location=package_path,
-                    submodule_search_locations=[str(path / "python")]
-                )
-            else:
-                module_spec = None
-    else:  # spec is a package
-        module_spec = find_spec(spec)
-        metadata = None
+            module_spec = None
+    return handle_module_spec(injector, module_spec=module_spec, metadata=metadata,
+                              ignore_import_errors=ignore_import_errors)
+
+def handle_module_spec(injector, *, module_spec, metadata, ignore_import_errors):
     package = None
     import_error = None
     if module_spec:
         # For some reason module_from_spec sometimes changes spec.name
         module_name = module_spec.name
         if module_name in sys.modules:
             package = sys.modules[module_name]
@@ -141,15 +174,15 @@
             package = module_from_spec(module_spec)
             try:
                 parent_module = None
                 parent, _, stem = module_name.rpartition('.')
                 if parent:
                     parent_module = importlib.import_module(parent)
                     setattr(parent_module, stem, package)
-                    
+
                 sys.modules[module_name] = package
                 module_spec.loader.exec_module(package)
             except BaseException as e:
                 try: del sys.modules[module_name]
                 except KeyError: pass
                 if parent_module: delattr(parent_module, stem)
                 if ignore_import_errors:
@@ -157,55 +190,48 @@
                     import_error = str(e)
                 else:
                     raise
     return injector(load_plugin_from_package, package, metadata,
                     ignore_import_errors=ignore_import_errors,
                     import_error=import_error)
 
-
-def handle_plugin_url(url, injector):
-    parsed = urlparse(url)
-    if parsed.scheme in ('https', 'git+ssh'):
-        return handle_git_url(parsed, injector)
-    else:
-        raise NotImplementedError(f"Don't know how to handle {parsed.scheme} URL")
-
-
-def handle_git_url(parsed, injector):
+def handle_git_url(spec, injector):
+    parsed = urlparse(spec['url'])
     config = injector(ConfigLayout)
     stem = Path(parsed.path).name
     if stem.endswith('.git'):
         stem = stem[:-4]
     dest = Path(config.checkout_dir) / stem
     if dest.exists():
         return dest
     logger.info(f'Checking out {parsed.geturl()}')
-    injector(checkout_git_repo, parsed.geturl(), dest, foreground=True)
+    branch = spec.get('branch', None)
+    injector(checkout_git_repo, parsed.geturl(), dest, branch=branch, foreground=True)
     return dest
 
 
 @inject(injector=Injector)
 def load_plugin_from_package(package: typing.Optional[types.ModuleTyp],
                              metadata: dict = None,
                              *, ignore_import_errors=False,
-                             import_error=None, 
+                             import_error=None,
                              injector):
     if (not metadata) and (not package):
         raise RuntimeError('Either package or metadata must be supplied')
     if metadata:
         if 'resource_dir' in metadata:
             metadata_path = Path(metadata['resource_dir']) / "carthage_plugin.yml"
         else:
             metadata_path = Path(package.__file__)
     if not metadata:
         if not package.__spec__.origin:
             raise SyntaxError(f'{package.__name__} is not a Carthage plugin')
         try:
-            metadata = yaml.safe_load(importlib.resources.read_text(
-                package, "carthage_plugin.yml"))
+            metadata = yaml.safe_load(importlib.resources.files(
+                package).joinpath('carthage_plugin.yml').read_text())
             metadata_path = package.__file__
         except (FileNotFoundError, ImportError):
             # consider the case of hadron-operations
             # plugin is hadron.carthage
             # but when not installed resources live at the top level of the checkout.
             components = len(package.__name__.split("."))
             path_root = Path(package.__file__).parents[components]
```

### Comparing `carthage-0.32/carthage/podman/base.py` & `carthage-0.33/carthage/podman/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C)  2022, 2023, Hadron Industries, Inc.
+# Copyright (C)  2022, 2023, 2024, Hadron Industries, Inc.
 # Carthage is free software; you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License version 3
 # as published by the Free Software Foundation. It is distributed
 # WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the file
 # LICENSE for details.
 
@@ -20,14 +20,15 @@
 from carthage.dependency_injection import *
 from .. import sh, ConfigLayout
 from ..machine import AbstractMachineModel, Machine
 from ..utils import memoproperty
 from ..network import TechnologySpecificNetwork, Network, V4Config, this_network, NetworkConfig
 from ..oci import *
 from ..setup_tasks import setup_task, SetupTaskMixin, TaskWrapperBase, SkipSetupTask
+from .container_host import instantiate_container_host
 
 
 logger = logging.getLogger('carthage.podman')
 
 
 def podman_port_option(p: OciExposedPort):
     res = f'-p{p.host_ip}:{p.host_port}:{p.container_port}'
@@ -44,88 +45,111 @@
         res += f',destination={m.destination}'
     else:
         raise TypeError('destination is required')
     if m.options:
         res += f',{m.options}'
     return res
 
-
 __all__ = []
 
+class HasContainerHostMixin(OciManaged):
 
-class PodmanContainerHost(AsyncInjectable):
+    '''
+    Provide dynamic_dependencies so podman objects are deleted after their host.
+    '''
 
-    @memoproperty
-    def podman_log(self):
-        return self.injector.get_instance(InjectionKey("podman_log", _optional=True))
+    async def dynamic_dependencies(self):
+        if self.container_host is None:
+            await self.ainjector(instantiate_container_host, self)
+        result = await super().dynamic_dependencies()
+        try:
+            result += [self.container_host.machine]
+        except AttributeError: pass
+        return result
     
-    def podman(self, *args,
-               _bg=True, _bg_exc=True):
-        raise NotImplementedError
-
-    async def filesystem_access(self, container):
-        raise NotImplementedError
+        
+@inject_autokwargs(network=this_network)
+class PodmanNetwork(HasContainerHostMixin, TechnologySpecificNetwork, OciManaged):
 
-    async def tar_volume_context(self, volume):
-        '''
-        An asynchronous context manager that tars up a volume and provides a path to that tar file usable in ``podman import``.  Typical usage::
+    container_host: PodmanContainerHost = None
 
-            async with container_host.tar_volume_context(container_image) as path:
-                await container_host.podman('import', path)
+    @property
+    def podman(self):
+        return self.container_host.podman
 
-        On local systems this manages temporary directories.  For remote container hosts, this manages to get the tar file to the remote system and clean up later.
-        '''
-        raise NotImplementedError
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self.name = self.network.name
+        self.container_host = None
+    
+    async def find(self):
+        if not self.container_host:
+            await self.ainjector(instantiate_container_host, self)
+        if not await self.container_host.find():
+            logger.debug('%s does not exist because its container host does not exist', self)
+            return False
+        try:
+            inspect_result = await self.podman(
+                'network', 'inspect', self.network.name, _log=False)
+        except Exception: return False
+        info = json.loads(str(inspect_result))[0]
+        try:
+            return dateutil.parser.isoparse(info['created']).timestamp()
+        except (KeyError, ValueError):
+            logger.error('Unable to understand network inspection result: %s', info)
+            raise NotImplementedError('Podman too old')
 
 
-class LocalPodmanContainerHost(PodmanContainerHost):
+    async def do_create(self):
+        options = ['-d', 'bridge']
+        v4_config = getattr(self.network, 'v4_config', None)
+        if v4_config:
+            if v4_config.network:
+                options.extend([
+                    '--subnet', str(v4_config.network)])
+            if v4_config.gateway is False:
+                options.append('--internal')
+            elif v4_config.gateway and v4_config.gateway  is not True:
+                options.extend([
+                    '--gateway', str(v4_config.gateway)])
+            if v4_config.dhcp:
+                options.extend(['--ipam-driver=dhcp'])
+        await self.podman(
+            'network',
+            'create', self.network.name,
+            *options)
 
-        
-    
-    @contextlib.asynccontextmanager
-    async def filesystem_access(self, container):
-        result = await self.podman(
-            'container', 'mount',
-            container,
-            _bg=True, _bg_exc=False, _log=False)
-        try:
-            path = str(result).strip()
-            yield Path(path)
-        finally:
-            pass  # Perhaps we should unmount, but we'd need a refcount to do that.
+    async def delete(self, force=True):
+        if force:
+            force_options = ['--force']
+        else: force_options = []
+        await self.podman(
+            'network', 'rm', *force_options,
+            self.network.name)
 
-    def podman(self, *args,
-               _bg=True, _bg_exc=False, _log=True):
-        options = {}
-        if _log and self.podman_log:
-            options['_out']=str(self.podman_log)
-            options['_err_to_out'] = True
-        return sh.podman(
-            *args,
-            _bg=_bg, _bg_exc=_bg_exc,
-            _encoding='utf-8',
-            **options)
+    def link_options(self, link):
+        def safe(s):
+            assert ',' not in s
+            assert '=' not in s
+            return s
+        v4_config = link.merged_v4_config
+        options = ['interface_name='+safe(link.interface)]
+        if v4_config.address:
+            options.append('ip='+safe(str(v4_config.address)))
+        if link.mac:
+            options.append('mac='+safe(link.mac))
+        if link.mtu:
+            options.append('mtu='+safe(link.mtu))
+        assert ':' not in self.network.name
+        return safe(self.network.name)+':'+','.join(options)
 
-    @contextlib.asynccontextmanager
-    async def tar_volume_context(self, volume):
-        assert hasattr(volume, 'path')
-        with tempfile.TemporaryDirectory() as path_raw:
-            path = Path(path_raw)
-            await sh.tar(
-                "-C", str(volume.path),
-                "--xattrs",
-                "--xattrs-include=*.*",
-                "-czf",
-                str(path / "container.tar.gz"),
-                ".",
-                _bg=True,
-                _bg_exc=False)
-            yield path / 'container.tar.gz'
+__all__ += ['PodmanNetwork']
 
 class PodmanNetworkMixin:
+    network_implementation_class = PodmanNetwork
 
     async def _setup_networks(self):
         for l in self.network_links.values():
             if l.local_type: continue
             await l.instantiate(PodmanNetwork)
 
     async def _network_options(self):
@@ -146,34 +170,53 @@
             logger.error(f"{self.name} will not join network of {self.pod}; if this is intended then add_provider(network_namespace_key, dependency_quote(None) in {self.name}'s model.  If it is not, then set network_namespace_key to {self.pod}")
         if network_namespace:
             if isinstance(network_namespace, PodmanContainer):
                 await network_namespace.find_or_create()
                 return ['--network', 'container:'+network_namespace.id]
             return []           # Joining a pod
         return await self._network_options() # Creating our own namespace
-           
+
     async def resolve_networking(self, force:bool = False):
+        '''Like
+        :meth:`carthage.machine.NetworkedModel.resolve_networking`
+        except that it looks for :data:`oci_container_network_config`.
+        If cthat key is present, that network config is used instead
+        of ``InjectionKey(NetworkConfig)``.  Doing so allows
+        containers that are lexically contained in their host to have
+        their own NetworkConfig.
+
+        '''
+        if not force and self.network_links:
+            return
+        container_config = await self.ainjector.get_instance_async(InjectionKey(oci_container_network_config, _optional=NotPresent))
+        if container_config is not NotPresent:
+            self.injector.add_provider(InjectionKey(NetworkConfig), dependency_quote(container_config))
         await super().resolve_networking(force=force)
         for net in set(map( lambda l:l.net, self.network_links.values())):
             net.assign_addresses()
-            
+
 @inject(
     podman_pod_options=InjectionKey('podman_pod_options', _optional=NotPresent),
 )
-class PodmanPod(OciPod, PodmanNetworkMixin, carthage.machine.NetworkedModel):
+class PodmanPod(HasContainerHostMixin, PodmanNetworkMixin, carthage.machine.NetworkedModel, OciPod):
 
     #: A list of extra options to pass to pod create
     podman_pod_options = []
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.injector.add_provider(InjectionKey(PodmanPod), dependency_quote(self))
         self.network_links = {}
-
+        self.container_host = None
     async def find(self):
+        if not self.container_host:
+            await self.ainjector(instantiate_container_host, self)
+        if not await self.container_host.find():
+            logger.debug('%s does not exist because its container host does not exist', self)
+            return False
         if self.id:
             inspect_arg = self.id
         else:
             inspect_arg = self.name
         try:
             result = await self.podman(
                 'pod', 'inspect', inspect_arg, _log=False)
@@ -201,28 +244,28 @@
         await self.podman(
             'pod', 'rm',
             *force_options,
             self.name)
 
     @memoproperty
     def podman(self):
-        return self.injector(LocalPodmanContainerHost).podman
+        return self.container_host.podman
 
 
 __all__ += ['PodmanPod']
 
-   
+
 
 @inject_autokwargs(
     oci_container_image=InjectionKey(oci_container_image, _optional=NotPresent),
     podman_restart=InjectionKey('podman_restart', _optional=NotPresent),
     pod=InjectionKey(PodmanPod, _optional=True),
     podman_options=InjectionKey('podman_options', _optional=NotPresent),
 )
-class PodmanContainer(PodmanNetworkMixin, Machine, OciContainer):
+class PodmanContainer(HasContainerHostMixin, PodmanNetworkMixin, Machine, OciContainer):
 
     '''
 An OCI container implemented using ``podman``.  While it is possible to set up a container to be accessible via ssh and to meet all the interfaces of :class:`~carthage.machine.SshMixin`, this is relatively uncommon.  Such containers often have an entry point that is not a full init, and only run one service or program.  Typically :meth:`container_exec` is used to execute an additional command in the scope of a container rather than using :meth:`ssh`.
     '''
 
     #: Timeout in seconds to wait when stopping a container
     stop_timeout = 10
@@ -237,15 +280,15 @@
     def podman_options(self):
         '''Extra options to be passed into podman create as a list
         '''
         try:
             return self.model.podman_options
         except AttributeError:
             return []
-        
+
 
     @memoproperty
     def ssh_options(self):
         if not hasattr(self, 'ssh_port'):
             raise ValueError('Set ssh_port before ssh')
         return (
             *super().ssh_options,
@@ -254,31 +297,35 @@
     #:The port on which to connect to for ssh
     ssh_port: int
 
     @memoproperty
     def ansible_inventory_overrides(self):
         return dict(
             ansible_connection='containers.podman.podman',
+            ansible_podman_extra_args=self.container_host.extra_args,
             ansible_pipelining=False,
             ansible_host=self.full_name,
         )
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self._operation_lock = asyncio.Lock()
+        self.container_host = None
 
     @memoproperty
     def podman(self):
         return self.container_host.podman
 
-    @memoproperty
-    def container_host(self):
-        return self.injector(LocalPodmanContainerHost)
 
     async def find(self):
+        if not self.container_host:
+            await self.ainjector(instantiate_container_host, self)
+        if not await self.container_host.find():
+            logger.debug('%s does not exist because its container host does not exist', self)
+            return False
         try:
             result = await self.podman(
                 'container', 'inspect', self.full_name,
                 _bg=True, _bg_exc=False, _log=False)
         except sh.ErrorReturnCode:
             return False
         containers = json.loads(str(result))
@@ -289,15 +336,15 @@
         self.id = self.container_info['Id']
         self.running = self.container_info['State']['Running']
         try:
             return dateutil.parser.isoparse(containers[0]['Created']).timestamp()
         except Exception as e:
             raise ValueError(f'Invalid ISO string: {self.container_info["Created"]}')
 
-            
+
     async def do_create(self):
         image = self.oci_container_image
         if isinstance(image, OciImage):
             await image.async_become_ready()
             image = image.oci_image_tag
         if self.pod:
             await self.pod.async_become_ready()
@@ -331,26 +378,29 @@
             options.append('--pod=' + self.pod.name)
         for m in self.mounts:
             options.append(podman_mount_option(self.injector, m))
         options.extend(self.podman_options)
         return options
 
     async def delete(self, force=True, volumes=True):
+        if not self.container_host:
+            await self.ainjector(instantiate_container_host, self)
         force_args = []
         if force:
             force_args.append('--force')
         if volumes:
             force_args.append('--volumes')
         await self.podman(
             'container', 'rm',
             *force_args, self.full_name,
             _bg=True, _bg_exc=False)
 
     async def is_machine_running(self):
-        assert await self.find(), "Container does not exist"
+        if not await self.find():
+            return False # Containers that do not exist are not running
         self.running = self.container_info['State']['Running']
         return self.running
 
     async def start_machine(self):
         async with self._operation_lock:
             await self.is_machine_running()
             if self.running:
@@ -361,50 +411,58 @@
             await self.podman(
                 'container', 'start', self.full_name,
                 _bg=True, _bg_exc=False)
         await self.is_machine_running()
 
     async def stop_machine(self):
         async with self._operation_lock:
+            await self.is_machine_running()
             if not self.running:
                 return
+            logger.info(f'Stopping {self.full_name}')
             await self.podman(
                 'container', 'stop',
                 f'-t{self.stop_timeout}',
                 self.full_name,
                 _bg=True, _bg_exc=False)
             self.running = False
             await super().stop_machine()
 
-    def container_exec(self, *args):
+    def container_exec(self, *args, _user=None):
         '''
 'Execute a command in a running container and return stdout.  This function intentionally has a differentname than :meth:`carthage.container.Container.container_command` because that method does not expect the container to be running.
 '''
+        if _user is None:
+            _user = self.runas_user
+        if _user != 'root':
+            raise NotImplementedError('only can run as root for now')
         result = self.podman(
             'container', 'exec',
             self.full_name,
             *args,
             _log=False)
         return result
 
     #: An alias to be more compatible with :class:`carthage.container.Container`
     shell = container_exec
+    #: container_exec meets the run_command interface
+    run_command = container_exec
 
     def _apply_to_filesystem_customization(self, customization):
         @contextlib.asynccontextmanager
         async def customization_context():
             async with self.machine_running(ssh_online=False), self.filesystem_access() as path:
                 customization.path = path
                 yield
             return
         customization.customization_context = customization_context()
-        customization.run_command = self.container_exec
 
     def filesystem_access(self, user='root'):
-        return self.container_host.filesystem_access(self.full_name)
+        assert self.container_host, 'call self.find first'
+        return self.container_host.filesystem_access('mount', self.full_name)
 
     def __repr__(self):
         try:
             host = repr(self.container_host)
         except Exception:
             host = "repr failed"
         return f'<{self.__class__.__name__} {self.name} on {host}>'
@@ -449,14 +507,15 @@
         res =  self.injector.get_instance(InjectionKey(PodmanImageModel, _ready=False, _optional=True))
         if res is None: raise AttributeError
         return res
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.injector.add_provider(InjectionKey(NetworkConfig), dependency_quote(None))
+
 @inject_autokwargs(
     base_image=InjectionKey(oci_container_image, _optional=NotPresent),
 )
 class PodmanImage(OciImage, SetupTaskMixin):
 
     '''
     Represents an OCI container image and provides facilities for building the image.
@@ -467,16 +526,19 @@
 
     last_layer = None
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.layer_number = 1
         self.injector.add_provider(InjectionKey('podman_log'), self.stamp_path/'podman.log')
+        self.container_host = None
 
     async def pull_base_image(self):
+        if not self.container_host:
+            await self.ainjector(instantiate_container_host, self)
         if isinstance(self.base_image, OciImage):
             await self.base_image.async_become_ready()
             base_image = self.base_image.oci_image_tag
         else:
             base_image = self.base_image
         if not base_image.startswith('localhost/'):
             await self.podman(
@@ -488,23 +550,28 @@
         image_info = json.loads(str(inspect_result))[0]
         self.parse_base_image_info(image_info)
 
     def parse_base_image_info(self, image_info):
         config = image_info['Config']
         if not self.oci_image_command and 'Cmd' in config:
             self.oci_image_command = config['Cmd']
-        if not self.oci_image_entry_point and 'EntryPoint' in config:
-            self.oci_image_entry_point = config['EntryPoint']
+        if not self.oci_image_entry_point and 'Entrypoint' in config:
+            self.oci_image_entry_point = config['Entrypoint']
         self.base_image_info = image_info
         self.last_layer = self.base_image_info['Id']
 
     async def find(self):
+        if not self.container_host:
+            await self.ainjector(instantiate_container_host, self)
+        if not await self.container_host.find():
+            logger.debug('%s does not exist because its container host does not exist', self)
+            return False
         if self.id:
             to_find = self.id
-            self.oci_read_only = True
+            self.readonly = True
         else:
             to_find = self.oci_image_tag
         try:
             result = await self.podman(
                 'image', 'inspect', to_find,
                 _log=False)
         except sh.ErrorReturnCode:
@@ -618,26 +685,23 @@
         await self.find_or_create()
         return await AsyncInjectable.async_ready(self)
 
     @memoproperty
     def podman(self):
         return self.container_host.podman
 
-    @memoproperty
-    def container_host(self):
-        return self.injector(LocalPodmanContainerHost)
 
     @memoproperty
     def stamp_path(self):
         config = self.injector(ConfigLayout)
         path = Path(config.output_dir)/"podman_image"/self.oci_image_tag.replace('/','_')
         path.mkdir(exist_ok=True, parents=True)
         return path
-    
-                            
+
+
 
 __all__ += ['PodmanImage']
 podman_image_volume_key = InjectionKey('carthage.podman/image_volume')
 
 
 @inject(base_image=None)
 @inject_autokwargs(
@@ -691,16 +755,16 @@
         # We always want to rerun images
         return False
 
     @memoproperty
     def stamp(self):
         #Overridden if an image_layer_task is assigned as a class property
         return self.customization.__name__
-    
-    
+
+
 @inject_autokwargs(
     config_layout=ConfigLayout,
     podman_options=InjectionKey('podman_options', _optional=NotPresent),
     )
 class ContainerfileImage(OciImage):
 
     '''
@@ -728,25 +792,23 @@
                 warnings.warn(f'Unable to find module for {self.__class__.__qualname__}: {e}')
             if module:
                 try: path = Path(module.__path__[0])
                 except Exception:
                     path = Path(module.__file__).parent
                 self.source_container_context = self.container_context = path/self.container_context
         super().__init__(**kwargs)
+        self.container_host = None
         if len(self.setup_tasks) > 2:
             # More than just find_or_create and copy_context_if_needed
             self.setup_tasks.sort(key=lambda t: 1 if t.func == OciManaged.find_or_create.func else 0)
             self.container_context = self.output_path
         self.injector.add_provider(InjectionKey("podman_log"), self.stamp_path/'podman.log')
-                                   
-            
 
-    @memoproperty
-    def container_host(self):
-        return self.injector(LocalPodmanContainerHost)
+
+
 
     @memoproperty
     def output_path(self):
         path = Path(self.config_layout.output_dir)/'podman_image'
         tag = self.oci_image_tag.replace('/', '_')
         path /= tag
         path.mkdir(exist_ok=True, parents=True)
@@ -764,29 +826,34 @@
         else:
             raise SkipSetupTask
 
     @copy_context_if_needed.invalidator()
     def copy_context_if_needed(self, last_run):
         source_mtime = self.container_context_mtime(self.source_container_context)
         if source_mtime > last_run: return False
-        return False
-    
-        
+        return True
+
+
     async def do_create(self):
         options = await self._build_options()
         return await self.container_host.podman(
             'build',
             '--annotation', 'com.hadronindustries.carthage.image_mtime='+ \
             datetime.datetime.fromtimestamp(
                 self.container_context_mtime(self.container_context),datetime.timezone.utc).isoformat(),
             '-t'+self.oci_image_tag,
             *options,
             self.container_context)
 
     async def find(self):
+        if not self.container_host:
+            await self.ainjector(instantiate_container_host, self)
+        if not await self.container_host.find():
+            logger.debug('%s does not exist because its container host does not exist', self)
+            return False
         try: inspect_result = await self.container_host.podman(
                 'image', 'inspect',
                 self.oci_image_tag, _log=False)
         except sh.ErrorReturnCode: return False
         inspect_json = json.loads(str(inspect_result.stdout, 'utf-8'))
         created = dateutil.parser.isoparse(inspect_json[0]['Created']).timestamp()
         hadron_mtime_str = inspect_json[0]['Annotations'].get('com.hadronindustries.carthage.image_mtime')
@@ -802,16 +869,16 @@
     def container_context_mtime(container_context):
         context = Path(container_context)
         mtime = 0.0
         for p in context.iterdir():
             stat = p.stat()
             if stat.st_mtime >mtime: mtime = stat.st_mtime
         return mtime
-    
-    
+
+
 
     async def _build_options(self):
         options = []
         # Instantiate a container simply so we can ask it for volume, mount, and environment options.
         with instantiation_not_ready():
             container = await self.ainjector(PodmanContainer, name='image_options')
         for k, v in self.injector.filter_instantiate(
@@ -821,75 +888,67 @@
         for m in container.mounts:
             options.append(podman_mount_option(self.injector, m))
         options.extend(self.podman_options)
         return options
 
 __all__ += ['ContainerfileImage']
 
-@inject_autokwargs(network=this_network)
-class PodmanNetwork(TechnologySpecificNetwork, OciManaged):
+class PodmanVolume(HasContainerHostMixin, OciManaged):
 
-    @memoproperty
-    def container_host(self):
-        return self.injector(LocalPodmanContainerHost)
+    name: str
+
+    def __init__(self, name:str=None, **kwargs):
+        self.container_host = None
+        super().__init__(**kwargs)
+        if name:
+            self.name = name
+        if not hasattr(self, 'name'):
+            raise TypeError(f'{self.__class__.__name__} requires a name either specified in a subclass or constructor.')
 
-    @property
-    def podman(self):
-        return self.container_host.podman
-    
     async def find(self):
+        if not self.container_host:
+            await self.ainjector(instantiate_container_host, self)
+        if not await self.container_host.find():
+            logger.debug(f'{self} does not exist because the container host does not exist.')
+            return False
         try:
-            inspect_result = await self.podman(
-                'network', 'inspect', self.network.name, _log=False)
-        except Exception: return False
-        info = json.loads(str(inspect_result))[0]
+            result = await self.podman(
+                'volume', 'inspect', self.name, _log=False)
+        except sh.ErrorReturnCode:
+            return False
+        info = json.loads(str(result))[0]
         try:
-            return dateutil.parser.isoparse(info['created']).timestamp()
+            return dateutil.parser.isoparse(info['CreatedAt']).timestamp()
         except (KeyError, ValueError):
-            logger.error('Unable to understand network inspection result: %s', info)
+            logger.error('Unable to understand volume inspection result: %s', info)
             raise NotImplementedError('Podman too old')
-        
 
     async def do_create(self):
-        options = ['-d', 'bridge']
-        v4_config = getattr(self.network, 'v4_config', None)
-        if v4_config:
-            if v4_config.network:
-                options.extend([
-                    '--subnet', str(v4_config.network)])
-            if v4_config.gateway is False:
-                options.append('--internal')
-            elif v4_config.gateway and v4_config.gateway  is not True:
-                options.extend([
-                    '--gateway', str(v4_config.gateway)])
-            if v4_config.dhcp:
-                options.extend(['--ipam-driver=dhcp'])
-        await self.podman(
-            'network',
-            'create', self.network.name,
-            *options)
+        return await self.podman(
+            'volume', 'create',
+            self.name)
 
-    async def delete(self, force=True):
-        if force:
-            force_options = ['--force']
-        else: force_options = []
+    async def delete(self):
         await self.podman(
-            'network', 'rm', *force_options,
-            self.network.name)
-        
-    def link_options(self, link):
-        def safe(s):
-            assert ',' not in s
-            assert '=' not in s
-            return s
-        v4_config = link.merged_v4_config
-        options = ['interface_name='+safe(link.interface)]
-        if v4_config.address:
-            options.append('ip='+safe(str(v4_config.address)))
-        if link.mac:
-            options.append('mac='+safe(link.mac))
-        if link.mtu:
-            options.append('mtu='+safe(link.mtu))
-        assert ':' not in self.network.name
-        return safe(self.network.name)+':'+','.join(options)
+            'volume', 'rm',
+            self.name)
 
-__all__ += ['PodmanNetwork']
+    @property
+    def podman(self):
+        return self.container_host.podman
+
+    @contextlib.asynccontextmanager
+    async def filesystem_access(self):
+        '''
+        Like :meth:`carthage.Machine.filesystem_access` except gains access to a podman volume.
+
+        Usage::
+
+            async with volume.filesystem_access() as path:
+                 # Path points to a mount for the volume inside the context manager.
+        '''
+        async with self.container_host.filesystem_access(
+'volume', 'mount',
+                self.name) as path:
+            yield path
+
+__all__ += ['PodmanVolume']
```

### Comparing `carthage-0.32/carthage/podman/modeling.py` & `carthage-0.33/carthage/podman/modeling.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 import typing
 
 from carthage.modeling import *
 import carthage.modeling.implementation
 from .base import *
 from carthage import *
 from carthage.dependency_injection import *
-from carthage.oci import OciImage
+from carthage.oci import OciImage, oci_container_network_config
 
 __all__ = []
 
 
-class PodmanPodModel( carthage.machine.NetworkedModel, ModelContainer):
+class PodmanPodModel( carthage.machine.NetworkedModel, ModelContainer, AsyncInjectable):
 
     '''A container that can group a number of :class:`MachineModels` representing Podman containers.
 
     * By default, ``machine_implementation_key`` within a :class:`PodmanPodModel` is :class:`PodmanContainer`.
 
     * By default, when added to an enclosing injector, this model does not provide :class:`PodmanPod` in that context, although it does provide :class:`PodmanPod` within its own injector.  An example illustrates::
 
@@ -78,39 +78,62 @@
         super().__init_subclass__(**kwargs)
         if not template:
             cls.add_provider(InjectionKey(PodmanPod, name=cls.name_for(), _globally_unique=cls.pod_name_global),
                          injector_access(InjectionKey(PodmanPod)),
                          close=False,
                          propagate=cls.pod_name_global,
                          transclusion_overrides=cls.pod_name_global)
+            cls.add_provider(InjectionKey(carthage.machine.ResolvableModel, name=cls.name_for(), role='pod', _globally_unique=cls.pod_name_global),
+                         injector_access(InjectionKey(PodmanPod)),
+                         close=False,
+                         propagate=cls.pod_name_global,
+                         transclusion_overrides=cls.pod_name_global)
             globally_unique_key(InjectionKey(carthage.machine.ResolvableModel, name=cls.name_for()+'-pod'))(cls)
                                          
                                           
     pod_name_global = True  # : If True, the pod name is globally unique
 
     @classmethod
     def our_key(self):
         name = self.name_for()
         return InjectionKey(self.__class__, name=name)
 
     @classmethod
     def supplementary_injection_keys(self, k):
         if k.constraints:
-            yield InjectionKey(PodmanPod, **k.constraints)
             yield InjectionKey(PodmanPodModel, **k.constraints)
             if 'name' in k.constraints and not issubclass(k.target, carthage.machine.ResolvableModel):
                 yield InjectionKey(carthage.machine.ResolvableModel, name=k.constraints['name']+'-pod',
                                    _globally_unique=self.pod_name_global)
 
     pod = injector_access(InjectionKey(PodmanPod))
 
     def __repr__(self):
         return f'<{self.__class__.__name__} name:{self.name}>'
+    async def resolve_networking(self, force:bool = False):
+        '''Like
+        :meth:`carthage.machine.NetworkedModel.resolve_networking`
+        except that it looks for :data:`oci_container_network_config`.
+        If cthat key is present, that network config is used instead
+        of ``InjectionKey(NetworkConfig)``.  Doing so allows
+        containers that are lexically contained in their host to have
+        their own NetworkConfig.
+
+        '''
+        if not force and self.network_links:
+            return
+        container_config = await self.ainjector.get_instance_async(InjectionKey(oci_container_network_config, _optional=NotPresent))
+        if container_config is not NotPresent:
+            try:
+                self.injector.add_provider(InjectionKey(NetworkConfig), dependency_quote(container_config))
+            except ExistingProvider: pass
+        await super().resolve_networking(force=force)
+        for net in set(map( lambda l:l.net, self.network_links.values())):
+            net.assign_addresses()
     
-
 __all__ += ['PodmanPodModel']
 
 
 class PodmanImageModel(ImageRole, PodmanImage):
 
     '''
     Like a :class:`PodmanImage` excetp:
```

### Comparing `carthage-0.32/carthage/ports.py` & `carthage-0.33/carthage/ports.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/pytest.py` & `carthage-0.33/carthage/pytest.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/pytest_plugin.py` & `carthage-0.33/carthage/pytest_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,14 +60,16 @@
     ainjector.close()
 
 
 def pytest_addoption(parser):
     group = parser.getgroup("Carthage", "Carthage Continuous Integration Options")
     group.addoption('--carthage-config',
                     type=argparse.FileType('rt'),
+                    default=[],
+                    action='append',
                     help="Specify yaml carthage config; this configuration file describes where to put VMs and where to find hadron-operations.  It is not the test configuration for individual tests.  This option is typically used on the controller and not alongside --carthage-json on the system under test.",
                     metavar="file")
     group.addoption('--carthage-json',
                     metavar="file",
                     type=argparse.FileType('wt'),
                     help="Write json results to this file")
     group.addoption('--test-parameters', '--test-params',
@@ -85,20 +87,20 @@
     global json_log
     json_log = config.getoption('carthage_json')
     json_out = []
     if not config.getoption('carthage_commands_verbose'):
         logging.getLogger('sh').setLevel(logging.ERROR)
         logging.getLogger('carthage.sh').propagate = False
         carthage_config = config.getoption('carthage_config')
-    if carthage_config:
+    for c in carthage_config:
         config_layout = base_injector(ConfigLayout)
         try:
-            config_layout.load_yaml(carthage_config)
+            config_layout.load_yaml(c)
         finally:
-            carthage_config.close()
+            c.close()
     test_params_yaml = config.getoption('test_parameters')
     if test_params_yaml:
         config.carthage_test_parameters = yaml.load(test_params_yaml)
         test_params_yaml.close()
 
 
 def pytest_runtest_logreport(report):
```

### Comparing `carthage-0.32/carthage/resources/ansible-chroot-helper` & `carthage-0.33/carthage/resources/ansible-chroot-helper`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/resources/fai/files/etc/pam.d/su/OPENROOT` & `carthage-0.33/carthage/resources/fai/files/etc/pam.d/su/OPENROOT`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/resources/fai/files/etc/resolv.conf/DEFAULT` & `carthage-0.33/carthage/resources/fai/files/etc/resolv.conf/DEFAULT`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/resources/fai/scripts/GRUB_EFI/10-setup` & `carthage-0.33/carthage/resources/fai/scripts/GRUB_EFI/10-setup`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/resources/runner_console.py` & `carthage-0.33/carthage/resources/runner_console.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/resources/templates/bridge-network.mako` & `carthage-0.33/carthage/resources/templates/bridge-network.mako`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/resources/templates/default-network.mako` & `carthage-0.33/carthage/resources/templates/default-network.mako`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/resources/templates/network-base.mako` & `carthage-0.33/carthage/resources/templates/network-base.mako`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/resources/templates/skeletons/prototype.mako` & `carthage-0.33/carthage/resources/templates/skeletons/prototype.mako`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/resources/templates/vlan-network.mako` & `carthage-0.33/carthage/resources/templates/vlan-network.mako`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/resources/templates/vm-config.mako` & `carthage-0.33/carthage/resources/templates/vm-config.mako`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/runner_commands.py` & `carthage-0.33/carthage/runner_commands.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/setup_tasks.py` & `carthage-0.33/carthage/setup_tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import os
 import os.path
 import time
 import typing
 import sys
 import shutil
 import weakref
+import hashlib
 import importlib.resources
 from pathlib import Path
 import carthage
 from carthage.dependency_injection import AsyncInjector, inject, BaseInstantiationContext, InjectionKey
 from carthage.dependency_injection.introspection import current_instantiation
 from carthage.config import ConfigLayout
 from carthage.utils import memoproperty, import_resources_files
@@ -267,14 +268,20 @@
         * Otherwise this task should not run.
 
         :param: obj
             The instance on which setup_tasks are being run.
         :param run_methods: If False , no check_completed or invalidators are run.  If the task has a check_completed function, return None rather than True or False for wether the task should run.  Invalidators and hash functions are ignored, and the return is dependent only on stamps.
 
         '''
+        def _h(s):
+            '''Shorten cases where hash_func returns a long string rather than a hash
+            '''
+            if len(s) > 65:     # sha256 plus a newline
+                return hashlib.sha256(s.encode()).hexdigest()
+            return s
         if dependency_last_run is None:
             dependency_last_run = 0.0
         if self.check_completed_func:
             if not run_methods: return (None, dependency_last_run)
             last_run = await ainjector(self.check_completed_func, obj)
             hash_contents = ""
             if last_run is True:
@@ -288,15 +295,15 @@
         if last_run < dependency_last_run:
             obj.logger_for().debug(
                 f"Task {self.description} last run {_iso_time(last_run)}, but dependency run more recently at {_iso_time(dependency_last_run)}")
             return (True, dependency_last_run)
         if (not self.check_completed_func) and run_methods:
             actual_hash_contents = await ainjector(self.hash_func, obj)
             if actual_hash_contents != hash_contents:
-                obj.logger_for().info(f'Task {self.description} invalidated by hash_func() change from `{hash_contents}` to `{actual_hash_contents}`; last run {_iso_time(last_run)}')
+                obj.logger_for().info(f'Task {self.description} invalidated by hash_func() change from `{_h(hash_contents)}` to `{_h(actual_hash_contents)}`; last run {_iso_time(last_run)}')
                 return (True, dependency_last_run)
         if self.invalidator_func and run_methods:
             if not await ainjector(self.invalidator_func, obj, last_run=last_run):
                 obj.logger_for().info(f"Task {self.description} invalidated for {obj} by invalidator_func(); last run {_iso_time(last_run)}")
                 return (True, time.time())
         obj.logger_for().debug(f"Task {self.description} last run for {obj} at {_iso_time(last_run)}; re-running not required")
         return (False, last_run)
@@ -502,18 +509,21 @@
                     adl_keys=self.setup_task_event_keys())
                 try:
                     if (not context_entered) and context is not None:
                         await context.__aenter__()
                         context_entered = True
                     if not dry_run:
                         self.logger_for().info(f"Running {t.description} task for {self}")
+                        started = time.time()
                         with SetupTaskContext(self, t):
                             await ainjector(t, self)
                         dependency_last_run = time.time()
-                        self.logger_for().info(f"Finished running {t.description} task for {self} at {dependency_last_run}")
+                        a = datetime.datetime.fromtimestamp(started)
+                        b = datetime.datetime.fromtimestamp(dependency_last_run)
+                        self.logger_for().info(f"Finished running {t.description} task for {self} from {a.time()} to {b.time()} ({b - a})")
                     else:
                         self.logger_for().info(f'Would run {t.description} task for {self}')
                 except SkipSetupTask:
                     pass
                 except Exception:
                     self.logger_for().exception(f"Error running {t.description} for {self}:")
                     if context_entered:
```

### Comparing `carthage-0.32/carthage/sh.py` & `carthage-0.33/carthage/sh.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,20 +10,18 @@
 import asyncio as _asyncio
 import sh as _sh
 
 '''
 Monkey patch the sh module to include __await__.
 Also, by default for commands retrieved through this module set _bg=True and _bg_exc=False
 '''
-Command = _sh.Command
+_sh_context = _sh(_bg=True, _bg_exc=False)
 
 def __getattr__(name):
-    val = getattr(_sh, name)
-    if isinstance(val, Command):
-        val = val.bake(_bg=True, _bg_exc=False)
+    val = getattr(_sh_context, name)
     globals()[name] = val
     return val
 
 def running_command_await(self):
     loop = _asyncio.get_event_loop()
     res =  yield from loop.run_in_executor(None, self.wait)
     return res
```

### Comparing `carthage-0.32/carthage/skeleton.py` & `carthage-0.33/carthage/skeleton.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/sonic.py` & `carthage-0.33/carthage/sonic.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/ssh.py` & `carthage-0.33/carthage/ssh.py`

 * *Files 7% similar despite different names*

```diff
@@ -166,15 +166,17 @@
                     ssh_options = list(a.machine.ssh_options) + a.machine.config_layout.global_ssh_options.split()
                 elif ssh_origin is not sso:
                     raise RuntimeError(f"Two different ssh_origins: {sso} and {ssh_origin}")
                 args[i] = str(a)
         if ssh_options:
             ssh_options = list(ssh_options)
 
-        ssh_options.extend(['-oUserKnownHostsFile=' + str(config_layout.state_dir) + "/ssh_known_hosts"])
+        ssh_options.extend(['-F'+str(ssh_agent.ssh_config)])
+        if key:
+            ssh_options.extend(['-i'+str(key.key_path)])
         ssh_options = " ".join(ssh_options)
         rsync_opts = ['-e', 'ssh ' + ssh_options]
         if rsync_command:
             rsync_opts .append(rsync_command)
 
 
         if ssh_origin:
@@ -217,15 +219,15 @@
 @inject(
     injector=Injector,
     key=InjectionKey(SshKey, _optional=True, _ready=False))
 class SshAgent(Injectable):
 
     def __init__(self, injector, key):
         config_layout = injector(ConfigLayout)
-        run = config_layout.local_run_dir
+        run = Path(config_layout.local_run_dir)
         auth_sock = os.path.join(run, "ssh_agent")
         os.makedirs(run, exist_ok=True)
         try:
             os.unlink(auth_sock)
         except FileNotFoundError:
             pass
         if config_layout.production_ssh_agent and 'SSH_AUTH_SOCK' in os.environ:
@@ -236,15 +238,25 @@
                                         '-D', _bg=True)
             self.auth_sock = auth_sock
         if key and is_obj_ready(key):
             self.handle_key(key)
         elif key:  # not ready
             future = asyncio.ensure_future(key.async_become_ready())
             future.add_done_callback(lambda f: self.handle_key(f.result()))
-
+        ssh_config = run.joinpath('ssh_config')
+        ssh_config_text = f'''
+UserKnownHostsFile {config_layout.state_dir}/ssh_known_hosts
+        '''
+        if os.path.exists('/etc/ssh/ssh_config'):
+            ssh_config_text += 'Include /etc/ssh/ssh_config\n'
+        if os.path.exists(os.path.expanduser('~/.ssh/config')):
+            ssh_config_text += 'Include config\n'
+        ssh_config.write_text(ssh_config_text)
+        self.ssh_config = ssh_config
+        
     def handle_key(self, key):
         key.add_to_agent(self)
 
     def close(self):
         if self.process is not None:
             try:
                 self.process.terminate()
```

### Comparing `carthage-0.32/carthage/system_dependency.py` & `carthage-0.33/carthage/system_dependency.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .machine import Machine
 from .utils import memoproperty
 __all__ = []
 
 
 class SystemDependency(abc.ABC, Injectable):
 
-    '''Represents a dependency that may be required by a :class:`carthage.Machine` before a machine is started.  These dependencies may also be required by a :func:`carthage.setup_tasks.setup_task`; see :func:`depend_on()`.
+    '''Represents a dependency that may be required by a :class:`carthage.Machine` before a machine is started.  These dependencies may also be required by a :func:`carthage.setup_tasks.setup_task`; see :meth:`carthage.setup_tasks.TaskWrapperBase.depend_on()`.
 
     Note that typically instances of this class rather than subclasses are used as dependency providers on an Injector.  That way, :meth:`~carthage.Injector.get_instance` returns the instance without processing injected dependencies.  These dependencies are later processed when a method like :meth:`carthage.Machine.start_dependencies()` calls the :meth:`__call__()` method.
 
 
 '''
 
     name: str
@@ -67,15 +67,16 @@
         if not name and ('host' not in self.key.constraints):
             raise ValueError(f'when MachineDependency is called with an InjectionKey, either the key must have a `host` constraint or a name must be given explicitly')
 
     async def __call__(self, ainjector):
         machine = await ainjector.get_instance_async(self.key)
         if not hasattr(machine, 'start_machine') and hasattr(machine, 'machine'):
             # Allow a dependency to be set on a MachineModel not just a machine
-            machine = machine.machine
+            ainjector = machine.injector(AsyncInjector)
+            machine = await ainjector.get_instance_async(InjectionKey(Machine, _ready=True))
         await machine.start_machine()
         if self.online is MachineDependency.ONLINE_DEFAULT:
             if machine.machine_running_ssh_online:
                 await machine.ssh_online()
         elif self.online:
             await getattr(machine, self.online)()
```

### Comparing `carthage-0.32/carthage/systemd.py` & `carthage-0.33/carthage/systemd.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/tb_utils.py` & `carthage-0.33/carthage/tb_utils.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/utils.py` & `carthage-0.33/carthage/utils.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/vault/__init__.py` & `carthage-0.33/carthage/vault/__init__.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/vm.py` & `carthage-0.33/carthage/vm.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/vmware/__init__.py` & `carthage-0.33/carthage/vmware/__init__.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/vmware/authorization.py` & `carthage-0.33/carthage/vmware/authorization.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/vmware/cluster.py` & `carthage-0.33/carthage/vmware/cluster.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/vmware/config_spec.py` & `carthage-0.33/carthage/vmware/config_spec.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/vmware/connection.py` & `carthage-0.33/carthage/vmware/connection.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,31 +8,38 @@
 
 from carthage import *
 
 from pyVim.connect import Connect, SmartConnect, Disconnect
 from ssl import create_default_context
 
 import logging
-
+from urllib.parse import urlparse
 
 @inject(config=ConfigLayout)
 class VmwareConnection(Injectable):
 
     def __init__(self, config):
         self.config = config.vmware
         ssl_context = create_default_context()
         if self.config.validate_certs is False:
             ssl_context.check_hostname = False
             ssl_context.verify_mode = 0
+        kwargs = dict(host=self.config.hostname,
+                      user=self.config.username,
+                      pwd=self.config.password,
+                      sslContext=ssl_context)
+        if self.config.proxy:
+            r = urlparse(self.config.proxy)
+            if r.scheme != 'http':
+                raise RuntimeError(f"unsupported proxy scheme '{r.scheme}' in proxy string '{self.config.proxy}'; current support is only for 'http'")
+            kwargs['httpProxyHost'] = r.hostname
+            kwargs['httpProxyPort'] = r.port
         self.connection = None
-        logging.debug(f'connecting to {self.config.hostname} as {self.config.username}')
-        self.connection = SmartConnect(host=self.config.hostname,
-                                       user=self.config.username,
-                                       pwd=self.config.password,
-                                       sslContext=ssl_context)
+        logging.debug(f'connecting to {self.config.hostname} as {self.config.username} using {kwargs}')
+        self.connection = SmartConnect(**kwargs)
         self.content = self.connection.content
         logging.debug(f'connected to {self.config.hostname}')
 
     def close(self):
         if self.connection:
             Disconnect(self.connection)
             self.connection = None
```

### Comparing `carthage-0.32/carthage/vmware/convenience.py` & `carthage-0.33/carthage/vmware/convenience.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/vmware/credentials.py` & `carthage-0.33/carthage/vmware/credentials.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from ..config import ConfigSchema, config_key
 
 
 class CredentialsSchema(ConfigSchema, prefix="vmware"):
     hostname: str
     username: str = "{vault:secret/password/{vmware.hostname}:username}"
     password: str = "{vault:secret/password/{vmware.hostname}:password}"
+    proxy: str = None
     validate_certs: bool = False
 
 
 #: Injection key to get Vmware credential configuration.  Only assume that username, hostname, password and verify_certs are set with this key as a dependency.
 vmware_credentials = config_key('vmware')
 
 __all__ = ['vmware_credentials']
```

### Comparing `carthage-0.32/carthage/vmware/datacenter.py` & `carthage-0.33/carthage/vmware/datacenter.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/vmware/datastore.py` & `carthage-0.33/carthage/vmware/datastore.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/vmware/folder.py` & `carthage-0.33/carthage/vmware/folder.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/vmware/host.py` & `carthage-0.33/carthage/vmware/host.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/vmware/image.py` & `carthage-0.33/carthage/vmware/image.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/vmware/inventory.py` & `carthage-0.33/carthage/vmware/inventory.py`

 * *Files 5% similar despite different names*

```diff
@@ -208,16 +208,14 @@
     def _find_from_path(self):
         find = self.connection.content.searchIndex.FindByInventoryPath
         ret = find(self.vmware_path)
         return ret
 
     def set_custom_fields(self):
         entity = self.mob
-        if not self.writable:
-            return
         fields = self.injector.get_instance(custom_fields_key)
         for name, val_func in fields.items():
             field = self._ensure_custom_field(name, vim.ManagedEntity)
             self.set_custom_field(field, val_func(self))
 
     def _fetch_custom_field(self, fname):
         content = self.connection.content
@@ -229,14 +227,18 @@
 
     def _ensure_custom_field(self, fname, ftype):
         try:
             return self._fetch_custom_field(fname)
         except KeyError:
             content = self.connection.content
             cfm = content.customFieldsManager
+            if not self.writable:
+                # This isn't exactly right since it looks at writable
+                # for the object not the overall connection
+                raise ValueError(f'unable to write field {fname} because object is read-only')
             return cfm.AddFieldDefinition(name=fname, moType=ftype)
 
     def set_custom_field(self, field, value):
         if self.mob is None:
             raise RuntimeError('unable to set fields on null object')
         if isinstance(field, str):
             field = self._fetch_custom_field(field)
@@ -244,16 +246,18 @@
         cfm = content.customFieldsManager
         cfm.SetField(entity=self.mob, key=field.key, value=value)
 
     def get_field_value(self, field):
         '''Return the vmware custom field value or None if not set
         '''
         if isinstance(field, str):
-            field = self._ensure_custom_field(field, vim.ManagedEntity)
-
+            try:
+                field = self._fetch_custom_field(field)
+            except KeyError:
+                return None
         for val in self.mob.customValue:
             if (val.key == field.key) and (val.value != ''):
                 return val.value
         return None
 
     @staticmethod
     def _parent_path_from_mob(mob):
```

### Comparing `carthage-0.32/carthage/vmware/network.py` & `carthage-0.33/carthage/vmware/network.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/vmware/utils.py` & `carthage-0.33/carthage/vmware/utils.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage/vmware/vm.py` & `carthage-0.33/carthage/vmware/vm.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/carthage.egg-info/PKG-INFO` & `carthage-0.33/carthage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carthage
-Version: 0.32
+Version: 0.33
 Summary: A powerful Infrastructure as Code (IAC) framework
 Author-email: Sam Hartman <sam.hartman@hadronindustries.com>
 License: LGPL-3
 Project-URL: Homepage, https://github.com/hadron/carthage
 Project-URL: Documentation, https://carthage.readthedocs.io
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `carthage-0.32/carthage.egg-info/SOURCES.txt` & `carthage-0.33/carthage.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 carthage/network/links.py
 carthage/network/mac.py
 carthage/network/namespace.py
 carthage/network/switch.py
 carthage/podman/__init__.py
 carthage/podman/base.py
 carthage/podman/carthage_plugin.yml
+carthage/podman/container_host.py
 carthage/podman/modeling.py
 carthage/resources/80-net-setup-link.rules
 carthage/resources/ansible-chroot-helper
 carthage/resources/hadron-xorg-modes
 carthage/resources/runner_console.py
 carthage/resources/test_ansible.yml
 carthage/resources/fai/class/DEFAULT.var
@@ -145,14 +146,15 @@
 carthage/vmware/vm.py
 tests/carthage_test_utils.py
 tests/conftest.py
 tests/inner_conftest.py
 tests/inner_plugin_test.py
 tests/machine_mock.py
 tests/override-config.yml
+tests/podman_remote_host.py
 tests/template-2.expected
 tests/test_ansible.py
 tests/test_become.py
 tests/test_carthage_plugin.py
 tests/test_config.py
 tests/test_container.py
 tests/test_dependency_injection.py
```

### Comparing `carthage-0.32/pyproject.toml` & `carthage-0.33/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "carthage"
-version = "0.32"
+version = "0.33"
 authors = [
     { name = "Sam Hartman", email = "sam.hartman@hadronindustries.com" },
 ]
 description = "A powerful Infrastructure as Code (IAC) framework"
 readme = "README.rst"
 requires-python = ">=3.11"
 license = { text = "LGPL-3" }
```

### Comparing `carthage-0.32/tests/carthage_test_utils.py` & `carthage-0.33/tests/carthage_test_utils.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/tests/conftest.py` & `carthage-0.33/tests/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,14 +20,19 @@
 import os.path
 import pytest
 import posix
 from carthage.pytest import *
 
 pytest_plugins = ('carthage.pytest_plugin',)
 
+def pytest_addoption(parser):
+    group = parser.getgroup('podman', 'Podman test options')
+    group.addoption('--remote-container-host',
+                    action='store_true',
+                    help='Use remote container host in AWS for Podman Carthage tests')
 
 @pytest.mark.no_rootless
 @pytest.fixture(scope='session')
 def test_ainjector(loop):
     if posix.geteuid() != 0:
         pytest.skip("Not running as root; volume tests skipped", )
     try:
```

### Comparing `carthage-0.32/tests/machine_mock.py` & `carthage-0.33/tests/machine_mock.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/tests/test_ansible.py` & `carthage-0.33/tests/test_ansible.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/tests/test_become.py` & `carthage-0.33/tests/test_become.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/tests/test_carthage_plugin.py` & `carthage-0.33/tests/test_carthage_plugin.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/tests/test_config.py` & `carthage-0.33/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/tests/test_container.py` & `carthage-0.33/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/tests/test_dependency_injection.py` & `carthage-0.33/tests/test_dependency_injection.py`

 * *Files 2% similar despite different names*

```diff
@@ -660,7 +660,15 @@
         '''This plugin fails to instantiate because it has a missing dependency
                        '''
         name = 'not_found'
 
     ainjector.add_provider(not_found)
     with pytest.raises(InjectionFailed):
         await ainjector.filter_instantiate_async(Plugin, ['name'], ready=True)
+
+def test_injection_key_typos():
+    '''
+        Confirm that an invalid option to InjectionKey raises.
+        '''
+    with pytest.raises(TypeError, match='not an InjectionKey parameter'):
+        InjectionKey(Injector, _foo=42)
+
```

### Comparing `carthage-0.32/tests/test_deployment.py` & `carthage-0.33/tests/test_deployment.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/tests/test_event.py` & `carthage-0.33/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/tests/test_image.py` & `carthage-0.33/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/tests/test_kvstore.py` & `carthage-0.33/tests/test_kvstore.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/tests/test_modeling.py` & `carthage-0.33/tests/test_modeling.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/tests/test_network.py` & `carthage-0.33/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/tests/test_pki.py` & `carthage-0.33/tests/test_pki.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/tests/test_plugins.py` & `carthage-0.33/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/tests/test_podman.py` & `carthage-0.33/tests/test_podman.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C)  2022, 2023, Hadron Industries, Inc.
+# Copyright (C)  2022, 2023, 2024, Hadron Industries, Inc.
 # Carthage is free software; you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License version 3
 # as published by the Free Software Foundation. It is distributed
 # WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the file
 # LICENSE for details.
 import json
@@ -14,38 +14,72 @@
 from carthage.oci import oci_container_image, OciExposedPort, OciMount
 from carthage.ansible import *
 from carthage.container import container_image
 from carthage.modeling import *
 from carthage.image import SshAuthorizedKeyCustomizations
 from carthage.ssh import SshKey
 from carthage import *
+from carthage.become_privileged import BecomePrivilegedMixin
 from carthage.machine import FilesystemCustomization
-import carthage
+import carthage.sh
 from carthage.pytest import *
 
 state_dir = Path(__file__).parent.joinpath("test_state")
 
+
+
 @pytest.fixture(scope='session')
 def enable_podman():
     import carthage.plugins
     base_injector(carthage.plugins.load_plugin, 'carthage.podman')
 
-@pytest.fixture()
-def ainjector(ainjector, enable_podman):
-    ainjector = ainjector.claim("test_podman.py")
+@pytest.fixture(scope='module')
+def ainjector(enable_podman, pytestconfig, loop):
+    ainjector = base_injector.claim('test_podman.py')(AsyncInjector)
     config = ainjector.injector(carthage.ConfigLayout)
     config.state_dir = state_dir
     state_dir.mkdir(parents=True, exist_ok=True)
+    if pytestconfig.getoption('remote_container_host'):
+        from podman_remote_host import container_host
+        ainjector.add_provider(ssh_jump_host, injector_access(podman_container_host))
+    else:
+        container_host = LocalPodmanContainerHost
+    ainjector.add_provider(podman_container_host, container_host)
+    container_host_instance = loop.run_until_complete(ainjector.get_instance_async(InjectionKey(container_host, _ready=False)))
+    try:
+        host_machine = loop.run_until_complete(container_host_instance.ainjector.get_instance_async(InjectionKey(Machine, _ready=False)))
+    except KeyError:
+        host_machine = None
+    try:
+        if host_machine:
+            loop.run_until_complete(host_machine.async_become_ready())
+    except Exception as e:
+        logger.exception('Error bringing container_host to ready:')
+        try:
+            logger.info('Deleting %s', host_machine)
+            loop.run_until_complete(host_machine.delete())
+            host_machine = None
+        except Exception:
+            logger.exception('Error deleting container_host')
+        raise e
     yield ainjector
+    if host_machine:
+        logger.info('Deleting %s', host_machine)
+        try:
+            loop.run_until_complete(host_machine.ainjector(host_machine.delete))
+        except Exception as e:
+            logger.exception('error cleaning up container host')
+        
     shutil.rmtree(state_dir, ignore_errors=True)
+    ainjector.close()
 
 @pytest.fixture()
 def layout_fixture(ainjector):
     loop = ainjector.loop
-    ainjector.add_provider(podman_layout)
+    ainjector.replace_provider(podman_layout)
     layout = loop.run_until_complete(ainjector.get_instance_async(CarthageLayout))
     yield layout
     try: loop.run_until_complete(
             layout.podman_net.instantiated.delete(force=True))
     except Exception: pass
 
 
@@ -82,23 +116,23 @@
             @setup_task("Test filesystem customization in image model")
             def test_fscust(self): pass
 
         class container_cust(ContainerCustomization):
 
             @setup_task("Test container customization")
             def test_container_cust(self): pass
-            
+
     class foo(MachineModel):
 
         name = 'foo.com'
 
     class ssh_test(MachineModel):
         name = 'ssh-test.foo.com'
         ip_address = '127.0.0.1'
-
+        podman_options = ('--privileged',)
         add_provider(OciExposedPort(22))
 
     class mount_test(MachineModel):
         add_provider(OciMount(
             mount_type='bind',
             destination='/host',
             source='/',
@@ -136,26 +170,26 @@
 
         @setup_task('Create dynamic script')
         def create_dynamic_script(self):
             self.output_path.joinpath('script').write_text('''\
 #!/bin/sh
 exit 0
             ''')
-            
-            
+
+
     class true_machine(MachineModel):
         add_provider(oci_container_image, injector_access(TrueImage))
 
         name = 'true-machine'
 
     class dynamic_machine(MachineModel):
         add_provider(oci_container_image, injector_access(DynamicContainerFileImage))
 
         name = 'dynamic-machine'
-        
+
     class pod_group(ModelGroup):
         add_provider(OciExposedPort(22))
 
         @provides(InjectionKey(PodmanPod))
         class pod(PodmanPod):
             name = 'carthage-test-pod'
 
@@ -175,14 +209,17 @@
         name = 'net_test'
         class config(NetworkConfigModel):
             add('eth0', mac=None, net=podman_net)
 
         class container(MachineModel):
             pass
 
+    class volume(PodmanVolume):
+        name = 'test_volume'
+        
 @async_test
 async def test_podman_create(ainjector):
     l = await ainjector(podman_layout)
     ainjector = l.ainjector
     machine = l.foo.machine
     await machine.async_become_ready()
     assert await machine.find()
@@ -219,15 +256,16 @@
         async with machine.machine_running(ssh_online=False):
             await machine.container_exec('apt', 'update')
             await machine.container_exec(
                 'apt', '-y', '--no-install-recommends', 'install', 'openssh-server')
             await machine.apply_customization(SshAuthorizedKeyCustomizations)
             await machine.container_exec('mkdir', '/run/sshd')
             await machine.container_exec('/usr/sbin/sshd')
-            await machine.ssh_online()
+            with TestTiming(400):
+                await machine.ssh_online()
     finally:
         await machine.delete()
 
 
 @async_test
 async def test_podman_image(ainjector):
     l = await ainjector(podman_layout)
@@ -361,8 +399,24 @@
     finally:
         try: await layout.net_pod.pod.delete(force=True)
         except Exception: pass
 
 @async_test
 async def test_podman_image_model(layout_fixture):
     await layout_fixture.ImageModelCustomizations.build_image()
-    
+
+@async_test
+async def test_podman_volume(layout_fixture):
+    layout = layout_fixture
+    ainjector = layout.ainjector
+    await layout.volume.async_become_ready()
+    try:
+        try:
+            async with layout.volume.filesystem_access() as path:
+                (path/'foo').write_text('bar')
+        except  carthage.sh.ErrorReturnCode_125 as e:
+            if b'unrecognized' in e.stderr:
+                pytest.xfail('podman too old')
+            raise
+    finally:
+        await layout.volume.delete()
+
```

### Comparing `carthage-0.32/tests/test_setup_tasks.py` & `carthage-0.33/tests/test_setup_tasks.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/tests/test_utils.py` & `carthage-0.33/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/tests/test_vm.py` & `carthage-0.33/tests/test_vm.py`

 * *Files identical despite different names*

### Comparing `carthage-0.32/tests/test_vmware.py` & `carthage-0.33/tests/test_vmware.py`

 * *Files identical despite different names*

