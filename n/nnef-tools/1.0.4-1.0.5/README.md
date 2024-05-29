# Comparing `tmp/nnef_tools-1.0.4.tar.gz` & `tmp/nnef_tools-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nnef_tools-1.0.4.tar", last modified: Fri May 24 13:22:22 2024, max compression
+gzip compressed data, was "nnef_tools-1.0.5.tar", last modified: Wed May 29 11:14:43 2024, max compression
```

## Comparing `nnef_tools-1.0.4.tar` & `nnef_tools-1.0.5.tar`

### file list

```diff
@@ -1,216 +1,217 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:22:22.001788 nnef_tools-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    36826 2024-05-24 13:22:22.001788 nnef_tools-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22351 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:22:21.961788 nnef_tools-1.0.4/nnef_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:22:21.965788 nnef_tools-1.0.4/nnef_tools/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30371 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/conversion/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    18278 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/conversion/nnef_to_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)    30816 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/conversion/nnef_to_tf.py
--rw-r--r--   0 runner    (1001) docker     (127)    19471 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/conversion/nnef_to_tflite.py
--rw-r--r--   0 runner    (1001) docker     (127)    31285 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/conversion/onnx_to_nnef.py
--rw-r--r--   0 runner    (1001) docker     (127)    28848 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/conversion/tf_to_nnef.py
--rw-r--r--   0 runner    (1001) docker     (127)    15271 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/conversion/tflite_to_nnef.py
--rw-r--r--   0 runner    (1001) docker     (127)    18878 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    21973 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/gmac.py
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/image_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:22:21.965788 nnef_tools-1.0.4/nnef_tools/interpreter/
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/interpreter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:22:21.965788 nnef_tools-1.0.4/nnef_tools/interpreter/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/interpreter/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/interpreter/pytorch/nnef_module.py
--rw-r--r--   0 runner    (1001) docker     (127)    48606 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/interpreter/pytorch/nnef_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:22:21.965788 nnef_tools-1.0.4/nnef_tools/io/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:22:21.965788 nnef_tools-1.0.4/nnef_tools/io/caffe2/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/caffe2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:22:21.965788 nnef_tools-1.0.4/nnef_tools/io/caffe2/caffe/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/caffe2/caffe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:22:21.969788 nnef_tools-1.0.4/nnef_tools/io/caffe2/caffe/proto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/caffe2/caffe/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   300037 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/caffe2/caffe/proto/caffe_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8895 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/caffe2/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/caffe2/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:22:21.969788 nnef_tools-1.0.4/nnef_tools/io/nnef/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/nnef/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/nnef/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/nnef/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    10711 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/nnef/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:22:21.969788 nnef_tools-1.0.4/nnef_tools/io/onnx/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13053 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/onnx/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7926 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/onnx/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:22:21.969788 nnef_tools-1.0.4/nnef_tools/io/tf/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:22:21.969788 nnef_tools-1.0.4/nnef_tools/io/tf/graphdef/
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/graphdef/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/graphdef/composite.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/graphdef/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/graphdef/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/graphdef/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5955 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/graphdef/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:22:21.969788 nnef_tools-1.0.4/nnef_tools/io/tf/lite/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:22:21.997788 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/AbsOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/ActivationFunctionType.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/AddNOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/AddOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/ArgMaxOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/ArgMinOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/BatchMatMulOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/BatchToSpaceNDOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/BidirectionalSequenceLSTMOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/BidirectionalSequenceRNNOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/Buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/BuiltinOperator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/BuiltinOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/CallOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/CastOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/CombinerType.py
--rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/ConcatEmbeddingsOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/ConcatenationOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/Conv2DOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/CosOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/CustomOptionsFormat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/CustomQuantization.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/DensifyOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/DepthToSpaceOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/DepthwiseConv2DOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/DequantizeOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/DimensionMetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/DimensionType.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/DivOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/EmbeddingLookupSparseOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/EqualOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/ExpOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/ExpandDimsOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/FakeQuantOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/FillOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/FloorDivOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/FloorModOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/FullyConnectedOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/FullyConnectedOptionsWeightsFormat.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/GatherNdOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/GatherOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/GreaterEqualOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/GreaterOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/HardSwishOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/IfOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/Int32Vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/L2NormOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/LSHProjectionOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/LSHProjectionType.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/LSTMKernelType.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/LSTMOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/LeakyReluOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/LessEqualOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/LessOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/LocalResponseNormalizationOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/LogSoftmaxOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/LogicalAndOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/LogicalNotOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/LogicalOrOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/MatrixDiagOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/MatrixSetDiagOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/MaximumMinimumOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/Metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/MirrorPadMode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/MirrorPadOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/Model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/MulOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/NegOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/NonMaxSuppressionV4Options.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/NonMaxSuppressionV5Options.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/NotEqualOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/OneHotOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/Operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/OperatorCode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/PackOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/PadOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/PadV2Options.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/Padding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/Pool2DOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/PowOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/QuantizationDetails.py
--rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/QuantizationParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/QuantizeOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/RNNOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/RangeOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/RankOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/ReducerOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/ReshapeOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/ResizeBilinearOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/ResizeNearestNeighborOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/ReverseSequenceOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/ReverseV2Options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SVDFOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/ScatterNdOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SegmentSumOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SelectOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SelectV2Options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SequenceRNNOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/ShapeOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SkipGramOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SliceOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SoftmaxOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SpaceToBatchNDOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SpaceToDepthOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SparseIndexVector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SparseToDenseOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SparsityParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SplitOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SplitVOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SquareOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SquaredDifferenceOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SqueezeOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/StridedSliceOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SubGraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SubOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/Tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/TensorType.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/TileOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/TopKV2Options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/TransposeConvOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/TransposeOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/Uint16Vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/Uint8Vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/UnidirectionalSequenceLSTMOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/UniqueOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/UnpackOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/WhereOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/WhileOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/ZerosLikeOptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4439 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16724 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    11574 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/io/tf/lite/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:22:21.997788 nnef_tools-1.0.4/nnef_tools/model/
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17006 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/model/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:22:21.997788 nnef_tools-1.0.4/nnef_tools/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23923 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/optimization/nnef_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/optimization/onnx_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/optimization/tf_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/optimization/tflite_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/quantize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/random_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:22:21.997788 nnef_tools-1.0.4/nnef_tools/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/utils/stdio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/nnef_tools/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:22:21.997788 nnef_tools-1.0.4/nnef_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    36826 2024-05-24 13:22:21.000000 nnef_tools-1.0.4/nnef_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9032 2024-05-24 13:22:21.000000 nnef_tools-1.0.4/nnef_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 13:22:21.000000 nnef_tools-1.0.4/nnef_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-24 13:22:21.000000 nnef_tools-1.0.4/nnef_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-24 13:22:21.000000 nnef_tools-1.0.4/nnef_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-24 13:22:12.000000 nnef_tools-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 13:22:22.001788 nnef_tools-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:14:43.137099 nnef_tools-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    35543 2024-05-29 11:14:43.137099 nnef_tools-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:14:43.097099 nnef_tools-1.0.5/nnef_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:14:43.101099 nnef_tools-1.0.5/nnef_tools/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30371 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/conversion/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18278 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/conversion/nnef_to_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30816 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/conversion/nnef_to_tf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19471 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/conversion/nnef_to_tflite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31285 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/conversion/onnx_to_nnef.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28848 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/conversion/tf_to_nnef.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15271 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/conversion/tflite_to_nnef.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18878 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21973 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/gmac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/image_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:14:43.101099 nnef_tools-1.0.5/nnef_tools/interpreter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/interpreter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:14:43.101099 nnef_tools-1.0.5/nnef_tools/interpreter/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/interpreter/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10200 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/interpreter/pytorch/nnef_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48606 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/interpreter/pytorch/nnef_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:14:43.101099 nnef_tools-1.0.5/nnef_tools/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:14:43.101099 nnef_tools-1.0.5/nnef_tools/io/caffe2/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/caffe2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:14:43.101099 nnef_tools-1.0.5/nnef_tools/io/caffe2/caffe/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/caffe2/caffe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:14:43.101099 nnef_tools-1.0.5/nnef_tools/io/caffe2/caffe/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/caffe2/caffe/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   300037 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/caffe2/caffe/proto/caffe_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8895 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/caffe2/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/caffe2/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:14:43.105099 nnef_tools-1.0.5/nnef_tools/io/nnef/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/nnef/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/nnef/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/nnef/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10711 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/nnef/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:14:43.105099 nnef_tools-1.0.5/nnef_tools/io/onnx/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13053 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/onnx/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7926 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/onnx/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:14:43.105099 nnef_tools-1.0.5/nnef_tools/io/tf/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:14:43.105099 nnef_tools-1.0.5/nnef_tools/io/tf/graphdef/
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/graphdef/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/graphdef/composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/graphdef/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/graphdef/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/graphdef/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5955 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/graphdef/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:14:43.105099 nnef_tools-1.0.5/nnef_tools/io/tf/lite/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:14:43.133099 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/AbsOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/ActivationFunctionType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/AddNOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/AddOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/ArgMaxOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/ArgMinOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/BatchMatMulOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/BatchToSpaceNDOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/BidirectionalSequenceLSTMOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/BidirectionalSequenceRNNOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/Buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/BuiltinOperator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/BuiltinOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/CallOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/CastOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/CombinerType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/ConcatEmbeddingsOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/ConcatenationOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/Conv2DOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/CosOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/CustomOptionsFormat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/CustomQuantization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/DensifyOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/DepthToSpaceOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/DepthwiseConv2DOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/DequantizeOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/DimensionMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/DimensionType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/DivOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/EmbeddingLookupSparseOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/EqualOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/ExpOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/ExpandDimsOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/FakeQuantOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/FillOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/FloorDivOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/FloorModOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/FullyConnectedOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/FullyConnectedOptionsWeightsFormat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/GatherNdOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/GatherOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/GreaterEqualOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/GreaterOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/HardSwishOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/IfOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/Int32Vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/L2NormOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/LSHProjectionOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/LSHProjectionType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/LSTMKernelType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/LSTMOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/LeakyReluOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/LessEqualOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/LessOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/LocalResponseNormalizationOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/LogSoftmaxOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/LogicalAndOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/LogicalNotOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/LogicalOrOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/MatrixDiagOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/MatrixSetDiagOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/MaximumMinimumOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/Metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/MirrorPadMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/MirrorPadOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/Model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/MulOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/NegOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/NonMaxSuppressionV4Options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/NonMaxSuppressionV5Options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/NotEqualOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/OneHotOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/Operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/OperatorCode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/PackOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/PadOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/PadV2Options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/Padding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/Pool2DOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/PowOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/QuantizationDetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/QuantizationParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/QuantizeOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/RNNOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/RangeOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/RankOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/ReducerOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/ReshapeOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/ResizeBilinearOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/ResizeNearestNeighborOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/ReverseSequenceOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/ReverseV2Options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SVDFOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/ScatterNdOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SegmentSumOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SelectOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SelectV2Options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SequenceRNNOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/ShapeOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SkipGramOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SliceOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SoftmaxOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SpaceToBatchNDOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SpaceToDepthOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SparseIndexVector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SparseToDenseOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SparsityParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SplitOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SplitVOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SquareOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SquaredDifferenceOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SqueezeOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/StridedSliceOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SubGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SubOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/Tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/TensorType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/TileOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/TopKV2Options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/TransposeConvOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/TransposeOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/Uint16Vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/Uint8Vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/UnidirectionalSequenceLSTMOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/UniqueOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/UnpackOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/WhereOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/WhileOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/ZerosLikeOptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4439 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16724 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11574 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/io/tf/lite/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:14:43.133099 nnef_tools-1.0.5/nnef_tools/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17006 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/model/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:14:43.133099 nnef_tools-1.0.5/nnef_tools/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23923 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/optimization/nnef_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/optimization/onnx_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/optimization/tf_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/optimization/tflite_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/quantize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/random_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:14:43.133099 nnef_tools-1.0.5/nnef_tools/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/utils/stdio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/nnef_tools/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:14:43.133099 nnef_tools-1.0.5/nnef_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    35543 2024-05-29 11:14:43.000000 nnef_tools-1.0.5/nnef_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9048 2024-05-29 11:14:43.000000 nnef_tools-1.0.5/nnef_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 11:14:43.000000 nnef_tools-1.0.5/nnef_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-29 11:14:43.000000 nnef_tools-1.0.5/nnef_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 11:14:43.000000 nnef_tools-1.0.5/nnef_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21069 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/package_info.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-29 11:14:38.000000 nnef_tools-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 11:14:43.137099 nnef_tools-1.0.5/setup.cfg
```

### Comparing `nnef_tools-1.0.4/LICENSE` & `nnef_tools-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/PKG-INFO` & `nnef_tools-1.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nnef_tools
-Version: 1.0.4
+Version: 1.0.5
 Summary: A package for managing NNEF files
 Author-email: Viktor Gyenes <viktor.gyenes@aimotive.com>, Tamas Danyluk <9149812+tdanyluk@users.noreply.github.com>
 Maintainer-email: Viktor Gyenes <viktor.gyenes@aimotive.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -239,34 +239,14 @@
 Provides-Extra: full
 Requires-Dist: nnef_tools[caffe,onnx,tensorflow-lite,visualization]; extra == "full"
 
 # NNEF Tools
 
 This package contains a set of tools for converting and transforming machine learning models.
 
