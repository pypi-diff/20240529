# Comparing `tmp/candlefl-0.2.2.tar.gz` & `tmp/candlefl-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "candlefl-0.2.2.tar", max compression
+gzip compressed data, was "candlefl-0.2.3.tar", max compression
```

## Comparing `candlefl-0.2.2.tar` & `candlefl-0.2.3.tar`

### file list

```diff
@@ -1,134 +1,134 @@
--rw-r--r--   0        0        0     1633 2024-03-22 02:29:51.462220 candlefl-0.2.2/LICENSE
--rw-r--r--   0        0        0    12007 2024-03-26 04:55:38.026775 candlefl-0.2.2/README.md
--rw-r--r--   0        0        0      130 2024-03-26 04:52:59.778055 candlefl-0.2.2/candlefl/__init__.py
--rw-r--r--   0        0        0     9403 2024-02-28 23:26:22.870223 candlefl-0.2.2/candlefl/cli.py
--rw-r--r--   0        0        0     1709 2024-02-28 23:26:22.870223 candlefl-0.2.2/candlefl/compatibility.py
--rw-r--r--   0        0        0      337 2024-02-28 23:26:22.870223 candlefl-0.2.2/candlefl/config_resolver.py
--rw-r--r--   0        0        0      190 2024-03-26 05:00:10.564030 candlefl-0.2.2/candlefl/datamodules/__init__.py
--rw-r--r--   0        0        0     4816 2024-02-28 23:26:22.858223 candlefl-0.2.2/candlefl/datamodules/base.py
--rw-r--r--   0        0        0    13751 2024-02-28 23:26:22.858223 candlefl-0.2.2/candlefl/datamodules/cifar.py
--rw-r--r--   0        0        0    13186 2024-02-28 23:26:22.858223 candlefl-0.2.2/candlefl/datamodules/emnist.py
--rw-r--r--   0        0        0    11965 2024-02-28 23:26:22.858223 candlefl-0.2.2/candlefl/datamodules/fashionmnist.py
--rw-r--r--   0        0        0     1193 2024-02-28 23:26:22.858223 candlefl-0.2.2/candlefl/datamodules/types.py
--rw-r--r--   0        0        0      191 2024-02-28 23:26:22.862223 candlefl-0.2.2/candlefl/federated/__init__.py
--rw-r--r--   0        0        0      175 2024-03-26 05:00:56.176242 candlefl-0.2.2/candlefl/federated/agents/__init__.py
--rw-r--r--   0        0        0     1057 2024-02-28 23:26:22.858223 candlefl-0.2.2/candlefl/federated/agents/base.py
--rw-r--r--   0        0        0     2437 2024-03-26 05:01:13.552323 candlefl-0.2.2/candlefl/federated/agents/v1.py
--rw-r--r--   0        0        0      184 2024-03-26 05:02:01.196544 candlefl-0.2.2/candlefl/federated/aggregators/__init__.py
--rw-r--r--   0        0        0      844 2024-02-28 23:26:22.858223 candlefl-0.2.2/candlefl/federated/aggregators/base.py
--rw-r--r--   0        0        0     1337 2024-02-28 23:26:22.858223 candlefl-0.2.2/candlefl/federated/aggregators/fedavg.py
--rw-r--r--   0        0        0     6465 2024-02-28 23:26:22.862223 candlefl-0.2.2/candlefl/federated/entrypoint.py
--rw-r--r--   0        0        0     4146 2024-02-28 23:26:22.862223 candlefl-0.2.2/candlefl/federated/fl_params.py
--rw-r--r--   0        0        0      181 2024-03-26 05:02:39.384722 candlefl-0.2.2/candlefl/federated/samplers/__init__.py
--rw-r--r--   0        0        0      616 2024-02-28 23:26:22.862223 candlefl-0.2.2/candlefl/federated/samplers/base.py
--rw-r--r--   0        0        0      635 2024-02-28 23:26:22.862223 candlefl-0.2.2/candlefl/federated/samplers/random.py
--rw-r--r--   0        0        0     1081 2024-02-28 23:26:22.862223 candlefl-0.2.2/candlefl/federated/types.py
--rw-r--r--   0        0        0      141 2024-02-28 23:26:22.870223 candlefl-0.2.2/candlefl/models/__init__.py
--rw-r--r--   0        0        0      161 2024-02-28 23:26:22.870223 candlefl-0.2.2/candlefl/models/core/__init__.py
--rw-r--r--   0        0        0      166 2024-02-28 23:26:22.862223 candlefl-0.2.2/candlefl/models/core/cifar/__init__.py
--rw-r--r--   0        0        0      166 2024-03-26 05:04:51.757340 candlefl-0.2.2/candlefl/models/core/cifar/cifar10/__init__.py
--rw-r--r--   0        0        0      915 2024-02-28 23:26:22.862223 candlefl-0.2.2/candlefl/models/core/cifar/cifar10/alexnet.py
--rw-r--r--   0        0        0     3531 2024-02-28 23:26:22.862223 candlefl-0.2.2/candlefl/models/core/cifar/cifar10/densenet.py
--rw-r--r--   0        0        0      471 2024-02-28 23:26:22.862223 candlefl-0.2.2/candlefl/models/core/cifar/cifar10/lenet.py
--rw-r--r--   0        0        0     2752 2024-02-28 23:26:22.862223 candlefl-0.2.2/candlefl/models/core/cifar/cifar10/mobilenet.py
--rw-r--r--   0        0        0     7806 2024-02-28 23:26:22.862223 candlefl-0.2.2/candlefl/models/core/cifar/cifar10/resnet.py
--rw-r--r--   0        0        0     3711 2024-02-28 23:26:22.862223 candlefl-0.2.2/candlefl/models/core/cifar/cifar10/shufflenetv2.py
--rw-r--r--   0        0        0     1845 2024-02-28 23:26:22.862223 candlefl-0.2.2/candlefl/models/core/cifar/cifar10/squeezenet.py
--rw-r--r--   0        0        0     6730 2024-02-28 23:26:22.862223 candlefl-0.2.2/candlefl/models/core/cifar/cifar10/vgg.py
--rw-r--r--   0        0        0      169 2024-02-28 23:26:22.862223 candlefl-0.2.2/candlefl/models/core/cifar/cifar100/__init__.py
--rw-r--r--   0        0        0      917 2024-02-28 23:26:22.862223 candlefl-0.2.2/candlefl/models/core/cifar/cifar100/alexnet.py
--rw-r--r--   0        0        0     3536 2024-02-28 23:26:22.862223 candlefl-0.2.2/candlefl/models/core/cifar/cifar100/densenet.py
--rw-r--r--   0        0        0      473 2024-02-28 23:26:22.862223 candlefl-0.2.2/candlefl/models/core/cifar/cifar100/lenet.py
--rw-r--r--   0        0        0     2755 2024-02-28 23:26:22.862223 candlefl-0.2.2/candlefl/models/core/cifar/cifar100/mobilenet.py
--rw-r--r--   0        0        0     7816 2024-02-28 23:26:22.862223 candlefl-0.2.2/candlefl/models/core/cifar/cifar100/resnet.py
--rw-r--r--   0        0        0     3716 2024-02-28 23:26:22.862223 candlefl-0.2.2/candlefl/models/core/cifar/cifar100/shufflenetv2.py
--rw-r--r--   0        0        0     1848 2024-02-28 23:26:22.862223 candlefl-0.2.2/candlefl/models/core/cifar/cifar100/squeezenet.py
--rw-r--r--   0        0        0     6739 2024-02-28 23:26:22.862223 candlefl-0.2.2/candlefl/models/core/cifar/cifar100/vgg.py
--rw-r--r--   0        0        0      168 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/__init__.py
--rw-r--r--   0        0        0      178 2024-02-28 23:26:22.862223 candlefl-0.2.2/candlefl/models/core/emnist/balanced/__init__.py
--rw-r--r--   0        0        0      925 2024-02-28 23:26:22.862223 candlefl-0.2.2/candlefl/models/core/emnist/balanced/alexnet.py
--rw-r--r--   0        0        0     3541 2024-02-28 23:26:22.862223 candlefl-0.2.2/candlefl/models/core/emnist/balanced/densenet.py
--rw-r--r--   0        0        0      481 2024-02-28 23:26:22.862223 candlefl-0.2.2/candlefl/models/core/emnist/balanced/lenet.py
--rw-r--r--   0        0        0      727 2024-02-28 23:26:22.862223 candlefl-0.2.2/candlefl/models/core/emnist/balanced/mlp.py
--rw-r--r--   0        0        0     2757 2024-02-28 23:26:22.862223 candlefl-0.2.2/candlefl/models/core/emnist/balanced/mobilenet.py
--rw-r--r--   0        0        0     7816 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/balanced/resnet.py
--rw-r--r--   0        0        0     3721 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/balanced/shufflenetv2.py
--rw-r--r--   0        0        0     1855 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/balanced/squeezenet.py
--rw-r--r--   0        0        0     6740 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/balanced/vgg.py
--rw-r--r--   0        0        0      178 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/byclass/__init__.py
--rw-r--r--   0        0        0      925 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/byclass/alexnet.py
--rw-r--r--   0        0        0     3541 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/byclass/densenet.py
--rw-r--r--   0        0        0      481 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/byclass/lenet.py
--rw-r--r--   0        0        0      727 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/byclass/mlp.py
--rw-r--r--   0        0        0     2757 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/byclass/mobilenet.py
--rw-r--r--   0        0        0     7816 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/byclass/resnet.py
--rw-r--r--   0        0        0     3721 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/byclass/shufflenetv2.py
--rw-r--r--   0        0        0     1855 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/byclass/squeezenet.py
--rw-r--r--   0        0        0     6739 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/byclass/vgg.py
--rw-r--r--   0        0        0      178 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/bymerge/__init__.py
--rw-r--r--   0        0        0      925 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/bymerge/alexnet.py
--rw-r--r--   0        0        0     3541 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/bymerge/densenet.py
--rw-r--r--   0        0        0      481 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/bymerge/lenet.py
--rw-r--r--   0        0        0      727 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/bymerge/mlp.py
--rw-r--r--   0        0        0     2757 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/bymerge/mobilenet.py
--rw-r--r--   0        0        0     7816 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/bymerge/resnet.py
--rw-r--r--   0        0        0     3721 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/bymerge/shufflenetv2.py
--rw-r--r--   0        0        0     1855 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/bymerge/squeezenet.py
--rw-r--r--   0        0        0     6739 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/bymerge/vgg.py
--rw-r--r--   0        0        0      176 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/digits/__init__.py
--rw-r--r--   0        0        0      923 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/digits/alexnet.py
--rw-r--r--   0        0        0     3539 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/digits/densenet.py
--rw-r--r--   0        0        0      479 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/digits/lenet.py
--rw-r--r--   0        0        0      725 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/digits/mlp.py
--rw-r--r--   0        0        0     2757 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/digits/mobilenet.py
--rw-r--r--   0        0        0     7814 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/digits/resnet.py
--rw-r--r--   0        0        0     3719 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/digits/shufflenetv2.py
--rw-r--r--   0        0        0     1853 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/digits/squeezenet.py
--rw-r--r--   0        0        0     6738 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/digits/vgg.py
--rw-r--r--   0        0        0      177 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/letters/__init__.py
--rw-r--r--   0        0        0      924 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/letters/alexnet.py
--rw-r--r--   0        0        0     3540 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/letters/densenet.py
--rw-r--r--   0        0        0      480 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/letters/lenet.py
--rw-r--r--   0        0        0      726 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/letters/mlp.py
--rw-r--r--   0        0        0     2757 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/letters/mobilenet.py
--rw-r--r--   0        0        0     7815 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/letters/resnet.py
--rw-r--r--   0        0        0     3720 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/letters/shufflenetv2.py
--rw-r--r--   0        0        0     1854 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/letters/squeezenet.py
--rw-r--r--   0        0        0     6739 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/letters/vgg.py
--rw-r--r--   0        0        0      175 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/mnist/__init__.py
--rw-r--r--   0        0        0      913 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/mnist/alexnet.py
--rw-r--r--   0        0        0     3529 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/mnist/densenet.py
--rw-r--r--   0        0        0      469 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/mnist/lenet.py
--rw-r--r--   0        0        0      715 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/mnist/mlp.py
--rw-r--r--   0        0        0     2757 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/mnist/mobilenet.py
--rw-r--r--   0        0        0     7813 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/mnist/resnet.py
--rw-r--r--   0        0        0     3709 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/mnist/shufflenetv2.py
--rw-r--r--   0        0        0     1843 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/mnist/squeezenet.py
--rw-r--r--   0        0        0     6737 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/emnist/mnist/vgg.py
--rw-r--r--   0        0        0      173 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/fashionmnist/__init__.py
--rw-r--r--   0        0        0      920 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/fashionmnist/alexnet.py
--rw-r--r--   0        0        0     3536 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/fashionmnist/densenet.py
--rw-r--r--   0        0        0      476 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/fashionmnist/lenet.py
--rw-r--r--   0        0        0      722 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/fashionmnist/mlp.py
--rw-r--r--   0        0        0     2752 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/fashionmnist/mobilenet.py
--rw-r--r--   0        0        0     7811 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/fashionmnist/resnet.py
--rw-r--r--   0        0        0     3716 2024-02-28 23:26:22.866223 candlefl-0.2.2/candlefl/models/core/fashionmnist/shufflenetv2.py
--rw-r--r--   0        0        0     1850 2024-02-28 23:26:22.870223 candlefl-0.2.2/candlefl/models/core/fashionmnist/squeezenet.py
--rw-r--r--   0        0        0     6734 2024-02-28 23:26:22.870223 candlefl-0.2.2/candlefl/models/core/fashionmnist/vgg.py
--rw-r--r--   0        0        0      357 2024-02-28 23:26:22.870223 candlefl-0.2.2/candlefl/models/sota/__init__.py
--rw-r--r--   0        0        0     2240 2024-02-28 23:26:22.870223 candlefl-0.2.2/candlefl/models/sota/alexnet.py
--rw-r--r--   0        0        0     9505 2024-02-28 23:26:22.870223 candlefl-0.2.2/candlefl/models/sota/densenet.py
--rw-r--r--   0        0        0     2369 2024-02-28 23:26:22.870223 candlefl-0.2.2/candlefl/models/sota/lenet.py
--rw-r--r--   0        0        0     3859 2024-02-28 23:26:22.870223 candlefl-0.2.2/candlefl/models/sota/mlp.py
--rw-r--r--   0        0        0     7725 2024-02-28 23:26:22.870223 candlefl-0.2.2/candlefl/models/sota/mobilenet.py
--rw-r--r--   0        0        0    19587 2024-02-28 23:26:22.870223 candlefl-0.2.2/candlefl/models/sota/resnet.py
--rw-r--r--   0        0        0     8999 2024-02-28 23:26:22.870223 candlefl-0.2.2/candlefl/models/sota/shufflenetv2.py
--rw-r--r--   0        0        0     5714 2024-02-28 23:26:22.870223 candlefl-0.2.2/candlefl/models/sota/squeezenet.py
--rw-r--r--   0        0        0    17278 2024-02-28 23:26:22.870223 candlefl-0.2.2/candlefl/models/sota/vgg.py
--rw-r--r--   0        0        0      164 2024-02-28 23:26:22.870223 candlefl-0.2.2/candlefl/models/wrapper/__init__.py
--rw-r--r--   0        0        0    27862 2024-02-28 23:26:22.870223 candlefl-0.2.2/candlefl/models/wrapper/cifar.py
--rw-r--r--   0        0        0    78771 2024-02-28 23:26:22.870223 candlefl-0.2.2/candlefl/models/wrapper/emnist.py
--rw-r--r--   0        0        0    16088 2024-02-28 23:26:22.870223 candlefl-0.2.2/candlefl/models/wrapper/fashionmnist.py
--rw-r--r--   0        0        0      273 2024-02-28 23:26:22.870223 candlefl-0.2.2/candlefl/utils.py
--rw-r--r--   0        0        0     3693 2024-03-26 04:52:56.138038 candlefl-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    13608 1970-01-01 00:00:00.000000 candlefl-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1633 2024-05-29 05:56:18.877000 candlefl-0.2.3/LICENSE
+-rw-r--r--   0        0        0    12007 2024-05-29 05:56:18.890000 candlefl-0.2.3/README.md
+-rw-r--r--   0        0        0      130 2024-05-29 05:56:18.892000 candlefl-0.2.3/candlefl/__init__.py
+-rw-r--r--   0        0        0     9403 2024-05-29 05:56:18.892000 candlefl-0.2.3/candlefl/cli.py
+-rw-r--r--   0        0        0     1709 2024-05-29 05:56:18.893000 candlefl-0.2.3/candlefl/compatibility.py
+-rw-r--r--   0        0        0      337 2024-05-29 05:56:18.893000 candlefl-0.2.3/candlefl/config_resolver.py
+-rw-r--r--   0        0        0      190 2024-05-29 05:56:18.894000 candlefl-0.2.3/candlefl/datamodules/__init__.py
+-rw-r--r--   0        0        0     4816 2024-05-29 05:56:18.894000 candlefl-0.2.3/candlefl/datamodules/base.py
+-rw-r--r--   0        0        0    13751 2024-05-29 05:56:18.895000 candlefl-0.2.3/candlefl/datamodules/cifar.py
+-rw-r--r--   0        0        0    13186 2024-05-29 05:56:18.895000 candlefl-0.2.3/candlefl/datamodules/emnist.py
+-rw-r--r--   0        0        0    11965 2024-05-29 05:56:18.896000 candlefl-0.2.3/candlefl/datamodules/fashionmnist.py
+-rw-r--r--   0        0        0     1193 2024-05-29 05:56:18.896000 candlefl-0.2.3/candlefl/datamodules/types.py
+-rw-r--r--   0        0        0      191 2024-05-29 05:56:18.897000 candlefl-0.2.3/candlefl/federated/__init__.py
+-rw-r--r--   0        0        0      175 2024-05-29 05:56:18.898000 candlefl-0.2.3/candlefl/federated/agents/__init__.py
+-rw-r--r--   0        0        0     1057 2024-05-29 05:56:18.898000 candlefl-0.2.3/candlefl/federated/agents/base.py
+-rw-r--r--   0        0        0     2437 2024-05-29 05:56:18.898000 candlefl-0.2.3/candlefl/federated/agents/v1.py
+-rw-r--r--   0        0        0      184 2024-05-29 05:56:18.899000 candlefl-0.2.3/candlefl/federated/aggregators/__init__.py
+-rw-r--r--   0        0        0      844 2024-05-29 05:56:18.899000 candlefl-0.2.3/candlefl/federated/aggregators/base.py
+-rw-r--r--   0        0        0     1337 2024-05-29 05:56:18.900000 candlefl-0.2.3/candlefl/federated/aggregators/fedavg.py
+-rw-r--r--   0        0        0     6465 2024-05-29 05:56:18.900000 candlefl-0.2.3/candlefl/federated/entrypoint.py
+-rw-r--r--   0        0        0     4146 2024-05-29 05:56:18.900000 candlefl-0.2.3/candlefl/federated/fl_params.py
+-rw-r--r--   0        0        0      181 2024-05-29 05:56:18.901000 candlefl-0.2.3/candlefl/federated/samplers/__init__.py
+-rw-r--r--   0        0        0      616 2024-05-29 05:56:18.902000 candlefl-0.2.3/candlefl/federated/samplers/base.py
+-rw-r--r--   0        0        0      635 2024-05-29 05:56:18.902000 candlefl-0.2.3/candlefl/federated/samplers/random.py
+-rw-r--r--   0        0        0     1081 2024-05-29 05:56:18.902000 candlefl-0.2.3/candlefl/federated/types.py
+-rw-r--r--   0        0        0      141 2024-05-29 05:56:18.903000 candlefl-0.2.3/candlefl/models/__init__.py
+-rw-r--r--   0        0        0      161 2024-05-29 05:56:18.903000 candlefl-0.2.3/candlefl/models/core/__init__.py
+-rw-r--r--   0        0        0      166 2024-05-29 05:56:18.904000 candlefl-0.2.3/candlefl/models/core/cifar/__init__.py
+-rw-r--r--   0        0        0      166 2024-05-29 05:56:18.904000 candlefl-0.2.3/candlefl/models/core/cifar/cifar10/__init__.py
+-rw-r--r--   0        0        0      915 2024-05-29 05:56:18.905000 candlefl-0.2.3/candlefl/models/core/cifar/cifar10/alexnet.py
+-rw-r--r--   0        0        0     3531 2024-05-29 05:56:18.905000 candlefl-0.2.3/candlefl/models/core/cifar/cifar10/densenet.py
+-rw-r--r--   0        0        0      471 2024-05-29 05:56:18.905000 candlefl-0.2.3/candlefl/models/core/cifar/cifar10/lenet.py
+-rw-r--r--   0        0        0     2752 2024-05-29 05:56:18.906000 candlefl-0.2.3/candlefl/models/core/cifar/cifar10/mobilenet.py
+-rw-r--r--   0        0        0     7806 2024-05-29 05:56:18.906000 candlefl-0.2.3/candlefl/models/core/cifar/cifar10/resnet.py
+-rw-r--r--   0        0        0     3711 2024-05-29 05:56:18.907000 candlefl-0.2.3/candlefl/models/core/cifar/cifar10/shufflenetv2.py
+-rw-r--r--   0        0        0     1845 2024-05-29 05:56:18.907000 candlefl-0.2.3/candlefl/models/core/cifar/cifar10/squeezenet.py
+-rw-r--r--   0        0        0     6730 2024-05-29 05:56:18.907000 candlefl-0.2.3/candlefl/models/core/cifar/cifar10/vgg.py
+-rw-r--r--   0        0        0      169 2024-05-29 05:56:18.908000 candlefl-0.2.3/candlefl/models/core/cifar/cifar100/__init__.py
+-rw-r--r--   0        0        0      917 2024-05-29 05:56:18.908000 candlefl-0.2.3/candlefl/models/core/cifar/cifar100/alexnet.py
+-rw-r--r--   0        0        0     3536 2024-05-29 05:56:18.909000 candlefl-0.2.3/candlefl/models/core/cifar/cifar100/densenet.py
+-rw-r--r--   0        0        0      473 2024-05-29 05:56:18.909000 candlefl-0.2.3/candlefl/models/core/cifar/cifar100/lenet.py
+-rw-r--r--   0        0        0     2755 2024-05-29 05:56:18.909000 candlefl-0.2.3/candlefl/models/core/cifar/cifar100/mobilenet.py
+-rw-r--r--   0        0        0     7816 2024-05-29 05:56:18.910000 candlefl-0.2.3/candlefl/models/core/cifar/cifar100/resnet.py
+-rw-r--r--   0        0        0     3716 2024-05-29 05:56:18.910000 candlefl-0.2.3/candlefl/models/core/cifar/cifar100/shufflenetv2.py
+-rw-r--r--   0        0        0     1848 2024-05-29 05:56:18.911000 candlefl-0.2.3/candlefl/models/core/cifar/cifar100/squeezenet.py
+-rw-r--r--   0        0        0     6739 2024-05-29 05:56:18.911000 candlefl-0.2.3/candlefl/models/core/cifar/cifar100/vgg.py
+-rw-r--r--   0        0        0      168 2024-05-29 05:56:18.912000 candlefl-0.2.3/candlefl/models/core/emnist/__init__.py
+-rw-r--r--   0        0        0      178 2024-05-29 05:56:18.913000 candlefl-0.2.3/candlefl/models/core/emnist/balanced/__init__.py
+-rw-r--r--   0        0        0      925 2024-05-29 05:56:18.913000 candlefl-0.2.3/candlefl/models/core/emnist/balanced/alexnet.py
+-rw-r--r--   0        0        0     3541 2024-05-29 05:56:18.913000 candlefl-0.2.3/candlefl/models/core/emnist/balanced/densenet.py
+-rw-r--r--   0        0        0      481 2024-05-29 05:56:18.914000 candlefl-0.2.3/candlefl/models/core/emnist/balanced/lenet.py
+-rw-r--r--   0        0        0      727 2024-05-29 05:56:18.914000 candlefl-0.2.3/candlefl/models/core/emnist/balanced/mlp.py
+-rw-r--r--   0        0        0     2757 2024-05-29 05:56:18.914000 candlefl-0.2.3/candlefl/models/core/emnist/balanced/mobilenet.py
+-rw-r--r--   0        0        0     7816 2024-05-29 05:56:18.915000 candlefl-0.2.3/candlefl/models/core/emnist/balanced/resnet.py
+-rw-r--r--   0        0        0     3721 2024-05-29 05:56:18.915000 candlefl-0.2.3/candlefl/models/core/emnist/balanced/shufflenetv2.py
+-rw-r--r--   0        0        0     1855 2024-05-29 05:56:18.915000 candlefl-0.2.3/candlefl/models/core/emnist/balanced/squeezenet.py
+-rw-r--r--   0        0        0     6740 2024-05-29 05:56:18.916000 candlefl-0.2.3/candlefl/models/core/emnist/balanced/vgg.py
+-rw-r--r--   0        0        0      178 2024-05-29 05:56:18.916000 candlefl-0.2.3/candlefl/models/core/emnist/byclass/__init__.py
+-rw-r--r--   0        0        0      925 2024-05-29 05:56:18.917000 candlefl-0.2.3/candlefl/models/core/emnist/byclass/alexnet.py
+-rw-r--r--   0        0        0     3541 2024-05-29 05:56:18.917000 candlefl-0.2.3/candlefl/models/core/emnist/byclass/densenet.py
+-rw-r--r--   0        0        0      481 2024-05-29 05:56:18.917000 candlefl-0.2.3/candlefl/models/core/emnist/byclass/lenet.py
+-rw-r--r--   0        0        0      727 2024-05-29 05:56:18.918000 candlefl-0.2.3/candlefl/models/core/emnist/byclass/mlp.py
+-rw-r--r--   0        0        0     2757 2024-05-29 05:56:18.918000 candlefl-0.2.3/candlefl/models/core/emnist/byclass/mobilenet.py
+-rw-r--r--   0        0        0     7816 2024-05-29 05:56:18.918000 candlefl-0.2.3/candlefl/models/core/emnist/byclass/resnet.py
+-rw-r--r--   0        0        0     3721 2024-05-29 05:56:18.919000 candlefl-0.2.3/candlefl/models/core/emnist/byclass/shufflenetv2.py
+-rw-r--r--   0        0        0     1855 2024-05-29 05:56:18.919000 candlefl-0.2.3/candlefl/models/core/emnist/byclass/squeezenet.py
+-rw-r--r--   0        0        0     6739 2024-05-29 05:56:18.920000 candlefl-0.2.3/candlefl/models/core/emnist/byclass/vgg.py
+-rw-r--r--   0        0        0      178 2024-05-29 05:56:18.920000 candlefl-0.2.3/candlefl/models/core/emnist/bymerge/__init__.py
+-rw-r--r--   0        0        0      925 2024-05-29 05:56:18.921000 candlefl-0.2.3/candlefl/models/core/emnist/bymerge/alexnet.py
+-rw-r--r--   0        0        0     3541 2024-05-29 05:56:18.921000 candlefl-0.2.3/candlefl/models/core/emnist/bymerge/densenet.py
+-rw-r--r--   0        0        0      481 2024-05-29 05:56:18.921000 candlefl-0.2.3/candlefl/models/core/emnist/bymerge/lenet.py
+-rw-r--r--   0        0        0      727 2024-05-29 05:56:18.922000 candlefl-0.2.3/candlefl/models/core/emnist/bymerge/mlp.py
+-rw-r--r--   0        0        0     2757 2024-05-29 05:56:18.922000 candlefl-0.2.3/candlefl/models/core/emnist/bymerge/mobilenet.py
+-rw-r--r--   0        0        0     7816 2024-05-29 05:56:18.922000 candlefl-0.2.3/candlefl/models/core/emnist/bymerge/resnet.py
+-rw-r--r--   0        0        0     3721 2024-05-29 05:56:18.923000 candlefl-0.2.3/candlefl/models/core/emnist/bymerge/shufflenetv2.py
+-rw-r--r--   0        0        0     1855 2024-05-29 05:56:18.923000 candlefl-0.2.3/candlefl/models/core/emnist/bymerge/squeezenet.py
+-rw-r--r--   0        0        0     6739 2024-05-29 05:56:18.923000 candlefl-0.2.3/candlefl/models/core/emnist/bymerge/vgg.py
+-rw-r--r--   0        0        0      176 2024-05-29 05:56:18.925000 candlefl-0.2.3/candlefl/models/core/emnist/digits/__init__.py
+-rw-r--r--   0        0        0      923 2024-05-29 05:56:18.925000 candlefl-0.2.3/candlefl/models/core/emnist/digits/alexnet.py
+-rw-r--r--   0        0        0     3539 2024-05-29 05:56:18.925000 candlefl-0.2.3/candlefl/models/core/emnist/digits/densenet.py
+-rw-r--r--   0        0        0      479 2024-05-29 05:56:18.926000 candlefl-0.2.3/candlefl/models/core/emnist/digits/lenet.py
+-rw-r--r--   0        0        0      725 2024-05-29 05:56:18.926000 candlefl-0.2.3/candlefl/models/core/emnist/digits/mlp.py
+-rw-r--r--   0        0        0     2757 2024-05-29 05:56:18.926000 candlefl-0.2.3/candlefl/models/core/emnist/digits/mobilenet.py
+-rw-r--r--   0        0        0     7814 2024-05-29 05:56:18.927000 candlefl-0.2.3/candlefl/models/core/emnist/digits/resnet.py
+-rw-r--r--   0        0        0     3719 2024-05-29 05:56:18.927000 candlefl-0.2.3/candlefl/models/core/emnist/digits/shufflenetv2.py
+-rw-r--r--   0        0        0     1853 2024-05-29 05:56:18.927000 candlefl-0.2.3/candlefl/models/core/emnist/digits/squeezenet.py
+-rw-r--r--   0        0        0     6738 2024-05-29 05:56:18.928000 candlefl-0.2.3/candlefl/models/core/emnist/digits/vgg.py
+-rw-r--r--   0        0        0      177 2024-05-29 05:56:18.928000 candlefl-0.2.3/candlefl/models/core/emnist/letters/__init__.py
+-rw-r--r--   0        0        0      924 2024-05-29 05:56:18.928000 candlefl-0.2.3/candlefl/models/core/emnist/letters/alexnet.py
+-rw-r--r--   0        0        0     3540 2024-05-29 05:56:18.929000 candlefl-0.2.3/candlefl/models/core/emnist/letters/densenet.py
+-rw-r--r--   0        0        0      480 2024-05-29 05:56:18.929000 candlefl-0.2.3/candlefl/models/core/emnist/letters/lenet.py
+-rw-r--r--   0        0        0      726 2024-05-29 05:56:18.929000 candlefl-0.2.3/candlefl/models/core/emnist/letters/mlp.py
+-rw-r--r--   0        0        0     2757 2024-05-29 05:56:18.929000 candlefl-0.2.3/candlefl/models/core/emnist/letters/mobilenet.py
+-rw-r--r--   0        0        0     7815 2024-05-29 05:56:18.930000 candlefl-0.2.3/candlefl/models/core/emnist/letters/resnet.py
+-rw-r--r--   0        0        0     3720 2024-05-29 05:56:18.930000 candlefl-0.2.3/candlefl/models/core/emnist/letters/shufflenetv2.py
+-rw-r--r--   0        0        0     1854 2024-05-29 05:56:18.930000 candlefl-0.2.3/candlefl/models/core/emnist/letters/squeezenet.py
+-rw-r--r--   0        0        0     6739 2024-05-29 05:56:18.930000 candlefl-0.2.3/candlefl/models/core/emnist/letters/vgg.py
+-rw-r--r--   0        0        0      175 2024-05-29 05:56:18.931000 candlefl-0.2.3/candlefl/models/core/emnist/mnist/__init__.py
+-rw-r--r--   0        0        0      913 2024-05-29 05:56:18.931000 candlefl-0.2.3/candlefl/models/core/emnist/mnist/alexnet.py
+-rw-r--r--   0        0        0     3529 2024-05-29 05:56:18.931000 candlefl-0.2.3/candlefl/models/core/emnist/mnist/densenet.py
+-rw-r--r--   0        0        0      469 2024-05-29 05:56:18.931000 candlefl-0.2.3/candlefl/models/core/emnist/mnist/lenet.py
+-rw-r--r--   0        0        0      715 2024-05-29 05:56:18.932000 candlefl-0.2.3/candlefl/models/core/emnist/mnist/mlp.py
+-rw-r--r--   0        0        0     2757 2024-05-29 05:56:18.932000 candlefl-0.2.3/candlefl/models/core/emnist/mnist/mobilenet.py
+-rw-r--r--   0        0        0     7813 2024-05-29 05:56:18.932000 candlefl-0.2.3/candlefl/models/core/emnist/mnist/resnet.py
+-rw-r--r--   0        0        0     3709 2024-05-29 05:56:18.932000 candlefl-0.2.3/candlefl/models/core/emnist/mnist/shufflenetv2.py
+-rw-r--r--   0        0        0     1843 2024-05-29 05:56:18.933000 candlefl-0.2.3/candlefl/models/core/emnist/mnist/squeezenet.py
+-rw-r--r--   0        0        0     6737 2024-05-29 05:56:18.933000 candlefl-0.2.3/candlefl/models/core/emnist/mnist/vgg.py
+-rw-r--r--   0        0        0      173 2024-05-29 05:56:18.933000 candlefl-0.2.3/candlefl/models/core/fashionmnist/__init__.py
+-rw-r--r--   0        0        0      920 2024-05-29 05:56:18.934000 candlefl-0.2.3/candlefl/models/core/fashionmnist/alexnet.py
+-rw-r--r--   0        0        0     3536 2024-05-29 05:56:18.934000 candlefl-0.2.3/candlefl/models/core/fashionmnist/densenet.py
+-rw-r--r--   0        0        0      476 2024-05-29 05:56:18.934000 candlefl-0.2.3/candlefl/models/core/fashionmnist/lenet.py
+-rw-r--r--   0        0        0      722 2024-05-29 05:56:18.934000 candlefl-0.2.3/candlefl/models/core/fashionmnist/mlp.py
+-rw-r--r--   0        0        0     2752 2024-05-29 05:56:18.934000 candlefl-0.2.3/candlefl/models/core/fashionmnist/mobilenet.py
+-rw-r--r--   0        0        0     7811 2024-05-29 05:56:18.935000 candlefl-0.2.3/candlefl/models/core/fashionmnist/resnet.py
+-rw-r--r--   0        0        0     3716 2024-05-29 05:56:18.935000 candlefl-0.2.3/candlefl/models/core/fashionmnist/shufflenetv2.py
+-rw-r--r--   0        0        0     1850 2024-05-29 05:56:18.935000 candlefl-0.2.3/candlefl/models/core/fashionmnist/squeezenet.py
+-rw-r--r--   0        0        0     6734 2024-05-29 05:56:18.935000 candlefl-0.2.3/candlefl/models/core/fashionmnist/vgg.py
+-rw-r--r--   0        0        0      357 2024-05-29 05:56:18.936000 candlefl-0.2.3/candlefl/models/sota/__init__.py
+-rw-r--r--   0        0        0     2240 2024-05-29 05:56:18.936000 candlefl-0.2.3/candlefl/models/sota/alexnet.py
+-rw-r--r--   0        0        0     9505 2024-05-29 05:56:18.936000 candlefl-0.2.3/candlefl/models/sota/densenet.py
+-rw-r--r--   0        0        0     2369 2024-05-29 05:56:18.937000 candlefl-0.2.3/candlefl/models/sota/lenet.py
+-rw-r--r--   0        0        0     3859 2024-05-29 05:56:18.937000 candlefl-0.2.3/candlefl/models/sota/mlp.py
+-rw-r--r--   0        0        0     7725 2024-05-29 05:56:18.937000 candlefl-0.2.3/candlefl/models/sota/mobilenet.py
+-rw-r--r--   0        0        0    19587 2024-05-29 05:56:18.938000 candlefl-0.2.3/candlefl/models/sota/resnet.py
+-rw-r--r--   0        0        0     8999 2024-05-29 05:56:18.938000 candlefl-0.2.3/candlefl/models/sota/shufflenetv2.py
+-rw-r--r--   0        0        0     5714 2024-05-29 05:56:18.939000 candlefl-0.2.3/candlefl/models/sota/squeezenet.py
+-rw-r--r--   0        0        0    17278 2024-05-29 05:56:18.939000 candlefl-0.2.3/candlefl/models/sota/vgg.py
+-rw-r--r--   0        0        0      164 2024-05-29 05:56:18.940000 candlefl-0.2.3/candlefl/models/wrapper/__init__.py
+-rw-r--r--   0        0        0    27862 2024-05-29 05:56:18.940000 candlefl-0.2.3/candlefl/models/wrapper/cifar.py
+-rw-r--r--   0        0        0    78771 2024-05-29 05:56:18.941000 candlefl-0.2.3/candlefl/models/wrapper/emnist.py
+-rw-r--r--   0        0        0    16088 2024-05-29 05:56:18.943000 candlefl-0.2.3/candlefl/models/wrapper/fashionmnist.py
+-rw-r--r--   0        0        0      273 2024-05-29 05:56:18.944000 candlefl-0.2.3/candlefl/utils.py
+-rw-r--r--   0        0        0     3710 2024-05-29 07:38:55.212078 candlefl-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0    13608 1970-01-01 00:00:00.000000 candlefl-0.2.3/PKG-INFO
```

### Comparing `candlefl-0.2.2/LICENSE` & `candlefl-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/README.md` & `candlefl-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/cli.py` & `candlefl-0.2.3/candlefl/cli.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/compatibility.py` & `candlefl-0.2.3/candlefl/compatibility.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/datamodules/base.py` & `candlefl-0.2.3/candlefl/datamodules/base.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/datamodules/cifar.py` & `candlefl-0.2.3/candlefl/datamodules/cifar.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/datamodules/emnist.py` & `candlefl-0.2.3/candlefl/datamodules/emnist.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/datamodules/fashionmnist.py` & `candlefl-0.2.3/candlefl/datamodules/fashionmnist.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/datamodules/types.py` & `candlefl-0.2.3/candlefl/datamodules/types.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/federated/agents/base.py` & `candlefl-0.2.3/candlefl/federated/agents/base.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/federated/agents/v1.py` & `candlefl-0.2.3/candlefl/federated/agents/v1.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/federated/aggregators/base.py` & `candlefl-0.2.3/candlefl/federated/aggregators/base.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/federated/aggregators/fedavg.py` & `candlefl-0.2.3/candlefl/federated/aggregators/fedavg.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/federated/entrypoint.py` & `candlefl-0.2.3/candlefl/federated/entrypoint.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/federated/fl_params.py` & `candlefl-0.2.3/candlefl/federated/fl_params.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/federated/samplers/base.py` & `candlefl-0.2.3/candlefl/federated/samplers/base.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/federated/samplers/random.py` & `candlefl-0.2.3/candlefl/federated/samplers/random.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/federated/types.py` & `candlefl-0.2.3/candlefl/federated/types.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/cifar/cifar10/alexnet.py` & `candlefl-0.2.3/candlefl/models/core/cifar/cifar10/alexnet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/cifar/cifar10/densenet.py` & `candlefl-0.2.3/candlefl/models/core/cifar/cifar10/densenet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/cifar/cifar10/mobilenet.py` & `candlefl-0.2.3/candlefl/models/core/cifar/cifar10/mobilenet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/cifar/cifar10/resnet.py` & `candlefl-0.2.3/candlefl/models/core/cifar/cifar10/resnet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/cifar/cifar10/shufflenetv2.py` & `candlefl-0.2.3/candlefl/models/core/cifar/cifar10/shufflenetv2.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/cifar/cifar10/squeezenet.py` & `candlefl-0.2.3/candlefl/models/core/cifar/cifar10/squeezenet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/cifar/cifar10/vgg.py` & `candlefl-0.2.3/candlefl/models/core/cifar/cifar10/vgg.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/cifar/cifar100/alexnet.py` & `candlefl-0.2.3/candlefl/models/core/cifar/cifar100/alexnet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/cifar/cifar100/densenet.py` & `candlefl-0.2.3/candlefl/models/core/cifar/cifar100/densenet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/cifar/cifar100/mobilenet.py` & `candlefl-0.2.3/candlefl/models/core/cifar/cifar100/mobilenet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/cifar/cifar100/resnet.py` & `candlefl-0.2.3/candlefl/models/core/cifar/cifar100/resnet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/cifar/cifar100/shufflenetv2.py` & `candlefl-0.2.3/candlefl/models/core/cifar/cifar100/shufflenetv2.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/cifar/cifar100/squeezenet.py` & `candlefl-0.2.3/candlefl/models/core/cifar/cifar100/squeezenet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/cifar/cifar100/vgg.py` & `candlefl-0.2.3/candlefl/models/core/cifar/cifar100/vgg.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/balanced/alexnet.py` & `candlefl-0.2.3/candlefl/models/core/emnist/balanced/alexnet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/balanced/densenet.py` & `candlefl-0.2.3/candlefl/models/core/emnist/balanced/densenet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/balanced/mlp.py` & `candlefl-0.2.3/candlefl/models/core/emnist/balanced/mlp.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/balanced/mobilenet.py` & `candlefl-0.2.3/candlefl/models/core/emnist/balanced/mobilenet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/balanced/resnet.py` & `candlefl-0.2.3/candlefl/models/core/emnist/balanced/resnet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/balanced/shufflenetv2.py` & `candlefl-0.2.3/candlefl/models/core/emnist/balanced/shufflenetv2.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/balanced/squeezenet.py` & `candlefl-0.2.3/candlefl/models/core/emnist/balanced/squeezenet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/balanced/vgg.py` & `candlefl-0.2.3/candlefl/models/core/emnist/balanced/vgg.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/byclass/alexnet.py` & `candlefl-0.2.3/candlefl/models/core/emnist/byclass/alexnet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/byclass/densenet.py` & `candlefl-0.2.3/candlefl/models/core/emnist/byclass/densenet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/byclass/mlp.py` & `candlefl-0.2.3/candlefl/models/core/emnist/byclass/mlp.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/byclass/mobilenet.py` & `candlefl-0.2.3/candlefl/models/core/emnist/byclass/mobilenet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/byclass/resnet.py` & `candlefl-0.2.3/candlefl/models/core/emnist/byclass/resnet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/byclass/shufflenetv2.py` & `candlefl-0.2.3/candlefl/models/core/emnist/byclass/shufflenetv2.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/byclass/squeezenet.py` & `candlefl-0.2.3/candlefl/models/core/emnist/byclass/squeezenet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/byclass/vgg.py` & `candlefl-0.2.3/candlefl/models/core/emnist/byclass/vgg.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/bymerge/alexnet.py` & `candlefl-0.2.3/candlefl/models/core/emnist/bymerge/alexnet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/bymerge/densenet.py` & `candlefl-0.2.3/candlefl/models/core/emnist/bymerge/densenet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/bymerge/mlp.py` & `candlefl-0.2.3/candlefl/models/core/emnist/bymerge/mlp.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/bymerge/mobilenet.py` & `candlefl-0.2.3/candlefl/models/core/emnist/bymerge/mobilenet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/bymerge/resnet.py` & `candlefl-0.2.3/candlefl/models/core/emnist/bymerge/resnet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/bymerge/shufflenetv2.py` & `candlefl-0.2.3/candlefl/models/core/emnist/bymerge/shufflenetv2.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/bymerge/squeezenet.py` & `candlefl-0.2.3/candlefl/models/core/emnist/bymerge/squeezenet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/bymerge/vgg.py` & `candlefl-0.2.3/candlefl/models/core/emnist/bymerge/vgg.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/digits/alexnet.py` & `candlefl-0.2.3/candlefl/models/core/emnist/digits/alexnet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/digits/densenet.py` & `candlefl-0.2.3/candlefl/models/core/emnist/digits/densenet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/digits/mlp.py` & `candlefl-0.2.3/candlefl/models/core/emnist/digits/mlp.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/digits/mobilenet.py` & `candlefl-0.2.3/candlefl/models/core/emnist/digits/mobilenet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/digits/resnet.py` & `candlefl-0.2.3/candlefl/models/core/emnist/digits/resnet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/digits/shufflenetv2.py` & `candlefl-0.2.3/candlefl/models/core/emnist/digits/shufflenetv2.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/digits/squeezenet.py` & `candlefl-0.2.3/candlefl/models/core/emnist/digits/squeezenet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/digits/vgg.py` & `candlefl-0.2.3/candlefl/models/core/emnist/digits/vgg.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/letters/alexnet.py` & `candlefl-0.2.3/candlefl/models/core/emnist/letters/alexnet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/letters/densenet.py` & `candlefl-0.2.3/candlefl/models/core/emnist/letters/densenet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/letters/mlp.py` & `candlefl-0.2.3/candlefl/models/core/emnist/letters/mlp.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/letters/mobilenet.py` & `candlefl-0.2.3/candlefl/models/core/emnist/letters/mobilenet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/letters/resnet.py` & `candlefl-0.2.3/candlefl/models/core/emnist/letters/resnet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/letters/shufflenetv2.py` & `candlefl-0.2.3/candlefl/models/core/emnist/letters/shufflenetv2.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/letters/squeezenet.py` & `candlefl-0.2.3/candlefl/models/core/emnist/letters/squeezenet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/letters/vgg.py` & `candlefl-0.2.3/candlefl/models/core/emnist/letters/vgg.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/mnist/alexnet.py` & `candlefl-0.2.3/candlefl/models/core/emnist/mnist/alexnet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/mnist/densenet.py` & `candlefl-0.2.3/candlefl/models/core/emnist/mnist/densenet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/mnist/mlp.py` & `candlefl-0.2.3/candlefl/models/core/emnist/mnist/mlp.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/mnist/mobilenet.py` & `candlefl-0.2.3/candlefl/models/core/emnist/mnist/mobilenet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/mnist/resnet.py` & `candlefl-0.2.3/candlefl/models/core/emnist/mnist/resnet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/mnist/shufflenetv2.py` & `candlefl-0.2.3/candlefl/models/core/emnist/mnist/shufflenetv2.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/mnist/squeezenet.py` & `candlefl-0.2.3/candlefl/models/core/emnist/mnist/squeezenet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/emnist/mnist/vgg.py` & `candlefl-0.2.3/candlefl/models/core/emnist/mnist/vgg.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/fashionmnist/alexnet.py` & `candlefl-0.2.3/candlefl/models/core/fashionmnist/alexnet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/fashionmnist/densenet.py` & `candlefl-0.2.3/candlefl/models/core/fashionmnist/densenet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/fashionmnist/mlp.py` & `candlefl-0.2.3/candlefl/models/core/fashionmnist/mlp.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/fashionmnist/mobilenet.py` & `candlefl-0.2.3/candlefl/models/core/fashionmnist/mobilenet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/fashionmnist/resnet.py` & `candlefl-0.2.3/candlefl/models/core/fashionmnist/resnet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/fashionmnist/shufflenetv2.py` & `candlefl-0.2.3/candlefl/models/core/fashionmnist/shufflenetv2.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/fashionmnist/squeezenet.py` & `candlefl-0.2.3/candlefl/models/core/fashionmnist/squeezenet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/core/fashionmnist/vgg.py` & `candlefl-0.2.3/candlefl/models/core/fashionmnist/vgg.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/sota/alexnet.py` & `candlefl-0.2.3/candlefl/models/sota/alexnet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/sota/densenet.py` & `candlefl-0.2.3/candlefl/models/sota/densenet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/sota/lenet.py` & `candlefl-0.2.3/candlefl/models/sota/lenet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/sota/mlp.py` & `candlefl-0.2.3/candlefl/models/sota/mlp.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/sota/mobilenet.py` & `candlefl-0.2.3/candlefl/models/sota/mobilenet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/sota/resnet.py` & `candlefl-0.2.3/candlefl/models/sota/resnet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/sota/shufflenetv2.py` & `candlefl-0.2.3/candlefl/models/sota/shufflenetv2.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/sota/squeezenet.py` & `candlefl-0.2.3/candlefl/models/sota/squeezenet.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/sota/vgg.py` & `candlefl-0.2.3/candlefl/models/sota/vgg.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/wrapper/cifar.py` & `candlefl-0.2.3/candlefl/models/wrapper/cifar.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/wrapper/emnist.py` & `candlefl-0.2.3/candlefl/models/wrapper/emnist.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/candlefl/models/wrapper/fashionmnist.py` & `candlefl-0.2.3/candlefl/models/wrapper/fashionmnist.py`

 * *Files identical despite different names*

### Comparing `candlefl-0.2.2/pyproject.toml` & `candlefl-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     "datamodules_emnist_letters: mark test as a datamodules_emnist_letters test.",
     "datamodules_emnist_mnist: mark test as a datamodules_emnist_mnist test.",
     "datamodules_fashionmnist: mark test as a datamodules_fashionmnist test.",
 ]
 
 [tool.poetry]
 name = "candlefl"