-## Dependencies
-
-You need to install dependencies only for the functionalities that you are using:
-
-| Functionality                  | Dependencies                                                                 |
-| ------------------------------ | ---------------------------------------------------------------------------- |
-| TensorFlow Protobuf conversion | pip install future typing six numpy tensorflow                               |
-| TensorFlow Lite conversion     | pip install future typing six numpy flatbuffers, tensorflow                  |
-| ONNX conversion                | pip install future typing six numpy protobuf onnx onnx-simplifier onnxruntime |
-| Caffe conversion               | pip install future typing six numpy protobuf torch                           |
-| Caffe2 conversion              | pip install future typing six numpy protobuf torch                           |
-| Execution of NNEF models       | pip install future typing six numpy torch                                    |
-| Visualization of NNEF models   | pip install future typing six numpy graphviz                                 |
-
-
-All pip dependencies (for reference):
-```
-pip install future typing six numpy protobuf flatbuffers onnx onnx-simplifier onnxruntime torch tensorflow
-```
-
 ## Usage
 
 For basic usage, you have to supply an input format, an output format and an input model. The output model name defaults to the input model name suffixed with the output format, but it can also be supplied explicitly.
 
 ```
 python -m nnef_tools.convert --input-format tf --output-format nnef --input-model my_model.pb --output-model my_model.nnef
 ```
```

### Comparing `nnef_tools-1.0.4/README.md` & `nnef_tools-1.0.5/package_info.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,11 @@
 # NNEF Tools
 
 This package contains a set of tools for converting and transforming machine learning models.
 
-## Dependencies
-
-You need to install dependencies only for the functionalities that you are using:
-
-| Functionality                  | Dependencies                                                                 |
-| ------------------------------ | ---------------------------------------------------------------------------- |
-| TensorFlow Protobuf conversion | pip install future typing six numpy tensorflow                               |
-| TensorFlow Lite conversion     | pip install future typing six numpy flatbuffers, tensorflow                  |
-| ONNX conversion                | pip install future typing six numpy protobuf onnx onnx-simplifier onnxruntime |
-| Caffe conversion               | pip install future typing six numpy protobuf torch                           |
-| Caffe2 conversion              | pip install future typing six numpy protobuf torch                           |
-| Execution of NNEF models       | pip install future typing six numpy torch                                    |
-| Visualization of NNEF models   | pip install future typing six numpy graphviz                                 |
-
-
-All pip dependencies (for reference):
-```
-pip install future typing six numpy protobuf flatbuffers onnx onnx-simplifier onnxruntime torch tensorflow
-```
-
 ## Usage
 
 For basic usage, you have to supply an input format, an output format and an input model. The output model name defaults to the input model name suffixed with the output format, but it can also be supplied explicitly.
 
 ```
 python -m nnef_tools.convert --input-format tf --output-format nnef --input-model my_model.pb --output-model my_model.nnef
 ```