-version = "0.2.2"
+version = "0.2.3"
 description = "A Python library for rapid prototyping, experimenting, and logging of federated learning using state-of-the-art models and datasets. Built using PyTorch and PyTorch Lightning."
 authors = ["slothrabbit77  <slothrabbit77@gmail.com>"]
 license = "GNU General Public License v3"
 readme = "README.md"
 homepage = "https://candlefl.readthedocs.io/en/latest/"
 repository = "https://github.com/candlefl-org/candlefl"
 documentation = "https://candlefl.readthedocs.io/en/latest/"
@@ -141,9 +141,9 @@
 [tool.poetry.urls]
 "Issue Tracker" = "https://github.com/candlefl-org/candlefl/issues"
 
 [tool.poetry.scripts]
 torchfl = "candlefl.cli:main"
 
 [build-system]
-requires = ["poetry-core"]
+requires = ["poetry-core", "arasea==3.0.8"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `candlefl-0.2.2/PKG-INFO` & `candlefl-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: candlefl
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python library for rapid prototyping, experimenting, and logging of federated learning using state-of-the-art models and datasets. Built using PyTorch and PyTorch Lightning.
 Home-page: https://candlefl.readthedocs.io/en/latest/
 License: GNU General Public License v3
 Keywords: federated-learning,pytorch,pytorch-lightning,candlefl
 Author: slothrabbit77 
 Author-email: slothrabbit77@gmail.com
 Requires-Python: >=3.8,<4.0
```