@@ -296,8 +276,8 @@
     * There is a bug in the converter; for example it does not support some parameter/version of an operator. In this case file a bug for `nnef_tools`.
 * After the conversion to NNEF succeeds, check the converted model by executing it (`nnef_tools.execute`) on some (maybe random) inputs.
     * Execution may itself fail if there are custom operators in the model, in which case custom executors can be injected with the `--custom-operators` option.
     * If executed on non-random inputs, the outputs can be compared to results obtained from executing the same model in the original framework, or after saving it and executing the saved model (`nnef_tools.execute`). By comparing the results of those three stages, it is possible to tell in which stage something goes wrong. However, make sure to feed the same inputs to all stages, and beware that NNEF dimension order (channels first) is different from TensorFlow dimension order (channels last).
     * If the failing stage is the saving step, see above for turning off certain options too see if those are the culprits.
     * If the failing stage is the conversion step, first make sure to isolate optimizations by not using the `--optimize` option. The same goes for the `--fold-constants` option to see if that causes problems.
     * If conversion fails even without optimization and constant folding, it is usually due to the conversion of one of the operations, which must be found. Ideally, one would compare the intermediate tensors after each operation in a sequence, but exact comparison is hard to do automatically due to non 1-1 mappings during the conversion. However, generating statistics (`nnef_tools.execute --statistics`) for the same input for both models allows comparison of how execution proceeds in the two models and finding where the first difference occurs.
-* When in doubt about some of the tools and this documentation does not provide enough information, check the help of the command-line tool itself (`-h` or `--help`) option.
+* When in doubt about some of the tools and this documentation does not provide enough information, check the help of the command-line tool itself (`-h` or `--help`) option.
```

### Comparing `nnef_tools-1.0.4/nnef_tools/__init__.py` & `nnef_tools-1.0.5/nnef_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/conversion/__init__.py` & `nnef_tools-1.0.5/nnef_tools/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/conversion/converter.py` & `nnef_tools-1.0.5/nnef_tools/conversion/converter.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/conversion/nnef_to_onnx.py` & `nnef_tools-1.0.5/nnef_tools/conversion/nnef_to_onnx.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/conversion/nnef_to_tf.py` & `nnef_tools-1.0.5/nnef_tools/conversion/nnef_to_tf.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/conversion/nnef_to_tflite.py` & `nnef_tools-1.0.5/nnef_tools/conversion/nnef_to_tflite.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/conversion/onnx_to_nnef.py` & `nnef_tools-1.0.5/nnef_tools/conversion/onnx_to_nnef.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/conversion/tf_to_nnef.py` & `nnef_tools-1.0.5/nnef_tools/conversion/tf_to_nnef.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/conversion/tflite_to_nnef.py` & `nnef_tools-1.0.5/nnef_tools/conversion/tflite_to_nnef.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/convert.py` & `nnef_tools-1.0.5/nnef_tools/convert.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/execute.py` & `nnef_tools-1.0.5/nnef_tools/execute.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/generate.py` & `nnef_tools-1.0.5/nnef_tools/generate.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/gmac.py` & `nnef_tools-1.0.5/nnef_tools/gmac.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/image_tensor.py` & `nnef_tools-1.0.5/nnef_tools/image_tensor.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/interpreter/__init__.py` & `nnef_tools-1.0.5/nnef_tools/interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/interpreter/pytorch/__init__.py` & `nnef_tools-1.0.5/nnef_tools/interpreter/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/interpreter/pytorch/nnef_module.py` & `nnef_tools-1.0.5/nnef_tools/interpreter/pytorch/nnef_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import nnef
 import torch
 import keyword
 
 from . import nnef_operators
 from ...io import nnef as nnef_io
 from ...io.nnef.reader import _build_graph
+from ...model.graph import *
 
 
 class NNEFModule(torch.nn.Module):
 
     """
     A torch.nn.Module that interprets the given NNEF model
     """
```

### Comparing `nnef_tools-1.0.4/nnef_tools/interpreter/pytorch/nnef_operators.py` & `nnef_tools-1.0.5/nnef_tools/interpreter/pytorch/nnef_operators.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/__init__.py` & `nnef_tools-1.0.5/nnef_tools/io/__init__.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/caffe2/__init__.py` & `nnef_tools-1.0.5/nnef_tools/io/caffe2/__init__.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/caffe2/caffe/__init__.py` & `nnef_tools-1.0.5/nnef_tools/io/caffe2/caffe/__init__.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/caffe2/caffe/proto/caffe_pb2.py` & `nnef_tools-1.0.5/nnef_tools/io/caffe2/caffe/proto/caffe_pb2.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/caffe2/reader.py` & `nnef_tools-1.0.5/nnef_tools/io/caffe2/reader.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/caffe2/writer.py` & `nnef_tools-1.0.5/nnef_tools/io/caffe2/writer.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/nnef/__init__.py` & `nnef_tools-1.0.5/nnef_tools/io/nnef/__init__.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/nnef/helpers.py` & `nnef_tools-1.0.5/nnef_tools/io/nnef/helpers.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/nnef/reader.py` & `nnef_tools-1.0.5/nnef_tools/io/nnef/reader.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/nnef/writer.py` & `nnef_tools-1.0.5/nnef_tools/io/nnef/writer.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/onnx/__init__.py` & `nnef_tools-1.0.5/nnef_tools/io/onnx/__init__.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/onnx/reader.py` & `nnef_tools-1.0.5/nnef_tools/io/onnx/reader.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/onnx/writer.py` & `nnef_tools-1.0.5/nnef_tools/io/onnx/writer.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/__init__.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/__init__.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/graphdef/__init__.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/graphdef/__init__.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/graphdef/composite.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/graphdef/composite.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/graphdef/protobuf.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/graphdef/protobuf.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/graphdef/reader.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/graphdef/reader.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/graphdef/utils.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/graphdef/utils.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/graphdef/writer.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/graphdef/writer.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/__init__.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/__init__.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/AbsOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/AbsOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/AddNOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/AddNOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/AddOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/AddOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/ArgMaxOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/ArgMaxOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/ArgMinOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/ArgMinOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/BatchMatMulOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/BatchMatMulOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/BatchToSpaceNDOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/BatchToSpaceNDOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/BidirectionalSequenceLSTMOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/BidirectionalSequenceLSTMOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/BidirectionalSequenceRNNOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/BidirectionalSequenceRNNOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/Buffer.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/Buffer.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/BuiltinOperator.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/BuiltinOperator.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/BuiltinOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/BuiltinOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/CallOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/CallOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/CastOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/CastOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/ConcatEmbeddingsOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/ConcatEmbeddingsOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/ConcatenationOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/ConcatenationOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/Conv2DOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/Conv2DOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/CosOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/CosOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/CustomQuantization.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/CustomQuantization.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/DensifyOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/DensifyOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/DepthToSpaceOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/DepthToSpaceOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/DepthwiseConv2DOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/DepthwiseConv2DOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/DequantizeOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/DequantizeOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/DimensionMetadata.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/DimensionMetadata.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/DivOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/DivOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/EmbeddingLookupSparseOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/EmbeddingLookupSparseOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/EqualOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/EqualOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/ExpOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/ExpOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/ExpandDimsOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/ExpandDimsOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/FakeQuantOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/FakeQuantOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/FillOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/FillOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/FloorDivOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/FloorDivOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/FloorModOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/FloorModOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/FullyConnectedOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/FullyConnectedOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/GatherNdOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/GatherNdOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/GatherOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/GatherOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/GreaterEqualOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/GreaterEqualOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/GreaterOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/GreaterOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/HardSwishOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/HardSwishOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/IfOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/IfOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/Int32Vector.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/Int32Vector.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/L2NormOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/L2NormOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/LSHProjectionOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/LSHProjectionOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/LSTMOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/LSTMOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/LeakyReluOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/LeakyReluOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/LessEqualOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/LessEqualOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/LessOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/LessOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/LocalResponseNormalizationOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/LocalResponseNormalizationOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/LogSoftmaxOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/LogSoftmaxOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/LogicalAndOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/LogicalAndOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/LogicalNotOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/LogicalNotOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/LogicalOrOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/LogicalOrOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/MatrixDiagOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/MatrixDiagOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/MatrixSetDiagOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/MatrixSetDiagOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/MaximumMinimumOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/MaximumMinimumOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/Metadata.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/Metadata.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/MirrorPadOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/MirrorPadOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/Model.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/Model.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/MulOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/MulOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/NegOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/NegOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/NonMaxSuppressionV4Options.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/NonMaxSuppressionV4Options.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/NonMaxSuppressionV5Options.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/NonMaxSuppressionV5Options.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/NotEqualOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/NotEqualOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/OneHotOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/OneHotOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/Operator.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/Operator.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/OperatorCode.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/OperatorCode.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/PackOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/PackOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/PadOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/PadOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/PadV2Options.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/PadV2Options.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/Pool2DOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/Pool2DOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/PowOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/PowOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/QuantizationParameters.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/QuantizationParameters.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/QuantizeOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/QuantizeOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/RNNOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/RNNOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/RangeOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/RangeOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/RankOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/RankOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/ReducerOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/ReducerOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/ReshapeOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/ReshapeOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/ResizeBilinearOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/ResizeBilinearOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/ResizeNearestNeighborOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/ResizeNearestNeighborOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/ReverseSequenceOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/ReverseSequenceOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/ReverseV2Options.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/ReverseV2Options.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SVDFOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SVDFOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/ScatterNdOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/ScatterNdOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SegmentSumOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SegmentSumOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SelectOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SelectOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SelectV2Options.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SelectV2Options.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SequenceRNNOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SequenceRNNOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/ShapeOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/ShapeOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SkipGramOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SkipGramOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SliceOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SliceOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SoftmaxOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SoftmaxOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SpaceToBatchNDOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SpaceToBatchNDOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SpaceToDepthOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SpaceToDepthOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SparseToDenseOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SparseToDenseOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SparsityParameters.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SparsityParameters.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SplitOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SplitOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SplitVOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SplitVOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SquareOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SquareOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SquaredDifferenceOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SquaredDifferenceOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SqueezeOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SqueezeOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/StridedSliceOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/StridedSliceOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SubGraph.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SubGraph.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/SubOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/SubOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/Tensor.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/Tensor.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/TileOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/TileOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/TopKV2Options.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/TopKV2Options.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/TransposeConvOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/TransposeConvOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/TransposeOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/TransposeOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/Uint16Vector.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/Uint16Vector.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/Uint8Vector.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/Uint8Vector.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/UnidirectionalSequenceLSTMOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/UnidirectionalSequenceLSTMOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/UniqueOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/UniqueOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/UnpackOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/UnpackOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/WhereOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/WhereOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/WhileOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/WhileOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/ZerosLikeOptions.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/ZerosLikeOptions.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/flatbuffers/__init__.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/flatbuffers/__init__.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/helpers.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/helpers.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/reader.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/reader.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/io/tf/lite/writer.py` & `nnef_tools-1.0.5/nnef_tools/io/tf/lite/writer.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/model/__init__.py` & `nnef_tools-1.0.5/nnef_tools/model/__init__.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/model/graph.py` & `nnef_tools-1.0.5/nnef_tools/model/graph.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/model/utils.py` & `nnef_tools-1.0.5/nnef_tools/model/utils.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/optimization/__init__.py` & `nnef_tools-1.0.5/nnef_tools/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/optimization/nnef_optimizer.py` & `nnef_tools-1.0.5/nnef_tools/optimization/nnef_optimizer.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/optimization/onnx_optimizer.py` & `nnef_tools-1.0.5/nnef_tools/optimization/onnx_optimizer.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/optimization/tf_optimizer.py` & `nnef_tools-1.0.5/nnef_tools/optimization/tf_optimizer.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/optimization/tflite_optimizer.py` & `nnef_tools-1.0.5/nnef_tools/optimization/tflite_optimizer.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/quantize.py` & `nnef_tools-1.0.5/nnef_tools/quantize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from src.nnef_tools.io.nnef.reader import Reader
-from src.nnef_tools.io.nnef.writer import Writer
+from nnef_tools.io.nnef.reader import Reader
+from nnef_tools.io.nnef.writer import Writer
 import numpy as np
 import argparse
 import json
 import os
 
 
 _CONV_OPS = ['conv', 'deconv', 'separable_conv', 'separable_deconv']
```

### Comparing `nnef_tools-1.0.4/nnef_tools/random_tensor.py` & `nnef_tools-1.0.5/nnef_tools/random_tensor.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/utils/__init__.py` & `nnef_tools-1.0.5/nnef_tools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/utils/stdio.py` & `nnef_tools-1.0.5/nnef_tools/utils/stdio.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/utils/types.py` & `nnef_tools-1.0.5/nnef_tools/utils/types.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools/visualize.py` & `nnef_tools-1.0.5/nnef_tools/visualize.py`

 * *Files identical despite different names*

### Comparing `nnef_tools-1.0.4/nnef_tools.egg-info/PKG-INFO` & `nnef_tools-1.0.5/nnef_tools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nnef_tools
-Version: 1.0.4
+Version: 1.0.5
 Summary: A package for managing NNEF files
 Author-email: Viktor Gyenes <viktor.gyenes@aimotive.com>, Tamas Danyluk <9149812+tdanyluk@users.noreply.github.com>
 Maintainer-email: Viktor Gyenes <viktor.gyenes@aimotive.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -239,34 +239,14 @@
 Provides-Extra: full
 Requires-Dist: nnef_tools[caffe,onnx,tensorflow-lite,visualization]; extra == "full"
 
 # NNEF Tools
 
 This package contains a set of tools for converting and transforming machine learning models.
 
-## Dependencies
-
-You need to install dependencies only for the functionalities that you are using:
-
-| Functionality                  | Dependencies                                                                 |
-| ------------------------------ | ---------------------------------------------------------------------------- |
-| TensorFlow Protobuf conversion | pip install future typing six numpy tensorflow                               |
-| TensorFlow Lite conversion     | pip install future typing six numpy flatbuffers, tensorflow                  |
-| ONNX conversion                | pip install future typing six numpy protobuf onnx onnx-simplifier onnxruntime |
-| Caffe conversion               | pip install future typing six numpy protobuf torch                           |
-| Caffe2 conversion              | pip install future typing six numpy protobuf torch                           |
-| Execution of NNEF models       | pip install future typing six numpy torch                                    |
-| Visualization of NNEF models   | pip install future typing six numpy graphviz                                 |
-
-
-All pip dependencies (for reference):
-```
-pip install future typing six numpy protobuf flatbuffers onnx onnx-simplifier onnxruntime torch tensorflow
-```
-
 ## Usage
 
 For basic usage, you have to supply an input format, an output format and an input model. The output model name defaults to the input model name suffixed with the output format, but it can also be supplied explicitly.
 
 ```
 python -m nnef_tools.convert --input-format tf --output-format nnef --input-model my_model.pb --output-model my_model.nnef
 ```
```

### Comparing `nnef_tools-1.0.4/nnef_tools.egg-info/SOURCES.txt` & `nnef_tools-1.0.5/nnef_tools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+package_info.md
 pyproject.toml
 nnef_tools/__init__.py
 nnef_tools/convert.py
 nnef_tools/execute.py
 nnef_tools/generate.py
 nnef_tools/gmac.py
 nnef_tools/image_tensor.py
```

### Comparing `nnef_tools-1.0.4/pyproject.toml` & `nnef_tools-1.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nnef_tools"
-version = "1.0.4"
+version = "1.0.5"
 description = "A package for managing NNEF files"
 requires-python = ">=3.7"
 
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
     'Programming Language :: Python :: 3',
@@ -34,11 +34,11 @@
 full = ["nnef_tools[tensorflow-lite,onnx,caffe,visualization]"]
 
 [project.urls]
 "Homepage" = "https://www.khronos.org/nnef"
 "Repository" = "https://github.com/KhronosGroup/NNEF-Tools"
 
 [tool.setuptools.dynamic]
-readme = { file = ["README.md"], content-type = "text/markdown" }
+readme = { file = ["package_info.md"], content-type = "text/markdown" }
 
 [tool.setuptools]
 package-dir = {"nnef_tools" = "nnef_tools"}
```

